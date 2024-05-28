# Comparing `tmp/KratosMPMApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/KratosMPMApplication-9.5.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,1491 +1,1061 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   3855905 (00000000003AD621h)
-  Actual end-cent-dir record offset:       3855883 (00000000003AD60Bh)
-  Expected end-cent-dir record offset:     3855883 (00000000003AD60Bh)
+  Zip archive file size:                   1585632 (00000000001831E0h)
+  Actual end-cent-dir record offset:       1585610 (00000000001831CAh)
+  Expected end-cent-dir record offset:     1585610 (00000000001831CAh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 40 entries.
-  The central directory is 5198 (000000000000144Eh) bytes long,
+  central directory contains 36 entries.
+  The central directory is 3926 (0000000000000F56h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 3850685 (00000000003AC1BDh).
+  is 1581684 (0000000000182274h).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosMPMApplication-9.5.dist-info/
+  KratosMultiphysics/.libs/KratosMPMApplication.pyd
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:46
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             35 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:38
+  32-bit CRC value (hex):                         802844b2
+  compressed size:                                583580 bytes
+  uncompressed size:                              1924096 bytes
+  length of filename:                             49 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+  non-MSDOS external file attributes:             81B600 hex
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  KratosMPMApplication-9.5.dist-info/METADATA
+  KratosMultiphysics/.libs/KratosMPMCore.dll
 
-  offset of local header from start of archive:   93
-                                                  (000000000000005Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   583659
+                                                  (000000000008E7EBh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         eeea6fea
-  compressed size:                                3702 bytes
-  uncompressed size:                              9084 bytes
-  length of filename:                             43 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:38
+  32-bit CRC value (hex):                         8d2b534c
+  compressed size:                                900945 bytes
+  uncompressed size:                              2701824 bytes
+  length of filename:                             42 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  KratosMPMApplication-9.5.dist-info/WHEEL
+  KratosMultiphysics/.libs/KratosMPMCore.lib
 
-  offset of local header from start of archive:   3896
-                                                  (0000000000000F38h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1484676
+                                                  (000000000016A784h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         90d34e0d
-  compressed size:                                116 bytes
-  uncompressed size:                              148 bytes
-  length of filename:                             40 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:38
+  32-bit CRC value (hex):                         44b6fbed
+  compressed size:                                50302 bytes
+  uncompressed size:                              528356 bytes
+  length of filename:                             42 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  KratosMPMApplication-9.5.dist-info/top_level.txt
+  KratosMultiphysics/MPMApplication/__init__.py
 
-  offset of local header from start of archive:   4110
-                                                  (000000000000100Eh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1535050
+                                                  (0000000000176C4Ah) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         f32d789f
-  compressed size:                                19 bytes
-  uncompressed size:                              19 bytes
-  length of filename:                             48 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         67b552b7
+  compressed size:                                99 bytes
+  uncompressed size:                              221 bytes
+  length of filename:                             45 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  KratosMPMApplication-9.5.dist-info/RECORD
+  KratosMultiphysics/MPMApplication/apply_mpm_3d_rotating_dirichlet_condition_process.py
 
-  offset of local header from start of archive:   4235
-                                                  (000000000000108Bh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1535224
+                                                  (0000000000176CF8h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:46
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 UTC
-  32-bit CRC value (hex):                         a4f7c764
-  compressed size:                                1859 bytes
-  uncompressed size:                              4336 bytes
-  length of filename:                             41 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         1b5a11df
+  compressed size:                                1749 bytes
+  uncompressed size:                              6863 bytes
+  length of filename:                             86 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #6:
 ---------------------------
 
-  KratosMPMApplication.libs/
+  KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_dirichlet_condition_process.py
 
-  offset of local header from start of archive:   6193
-                                                  (0000000000001831h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1537089
+                                                  (0000000000177441h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:46
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             26 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         5c1acd48
+  compressed size:                                1752 bytes
+  uncompressed size:                              6700 bytes
+  length of filename:                             93 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+  non-MSDOS external file attributes:             81B600 hex
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #7:
 ---------------------------
 
-  KratosMPMApplication.libs/libKratosMPMCore-b22ee70f.so
+  KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_neumann_condition_process.py
 
-  offset of local header from start of archive:   6277
-                                                  (0000000000001885h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1538964
+                                                  (0000000000177B94h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         a10a1a20
-  compressed size:                                2441136 bytes
-  uncompressed size:                              9310457 bytes
-  length of filename:                             54 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         c15e2e67
+  compressed size:                                1493 bytes
+  uncompressed size:                              5408 bytes
+  length of filename:                             91 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100755 octal):            -rwxr-xr-x
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #8:
 ---------------------------
 
-  KratosMultiphysics/
+  KratosMultiphysics/MPMApplication/apply_mpm_particle_dirichlet_condition_process.py
 
-  offset of local header from start of archive:   2447525
-                                                  (00000000002558A5h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1540578
+                                                  (00000000001781E2h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             19 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         84d82973
+  compressed size:                                2564 bytes
+  uncompressed size:                              9320 bytes
+  length of filename:                             83 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+  non-MSDOS external file attributes:             81B600 hex
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #9:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/
+  KratosMultiphysics/MPMApplication/apply_mpm_particle_neumann_condition_process.py
 
-  offset of local header from start of archive:   2447602
-                                                  (00000000002558F2h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1543255
+                                                  (0000000000178C57h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             34 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         3a312f80
+  compressed size:                                2266 bytes
+  uncompressed size:                              8773 bytes
+  length of filename:                             81 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
+  non-MSDOS external file attributes:             81B600 hex
+  MS-DOS file attributes (00 hex):                none
 
   There is no file comment.
 
 Central directory entry #10:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/particle_mechanics_analysis.py
+  KratosMultiphysics/MPMApplication/apply_mpm_slip_boundary_process.py
 
-  offset of local header from start of archive:   2447694
-                                                  (000000000025594Eh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1545632
+                                                  (00000000001795A0h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         a2c7b02c
-  compressed size:                                544 bytes
-  uncompressed size:                              1461 bytes
-  length of filename:                             64 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         ad4c3641
+  compressed size:                                752 bytes
+  uncompressed size:                              1947 bytes
+  length of filename:                             68 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #11:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_vtk_output_process.py
+  KratosMultiphysics/MPMApplication/assign_gravity_to_material_point_process.py
 
-  offset of local header from start of archive:   2448360
-                                                  (0000000000255BE8h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1546482
+                                                  (00000000001798F2h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         80c5626e
-  compressed size:                                1274 bytes
-  uncompressed size:                              5070 bytes
-  length of filename:                             59 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         aa0d9815
+  compressed size:                                991 bytes
+  uncompressed size:                              2930 bytes
+  length of filename:                             77 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #12:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_json_output_process.py
+  KratosMultiphysics/MPMApplication/assign_gravity_to_particle_process.py
 
-  offset of local header from start of archive:   2449751
-                                                  (0000000000256157h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1547580
+                                                  (0000000000179D3Ch) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         7b618080
-  compressed size:                                1325 bytes
-  uncompressed size:                              8063 bytes
-  length of filename:                             60 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         56ac293c
+  compressed size:                                346 bytes
+  uncompressed size:                              826 bytes
+  length of filename:                             71 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #13:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/particle_vtk_output_process.py
+  KratosMultiphysics/MPMApplication/assign_initial_velocity_to_material_point_process.py
 
-  offset of local header from start of archive:   2451194
-                                                  (00000000002566FAh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1548027
+                                                  (0000000000179EFBh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         4bc4adfe
-  compressed size:                                325 bytes
-  uncompressed size:                              818 bytes
-  length of filename:                             64 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         02224e9f
+  compressed size:                                1201 bytes
+  uncompressed size:                              3471 bytes
+  length of filename:                             86 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #14:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/assign_gravity_to_material_point_process.py
+  KratosMultiphysics/MPMApplication/assign_initial_velocity_to_particle_process.py
 
-  offset of local header from start of archive:   2451641
-                                                  (00000000002568B9h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1549344
+                                                  (000000000017A420h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         278b18db
-  compressed size:                                982 bytes
-  uncompressed size:                              2876 bytes
-  length of filename:                             77 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         b2e3cdbd
+  compressed size:                                355 bytes
+  uncompressed size:                              869 bytes
+  length of filename:                             80 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #15:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/apply_mpm_slip_boundary_process.py
+  KratosMultiphysics/MPMApplication/kratos_main_mpm.py
 
-  offset of local header from start of archive:   2452758
-                                                  (0000000000256D16h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1549809
+                                                  (000000000017A5F1h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         74b80942
-  compressed size:                                745 bytes
-  uncompressed size:                              1907 bytes
-  length of filename:                             68 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         fe0a71c1
+  compressed size:                                260 bytes
+  uncompressed size:                              497 bytes
+  length of filename:                             52 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #16:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/apply_mpm_particle_dirichlet_condition_process.py
+  KratosMultiphysics/MPMApplication/mpm_analysis.py
 
-  offset of local header from start of archive:   2453629
-                                                  (000000000025707Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1550151
+                                                  (000000000017A747h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         2c6449ca
-  compressed size:                                2549 bytes
-  uncompressed size:                              9141 bytes
-  length of filename:                             83 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         3912048a
+  compressed size:                                1791 bytes
+  uncompressed size:                              6640 bytes
+  length of filename:                             49 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #17:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_solver.py
+  KratosMultiphysics/MPMApplication/mpm_explicit_solver.py
 
-  offset of local header from start of archive:   2456319
-                                                  (0000000000257AFFh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1552021
+                                                  (000000000017AE95h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         33c3a5db
-  compressed size:                                5427 bytes
-  uncompressed size:                              27296 bytes
-  length of filename:                             47 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         5022cbf2
+  compressed size:                                1688 bytes
+  uncompressed size:                              6430 bytes
+  length of filename:                             56 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #18:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/apply_mpm_3d_rotating_dirichlet_condition_process.py
+  KratosMultiphysics/MPMApplication/mpm_from_json_check_result_process.py
 
-  offset of local header from start of archive:   2461851
-                                                  (000000000025909Bh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1553795
+                                                  (000000000017B583h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         9fa63198
-  compressed size:                                1734 bytes
-  uncompressed size:                              6722 bytes
-  length of filename:                             86 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         8bc3bb9d
+  compressed size:                                3698 bytes
+  uncompressed size:                              21391 bytes
+  length of filename:                             71 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #19:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_dirichlet_condition_process.py
+  KratosMultiphysics/MPMApplication/mpm_gid_output_process.py
 
-  offset of local header from start of archive:   2463729
-                                                  (00000000002597F1h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1557594
+                                                  (000000000017C45Ah) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         857fe2e3
-  compressed size:                                1743 bytes
-  uncompressed size:                              6582 bytes
-  length of filename:                             93 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         ece183aa
+  compressed size:                                2946 bytes
+  uncompressed size:                              11513 bytes
+  length of filename:                             59 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #20:
 ---------------------------
 
   KratosMultiphysics/MPMApplication/mpm_implicit_dynamic_solver.py
 
-  offset of local header from start of archive:   2465623
-                                                  (0000000000259F57h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1560629
+                                                  (000000000017D035h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         4c7dfd95
-  compressed size:                                936 bytes
-  uncompressed size:                              2970 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         f9b5b227
+  compressed size:                                948 bytes
+  uncompressed size:                              3040 bytes
   length of filename:                             64 characters
-  length of extra field:                          24 bytes
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #21:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/kratos_main_mpm.py
+  KratosMultiphysics/MPMApplication/mpm_json_output_process.py
 
-  offset of local header from start of archive:   2466681
-                                                  (000000000025A379h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1561671
+                                                  (000000000017D447h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         b263765b
-  compressed size:                                254 bytes
-  uncompressed size:                              480 bytes
-  length of filename:                             52 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         7ed2eebd
+  compressed size:                                1335 bytes
+  uncompressed size:                              8221 bytes
+  length of filename:                             60 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #22:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/particle_json_output_process.py
+  KratosMultiphysics/MPMApplication/mpm_quasi_static_solver.py
 
-  offset of local header from start of archive:   2467045
-                                                  (000000000025A4E5h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1563096
+                                                  (000000000017D9D8h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         04f9c95b
-  compressed size:                                321 bytes
-  uncompressed size:                              728 bytes
-  length of filename:                             65 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         92a86f7a
+  compressed size:                                339 bytes
+  uncompressed size:                              778 bytes
+  length of filename:                             60 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #23:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_explicit_solver.py
+  KratosMultiphysics/MPMApplication/mpm_solver.py
 
-  offset of local header from start of archive:   2467489
-                                                  (000000000025A6A1h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1563525
+                                                  (000000000017DB85h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         9a5c0ee6
-  compressed size:                                1677 bytes
-  uncompressed size:                              6302 bytes
-  length of filename:                             56 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         ce9f1fe7
+  compressed size:                                5446 bytes
+  uncompressed size:                              27814 bytes
+  length of filename:                             47 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #24:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/apply_mpm_particle_neumann_condition_process.py
+  KratosMultiphysics/MPMApplication/mpm_static_solver.py
 
-  offset of local header from start of archive:   2469280
-                                                  (000000000025ADA0h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1569048
+                                                  (000000000017F118h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         ef93060a
-  compressed size:                                2257 bytes
-  uncompressed size:                              8604 bytes
-  length of filename:                             81 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         e6339ae5
+  compressed size:                                325 bytes
+  uncompressed size:                              741 bytes
+  length of filename:                             54 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #25:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/python_solvers_wrapper_mpm.py
+  KratosMultiphysics/MPMApplication/mpm_vtk_condition_output_process.py
 
-  offset of local header from start of archive:   2471676
-                                                  (000000000025B6FCh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1569457
+                                                  (000000000017F2B1h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         f7097746
-  compressed size:                                728 bytes
-  uncompressed size:                              2578 bytes
-  length of filename:                             63 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         897613c4
+  compressed size:                                1529 bytes
+  uncompressed size:                              5415 bytes
+  length of filename:                             69 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #26:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/assign_gravity_to_particle_process.py
+  KratosMultiphysics/MPMApplication/mpm_vtk_output_process.py
 
-  offset of local header from start of archive:   2472525
-                                                  (000000000025BA4Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1571085
+                                                  (000000000017F90Dh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         2f1dabec
-  compressed size:                                342 bytes
-  uncompressed size:                              813 bytes
-  length of filename:                             71 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         3d0111fc
+  compressed size:                                1284 bytes
+  uncompressed size:                              5161 bytes
+  length of filename:                             59 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #27:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_analysis.py
+  KratosMultiphysics/MPMApplication/particle_from_json_check_result_process.py
 
-  offset of local header from start of archive:   2472996
-                                                  (000000000025BC24h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1572458
+                                                  (000000000017FE6Ah) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         69edafd3
-  compressed size:                                1779 bytes
-  uncompressed size:                              6525 bytes
-  length of filename:                             49 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         aa638ef2
+  compressed size:                                336 bytes
+  uncompressed size:                              786 bytes
+  length of filename:                             76 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #28:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/assign_initial_velocity_to_particle_process.py
+  KratosMultiphysics/MPMApplication/particle_gid_output_process.py
 
-  offset of local header from start of archive:   2474882
-                                                  (000000000025C382h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1572900
+                                                  (0000000000180024h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         1d901f57
-  compressed size:                                346 bytes
-  uncompressed size:                              856 bytes
-  length of filename:                             80 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         b2201741
+  compressed size:                                388 bytes
+  uncompressed size:                              980 bytes
+  length of filename:                             64 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #29:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_gid_output_process.py
+  KratosMultiphysics/MPMApplication/particle_json_output_process.py
 
-  offset of local header from start of archive:   2475366
-                                                  (000000000025C566h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1573382
+                                                  (0000000000180206h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         ffbef12c
-  compressed size:                                2920 bytes
-  uncompressed size:                              11253 bytes
-  length of filename:                             59 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         4c88e91a
+  compressed size:                                326 bytes
+  uncompressed size:                              740 bytes
+  length of filename:                             65 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #30:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_quasi_static_solver.py
+  KratosMultiphysics/MPMApplication/particle_mechanics_analysis.py
 
-  offset of local header from start of archive:   2478403
-                                                  (000000000025D143h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1573803
+                                                  (00000000001803ABh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         7f7069cc
-  compressed size:                                332 bytes
-  uncompressed size:                              756 bytes
-  length of filename:                             60 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         04413d92
+  compressed size:                                550 bytes
+  uncompressed size:                              1494 bytes
+  length of filename:                             64 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #31:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_static_solver.py
+  KratosMultiphysics/MPMApplication/particle_vtk_output_process.py
 
-  offset of local header from start of archive:   2478853
-                                                  (000000000025D305h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1574447
+                                                  (000000000018062Fh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         5ece0b3c
-  compressed size:                                317 bytes
-  uncompressed size:                              723 bytes
-  length of filename:                             54 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         db0c052b
+  compressed size:                                330 bytes
+  uncompressed size:                              829 bytes
+  length of filename:                             64 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #32:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_neumann_condition_process.py
+  KratosMultiphysics/MPMApplication/python_solvers_wrapper_mpm.py
 
-  offset of local header from start of archive:   2479282
-                                                  (000000000025D4B2h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1574871
+                                                  (00000000001807D7h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         6a3be701
-  compressed size:                                1478 bytes
-  uncompressed size:                              5307 bytes
-  length of filename:                             91 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         7cf2a9a6
+  compressed size:                                738 bytes
+  uncompressed size:                              2633 bytes
+  length of filename:                             63 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #33:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/assign_initial_velocity_to_material_point_process.py
+  KratosMPMApplication-9.5.1.dist-info/METADATA
 
-  offset of local header from start of archive:   2480909
-                                                  (000000000025DB0Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1575702
+                                                  (0000000000180B16h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         a68f58d4
-  compressed size:                                1190 bytes
-  uncompressed size:                              3406 bytes
-  length of filename:                             86 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:38
+  32-bit CRC value (hex):                         c4141e4d
+  compressed size:                                3732 bytes
+  uncompressed size:                              9278 bytes
+  length of filename:                             45 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #34:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/particle_from_json_check_result_process.py
+  KratosMPMApplication-9.5.1.dist-info/WHEEL
 
-  offset of local header from start of archive:   2482243
-                                                  (000000000025E043h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1579509
+                                                  (00000000001819F5h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         a14be6ef
-  compressed size:                                329 bytes
-  uncompressed size:                              774 bytes
-  length of filename:                             76 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:38
+  32-bit CRC value (hex):                         86fb6b41
+  compressed size:                                96 bytes
+  uncompressed size:                              100 bytes
+  length of filename:                             42 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #35:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/particle_gid_output_process.py
+  KratosMPMApplication-9.5.1.dist-info/top_level.txt
 
-  offset of local header from start of archive:   2482706
-                                                  (000000000025E212h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1579677
+                                                  (0000000000181A9Dh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         3473a6ed
-  compressed size:                                383 bytes
-  uncompressed size:                              965 bytes
-  length of filename:                             64 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:38
+  32-bit CRC value (hex):                         f32d789f
+  compressed size:                                21 bytes
+  uncompressed size:                              19 bytes
+  length of filename:                             50 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             81B600 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
 
 Central directory entry #36:
 ---------------------------
 
-  KratosMultiphysics/MPMApplication/mpm_from_json_check_result_process.py
-
-  offset of local header from start of archive:   2483211
-                                                  (000000000025E40Bh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         3c6062c6
-  compressed size:                                3670 bytes
-  uncompressed size:                              20995 bytes
-  length of filename:                             71 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #37:
----------------------------
-
-  KratosMultiphysics/MPMApplication/__init__.py
-
-  offset of local header from start of archive:   2487010
-                                                  (000000000025F2E2h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         0fa98a56
-  compressed size:                                95 bytes
-  uncompressed size:                              215 bytes
-  length of filename:                             45 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #38:
----------------------------
-
-  KratosMultiphysics/MPMApplication/mpm_vtk_condition_output_process.py
-
-  offset of local header from start of archive:   2487208
-                                                  (000000000025F3A8h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         544cdc64
-  compressed size:                                1516 bytes
-  uncompressed size:                              5301 bytes
-  length of filename:                             69 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             text
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #39:
----------------------------
+  KratosMPMApplication-9.5.1.dist-info/RECORD
 
-  KratosMultiphysics/.libs/
-
-  offset of local header from start of archive:   2488851
-                                                  (000000000025FA13h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:46
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:46 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             25 characters
-  length of extra field:                          24 bytes
-  length of file comment:                         0 characters
-  disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (040755 octal):            drwxr-xr-x
-  MS-DOS file attributes (10 hex):                dir 
-
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
-  There is no file comment.
-
-Central directory entry #40:
----------------------------
-
-  KratosMultiphysics/.libs/KratosMPMApplication.cpython-39-x86_64-linux-gnu.so
-
-  offset of local header from start of archive:   2488934
-                                                  (000000000025FA66h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   1579778
+                                                  (0000000000181B02h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 16:00:40
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 16:00:40 UTC
-  32-bit CRC value (hex):                         f802c35d
-  compressed size:                                1361617 bytes
-  uncompressed size:                              3737889 bytes
-  length of filename:                             76 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:38
+  32-bit CRC value (hex):                         b7ce4287
+  compressed size:                                1833 bytes
+  uncompressed size:                              4266 bytes
+  length of filename:                             43 characters
+  length of extra field:                          0 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100755 octal):            -rwxr-xr-x
+  non-MSDOS external file attributes:             81B400 hex
   MS-DOS file attributes (00 hex):                none
 
-  The central-directory extra field contains:
-  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
-    The local extra field has UTC/GMT modification/access times.
-  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
-    01 04 00 00 00 00 04 00 00 00 00.
-
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,121 +1,109 @@
-Filename: KratosMPMApplication-9.5.dist-info/
+Filename: KratosMultiphysics/.libs/KratosMPMApplication.pyd
 Comment: 
 
-Filename: KratosMPMApplication-9.5.dist-info/METADATA
+Filename: KratosMultiphysics/.libs/KratosMPMCore.dll
 Comment: 
 
-Filename: KratosMPMApplication-9.5.dist-info/WHEEL
+Filename: KratosMultiphysics/.libs/KratosMPMCore.lib
 Comment: 
 
-Filename: KratosMPMApplication-9.5.dist-info/top_level.txt
-Comment: 
-
-Filename: KratosMPMApplication-9.5.dist-info/RECORD
-Comment: 
-
-Filename: KratosMPMApplication.libs/
-Comment: 
-
-Filename: KratosMPMApplication.libs/libKratosMPMCore-b22ee70f.so
+Filename: KratosMultiphysics/MPMApplication/__init__.py
 Comment: 
 
-Filename: KratosMultiphysics/
+Filename: KratosMultiphysics/MPMApplication/apply_mpm_3d_rotating_dirichlet_condition_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/
+Filename: KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_dirichlet_condition_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/particle_mechanics_analysis.py
+Filename: KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_neumann_condition_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_vtk_output_process.py
+Filename: KratosMultiphysics/MPMApplication/apply_mpm_particle_dirichlet_condition_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_json_output_process.py
+Filename: KratosMultiphysics/MPMApplication/apply_mpm_particle_neumann_condition_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/particle_vtk_output_process.py
+Filename: KratosMultiphysics/MPMApplication/apply_mpm_slip_boundary_process.py
 Comment: 
 
 Filename: KratosMultiphysics/MPMApplication/assign_gravity_to_material_point_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/apply_mpm_slip_boundary_process.py
-Comment: 
-
-Filename: KratosMultiphysics/MPMApplication/apply_mpm_particle_dirichlet_condition_process.py
+Filename: KratosMultiphysics/MPMApplication/assign_gravity_to_particle_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_solver.py
+Filename: KratosMultiphysics/MPMApplication/assign_initial_velocity_to_material_point_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/apply_mpm_3d_rotating_dirichlet_condition_process.py
+Filename: KratosMultiphysics/MPMApplication/assign_initial_velocity_to_particle_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_dirichlet_condition_process.py
+Filename: KratosMultiphysics/MPMApplication/kratos_main_mpm.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_implicit_dynamic_solver.py
+Filename: KratosMultiphysics/MPMApplication/mpm_analysis.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/kratos_main_mpm.py
+Filename: KratosMultiphysics/MPMApplication/mpm_explicit_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/particle_json_output_process.py
+Filename: KratosMultiphysics/MPMApplication/mpm_from_json_check_result_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_explicit_solver.py
+Filename: KratosMultiphysics/MPMApplication/mpm_gid_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/apply_mpm_particle_neumann_condition_process.py
+Filename: KratosMultiphysics/MPMApplication/mpm_implicit_dynamic_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/python_solvers_wrapper_mpm.py
+Filename: KratosMultiphysics/MPMApplication/mpm_json_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/assign_gravity_to_particle_process.py
+Filename: KratosMultiphysics/MPMApplication/mpm_quasi_static_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_analysis.py
+Filename: KratosMultiphysics/MPMApplication/mpm_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/assign_initial_velocity_to_particle_process.py
+Filename: KratosMultiphysics/MPMApplication/mpm_static_solver.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_gid_output_process.py
+Filename: KratosMultiphysics/MPMApplication/mpm_vtk_condition_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_quasi_static_solver.py
+Filename: KratosMultiphysics/MPMApplication/mpm_vtk_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_static_solver.py
+Filename: KratosMultiphysics/MPMApplication/particle_from_json_check_result_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_neumann_condition_process.py
+Filename: KratosMultiphysics/MPMApplication/particle_gid_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/assign_initial_velocity_to_material_point_process.py
+Filename: KratosMultiphysics/MPMApplication/particle_json_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/particle_from_json_check_result_process.py
+Filename: KratosMultiphysics/MPMApplication/particle_mechanics_analysis.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/particle_gid_output_process.py
+Filename: KratosMultiphysics/MPMApplication/particle_vtk_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_from_json_check_result_process.py
+Filename: KratosMultiphysics/MPMApplication/python_solvers_wrapper_mpm.py
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/__init__.py
+Filename: KratosMPMApplication-9.5.1.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/MPMApplication/mpm_vtk_condition_output_process.py
+Filename: KratosMPMApplication-9.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/.libs/
+Filename: KratosMPMApplication-9.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosMPMApplication.cpython-39-x86_64-linux-gnu.so
+Filename: KratosMPMApplication-9.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## KratosMultiphysics/MPMApplication/particle_mechanics_analysis.py

 * *Ordering differences only*

```diff
@@ -1,33 +1,33 @@
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-from KratosMultiphysics.MPMApplication.mpm_analysis import MPMAnalysis
-
-class ParticleMechanicsAnalysis(MPMAnalysis):
-
-    def __init__(self, model, project_parameters):
-        IssueDeprecationWarning("MPMApplication:","`ParticleMechanicsAnalysis` is deprecated and replaced with `MPMAnalysis`")
-        super().__init__(model, project_parameters)
-
-if __name__ == "__main__":
-    from sys import argv
-
-    if len(argv) > 2:
-        err_msg =  'Too many input arguments!\n'
-        err_msg += 'Use this script in the following way:\n'
-        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
-        err_msg += '    "python3 particle_mechanics_analysis.py"\n'
-        err_msg += '- With custom ProjectParameters:\n'
-        err_msg += '    "python3 particle_mechanics_analysis.py CustomProjectParameters.json"\n'
-        raise Exception(err_msg)
-
-    if len(argv) == 2: # ProjectParameters is being passed from outside
-        project_parameters_file_name = argv[1]
-    else: # using default name
-        project_parameters_file_name = "ProjectParameters.json"
-
-    with open(project_parameters_file_name,'r') as parameter_file:
-        parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-    model = KratosMultiphysics.Model()
-    simulation = ParticleMechanicsAnalysis(model, parameters)
-    simulation.Run()
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+from KratosMultiphysics.MPMApplication.mpm_analysis import MPMAnalysis
+
+class ParticleMechanicsAnalysis(MPMAnalysis):
+
+    def __init__(self, model, project_parameters):
+        IssueDeprecationWarning("MPMApplication:","`ParticleMechanicsAnalysis` is deprecated and replaced with `MPMAnalysis`")
+        super().__init__(model, project_parameters)
+
+if __name__ == "__main__":
+    from sys import argv
+
+    if len(argv) > 2:
+        err_msg =  'Too many input arguments!\n'
+        err_msg += 'Use this script in the following way:\n'
+        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
+        err_msg += '    "python3 particle_mechanics_analysis.py"\n'
+        err_msg += '- With custom ProjectParameters:\n'
+        err_msg += '    "python3 particle_mechanics_analysis.py CustomProjectParameters.json"\n'
+        raise Exception(err_msg)
+
+    if len(argv) == 2: # ProjectParameters is being passed from outside
+        project_parameters_file_name = argv[1]
+    else: # using default name
+        project_parameters_file_name = "ProjectParameters.json"
+
+    with open(project_parameters_file_name,'r') as parameter_file:
+        parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+    model = KratosMultiphysics.Model()
+    simulation = ParticleMechanicsAnalysis(model, parameters)
+    simulation.Run()
```

## KratosMultiphysics/MPMApplication/mpm_vtk_output_process.py

 * *Ordering differences only*

```diff
@@ -1,91 +1,91 @@
-import KratosMultiphysics
-import KratosMultiphysics.kratos_utilities as kratos_utils
-from  KratosMultiphysics.deprecation_management import DeprecationManager
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-def Factory(settings: KratosMultiphysics.Parameters, model: KratosMultiphysics.Model) -> KratosMultiphysics.OutputProcess:
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a Model object, encapsulating a json string")
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return MPMVtkOutputProcess(model, settings["Parameters"])
-
-class MPMVtkOutputProcess(KratosMultiphysics.OutputProcess):
-
-    def __init__(self, model: KratosMultiphysics.Model, settings: KratosMultiphysics.Parameters) -> None:
-        super().__init__()
-
-        self.model = model
-        self.settings = settings
-
-        self.full_model_part_name = self.settings["model_part_name"].GetString()
-        if self.full_model_part_name.startswith('Background_Grid'):
-            self.full_model_part_name = self.full_model_part_name.replace('Background_Grid','MPM_Material')
-        main_model_part_name = self.full_model_part_name.split(".",1)[0]
-        self.main_model_part = self.model[main_model_part_name]
-
-        # Change name deprecated settings
-        self.TranslateLegacyVariablesAccordingToCurrentStandard(self.settings)
-        # Validate settings using default parameters defined in MPMVtkOutput process
-        # Default settings can be found in "custom_io/mpm_vtk_output.cpp"
-        default_settings = KratosMPM.MPMVtkOutput.GetDefaultParameters()
-        self.settings.ValidateAndAssignDefaults(default_settings)
-
-        if self.settings["save_output_files_in_folder"].GetBool():
-            if self.main_model_part.GetCommunicator().MyPID() == 0:
-                output_path = self.settings["output_path"].GetString()
-                if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
-                    kratos_utils.DeleteDirectoryIfExisting(output_path)
-            self.main_model_part.GetCommunicator().GetDataCommunicator().Barrier()
-
-        # Print background grid model part
-        if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
-            grid_settings = KratosMultiphysics.Parameters()
-            grid_settings.AddString("model_part_name","Background_Grid")
-            grid_settings.AddString("file_format",self.settings["file_format"].GetString())
-            grid_settings.AddDouble("output_precision",self.settings["output_precision"].GetDouble())
-            grid_settings.AddBool("output_sub_model_parts",self.settings["output_sub_model_parts"].GetBool())
-            grid_settings.AddString("output_path",self.settings["output_path"].GetString())
-            grid_settings.AddBool("save_output_files_in_folder",self.settings["save_output_files_in_folder"].GetBool())
-            background_grid = self.model["Background_Grid"]
-            KratosMultiphysics.VtkOutput(background_grid, grid_settings).PrintOutput()
-
-    # This function can be extended with new deprecated variables as they are generated
-    def TranslateLegacyVariablesAccordingToCurrentStandard(self, settings: KratosMultiphysics.Parameters) -> None:
-        context_string = type(self).__name__
-
-        old_name = 'output_frequency'
-        new_name = 'output_interval'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        old_name = 'write_properties_id'
-        new_name = 'write_ids'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        old_name = 'folder_name'
-        new_name = 'output_path'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        old_name = 'gauss_point_results'
-        new_name = 'gauss_point_variables_in_elements'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-    def ExecuteBeforeSolutionLoop(self) -> None:
-        vtk_model_part = self.model[self.full_model_part_name]
-        self.vtk_io = KratosMPM.MPMVtkOutput(vtk_model_part, self.settings)
-
-        self.__controller = KratosMultiphysics.OutputController(self.model, self.settings)
-
-        if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
-            self.vtk_io.PrintOutput()
-
-    def PrintOutput(self) -> None:
-        self.vtk_io.PrintOutput()
-        self.__controller.Update()
-
-    def IsOutputStep(self) -> bool:
-        return self.__controller.Evaluate()
+import KratosMultiphysics
+import KratosMultiphysics.kratos_utilities as kratos_utils
+from  KratosMultiphysics.deprecation_management import DeprecationManager
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+def Factory(settings: KratosMultiphysics.Parameters, model: KratosMultiphysics.Model) -> KratosMultiphysics.OutputProcess:
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a Model object, encapsulating a json string")
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return MPMVtkOutputProcess(model, settings["Parameters"])
+
+class MPMVtkOutputProcess(KratosMultiphysics.OutputProcess):
+
+    def __init__(self, model: KratosMultiphysics.Model, settings: KratosMultiphysics.Parameters) -> None:
+        super().__init__()
+
+        self.model = model
+        self.settings = settings
+
+        self.full_model_part_name = self.settings["model_part_name"].GetString()
+        if self.full_model_part_name.startswith('Background_Grid'):
+            self.full_model_part_name = self.full_model_part_name.replace('Background_Grid','MPM_Material')
+        main_model_part_name = self.full_model_part_name.split(".",1)[0]
+        self.main_model_part = self.model[main_model_part_name]
+
+        # Change name deprecated settings
+        self.TranslateLegacyVariablesAccordingToCurrentStandard(self.settings)
+        # Validate settings using default parameters defined in MPMVtkOutput process
+        # Default settings can be found in "custom_io/mpm_vtk_output.cpp"
+        default_settings = KratosMPM.MPMVtkOutput.GetDefaultParameters()
+        self.settings.ValidateAndAssignDefaults(default_settings)
+
+        if self.settings["save_output_files_in_folder"].GetBool():
+            if self.main_model_part.GetCommunicator().MyPID() == 0:
+                output_path = self.settings["output_path"].GetString()
+                if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
+                    kratos_utils.DeleteDirectoryIfExisting(output_path)
+            self.main_model_part.GetCommunicator().GetDataCommunicator().Barrier()
+
+        # Print background grid model part
+        if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
+            grid_settings = KratosMultiphysics.Parameters()
+            grid_settings.AddString("model_part_name","Background_Grid")
+            grid_settings.AddString("file_format",self.settings["file_format"].GetString())
+            grid_settings.AddDouble("output_precision",self.settings["output_precision"].GetDouble())
+            grid_settings.AddBool("output_sub_model_parts",self.settings["output_sub_model_parts"].GetBool())
+            grid_settings.AddString("output_path",self.settings["output_path"].GetString())
+            grid_settings.AddBool("save_output_files_in_folder",self.settings["save_output_files_in_folder"].GetBool())
+            background_grid = self.model["Background_Grid"]
+            KratosMultiphysics.VtkOutput(background_grid, grid_settings).PrintOutput()
+
+    # This function can be extended with new deprecated variables as they are generated
+    def TranslateLegacyVariablesAccordingToCurrentStandard(self, settings: KratosMultiphysics.Parameters) -> None:
+        context_string = type(self).__name__
+
+        old_name = 'output_frequency'
+        new_name = 'output_interval'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        old_name = 'write_properties_id'
+        new_name = 'write_ids'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        old_name = 'folder_name'
+        new_name = 'output_path'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        old_name = 'gauss_point_results'
+        new_name = 'gauss_point_variables_in_elements'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+    def ExecuteBeforeSolutionLoop(self) -> None:
+        vtk_model_part = self.model[self.full_model_part_name]
+        self.vtk_io = KratosMPM.MPMVtkOutput(vtk_model_part, self.settings)
+
+        self.__controller = KratosMultiphysics.OutputController(self.model, self.settings)
+
+        if not self.main_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
+            self.vtk_io.PrintOutput()
+
+    def PrintOutput(self) -> None:
+        self.vtk_io.PrintOutput()
+        self.__controller.Update()
+
+    def IsOutputStep(self) -> bool:
+        return self.__controller.Evaluate()
```

## KratosMultiphysics/MPMApplication/mpm_json_output_process.py

 * *Ordering differences only*

```diff
@@ -1,158 +1,158 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-from KratosMultiphysics.json_utilities import read_external_json, write_external_json
-
-# Importing the base class
-from KratosMultiphysics.json_output_process import JsonOutputProcess
-
-def Factory(settings, Model):
-    if(type(settings) != KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    return MPMJsonOutputProcess(Model, settings["Parameters"])
-
-# All the processes python processes should be derived from "Process"
-
-class MPMJsonOutputProcess(JsonOutputProcess):
-
-    def ExecuteBeforeSolutionLoop(self):
-
-        data = {}
-        data["TIME"] = []
-        count = 0
-
-        # Material points values
-        for mp in self.sub_model_part.Elements:
-            compute = self.__check_flag(mp)
-
-            if (compute == True):
-                if (self.resultant_solution == False):
-                    data["MP_" + str(mp.Id)] = {}
-                else:
-                    data["RESULTANT"] = {}
-
-                for i in range(self.params["gauss_points_output_variables"].size()):
-                    out = self.params["gauss_points_output_variables"][i]
-                    variable_name = out.GetString()
-                    variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
-
-                    if (variable_type == "Double" or variable_type == "Integer" or variable_type == "Component"):
-                        if (self.resultant_solution == False):
-                            data["MP_" + str(mp.Id)][variable_name] = []
-                        else:
-                            if (count == 0):
-                                data["RESULTANT"][variable_name] = []
-                    elif variable_type == "Array":
-                        if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
-                            if (self.resultant_solution == False):
-                                data["MP_" + str(mp.Id)][variable_name + "_X"] = []
-                                data["MP_" + str(mp.Id)][variable_name + "_Y"] = []
-                                data["MP_" + str(mp.Id)][variable_name + "_Z"] = []
-                            else:
-                                if (count == 0):
-                                    data["RESULTANT"][variable_name + "_X"] = []
-                                    data["RESULTANT"][variable_name + "_Y"] = []
-                                    data["RESULTANT"][variable_name + "_Z"] = []
-                        else:
-                            if (self.resultant_solution == False):
-                                data["MP_" + str(mp.Id)][variable_name] = []
-                            else:
-                                if (count == 0):
-                                    data["RESULTANT"][variable_name] = []
-                    elif variable_type == "Vector":
-                        if (self.resultant_solution == False):
-                            data["MP_" + str(mp.Id)][variable_name] = []
-                        else:
-                            if (count == 0):
-                                data["RESULTANT"][variable_name] = []
-
-                count += 1
-
-        write_external_json(self.output_file_name, data)
-
-    def ExecuteFinalizeSolutionStep(self):
-
-        data = read_external_json(self.output_file_name)
-
-        time = self.sub_model_part.ProcessInfo.GetValue(KratosMultiphysics.TIME)
-        dt = self.sub_model_part.ProcessInfo.GetValue(KratosMultiphysics.DELTA_TIME)
-        self.time_counter += dt
-        if self.time_counter > self.frequency:
-            self.time_counter = 0.0
-            data["TIME"].append(time)
-            count = 0
-
-            # Material points values
-            for mp in self.sub_model_part.Elements:
-                compute = self.__check_flag(mp)
-
-                if (compute == True):
-                    for i in range(self.params["gauss_points_output_variables"].size()):
-                        out = self.params["gauss_points_output_variables"][i]
-                        variable_name = out.GetString()
-                        variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
-                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
-                        values_vector = mp.CalculateOnIntegrationPoints(variable, self.sub_model_part.ProcessInfo)
-                        value = values_vector[0]
-
-                        if (variable_type == "Double" or variable_type == "Integer" or variable_type == "Component"):
-                            if (self.resultant_solution == False):
-                                data["MP_" + str(mp.Id)][variable_name].append(value)
-                            else:
-                                if (count == 0):
-                                    data["RESULTANT"][variable_name].append(value)
-                                else:
-                                    data["RESULTANT"][variable_name][-1] += value
-                        elif variable_type == "Array":
-                            if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
-                                if (self.resultant_solution == False):
-                                    data["MP_" + str(mp.Id)][variable_name + "_X"].append(value[0])
-                                    data["MP_" + str(mp.Id)][variable_name + "_Y"].append(value[1])
-                                    data["MP_" + str(mp.Id)][variable_name + "_Z"].append(value[2])
-                                else:
-                                    if (count == 0):
-                                        data["RESULTANT"][variable_name + "_X"].append(value[0])
-                                        data["RESULTANT"][variable_name + "_Y"].append(value[1])
-                                        data["RESULTANT"][variable_name + "_Z"].append(value[2])
-                                    else:
-                                        data["RESULTANT"][variable_name + "_X"][-1] += value[0]
-                                        data["RESULTANT"][variable_name + "_Y"][-1] += value[1]
-                                        data["RESULTANT"][variable_name + "_Z"][-1] += value[2]
-                            else:
-                                if (self.resultant_solution == False):
-                                    list = self.__kratos_vector_to__python_list(value)
-                                    data["MP_" + str(mp.Id)][variable_name ].append(list)
-                                else:
-                                    aux = 0.0
-                                    for index in range(len(value)):
-                                        aux += value[index]
-                                    if (count == 0):
-                                        data["RESULTANT"][variable_name ].append(aux)
-                                    else:
-                                        data["RESULTANT"][variable_name ][-1] += aux
-                        elif variable_type == "Vector":
-                            if (self.resultant_solution == False):
-                                list = self.__kratos_vector_to__python_list(value)
-                                data["MP_" + str(mp.Id)][variable_name].append(list)
-                            else:
-                                if (count == 0):
-                                    list = self.__kratos_vector_to__python_list(value)
-                                    data["RESULTANT"][variable_name][-1] += list
-
-                count += 1
-
-        write_external_json(self.output_file_name, data)
-
-    def __kratos_vector_to__python_list(self, value):
-
-        list = []
-        for index in range(len(value)):
-            list.append(value[index])
-        return list
-
-    def __check_flag(self, component):
-
-        if self.flag != None:
-            if component.Is(self.flag) == False:
-                return False
-
-        return True
+# Importing the Kratos Library
+import KratosMultiphysics
+from KratosMultiphysics.json_utilities import read_external_json, write_external_json
+
+# Importing the base class
+from KratosMultiphysics.json_output_process import JsonOutputProcess
+
+def Factory(settings, Model):
+    if(type(settings) != KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    return MPMJsonOutputProcess(Model, settings["Parameters"])
+
+# All the processes python processes should be derived from "Process"
+
+class MPMJsonOutputProcess(JsonOutputProcess):
+
+    def ExecuteBeforeSolutionLoop(self):
+
+        data = {}
+        data["TIME"] = []
+        count = 0
+
+        # Material points values
+        for mp in self.sub_model_part.Elements:
+            compute = self.__check_flag(mp)
+
+            if (compute == True):
+                if (self.resultant_solution == False):
+                    data["MP_" + str(mp.Id)] = {}
+                else:
+                    data["RESULTANT"] = {}
+
+                for i in range(self.params["gauss_points_output_variables"].size()):
+                    out = self.params["gauss_points_output_variables"][i]
+                    variable_name = out.GetString()
+                    variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
+
+                    if (variable_type == "Double" or variable_type == "Integer" or variable_type == "Component"):
+                        if (self.resultant_solution == False):
+                            data["MP_" + str(mp.Id)][variable_name] = []
+                        else:
+                            if (count == 0):
+                                data["RESULTANT"][variable_name] = []
+                    elif variable_type == "Array":
+                        if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
+                            if (self.resultant_solution == False):
+                                data["MP_" + str(mp.Id)][variable_name + "_X"] = []
+                                data["MP_" + str(mp.Id)][variable_name + "_Y"] = []
+                                data["MP_" + str(mp.Id)][variable_name + "_Z"] = []
+                            else:
+                                if (count == 0):
+                                    data["RESULTANT"][variable_name + "_X"] = []
+                                    data["RESULTANT"][variable_name + "_Y"] = []
+                                    data["RESULTANT"][variable_name + "_Z"] = []
+                        else:
+                            if (self.resultant_solution == False):
+                                data["MP_" + str(mp.Id)][variable_name] = []
+                            else:
+                                if (count == 0):
+                                    data["RESULTANT"][variable_name] = []
+                    elif variable_type == "Vector":
+                        if (self.resultant_solution == False):
+                            data["MP_" + str(mp.Id)][variable_name] = []
+                        else:
+                            if (count == 0):
+                                data["RESULTANT"][variable_name] = []
+
+                count += 1
+
+        write_external_json(self.output_file_name, data)
+
+    def ExecuteFinalizeSolutionStep(self):
+
+        data = read_external_json(self.output_file_name)
+
+        time = self.sub_model_part.ProcessInfo.GetValue(KratosMultiphysics.TIME)
+        dt = self.sub_model_part.ProcessInfo.GetValue(KratosMultiphysics.DELTA_TIME)
+        self.time_counter += dt
+        if self.time_counter > self.frequency:
+            self.time_counter = 0.0
+            data["TIME"].append(time)
+            count = 0
+
+            # Material points values
+            for mp in self.sub_model_part.Elements:
+                compute = self.__check_flag(mp)
+
+                if (compute == True):
+                    for i in range(self.params["gauss_points_output_variables"].size()):
+                        out = self.params["gauss_points_output_variables"][i]
+                        variable_name = out.GetString()
+                        variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
+                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
+                        values_vector = mp.CalculateOnIntegrationPoints(variable, self.sub_model_part.ProcessInfo)
+                        value = values_vector[0]
+
+                        if (variable_type == "Double" or variable_type == "Integer" or variable_type == "Component"):
+                            if (self.resultant_solution == False):
+                                data["MP_" + str(mp.Id)][variable_name].append(value)
+                            else:
+                                if (count == 0):
+                                    data["RESULTANT"][variable_name].append(value)
+                                else:
+                                    data["RESULTANT"][variable_name][-1] += value
+                        elif variable_type == "Array":
+                            if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
+                                if (self.resultant_solution == False):
+                                    data["MP_" + str(mp.Id)][variable_name + "_X"].append(value[0])
+                                    data["MP_" + str(mp.Id)][variable_name + "_Y"].append(value[1])
+                                    data["MP_" + str(mp.Id)][variable_name + "_Z"].append(value[2])
+                                else:
+                                    if (count == 0):
+                                        data["RESULTANT"][variable_name + "_X"].append(value[0])
+                                        data["RESULTANT"][variable_name + "_Y"].append(value[1])
+                                        data["RESULTANT"][variable_name + "_Z"].append(value[2])
+                                    else:
+                                        data["RESULTANT"][variable_name + "_X"][-1] += value[0]
+                                        data["RESULTANT"][variable_name + "_Y"][-1] += value[1]
+                                        data["RESULTANT"][variable_name + "_Z"][-1] += value[2]
+                            else:
+                                if (self.resultant_solution == False):
+                                    list = self.__kratos_vector_to__python_list(value)
+                                    data["MP_" + str(mp.Id)][variable_name ].append(list)
+                                else:
+                                    aux = 0.0
+                                    for index in range(len(value)):
+                                        aux += value[index]
+                                    if (count == 0):
+                                        data["RESULTANT"][variable_name ].append(aux)
+                                    else:
+                                        data["RESULTANT"][variable_name ][-1] += aux
+                        elif variable_type == "Vector":
+                            if (self.resultant_solution == False):
+                                list = self.__kratos_vector_to__python_list(value)
+                                data["MP_" + str(mp.Id)][variable_name].append(list)
+                            else:
+                                if (count == 0):
+                                    list = self.__kratos_vector_to__python_list(value)
+                                    data["RESULTANT"][variable_name][-1] += list
+
+                count += 1
+
+        write_external_json(self.output_file_name, data)
+
+    def __kratos_vector_to__python_list(self, value):
+
+        list = []
+        for index in range(len(value)):
+            list.append(value[index])
+        return list
+
+    def __check_flag(self, component):
+
+        if self.flag != None:
+            if component.Is(self.flag) == False:
+                return False
+
+        return True
```

## KratosMultiphysics/MPMApplication/particle_vtk_output_process.py

 * *Ordering differences only*

```diff
@@ -1,11 +1,11 @@
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-from KratosMultiphysics.MPMApplication.mpm_vtk_output_process import MPMVtkOutputProcess
-
-def Factory(settings: KratosMultiphysics.Parameters, model: KratosMultiphysics.Model) -> KratosMultiphysics.OutputProcess:
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a Model object, encapsulating a json string")
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    IssueDeprecationWarning("MPMApplication:","`ParticleVTKOutputProcess` is deprecated and replaced with `MPMVtkOutputProcess`")
-    return MPMVtkOutputProcess(model, settings["Parameters"])
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+from KratosMultiphysics.MPMApplication.mpm_vtk_output_process import MPMVtkOutputProcess
+
+def Factory(settings: KratosMultiphysics.Parameters, model: KratosMultiphysics.Model) -> KratosMultiphysics.OutputProcess:
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a Model object, encapsulating a json string")
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    IssueDeprecationWarning("MPMApplication:","`ParticleVTKOutputProcess` is deprecated and replaced with `MPMVtkOutputProcess`")
+    return MPMVtkOutputProcess(model, settings["Parameters"])
```

## KratosMultiphysics/MPMApplication/assign_gravity_to_material_point_process.py

 * *Ordering differences only*

```diff
@@ -1,54 +1,54 @@
-import KratosMultiphysics
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return AssignGravityToMaterialPointProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class AssignGravityToMaterialPointProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        default_settings = KratosMultiphysics.Parameters("""
-            {
-                "mesh_id"              : 0,
-                "model_part_name"      : "please_specify_model_part_name",
-                "variable_name"        : "MP_VOLUME_ACCELERATION",
-                "modulus"              : 1.0,
-                "constrained"          : true,
-                "direction"            : [0.0, 0.0, 0.0],
-                "local_axes"           : {}
-            }
-            """)
-
-        # Trick: allow "modulus" and "direction" to be a double or a string value (otherwise the ValidateAndAssignDefaults might fail)
-        if(settings.Has("modulus")):
-            if(settings["modulus"].IsString()):
-                default_settings["modulus"].SetString("0.0")
-
-        if(settings.Has("direction")):
-            if(settings["direction"].IsString()):
-                default_settings["direction"].SetString("Automatic")
-
-        # Detect if variable_name is MP_VOLUME_ACCELERATION
-        if(settings.Has("variable_name")):
-            if(settings["variable_name"].GetString() != "MP_VOLUME_ACCELERATION"):
-                KratosMultiphysics.Logger.PrintInfo("Warning in apply gravity to material point", "Error in determining variable_name")
-                raise Exception('The assign_gravity_to_material_point_process only accepts \"MP_VOLUME_ACCELERATION\" as variable_name.')
-
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        # Default settings
-        self.model_part = Model[settings["model_part_name"].GetString()]
-        self.modulus = settings["modulus"].GetDouble()
-        self.gravity_direction = settings["direction"].GetVector()
-        self.gravity_acceleration = self.modulus * self.gravity_direction
-
-    def ExecuteBeforeSolutionLoop(self):
-        if not self.model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
-            # Assign gravity to MP after solver.Initialize() - only apply once at the beginning!
-            for element in self.model_part.Elements:
-                element.SetValuesOnIntegrationPoints(KratosMPM.MP_VOLUME_ACCELERATION,[self.gravity_acceleration],self.model_part.ProcessInfo)
-                element.SetValuesOnIntegrationPoints(KratosMPM.MP_ACCELERATION,[self.gravity_acceleration],self.model_part.ProcessInfo)
+import KratosMultiphysics
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return AssignGravityToMaterialPointProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class AssignGravityToMaterialPointProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        default_settings = KratosMultiphysics.Parameters("""
+            {
+                "mesh_id"              : 0,
+                "model_part_name"      : "please_specify_model_part_name",
+                "variable_name"        : "MP_VOLUME_ACCELERATION",
+                "modulus"              : 1.0,
+                "constrained"          : true,
+                "direction"            : [0.0, 0.0, 0.0],
+                "local_axes"           : {}
+            }
+            """)
+
+        # Trick: allow "modulus" and "direction" to be a double or a string value (otherwise the ValidateAndAssignDefaults might fail)
+        if(settings.Has("modulus")):
+            if(settings["modulus"].IsString()):
+                default_settings["modulus"].SetString("0.0")
+
+        if(settings.Has("direction")):
+            if(settings["direction"].IsString()):
+                default_settings["direction"].SetString("Automatic")
+
+        # Detect if variable_name is MP_VOLUME_ACCELERATION
+        if(settings.Has("variable_name")):
+            if(settings["variable_name"].GetString() != "MP_VOLUME_ACCELERATION"):
+                KratosMultiphysics.Logger.PrintInfo("Warning in apply gravity to material point", "Error in determining variable_name")
+                raise Exception('The assign_gravity_to_material_point_process only accepts \"MP_VOLUME_ACCELERATION\" as variable_name.')
+
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        # Default settings
+        self.model_part = Model[settings["model_part_name"].GetString()]
+        self.modulus = settings["modulus"].GetDouble()
+        self.gravity_direction = settings["direction"].GetVector()
+        self.gravity_acceleration = self.modulus * self.gravity_direction
+
+    def ExecuteBeforeSolutionLoop(self):
+        if not self.model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
+            # Assign gravity to MP after solver.Initialize() - only apply once at the beginning!
+            for element in self.model_part.Elements:
+                element.SetValuesOnIntegrationPoints(KratosMPM.MP_VOLUME_ACCELERATION,[self.gravity_acceleration],self.model_part.ProcessInfo)
+                element.SetValuesOnIntegrationPoints(KratosMPM.MP_ACCELERATION,[self.gravity_acceleration],self.model_part.ProcessInfo)
```

## KratosMultiphysics/MPMApplication/apply_mpm_slip_boundary_process.py

 * *Ordering differences only*

```diff
@@ -1,40 +1,40 @@
-import KratosMultiphysics
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyMPMSlipBoundaryProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ApplyMPMSlipBoundaryProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        default_parameters = KratosMultiphysics.Parameters( """
-            {
-                "model_part_name":"PLEASE_CHOOSE_MODEL_PART_NAME",
-                "mesh_id": 0,
-                "avoid_recomputing_normals": true
-            }  """ )
-
-        settings.ValidateAndAssignDefaults(default_parameters)
-
-        self.model_part = Model[settings["model_part_name"].GetString()]
-        self.avoid_recomputing_normals = settings["avoid_recomputing_normals"].GetBool()
-
-        # Compute the normal on the nodes of interest -
-        # Note that the model part employed here is supposed to only have slip "conditions"
-        KratosMultiphysics.NormalCalculationUtils().CalculateOnSimplex(self.model_part, self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE])
-
-        #TODO: Remove the IS_STRUCTURE variable set as soon as the flag SLIP migration is done
-        for node in self.model_part.Nodes:
-            node.Set(KratosMultiphysics.SLIP, True)
-            node.SetValue(KratosMultiphysics.IS_STRUCTURE,1.0)
-            node.SetSolutionStepValue(KratosMultiphysics.IS_STRUCTURE,0,1.0)
-
-
-
-    def ExecuteInitializeSolutionStep(self):
-        # Recompute the normals if needed
-        if self.avoid_recomputing_normals == False:
-            KratosMultiphysics.NormalCalculationUtils().CalculateOnSimplex(self.model_part, self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE])
+import KratosMultiphysics
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyMPMSlipBoundaryProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ApplyMPMSlipBoundaryProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        default_parameters = KratosMultiphysics.Parameters( """
+            {
+                "model_part_name":"PLEASE_CHOOSE_MODEL_PART_NAME",
+                "mesh_id": 0,
+                "avoid_recomputing_normals": true
+            }  """ )
+
+        settings.ValidateAndAssignDefaults(default_parameters)
+
+        self.model_part = Model[settings["model_part_name"].GetString()]
+        self.avoid_recomputing_normals = settings["avoid_recomputing_normals"].GetBool()
+
+        # Compute the normal on the nodes of interest -
+        # Note that the model part employed here is supposed to only have slip "conditions"
+        KratosMultiphysics.NormalCalculationUtils().CalculateOnSimplex(self.model_part, self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE])
+
+        #TODO: Remove the IS_STRUCTURE variable set as soon as the flag SLIP migration is done
+        for node in self.model_part.Nodes:
+            node.Set(KratosMultiphysics.SLIP, True)
+            node.SetValue(KratosMultiphysics.IS_STRUCTURE,1.0)
+            node.SetSolutionStepValue(KratosMultiphysics.IS_STRUCTURE,0,1.0)
+
+
+
+    def ExecuteInitializeSolutionStep(self):
+        # Recompute the normals if needed
+        if self.avoid_recomputing_normals == False:
+            KratosMultiphysics.NormalCalculationUtils().CalculateOnSimplex(self.model_part, self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE])
```

## KratosMultiphysics/MPMApplication/apply_mpm_particle_dirichlet_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,179 +1,179 @@
-import KratosMultiphysics
-from KratosMultiphysics.deprecation_management import DeprecationManager
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyMPMParticleDirichletConditionProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ApplyMPMParticleDirichletConditionProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        default_parameters = KratosMultiphysics.Parameters( """
-            {
-                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
-                "material_points_per_condition"   : 0,
-                "imposition_type"           : "penalty",
-                "penalty_factor"            : 0,
-                "variable_name"             : "DISPLACEMENT",
-                "constrained"               : "fixed",
-                "value"                     : [0.0, "0*t", 0.0],
-                "interval"                  : [0.0, 1e30],
-                "option"                    : "",
-                "is_equal_distributed"      : false,
-                "local_axes"                : {}
-            }  """ )
-
-         # Assign this here since it will change the "interval" prior to validation
-        self.interval = KratosMultiphysics.IntervalUtility(settings)
-
-        context_string = type(self).__name__
-        old_name = 'particles_per_condition'
-        new_name = 'material_points_per_condition'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        settings.ValidateAndAssignDefaults(default_parameters)
-
-        self.model_part = Model[settings["model_part_name"].GetString()]
-        self.model_part_name = settings["model_part_name"].GetString()
-        self.model = Model
-        self.material_points_per_condition = settings["material_points_per_condition"].GetInt()
-        self.imposition_type = settings["imposition_type"].GetString()
-        self.is_neumann_boundary = False
-        self.option = settings["option"].GetString()
-
-        #is_equal_distributed = false (material point conditions at Gauss Point Positions)
-        #is_equal_distributed = true (material point conditions equally distributed; also at nodes; only 2D)
-        self.is_equal_distributed = settings["is_equal_distributed"].GetBool()
-
-        """
-        Set boundary_condition_type:
-        1. penalty
-        2. lagrange (WIP)
-        3. fixdof (WIP)
-        """
-
-        # set type of boundary
-        if (self.imposition_type == "penalty" or self.imposition_type == "Penalty"):
-            self.penalty_factor = settings["penalty_factor"].GetDouble()
-            self.boundary_condition_type = 1
-        else:
-            err_msg =  "The requested type of Dirichlet boundary imposition: \"" + self.imposition_type + "\" is not available!\n"
-            err_msg += "Available option is: \"penalty\"."
-            raise Exception(err_msg)
-
-        # check constraint
-        self.constrained = settings["constrained"].GetString()
-        self.is_slip_boundary = False
-        self.is_contact_boundary = False
-        if (self.constrained == "fixed"):
-            pass
-        elif (self.constrained == "contact"):
-            self.is_contact_boundary = True
-        elif (self.constrained == "slip"):
-            self.is_slip_boundary = True
-        elif (self.constrained == "contact_slip"):
-            self.is_contact_boundary = True
-            self.is_slip_boundary = True
-        else:
-            err_msg =  "The requested type of constrain: \"" + self.constrained + "\" is not available!\n"
-            err_msg += "Available options are: \"fixed\", \"contact\" and \"slip\"."
-            raise Exception(err_msg)
-
-        # get variable imposed and check
-        variable_name = settings["variable_name"].GetString()
-        variable_name_list = ["DISPLACEMENT","VELOCITY","ACCELERATION"]
-        if(variable_name in variable_name_list):
-            self.variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
-        else:
-            err_msg =  "The given variable \"" + variable_name + "\" is not available to be imposed with this process.\n"
-            err_msg += "Available options are: " + ", ".join(variable_name_list)
-            raise Exception(err_msg)
-
-        self.value_is_numeric = [False, False, False]
-        self.value = KratosMultiphysics.Vector(3)
-        self.aux_function = ["0.0","0.0","0.0"]
-        self.name = ["0.0","0.0","0.0"]
-        # Loop over components X, Y and Z
-        for i, variable in enumerate(["_X", "_Y", "_Z"]):
-            self.name[i] = settings["variable_name"].GetString() + variable
-            if settings["value"][i].IsNumber():
-                self.value_is_numeric[i] = True
-                self.value[i] = settings["value"][i].GetDouble()
-            else:
-                self.function_string = settings["value"][i].GetString()
-                self.aux_function[i] = KratosMultiphysics.GenericFunctionUtility(self.function_string, settings["local_axes"])
-
-
-        # Compute the normal on the nodes of interest
-        KratosMultiphysics.NormalCalculationUtils().CalculateOnSimplex(self.model_part, self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE])
-        self.modified_normal = False
-        if self.option == "flip_normal":
-            self.modified_normal = True
-
-        # Set Flag BOUNDARY and variables MATERIAL_POINTS_PER_CONDITION
-        if self.material_points_per_condition >= 0:
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BOUNDARY, True, self.model_part.Nodes)
-
-            for condition in self.model_part.Conditions:
-                condition.Set(KratosMultiphysics.BOUNDARY, True)
-                condition.Set(KratosMultiphysics.SLIP, self.is_slip_boundary)
-                condition.Set(KratosMultiphysics.CONTACT, self.is_contact_boundary)
-                condition.Set(KratosMultiphysics.MODIFIED, self.modified_normal)
-                condition.SetValue(KratosMPM.MATERIAL_POINTS_PER_CONDITION, self.material_points_per_condition)
-                condition.SetValue(KratosMPM.IS_EQUAL_DISTRIBUTED, self.is_equal_distributed)
-                condition.SetValue(KratosMPM.MPC_IS_NEUMANN, self.is_neumann_boundary)
-                condition.SetValue(KratosMPM.MPC_BOUNDARY_CONDITION_TYPE, self.boundary_condition_type)
-
-                ### Set necessary essential BC variables
-                if self.boundary_condition_type==1:
-                    condition.SetValue(KratosMPM.PENALTY_FACTOR, self.penalty_factor)
-        else:
-            err_msg = '\n::[ApplyMPMParticleDirichletConditionProcess]:: W-A-R-N-I-N-G: You have specified invalid "material_points_per_condition", '
-            err_msg += 'or assigned negative values. \nPlease assign: "material_points_per_condition" > 0 or = 0 (for automatic value)!\n'
-            raise Exception(err_msg)
-
-    def ExecuteBeforeSolutionLoop(self):
-        """ This method is executed in before initialize the solution step
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-
-        # Get updated model_part
-        if (self.model_part_name.startswith('Background_Grid.')):
-            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
-        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
-        self.model_part = self.model[mpm_material_model_part_name]
-        self.ExecuteInitializeSolutionStep()
-
-    def ExecuteInitializeSolutionStep(self):
-        """ This method is executed in order to initialize the current step
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-
-        for mpc in self.model_part.Conditions:
-            current_time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
-            mpc_coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
-
-            if self.interval.IsInInterval(current_time):
-
-                self.step_is_active = True
-
-                # Loop over components X, Y and Z
-                for i in range(3):
-                    self.variable = self.name[i]
-                    if  not self.value_is_numeric[i]:
-                        if self.aux_function[i].DependsOnSpace() == False: #depends on time only
-                            self.value[i] = self.aux_function[i].CallFunction(0.0,0.0,0.0,current_time,0.0,0.0,0.0)
-                        else: #most general case - space varying function (possibly also time varying)
-                            self.value[i] = self.aux_function[i].CallFunction(mpc_coord[0],mpc_coord[1],mpc_coord[2],current_time,0.0,0.0,0.0)
-
-
-                mpc.SetValuesOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT,[self.value],self.model_part.ProcessInfo)
+import KratosMultiphysics
+from KratosMultiphysics.deprecation_management import DeprecationManager
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyMPMParticleDirichletConditionProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ApplyMPMParticleDirichletConditionProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        default_parameters = KratosMultiphysics.Parameters( """
+            {
+                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
+                "material_points_per_condition"   : 0,
+                "imposition_type"           : "penalty",
+                "penalty_factor"            : 0,
+                "variable_name"             : "DISPLACEMENT",
+                "constrained"               : "fixed",
+                "value"                     : [0.0, "0*t", 0.0],
+                "interval"                  : [0.0, 1e30],
+                "option"                    : "",
+                "is_equal_distributed"      : false,
+                "local_axes"                : {}
+            }  """ )
+
+         # Assign this here since it will change the "interval" prior to validation
+        self.interval = KratosMultiphysics.IntervalUtility(settings)
+
+        context_string = type(self).__name__
+        old_name = 'particles_per_condition'
+        new_name = 'material_points_per_condition'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        settings.ValidateAndAssignDefaults(default_parameters)
+
+        self.model_part = Model[settings["model_part_name"].GetString()]
+        self.model_part_name = settings["model_part_name"].GetString()
+        self.model = Model
+        self.material_points_per_condition = settings["material_points_per_condition"].GetInt()
+        self.imposition_type = settings["imposition_type"].GetString()
+        self.is_neumann_boundary = False
+        self.option = settings["option"].GetString()
+
+        #is_equal_distributed = false (material point conditions at Gauss Point Positions)
+        #is_equal_distributed = true (material point conditions equally distributed; also at nodes; only 2D)
+        self.is_equal_distributed = settings["is_equal_distributed"].GetBool()
+
+        """
+        Set boundary_condition_type:
+        1. penalty
+        2. lagrange (WIP)
+        3. fixdof (WIP)
+        """
+
+        # set type of boundary
+        if (self.imposition_type == "penalty" or self.imposition_type == "Penalty"):
+            self.penalty_factor = settings["penalty_factor"].GetDouble()
+            self.boundary_condition_type = 1
+        else:
+            err_msg =  "The requested type of Dirichlet boundary imposition: \"" + self.imposition_type + "\" is not available!\n"
+            err_msg += "Available option is: \"penalty\"."
+            raise Exception(err_msg)
+
+        # check constraint
+        self.constrained = settings["constrained"].GetString()
+        self.is_slip_boundary = False
+        self.is_contact_boundary = False
+        if (self.constrained == "fixed"):
+            pass
+        elif (self.constrained == "contact"):
+            self.is_contact_boundary = True
+        elif (self.constrained == "slip"):
+            self.is_slip_boundary = True
+        elif (self.constrained == "contact_slip"):
+            self.is_contact_boundary = True
+            self.is_slip_boundary = True
+        else:
+            err_msg =  "The requested type of constrain: \"" + self.constrained + "\" is not available!\n"
+            err_msg += "Available options are: \"fixed\", \"contact\" and \"slip\"."
+            raise Exception(err_msg)
+
+        # get variable imposed and check
+        variable_name = settings["variable_name"].GetString()
+        variable_name_list = ["DISPLACEMENT","VELOCITY","ACCELERATION"]
+        if(variable_name in variable_name_list):
+            self.variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
+        else:
+            err_msg =  "The given variable \"" + variable_name + "\" is not available to be imposed with this process.\n"
+            err_msg += "Available options are: " + ", ".join(variable_name_list)
+            raise Exception(err_msg)
+
+        self.value_is_numeric = [False, False, False]
+        self.value = KratosMultiphysics.Vector(3)
+        self.aux_function = ["0.0","0.0","0.0"]
+        self.name = ["0.0","0.0","0.0"]
+        # Loop over components X, Y and Z
+        for i, variable in enumerate(["_X", "_Y", "_Z"]):
+            self.name[i] = settings["variable_name"].GetString() + variable
+            if settings["value"][i].IsNumber():
+                self.value_is_numeric[i] = True
+                self.value[i] = settings["value"][i].GetDouble()
+            else:
+                self.function_string = settings["value"][i].GetString()
+                self.aux_function[i] = KratosMultiphysics.GenericFunctionUtility(self.function_string, settings["local_axes"])
+
+
+        # Compute the normal on the nodes of interest
+        KratosMultiphysics.NormalCalculationUtils().CalculateOnSimplex(self.model_part, self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE])
+        self.modified_normal = False
+        if self.option == "flip_normal":
+            self.modified_normal = True
+
+        # Set Flag BOUNDARY and variables MATERIAL_POINTS_PER_CONDITION
+        if self.material_points_per_condition >= 0:
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BOUNDARY, True, self.model_part.Nodes)
+
+            for condition in self.model_part.Conditions:
+                condition.Set(KratosMultiphysics.BOUNDARY, True)
+                condition.Set(KratosMultiphysics.SLIP, self.is_slip_boundary)
+                condition.Set(KratosMultiphysics.CONTACT, self.is_contact_boundary)
+                condition.Set(KratosMultiphysics.MODIFIED, self.modified_normal)
+                condition.SetValue(KratosMPM.MATERIAL_POINTS_PER_CONDITION, self.material_points_per_condition)
+                condition.SetValue(KratosMPM.IS_EQUAL_DISTRIBUTED, self.is_equal_distributed)
+                condition.SetValue(KratosMPM.MPC_IS_NEUMANN, self.is_neumann_boundary)
+                condition.SetValue(KratosMPM.MPC_BOUNDARY_CONDITION_TYPE, self.boundary_condition_type)
+
+                ### Set necessary essential BC variables
+                if self.boundary_condition_type==1:
+                    condition.SetValue(KratosMPM.PENALTY_FACTOR, self.penalty_factor)
+        else:
+            err_msg = '\n::[ApplyMPMParticleDirichletConditionProcess]:: W-A-R-N-I-N-G: You have specified invalid "material_points_per_condition", '
+            err_msg += 'or assigned negative values. \nPlease assign: "material_points_per_condition" > 0 or = 0 (for automatic value)!\n'
+            raise Exception(err_msg)
+
+    def ExecuteBeforeSolutionLoop(self):
+        """ This method is executed in before initialize the solution step
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+
+        # Get updated model_part
+        if (self.model_part_name.startswith('Background_Grid.')):
+            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
+        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
+        self.model_part = self.model[mpm_material_model_part_name]
+        self.ExecuteInitializeSolutionStep()
+
+    def ExecuteInitializeSolutionStep(self):
+        """ This method is executed in order to initialize the current step
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+
+        for mpc in self.model_part.Conditions:
+            current_time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
+            mpc_coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
+
+            if self.interval.IsInInterval(current_time):
+
+                self.step_is_active = True
+
+                # Loop over components X, Y and Z
+                for i in range(3):
+                    self.variable = self.name[i]
+                    if  not self.value_is_numeric[i]:
+                        if self.aux_function[i].DependsOnSpace() == False: #depends on time only
+                            self.value[i] = self.aux_function[i].CallFunction(0.0,0.0,0.0,current_time,0.0,0.0,0.0)
+                        else: #most general case - space varying function (possibly also time varying)
+                            self.value[i] = self.aux_function[i].CallFunction(mpc_coord[0],mpc_coord[1],mpc_coord[2],current_time,0.0,0.0,0.0)
+
+
+                mpc.SetValuesOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT,[self.value],self.model_part.ProcessInfo)
```

## KratosMultiphysics/MPMApplication/mpm_solver.py

 * *Ordering differences only*

```diff
@@ -1,518 +1,518 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications and dependencies
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-# Importing the base class
-from KratosMultiphysics.python_solver import PythonSolver
-
-# Other imports
-from KratosMultiphysics import auxiliary_solver_utilities
-from KratosMultiphysics import python_linear_solver_factory as linear_solver_factory
-from KratosMultiphysics.deprecation_management import DeprecationManager
-
-def CreateSolver(model, custom_settings):
-    return MPMSolver(model, custom_settings)
-
-class MPMSolver(PythonSolver):
-
-    ### Solver constructor
-    def __init__(self, model, custom_settings):
-        self._validate_settings_in_baseclass=True # To be removed eventually
-        super(MPMSolver, self).__init__(model, custom_settings)
-
-        # Add model part containers
-        self._AddModelPartContainers()
-
-        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ", "Solver is constructed correctly.")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""
-        {
-            "model_part_name" : "MPM_Material",
-            "domain_size"     : -1,
-            "echo_level"      : 0,
-            "time_stepping"   : { },
-            "time_integration_method"   : "implicit",
-            "analysis_type"   : "non_linear",
-            "grid_model_import_settings" : {
-                "input_type"     : "mdpa",
-                "input_filename" : "unknown_name_Grid"
-            },
-            "model_import_settings" : {
-                "input_type"        : "mdpa",
-                "input_filename"    : "unknown_name_Body"
-            },
-            "material_import_settings" : {
-                "materials_filename" : ""
-            },
-            "compute_reactions"                  : false,
-            "convergence_criterion"              : "Residual_criteria",
-            "displacement_relative_tolerance"    : 1.0E-4,
-            "displacement_absolute_tolerance"    : 1.0E-9,
-            "residual_relative_tolerance"        : 1.0E-4,
-            "residual_absolute_tolerance"        : 1.0E-9,
-            "max_iteration"                      : 20,
-            "pressure_dofs"                      : false,
-            "stabilization"                      : "ppp",
-            "compressible"                       : true,
-            "axis_symmetric_flag"                : false,
-            "consistent_mass_matrix"             : false,
-            "block_builder"                      : true,
-            "move_mesh_flag"                     : false,
-            "problem_domain_sub_model_part_list" : [],
-            "processes_sub_model_part_list"      : [],
-            "auxiliary_variables_list"           : [],
-            "auxiliary_dofs_list"                : [],
-            "auxiliary_reaction_list"            : [],
-            "element_search_settings"            : {
-                "search_algorithm_type"          : "bin_based",
-                "max_number_of_results"          : 1000,
-                "searching_tolerance"            : 1.0E-5,
-                "remove_entities_not_found"      : true
-            },
-            "linear_solver_settings"             : {
-                "solver_type" : "amgcl",
-                "smoother_type":"damped_jacobi",
-                "krylov_type": "cg",
-                "coarsening_type": "aggregation",
-                "max_iteration": 200,
-                "provide_coordinates": false,
-                "gmres_krylov_space_dimension": 100,
-                "verbosity" : 0,
-                "tolerance": 1e-7,
-                "scaling": false,
-                "block_size": 3,
-                "use_block_matrices_if_possible" : true,
-                "coarse_enough" : 50
-            }
-        }""")
-        this_defaults.AddMissingParameters(super(MPMSolver, cls).GetDefaultParameters())
-        return this_defaults
-
-    ### Solver public functions
-
-    def GetMinimumBufferSize(self):
-        return 2
-
-    def AddVariables(self):
-        # Add variables to background grid model part
-        self._AddVariablesToModelPart(self.grid_model_part)
-
-        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ", "Variables are added.")
-
-    def ImportModelPart(self):
-        # Read model part
-        self._ModelPartReading()
-
-        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","Models are imported.")
-
-    def PrepareModelPart(self):
-        # Set buffer size
-        self._SetAndFillBuffer()
-
-        # Executes the check and prepare model process
-        self.__ExecuteCheckAndPrepare()
-
-        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ", "ModelPart prepared for Solver.")
-
-    def GetComputingModelPart(self):
-        if not self.model.HasModelPart(self.settings["model_part_name"].GetString()):
-            raise Exception("The ComputingModelPart was not created yet!")
-        return self.model.GetModelPart(self.settings["model_part_name"].GetString())
-
-    def GetGridModelPart(self):
-        if not self.model.HasModelPart("Background_Grid"):
-            raise Exception("The GridModelPart was not created yet!")
-        return self.model.GetModelPart("Background_Grid")
-
-    def AddDofs(self):
-        # Add dofs to background grid model part
-        self._AddDofsToModelPart(self.grid_model_part)
-
-        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","DOFs are added.")
-
-    def Initialize(self):
-        # The material point solution strategy is created here if it does not already exist.
-        material_point_solution_strategy = self._GetSolutionStrategy()
-        material_point_solution_strategy.SetEchoLevel(self.settings["echo_level"].GetInt())
-
-        # Generate material points
-        self._GenerateMaterialPoint()
-
-        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","Solver is initialized correctly.")
-
-    def AdvanceInTime(self, current_time):
-        dt = self.__ComputeDeltaTime()
-        new_time = current_time + dt
-        self.grid_model_part.ProcessInfo[KratosMultiphysics.STEP] += 1
-        self.grid_model_part.CloneTimeStep(new_time)
-
-        return new_time
-
-    def InitializeSolutionStep(self):
-        self._SearchElement()
-        self._GetSolutionStrategy().Initialize()
-
-        #clean nodal values and map from MPs to nodes
-        self._GetSolutionStrategy().InitializeSolutionStep()
-
-    def Predict(self):
-        self._GetSolutionStrategy().Predict()
-
-    def SolveSolutionStep(self):
-        # Calc residual, update momenta
-        is_converged = self._GetSolutionStrategy().SolveSolutionStep()
-        return is_converged
-
-    def FinalizeSolutionStep(self):
-        self._GetSolutionStrategy().FinalizeSolutionStep()
-
-        self._GetSolutionStrategy().Clear()
-
-        if self.is_restarted():
-            self.material_point_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED] = False
-
-    def Check(self):
-        self._GetSolutionStrategy().Check()
-
-    def Clear(self):
-        self._GetSolutionStrategy().Clear()
-
-    ### Solver special protected functions
-
-    def _GetSolutionScheme(self):
-        if not hasattr(self, '_solution_scheme'):
-            self._solution_scheme = self._CreateSolutionScheme()
-        return self._solution_scheme
-
-    def _GetConvergenceCriteria(self):
-        if not hasattr(self, '_convergence_criterion'):
-            self._convergence_criterion = self._CreateConvergenceCriteria()
-        return self._convergence_criterion
-
-    def _GetLinearSolver(self):
-        if not hasattr(self, '_linear_solver'):
-            self._linear_solver = self._CreateLinearSolver()
-        return self._linear_solver
-
-    def _GetBuilderAndSolver(self):
-        if not hasattr(self, '_builder_and_solver'):
-            self._builder_and_solver = self._CreateBuilderAndSolver()
-        return self._builder_and_solver
-
-    def _GetSolutionStrategy(self):
-        if not hasattr(self, '_solution_strategy'):
-            self._solution_strategy = self._CreateSolutionStrategy()
-        return self._solution_strategy
-
-    ### Solver protected functions
-
-    def _GenerateMaterialPoint(self):
-        pressure_dofs          = self.settings["pressure_dofs"].GetBool()
-        axis_symmetric_flag    = self.settings["axis_symmetric_flag"].GetBool()
-        if axis_symmetric_flag:
-            self.grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_AXISYMMETRIC, True)
-        else:
-            self.grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_AXISYMMETRIC, False)
-        stabilization          = self.settings["stabilization"].GetString()
-        if pressure_dofs:
-            if (stabilization=="none"):
-                stabilization_type = 0
-                KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","WARNING: No stabilization considered for a mixed formulation.")
-            elif (stabilization =="ppp"): #Polynomial Pressure Projection stabilization
-                stabilization_type = 1
-            self.grid_model_part.ProcessInfo.SetValue(KratosMPM.STABILIZATION_TYPE, stabilization_type)
-
-        # Assigning extra information to the main model part
-        self.material_point_model_part.SetNodes(self.grid_model_part.GetNodes())
-
-        if not self.is_restarted():
-            self.material_point_model_part.ProcessInfo = self.grid_model_part.ProcessInfo
-
-            # Generate MP Element and Condition
-            KratosMPM.GenerateMaterialPointElement(self.grid_model_part, self.initial_mesh_model_part, self.material_point_model_part, pressure_dofs)
-            KratosMPM.GenerateMaterialPointCondition(self.grid_model_part, self.initial_mesh_model_part, self.material_point_model_part)
-        else:
-            self.grid_model_part.ProcessInfo = self.material_point_model_part.ProcessInfo
-
-    def _SearchElement(self):
-        searching_alg_type = self.settings["element_search_settings"]["search_algorithm_type"].GetString()
-        max_number_of_search_results = self.settings["element_search_settings"]["max_number_of_results"].GetInt()
-        searching_tolerance          = self.settings["element_search_settings"]["searching_tolerance"].GetDouble()
-        if (searching_alg_type == "bin_based"):
-            KratosMPM.SearchElement(self.grid_model_part, self.material_point_model_part, max_number_of_search_results, searching_tolerance)
-        else:
-            err_msg  = "The requested searching algorithm \"" + searching_alg_type
-            err_msg += "\" is not available for MPMApplication!\n"
-            err_msg += "Available options are: \"bin_based\""
-            raise Exception(err_msg)
-        remove_entities_not_found = self.settings["element_search_settings"]["remove_entities_not_found"].GetBool()
-        if remove_entities_not_found: KratosMPM.MaterialPointEraseProcess(self.material_point_model_part).Execute()
-
-    def _AddModelPartContainers(self):
-        domain_size = self._GetDomainSize()
-        if domain_size not in [2,3]:
-            err_msg  = "The input \"domain_size\" is wrong!"
-            err_msg += "Available options are: \"2\" or \"3\""
-            raise Exception(err_msg)
-
-        ## In MPM three model parts are needed
-        # Material model part definition
-        material_point_model_part_name = self.settings["model_part_name"].GetString()
-        if not self.model.HasModelPart(material_point_model_part_name):
-            self.material_point_model_part = self.model.CreateModelPart(material_point_model_part_name) # Equivalent to model_part3 in the old format
-            self.material_point_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
-
-        # Grid model part definition
-        if not self.model.HasModelPart("Background_Grid"):
-            self.grid_model_part = self.model.CreateModelPart("Background_Grid") #Equivalent to model_part1 in the old format
-            self.grid_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
-
-        if not self.is_restarted():
-            # Initial material model part definition
-            initial_mesh_model_part_name = "Initial_" + material_point_model_part_name
-            if not self.model.HasModelPart(initial_mesh_model_part_name):
-                self.initial_mesh_model_part = self.model.CreateModelPart(initial_mesh_model_part_name) #Equivalent to model_part2 in the old format
-                self.initial_mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
-
-
-    def _AddVariablesToModelPart(self, model_part):
-        # Add displacements and reaction
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
-
-        # Add specific variables for the problem conditions
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
-
-        # MPM specific nodal variables
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_MASS)
-        model_part.AddNodalSolutionStepVariable(KratosMPM.NODAL_MOMENTUM)
-        model_part.AddNodalSolutionStepVariable(KratosMPM.NODAL_INERTIA)
-
-        # Add variables that the user defined in the ProjectParameters
-        auxiliary_solver_utilities.AddVariables(model_part, self.settings["auxiliary_variables_list"])
-
-        # Add variables for specific cases
-        if self.settings["pressure_dofs"].GetBool():
-            # add specific variables for the problem (pressure dofs)
-            model_part.AddNodalSolutionStepVariable(KratosMPM.PRESSURE_REACTION)
-            model_part.AddNodalSolutionStepVariable(KratosMPM.NODAL_MPRESSURE)
-
-    def _AddDynamicVariables(self, model_part):
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
-
-    def _ModelPartReading(self):
-        # reading the model part of the background grid
-        if(self.settings["grid_model_import_settings"]["input_type"].GetString() == "mdpa"):
-            self._ImportModelPart(self.grid_model_part, self.settings["grid_model_import_settings"])
-        else:
-            raise Exception("Other input options are not implemented yet.")
-
-        # reading the model part of the material point
-        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
-            self._ImportModelPart(self.initial_mesh_model_part, self.settings["model_import_settings"])
-        elif(self.settings["model_import_settings"]["input_type"].GetString() == "rest"):
-            self.settings["model_import_settings"]["input_filename"].SetString("MPM_Material")
-            self._ImportModelPart(self.material_point_model_part, self.settings["model_import_settings"])
-        else:
-            raise Exception("Other input options are not implemented yet.")
-
-    def _AddDofsToModelPart(self, model_part):
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X, model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y, model_part)
-        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z, model_part)
-
-        if self.settings["pressure_dofs"].GetBool():
-            KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.PRESSURE, KratosMPM.PRESSURE_REACTION, model_part)
-
-        # Add dofs that the user defined in the ProjectParameters
-        auxiliary_solver_utilities.AddDofs(model_part, self.settings["auxiliary_dofs_list"], self.settings["auxiliary_reaction_list"])
-
-    def _GetDomainSize(self):
-        if not hasattr(self, '_domain_size'):
-            self._domain_size = self.settings["domain_size"].GetInt()
-        return self._domain_size
-
-    def _GetConvergenceCriteriaSettings(self):
-        # Create an auxiliary Kratos parameters object to store the convergence settings.
-        conv_params = KratosMultiphysics.Parameters("{}")
-        conv_params.AddValue("convergence_criterion",self.settings["convergence_criterion"])
-        conv_params.AddValue("echo_level",self.settings["echo_level"])
-        conv_params.AddValue("displacement_relative_tolerance",self.settings["displacement_relative_tolerance"])
-        conv_params.AddValue("displacement_absolute_tolerance",self.settings["displacement_absolute_tolerance"])
-        conv_params.AddValue("residual_relative_tolerance",self.settings["residual_relative_tolerance"])
-        conv_params.AddValue("residual_absolute_tolerance",self.settings["residual_absolute_tolerance"])
-
-        return conv_params
-
-    def _CreateConvergenceCriteria(self):
-        convergence_criterion_parameters = self._GetConvergenceCriteriaSettings()
-        if (convergence_criterion_parameters["convergence_criterion"].GetString() == "residual_criterion"):
-            R_RT = convergence_criterion_parameters["residual_relative_tolerance"].GetDouble()
-            R_AT = convergence_criterion_parameters["residual_absolute_tolerance"].GetDouble()
-            convergence_criterion = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
-            convergence_criterion.SetEchoLevel(convergence_criterion_parameters["echo_level"].GetInt())
-        elif (convergence_criterion_parameters["convergence_criterion"].GetString() == "displacement_criterion"):
-            D_RT = convergence_criterion_parameters["displacement_relative_tolerance"].GetDouble()
-            D_AT = convergence_criterion_parameters["displacement_absolute_tolerance"].GetDouble()
-            convergence_criterion = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
-            convergence_criterion.SetEchoLevel(convergence_criterion_parameters["echo_level"].GetInt())
-        else:
-            err_msg  = "The requested convergence criteria \"" + convergence_criterion_parameters["convergence_criterion"].GetString()
-            err_msg += "\" is not supported for MPMApplication!\n"
-            err_msg += "Available options are: \"residual_criterion\" or \"displacement_criterion\""
-            raise Exception(err_msg)
-
-        return convergence_criterion
-
-    def _CreateLinearSolver(self):
-        linear_solver_configuration = self.settings["linear_solver_settings"]
-        if linear_solver_configuration.Has("solver_type"): # user specified a linear solver
-            return linear_solver_factory.ConstructSolver(linear_solver_configuration)
-        else:
-            KratosMultiphysics.Logger.PrintInfo('::[MPMSolver]:: No linear solver was specified, using fastest available solver')
-            return linear_solver_factory.CreateFastestAvailableDirectLinearSolver()
-
-    def _CreateBuilderAndSolver(self):
-        linear_solver = self._GetLinearSolver()
-        if self.settings["block_builder"].GetBool():
-            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(linear_solver)
-        else:
-            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(linear_solver)
-        return builder_and_solver
-
-    def _CreateSolutionScheme(self):
-        """Create the solution scheme for interested problem."""
-        raise Exception("Solution Scheme creation must be implemented in the derived class.")
-
-    def _CreateSolutionStrategy(self):
-        # this is for implicit only. explicit is implemented in derived mpm_explicit_solver
-        grid_model_part = self.GetGridModelPart();
-        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT, False)
-        analysis_type = self.settings["analysis_type"].GetString()
-        is_consistent_mass_matrix = self.settings["consistent_mass_matrix"].GetBool()
-        if is_consistent_mass_matrix:
-            self.grid_model_part.ProcessInfo.SetValue(KratosMultiphysics.COMPUTE_LUMPED_MASS_MATRIX, False)
-        else:
-            self.grid_model_part.ProcessInfo.SetValue(KratosMultiphysics.COMPUTE_LUMPED_MASS_MATRIX, True)
-        if analysis_type == "non_linear":
-                solution_strategy = self._CreateNewtonRaphsonStrategy()
-        elif analysis_type == 'linear':
-                self.material_point_model_part.ProcessInfo.SetValue(KratosMPM.IGNORE_GEOMETRIC_STIFFNESS, True)
-                solution_strategy = self._CreateLinearStrategy();
-        else:
-            err_msg =  "The requested implicit analysis type \"" + analysis_type + "\" is not available!\n"
-            err_msg += "Available implicit options are: \"linear\", \"non_linear\""
-            raise Exception(err_msg)
-        return solution_strategy
-
-    def _CreateNewtonRaphsonStrategy(self):
-        computing_model_part = self.GetComputingModelPart()
-        solution_scheme = self._GetSolutionScheme()
-        convergence_criterion = self._GetConvergenceCriteria()
-        builder_and_solver = self._GetBuilderAndSolver()
-        reform_dofs_at_each_step = False ## hard-coded, but can be changed upon implementation
-        return KratosMPM.MPMResidualBasedNewtonRaphsonStrategy(computing_model_part,
-                                                                        solution_scheme,
-                                                                        convergence_criterion,
-                                                                        builder_and_solver,
-                                                                        self.settings["max_iteration"].GetInt(),
-                                                                        self.settings["compute_reactions"].GetBool(),
-                                                                        reform_dofs_at_each_step,
-                                                                        self.settings["move_mesh_flag"].GetBool())
-
-    def _CreateLinearStrategy(self):
-        computing_model_part = self.GetComputingModelPart()
-        solution_scheme = self._GetSolutionScheme()
-        linear_solver = self._GetLinearSolver()
-        reform_dofs_at_each_step = False ## hard-coded, but can be changed upon implementation
-        calc_norm_dx_flag = False ## hard-coded, but can be changed upon implementation
-        return KratosMultiphysics.ResidualBasedLinearStrategy(computing_model_part,
-                                                              solution_scheme,
-                                                              linear_solver,
-                                                              self.settings["compute_reactions"].GetBool(),
-                                                              reform_dofs_at_each_step,
-                                                              calc_norm_dx_flag,
-                                                              self.settings["move_mesh_flag"].GetBool())
-
-    def _SetAndFillBuffer(self):
-        delta_time = self.material_point_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-        if not self.is_restarted():
-            required_buffer_size = self.GetMinimumBufferSize()
-            auxiliary_solver_utilities.SetAndFillBuffer(self.material_point_model_part, required_buffer_size, delta_time)
-            auxiliary_solver_utilities.SetAndFillBuffer(self.grid_model_part, required_buffer_size, delta_time)
-        else:
-            required_buffer_size = self.material_point_model_part.GetBufferSize()
-            auxiliary_solver_utilities.SetAndFillBuffer(self.grid_model_part, required_buffer_size, delta_time)
-
-    ### Solver private functions
-
-    def __ComputeDeltaTime(self):
-        if self.settings["time_stepping"].Has("time_step"):
-            return self.settings["time_stepping"]["time_step"].GetDouble()
-        elif self.settings["time_stepping"].Has("time_step_table"):
-            current_time = self.grid_model_part.ProcessInfo[KratosMultiphysics.TIME]
-            time_step_table = self.settings["time_stepping"]["time_step_table"].GetMatrix()
-            tb = KratosMultiphysics.PiecewiseLinearTable(time_step_table)
-            return tb.GetValue(current_time)
-        else:
-            raise Exception("::[MPMSolver]:: Time stepping not defined!")
-
-    def __ExecuteCheckAndPrepare(self):
-        # Specific active node and element check for MPM solver
-        for node in self.grid_model_part.Nodes:
-            if (node.Is(KratosMultiphysics.ACTIVE)):
-                KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","WARNING: This grid node has been set active: ", node.Id)
-
-        if not self.is_restarted():
-            # Setting active initial elements
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.ACTIVE, True, self.initial_mesh_model_part.Elements)
-
-            # Read material property
-            materials_imported = self.__ImportConstitutiveLaws()
-            if materials_imported:
-                KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","Constitutive law was successfully imported.")
-            else:
-                KratosMultiphysics.Logger.PrintWarning("::[MPMSolver]:: ","Constitutive law was not imported.")
-
-            # Clone property of model_part2 to model_part3
-            self.material_point_model_part.Properties = self.initial_mesh_model_part.Properties
-        else:
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.ACTIVE, True, self.material_point_model_part.Elements)
-
-    def __ImportConstitutiveLaws(self):
-        materials_filename = self.settings["material_import_settings"]["materials_filename"].GetString()
-        if (materials_filename != ""):
-            # Change deprecated parameter
-            with open(materials_filename, 'r') as parameter_file:
-                materials_parameters = KratosMultiphysics.Parameters(parameter_file.read())
-            has_deprecated_param = False
-            for param in materials_parameters["properties"].values():
-                settings = param["Material"]["Variables"]
-                old_name = "PARTICLES_PER_ELEMENT"
-                new_name = "MATERIAL_POINTS_PER_ELEMENT"
-                if DeprecationManager.HasDeprecatedVariable("", settings, old_name, new_name):
-                    DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-                    has_deprecated_param = True
-            if has_deprecated_param:
-                with open(materials_filename,'w') as parameter_file:
-                    parameter_file.write(materials_parameters.WriteJsonString())
-            # Add constitutive laws and material properties from json file to model parts.
-            material_settings = KratosMultiphysics.Parameters("""{"Parameters": {"materials_filename": ""}} """)
-            material_settings["Parameters"]["materials_filename"].SetString(materials_filename)
-            KratosMultiphysics.ReadMaterialsUtility(material_settings, self.model)
-            materials_imported = True
-        else:
-            materials_imported = False
-        return materials_imported
-
-    def is_restarted(self):
-        # this function avoids the long call to ProcessInfo and is also safer
-        # in case the detection of a restart is changed later
-        return self.material_point_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications and dependencies
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+# Importing the base class
+from KratosMultiphysics.python_solver import PythonSolver
+
+# Other imports
+from KratosMultiphysics import auxiliary_solver_utilities
+from KratosMultiphysics import python_linear_solver_factory as linear_solver_factory
+from KratosMultiphysics.deprecation_management import DeprecationManager
+
+def CreateSolver(model, custom_settings):
+    return MPMSolver(model, custom_settings)
+
+class MPMSolver(PythonSolver):
+
+    ### Solver constructor
+    def __init__(self, model, custom_settings):
+        self._validate_settings_in_baseclass=True # To be removed eventually
+        super(MPMSolver, self).__init__(model, custom_settings)
+
+        # Add model part containers
+        self._AddModelPartContainers()
+
+        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ", "Solver is constructed correctly.")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""
+        {
+            "model_part_name" : "MPM_Material",
+            "domain_size"     : -1,
+            "echo_level"      : 0,
+            "time_stepping"   : { },
+            "time_integration_method"   : "implicit",
+            "analysis_type"   : "non_linear",
+            "grid_model_import_settings" : {
+                "input_type"     : "mdpa",
+                "input_filename" : "unknown_name_Grid"
+            },
+            "model_import_settings" : {
+                "input_type"        : "mdpa",
+                "input_filename"    : "unknown_name_Body"
+            },
+            "material_import_settings" : {
+                "materials_filename" : ""
+            },
+            "compute_reactions"                  : false,
+            "convergence_criterion"              : "Residual_criteria",
+            "displacement_relative_tolerance"    : 1.0E-4,
+            "displacement_absolute_tolerance"    : 1.0E-9,
+            "residual_relative_tolerance"        : 1.0E-4,
+            "residual_absolute_tolerance"        : 1.0E-9,
+            "max_iteration"                      : 20,
+            "pressure_dofs"                      : false,
+            "stabilization"                      : "ppp",
+            "compressible"                       : true,
+            "axis_symmetric_flag"                : false,
+            "consistent_mass_matrix"             : false,
+            "block_builder"                      : true,
+            "move_mesh_flag"                     : false,
+            "problem_domain_sub_model_part_list" : [],
+            "processes_sub_model_part_list"      : [],
+            "auxiliary_variables_list"           : [],
+            "auxiliary_dofs_list"                : [],
+            "auxiliary_reaction_list"            : [],
+            "element_search_settings"            : {
+                "search_algorithm_type"          : "bin_based",
+                "max_number_of_results"          : 1000,
+                "searching_tolerance"            : 1.0E-5,
+                "remove_entities_not_found"      : true
+            },
+            "linear_solver_settings"             : {
+                "solver_type" : "amgcl",
+                "smoother_type":"damped_jacobi",
+                "krylov_type": "cg",
+                "coarsening_type": "aggregation",
+                "max_iteration": 200,
+                "provide_coordinates": false,
+                "gmres_krylov_space_dimension": 100,
+                "verbosity" : 0,
+                "tolerance": 1e-7,
+                "scaling": false,
+                "block_size": 3,
+                "use_block_matrices_if_possible" : true,
+                "coarse_enough" : 50
+            }
+        }""")
+        this_defaults.AddMissingParameters(super(MPMSolver, cls).GetDefaultParameters())
+        return this_defaults
+
+    ### Solver public functions
+
+    def GetMinimumBufferSize(self):
+        return 2
+
+    def AddVariables(self):
+        # Add variables to background grid model part
+        self._AddVariablesToModelPart(self.grid_model_part)
+
+        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ", "Variables are added.")
+
+    def ImportModelPart(self):
+        # Read model part
+        self._ModelPartReading()
+
+        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","Models are imported.")
+
+    def PrepareModelPart(self):
+        # Set buffer size
+        self._SetAndFillBuffer()
+
+        # Executes the check and prepare model process
+        self.__ExecuteCheckAndPrepare()
+
+        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ", "ModelPart prepared for Solver.")
+
+    def GetComputingModelPart(self):
+        if not self.model.HasModelPart(self.settings["model_part_name"].GetString()):
+            raise Exception("The ComputingModelPart was not created yet!")
+        return self.model.GetModelPart(self.settings["model_part_name"].GetString())
+
+    def GetGridModelPart(self):
+        if not self.model.HasModelPart("Background_Grid"):
+            raise Exception("The GridModelPart was not created yet!")
+        return self.model.GetModelPart("Background_Grid")
+
+    def AddDofs(self):
+        # Add dofs to background grid model part
+        self._AddDofsToModelPart(self.grid_model_part)
+
+        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","DOFs are added.")
+
+    def Initialize(self):
+        # The material point solution strategy is created here if it does not already exist.
+        material_point_solution_strategy = self._GetSolutionStrategy()
+        material_point_solution_strategy.SetEchoLevel(self.settings["echo_level"].GetInt())
+
+        # Generate material points
+        self._GenerateMaterialPoint()
+
+        KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","Solver is initialized correctly.")
+
+    def AdvanceInTime(self, current_time):
+        dt = self.__ComputeDeltaTime()
+        new_time = current_time + dt
+        self.grid_model_part.ProcessInfo[KratosMultiphysics.STEP] += 1
+        self.grid_model_part.CloneTimeStep(new_time)
+
+        return new_time
+
+    def InitializeSolutionStep(self):
+        self._SearchElement()
+        self._GetSolutionStrategy().Initialize()
+
+        #clean nodal values and map from MPs to nodes
+        self._GetSolutionStrategy().InitializeSolutionStep()
+
+    def Predict(self):
+        self._GetSolutionStrategy().Predict()
+
+    def SolveSolutionStep(self):
+        # Calc residual, update momenta
+        is_converged = self._GetSolutionStrategy().SolveSolutionStep()
+        return is_converged
+
+    def FinalizeSolutionStep(self):
+        self._GetSolutionStrategy().FinalizeSolutionStep()
+
+        self._GetSolutionStrategy().Clear()
+
+        if self.is_restarted():
+            self.material_point_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED] = False
+
+    def Check(self):
+        self._GetSolutionStrategy().Check()
+
+    def Clear(self):
+        self._GetSolutionStrategy().Clear()
+
+    ### Solver special protected functions
+
+    def _GetSolutionScheme(self):
+        if not hasattr(self, '_solution_scheme'):
+            self._solution_scheme = self._CreateSolutionScheme()
+        return self._solution_scheme
+
+    def _GetConvergenceCriteria(self):
+        if not hasattr(self, '_convergence_criterion'):
+            self._convergence_criterion = self._CreateConvergenceCriteria()
+        return self._convergence_criterion
+
+    def _GetLinearSolver(self):
+        if not hasattr(self, '_linear_solver'):
+            self._linear_solver = self._CreateLinearSolver()
+        return self._linear_solver
+
+    def _GetBuilderAndSolver(self):
+        if not hasattr(self, '_builder_and_solver'):
+            self._builder_and_solver = self._CreateBuilderAndSolver()
+        return self._builder_and_solver
+
+    def _GetSolutionStrategy(self):
+        if not hasattr(self, '_solution_strategy'):
+            self._solution_strategy = self._CreateSolutionStrategy()
+        return self._solution_strategy
+
+    ### Solver protected functions
+
+    def _GenerateMaterialPoint(self):
+        pressure_dofs          = self.settings["pressure_dofs"].GetBool()
+        axis_symmetric_flag    = self.settings["axis_symmetric_flag"].GetBool()
+        if axis_symmetric_flag:
+            self.grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_AXISYMMETRIC, True)
+        else:
+            self.grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_AXISYMMETRIC, False)
+        stabilization          = self.settings["stabilization"].GetString()
+        if pressure_dofs:
+            if (stabilization=="none"):
+                stabilization_type = 0
+                KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","WARNING: No stabilization considered for a mixed formulation.")
+            elif (stabilization =="ppp"): #Polynomial Pressure Projection stabilization
+                stabilization_type = 1
+            self.grid_model_part.ProcessInfo.SetValue(KratosMPM.STABILIZATION_TYPE, stabilization_type)
+
+        # Assigning extra information to the main model part
+        self.material_point_model_part.SetNodes(self.grid_model_part.GetNodes())
+
+        if not self.is_restarted():
+            self.material_point_model_part.ProcessInfo = self.grid_model_part.ProcessInfo
+
+            # Generate MP Element and Condition
+            KratosMPM.GenerateMaterialPointElement(self.grid_model_part, self.initial_mesh_model_part, self.material_point_model_part, pressure_dofs)
+            KratosMPM.GenerateMaterialPointCondition(self.grid_model_part, self.initial_mesh_model_part, self.material_point_model_part)
+        else:
+            self.grid_model_part.ProcessInfo = self.material_point_model_part.ProcessInfo
+
+    def _SearchElement(self):
+        searching_alg_type = self.settings["element_search_settings"]["search_algorithm_type"].GetString()
+        max_number_of_search_results = self.settings["element_search_settings"]["max_number_of_results"].GetInt()
+        searching_tolerance          = self.settings["element_search_settings"]["searching_tolerance"].GetDouble()
+        if (searching_alg_type == "bin_based"):
+            KratosMPM.SearchElement(self.grid_model_part, self.material_point_model_part, max_number_of_search_results, searching_tolerance)
+        else:
+            err_msg  = "The requested searching algorithm \"" + searching_alg_type
+            err_msg += "\" is not available for MPMApplication!\n"
+            err_msg += "Available options are: \"bin_based\""
+            raise Exception(err_msg)
+        remove_entities_not_found = self.settings["element_search_settings"]["remove_entities_not_found"].GetBool()
+        if remove_entities_not_found: KratosMPM.MaterialPointEraseProcess(self.material_point_model_part).Execute()
+
+    def _AddModelPartContainers(self):
+        domain_size = self._GetDomainSize()
+        if domain_size not in [2,3]:
+            err_msg  = "The input \"domain_size\" is wrong!"
+            err_msg += "Available options are: \"2\" or \"3\""
+            raise Exception(err_msg)
+
+        ## In MPM three model parts are needed
+        # Material model part definition
+        material_point_model_part_name = self.settings["model_part_name"].GetString()
+        if not self.model.HasModelPart(material_point_model_part_name):
+            self.material_point_model_part = self.model.CreateModelPart(material_point_model_part_name) # Equivalent to model_part3 in the old format
+            self.material_point_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
+
+        # Grid model part definition
+        if not self.model.HasModelPart("Background_Grid"):
+            self.grid_model_part = self.model.CreateModelPart("Background_Grid") #Equivalent to model_part1 in the old format
+            self.grid_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
+
+        if not self.is_restarted():
+            # Initial material model part definition
+            initial_mesh_model_part_name = "Initial_" + material_point_model_part_name
+            if not self.model.HasModelPart(initial_mesh_model_part_name):
+                self.initial_mesh_model_part = self.model.CreateModelPart(initial_mesh_model_part_name) #Equivalent to model_part2 in the old format
+                self.initial_mesh_model_part.ProcessInfo.SetValue(KratosMultiphysics.DOMAIN_SIZE, domain_size)
+
+
+    def _AddVariablesToModelPart(self, model_part):
+        # Add displacements and reaction
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.REACTION)
+
+        # Add specific variables for the problem conditions
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.PRESSURE)
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.POSITIVE_FACE_PRESSURE)
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VOLUME_ACCELERATION)
+
+        # MPM specific nodal variables
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NODAL_MASS)
+        model_part.AddNodalSolutionStepVariable(KratosMPM.NODAL_MOMENTUM)
+        model_part.AddNodalSolutionStepVariable(KratosMPM.NODAL_INERTIA)
+
+        # Add variables that the user defined in the ProjectParameters
+        auxiliary_solver_utilities.AddVariables(model_part, self.settings["auxiliary_variables_list"])
+
+        # Add variables for specific cases
+        if self.settings["pressure_dofs"].GetBool():
+            # add specific variables for the problem (pressure dofs)
+            model_part.AddNodalSolutionStepVariable(KratosMPM.PRESSURE_REACTION)
+            model_part.AddNodalSolutionStepVariable(KratosMPM.NODAL_MPRESSURE)
+
+    def _AddDynamicVariables(self, model_part):
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        model_part.AddNodalSolutionStepVariable(KratosMultiphysics.ACCELERATION)
+
+    def _ModelPartReading(self):
+        # reading the model part of the background grid
+        if(self.settings["grid_model_import_settings"]["input_type"].GetString() == "mdpa"):
+            self._ImportModelPart(self.grid_model_part, self.settings["grid_model_import_settings"])
+        else:
+            raise Exception("Other input options are not implemented yet.")
+
+        # reading the model part of the material point
+        if(self.settings["model_import_settings"]["input_type"].GetString() == "mdpa"):
+            self._ImportModelPart(self.initial_mesh_model_part, self.settings["model_import_settings"])
+        elif(self.settings["model_import_settings"]["input_type"].GetString() == "rest"):
+            self.settings["model_import_settings"]["input_filename"].SetString("MPM_Material")
+            self._ImportModelPart(self.material_point_model_part, self.settings["model_import_settings"])
+        else:
+            raise Exception("Other input options are not implemented yet.")
+
+    def _AddDofsToModelPart(self, model_part):
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_X, KratosMultiphysics.REACTION_X, model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Y, KratosMultiphysics.REACTION_Y, model_part)
+        KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.DISPLACEMENT_Z, KratosMultiphysics.REACTION_Z, model_part)
+
+        if self.settings["pressure_dofs"].GetBool():
+            KratosMultiphysics.VariableUtils().AddDof(KratosMultiphysics.PRESSURE, KratosMPM.PRESSURE_REACTION, model_part)
+
+        # Add dofs that the user defined in the ProjectParameters
+        auxiliary_solver_utilities.AddDofs(model_part, self.settings["auxiliary_dofs_list"], self.settings["auxiliary_reaction_list"])
+
+    def _GetDomainSize(self):
+        if not hasattr(self, '_domain_size'):
+            self._domain_size = self.settings["domain_size"].GetInt()
+        return self._domain_size
+
+    def _GetConvergenceCriteriaSettings(self):
+        # Create an auxiliary Kratos parameters object to store the convergence settings.
+        conv_params = KratosMultiphysics.Parameters("{}")
+        conv_params.AddValue("convergence_criterion",self.settings["convergence_criterion"])
+        conv_params.AddValue("echo_level",self.settings["echo_level"])
+        conv_params.AddValue("displacement_relative_tolerance",self.settings["displacement_relative_tolerance"])
+        conv_params.AddValue("displacement_absolute_tolerance",self.settings["displacement_absolute_tolerance"])
+        conv_params.AddValue("residual_relative_tolerance",self.settings["residual_relative_tolerance"])
+        conv_params.AddValue("residual_absolute_tolerance",self.settings["residual_absolute_tolerance"])
+
+        return conv_params
+
+    def _CreateConvergenceCriteria(self):
+        convergence_criterion_parameters = self._GetConvergenceCriteriaSettings()
+        if (convergence_criterion_parameters["convergence_criterion"].GetString() == "residual_criterion"):
+            R_RT = convergence_criterion_parameters["residual_relative_tolerance"].GetDouble()
+            R_AT = convergence_criterion_parameters["residual_absolute_tolerance"].GetDouble()
+            convergence_criterion = KratosMultiphysics.ResidualCriteria(R_RT, R_AT)
+            convergence_criterion.SetEchoLevel(convergence_criterion_parameters["echo_level"].GetInt())
+        elif (convergence_criterion_parameters["convergence_criterion"].GetString() == "displacement_criterion"):
+            D_RT = convergence_criterion_parameters["displacement_relative_tolerance"].GetDouble()
+            D_AT = convergence_criterion_parameters["displacement_absolute_tolerance"].GetDouble()
+            convergence_criterion = KratosMultiphysics.DisplacementCriteria(D_RT, D_AT)
+            convergence_criterion.SetEchoLevel(convergence_criterion_parameters["echo_level"].GetInt())
+        else:
+            err_msg  = "The requested convergence criteria \"" + convergence_criterion_parameters["convergence_criterion"].GetString()
+            err_msg += "\" is not supported for MPMApplication!\n"
+            err_msg += "Available options are: \"residual_criterion\" or \"displacement_criterion\""
+            raise Exception(err_msg)
+
+        return convergence_criterion
+
+    def _CreateLinearSolver(self):
+        linear_solver_configuration = self.settings["linear_solver_settings"]
+        if linear_solver_configuration.Has("solver_type"): # user specified a linear solver
+            return linear_solver_factory.ConstructSolver(linear_solver_configuration)
+        else:
+            KratosMultiphysics.Logger.PrintInfo('::[MPMSolver]:: No linear solver was specified, using fastest available solver')
+            return linear_solver_factory.CreateFastestAvailableDirectLinearSolver()
+
+    def _CreateBuilderAndSolver(self):
+        linear_solver = self._GetLinearSolver()
+        if self.settings["block_builder"].GetBool():
+            builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(linear_solver)
+        else:
+            builder_and_solver = KratosMultiphysics.ResidualBasedEliminationBuilderAndSolver(linear_solver)
+        return builder_and_solver
+
+    def _CreateSolutionScheme(self):
+        """Create the solution scheme for interested problem."""
+        raise Exception("Solution Scheme creation must be implemented in the derived class.")
+
+    def _CreateSolutionStrategy(self):
+        # this is for implicit only. explicit is implemented in derived mpm_explicit_solver
+        grid_model_part = self.GetGridModelPart();
+        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT, False)
+        analysis_type = self.settings["analysis_type"].GetString()
+        is_consistent_mass_matrix = self.settings["consistent_mass_matrix"].GetBool()
+        if is_consistent_mass_matrix:
+            self.grid_model_part.ProcessInfo.SetValue(KratosMultiphysics.COMPUTE_LUMPED_MASS_MATRIX, False)
+        else:
+            self.grid_model_part.ProcessInfo.SetValue(KratosMultiphysics.COMPUTE_LUMPED_MASS_MATRIX, True)
+        if analysis_type == "non_linear":
+                solution_strategy = self._CreateNewtonRaphsonStrategy()
+        elif analysis_type == 'linear':
+                self.material_point_model_part.ProcessInfo.SetValue(KratosMPM.IGNORE_GEOMETRIC_STIFFNESS, True)
+                solution_strategy = self._CreateLinearStrategy();
+        else:
+            err_msg =  "The requested implicit analysis type \"" + analysis_type + "\" is not available!\n"
+            err_msg += "Available implicit options are: \"linear\", \"non_linear\""
+            raise Exception(err_msg)
+        return solution_strategy
+
+    def _CreateNewtonRaphsonStrategy(self):
+        computing_model_part = self.GetComputingModelPart()
+        solution_scheme = self._GetSolutionScheme()
+        convergence_criterion = self._GetConvergenceCriteria()
+        builder_and_solver = self._GetBuilderAndSolver()
+        reform_dofs_at_each_step = False ## hard-coded, but can be changed upon implementation
+        return KratosMPM.MPMResidualBasedNewtonRaphsonStrategy(computing_model_part,
+                                                                        solution_scheme,
+                                                                        convergence_criterion,
+                                                                        builder_and_solver,
+                                                                        self.settings["max_iteration"].GetInt(),
+                                                                        self.settings["compute_reactions"].GetBool(),
+                                                                        reform_dofs_at_each_step,
+                                                                        self.settings["move_mesh_flag"].GetBool())
+
+    def _CreateLinearStrategy(self):
+        computing_model_part = self.GetComputingModelPart()
+        solution_scheme = self._GetSolutionScheme()
+        linear_solver = self._GetLinearSolver()
+        reform_dofs_at_each_step = False ## hard-coded, but can be changed upon implementation
+        calc_norm_dx_flag = False ## hard-coded, but can be changed upon implementation
+        return KratosMultiphysics.ResidualBasedLinearStrategy(computing_model_part,
+                                                              solution_scheme,
+                                                              linear_solver,
+                                                              self.settings["compute_reactions"].GetBool(),
+                                                              reform_dofs_at_each_step,
+                                                              calc_norm_dx_flag,
+                                                              self.settings["move_mesh_flag"].GetBool())
+
+    def _SetAndFillBuffer(self):
+        delta_time = self.material_point_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+        if not self.is_restarted():
+            required_buffer_size = self.GetMinimumBufferSize()
+            auxiliary_solver_utilities.SetAndFillBuffer(self.material_point_model_part, required_buffer_size, delta_time)
+            auxiliary_solver_utilities.SetAndFillBuffer(self.grid_model_part, required_buffer_size, delta_time)
+        else:
+            required_buffer_size = self.material_point_model_part.GetBufferSize()
+            auxiliary_solver_utilities.SetAndFillBuffer(self.grid_model_part, required_buffer_size, delta_time)
+
+    ### Solver private functions
+
+    def __ComputeDeltaTime(self):
+        if self.settings["time_stepping"].Has("time_step"):
+            return self.settings["time_stepping"]["time_step"].GetDouble()
+        elif self.settings["time_stepping"].Has("time_step_table"):
+            current_time = self.grid_model_part.ProcessInfo[KratosMultiphysics.TIME]
+            time_step_table = self.settings["time_stepping"]["time_step_table"].GetMatrix()
+            tb = KratosMultiphysics.PiecewiseLinearTable(time_step_table)
+            return tb.GetValue(current_time)
+        else:
+            raise Exception("::[MPMSolver]:: Time stepping not defined!")
+
+    def __ExecuteCheckAndPrepare(self):
+        # Specific active node and element check for MPM solver
+        for node in self.grid_model_part.Nodes:
+            if (node.Is(KratosMultiphysics.ACTIVE)):
+                KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","WARNING: This grid node has been set active: ", node.Id)
+
+        if not self.is_restarted():
+            # Setting active initial elements
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.ACTIVE, True, self.initial_mesh_model_part.Elements)
+
+            # Read material property
+            materials_imported = self.__ImportConstitutiveLaws()
+            if materials_imported:
+                KratosMultiphysics.Logger.PrintInfo("::[MPMSolver]:: ","Constitutive law was successfully imported.")
+            else:
+                KratosMultiphysics.Logger.PrintWarning("::[MPMSolver]:: ","Constitutive law was not imported.")
+
+            # Clone property of model_part2 to model_part3
+            self.material_point_model_part.Properties = self.initial_mesh_model_part.Properties
+        else:
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.ACTIVE, True, self.material_point_model_part.Elements)
+
+    def __ImportConstitutiveLaws(self):
+        materials_filename = self.settings["material_import_settings"]["materials_filename"].GetString()
+        if (materials_filename != ""):
+            # Change deprecated parameter
+            with open(materials_filename, 'r') as parameter_file:
+                materials_parameters = KratosMultiphysics.Parameters(parameter_file.read())
+            has_deprecated_param = False
+            for param in materials_parameters["properties"].values():
+                settings = param["Material"]["Variables"]
+                old_name = "PARTICLES_PER_ELEMENT"
+                new_name = "MATERIAL_POINTS_PER_ELEMENT"
+                if DeprecationManager.HasDeprecatedVariable("", settings, old_name, new_name):
+                    DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+                    has_deprecated_param = True
+            if has_deprecated_param:
+                with open(materials_filename,'w') as parameter_file:
+                    parameter_file.write(materials_parameters.WriteJsonString())
+            # Add constitutive laws and material properties from json file to model parts.
+            material_settings = KratosMultiphysics.Parameters("""{"Parameters": {"materials_filename": ""}} """)
+            material_settings["Parameters"]["materials_filename"].SetString(materials_filename)
+            KratosMultiphysics.ReadMaterialsUtility(material_settings, self.model)
+            materials_imported = True
+        else:
+            materials_imported = False
+        return materials_imported
+
+    def is_restarted(self):
+        # this function avoids the long call to ProcessInfo and is also safer
+        # in case the detection of a restart is changed later
+        return self.material_point_model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]
```

## KratosMultiphysics/MPMApplication/apply_mpm_3d_rotating_dirichlet_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,141 +1,141 @@
-import KratosMultiphysics
-from KratosMultiphysics.deprecation_management import DeprecationManager
-import KratosMultiphysics.MPMApplication as KratosMPM
-from KratosMultiphysics.MPMApplication.apply_mpm_particle_dirichlet_condition_process import ApplyMPMParticleDirichletConditionProcess
-
-import math
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyMPM3DRotatingDirichletConditionProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ApplyMPM3DRotatingDirichletConditionProcess(ApplyMPMParticleDirichletConditionProcess):
-    def __init__(self, Model, settings ):
-
-        default_parameters = KratosMultiphysics.Parameters( """
-            {
-                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
-                "material_points_per_condition"   : 0,
-                "imposition_type"           : "penalty",
-                "penalty_factor"            : 0,
-                "constrained"               : "fixed",
-                "option"                    : "",
-                "rotation_center"           : [0.0, 0.0, 0.0],
-                "rotation_velocity"         : [0.0, 0.0, 0.0],
-                "compute_rotation_center"   : false,
-                "rotation_option"           : ""
-            }  """ )
-
-        context_string = type(self).__name__
-        old_name = 'particles_per_condition'
-        new_name = 'material_points_per_condition'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        settings.ValidateAndAssignDefaults(default_parameters)
-        self.model = Model
-        self.model_part_name = settings["model_part_name"].GetString()
-
-        # Private process variables
-        self.rotation_center = settings["rotation_center"].GetVector()
-        self.rotation_velocity = settings["rotation_velocity"].GetVector()
-        self.compute_rotation_center = settings["compute_rotation_center"].GetBool()
-        self.rotation_option = settings["rotation_option"].GetString()
-
-        settings.RemoveValue("rotation_center")
-        settings.RemoveValue("rotation_velocity")
-        settings.RemoveValue("compute_rotation_center")
-        settings.RemoveValue("rotation_option")
-
-        # Initiate base class - Dirichlet condition
-        super().__init__(Model, settings)
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        # Get updated model_part
-        if (self.model_part_name.startswith('Background_Grid.')):
-            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
-        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
-        self.model_part = self.model[mpm_material_model_part_name]
-
-        # If compute rotation center automatically is needed
-        if self.compute_rotation_center:
-            self._ComputeCenterRotation()
-
-        # Initial Quaternion, its increment, and rotation_matrix
-        self._InitializeRotationVariables()
-
-    def ExecuteInitializeSolutionStep(self):
-
-        # If compute rotation center automatically is needed and if the center is moved
-        if self.compute_rotation_center and self.rotation_option == "moving_center":
-            self._ComputeCenterRotation()
-
-        # Compute delta quaternion
-        self._ComputeDeltaQuaternion(self.rotation_velocity)
-        
-        self._quaternion = self._quaternion.MultiplyQuaternion(self._delta_quaternion, self._quaternion)
-        
-        # Normalize quaternion
-        self._quaternion.Normalize()
-        
-        # Compute rotation matrix
-        new_rotation_matrix = KratosMultiphysics.Matrix(3,3)
-        self._quaternion.ToRotationMatrix(new_rotation_matrix)
-
-        for mpc in self.model_part.Conditions:
-            # Compute current radius
-            mpc_coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
-            radius = mpc_coord - self.rotation_center
-
-            # Update impose_displacement
-            imposed_disp = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT,self.model_part.ProcessInfo)[0]
-            
-            imposed_disp += new_rotation_matrix * (self._rotation_matrix.transpose() * radius) - radius
-            mpc.SetValuesOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT,[imposed_disp],self.model_part.ProcessInfo)
-
-            # Update normal vector
-            normal = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_NORMAL,self.model_part.ProcessInfo)[0]
-            modified_normal = new_rotation_matrix * (self._rotation_matrix.transpose() * normal)
-            mpc.SetValuesOnIntegrationPoints(KratosMPM.MPC_NORMAL,[modified_normal],self.model_part.ProcessInfo)
-
-
-        # Copy rotation matrix
-        self._rotation_matrix = new_rotation_matrix
-
-    ### Protected functions
-    def _ComputeCenterRotation(self):
-        auto_rc = KratosMultiphysics.Vector(3)
-        for mpc in self.model_part.Conditions:
-            auto_rc += mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
-
-        auto_rc = auto_rc / self.model_part.NumberOfConditions()
-        self.rotation_center = auto_rc
-
-    def _InitializeRotationVariables(self):
-        self._quaternion = KratosMultiphysics.Quaternion()
-        self._quaternion = self._quaternion.Identity()
-        
-        self._delta_quaternion = KratosMultiphysics.Quaternion()
-        self._delta_quaternion = self._delta_quaternion.Identity()
-
-        self._rotation_matrix = KratosMultiphysics.Matrix(3,3)
-        self._rotation_matrix.fill_identity()
-
-    def _ComputeDeltaQuaternion(self, rot_velocity):
-        if (not isinstance(rot_velocity, KratosMultiphysics.Vector)) and rot_velocity.Size() != 3:
-            raise Exception("expected input shall be a KratosMultiphysics.Vector object with size 3")
-
-        omega = math.sqrt(rot_velocity[0]*rot_velocity[0] + rot_velocity[1]*rot_velocity[1] + rot_velocity[2]*rot_velocity[2])
-        if omega < 1.e-12:
-            omega = 1.e-12
-
-        dt = self.model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-        
-        self._delta_quaternion = KratosMultiphysics.Quaternion()
-        self._delta_quaternion.W = math.cos(omega * dt / 2.0)
-        self._delta_quaternion.X = math.sin(omega * dt / 2.0) * rot_velocity[0] / omega
-        self._delta_quaternion.Y = math.sin(omega * dt / 2.0) * rot_velocity[1] / omega
-        self._delta_quaternion.Z = math.sin(omega * dt / 2.0) * rot_velocity[2] / omega
+import KratosMultiphysics
+from KratosMultiphysics.deprecation_management import DeprecationManager
+import KratosMultiphysics.MPMApplication as KratosMPM
+from KratosMultiphysics.MPMApplication.apply_mpm_particle_dirichlet_condition_process import ApplyMPMParticleDirichletConditionProcess
+
+import math
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyMPM3DRotatingDirichletConditionProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ApplyMPM3DRotatingDirichletConditionProcess(ApplyMPMParticleDirichletConditionProcess):
+    def __init__(self, Model, settings ):
+
+        default_parameters = KratosMultiphysics.Parameters( """
+            {
+                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
+                "material_points_per_condition"   : 0,
+                "imposition_type"           : "penalty",
+                "penalty_factor"            : 0,
+                "constrained"               : "fixed",
+                "option"                    : "",
+                "rotation_center"           : [0.0, 0.0, 0.0],
+                "rotation_velocity"         : [0.0, 0.0, 0.0],
+                "compute_rotation_center"   : false,
+                "rotation_option"           : ""
+            }  """ )
+
+        context_string = type(self).__name__
+        old_name = 'particles_per_condition'
+        new_name = 'material_points_per_condition'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        settings.ValidateAndAssignDefaults(default_parameters)
+        self.model = Model
+        self.model_part_name = settings["model_part_name"].GetString()
+
+        # Private process variables
+        self.rotation_center = settings["rotation_center"].GetVector()
+        self.rotation_velocity = settings["rotation_velocity"].GetVector()
+        self.compute_rotation_center = settings["compute_rotation_center"].GetBool()
+        self.rotation_option = settings["rotation_option"].GetString()
+
+        settings.RemoveValue("rotation_center")
+        settings.RemoveValue("rotation_velocity")
+        settings.RemoveValue("compute_rotation_center")
+        settings.RemoveValue("rotation_option")
+
+        # Initiate base class - Dirichlet condition
+        super().__init__(Model, settings)
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        # Get updated model_part
+        if (self.model_part_name.startswith('Background_Grid.')):
+            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
+        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
+        self.model_part = self.model[mpm_material_model_part_name]
+
+        # If compute rotation center automatically is needed
+        if self.compute_rotation_center:
+            self._ComputeCenterRotation()
+
+        # Initial Quaternion, its increment, and rotation_matrix
+        self._InitializeRotationVariables()
+
+    def ExecuteInitializeSolutionStep(self):
+
+        # If compute rotation center automatically is needed and if the center is moved
+        if self.compute_rotation_center and self.rotation_option == "moving_center":
+            self._ComputeCenterRotation()
+
+        # Compute delta quaternion
+        self._ComputeDeltaQuaternion(self.rotation_velocity)
+        
+        self._quaternion = self._quaternion.MultiplyQuaternion(self._delta_quaternion, self._quaternion)
+        
+        # Normalize quaternion
+        self._quaternion.Normalize()
+        
+        # Compute rotation matrix
+        new_rotation_matrix = KratosMultiphysics.Matrix(3,3)
+        self._quaternion.ToRotationMatrix(new_rotation_matrix)
+
+        for mpc in self.model_part.Conditions:
+            # Compute current radius
+            mpc_coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
+            radius = mpc_coord - self.rotation_center
+
+            # Update impose_displacement
+            imposed_disp = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT,self.model_part.ProcessInfo)[0]
+            
+            imposed_disp += new_rotation_matrix * (self._rotation_matrix.transpose() * radius) - radius
+            mpc.SetValuesOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT,[imposed_disp],self.model_part.ProcessInfo)
+
+            # Update normal vector
+            normal = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_NORMAL,self.model_part.ProcessInfo)[0]
+            modified_normal = new_rotation_matrix * (self._rotation_matrix.transpose() * normal)
+            mpc.SetValuesOnIntegrationPoints(KratosMPM.MPC_NORMAL,[modified_normal],self.model_part.ProcessInfo)
+
+
+        # Copy rotation matrix
+        self._rotation_matrix = new_rotation_matrix
+
+    ### Protected functions
+    def _ComputeCenterRotation(self):
+        auto_rc = KratosMultiphysics.Vector(3)
+        for mpc in self.model_part.Conditions:
+            auto_rc += mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
+
+        auto_rc = auto_rc / self.model_part.NumberOfConditions()
+        self.rotation_center = auto_rc
+
+    def _InitializeRotationVariables(self):
+        self._quaternion = KratosMultiphysics.Quaternion()
+        self._quaternion = self._quaternion.Identity()
+        
+        self._delta_quaternion = KratosMultiphysics.Quaternion()
+        self._delta_quaternion = self._delta_quaternion.Identity()
+
+        self._rotation_matrix = KratosMultiphysics.Matrix(3,3)
+        self._rotation_matrix.fill_identity()
+
+    def _ComputeDeltaQuaternion(self, rot_velocity):
+        if (not isinstance(rot_velocity, KratosMultiphysics.Vector)) and rot_velocity.Size() != 3:
+            raise Exception("expected input shall be a KratosMultiphysics.Vector object with size 3")
+
+        omega = math.sqrt(rot_velocity[0]*rot_velocity[0] + rot_velocity[1]*rot_velocity[1] + rot_velocity[2]*rot_velocity[2])
+        if omega < 1.e-12:
+            omega = 1.e-12
+
+        dt = self.model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+        
+        self._delta_quaternion = KratosMultiphysics.Quaternion()
+        self._delta_quaternion.W = math.cos(omega * dt / 2.0)
+        self._delta_quaternion.X = math.sin(omega * dt / 2.0) * rot_velocity[0] / omega
+        self._delta_quaternion.Y = math.sin(omega * dt / 2.0) * rot_velocity[1] / omega
+        self._delta_quaternion.Z = math.sin(omega * dt / 2.0) * rot_velocity[2] / omega
```

## KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_dirichlet_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,118 +1,118 @@
-import KratosMultiphysics
-from KratosMultiphysics.deprecation_management import DeprecationManager
-import KratosMultiphysics.MPMApplication as KratosMPM
-from KratosMultiphysics.MPMApplication.apply_mpm_particle_dirichlet_condition_process import ApplyMPMParticleDirichletConditionProcess
-
-from math import sqrt
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyMPMCouplingInterfaceDirichletConditionProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ApplyMPMCouplingInterfaceDirichletConditionProcess(ApplyMPMParticleDirichletConditionProcess):
-    def __init__(self, Model, settings ):
-
-        default_parameters = KratosMultiphysics.Parameters( """
-            {
-                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
-                "material_points_per_condition"   : 0,
-                "imposition_type"           : "penalty",
-                "penalty_factor"            : 0,
-                "constrained"               : "fixed",
-                "option"                    : "",
-                "is_equal_distributed"      : false
-            }  """ )
-
-        context_string = type(self).__name__
-        old_name = 'particles_per_condition'
-        new_name = 'material_points_per_condition'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        settings.ValidateAndAssignDefaults(default_parameters)
-        self.model = Model
-        self.model_part_name = settings["model_part_name"].GetString()
-
-        # Initiate base class - Dirichlet condition
-        super(ApplyMPMCouplingInterfaceDirichletConditionProcess, self).__init__(Model, settings)
-
-        # Set INTERFACE flag active
-        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self.model_part.Conditions)
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        # Get updated model_part
-        if (self.model_part_name.startswith('Background_Grid.')):
-            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
-        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
-        self.model_part = self.model[mpm_material_model_part_name]
-
-        ### Translate conditions with INTERFACE flag into a new model part "MPM_Coupling_Dirichlet_Interface" responsible for coupling with structure
-        # Create coupling model part
-        if not self.model.HasModelPart("MPM_Coupling_Dirichlet_Interface"):
-            self.model.CreateModelPart("MPM_Coupling_Dirichlet_Interface")
-        self.coupling_model_part = self.model.GetModelPart("MPM_Coupling_Dirichlet_Interface").CreateSubModelPart(self.model_part_name)
-
-        # Prepare coupling model part
-        self._prepare_coupling_model_part(self.coupling_model_part)
-
-        # Create nodes and fill coupling model part
-        for mpc in self.model_part.Conditions:
-            if (mpc.Is(KratosMultiphysics.INTERFACE)):
-                node_id         = mpc.Id
-                node_coordinate = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD, self.model_part.ProcessInfo)[0]
-                coupling_node   = self.coupling_model_part.CreateNewNode(node_id, node_coordinate[0], node_coordinate[1], node_coordinate[2])
-
-                ## Set Displacement and Normal
-                normal = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_NORMAL, self.model_part.ProcessInfo)[0]
-                coupling_node.SetSolutionStepValue(KratosMultiphysics.NORMAL,0,normal)
-
-
-    def ExecuteInitializeSolutionStep(self):
-        ### Clone delta time
-        self.coupling_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME] = self.model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-
-        ### Send displacement from coupling_mp to mp
-        for coupling_node in self.coupling_model_part.Nodes:
-            coupling_id  = coupling_node.Id
-
-            ## IMPOSED DISPLACEMENT
-            total_displacement = coupling_node.GetSolutionStepValue(KratosMultiphysics.DISPLACEMENT,0)
-            old_displacement = self.model_part.GetCondition(coupling_id).CalculateOnIntegrationPoints(KratosMPM.MPC_DISPLACEMENT, self.model_part.ProcessInfo)[0]
-            incremental_displacement = total_displacement - old_displacement
-            self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT, [incremental_displacement], self.model_part.ProcessInfo)
-
-            ## ADD VELOCITY
-            current_velocity = coupling_node.GetSolutionStepValue(KratosMultiphysics.VELOCITY,0)
-            self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.MPC_VELOCITY, [current_velocity], self.model_part.ProcessInfo)
-
-            ## ADD NORMAL
-            normal = coupling_node.GetSolutionStepValue(KratosMultiphysics.NORMAL,0)
-            # Check and see whether the normal is not zero
-            norm_normal = sqrt(normal[0]*normal[0] + normal[1]*normal[1] + normal[2]*normal[2])
-            if norm_normal > 1.e-10:
-                self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.MPC_NORMAL, [normal], self.model_part.ProcessInfo)
-
-
-    def ExecuteFinalizeSolutionStep(self):
-        ### Get contact force from mp to coupling_mp
-        for mpc in self.model_part.Conditions:
-            if (mpc.Is(KratosMultiphysics.INTERFACE)):
-                coupling_id   = mpc.Id
-                contact_force = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_CONTACT_FORCE, self.model_part.ProcessInfo)[0]
-                self.coupling_model_part.GetNode(coupling_id).SetSolutionStepValue(KratosMultiphysics.CONTACT_FORCE,0,contact_force)
-
-
-    # Local functions
-    def _prepare_coupling_model_part(self, coupling_model_part):
-        # Define domain size
-        domain_size = self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-        coupling_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE] = domain_size
-
-        # Add variables
-        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONTACT_FORCE)
-        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NORMAL)
+import KratosMultiphysics
+from KratosMultiphysics.deprecation_management import DeprecationManager
+import KratosMultiphysics.MPMApplication as KratosMPM
+from KratosMultiphysics.MPMApplication.apply_mpm_particle_dirichlet_condition_process import ApplyMPMParticleDirichletConditionProcess
+
+from math import sqrt
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyMPMCouplingInterfaceDirichletConditionProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ApplyMPMCouplingInterfaceDirichletConditionProcess(ApplyMPMParticleDirichletConditionProcess):
+    def __init__(self, Model, settings ):
+
+        default_parameters = KratosMultiphysics.Parameters( """
+            {
+                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
+                "material_points_per_condition"   : 0,
+                "imposition_type"           : "penalty",
+                "penalty_factor"            : 0,
+                "constrained"               : "fixed",
+                "option"                    : "",
+                "is_equal_distributed"      : false
+            }  """ )
+
+        context_string = type(self).__name__
+        old_name = 'particles_per_condition'
+        new_name = 'material_points_per_condition'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        settings.ValidateAndAssignDefaults(default_parameters)
+        self.model = Model
+        self.model_part_name = settings["model_part_name"].GetString()
+
+        # Initiate base class - Dirichlet condition
+        super(ApplyMPMCouplingInterfaceDirichletConditionProcess, self).__init__(Model, settings)
+
+        # Set INTERFACE flag active
+        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self.model_part.Conditions)
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        # Get updated model_part
+        if (self.model_part_name.startswith('Background_Grid.')):
+            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
+        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
+        self.model_part = self.model[mpm_material_model_part_name]
+
+        ### Translate conditions with INTERFACE flag into a new model part "MPM_Coupling_Dirichlet_Interface" responsible for coupling with structure
+        # Create coupling model part
+        if not self.model.HasModelPart("MPM_Coupling_Dirichlet_Interface"):
+            self.model.CreateModelPart("MPM_Coupling_Dirichlet_Interface")
+        self.coupling_model_part = self.model.GetModelPart("MPM_Coupling_Dirichlet_Interface").CreateSubModelPart(self.model_part_name)
+
+        # Prepare coupling model part
+        self._prepare_coupling_model_part(self.coupling_model_part)
+
+        # Create nodes and fill coupling model part
+        for mpc in self.model_part.Conditions:
+            if (mpc.Is(KratosMultiphysics.INTERFACE)):
+                node_id         = mpc.Id
+                node_coordinate = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD, self.model_part.ProcessInfo)[0]
+                coupling_node   = self.coupling_model_part.CreateNewNode(node_id, node_coordinate[0], node_coordinate[1], node_coordinate[2])
+
+                ## Set Displacement and Normal
+                normal = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_NORMAL, self.model_part.ProcessInfo)[0]
+                coupling_node.SetSolutionStepValue(KratosMultiphysics.NORMAL,0,normal)
+
+
+    def ExecuteInitializeSolutionStep(self):
+        ### Clone delta time
+        self.coupling_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME] = self.model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+
+        ### Send displacement from coupling_mp to mp
+        for coupling_node in self.coupling_model_part.Nodes:
+            coupling_id  = coupling_node.Id
+
+            ## IMPOSED DISPLACEMENT
+            total_displacement = coupling_node.GetSolutionStepValue(KratosMultiphysics.DISPLACEMENT,0)
+            old_displacement = self.model_part.GetCondition(coupling_id).CalculateOnIntegrationPoints(KratosMPM.MPC_DISPLACEMENT, self.model_part.ProcessInfo)[0]
+            incremental_displacement = total_displacement - old_displacement
+            self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.MPC_IMPOSED_DISPLACEMENT, [incremental_displacement], self.model_part.ProcessInfo)
+
+            ## ADD VELOCITY
+            current_velocity = coupling_node.GetSolutionStepValue(KratosMultiphysics.VELOCITY,0)
+            self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.MPC_VELOCITY, [current_velocity], self.model_part.ProcessInfo)
+
+            ## ADD NORMAL
+            normal = coupling_node.GetSolutionStepValue(KratosMultiphysics.NORMAL,0)
+            # Check and see whether the normal is not zero
+            norm_normal = sqrt(normal[0]*normal[0] + normal[1]*normal[1] + normal[2]*normal[2])
+            if norm_normal > 1.e-10:
+                self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.MPC_NORMAL, [normal], self.model_part.ProcessInfo)
+
+
+    def ExecuteFinalizeSolutionStep(self):
+        ### Get contact force from mp to coupling_mp
+        for mpc in self.model_part.Conditions:
+            if (mpc.Is(KratosMultiphysics.INTERFACE)):
+                coupling_id   = mpc.Id
+                contact_force = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_CONTACT_FORCE, self.model_part.ProcessInfo)[0]
+                self.coupling_model_part.GetNode(coupling_id).SetSolutionStepValue(KratosMultiphysics.CONTACT_FORCE,0,contact_force)
+
+
+    # Local functions
+    def _prepare_coupling_model_part(self, coupling_model_part):
+        # Define domain size
+        domain_size = self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+        coupling_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE] = domain_size
+
+        # Add variables
+        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONTACT_FORCE)
+        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.NORMAL)
```

## KratosMultiphysics/MPMApplication/mpm_implicit_dynamic_solver.py

 * *Ordering differences only*

```diff
@@ -1,70 +1,70 @@
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications and dependencies
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-# Importing the base class
-from KratosMultiphysics.MPMApplication.mpm_solver import MPMSolver
-
-def CreateSolver(model, custom_settings):
-    return MPMImplicitDynamicSolver(model, custom_settings)
-
-class MPMImplicitDynamicSolver(MPMSolver):
-
-    def __init__(self, model, custom_settings):
-        # Set defaults and validate custom settings in the base class.
-        # Construct the base solver.
-        super(MPMImplicitDynamicSolver, self).__init__(model, custom_settings)
-        KratosMultiphysics.Logger.PrintInfo("::[MPMImplicitDynamicSolver]:: ", "Construction is finished.")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "scheme_type"   : "bossak",
-            "damp_factor_m" : -0.3,
-            "newmark_beta"  : 0.25
-        }""")
-        this_defaults.AddMissingParameters(super(MPMImplicitDynamicSolver, cls).GetDefaultParameters())
-        return this_defaults
-
-    def AddVariables(self):
-        super(MPMImplicitDynamicSolver, self).AddVariables()
-        self._AddDynamicVariables(self.grid_model_part)
-        KratosMultiphysics.Logger.PrintInfo("::[MPMImplicitDynamicSolver]:: ", "Variables are all added.")
-
-    ### Protected functions ###
-
-    def _CreateSolutionScheme(self):
-        grid_model_part = self.GetGridModelPart()
-        domain_size = self._GetDomainSize()
-        block_size  = domain_size
-        is_mixed_formulation = self.settings["pressure_dofs"].GetBool()
-        self.grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_MIXED_FORMULATION, is_mixed_formulation)
-        if (is_mixed_formulation):
-            block_size += 1
-
-        # Setting the time integration schemes
-        scheme_type = self.settings["scheme_type"].GetString()
-        if(scheme_type == "newmark"):
-            damp_factor_m = 0.0
-            newmark_beta = self.settings["newmark_beta"].GetDouble()
-        elif(scheme_type == "bossak"):
-            damp_factor_m = self.settings["damp_factor_m"].GetDouble()
-            newmark_beta = self.settings["newmark_beta"].GetDouble()
-        else:
-            err_msg = "The requested scheme type \"" + scheme_type + "\" is not available!\n"
-            err_msg += "Available options are: \"newmark\", \"bossak\""
-            raise Exception(err_msg)
-
-        is_dynamic = self._IsDynamic()
-
-        return KratosMPM.MPMResidualBasedBossakScheme( grid_model_part,
-                                                            domain_size,
-                                                            block_size,
-                                                            damp_factor_m,
-                                                            newmark_beta,
-                                                            is_dynamic)
-    def _IsDynamic(self):
-        return True
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications and dependencies
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+# Importing the base class
+from KratosMultiphysics.MPMApplication.mpm_solver import MPMSolver
+
+def CreateSolver(model, custom_settings):
+    return MPMImplicitDynamicSolver(model, custom_settings)
+
+class MPMImplicitDynamicSolver(MPMSolver):
+
+    def __init__(self, model, custom_settings):
+        # Set defaults and validate custom settings in the base class.
+        # Construct the base solver.
+        super(MPMImplicitDynamicSolver, self).__init__(model, custom_settings)
+        KratosMultiphysics.Logger.PrintInfo("::[MPMImplicitDynamicSolver]:: ", "Construction is finished.")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "scheme_type"   : "bossak",
+            "damp_factor_m" : -0.3,
+            "newmark_beta"  : 0.25
+        }""")
+        this_defaults.AddMissingParameters(super(MPMImplicitDynamicSolver, cls).GetDefaultParameters())
+        return this_defaults
+
+    def AddVariables(self):
+        super(MPMImplicitDynamicSolver, self).AddVariables()
+        self._AddDynamicVariables(self.grid_model_part)
+        KratosMultiphysics.Logger.PrintInfo("::[MPMImplicitDynamicSolver]:: ", "Variables are all added.")
+
+    ### Protected functions ###
+
+    def _CreateSolutionScheme(self):
+        grid_model_part = self.GetGridModelPart()
+        domain_size = self._GetDomainSize()
+        block_size  = domain_size
+        is_mixed_formulation = self.settings["pressure_dofs"].GetBool()
+        self.grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_MIXED_FORMULATION, is_mixed_formulation)
+        if (is_mixed_formulation):
+            block_size += 1
+
+        # Setting the time integration schemes
+        scheme_type = self.settings["scheme_type"].GetString()
+        if(scheme_type == "newmark"):
+            damp_factor_m = 0.0
+            newmark_beta = self.settings["newmark_beta"].GetDouble()
+        elif(scheme_type == "bossak"):
+            damp_factor_m = self.settings["damp_factor_m"].GetDouble()
+            newmark_beta = self.settings["newmark_beta"].GetDouble()
+        else:
+            err_msg = "The requested scheme type \"" + scheme_type + "\" is not available!\n"
+            err_msg += "Available options are: \"newmark\", \"bossak\""
+            raise Exception(err_msg)
+
+        is_dynamic = self._IsDynamic()
+
+        return KratosMPM.MPMResidualBasedBossakScheme( grid_model_part,
+                                                            domain_size,
+                                                            block_size,
+                                                            damp_factor_m,
+                                                            newmark_beta,
+                                                            is_dynamic)
+    def _IsDynamic(self):
+        return True
```

## KratosMultiphysics/MPMApplication/kratos_main_mpm.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-
-import KratosMultiphysics
-from KratosMultiphysics.MPMApplication.mpm_analysis import MPMAnalysis
-
-"""
-For user-scripting it is intended that a new class is derived
-from MPMAnalysis to do modifications
-"""
-
-if __name__ == "__main__":
-
-    with open("ProjectParameters.json",'r') as parameter_file:
-        parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-    model = KratosMultiphysics.Model()
-    simulation = MPMAnalysis(model,parameters)
-    simulation.Run()
+
+import KratosMultiphysics
+from KratosMultiphysics.MPMApplication.mpm_analysis import MPMAnalysis
+
+"""
+For user-scripting it is intended that a new class is derived
+from MPMAnalysis to do modifications
+"""
+
+if __name__ == "__main__":
+
+    with open("ProjectParameters.json",'r') as parameter_file:
+        parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+    model = KratosMultiphysics.Model()
+    simulation = MPMAnalysis(model,parameters)
+    simulation.Run()
```

## KratosMultiphysics/MPMApplication/particle_json_output_process.py

 * *Ordering differences only*

```diff
@@ -1,12 +1,12 @@
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-from KratosMultiphysics.MPMApplication.mpm_json_output_process import MPMJsonOutputProcess
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a model object")
-    wrng_msg = "Process `particle_json_output_process` is replaced by `mpm_json_output_process`."
-    IssueDeprecationWarning("MPMApplication:",wrng_msg)
-    return ParticleJsonOutputProcess(model, settings["Parameters"])
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+from KratosMultiphysics.MPMApplication.mpm_json_output_process import MPMJsonOutputProcess
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a model object")
+    wrng_msg = "Process `particle_json_output_process` is replaced by `mpm_json_output_process`."
+    IssueDeprecationWarning("MPMApplication:",wrng_msg)
+    return ParticleJsonOutputProcess(model, settings["Parameters"])
```

## KratosMultiphysics/MPMApplication/mpm_explicit_solver.py

 * *Ordering differences only*

```diff
@@ -1,129 +1,129 @@
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications and dependencies
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-# Importing the base class
-from KratosMultiphysics.MPMApplication.mpm_solver import MPMSolver
-
-def CreateSolver(model, custom_settings):
-    return MPMExplicitSolver(model, custom_settings)
-
-class MPMExplicitSolver(MPMSolver):
-
-    def __init__(self, model, custom_settings):
-        # Set defaults and validate custom settings in the base class.
-        # Construct the base solver.
-        super(MPMExplicitSolver, self).__init__(model, custom_settings)
-        KratosMultiphysics.Logger.PrintInfo("::[MPMExplicitSolver]:: ", "Construction is finished.")
-
-    @classmethod
-    def GetDefaultParameters(cls):
-        this_defaults = KratosMultiphysics.Parameters("""{
-            "time_integration_method"   : "explicit",
-            "scheme_type"   : "central_difference",
-            "stress_update" : "usf",
-            "is_fix_explicit_mp_on_grid_edge" : false,
-            "is_pqmpm"      : false,
-            "is_make_normal_mp_if_pqmpm_fails" : true,
-            "pqmpm_subpoint_min_volume_fraction" : 0.0
-        }""")
-        this_defaults.AddMissingParameters(super(MPMExplicitSolver, cls).GetDefaultParameters())
-        return this_defaults
-
-
-    def AddVariables(self):
-        super(MPMExplicitSolver, self).AddVariables()
-        self._AddDynamicVariables(self.grid_model_part)
-        grid_model_part = self.GetGridModelPart()
-
-        # Adding explicit variables
-        grid_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FORCE_RESIDUAL)
-        grid_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.RESIDUAL_VECTOR)
-
-        KratosMultiphysics.Logger.PrintInfo("::[MPMExplicitSolver]:: ", "Variables are all added.")
-
-    ### Protected functions ###
-
-    def _CreateSolutionScheme(self):
-        grid_model_part = self.GetGridModelPart()
-        domain_size = self._GetDomainSize()
-        block_size  = domain_size
-        if (self.settings["pressure_dofs"].GetBool()):
-            block_size += 1
-
-        # Check whether compressibility is considered
-        is_compressible = self.settings["compressible"].GetBool()
-        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_COMPRESSIBLE, is_compressible)
-
-        # Check whether the partitioned quadrature mpm (PQMPM) is used
-        is_pqmpm = self.settings["is_pqmpm"].GetBool()
-        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_PQMPM, is_pqmpm)
-        is_make_normal_mp_if_pqmpm_fails = self.settings["is_make_normal_mp_if_pqmpm_fails"].GetBool()
-        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_MAKE_NORMAL_MP_IF_PQMPM_FAILS, is_make_normal_mp_if_pqmpm_fails)
-        pqmpm_subpoint_min_volume_fraction = self.settings["pqmpm_subpoint_min_volume_fraction"].GetDouble()
-        grid_model_part.ProcessInfo.SetValue(KratosMPM.PQMPM_SUBPOINT_MIN_VOLUME_FRACTION, pqmpm_subpoint_min_volume_fraction)
-
-        # Check if we are fixing MPs that lie directly on the edge of grid elements
-        if is_pqmpm:
-            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_FIX_EXPLICIT_MP_ON_GRID_EDGE, False)
-        else:
-            is_fix_explicit_mp_on_grid_edge = self.settings["is_fix_explicit_mp_on_grid_edge"].GetBool()
-            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_FIX_EXPLICIT_MP_ON_GRID_EDGE, is_fix_explicit_mp_on_grid_edge)
-
-        # Setting the time integration schemes
-        scheme_type = self.settings["scheme_type"].GetString()
-
-        if scheme_type == "forward_euler":
-            stress_update_option = 10
-            stress_update = self.settings["stress_update"].GetString() #0 = USF, 1 = USL, 2 = MUSL
-            if stress_update == "usf":
-                stress_update_option = 0
-            elif stress_update == "usl":
-                stress_update_option = 1
-            elif stress_update == "musl":
-                stress_update_option = 2
-            else:
-                err_msg = "The requested stress update \"" + stress_update + "\" is not available!\n"
-                err_msg += "Available options are: \"usf\", \"usl\",\"musl\""
-            grid_model_part.ProcessInfo.SetValue(KratosMPM.EXPLICIT_STRESS_UPDATE_OPTION, stress_update_option)
-            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT_CENTRAL_DIFFERENCE, False)
-        elif scheme_type == "central_difference":
-            grid_model_part.ProcessInfo.SetValue(KratosMPM.EXPLICIT_STRESS_UPDATE_OPTION, 0)
-            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT_CENTRAL_DIFFERENCE, True)
-        else:
-            err_msg = "The requested scheme type \"" + scheme_type + "\" is not available!\n"
-            err_msg += "Available options are: \"forward_euler\", \"central_difference\""
-            raise Exception(err_msg)
-
-        return KratosMPM.MPMExplicitScheme( grid_model_part)
-
-    def _CreateSolutionStrategy(self):
-        analysis_type = self.settings["analysis_type"].GetString()
-        if analysis_type == "linear":
-                grid_model_part = self.GetGridModelPart();
-                grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT, True)
-                solution_strategy = self._CreateLinearStrategy()
-        else:
-            err_msg =  "The requested explicit analysis type \"" + analysis_type + "\" is not available!\n"
-            err_msg += "Available explicit options are: \"linear\""
-            raise Exception(err_msg)
-        return solution_strategy
-
-
-    def _CreateLinearStrategy(self):
-        computing_model_part = self.GetComputingModelPart()
-        solution_scheme = self._GetSolutionScheme()
-        reform_dofs_at_each_step = False ## hard-coded, but can be changed upon implementation
-        move_mesh_flag = self.settings["move_mesh_flag"].GetBool()
-        move_mesh_flag = False ## hard-coded
-        return KratosMPM.MPMExplicitStrategy(computing_model_part,
-                                                      solution_scheme,
-                                                      self.settings["compute_reactions"].GetBool(),
-                                                      reform_dofs_at_each_step,
-                                                      move_mesh_flag)
-
-    def _IsDynamic(self):
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications and dependencies
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+# Importing the base class
+from KratosMultiphysics.MPMApplication.mpm_solver import MPMSolver
+
+def CreateSolver(model, custom_settings):
+    return MPMExplicitSolver(model, custom_settings)
+
+class MPMExplicitSolver(MPMSolver):
+
+    def __init__(self, model, custom_settings):
+        # Set defaults and validate custom settings in the base class.
+        # Construct the base solver.
+        super(MPMExplicitSolver, self).__init__(model, custom_settings)
+        KratosMultiphysics.Logger.PrintInfo("::[MPMExplicitSolver]:: ", "Construction is finished.")
+
+    @classmethod
+    def GetDefaultParameters(cls):
+        this_defaults = KratosMultiphysics.Parameters("""{
+            "time_integration_method"   : "explicit",
+            "scheme_type"   : "central_difference",
+            "stress_update" : "usf",
+            "is_fix_explicit_mp_on_grid_edge" : false,
+            "is_pqmpm"      : false,
+            "is_make_normal_mp_if_pqmpm_fails" : true,
+            "pqmpm_subpoint_min_volume_fraction" : 0.0
+        }""")
+        this_defaults.AddMissingParameters(super(MPMExplicitSolver, cls).GetDefaultParameters())
+        return this_defaults
+
+
+    def AddVariables(self):
+        super(MPMExplicitSolver, self).AddVariables()
+        self._AddDynamicVariables(self.grid_model_part)
+        grid_model_part = self.GetGridModelPart()
+
+        # Adding explicit variables
+        grid_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.FORCE_RESIDUAL)
+        grid_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.RESIDUAL_VECTOR)
+
+        KratosMultiphysics.Logger.PrintInfo("::[MPMExplicitSolver]:: ", "Variables are all added.")
+
+    ### Protected functions ###
+
+    def _CreateSolutionScheme(self):
+        grid_model_part = self.GetGridModelPart()
+        domain_size = self._GetDomainSize()
+        block_size  = domain_size
+        if (self.settings["pressure_dofs"].GetBool()):
+            block_size += 1
+
+        # Check whether compressibility is considered
+        is_compressible = self.settings["compressible"].GetBool()
+        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_COMPRESSIBLE, is_compressible)
+
+        # Check whether the partitioned quadrature mpm (PQMPM) is used
+        is_pqmpm = self.settings["is_pqmpm"].GetBool()
+        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_PQMPM, is_pqmpm)
+        is_make_normal_mp_if_pqmpm_fails = self.settings["is_make_normal_mp_if_pqmpm_fails"].GetBool()
+        grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_MAKE_NORMAL_MP_IF_PQMPM_FAILS, is_make_normal_mp_if_pqmpm_fails)
+        pqmpm_subpoint_min_volume_fraction = self.settings["pqmpm_subpoint_min_volume_fraction"].GetDouble()
+        grid_model_part.ProcessInfo.SetValue(KratosMPM.PQMPM_SUBPOINT_MIN_VOLUME_FRACTION, pqmpm_subpoint_min_volume_fraction)
+
+        # Check if we are fixing MPs that lie directly on the edge of grid elements
+        if is_pqmpm:
+            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_FIX_EXPLICIT_MP_ON_GRID_EDGE, False)
+        else:
+            is_fix_explicit_mp_on_grid_edge = self.settings["is_fix_explicit_mp_on_grid_edge"].GetBool()
+            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_FIX_EXPLICIT_MP_ON_GRID_EDGE, is_fix_explicit_mp_on_grid_edge)
+
+        # Setting the time integration schemes
+        scheme_type = self.settings["scheme_type"].GetString()
+
+        if scheme_type == "forward_euler":
+            stress_update_option = 10
+            stress_update = self.settings["stress_update"].GetString() #0 = USF, 1 = USL, 2 = MUSL
+            if stress_update == "usf":
+                stress_update_option = 0
+            elif stress_update == "usl":
+                stress_update_option = 1
+            elif stress_update == "musl":
+                stress_update_option = 2
+            else:
+                err_msg = "The requested stress update \"" + stress_update + "\" is not available!\n"
+                err_msg += "Available options are: \"usf\", \"usl\",\"musl\""
+            grid_model_part.ProcessInfo.SetValue(KratosMPM.EXPLICIT_STRESS_UPDATE_OPTION, stress_update_option)
+            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT_CENTRAL_DIFFERENCE, False)
+        elif scheme_type == "central_difference":
+            grid_model_part.ProcessInfo.SetValue(KratosMPM.EXPLICIT_STRESS_UPDATE_OPTION, 0)
+            grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT_CENTRAL_DIFFERENCE, True)
+        else:
+            err_msg = "The requested scheme type \"" + scheme_type + "\" is not available!\n"
+            err_msg += "Available options are: \"forward_euler\", \"central_difference\""
+            raise Exception(err_msg)
+
+        return KratosMPM.MPMExplicitScheme( grid_model_part)
+
+    def _CreateSolutionStrategy(self):
+        analysis_type = self.settings["analysis_type"].GetString()
+        if analysis_type == "linear":
+                grid_model_part = self.GetGridModelPart();
+                grid_model_part.ProcessInfo.SetValue(KratosMPM.IS_EXPLICIT, True)
+                solution_strategy = self._CreateLinearStrategy()
+        else:
+            err_msg =  "The requested explicit analysis type \"" + analysis_type + "\" is not available!\n"
+            err_msg += "Available explicit options are: \"linear\""
+            raise Exception(err_msg)
+        return solution_strategy
+
+
+    def _CreateLinearStrategy(self):
+        computing_model_part = self.GetComputingModelPart()
+        solution_scheme = self._GetSolutionScheme()
+        reform_dofs_at_each_step = False ## hard-coded, but can be changed upon implementation
+        move_mesh_flag = self.settings["move_mesh_flag"].GetBool()
+        move_mesh_flag = False ## hard-coded
+        return KratosMPM.MPMExplicitStrategy(computing_model_part,
+                                                      solution_scheme,
+                                                      self.settings["compute_reactions"].GetBool(),
+                                                      reform_dofs_at_each_step,
+                                                      move_mesh_flag)
+
+    def _IsDynamic(self):
         return True
```

## KratosMultiphysics/MPMApplication/apply_mpm_particle_neumann_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,169 +1,169 @@
-import KratosMultiphysics
-from KratosMultiphysics.deprecation_management import DeprecationManager
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyMPMParticleNeumannConditionProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ApplyMPMParticleNeumannConditionProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        default_parameters = KratosMultiphysics.Parameters( """
-            {
-                "model_part_name"                 : "PLEASE_SPECIFY_MODEL_PART_NAME",
-                "material_points_per_condition"   : 0,
-                "variable_name"                   : "PLEASE_SPECIFY_LOADING_CONDITION",
-                "modulus"                         : 1.0,
-                "constrained"                     : "fixed",
-                "direction"                       : [0.0, 0.0, 0.0],
-                "interval"                        : [0.0, 1e30],
-                "option"                          : "",
-                "local_axes"                      : {}
-            }  """ )
-
-        # Trick: allow "modulus" and "direction" to be a double or a string value (otherwise the ValidateAndAssignDefaults might fail)
-        if settings.Has("modulus"):
-            if settings["modulus"].IsString():
-                default_parameters["modulus"].SetString("0.0")
-
-        if settings.Has("direction"):
-            if settings["direction"].IsString():
-                default_parameters["direction"].SetString("Automatic")
-
-        # Assign this here since it will change the "interval" prior to validation
-        self.interval = KratosMultiphysics.IntervalUtility(settings)
-
-        context_string = type(self).__name__
-        old_name = 'particles_per_condition'
-        new_name = 'material_points_per_condition'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        settings.ValidateAndAssignDefaults(default_parameters)
-
-        self.model_part = Model[settings["model_part_name"].GetString()]
-        self.model_part_name = settings["model_part_name"].GetString()
-        self.model = Model
-        self.material_points_per_condition = settings["material_points_per_condition"].GetInt()
-        self.is_neumann_boundary = True
-        self.option = settings["option"].GetString()
-
-        # check constraint
-        self.constrained = settings["constrained"].GetString()
-        if (self.constrained == "fixed"):
-            self.normal_following_load = False
-        elif (self.constrained == "normal"):
-            self.normal_following_load = True
-        else:
-            err_msg =  "The requested type of constrain: \"" + self.constrained + "\" is not available!\n"
-            err_msg += "Available options are: \"fixed\" and \"normal\"."
-            raise Exception(err_msg)
-
-        # get variable imposed and check
-        variable_name = settings["variable_name"].GetString()
-        variable_name_list = ["POINT_LOAD","LINE_LOAD","SURFACE_LOAD"]
-        if(variable_name in variable_name_list):
-            self.variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
-        else:
-            err_msg =  "The given variable \"" + variable_name + "\" is not available to be imposed with this process.\n"
-            err_msg += "Available options are: " + ", ".join(variable_name_list)
-            raise Exception(err_msg)
-
-
-        self.vector_direction = KratosMultiphysics.Vector(3)
-        self.aux_function_direction = ["0.0","0.0","0.0"]
-        self.value_direction_is_numeric = [False, False, False]
-        for i in range(3):
-            if settings["direction"][i].IsNumber():
-                self.value_direction_is_numeric[i] = True
-                self.vector_direction[i] = settings["direction"][i].GetDouble()
-            else:
-                self.function_string_direction = settings["direction"][i].GetString()
-                self.aux_function_direction[i] = KratosMultiphysics.GenericFunctionUtility(self.function_string_direction, settings["local_axes"])
-
-
-        self.value_is_numeric = False
-        self.value = KratosMultiphysics.Vector(3)
-        self.aux_function = "0.0"
-
-        if settings["modulus"].IsNumber():
-            self.value_is_numeric = True
-            self.modulus = settings["modulus"].GetDouble()
-            self.value = self.vector_direction * self.modulus
-        else:
-            self.function_string = settings["modulus"].GetString()
-            self.aux_function = KratosMultiphysics.GenericFunctionUtility(self.function_string, settings["local_axes"])
-
-
-        self.modified_normal = False
-
-        # Set Flag BOUNDARY and variables MATERIAL_POINTS_PER_CONDITION
-        if self.material_points_per_condition >= 0:
-            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BOUNDARY, True, self.model_part.Nodes)
-
-            for condition in self.model_part.Conditions:
-                condition.Set(KratosMultiphysics.BOUNDARY, True)
-                condition.Set(KratosMultiphysics.MARKER, self.normal_following_load)
-                condition.Set(KratosMultiphysics.MODIFIED, self.modified_normal)
-                condition.SetValue(KratosMPM.MATERIAL_POINTS_PER_CONDITION, self.material_points_per_condition)
-                condition.SetValue(KratosMPM.MPC_IS_NEUMANN, self.is_neumann_boundary)
-                condition.SetValue(self.variable, self.value)
-        else:
-            err_msg = '\n::[ApplyMPMParticleNeumannConditionProcess]:: W-A-R-N-I-N-G: You have specified invalid "material_points_per_condition", '
-            err_msg += 'or assigned negative values. \nPlease assign: "material_points_per_condition" > 0 or = 0 (for automatic value)!\n'
-            raise Exception(err_msg)
-
-    def ExecuteBeforeSolutionLoop(self):
-        """ This method is executed in before initialize the solution step
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-
-        # Get updated model_part
-        if (self.model_part_name.startswith('Background_Grid.')):
-            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
-        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
-        self.model_part = self.model[mpm_material_model_part_name]
-        self.ExecuteInitializeSolutionStep()
-
-    def ExecuteInitializeSolutionStep(self):
-        """ This method is executed in order to initialize the current step
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-
-        for mpc in self.model_part.Conditions:
-            current_time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
-
-            mpc_coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
-
-
-            if self.interval.IsInInterval(current_time):
-
-                self.step_is_active = True
-
-                for i in range(3):
-                    if not self.value_direction_is_numeric[i]:
-                        if self.aux_function_direction[i].DependsOnSpace() == False: #depends on time only
-                            self.vector_direction[i] = self.aux_function_direction[i].CallFunction(0.0,0.0,0.0,current_time,0.0,0.0,0.0)
-                        else: #most general case - space varying function (possibly also time varying)
-                            self.vector_direction[i]= self.aux_function_direction[i].CallFunction(mpc_coord[0],mpc_coord[1],mpc_coord[2],current_time,0.0,0.0,0.0)
-
-
-                if not self.value_is_numeric:
-                    if self.aux_function.DependsOnSpace() == False: #depends on time only
-                        self.value = self.aux_function.CallFunction(0.0,0.0,0.0,current_time,0.0,0.0,0.0) * self.vector_direction
-                    else: #most general case - space varying function (possibly also time varying)
-                        self.value = self.aux_function.CallFunction(mpc_coord[0],mpc_coord[1],mpc_coord[2],current_time,0.0,0.0,0.0) * self.vector_direction
-                else:
-                    self.value = self.vector_direction * self.modulus
-
-
-                mpc.SetValuesOnIntegrationPoints(KratosMPM.POINT_LOAD,[self.value],self.model_part.ProcessInfo)
-
+import KratosMultiphysics
+from KratosMultiphysics.deprecation_management import DeprecationManager
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyMPMParticleNeumannConditionProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ApplyMPMParticleNeumannConditionProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        default_parameters = KratosMultiphysics.Parameters( """
+            {
+                "model_part_name"                 : "PLEASE_SPECIFY_MODEL_PART_NAME",
+                "material_points_per_condition"   : 0,
+                "variable_name"                   : "PLEASE_SPECIFY_LOADING_CONDITION",
+                "modulus"                         : 1.0,
+                "constrained"                     : "fixed",
+                "direction"                       : [0.0, 0.0, 0.0],
+                "interval"                        : [0.0, 1e30],
+                "option"                          : "",
+                "local_axes"                      : {}
+            }  """ )
+
+        # Trick: allow "modulus" and "direction" to be a double or a string value (otherwise the ValidateAndAssignDefaults might fail)
+        if settings.Has("modulus"):
+            if settings["modulus"].IsString():
+                default_parameters["modulus"].SetString("0.0")
+
+        if settings.Has("direction"):
+            if settings["direction"].IsString():
+                default_parameters["direction"].SetString("Automatic")
+
+        # Assign this here since it will change the "interval" prior to validation
+        self.interval = KratosMultiphysics.IntervalUtility(settings)
+
+        context_string = type(self).__name__
+        old_name = 'particles_per_condition'
+        new_name = 'material_points_per_condition'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        settings.ValidateAndAssignDefaults(default_parameters)
+
+        self.model_part = Model[settings["model_part_name"].GetString()]
+        self.model_part_name = settings["model_part_name"].GetString()
+        self.model = Model
+        self.material_points_per_condition = settings["material_points_per_condition"].GetInt()
+        self.is_neumann_boundary = True
+        self.option = settings["option"].GetString()
+
+        # check constraint
+        self.constrained = settings["constrained"].GetString()
+        if (self.constrained == "fixed"):
+            self.normal_following_load = False
+        elif (self.constrained == "normal"):
+            self.normal_following_load = True
+        else:
+            err_msg =  "The requested type of constrain: \"" + self.constrained + "\" is not available!\n"
+            err_msg += "Available options are: \"fixed\" and \"normal\"."
+            raise Exception(err_msg)
+
+        # get variable imposed and check
+        variable_name = settings["variable_name"].GetString()
+        variable_name_list = ["POINT_LOAD","LINE_LOAD","SURFACE_LOAD"]
+        if(variable_name in variable_name_list):
+            self.variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
+        else:
+            err_msg =  "The given variable \"" + variable_name + "\" is not available to be imposed with this process.\n"
+            err_msg += "Available options are: " + ", ".join(variable_name_list)
+            raise Exception(err_msg)
+
+
+        self.vector_direction = KratosMultiphysics.Vector(3)
+        self.aux_function_direction = ["0.0","0.0","0.0"]
+        self.value_direction_is_numeric = [False, False, False]
+        for i in range(3):
+            if settings["direction"][i].IsNumber():
+                self.value_direction_is_numeric[i] = True
+                self.vector_direction[i] = settings["direction"][i].GetDouble()
+            else:
+                self.function_string_direction = settings["direction"][i].GetString()
+                self.aux_function_direction[i] = KratosMultiphysics.GenericFunctionUtility(self.function_string_direction, settings["local_axes"])
+
+
+        self.value_is_numeric = False
+        self.value = KratosMultiphysics.Vector(3)
+        self.aux_function = "0.0"
+
+        if settings["modulus"].IsNumber():
+            self.value_is_numeric = True
+            self.modulus = settings["modulus"].GetDouble()
+            self.value = self.vector_direction * self.modulus
+        else:
+            self.function_string = settings["modulus"].GetString()
+            self.aux_function = KratosMultiphysics.GenericFunctionUtility(self.function_string, settings["local_axes"])
+
+
+        self.modified_normal = False
+
+        # Set Flag BOUNDARY and variables MATERIAL_POINTS_PER_CONDITION
+        if self.material_points_per_condition >= 0:
+            KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.BOUNDARY, True, self.model_part.Nodes)
+
+            for condition in self.model_part.Conditions:
+                condition.Set(KratosMultiphysics.BOUNDARY, True)
+                condition.Set(KratosMultiphysics.MARKER, self.normal_following_load)
+                condition.Set(KratosMultiphysics.MODIFIED, self.modified_normal)
+                condition.SetValue(KratosMPM.MATERIAL_POINTS_PER_CONDITION, self.material_points_per_condition)
+                condition.SetValue(KratosMPM.MPC_IS_NEUMANN, self.is_neumann_boundary)
+                condition.SetValue(self.variable, self.value)
+        else:
+            err_msg = '\n::[ApplyMPMParticleNeumannConditionProcess]:: W-A-R-N-I-N-G: You have specified invalid "material_points_per_condition", '
+            err_msg += 'or assigned negative values. \nPlease assign: "material_points_per_condition" > 0 or = 0 (for automatic value)!\n'
+            raise Exception(err_msg)
+
+    def ExecuteBeforeSolutionLoop(self):
+        """ This method is executed in before initialize the solution step
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+
+        # Get updated model_part
+        if (self.model_part_name.startswith('Background_Grid.')):
+            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
+        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
+        self.model_part = self.model[mpm_material_model_part_name]
+        self.ExecuteInitializeSolutionStep()
+
+    def ExecuteInitializeSolutionStep(self):
+        """ This method is executed in order to initialize the current step
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+
+        for mpc in self.model_part.Conditions:
+            current_time = self.model_part.ProcessInfo[KratosMultiphysics.TIME]
+
+            mpc_coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
+
+
+            if self.interval.IsInInterval(current_time):
+
+                self.step_is_active = True
+
+                for i in range(3):
+                    if not self.value_direction_is_numeric[i]:
+                        if self.aux_function_direction[i].DependsOnSpace() == False: #depends on time only
+                            self.vector_direction[i] = self.aux_function_direction[i].CallFunction(0.0,0.0,0.0,current_time,0.0,0.0,0.0)
+                        else: #most general case - space varying function (possibly also time varying)
+                            self.vector_direction[i]= self.aux_function_direction[i].CallFunction(mpc_coord[0],mpc_coord[1],mpc_coord[2],current_time,0.0,0.0,0.0)
+
+
+                if not self.value_is_numeric:
+                    if self.aux_function.DependsOnSpace() == False: #depends on time only
+                        self.value = self.aux_function.CallFunction(0.0,0.0,0.0,current_time,0.0,0.0,0.0) * self.vector_direction
+                    else: #most general case - space varying function (possibly also time varying)
+                        self.value = self.aux_function.CallFunction(mpc_coord[0],mpc_coord[1],mpc_coord[2],current_time,0.0,0.0,0.0) * self.vector_direction
+                else:
+                    self.value = self.vector_direction * self.modulus
+
+
+                mpc.SetValuesOnIntegrationPoints(KratosMPM.POINT_LOAD,[self.value],self.model_part.ProcessInfo)
+
```

## KratosMultiphysics/MPMApplication/python_solvers_wrapper_mpm.py

 * *Ordering differences only*

```diff
@@ -1,56 +1,56 @@
-
-import KratosMultiphysics
-from importlib import import_module
-
-def CreateSolverByParameters(model, solver_settings, parallelism):
-
-    solver_type = solver_settings["solver_type"].GetString()
-
-    # Solvers for OpenMP parallelism
-    if (parallelism == "OpenMP"):
-        if (solver_type == "Dynamic" or solver_type == "dynamic"):
-            time_integration_method = solver_settings["time_integration_method"].GetString()
-            if (time_integration_method == "implicit"):
-                solver_module_name = "mpm_implicit_dynamic_solver"
-            elif (time_integration_method == "explicit"):
-                solver_module_name = "mpm_explicit_solver"
-            else:
-                err_msg =  "The requested time integration method \"" + time_integration_method + "\" is not in the python solvers wrapper\n"
-                err_msg += "Available options are: \"implicit\", \"explicit\""
-                raise Exception(err_msg)
-        elif (solver_type == "Quasi-static" or solver_type == "quasi_static"):
-            solver_module_name = "mpm_quasi_static_solver"
-        elif (solver_type == "Static" or solver_type == "static"):
-            solver_module_name = "mpm_static_solver"
-        else:
-            err_msg =  "The requested solver type \"" + solver_type + "\" is not in the python solvers wrapper\n"
-            err_msg += "Available options are: \"static\", \"dynamic\", \"quasi_static\""
-            raise Exception(err_msg)
-
-    else:
-        err_msg =  "The requested parallel type \"" + parallelism + "\" is not available!\n"
-        err_msg += "Available options are: \"OpenMP\""
-        raise Exception(err_msg)
-
-    # Remove settings that are not needed any more
-    solver_settings.RemoveValue("solver_type")
-    solver_settings.RemoveValue("time_integration_method") # does not throw even if the value is not existing
-
-    module_full = 'KratosMultiphysics.MPMApplication.' + solver_module_name
-    solver = import_module(module_full).CreateSolver(model, solver_settings)
-
-    return solver
-
-
-def CreateSolver(model, custom_settings):
-
-    if (type(model) != KratosMultiphysics.Model):
-        raise Exception("input is expected to be provided as a Kratos Model object")
-
-    if (type(custom_settings) != KratosMultiphysics.Parameters):
-        raise Exception("input is expected to be provided as a Kratos Parameters object")
-
-    solver_settings = custom_settings["solver_settings"]
-    parallelism = custom_settings["problem_data"]["parallel_type"].GetString()
-
+
+import KratosMultiphysics
+from importlib import import_module
+
+def CreateSolverByParameters(model, solver_settings, parallelism):
+
+    solver_type = solver_settings["solver_type"].GetString()
+
+    # Solvers for OpenMP parallelism
+    if (parallelism == "OpenMP"):
+        if (solver_type == "Dynamic" or solver_type == "dynamic"):
+            time_integration_method = solver_settings["time_integration_method"].GetString()
+            if (time_integration_method == "implicit"):
+                solver_module_name = "mpm_implicit_dynamic_solver"
+            elif (time_integration_method == "explicit"):
+                solver_module_name = "mpm_explicit_solver"
+            else:
+                err_msg =  "The requested time integration method \"" + time_integration_method + "\" is not in the python solvers wrapper\n"
+                err_msg += "Available options are: \"implicit\", \"explicit\""
+                raise Exception(err_msg)
+        elif (solver_type == "Quasi-static" or solver_type == "quasi_static"):
+            solver_module_name = "mpm_quasi_static_solver"
+        elif (solver_type == "Static" or solver_type == "static"):
+            solver_module_name = "mpm_static_solver"
+        else:
+            err_msg =  "The requested solver type \"" + solver_type + "\" is not in the python solvers wrapper\n"
+            err_msg += "Available options are: \"static\", \"dynamic\", \"quasi_static\""
+            raise Exception(err_msg)
+
+    else:
+        err_msg =  "The requested parallel type \"" + parallelism + "\" is not available!\n"
+        err_msg += "Available options are: \"OpenMP\""
+        raise Exception(err_msg)
+
+    # Remove settings that are not needed any more
+    solver_settings.RemoveValue("solver_type")
+    solver_settings.RemoveValue("time_integration_method") # does not throw even if the value is not existing
+
+    module_full = 'KratosMultiphysics.MPMApplication.' + solver_module_name
+    solver = import_module(module_full).CreateSolver(model, solver_settings)
+
+    return solver
+
+
+def CreateSolver(model, custom_settings):
+
+    if (type(model) != KratosMultiphysics.Model):
+        raise Exception("input is expected to be provided as a Kratos Model object")
+
+    if (type(custom_settings) != KratosMultiphysics.Parameters):
+        raise Exception("input is expected to be provided as a Kratos Parameters object")
+
+    solver_settings = custom_settings["solver_settings"]
+    parallelism = custom_settings["problem_data"]["parallel_type"].GetString()
+
     return CreateSolverByParameters(model, solver_settings, parallelism)
```

## KratosMultiphysics/MPMApplication/assign_gravity_to_particle_process.py

 * *Ordering differences only*

```diff
@@ -1,13 +1,13 @@
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-from KratosMultiphysics.MPMApplication.assign_gravity_to_material_point_process import AssignGravityToMaterialPointProcess
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a model object")
-    wrng_msg  = "Process `assign_gravity_to_particle_process` is replaced "
-    wrng_msg += "by `assign_gravity_to_material_point_process`."
-    IssueDeprecationWarning("MPMApplication:",wrng_msg)
-    return AssignGravityToMaterialPointProcess(model, settings["Parameters"])
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+from KratosMultiphysics.MPMApplication.assign_gravity_to_material_point_process import AssignGravityToMaterialPointProcess
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a model object")
+    wrng_msg  = "Process `assign_gravity_to_particle_process` is replaced "
+    wrng_msg += "by `assign_gravity_to_material_point_process`."
+    IssueDeprecationWarning("MPMApplication:",wrng_msg)
+    return AssignGravityToMaterialPointProcess(model, settings["Parameters"])
```

## KratosMultiphysics/MPMApplication/mpm_analysis.py

 * *Ordering differences only*

```diff
@@ -1,115 +1,115 @@
-
-# Importing Kratos Core, Applications and Dependencies
-import KratosMultiphysics
-
-# Importing the base class
-from KratosMultiphysics.analysis_stage import AnalysisStage
-from KratosMultiphysics.MPMApplication.python_solvers_wrapper_mpm import CreateSolver
-
-class MPMAnalysis(AnalysisStage):
-    """
-    This class is the main-script of the MPMApplication put in a class
-    """
-
-    def __init__(self, model, project_parameters):
-        # Making sure that older cases still work by properly initializing the parameters
-        solver_settings = project_parameters["solver_settings"]
-
-        # Import parallel modules if needed
-        # has to be done before the base-class constuctor is called (in which the solver is constructed)
-        # TODO: currently MPI parallelization is not present in MPMApplication
-        # TODO: the following import lines will be kept here for future reference
-        if (project_parameters["problem_data"]["parallel_type"].GetString() == "MPI"):
-            warn_msg  = 'Currently MPI parallelization is not present in MPMApplication!'
-            KratosMultiphysics.Logger.PrintWarning("MPMAnalysis", warn_msg)
-            # import KratosMultiphysics.MetisApplication as MetisApplication
-            # import KratosMultiphysics.TrilinosApplication as TrilinosApplication
-
-        super(MPMAnalysis, self).__init__(model, project_parameters)
-
-    #### Internal functions ####
-    def _CreateSolver(self):
-        """ Create the Solver (and create and import the ModelPart if it is not alread in the model) """
-        ## Solver construction
-        return CreateSolver(self.model, self.project_parameters)
-
-    def _CreateProcesses(self, parameter_name, initialization_order):
-        """Create a list of Processes"""
-        list_of_processes = super(MPMAnalysis, self)._CreateProcesses(parameter_name, initialization_order)
-
-        if parameter_name == "processes":
-            processes_block_names = ["constraints_process_list", "loads_process_list", "list_other_processes", "gravity"]
-            if len(list_of_processes) == 0: # Processes are given in the old format
-                info_msg  = "Using the old way to create the processes, this will be removed!\n"
-                info_msg += "Refer to \"https://github.com/KratosMultiphysics/Kratos/wiki/Common-"
-                info_msg += "Python-Interface-of-Applications-for-Users#analysisstage-usage\" "
-                info_msg += "for a description of the new format"
-                KratosMultiphysics.Logger.PrintWarning("MPMAnalysis", info_msg)
-                from KratosMultiphysics.process_factory import KratosProcessFactory
-                factory = KratosProcessFactory(self.model)
-                for process_name in processes_block_names:
-                    if (self.project_parameters.Has(process_name) is True):
-                        list_of_processes += factory.ConstructListOfProcesses(self.project_parameters[process_name])
-            else: # Processes are given in the new format
-                for process_name in processes_block_names:
-                    if (self.project_parameters.Has(process_name) is True):
-                        raise Exception("Mixing of process initialization is not allowed!")
-        elif parameter_name == "output_processes":
-            if self.project_parameters.Has("grid_output_configuration") or self.project_parameters.Has("body_output_configuration"):
-                info_msg  = "Using the old way to create the gid-output for grid, this will be removed!\n"
-                info_msg += "Refer to \"https://github.com/KratosMultiphysics/Kratos/wiki/Common-"
-                info_msg += "Python-Interface-of-Applications-for-Users#analysisstage-usage\" "
-                info_msg += "for a description of the new format"
-                KratosMultiphysics.Logger.PrintInfo("MPMAnalysis", info_msg)
-                if self.project_parameters.Has("grid_output_configuration"):
-                    grid_gid_output= self._SetUpGiDOutput("grid_output")
-                    list_of_processes += [grid_gid_output,]
-                if self.project_parameters.Has("body_output_configuration"):
-                    mp_gid_output= self._SetUpGiDOutput("body_output")
-                    list_of_processes += [mp_gid_output,]
-        else:
-            raise NameError("wrong parameter name")
-
-        return list_of_processes
-
-    def _SetUpGiDOutput(self, parameter_name):
-        '''Initialize a GiD output instance'''
-        if self.parallel_type == "OpenMP":
-            if parameter_name == "grid_output":
-                from KratosMultiphysics.gid_output_process import GiDOutputProcess as OutputProcess
-                grid_output_file_name = self.project_parameters["problem_data"]["problem_name"].GetString() + "_Grid"
-                gid_output = OutputProcess(self._GetSolver().GetGridModelPart(), grid_output_file_name,
-                                    self.project_parameters["grid_output_configuration"])
-            elif parameter_name == "body_output":
-                from KratosMultiphysics.MPMApplication.mpm_gid_output_process import MPMGiDOutputProcess as OutputProcess
-                mp_output_file_name = self.project_parameters["problem_data"]["problem_name"].GetString() + "_Body"
-                gid_output = OutputProcess(self._GetSolver().GetComputingModelPart(), mp_output_file_name,
-                                    self.project_parameters["body_output_configuration"])
-        return gid_output
-
-    def _GetSimulationName(self):
-        return "::[MPM Analysis]:: "
-
-if __name__ == "__main__":
-    from sys import argv
-
-    if len(argv) > 2:
-        err_msg =  'Too many input arguments!\n'
-        err_msg += 'Use this script in the following way:\n'
-        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
-        err_msg += '    "python3 mpm_analysis.py"\n'
-        err_msg += '- With custom ProjectParameters:\n'
-        err_msg += '    "python3 mpm_analysis.py CustomProjectParameters.json"\n'
-        raise Exception(err_msg)
-
-    if len(argv) == 2: # ProjectParameters is being passed from outside
-        project_parameters_file_name = argv[1]
-    else: # using default name
-        project_parameters_file_name = "ProjectParameters.json"
-
-    with open(project_parameters_file_name,'r') as parameter_file:
-        parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-    model = KratosMultiphysics.Model()
-    simulation = MPMAnalysis(model, parameters)
-    simulation.Run()
+
+# Importing Kratos Core, Applications and Dependencies
+import KratosMultiphysics
+
+# Importing the base class
+from KratosMultiphysics.analysis_stage import AnalysisStage
+from KratosMultiphysics.MPMApplication.python_solvers_wrapper_mpm import CreateSolver
+
+class MPMAnalysis(AnalysisStage):
+    """
+    This class is the main-script of the MPMApplication put in a class
+    """
+
+    def __init__(self, model, project_parameters):
+        # Making sure that older cases still work by properly initializing the parameters
+        solver_settings = project_parameters["solver_settings"]
+
+        # Import parallel modules if needed
+        # has to be done before the base-class constuctor is called (in which the solver is constructed)
+        # TODO: currently MPI parallelization is not present in MPMApplication
+        # TODO: the following import lines will be kept here for future reference
+        if (project_parameters["problem_data"]["parallel_type"].GetString() == "MPI"):
+            warn_msg  = 'Currently MPI parallelization is not present in MPMApplication!'
+            KratosMultiphysics.Logger.PrintWarning("MPMAnalysis", warn_msg)
+            # import KratosMultiphysics.MetisApplication as MetisApplication
+            # import KratosMultiphysics.TrilinosApplication as TrilinosApplication
+
+        super(MPMAnalysis, self).__init__(model, project_parameters)
+
+    #### Internal functions ####
+    def _CreateSolver(self):
+        """ Create the Solver (and create and import the ModelPart if it is not alread in the model) """
+        ## Solver construction
+        return CreateSolver(self.model, self.project_parameters)
+
+    def _CreateProcesses(self, parameter_name, initialization_order):
+        """Create a list of Processes"""
+        list_of_processes = super(MPMAnalysis, self)._CreateProcesses(parameter_name, initialization_order)
+
+        if parameter_name == "processes":
+            processes_block_names = ["constraints_process_list", "loads_process_list", "list_other_processes", "gravity"]
+            if len(list_of_processes) == 0: # Processes are given in the old format
+                info_msg  = "Using the old way to create the processes, this will be removed!\n"
+                info_msg += "Refer to \"https://github.com/KratosMultiphysics/Kratos/wiki/Common-"
+                info_msg += "Python-Interface-of-Applications-for-Users#analysisstage-usage\" "
+                info_msg += "for a description of the new format"
+                KratosMultiphysics.Logger.PrintWarning("MPMAnalysis", info_msg)
+                from KratosMultiphysics.process_factory import KratosProcessFactory
+                factory = KratosProcessFactory(self.model)
+                for process_name in processes_block_names:
+                    if (self.project_parameters.Has(process_name) is True):
+                        list_of_processes += factory.ConstructListOfProcesses(self.project_parameters[process_name])
+            else: # Processes are given in the new format
+                for process_name in processes_block_names:
+                    if (self.project_parameters.Has(process_name) is True):
+                        raise Exception("Mixing of process initialization is not allowed!")
+        elif parameter_name == "output_processes":
+            if self.project_parameters.Has("grid_output_configuration") or self.project_parameters.Has("body_output_configuration"):
+                info_msg  = "Using the old way to create the gid-output for grid, this will be removed!\n"
+                info_msg += "Refer to \"https://github.com/KratosMultiphysics/Kratos/wiki/Common-"
+                info_msg += "Python-Interface-of-Applications-for-Users#analysisstage-usage\" "
+                info_msg += "for a description of the new format"
+                KratosMultiphysics.Logger.PrintInfo("MPMAnalysis", info_msg)
+                if self.project_parameters.Has("grid_output_configuration"):
+                    grid_gid_output= self._SetUpGiDOutput("grid_output")
+                    list_of_processes += [grid_gid_output,]
+                if self.project_parameters.Has("body_output_configuration"):
+                    mp_gid_output= self._SetUpGiDOutput("body_output")
+                    list_of_processes += [mp_gid_output,]
+        else:
+            raise NameError("wrong parameter name")
+
+        return list_of_processes
+
+    def _SetUpGiDOutput(self, parameter_name):
+        '''Initialize a GiD output instance'''
+        if self.parallel_type == "OpenMP":
+            if parameter_name == "grid_output":
+                from KratosMultiphysics.gid_output_process import GiDOutputProcess as OutputProcess
+                grid_output_file_name = self.project_parameters["problem_data"]["problem_name"].GetString() + "_Grid"
+                gid_output = OutputProcess(self._GetSolver().GetGridModelPart(), grid_output_file_name,
+                                    self.project_parameters["grid_output_configuration"])
+            elif parameter_name == "body_output":
+                from KratosMultiphysics.MPMApplication.mpm_gid_output_process import MPMGiDOutputProcess as OutputProcess
+                mp_output_file_name = self.project_parameters["problem_data"]["problem_name"].GetString() + "_Body"
+                gid_output = OutputProcess(self._GetSolver().GetComputingModelPart(), mp_output_file_name,
+                                    self.project_parameters["body_output_configuration"])
+        return gid_output
+
+    def _GetSimulationName(self):
+        return "::[MPM Analysis]:: "
+
+if __name__ == "__main__":
+    from sys import argv
+
+    if len(argv) > 2:
+        err_msg =  'Too many input arguments!\n'
+        err_msg += 'Use this script in the following way:\n'
+        err_msg += '- With default ProjectParameters (read from "ProjectParameters.json"):\n'
+        err_msg += '    "python3 mpm_analysis.py"\n'
+        err_msg += '- With custom ProjectParameters:\n'
+        err_msg += '    "python3 mpm_analysis.py CustomProjectParameters.json"\n'
+        raise Exception(err_msg)
+
+    if len(argv) == 2: # ProjectParameters is being passed from outside
+        project_parameters_file_name = argv[1]
+    else: # using default name
+        project_parameters_file_name = "ProjectParameters.json"
+
+    with open(project_parameters_file_name,'r') as parameter_file:
+        parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+    model = KratosMultiphysics.Model()
+    simulation = MPMAnalysis(model, parameters)
+    simulation.Run()
```

## KratosMultiphysics/MPMApplication/assign_initial_velocity_to_particle_process.py

 * *Ordering differences only*

```diff
@@ -1,13 +1,13 @@
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-from KratosMultiphysics.MPMApplication.assign_initial_velocity_to_material_point_process import AssignInitialVelocityToMaterialPointProcess
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a model object")
-    wrng_msg  = "Process `assign_initial_velocity_to_particle_process` is replaced "
-    wrng_msg += "by `assign_initial_velocity_to_material_point_process`."
-    IssueDeprecationWarning("MPMApplication:",wrng_msg)
-    return AssignInitialVelocityToMaterialPointProcess(model, settings["Parameters"])
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+from KratosMultiphysics.MPMApplication.assign_initial_velocity_to_material_point_process import AssignInitialVelocityToMaterialPointProcess
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a model object")
+    wrng_msg  = "Process `assign_initial_velocity_to_particle_process` is replaced "
+    wrng_msg += "by `assign_initial_velocity_to_material_point_process`."
+    IssueDeprecationWarning("MPMApplication:",wrng_msg)
+    return AssignInitialVelocityToMaterialPointProcess(model, settings["Parameters"])
```

## KratosMultiphysics/MPMApplication/mpm_gid_output_process.py

 * *Ordering differences only*

```diff
@@ -1,260 +1,260 @@
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Import applications and dependencies
-import KratosMultiphysics.MPMApplication as KratosMPM
-from  KratosMultiphysics.deprecation_management import DeprecationManager
-
-# Import time library
-from time import time
-
-def Factory(settings, Model):
-    if(type(settings) != KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    model_part = Model[settings["Parameters"]["model_part_name"].GetString()]
-    output_name = settings["Parameters"]["output_name"].GetString()
-    postprocess_parameters = settings["Parameters"]["postprocess_parameters"]
-    return MPMGiDOutputProcess(model_part, output_name, postprocess_parameters)
-
-class MPMGiDOutputProcess(KratosMultiphysics.Process):
-    defaults = KratosMultiphysics.Parameters("""{
-        "result_file_configuration": {
-            "gidpost_flags": {
-                "GiDPostMode": "GiD_PostBinary",
-                "WriteDeformedMeshFlag": "WriteUndeformed",
-                "WriteConditionsFlag": "WriteElementsOnly",
-                "MultiFileFlag": "SingleFile"
-            },
-            "file_label": "time",
-            "output_control_type": "step",
-            "output_interval": 1.0,
-            "body_output": true,
-            "node_output": false,
-            "skin_output": false,
-            "plane_output": [],
-            "nodal_results": [],
-            "nodal_nonhistorical_results": [],
-            "nodal_flags_results": [],
-            "gauss_point_results": [],
-            "additional_list_files": []
-        },
-        "point_data_configuration": []
-    }""")
-
-
-    def __init__(self, model_part, file_name, param):
-
-        KratosMultiphysics.Process.__init__(self)
-
-        if param is None:
-            param = self.defaults
-        else:
-            self.TranslateLegacyVariablesAccordingToCurrentStandard(param)
-            param.ValidateAndAssignDefaults(self.defaults)
-
-        # Default
-        self.param = param
-        self.base_file_name = file_name
-        self.model_part = model_part
-
-        self.next_output = 0.0
-
-    # This function can be extended with new deprecated variables as they are generated
-    def TranslateLegacyVariablesAccordingToCurrentStandard(self, settings):
-        # Defining a string to help the user understand where the warnings come from (in case any is thrown)
-        context_string = type(self).__name__
-
-        if settings.Has('result_file_configuration'):
-            sub_settings_where_var_is = settings['result_file_configuration']
-            old_name = 'output_frequency'
-            new_name = 'output_interval'
-
-            if DeprecationManager.HasDeprecatedVariable(context_string, sub_settings_where_var_is, old_name, new_name):
-                DeprecationManager.ReplaceDeprecatedVariableName(sub_settings_where_var_is, old_name, new_name)
-
-    # Public Functions
-    def ExecuteInitialize(self):
-
-        result_file_configuration = self.param["result_file_configuration"]
-        result_file_configuration.ValidateAndAssignDefaults(self.defaults["result_file_configuration"])
-
-        # Set up output frequency and format
-        output_file_label = result_file_configuration["file_label"].GetString()
-        if output_file_label == "time":
-            self.output_label_is_time = True
-        elif output_file_label == "step":
-            self.output_label_is_time = False
-        else:
-            msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,output_file_label,"file_label")
-            raise Exception(msg)
-
-        output_control_type = result_file_configuration["output_control_type"].GetString()
-        if output_control_type == "time":
-            self.output_control_is_time = True
-        elif output_control_type == "step":
-            self.output_control_is_time = False
-        else:
-            msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,output_file_label,"file_label")
-            raise Exception(msg)
-
-        self.output_frequency = result_file_configuration["output_interval"].GetDouble()
-
-        # Set Variable list to print
-        self.variable_name_list = result_file_configuration["gauss_point_results"]
-        self.variable_list      = []
-        for i in range(self.variable_name_list.size()):
-            var_name = self.variable_name_list[i].GetString()
-            variable = self._get_variable(var_name)
-            self.variable_list.append(variable)
-
-    def ExecuteBeforeSolutionLoop(self):
-        # Initiate Output Mesh
-        self.mesh_file = open(self.base_file_name + ".post.msh",'w')
-        self.mesh_file.write("MESH \"")
-        self.mesh_file.write("outmesh")
-        self.mesh_file.write("\" dimension 3 ElemType Point Nnode 1\n")
-        self.mesh_file.write("Coordinates\n")
-        for mpm in self.model_part.Elements:
-            coord = mpm.CalculateOnIntegrationPoints(KratosMPM.MP_COORD,self.model_part.ProcessInfo)[0]
-            self.mesh_file.write("{} {} {} {}\n".format( mpm.Id, coord[0], coord[1], coord[2]))
-        self.mesh_file.write("End Coordinates\n")
-        self.mesh_file.write("Elements\n")
-        for mpm in self.model_part.Elements:
-            self.mesh_file.write("{} {}\n".format(mpm.Id, mpm.Id))
-        self.mesh_file.write("End Elements\n")
-        self.mesh_file.flush()
-
-        # Initiate Output File
-        self.result_file = open(self.base_file_name + ".post.res",'w')
-        self.result_file.write("GiD Post Results File 1.0\n")
-
-    def ExecuteInitializeSolutionStep(self): pass
-
-    def ExecuteFinalizeSolutionStep(self): pass
-
-    def ExecuteFinalize(self): pass
-
-    def PrintOutput(self):
-        # Print the output
-        time = self._get_pretty_time(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
-
-        # Write results to the initiated result file
-        self._write_mp_results(time)
-
-        # Schedule next output
-        if self.output_frequency > 0.0: # Note: if == 0, we'll just always print
-            if self.output_control_is_time:
-                while self._get_pretty_time(self.next_output) <= time:
-                    self.next_output += self.output_frequency
-            else:
-                while self.next_output <= self.model_part.ProcessInfo[KratosMultiphysics.STEP]:
-                    self.next_output += self.output_frequency
-
-
-    def IsOutputStep(self):
-        if self.output_control_is_time:
-            time = self._get_pretty_time(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
-            return (time >= self._get_pretty_time(self.next_output))
-        else:
-            return ( self.model_part.ProcessInfo[KratosMultiphysics.STEP] >= self.next_output )
-
-
-    # Private Functions
-    def _get_pretty_time(self,time):
-        pretty_time = "{0:.12g}".format(time)
-        pretty_time = float(pretty_time)
-        return pretty_time
-
-    def _get_attribute(self, my_string, function_pointer, attribute_type):
-        """Return the python object named by the string argument.
-
-        To be used with functions from KratosGlobals
-
-        Examples:
-        variable = self._get_attribute("DISPLACEMENT",
-                                       KratosMultiphysics.MPMApplication.GetVariable,
-                                       "Variable")
-        """
-        splitted = my_string.split(".")
-
-        if len(splitted) == 0:
-            raise Exception("Something wrong. Trying to split the string " + my_string)
-        if len(splitted) > 3:
-            raise Exception("Something wrong. String " + my_string + " has too many arguments")
-
-        attribute_name = splitted[-1]
-
-        if len(splitted) == 2 or len(splitted) == 3:
-            warning_msg =  "Ignoring \"" +  my_string.rsplit(".",1)[0]
-            warning_msg += "\" for " + attribute_type +" \"" + attribute_name + "\""
-            KratosMultiphysics.Logger.PrintInfo("Warning in mpm gid output", warning_msg)
-
-        return function_pointer(attribute_name) # This also checks if the application has been imported
-
-    def _get_variable(self, my_string):
-        """Return the python object of a Variable named by the string argument.
-
-        Examples:
-        recommended usage:
-        variable = self._get_variable("MP_VELOCITY")
-        deprecated:
-        variable = self._get_variables("KratosMultiphysics.MPMApplication.MP_VELOCITY")
-        """
-        return self._get_attribute(my_string, KratosMultiphysics.KratosGlobals.GetVariable, "Variable")
-
-    def _write_mp_results(self, step_label=None):
-        clock_time = self._start_time_measure()
-
-        for i in range(self.variable_name_list.size()):
-            var_name = self.variable_name_list[i].GetString()
-            variable = self.variable_list[i]
-
-            is_scalar = self._is_scalar(variable)
-
-            # Write in result file
-            self.result_file.write("Result \"")
-            self.result_file.write(var_name)
-
-            if is_scalar:
-                self.result_file.write('" "Kratos" {} Scalar OnNodes\n'.format(step_label))
-            else:
-                self.result_file.write('" "Kratos" {} Vector OnNodes\n'.format(step_label))
-
-            self.result_file.write("Values\n")
-            for mpm in self.model_part.Elements:
-                print_variable = mpm.CalculateOnIntegrationPoints(variable,self.model_part.ProcessInfo)[0]
-                # Check whether variable is a scalar or vector
-                if isinstance(print_variable, float) or isinstance(print_variable, int):
-                    print_size = 1
-                else:
-                    print_size = print_variable.Size()
-
-                # Write variable as formated
-                if print_size == 1:
-                    self.result_file.write("{} {}\n".format(mpm.Id, print_variable))
-                elif print_size == 3:
-                    self.result_file.write("{} {} {} {}\n".format(mpm.Id, print_variable[0], print_variable[1], print_variable[2]))
-                elif print_size == 6:
-                    self.result_file.write("{} {} {} {} {} {} {}\n".format(mpm.Id, print_variable[0], print_variable[1], print_variable[2], print_variable[3], print_variable[4], print_variable[5]))
-                else:
-                    KratosMultiphysics.Logger.PrintInfo("Warning in mpm gid output", "Printing format is not defined for variable: ", var_name, "with size: ", print_size)
-
-            self.result_file.write("End Values\n")
-
-        self._stop_time_measure(clock_time)
-
-    def _start_time_measure(self):
-        return time()
-
-    def _stop_time_measure(self, time_ip):
-        time_fp = time()
-        KratosMultiphysics.Logger.PrintInfo("::[MPM GiD Output Process]:: ", "[Spent time for output = ", time_fp - time_ip, "sec]")
-
-    def _is_scalar(self,variable):
-        is_scalar = False
-        if (isinstance(variable,KratosMultiphysics.IntegerVariable) or isinstance(variable,KratosMultiphysics.DoubleVariable) or isinstance(variable,KratosMultiphysics.BoolVariable)):
-            is_scalar = True
-        elif (isinstance(variable,KratosMultiphysics.StringVariable)):
-            raise Exception("String variable cant be printed.")
-        return is_scalar
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Import applications and dependencies
+import KratosMultiphysics.MPMApplication as KratosMPM
+from  KratosMultiphysics.deprecation_management import DeprecationManager
+
+# Import time library
+from time import time
+
+def Factory(settings, Model):
+    if(type(settings) != KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    model_part = Model[settings["Parameters"]["model_part_name"].GetString()]
+    output_name = settings["Parameters"]["output_name"].GetString()
+    postprocess_parameters = settings["Parameters"]["postprocess_parameters"]
+    return MPMGiDOutputProcess(model_part, output_name, postprocess_parameters)
+
+class MPMGiDOutputProcess(KratosMultiphysics.Process):
+    defaults = KratosMultiphysics.Parameters("""{
+        "result_file_configuration": {
+            "gidpost_flags": {
+                "GiDPostMode": "GiD_PostBinary",
+                "WriteDeformedMeshFlag": "WriteUndeformed",
+                "WriteConditionsFlag": "WriteElementsOnly",
+                "MultiFileFlag": "SingleFile"
+            },
+            "file_label": "time",
+            "output_control_type": "step",
+            "output_interval": 1.0,
+            "body_output": true,
+            "node_output": false,
+            "skin_output": false,
+            "plane_output": [],
+            "nodal_results": [],
+            "nodal_nonhistorical_results": [],
+            "nodal_flags_results": [],
+            "gauss_point_results": [],
+            "additional_list_files": []
+        },
+        "point_data_configuration": []
+    }""")
+
+
+    def __init__(self, model_part, file_name, param):
+
+        KratosMultiphysics.Process.__init__(self)
+
+        if param is None:
+            param = self.defaults
+        else:
+            self.TranslateLegacyVariablesAccordingToCurrentStandard(param)
+            param.ValidateAndAssignDefaults(self.defaults)
+
+        # Default
+        self.param = param
+        self.base_file_name = file_name
+        self.model_part = model_part
+
+        self.next_output = 0.0
+
+    # This function can be extended with new deprecated variables as they are generated
+    def TranslateLegacyVariablesAccordingToCurrentStandard(self, settings):
+        # Defining a string to help the user understand where the warnings come from (in case any is thrown)
+        context_string = type(self).__name__
+
+        if settings.Has('result_file_configuration'):
+            sub_settings_where_var_is = settings['result_file_configuration']
+            old_name = 'output_frequency'
+            new_name = 'output_interval'
+
+            if DeprecationManager.HasDeprecatedVariable(context_string, sub_settings_where_var_is, old_name, new_name):
+                DeprecationManager.ReplaceDeprecatedVariableName(sub_settings_where_var_is, old_name, new_name)
+
+    # Public Functions
+    def ExecuteInitialize(self):
+
+        result_file_configuration = self.param["result_file_configuration"]
+        result_file_configuration.ValidateAndAssignDefaults(self.defaults["result_file_configuration"])
+
+        # Set up output frequency and format
+        output_file_label = result_file_configuration["file_label"].GetString()
+        if output_file_label == "time":
+            self.output_label_is_time = True
+        elif output_file_label == "step":
+            self.output_label_is_time = False
+        else:
+            msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,output_file_label,"file_label")
+            raise Exception(msg)
+
+        output_control_type = result_file_configuration["output_control_type"].GetString()
+        if output_control_type == "time":
+            self.output_control_is_time = True
+        elif output_control_type == "step":
+            self.output_control_is_time = False
+        else:
+            msg = "{0} Error: Unknown value \"{1}\" read for parameter \"{2}\"".format(self.__class__.__name__,output_file_label,"file_label")
+            raise Exception(msg)
+
+        self.output_frequency = result_file_configuration["output_interval"].GetDouble()
+
+        # Set Variable list to print
+        self.variable_name_list = result_file_configuration["gauss_point_results"]
+        self.variable_list      = []
+        for i in range(self.variable_name_list.size()):
+            var_name = self.variable_name_list[i].GetString()
+            variable = self._get_variable(var_name)
+            self.variable_list.append(variable)
+
+    def ExecuteBeforeSolutionLoop(self):
+        # Initiate Output Mesh
+        self.mesh_file = open(self.base_file_name + ".post.msh",'w')
+        self.mesh_file.write("MESH \"")
+        self.mesh_file.write("outmesh")
+        self.mesh_file.write("\" dimension 3 ElemType Point Nnode 1\n")
+        self.mesh_file.write("Coordinates\n")
+        for mpm in self.model_part.Elements:
+            coord = mpm.CalculateOnIntegrationPoints(KratosMPM.MP_COORD,self.model_part.ProcessInfo)[0]
+            self.mesh_file.write("{} {} {} {}\n".format( mpm.Id, coord[0], coord[1], coord[2]))
+        self.mesh_file.write("End Coordinates\n")
+        self.mesh_file.write("Elements\n")
+        for mpm in self.model_part.Elements:
+            self.mesh_file.write("{} {}\n".format(mpm.Id, mpm.Id))
+        self.mesh_file.write("End Elements\n")
+        self.mesh_file.flush()
+
+        # Initiate Output File
+        self.result_file = open(self.base_file_name + ".post.res",'w')
+        self.result_file.write("GiD Post Results File 1.0\n")
+
+    def ExecuteInitializeSolutionStep(self): pass
+
+    def ExecuteFinalizeSolutionStep(self): pass
+
+    def ExecuteFinalize(self): pass
+
+    def PrintOutput(self):
+        # Print the output
+        time = self._get_pretty_time(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
+
+        # Write results to the initiated result file
+        self._write_mp_results(time)
+
+        # Schedule next output
+        if self.output_frequency > 0.0: # Note: if == 0, we'll just always print
+            if self.output_control_is_time:
+                while self._get_pretty_time(self.next_output) <= time:
+                    self.next_output += self.output_frequency
+            else:
+                while self.next_output <= self.model_part.ProcessInfo[KratosMultiphysics.STEP]:
+                    self.next_output += self.output_frequency
+
+
+    def IsOutputStep(self):
+        if self.output_control_is_time:
+            time = self._get_pretty_time(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
+            return (time >= self._get_pretty_time(self.next_output))
+        else:
+            return ( self.model_part.ProcessInfo[KratosMultiphysics.STEP] >= self.next_output )
+
+
+    # Private Functions
+    def _get_pretty_time(self,time):
+        pretty_time = "{0:.12g}".format(time)
+        pretty_time = float(pretty_time)
+        return pretty_time
+
+    def _get_attribute(self, my_string, function_pointer, attribute_type):
+        """Return the python object named by the string argument.
+
+        To be used with functions from KratosGlobals
+
+        Examples:
+        variable = self._get_attribute("DISPLACEMENT",
+                                       KratosMultiphysics.MPMApplication.GetVariable,
+                                       "Variable")
+        """
+        splitted = my_string.split(".")
+
+        if len(splitted) == 0:
+            raise Exception("Something wrong. Trying to split the string " + my_string)
+        if len(splitted) > 3:
+            raise Exception("Something wrong. String " + my_string + " has too many arguments")
+
+        attribute_name = splitted[-1]
+
+        if len(splitted) == 2 or len(splitted) == 3:
+            warning_msg =  "Ignoring \"" +  my_string.rsplit(".",1)[0]
+            warning_msg += "\" for " + attribute_type +" \"" + attribute_name + "\""
+            KratosMultiphysics.Logger.PrintInfo("Warning in mpm gid output", warning_msg)
+
+        return function_pointer(attribute_name) # This also checks if the application has been imported
+
+    def _get_variable(self, my_string):
+        """Return the python object of a Variable named by the string argument.
+
+        Examples:
+        recommended usage:
+        variable = self._get_variable("MP_VELOCITY")
+        deprecated:
+        variable = self._get_variables("KratosMultiphysics.MPMApplication.MP_VELOCITY")
+        """
+        return self._get_attribute(my_string, KratosMultiphysics.KratosGlobals.GetVariable, "Variable")
+
+    def _write_mp_results(self, step_label=None):
+        clock_time = self._start_time_measure()
+
+        for i in range(self.variable_name_list.size()):
+            var_name = self.variable_name_list[i].GetString()
+            variable = self.variable_list[i]
+
+            is_scalar = self._is_scalar(variable)
+
+            # Write in result file
+            self.result_file.write("Result \"")
+            self.result_file.write(var_name)
+
+            if is_scalar:
+                self.result_file.write('" "Kratos" {} Scalar OnNodes\n'.format(step_label))
+            else:
+                self.result_file.write('" "Kratos" {} Vector OnNodes\n'.format(step_label))
+
+            self.result_file.write("Values\n")
+            for mpm in self.model_part.Elements:
+                print_variable = mpm.CalculateOnIntegrationPoints(variable,self.model_part.ProcessInfo)[0]
+                # Check whether variable is a scalar or vector
+                if isinstance(print_variable, float) or isinstance(print_variable, int):
+                    print_size = 1
+                else:
+                    print_size = print_variable.Size()
+
+                # Write variable as formated
+                if print_size == 1:
+                    self.result_file.write("{} {}\n".format(mpm.Id, print_variable))
+                elif print_size == 3:
+                    self.result_file.write("{} {} {} {}\n".format(mpm.Id, print_variable[0], print_variable[1], print_variable[2]))
+                elif print_size == 6:
+                    self.result_file.write("{} {} {} {} {} {} {}\n".format(mpm.Id, print_variable[0], print_variable[1], print_variable[2], print_variable[3], print_variable[4], print_variable[5]))
+                else:
+                    KratosMultiphysics.Logger.PrintInfo("Warning in mpm gid output", "Printing format is not defined for variable: ", var_name, "with size: ", print_size)
+
+            self.result_file.write("End Values\n")
+
+        self._stop_time_measure(clock_time)
+
+    def _start_time_measure(self):
+        return time()
+
+    def _stop_time_measure(self, time_ip):
+        time_fp = time()
+        KratosMultiphysics.Logger.PrintInfo("::[MPM GiD Output Process]:: ", "[Spent time for output = ", time_fp - time_ip, "sec]")
+
+    def _is_scalar(self,variable):
+        is_scalar = False
+        if (isinstance(variable,KratosMultiphysics.IntegerVariable) or isinstance(variable,KratosMultiphysics.DoubleVariable) or isinstance(variable,KratosMultiphysics.BoolVariable)):
+            is_scalar = True
+        elif (isinstance(variable,KratosMultiphysics.StringVariable)):
+            raise Exception("String variable cant be printed.")
+        return is_scalar
```

## KratosMultiphysics/MPMApplication/mpm_quasi_static_solver.py

 * *Ordering differences only*

```diff
@@ -1,22 +1,22 @@
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Importing the base class
-from KratosMultiphysics.MPMApplication.mpm_implicit_dynamic_solver import MPMImplicitDynamicSolver
-
-def CreateSolver(model, custom_settings):
-    return MPMQuasiStaticSolver(model, custom_settings)
-
-class MPMQuasiStaticSolver(MPMImplicitDynamicSolver):
-
-    def __init__(self, model, custom_settings):
-        # Set defaults and validate custom settings in the base class.
-        # Construct the base solver.
-        super(MPMQuasiStaticSolver, self).__init__(model, custom_settings)
-        KratosMultiphysics.Logger.PrintInfo("::[MPMQuasiStaticSolver]:: ", "Construction is finished.")
-
-    ### Protected functions ###
-
-    def _IsDynamic(self):
-        return False
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Importing the base class
+from KratosMultiphysics.MPMApplication.mpm_implicit_dynamic_solver import MPMImplicitDynamicSolver
+
+def CreateSolver(model, custom_settings):
+    return MPMQuasiStaticSolver(model, custom_settings)
+
+class MPMQuasiStaticSolver(MPMImplicitDynamicSolver):
+
+    def __init__(self, model, custom_settings):
+        # Set defaults and validate custom settings in the base class.
+        # Construct the base solver.
+        super(MPMQuasiStaticSolver, self).__init__(model, custom_settings)
+        KratosMultiphysics.Logger.PrintInfo("::[MPMQuasiStaticSolver]:: ", "Construction is finished.")
+
+    ### Protected functions ###
+
+    def _IsDynamic(self):
+        return False
```

## KratosMultiphysics/MPMApplication/mpm_static_solver.py

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
-
-# Importing the Kratos Library
-import KratosMultiphysics
-
-# Importing the base class
-from KratosMultiphysics.MPMApplication.mpm_solver import MPMSolver
-
-def CreateSolver(model, custom_settings):
-    return MPMStaticSolver(model, custom_settings)
-
-class MPMStaticSolver(MPMSolver):
-    def __init__(self, model, custom_settings):
-        # Set defaults and validate custom settings in the base class.
-        # Construct the base solver.
-        super(MPMStaticSolver, self).__init__(model, custom_settings)
-        KratosMultiphysics.Logger.PrintInfo("::[MPMStaticSolver]:: ", "Construction is finished.")
-
-    def _CreateSolutionScheme(self):
+
+# Importing the Kratos Library
+import KratosMultiphysics
+
+# Importing the base class
+from KratosMultiphysics.MPMApplication.mpm_solver import MPMSolver
+
+def CreateSolver(model, custom_settings):
+    return MPMStaticSolver(model, custom_settings)
+
+class MPMStaticSolver(MPMSolver):
+    def __init__(self, model, custom_settings):
+        # Set defaults and validate custom settings in the base class.
+        # Construct the base solver.
+        super(MPMStaticSolver, self).__init__(model, custom_settings)
+        KratosMultiphysics.Logger.PrintInfo("::[MPMStaticSolver]:: ", "Construction is finished.")
+
+    def _CreateSolutionScheme(self):
         return KratosMultiphysics.ResidualBasedIncrementalUpdateStaticScheme()
```

## KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_neumann_condition_process.py

 * *Ordering differences only*

```diff
@@ -1,101 +1,101 @@
-import KratosMultiphysics
-from KratosMultiphysics.deprecation_management import DeprecationManager
-import KratosMultiphysics.MPMApplication as KratosMPM
-from KratosMultiphysics.MPMApplication.apply_mpm_particle_neumann_condition_process import ApplyMPMParticleNeumannConditionProcess
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return ApplyMPMCouplingInterfaceNeumannConditionProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class ApplyMPMCouplingInterfaceNeumannConditionProcess(ApplyMPMParticleNeumannConditionProcess):
-    def __init__(self, Model, settings ):
-
-        default_parameters = KratosMultiphysics.Parameters( """
-            {
-                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
-                "material_points_per_condition"   : 0,
-                "variable_name"             : "POINT_LOAD",
-                "constrained"               : "fixed",
-                "option"                    : ""
-            }  """ )
-
-        context_string = type(self).__name__
-        old_name = 'particles_per_condition'
-        new_name = 'material_points_per_condition'
-        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
-            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
-
-        settings.ValidateAndAssignDefaults(default_parameters)
-        self.model = Model
-        self.model_part_name = settings["model_part_name"].GetString()
-
-        # Initiate base class - Neumann condition
-        super(ApplyMPMCouplingInterfaceNeumannConditionProcess, self).__init__(Model, settings)
-
-        # Set INTERFACE flag active
-        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self.model_part.Conditions)
-
-
-    def ExecuteBeforeSolutionLoop(self):
-        # Get updated model_part
-        if (self.model_part_name.startswith('Background_Grid.')):
-            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
-        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
-        self.model_part = self.model[mpm_material_model_part_name]
-
-        ### Translate conditions with INTERFACE flag into a new model part "MPM_Coupling_Neumann_Interface" responsible for coupling 
-        # Create coupling model part
-        if not self.model.HasModelPart("MPM_Coupling_Neumann_Interface"):
-            self.model.CreateModelPart("MPM_Coupling_Neumann_Interface")
-        self.coupling_model_part = self.model.GetModelPart("MPM_Coupling_Neumann_Interface").CreateSubModelPart(self.model_part_name)
-
-        # Prepare coupling model part
-        self._prepare_coupling_model_part(self.coupling_model_part)
-
-        # Create nodes and fill coupling model part
-        for mpc in self.model_part.Conditions:
-            if (mpc.Is(KratosMultiphysics.INTERFACE)):
-                node_id         = mpc.Id
-                node_coordinate = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD, self.model_part.ProcessInfo)[0]
-                self.coupling_model_part.CreateNewNode(node_id, node_coordinate[0], node_coordinate[1], node_coordinate[2])
-
-
-    def ExecuteInitializeSolutionStep(self):
-        ### Clone delta time
-        self.coupling_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME] = self.model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
-
-        # ### Send Point Load from coupling node to condition
-
-        for coupling_node in self.coupling_model_part.Nodes:
-            coupling_id  = coupling_node.Id
-            point_load = coupling_node.GetSolutionStepValue(KratosMultiphysics.CONTACT_FORCE)
-
-            self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.POINT_LOAD, [point_load], self.model_part.ProcessInfo)
-
-
-
-    def ExecuteFinalizeSolutionStep(self):
-        ### Get kinematic variables from mp to coupling_mp
-        for mpc in self.model_part.Conditions:
-            if (mpc.Is(KratosMultiphysics.INTERFACE)):
-                coupling_id   = mpc.Id
-
-                displacement = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_DISPLACEMENT, self.model_part.ProcessInfo)[0]
-                velocity = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_VELOCITY, self.model_part.ProcessInfo)[0]
-                
-                self.coupling_model_part.GetNode(coupling_id).SetSolutionStepValue(KratosMultiphysics.VELOCITY,0,velocity)
-                self.coupling_model_part.GetNode(coupling_id).SetSolutionStepValue(KratosMultiphysics.DISPLACEMENT,0,displacement)
-
-    # Local functions
-    def _prepare_coupling_model_part(self, coupling_model_part):
-        # Define domain size
-        domain_size = self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
-        coupling_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE] = domain_size
-
-        # Add variables
-        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
-        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
-        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONTACT_FORCE)
-        
+import KratosMultiphysics
+from KratosMultiphysics.deprecation_management import DeprecationManager
+import KratosMultiphysics.MPMApplication as KratosMPM
+from KratosMultiphysics.MPMApplication.apply_mpm_particle_neumann_condition_process import ApplyMPMParticleNeumannConditionProcess
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return ApplyMPMCouplingInterfaceNeumannConditionProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class ApplyMPMCouplingInterfaceNeumannConditionProcess(ApplyMPMParticleNeumannConditionProcess):
+    def __init__(self, Model, settings ):
+
+        default_parameters = KratosMultiphysics.Parameters( """
+            {
+                "model_part_name"           : "PLEASE_SPECIFY_MODEL_PART_NAME",
+                "material_points_per_condition"   : 0,
+                "variable_name"             : "POINT_LOAD",
+                "constrained"               : "fixed",
+                "option"                    : ""
+            }  """ )
+
+        context_string = type(self).__name__
+        old_name = 'particles_per_condition'
+        new_name = 'material_points_per_condition'
+        if DeprecationManager.HasDeprecatedVariable(context_string, settings, old_name, new_name):
+            DeprecationManager.ReplaceDeprecatedVariableName(settings, old_name, new_name)
+
+        settings.ValidateAndAssignDefaults(default_parameters)
+        self.model = Model
+        self.model_part_name = settings["model_part_name"].GetString()
+
+        # Initiate base class - Neumann condition
+        super(ApplyMPMCouplingInterfaceNeumannConditionProcess, self).__init__(Model, settings)
+
+        # Set INTERFACE flag active
+        KratosMultiphysics.VariableUtils().SetFlag(KratosMultiphysics.INTERFACE, True, self.model_part.Conditions)
+
+
+    def ExecuteBeforeSolutionLoop(self):
+        # Get updated model_part
+        if (self.model_part_name.startswith('Background_Grid.')):
+            self.model_part_name = self.model_part_name.replace('Background_Grid.','')
+        mpm_material_model_part_name = "MPM_Material." + self.model_part_name
+        self.model_part = self.model[mpm_material_model_part_name]
+
+        ### Translate conditions with INTERFACE flag into a new model part "MPM_Coupling_Neumann_Interface" responsible for coupling 
+        # Create coupling model part
+        if not self.model.HasModelPart("MPM_Coupling_Neumann_Interface"):
+            self.model.CreateModelPart("MPM_Coupling_Neumann_Interface")
+        self.coupling_model_part = self.model.GetModelPart("MPM_Coupling_Neumann_Interface").CreateSubModelPart(self.model_part_name)
+
+        # Prepare coupling model part
+        self._prepare_coupling_model_part(self.coupling_model_part)
+
+        # Create nodes and fill coupling model part
+        for mpc in self.model_part.Conditions:
+            if (mpc.Is(KratosMultiphysics.INTERFACE)):
+                node_id         = mpc.Id
+                node_coordinate = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD, self.model_part.ProcessInfo)[0]
+                self.coupling_model_part.CreateNewNode(node_id, node_coordinate[0], node_coordinate[1], node_coordinate[2])
+
+
+    def ExecuteInitializeSolutionStep(self):
+        ### Clone delta time
+        self.coupling_model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME] = self.model_part.ProcessInfo[KratosMultiphysics.DELTA_TIME]
+
+        # ### Send Point Load from coupling node to condition
+
+        for coupling_node in self.coupling_model_part.Nodes:
+            coupling_id  = coupling_node.Id
+            point_load = coupling_node.GetSolutionStepValue(KratosMultiphysics.CONTACT_FORCE)
+
+            self.model_part.GetCondition(coupling_id).SetValuesOnIntegrationPoints(KratosMPM.POINT_LOAD, [point_load], self.model_part.ProcessInfo)
+
+
+
+    def ExecuteFinalizeSolutionStep(self):
+        ### Get kinematic variables from mp to coupling_mp
+        for mpc in self.model_part.Conditions:
+            if (mpc.Is(KratosMultiphysics.INTERFACE)):
+                coupling_id   = mpc.Id
+
+                displacement = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_DISPLACEMENT, self.model_part.ProcessInfo)[0]
+                velocity = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_VELOCITY, self.model_part.ProcessInfo)[0]
+                
+                self.coupling_model_part.GetNode(coupling_id).SetSolutionStepValue(KratosMultiphysics.VELOCITY,0,velocity)
+                self.coupling_model_part.GetNode(coupling_id).SetSolutionStepValue(KratosMultiphysics.DISPLACEMENT,0,displacement)
+
+    # Local functions
+    def _prepare_coupling_model_part(self, coupling_model_part):
+        # Define domain size
+        domain_size = self.model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE]
+        coupling_model_part.ProcessInfo[KratosMultiphysics.DOMAIN_SIZE] = domain_size
+
+        # Add variables
+        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.DISPLACEMENT)
+        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.VELOCITY)
+        coupling_model_part.AddNodalSolutionStepVariable(KratosMultiphysics.CONTACT_FORCE)
+
```

## KratosMultiphysics/MPMApplication/assign_initial_velocity_to_material_point_process.py

 * *Ordering differences only*

```diff
@@ -1,65 +1,65 @@
-import KratosMultiphysics
-import KratosMultiphysics.MPMApplication as KratosMPM
-
-def Factory(settings, Model):
-    if(not isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return AssignInitialVelocityToMaterialPointProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class AssignInitialVelocityToMaterialPointProcess(KratosMultiphysics.Process):
-    def __init__(self, Model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        default_settings = KratosMultiphysics.Parameters("""
-            {
-                "mesh_id"              : 0,
-                "model_part_name"      : "please_specify_model_part_name",
-                "variable_name"        : "MP_VELOCITY",
-                "modulus"              : 1.0,
-                "constrained"          : true,
-                "direction"            : [0.0, 0.0, 0.0],
-                "local_axes"           : {}
-            }
-            """)
-
-        # Trick: allow "modulus" and "direction" to be a double or a string value (otherwise the ValidateAndAssignDefaults might fail)
-        if(settings.Has("modulus")):
-            if(settings["modulus"].IsString()):
-                default_settings["modulus"].SetString("0.0")
-
-        if(settings.Has("direction")):
-            if(settings["direction"].IsString()):
-                default_settings["direction"].SetString("Automatic")
-
-        # Detect if variable_name is MP_VELOCITY
-        if(settings.Has("variable_name")):
-            if(settings["variable_name"].GetString() != "MP_VELOCITY"):
-                KratosMultiphysics.Logger.PrintInfo("Warning in apply velocity to material point", "Error in determining variable_name")
-                raise Exception('The assign_initial_velocity_to_material_point_process only accepts \"MP_VELOCITY\" as variable_name.')
-
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        # Get updated model_part
-        self.model = Model
-        model_part_name = settings["model_part_name"].GetString()
-        if (model_part_name.startswith('Initial_MPM_Material.')):
-            model_part_name = model_part_name.replace('Initial_MPM_Material.','')
-        self.mpm_material_model_part_name = "MPM_Material." + model_part_name
-        # The actual initial velocity application occurs after the submodelpart is
-        # transferred from the initial MPM material to the MPM material in the MaterialPointGeneratorUtility.
-        # Therefore we change the prefix from initial MPM material
-        # to MPM material.
-
-        # Default settings
-        self.modulus = settings["modulus"].GetDouble()
-        self.velocity_direction = settings["direction"].GetVector()
-        self.velocity = self.modulus * self.velocity_direction
-
-    def ExecuteBeforeSolutionLoop(self):
-        # Assign velocity to MP after solver.Initialize() - only apply once at the beginning!
-        model_part = self.model[self.mpm_material_model_part_name]
-        # the model part is identified here, AFTER it has been transferred to the MPM_material part!
-        if not model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
-            for element in model_part.Elements:
-                element.SetValuesOnIntegrationPoints(KratosMPM.MP_VELOCITY,[self.velocity],model_part.ProcessInfo)
+import KratosMultiphysics
+import KratosMultiphysics.MPMApplication as KratosMPM
+
+def Factory(settings, Model):
+    if(not isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return AssignInitialVelocityToMaterialPointProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class AssignInitialVelocityToMaterialPointProcess(KratosMultiphysics.Process):
+    def __init__(self, Model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        default_settings = KratosMultiphysics.Parameters("""
+            {
+                "mesh_id"              : 0,
+                "model_part_name"      : "please_specify_model_part_name",
+                "variable_name"        : "MP_VELOCITY",
+                "modulus"              : 1.0,
+                "constrained"          : true,
+                "direction"            : [0.0, 0.0, 0.0],
+                "local_axes"           : {}
+            }
+            """)
+
+        # Trick: allow "modulus" and "direction" to be a double or a string value (otherwise the ValidateAndAssignDefaults might fail)
+        if(settings.Has("modulus")):
+            if(settings["modulus"].IsString()):
+                default_settings["modulus"].SetString("0.0")
+
+        if(settings.Has("direction")):
+            if(settings["direction"].IsString()):
+                default_settings["direction"].SetString("Automatic")
+
+        # Detect if variable_name is MP_VELOCITY
+        if(settings.Has("variable_name")):
+            if(settings["variable_name"].GetString() != "MP_VELOCITY"):
+                KratosMultiphysics.Logger.PrintInfo("Warning in apply velocity to material point", "Error in determining variable_name")
+                raise Exception('The assign_initial_velocity_to_material_point_process only accepts \"MP_VELOCITY\" as variable_name.')
+
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        # Get updated model_part
+        self.model = Model
+        model_part_name = settings["model_part_name"].GetString()
+        if (model_part_name.startswith('Initial_MPM_Material.')):
+            model_part_name = model_part_name.replace('Initial_MPM_Material.','')
+        self.mpm_material_model_part_name = "MPM_Material." + model_part_name
+        # The actual initial velocity application occurs after the submodelpart is
+        # transferred from the initial MPM material to the MPM material in the MaterialPointGeneratorUtility.
+        # Therefore we change the prefix from initial MPM material
+        # to MPM material.
+
+        # Default settings
+        self.modulus = settings["modulus"].GetDouble()
+        self.velocity_direction = settings["direction"].GetVector()
+        self.velocity = self.modulus * self.velocity_direction
+
+    def ExecuteBeforeSolutionLoop(self):
+        # Assign velocity to MP after solver.Initialize() - only apply once at the beginning!
+        model_part = self.model[self.mpm_material_model_part_name]
+        # the model part is identified here, AFTER it has been transferred to the MPM_material part!
+        if not model_part.ProcessInfo[KratosMultiphysics.IS_RESTARTED]:
+            for element in model_part.Elements:
+                element.SetValuesOnIntegrationPoints(KratosMPM.MP_VELOCITY,[self.velocity],model_part.ProcessInfo)
```

## KratosMultiphysics/MPMApplication/particle_from_json_check_result_process.py

 * *Ordering differences only*

```diff
@@ -1,12 +1,12 @@
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-from KratosMultiphysics.MPMApplication.mpm_from_json_check_result_process import MPMFromJsonCheckResultProcess
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a model object")
-    wrng_msg = "Process `particle_from_json_check_result_process` is replaced by `mpm_from_json_check_result_process`."
-    IssueDeprecationWarning("MPMApplication:",wrng_msg)
-    return MPMFromJsonCheckResultProcess(model, settings["Parameters"])
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+from KratosMultiphysics.MPMApplication.mpm_from_json_check_result_process import MPMFromJsonCheckResultProcess
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a model object")
+    wrng_msg = "Process `particle_from_json_check_result_process` is replaced by `mpm_from_json_check_result_process`."
+    IssueDeprecationWarning("MPMApplication:",wrng_msg)
+    return MPMFromJsonCheckResultProcess(model, settings["Parameters"])
```

## KratosMultiphysics/MPMApplication/particle_gid_output_process.py

 * *Ordering differences only*

```diff
@@ -1,15 +1,15 @@
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-from KratosMultiphysics.MPMApplication.mpm_gid_output_process import MPMGiDOutputProcess
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a model object")
-    wrng_msg = "Process `particle_gid_output_process` is replaced by `mpm_gid_output_process`."
-    IssueDeprecationWarning("MPMApplication:",wrng_msg)
-    model_part = model[settings["Parameters"]["model_part_name"].GetString()]
-    output_name = settings["Parameters"]["output_name"].GetString()
-    postprocess_parameters = settings["Parameters"]["postprocess_parameters"]
-    return ParticleGiDOutputProcess(model_part, output_name, postprocess_parameters)
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+from KratosMultiphysics.MPMApplication.mpm_gid_output_process import MPMGiDOutputProcess
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a model object")
+    wrng_msg = "Process `particle_gid_output_process` is replaced by `mpm_gid_output_process`."
+    IssueDeprecationWarning("MPMApplication:",wrng_msg)
+    model_part = model[settings["Parameters"]["model_part_name"].GetString()]
+    output_name = settings["Parameters"]["output_name"].GetString()
+    postprocess_parameters = settings["Parameters"]["postprocess_parameters"]
+    return ParticleGiDOutputProcess(model_part, output_name, postprocess_parameters)
```

## KratosMultiphysics/MPMApplication/mpm_from_json_check_result_process.py

 * *Ordering differences only*

```diff
@@ -1,396 +1,396 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-from KratosMultiphysics.json_utilities import read_external_json
-
-# Import KratosUnittest
-from KratosMultiphysics.KratosUnittest import isclose as t_isclose
-import KratosMultiphysics.KratosUnittest as KratosUnittest
-
-# Math import
-from math import log10, ceil
-
-def Factory(settings, Model):
-    if(type(settings) != KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    return MPMFromJsonCheckResultProcess(Model, settings["Parameters"])
-
-class LegacyFromJsonCheckResultProcess(KratosMultiphysics.Process, KratosUnittest.TestCase):
-    """This class is used in order to check results using a json file
-    containing the solution a given model part with a certain frequency
-
-    Only the member variables listed below should be accessed directly.
-
-    Public member variables:
-    model -- the model contaning the model_parts
-    settings -- Kratos parameters containing solver settings.
-    """
-
-    def __init__(self, model, params):
-        """ The default constructor of the class
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        model -- the model contaning the model_parts
-        settings -- Kratos parameters containing solver settings.
-        """
-        KratosMultiphysics.Process.__init__(self)
-
-        ## Settings string in json format
-        default_parameters = KratosMultiphysics.Parameters("""{
-            "help"                 : "This process checks the solution obtained from a given json file. It can be used for generating tests for a problem",
-            "check_variables"      : [],
-            "gauss_points_check_variables" : [],
-            "input_file_name"      : "",
-            "model_part_name"      : "",
-            "sub_model_part_name"  : "",
-            "check_for_flag"       : "",
-            "historical_value"     : true,
-            "tolerance"            : 1e-3,
-            "relative_tolerance"   : 1e-6,
-            "time_frequency"       : 1.00,
-            "use_node_coordinates" : false,
-            "check_only_local_entities" : false
-        }""")
-
-        ## Overwrite the default settings with user-provided parameters
-        params.ValidateAndAssignDefaults(default_parameters)
-        self.params = params
-        self.model  = model
-
-    def ExecuteInitialize(self):
-        """ This method is executed at the begining to initialize the process
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        # We get the submodelpart
-        model_part_name = self.params["model_part_name"].GetString()
-        sub_model_part_name = self.params["sub_model_part_name"].GetString()
-        if (sub_model_part_name != ""):
-            self.model_part = self.model[model_part_name].GetSubModelPart(sub_model_part_name)
-        else:
-            self.model_part = self.model[model_part_name]
-
-        # If we consider any flag
-        flag_name = self.params["check_for_flag"].GetString()
-        if flag_name != "":
-            self.flag = KratosMultiphysics.KratosGlobals.GetFlag(flag_name)
-        else:
-            self.flag = None
-
-        self.check_variables = self.__generate_variable_list_from_input(self.params["check_variables"])
-        self.gauss_points_check_variables = self.__generate_variable_list_from_input(self.params["gauss_points_check_variables"])
-        self.frequency = self.params["time_frequency"].GetDouble()
-        self.historical_value = self.params["historical_value"].GetBool()
-        self.data = read_external_json(self.params["input_file_name"].GetString())
-        self.abs_tol = self.params["tolerance"].GetDouble()
-        self.rel_tol = self.params["relative_tolerance"].GetDouble()
-        self.use_node_coordinates = self.params["use_node_coordinates"].GetBool()
-        self.check_only_local_entities = self.params["check_only_local_entities"].GetBool()
-        self.rel_tol_digits = ComputeRelevantDigits(self.rel_tol)
-        self.abs_tol_digits = ComputeRelevantDigits(self.abs_tol)
-
-        # Initialize counter
-        self.step_counter = 0
-        self.time_counter = 0.0
-
-    def ExecuteFinalizeSolutionStep(self):
-        """ This method is executed in order to finalize the current step
-
-        Here the dictionary containing the solution is filled
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        """
-        time = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.TIME)
-        dt = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.DELTA_TIME)
-        step = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.STEP)
-        self.time_counter += dt
-        if self.time_counter > self.frequency:
-            self.time_counter = 0.0
-            input_time_list = self.data["TIME"]
-
-            # Nodal values
-            for node in self.__get_nodes():
-                compute = self.__check_flag(node)
-
-                if compute:
-                    node_identifier = "NODE_" + self.__get_node_identifier(node)
-
-                    for i in range(self.params["check_variables"].size()):
-                        out = self.params["check_variables"][i]
-                        variable_name = out.GetString()
-                        variable = KratosMultiphysics.KratosGlobals.GetVariable( variable_name )
-                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
-
-                        if self.historical_value:
-                            value = node.GetSolutionStepValue(variable, 0)
-                        else:
-                            value = node.GetValue(variable)
-
-                        # Scalar variable
-                        if variable_type == "Double":
-                            values_json = self.data[node_identifier][variable_name]
-                            value_json = self.__linear_interpolation(time, input_time_list, values_json)
-                            self.__check_values(node.Id, "Node", value, value_json, variable_name)
-                        # Array variable
-                        elif variable_type == "Array":
-                            if KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double":
-                                for component_index, component in enumerate(["_X", "_Y", "_Z"]):
-                                    values_json = self.data[node_identifier][variable_name+component]
-                                    value_json = self.__linear_interpolation(time, input_time_list, values_json)
-                                    self.__check_values(node.Id, "Node", value[component_index], value_json, variable_name+component)
-                            else:
-                                values_json = self.data[node_identifier][variable_name][self.step_counter]
-                                for index in range(len(value)):
-                                    value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
-                                    self.__check_values(node.Id, "Node", value[index], value_json, variable_name)
-                        # Vector variable
-                        elif variable_type == "Vector":
-                            values_json = self.data[node_identifier][variable_name][self.step_counter]
-                            for index in range(len(value)):
-                                value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
-                                self.__check_values(node.Id, "Node", value[index], value_json, variable_name)
-            # Nodal values
-            for elem in self.__get_elements():
-                compute = self.__check_flag(elem)
-
-                if compute is True:
-                    for i in range(self.params["gauss_points_check_variables"].size()):
-                        out = self.params["gauss_points_check_variables"][i]
-                        variable_name = out.GetString()
-                        variable = KratosMultiphysics.KratosGlobals.GetVariable( variable_name )
-                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
-
-                        value = elem.CalculateOnIntegrationPoints(variable, self.model_part.ProcessInfo)
-
-                        gauss_point_number = len(value)
-
-                        # Scalar variable
-                        if variable_type == "Double":
-                            for gp in range(gauss_point_number):
-                                values_json = self.data["ELEMENT_"+str(elem.Id)][variable_name][str(gp)]
-                                value_json = self.__linear_interpolation(time, input_time_list, values_json)
-                                self.__check_values(elem.Id, "Element", value[gp], value_json, variable_name)
-                        # Array variable
-                        elif variable_type == "Array":
-                            if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
-                                for gp in range(gauss_point_number):
-                                    for component_index, component in enumerate(["_X", "_Y", "_Z"]):
-                                        values_json = self.data["ELEMENT_" + str(elem.Id)][variable_name+component][str(gp)]
-                                        value_json = self.__linear_interpolation(time, input_time_list, values_json)
-                                        self.__check_values(elem.Id, "Element", value[gp][component_index], value_json, variable_name+component)
-                            else:
-                                for gp in range(gauss_point_number):
-                                    values_json = self.data["ELEMENT_" + str(elem.Id)][variable_name][str(gp)][self.step_counter]
-                                    for index in range(len(value[gp])):
-                                        value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
-                                        self.__check_values(elem.Id, "Element", value[gp][index], value_json, variable_name)
-                        # Vector variable
-                        elif variable_type == "Vector":
-                            for gp in range(gauss_point_number):
-                                values_json = self.data["ELEMENT_" + str(elem.Id)][variable_name][str(gp)][self.step_counter]
-                                for index in range(len(value[gp])):
-                                    value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
-                                    self.__check_values(elem.Id, "Element", value[gp][index], value_json, variable_name)
-
-                        # TODO: Add pending classes
-
-            self.step_counter += 1
-
-    def __linear_interpolation(self, x, x_list, y_list):
-        """ This method is defined to interpolate values of a
-        list using the PiecewiseLinearTable from Kratos
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        x -- The value to interpolate
-        x_list -- Values in X axis
-        y_list -- Values in Y axis
-        """
-
-        tb = KratosMultiphysics.PiecewiseLinearTable()
-        for i in range(len(x_list)):
-            tb.AddRow(x_list[i], y_list[i])
-
-        return tb.GetNearestValue(x)
-
-    def __generate_variable_list_from_input(self,param):
-        """ Parse a list of variables from input.
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        value -- The Kratos vector to transform
-        """
-
-        # At least verify that the input is a string
-        if not param.IsArray():
-            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
-        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
-
-    def __check_flag(self, component):
-        """ Checks the flag over a component
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        component -- The Kratos node or element to check
-        """
-
-        if self.flag is not None:
-            if component.Is(self.flag) == False:
-                return False
-
-        return True
-
-    def __check_values(self, entity_id, entity_type, value_entity, value_json, variable_name):
-        """ Checks if two values are the same and issues a detailed error message
-        in case they do not match up to the specified tolerance
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        entity_id -- The Kratos node or element to check
-        entity_type -- The type of the entity
-        value_entity -- The value on the entity
-        value_json -- The reference value from the json
-        variable_name -- The name of the variable
-        """
-        relevant_digits = int(max(self.rel_tol_digits, self.abs_tol_digits))+1 # +1 for one more digit of output
-        isclosethis = t_isclose(value_entity, value_json, rel_tol=self.rel_tol, abs_tol=self.abs_tol)
-        msg  = 'Error checking {} #{} for variable {} results:\n'.format(entity_type, entity_id, variable_name)
-        msg += '%.*f != %.*f; rel_tol=%.*f, abs_tol=%.*f' % (relevant_digits, value_entity, relevant_digits, value_json, self.rel_tol_digits, self.rel_tol, self.abs_tol_digits, self.abs_tol)
-        self.assertTrue(isclosethis, msg=msg)
-
-    def __get_node_identifier(self, node):
-        """ returns the identifier/key for saving nodal results in the json
-        this can be either the node Id or its coordinates
-        The coordinates can be used to check the nodal results in MPI
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        node -- The Kratos node to get the identifier for
-        """
-        if self.use_node_coordinates:
-            digits = 6
-            return 'X_%.*f_Y_%.*f_Z_%.*f' % (digits, node.X0, digits, node.Y0, digits, node.Z0)
-        else:
-            return str(node.Id)
-
-    def __get_nodes(self):
-        """ returns the nodes to be checked
-        Either only local or all (local and ghost)
-        This is ONLY relevant in MPI
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        node -- The Kratos node to get the identifier for
-        """
-        if self.check_only_local_entities:
-            return self.model_part.GetCommunicator().LocalMesh().Nodes
-        else:
-            return self.model_part.Nodes
-
-    def __get_elements(self):
-        """ returns the elements to be checked
-        Either only local or all (local and ghost)
-        This is ONLY relevant in MPI
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        node -- The Kratos node to get the identifier for
-        """
-        if self.check_only_local_entities:
-            return self.model_part.GetCommunicator().LocalMesh().Elements
-        else:
-            return self.model_part.Elements
-
-def ComputeRelevantDigits(number):
-    """ Computes the relevant digits
-
-    Keyword arguments:
-    self -- It signifies an instance of a class.
-    """
-    return int(ceil(abs(log10(number))))
-class MPMFromJsonCheckResultProcess(LegacyFromJsonCheckResultProcess, KratosUnittest.TestCase): # TODO: This must be updated to the new C++ version
-
-    def __init__(self, model_part, params):
-        super(MPMFromJsonCheckResultProcess, self).__init__(model_part, params)
-
-    def ExecuteFinalizeSolutionStep(self):
-
-        tol = self.params["tolerance"].GetDouble()
-        reltol = self.params["relative_tolerance"].GetDouble()
-        time = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.TIME)
-        dt = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.DELTA_TIME)
-        step = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.STEP)
-        self.time_counter += dt
-        if self.time_counter > self.frequency:
-            self.time_counter = 0.0
-            input_time_list = self.data["TIME"]
-
-            # Material points values
-            for mp in self.model_part.Elements:
-                compute = self.__check_flag(mp)
-
-                if (compute == True):
-                    for i in range(self.params["check_variables"].size()):
-                        out = self.params["check_variables"][i]
-                        variable_name = out.GetString()
-                        variable = KratosMultiphysics.KratosGlobals.GetVariable( variable_name )
-                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
-                        value = mp.CalculateOnIntegrationPoints(variable,self.model_part.ProcessInfo)[0]
-
-                        # Scalar variable
-                        if (variable_type == "Double" or variable_type == "Integer" or variable_type == "Component"):
-                            values_json = self.data["MP_" + str(mp.Id)][variable_name]
-                            value_json = self.__linear_interpolation(time, input_time_list, values_json)
-                            isclosethis = t_isclose(value, value_json, rel_tol=reltol, abs_tol=tol)
-                            self.assertTrue(isclosethis, msg=(str(value) + " != " + str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
-                        # Array variable
-                        elif variable_type == "Array":
-
-                            if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
-                                for component_index, component in enumerate(["_X", "_Y", "_Z"]):
-                                    values_json = self.data["MP_" + str(mp.Id)][variable_name +component]
-                                    value_json = self.__linear_interpolation(time, input_time_list, values_json)
-                                    isclosethis = t_isclose(value[component_index], value_json, rel_tol=reltol, abs_tol=tol)
-                                    self.assertTrue(isclosethis, msg=(str(value[component_index]) + " != "+str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
-                            else:
-                                values_json = self.data["MP_"+str(mp.Id)][variable_name][step - 1]
-                                for index in range(len(value)):
-                                    value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
-                                    isclosethis = t_isclose(value[index], value_json, rel_tol=reltol, abs_tol=tol)
-                                    self.assertTrue(isclosethis, msg=(str(value) + " != " + str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
-                        # Vector variable
-                        elif variable_type == "Vector":
-                            values_json = self.data["MP_"+str(mp.Id)][variable_name][step - 1]
-                            for index in range(len(value)):
-                                value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
-                                isclosethis = t_isclose(value[index], value_json, rel_tol=reltol, abs_tol=tol)
-                                self.assertTrue(isclosethis, msg=(str(value) + " != " + str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
-
-    def __linear_interpolation(self, x, x_list, y_list):
-
-        tb = KratosMultiphysics.PiecewiseLinearTable()
-        for i in range(len(x_list)):
-            tb.AddRow(x_list[i], y_list[i])
-
-        return tb.GetNearestValue(x)
-
-    def __generate_variable_list_from_input(self,param):
-
-        # At least verify that the input is a string
-        if not param.IsArray():
-            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
-
-        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
-        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
-
-    def __check_flag(self, component):
-
-        if self.flag != None:
-            if component.Is(self.flag) == False:
-                return False
-
-        return True
+# Importing the Kratos Library
+import KratosMultiphysics
+from KratosMultiphysics.json_utilities import read_external_json
+
+# Import KratosUnittest
+from KratosMultiphysics.KratosUnittest import isclose as t_isclose
+import KratosMultiphysics.KratosUnittest as KratosUnittest
+
+# Math import
+from math import log10, ceil
+
+def Factory(settings, Model):
+    if(type(settings) != KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    return MPMFromJsonCheckResultProcess(Model, settings["Parameters"])
+
+class LegacyFromJsonCheckResultProcess(KratosMultiphysics.Process, KratosUnittest.TestCase):
+    """This class is used in order to check results using a json file
+    containing the solution a given model part with a certain frequency
+
+    Only the member variables listed below should be accessed directly.
+
+    Public member variables:
+    model -- the model contaning the model_parts
+    settings -- Kratos parameters containing solver settings.
+    """
+
+    def __init__(self, model, params):
+        """ The default constructor of the class
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        model -- the model contaning the model_parts
+        settings -- Kratos parameters containing solver settings.
+        """
+        KratosMultiphysics.Process.__init__(self)
+
+        ## Settings string in json format
+        default_parameters = KratosMultiphysics.Parameters("""{
+            "help"                 : "This process checks the solution obtained from a given json file. It can be used for generating tests for a problem",
+            "check_variables"      : [],
+            "gauss_points_check_variables" : [],
+            "input_file_name"      : "",
+            "model_part_name"      : "",
+            "sub_model_part_name"  : "",
+            "check_for_flag"       : "",
+            "historical_value"     : true,
+            "tolerance"            : 1e-3,
+            "relative_tolerance"   : 1e-6,
+            "time_frequency"       : 1.00,
+            "use_node_coordinates" : false,
+            "check_only_local_entities" : false
+        }""")
+
+        ## Overwrite the default settings with user-provided parameters
+        params.ValidateAndAssignDefaults(default_parameters)
+        self.params = params
+        self.model  = model
+
+    def ExecuteInitialize(self):
+        """ This method is executed at the begining to initialize the process
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        # We get the submodelpart
+        model_part_name = self.params["model_part_name"].GetString()
+        sub_model_part_name = self.params["sub_model_part_name"].GetString()
+        if (sub_model_part_name != ""):
+            self.model_part = self.model[model_part_name].GetSubModelPart(sub_model_part_name)
+        else:
+            self.model_part = self.model[model_part_name]
+
+        # If we consider any flag
+        flag_name = self.params["check_for_flag"].GetString()
+        if flag_name != "":
+            self.flag = KratosMultiphysics.KratosGlobals.GetFlag(flag_name)
+        else:
+            self.flag = None
+
+        self.check_variables = self.__generate_variable_list_from_input(self.params["check_variables"])
+        self.gauss_points_check_variables = self.__generate_variable_list_from_input(self.params["gauss_points_check_variables"])
+        self.frequency = self.params["time_frequency"].GetDouble()
+        self.historical_value = self.params["historical_value"].GetBool()
+        self.data = read_external_json(self.params["input_file_name"].GetString())
+        self.abs_tol = self.params["tolerance"].GetDouble()
+        self.rel_tol = self.params["relative_tolerance"].GetDouble()
+        self.use_node_coordinates = self.params["use_node_coordinates"].GetBool()
+        self.check_only_local_entities = self.params["check_only_local_entities"].GetBool()
+        self.rel_tol_digits = ComputeRelevantDigits(self.rel_tol)
+        self.abs_tol_digits = ComputeRelevantDigits(self.abs_tol)
+
+        # Initialize counter
+        self.step_counter = 0
+        self.time_counter = 0.0
+
+    def ExecuteFinalizeSolutionStep(self):
+        """ This method is executed in order to finalize the current step
+
+        Here the dictionary containing the solution is filled
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        """
+        time = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.TIME)
+        dt = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.DELTA_TIME)
+        step = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.STEP)
+        self.time_counter += dt
+        if self.time_counter > self.frequency:
+            self.time_counter = 0.0
+            input_time_list = self.data["TIME"]
+
+            # Nodal values
+            for node in self.__get_nodes():
+                compute = self.__check_flag(node)
+
+                if compute:
+                    node_identifier = "NODE_" + self.__get_node_identifier(node)
+
+                    for i in range(self.params["check_variables"].size()):
+                        out = self.params["check_variables"][i]
+                        variable_name = out.GetString()
+                        variable = KratosMultiphysics.KratosGlobals.GetVariable( variable_name )
+                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
+
+                        if self.historical_value:
+                            value = node.GetSolutionStepValue(variable, 0)
+                        else:
+                            value = node.GetValue(variable)
+
+                        # Scalar variable
+                        if variable_type == "Double":
+                            values_json = self.data[node_identifier][variable_name]
+                            value_json = self.__linear_interpolation(time, input_time_list, values_json)
+                            self.__check_values(node.Id, "Node", value, value_json, variable_name)
+                        # Array variable
+                        elif variable_type == "Array":
+                            if KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double":
+                                for component_index, component in enumerate(["_X", "_Y", "_Z"]):
+                                    values_json = self.data[node_identifier][variable_name+component]
+                                    value_json = self.__linear_interpolation(time, input_time_list, values_json)
+                                    self.__check_values(node.Id, "Node", value[component_index], value_json, variable_name+component)
+                            else:
+                                values_json = self.data[node_identifier][variable_name][self.step_counter]
+                                for index in range(len(value)):
+                                    value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
+                                    self.__check_values(node.Id, "Node", value[index], value_json, variable_name)
+                        # Vector variable
+                        elif variable_type == "Vector":
+                            values_json = self.data[node_identifier][variable_name][self.step_counter]
+                            for index in range(len(value)):
+                                value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
+                                self.__check_values(node.Id, "Node", value[index], value_json, variable_name)
+            # Nodal values
+            for elem in self.__get_elements():
+                compute = self.__check_flag(elem)
+
+                if compute is True:
+                    for i in range(self.params["gauss_points_check_variables"].size()):
+                        out = self.params["gauss_points_check_variables"][i]
+                        variable_name = out.GetString()
+                        variable = KratosMultiphysics.KratosGlobals.GetVariable( variable_name )
+                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
+
+                        value = elem.CalculateOnIntegrationPoints(variable, self.model_part.ProcessInfo)
+
+                        gauss_point_number = len(value)
+
+                        # Scalar variable
+                        if variable_type == "Double":
+                            for gp in range(gauss_point_number):
+                                values_json = self.data["ELEMENT_"+str(elem.Id)][variable_name][str(gp)]
+                                value_json = self.__linear_interpolation(time, input_time_list, values_json)
+                                self.__check_values(elem.Id, "Element", value[gp], value_json, variable_name)
+                        # Array variable
+                        elif variable_type == "Array":
+                            if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
+                                for gp in range(gauss_point_number):
+                                    for component_index, component in enumerate(["_X", "_Y", "_Z"]):
+                                        values_json = self.data["ELEMENT_" + str(elem.Id)][variable_name+component][str(gp)]
+                                        value_json = self.__linear_interpolation(time, input_time_list, values_json)
+                                        self.__check_values(elem.Id, "Element", value[gp][component_index], value_json, variable_name+component)
+                            else:
+                                for gp in range(gauss_point_number):
+                                    values_json = self.data["ELEMENT_" + str(elem.Id)][variable_name][str(gp)][self.step_counter]
+                                    for index in range(len(value[gp])):
+                                        value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
+                                        self.__check_values(elem.Id, "Element", value[gp][index], value_json, variable_name)
+                        # Vector variable
+                        elif variable_type == "Vector":
+                            for gp in range(gauss_point_number):
+                                values_json = self.data["ELEMENT_" + str(elem.Id)][variable_name][str(gp)][self.step_counter]
+                                for index in range(len(value[gp])):
+                                    value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
+                                    self.__check_values(elem.Id, "Element", value[gp][index], value_json, variable_name)
+
+                        # TODO: Add pending classes
+
+            self.step_counter += 1
+
+    def __linear_interpolation(self, x, x_list, y_list):
+        """ This method is defined to interpolate values of a
+        list using the PiecewiseLinearTable from Kratos
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        x -- The value to interpolate
+        x_list -- Values in X axis
+        y_list -- Values in Y axis
+        """
+
+        tb = KratosMultiphysics.PiecewiseLinearTable()
+        for i in range(len(x_list)):
+            tb.AddRow(x_list[i], y_list[i])
+
+        return tb.GetNearestValue(x)
+
+    def __generate_variable_list_from_input(self,param):
+        """ Parse a list of variables from input.
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        value -- The Kratos vector to transform
+        """
+
+        # At least verify that the input is a string
+        if not param.IsArray():
+            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
+        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
+
+    def __check_flag(self, component):
+        """ Checks the flag over a component
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        component -- The Kratos node or element to check
+        """
+
+        if self.flag is not None:
+            if component.Is(self.flag) == False:
+                return False
+
+        return True
+
+    def __check_values(self, entity_id, entity_type, value_entity, value_json, variable_name):
+        """ Checks if two values are the same and issues a detailed error message
+        in case they do not match up to the specified tolerance
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        entity_id -- The Kratos node or element to check
+        entity_type -- The type of the entity
+        value_entity -- The value on the entity
+        value_json -- The reference value from the json
+        variable_name -- The name of the variable
+        """
+        relevant_digits = int(max(self.rel_tol_digits, self.abs_tol_digits))+1 # +1 for one more digit of output
+        isclosethis = t_isclose(value_entity, value_json, rel_tol=self.rel_tol, abs_tol=self.abs_tol)
+        msg  = 'Error checking {} #{} for variable {} results:\n'.format(entity_type, entity_id, variable_name)
+        msg += '%.*f != %.*f; rel_tol=%.*f, abs_tol=%.*f' % (relevant_digits, value_entity, relevant_digits, value_json, self.rel_tol_digits, self.rel_tol, self.abs_tol_digits, self.abs_tol)
+        self.assertTrue(isclosethis, msg=msg)
+
+    def __get_node_identifier(self, node):
+        """ returns the identifier/key for saving nodal results in the json
+        this can be either the node Id or its coordinates
+        The coordinates can be used to check the nodal results in MPI
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        node -- The Kratos node to get the identifier for
+        """
+        if self.use_node_coordinates:
+            digits = 6
+            return 'X_%.*f_Y_%.*f_Z_%.*f' % (digits, node.X0, digits, node.Y0, digits, node.Z0)
+        else:
+            return str(node.Id)
+
+    def __get_nodes(self):
+        """ returns the nodes to be checked
+        Either only local or all (local and ghost)
+        This is ONLY relevant in MPI
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        node -- The Kratos node to get the identifier for
+        """
+        if self.check_only_local_entities:
+            return self.model_part.GetCommunicator().LocalMesh().Nodes
+        else:
+            return self.model_part.Nodes
+
+    def __get_elements(self):
+        """ returns the elements to be checked
+        Either only local or all (local and ghost)
+        This is ONLY relevant in MPI
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        node -- The Kratos node to get the identifier for
+        """
+        if self.check_only_local_entities:
+            return self.model_part.GetCommunicator().LocalMesh().Elements
+        else:
+            return self.model_part.Elements
+
+def ComputeRelevantDigits(number):
+    """ Computes the relevant digits
+
+    Keyword arguments:
+    self -- It signifies an instance of a class.
+    """
+    return int(ceil(abs(log10(number))))
+class MPMFromJsonCheckResultProcess(LegacyFromJsonCheckResultProcess, KratosUnittest.TestCase): # TODO: This must be updated to the new C++ version
+
+    def __init__(self, model_part, params):
+        super(MPMFromJsonCheckResultProcess, self).__init__(model_part, params)
+
+    def ExecuteFinalizeSolutionStep(self):
+
+        tol = self.params["tolerance"].GetDouble()
+        reltol = self.params["relative_tolerance"].GetDouble()
+        time = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.TIME)
+        dt = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.DELTA_TIME)
+        step = self.model_part.ProcessInfo.GetValue(KratosMultiphysics.STEP)
+        self.time_counter += dt
+        if self.time_counter > self.frequency:
+            self.time_counter = 0.0
+            input_time_list = self.data["TIME"]
+
+            # Material points values
+            for mp in self.model_part.Elements:
+                compute = self.__check_flag(mp)
+
+                if (compute == True):
+                    for i in range(self.params["check_variables"].size()):
+                        out = self.params["check_variables"][i]
+                        variable_name = out.GetString()
+                        variable = KratosMultiphysics.KratosGlobals.GetVariable( variable_name )
+                        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
+                        value = mp.CalculateOnIntegrationPoints(variable,self.model_part.ProcessInfo)[0]
+
+                        # Scalar variable
+                        if (variable_type == "Double" or variable_type == "Integer" or variable_type == "Component"):
+                            values_json = self.data["MP_" + str(mp.Id)][variable_name]
+                            value_json = self.__linear_interpolation(time, input_time_list, values_json)
+                            isclosethis = t_isclose(value, value_json, rel_tol=reltol, abs_tol=tol)
+                            self.assertTrue(isclosethis, msg=(str(value) + " != " + str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
+                        # Array variable
+                        elif variable_type == "Array":
+
+                            if (KratosMultiphysics.KratosGlobals.GetVariableType(variable_name + "_X") == "Double"):
+                                for component_index, component in enumerate(["_X", "_Y", "_Z"]):
+                                    values_json = self.data["MP_" + str(mp.Id)][variable_name +component]
+                                    value_json = self.__linear_interpolation(time, input_time_list, values_json)
+                                    isclosethis = t_isclose(value[component_index], value_json, rel_tol=reltol, abs_tol=tol)
+                                    self.assertTrue(isclosethis, msg=(str(value[component_index]) + " != "+str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
+                            else:
+                                values_json = self.data["MP_"+str(mp.Id)][variable_name][step - 1]
+                                for index in range(len(value)):
+                                    value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
+                                    isclosethis = t_isclose(value[index], value_json, rel_tol=reltol, abs_tol=tol)
+                                    self.assertTrue(isclosethis, msg=(str(value) + " != " + str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
+                        # Vector variable
+                        elif variable_type == "Vector":
+                            values_json = self.data["MP_"+str(mp.Id)][variable_name][step - 1]
+                            for index in range(len(value)):
+                                value_json = values_json[index] # self.__linear_interpolation(time, input_time_list, values_json[index])
+                                isclosethis = t_isclose(value[index], value_json, rel_tol=reltol, abs_tol=tol)
+                                self.assertTrue(isclosethis, msg=(str(value) + " != " + str(value_json) + ", rel_tol = " + str(reltol) + ", abs_tol = " + str(tol) + " : Error checking material point " + str(mp.Id) + " " + variable_name + " results."))
+
+    def __linear_interpolation(self, x, x_list, y_list):
+
+        tb = KratosMultiphysics.PiecewiseLinearTable()
+        for i in range(len(x_list)):
+            tb.AddRow(x_list[i], y_list[i])
+
+        return tb.GetNearestValue(x)
+
+    def __generate_variable_list_from_input(self,param):
+
+        # At least verify that the input is a string
+        if not param.IsArray():
+            raise Exception("{0} Error: Variable list is unreadable".format(self.__class__.__name__))
+
+        # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
+        return [ KratosMultiphysics.KratosGlobals.GetVariable( param[i].GetString() ) for i in range( 0,param.size() ) ]
+
+    def __check_flag(self, component):
+
+        if self.flag != None:
+            if component.Is(self.flag) == False:
+                return False
+
+        return True
```

## KratosMultiphysics/MPMApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-from KratosMultiphysics import _ImportApplication
-from KratosMPMApplication import *
-application = KratosMPMApplication()
-application_name = "KratosMPMApplication"
-
-_ImportApplication(application, application_name)
+from KratosMultiphysics import _ImportApplication
+from KratosMPMApplication import *
+application = KratosMPMApplication()
+application_name = "KratosMPMApplication"
+
+_ImportApplication(application, application_name)
```

## KratosMultiphysics/MPMApplication/mpm_vtk_condition_output_process.py

 * *Ordering differences only*

```diff
@@ -1,114 +1,114 @@
-import numpy as np
-import KratosMultiphysics
-from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
-import KratosMultiphysics.MPMApplication as KratosMPM
-from KratosMultiphysics.MPMApplication.mpm_vtk_output_process import MPMVtkOutputProcess
-
-# Import time library
-from time import time
-
-def Factory(settings: KratosMultiphysics.Parameters, model: KratosMultiphysics.Model) -> KratosMultiphysics.OutputProcess:
-    if not isinstance(model, KratosMultiphysics.Model):
-        raise Exception("expected input shall be a Model object, encapsulating a json string")
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    IssueDeprecationWarning("MPMApplication:","`MPMConditionVTKOutputProcess` is deprecated and replaced with `MPMVtkOutputProcess`")
-    return MPMVtkOutputProcess(model, settings["Parameters"])
-
-class LegacyMPMConditionVTKOutputProcess(MPMVtkOutputProcess):
-    defaults = KratosMultiphysics.Parameters("""{
-        "model_part_name"                    : "MPM_Material",
-        "output_control_type"                : "step",
-        "output_interval"                   : 1,
-        "file_format"                        : "ascii",
-        "output_precision"                   : 7,
-        "folder_name"                        : "vtk_condition_output",
-        "output_sub_model_parts"             : false,
-        "save_output_files_in_folder"        : true,
-        "gauss_point_results" : []
-    }""")
-
-    def __init__(self, model_part, param, Model):
-
-        if param is None:
-            param = self.defaults
-        else:
-            param.ValidateAndAssignDefaults(self.defaults)
-
-        self.model = Model
-        self.param = param
-        self.model_part = model_part
-
-        # Initiate base class - material point output
-        MPMVTKOutputProcess.__init__(self, model_part, param)
-
-    def ExecuteBeforeSolutionLoop(self): 
-        if (self.problem_name.startswith('Background_Grid.')):
-            self.problem_name = self.problem_name.replace('Background_Grid.','')
-        mpm_material_model_part_name = "MPM_Material." + self.problem_name
-        self.model_part = self.model[mpm_material_model_part_name]
-
-
-    def _get_mp_coords(self):
-        number_of_mps = self.model_part.NumberOfConditions(0)
-        if len(self.coords_X) != number_of_mps:
-            self.coords_X = np.empty(number_of_mps)
-            self.coords_Y = np.empty(number_of_mps)
-            self.coords_Z = np.empty(number_of_mps)
-
-        i = 0
-        for mpc in self.model_part.Conditions:
-            coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
-            self.coords_X[i] = coord[0]
-            self.coords_Y[i] = coord[1]
-            self.coords_Z[i] = coord[2]
-            i += 1
-
-    def _get_mp_results(self):
-        clock_time = self._start_time_measure()
-        number_of_results = self.variable_name_list.size()
-        number_of_mps = self.model_part.NumberOfConditions(0)
-
-        if len(self.result_names) != number_of_results:
-            self.result_names = ["dummy"]*number_of_results
-        if len(self.temp_results) != number_of_results:
-            self.temp_results = np.empty([number_of_mps,3])
-
-        for result_index in range(number_of_results):
-            var_name = self.variable_name_list[result_index].GetString()
-            self.result_names[result_index] = var_name
-
-            variable = self.variable_list[result_index]
-            var_size = 0
-            is_scalar = self._is_scalar(variable)
-
-            # Write in result file
-            mpc_index = 0
-            for mpc in self.model_part.Conditions:
-                print_variable = mpc.CalculateOnIntegrationPoints(variable,self.model_part.ProcessInfo)[0]
-                if is_scalar:
-                    self.temp_results[mpc_index,0] = print_variable
-                else:
-                    var_size =  print_variable.Size()
-                    if var_size == 1 or var_size == 3:
-                        for i in range(var_size):
-                            self.temp_results[mpc_index,i] = print_variable[i]
-                    else:
-                        KratosMultiphysics.Logger.PrintInfo("Warning in mpm vtk condition output", "Printing format is not defined for variable: ", var_name, "with size: ", var_size)
-
-                mpc_index += 1
-
-            # store in dictionary
-            if var_size == 1 or is_scalar:
-                self.result_dict[var_name] = self._GetCSlice(0)
-            elif var_size == 3:
-                #self.result_dict[var_name] = (self.temp_results[:,0],self.temp_results[:,1],self.temp_results[:,2])
-                self.result_dict[var_name] = (self._GetCSlice(0),self._GetCSlice(1),self._GetCSlice(2))
-            else:
-                KratosMultiphysics.Logger.PrintInfo("Warning in mpm vtk condition output", "Printing format is not defined for variable: ", var_name, "with size: ", var_size)
-
-        self._stop_time_measure(clock_time)
-
-    def _stop_time_measure(self, time_ip):
-        time_fp = time()
-        KratosMultiphysics.Logger.PrintInfo("::[Material Point Condition VTK Output Process]:: ", "[Spent time for output = ", time_fp - time_ip, "sec]")
+import numpy as np
+import KratosMultiphysics
+from KratosMultiphysics.kratos_utilities import IssueDeprecationWarning
+import KratosMultiphysics.MPMApplication as KratosMPM
+from KratosMultiphysics.MPMApplication.mpm_vtk_output_process import MPMVtkOutputProcess
+
+# Import time library
+from time import time
+
+def Factory(settings: KratosMultiphysics.Parameters, model: KratosMultiphysics.Model) -> KratosMultiphysics.OutputProcess:
+    if not isinstance(model, KratosMultiphysics.Model):
+        raise Exception("expected input shall be a Model object, encapsulating a json string")
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    IssueDeprecationWarning("MPMApplication:","`MPMConditionVTKOutputProcess` is deprecated and replaced with `MPMVtkOutputProcess`")
+    return MPMVtkOutputProcess(model, settings["Parameters"])
+
+class LegacyMPMConditionVTKOutputProcess(MPMVtkOutputProcess):
+    defaults = KratosMultiphysics.Parameters("""{
+        "model_part_name"                    : "MPM_Material",
+        "output_control_type"                : "step",
+        "output_interval"                   : 1,
+        "file_format"                        : "ascii",
+        "output_precision"                   : 7,
+        "folder_name"                        : "vtk_condition_output",
+        "output_sub_model_parts"             : false,
+        "save_output_files_in_folder"        : true,
+        "gauss_point_results" : []
+    }""")
+
+    def __init__(self, model_part, param, Model):
+
+        if param is None:
+            param = self.defaults
+        else:
+            param.ValidateAndAssignDefaults(self.defaults)
+
+        self.model = Model
+        self.param = param
+        self.model_part = model_part
+
+        # Initiate base class - material point output
+        MPMVTKOutputProcess.__init__(self, model_part, param)
+
+    def ExecuteBeforeSolutionLoop(self): 
+        if (self.problem_name.startswith('Background_Grid.')):
+            self.problem_name = self.problem_name.replace('Background_Grid.','')
+        mpm_material_model_part_name = "MPM_Material." + self.problem_name
+        self.model_part = self.model[mpm_material_model_part_name]
+
+
+    def _get_mp_coords(self):
+        number_of_mps = self.model_part.NumberOfConditions(0)
+        if len(self.coords_X) != number_of_mps:
+            self.coords_X = np.empty(number_of_mps)
+            self.coords_Y = np.empty(number_of_mps)
+            self.coords_Z = np.empty(number_of_mps)
+
+        i = 0
+        for mpc in self.model_part.Conditions:
+            coord = mpc.CalculateOnIntegrationPoints(KratosMPM.MPC_COORD,self.model_part.ProcessInfo)[0]
+            self.coords_X[i] = coord[0]
+            self.coords_Y[i] = coord[1]
+            self.coords_Z[i] = coord[2]
+            i += 1
+
+    def _get_mp_results(self):
+        clock_time = self._start_time_measure()
+        number_of_results = self.variable_name_list.size()
+        number_of_mps = self.model_part.NumberOfConditions(0)
+
+        if len(self.result_names) != number_of_results:
+            self.result_names = ["dummy"]*number_of_results
+        if len(self.temp_results) != number_of_results:
+            self.temp_results = np.empty([number_of_mps,3])
+
+        for result_index in range(number_of_results):
+            var_name = self.variable_name_list[result_index].GetString()
+            self.result_names[result_index] = var_name
+
+            variable = self.variable_list[result_index]
+            var_size = 0
+            is_scalar = self._is_scalar(variable)
+
+            # Write in result file
+            mpc_index = 0
+            for mpc in self.model_part.Conditions:
+                print_variable = mpc.CalculateOnIntegrationPoints(variable,self.model_part.ProcessInfo)[0]
+                if is_scalar:
+                    self.temp_results[mpc_index,0] = print_variable
+                else:
+                    var_size =  print_variable.Size()
+                    if var_size == 1 or var_size == 3:
+                        for i in range(var_size):
+                            self.temp_results[mpc_index,i] = print_variable[i]
+                    else:
+                        KratosMultiphysics.Logger.PrintInfo("Warning in mpm vtk condition output", "Printing format is not defined for variable: ", var_name, "with size: ", var_size)
+
+                mpc_index += 1
+
+            # store in dictionary
+            if var_size == 1 or is_scalar:
+                self.result_dict[var_name] = self._GetCSlice(0)
+            elif var_size == 3:
+                #self.result_dict[var_name] = (self.temp_results[:,0],self.temp_results[:,1],self.temp_results[:,2])
+                self.result_dict[var_name] = (self._GetCSlice(0),self._GetCSlice(1),self._GetCSlice(2))
+            else:
+                KratosMultiphysics.Logger.PrintInfo("Warning in mpm vtk condition output", "Printing format is not defined for variable: ", var_name, "with size: ", var_size)
+
+        self._stop_time_measure(clock_time)
+
+    def _stop_time_measure(self, time_ip):
+        time_fp = time()
+        KratosMultiphysics.Logger.PrintInfo("::[Material Point Condition VTK Output Process]:: ", "[Spent time for output = ", time_fp - time_ip, "sec]")
```

## Comparing `KratosMPMApplication-9.5.dist-info/METADATA` & `KratosMPMApplication-9.5.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,136 +1,137 @@
-Metadata-Version: 2.1
-Name: KratosMPMApplication
-Version: 9.5
-Summary: KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-disciplinary simulation software, aiming at modularity, extensibility, and high performance. Kratos is written in C++, and counts with an extensive Python interface.
-Home-page: https://github.com/KratosMultiphysics/
-Author: Kratos Team
-Author-email: kratos@listas.cimne.upc.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Other Audience
-Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: KratosMultiphysics ==9.5
-Requires-Dist: KratosLinearSolversApplication ==9.5
-
-# MPM Application
-
-This application implements the Material Point Method (MPM) with main motivations of simulating non-linear large deformable materials, such as free-surface flows, geomechanical phenomena, and extreme events involving impact, penetration, fragmentation, blast, multi-phase interaction, failure evolution, etc.
-
-<p align="center">
-  <img src="https://github.com/KratosMultiphysics/Documentation/blob/master/Readme_files/MPMApplication.gif" width="618" height="280"/>
-</p>
-
-
-## Getting Started
-
-This application is part of the Kratos Multiphysics Platform. Instructions on how to download, install and run the software in your local machine for development and testing purposes are available for both Linux and Windows distributions [Installation page](https://github.com/KratosMultiphysics/Kratos/blob/master/INSTALL.md).
-
-### Prerequisites
-
-Build Kratos and check the [configuration files](https://github.com/KratosMultiphysics/Kratos/blob/master/INSTALL.md#configuration-scripts-examples)
-
-
-In LINUX: check that in the /path_to_kratos/scripts/configure.sh the followinglines are written:
-
-``` cmake
--DMPM_APPLICATION=ON
--DLINEAR_SOLVERS_APPLICATION=ON
-```
-
-In WINDOWS: check that in the /path_to_kratos/scripts/configute.bat the following lines appears:
-
-```set KRATOS_APPLICATIONS=
-CALL :add_app %KRATOS_APP_DIR%\LinearSolversApplication;
-CALL :add_app %KRATOS_APP_DIR%\MPMApplication;
-```
-
-so the MPM application is compiled along with auxiliary linear solvers required.
-
-## Examples
-Some use-cases and validation examples are available in the MPM section of the [Examples](https://kratosmultiphysics.github.io/Examples/) repository. Also, some unit tests of the main features can be found in the [tests](https://github.com/KratosMultiphysics/Kratos/tree/master/applications/MPMApplication/tests) folder.
-
-### GiD Interface
-A GiD user interface for the MPM application is also available. It is located in GiD interface repository in [GiD interface repository](https://github.com/KratosMultiphysics/GiDInterface/tree/master/).
-
-It requires [GiD](https://www.gidhome.com/) - Pre and Post Processing software.
-
-## Theory
-
-Particle or meshfree methods are a category of methods where the state of a system is represented by a set of particles, without a fixed connectivity; hence, making such methods suitable for the analysis of moving discontinuities and large deformations with breaking and fragmentation. This approach does not suffer from the mesh distortion and entanglement issues posed by other Lagrangian discretizations such as the finite element method.
-
-### Material Point Method
-
-The MPM is an hybrid thechnique which uses a fixed background grid (or mesh) for solving the governing equations in a FEM fashion and  set of material particles (MP) for storing all the hystorical variables and material informations. MPM has gained a remarkably increasing popularity due to its capability in simulating  problems involving historically dependent materials and large deformations. As MPM is able to combine the strengths of Eulerian and Lagrangian methods, it has been utilized in various engineering applications and industrial purposes, in particular in geomechanics and environmental fluid dynamics field.
-
-Recommended references for implementation details of MPM in Kratos:
-- Singer, V.; Sautter, K.B., Larese, A., Wüchner, R.; Bletzinger, K.U.; A partitioned material point method and discrete element method coupling scheme, Advanced Modeling and Simulation in Engineering Sciences, 9(16), (2022); DOI: https://doi.org/10.1186/s40323-022-00229-5
-- Chandra, B., Singer, V., Teschemacher, T., Wuechner, R., & Larese, A. (2021). Nonconforming Dirichlet boundary conditions in implicit material point method by means of penalty augmentation. Acta Geotechnica, 16(8), 2315-2335. DOI: 10.1007/s11440-020-01123-3
-- Wilson, P., Wüchner, R., & Fernando, D. (2021). Distillation of the material point method cell crossing error leading to a novel quadrature‐based C 0 remedy. International Journal for Numerical Methods in Engineering, 122(6), 1513-1537.
-- Iaconeta, I., Larese, A., Rossi, R., & Oñate, E. (2018). A stabilized mixed implicit Material Point Method for non-linear incompressible solid mechanics. *Computational Mechanics*, 1-18. DOI 10.1007/s00466-018-1647-9
-- Iaconeta, I., Larese, A., Rossi, R., & Zhiming, G. (2016). Comparison of a material point method and a Galerkin meshfree method for the simulation of cohesive-frictional materials. *Materials*, 10(10), p. 1150. doi: 10.3390/ma10101150
--
-## Features
-
-The following features are currently available and subject to development within the MPM Application:
-- Formulation:
-  * Irreducible formulations (U displacement based)
-  * Mixed UP formulations
-
-- Element types:
-    * Updated Lagrangian elements - triangular and quadrilatera (2D) and tetrahedral and hexahedral (3D), structured and unstructured, using classical or partitioned quadrature rules (this latter limited to explicit MPM)
-    * Updated Lagrangian axis-symmetric elements - triangular and quadrilateral (2D), structured and unstructured
-    * Updated Lagrangian mixed UP elements - triangular (2D) and tetrahedral (3D), structured and unstructured, stabilized using  Variational Multiscale Stabilization or Pressure Projection techniques
-
-- Constitutive laws:
-    * Linear isotropic elastic materials - plane strain, plane stress, axis-symmetric, and 3D
-    * Hyperelastic Neo-Hookean laws - finite strain, plane strain, axis-symmetric, and 3D
-    * Elasto-plastic laws:
-        * Mohr Coulomb - finite strain, associative and non-associative, plane strain, axis-symmetric, and 3D
-        * Mohr Coulomb with Strain Softening - finite strain, associative and non-associative, plane strain, axis-symmetric, and 3D
-    * Critical state laws:
-        * Modified Cam-Clay - finite strain, plane strain, axis-symmetric, and 3D
-        * Johnson Cook Thermal Plastic (just for explicit MPM)
-
-- A set of Boundary conditions:
-    * Grid-Based Conditions (conforming): applied directly on the background nodes
-        * Neumann: Point load
-        * Neumann: Line load (a distributed load applied over a line)
-        * Neumann: Surface load (a distributed load applied over a face)
-        * Dirichlet: Slip and No slip condition on arbitrary boundary.
-    * Material Point-Based Conditions (non conforming): applied in moveable boundary particles
-        * Neumann: Moving point load
-        * Dirichlet: Imposition of displacements (homogeneous and inhomogeneous) using penalty method
-
-- Strategies and schemes:
-    * Implicit - Newmark/Bossak prediction and correction scheme for static, quasi-static, and dynamic problems
-    * Explicit
-
-- Other features:
-    * Partitioned coupling with Finite Element Method - weak and strong coupling of nonconforming discretization
-    * Partitioned coupling with the Discrete Element Method
-    * material point erase features - to delete material points outside the interest domain
-
-## License
-
-The MPM Application is OPEN SOURCE. The main code and program structure is available and aimed to grow with the need of any user willing to expand it. The BSD (Berkeley Software Distribution) licence allows to use and distribute the existing code without any restriction, but with the possibility to develop new parts of the code on an open or close basis depending on the developers.
-
-## Contact
-
-* **Antonia Larese** - *Group Leader* - [antonia.larese@unipd.it](mailto:antonia.larese@unipd.it)
-* **Veronika Singer** - *Developer* - [veronika.singer@tum.de](mailto:veronika.singer@tum.de)
-* **Laura Moreno** - *Developer* - [laura.morenomartinez@unipd.it](mailto:laura.morenomartinez@unipd.it)
+Metadata-Version: 2.1
+Name: KratosMPMApplication
+Version: 9.5.1
+Summary: KRATOS Multiphysics ("Kratos") is a framework for building parallel, multi-disciplinary simulation software, aiming at modularity, extensibility, and high performance. Kratos is written in C++, and counts with an extensive Python interface.
+Home-page: https://github.com/KratosMultiphysics/
+Author: Kratos Team
+Author-email: kratos@listas.cimne.upc.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: BSD License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: KratosMultiphysics ==9.5.1
+Requires-Dist: KratosLinearSolversApplication ==9.5.1
+
+# MPM Application
+
+This application implements the Material Point Method (MPM) with main motivations of simulating non-linear large deformable materials, such as free-surface flows, geomechanical phenomena, and extreme events involving impact, penetration, fragmentation, blast, multi-phase interaction, failure evolution, etc.
+
+<p align="center">
+  <img src="https://github.com/KratosMultiphysics/Documentation/blob/master/Readme_files/MPMApplication.gif" width="618" height="280"/>
+</p>
+
+
+## Getting Started
+
+This application is part of the Kratos Multiphysics Platform. Instructions on how to download, install and run the software in your local machine for development and testing purposes are available for both Linux and Windows distributions [Installation page](https://github.com/KratosMultiphysics/Kratos/blob/master/INSTALL.md).
+
+### Prerequisites
+
+Build Kratos and check the [configuration files](https://github.com/KratosMultiphysics/Kratos/blob/master/INSTALL.md#configuration-scripts-examples)
+
+
+In LINUX: check that in the /path_to_kratos/scripts/configure.sh the followinglines are written:
+
+``` cmake
+-DMPM_APPLICATION=ON
+-DLINEAR_SOLVERS_APPLICATION=ON
+```
+
+In WINDOWS: check that in the /path_to_kratos/scripts/configute.bat the following lines appears:
+
+```set KRATOS_APPLICATIONS=
+CALL :add_app %KRATOS_APP_DIR%\LinearSolversApplication;
+CALL :add_app %KRATOS_APP_DIR%\MPMApplication;
+```
+
+so the MPM application is compiled along with auxiliary linear solvers required.
+
+## Examples
+Some use-cases and validation examples are available in the MPM section of the [Examples](https://kratosmultiphysics.github.io/Examples/) repository. Also, some unit tests of the main features can be found in the [tests](https://github.com/KratosMultiphysics/Kratos/tree/master/applications/MPMApplication/tests) folder.
+
+### GiD Interface
+A GiD user interface for the MPM application is also available. It is located in GiD interface repository in [GiD interface repository](https://github.com/KratosMultiphysics/GiDInterface/tree/master/).
+
+It requires [GiD](https://www.gidhome.com/) - Pre and Post Processing software.
+
+## Theory
+
+Particle or meshfree methods are a category of methods where the state of a system is represented by a set of particles, without a fixed connectivity; hence, making such methods suitable for the analysis of moving discontinuities and large deformations with breaking and fragmentation. This approach does not suffer from the mesh distortion and entanglement issues posed by other Lagrangian discretizations such as the finite element method.
+
+### Material Point Method
+
+The MPM is an hybrid thechnique which uses a fixed background grid (or mesh) for solving the governing equations in a FEM fashion and  set of material particles (MP) for storing all the hystorical variables and material informations. MPM has gained a remarkably increasing popularity due to its capability in simulating  problems involving historically dependent materials and large deformations. As MPM is able to combine the strengths of Eulerian and Lagrangian methods, it has been utilized in various engineering applications and industrial purposes, in particular in geomechanics and environmental fluid dynamics field.
+
+Recommended references for implementation details of MPM in Kratos:
+- Singer, V.; Sautter, K.B., Larese, A., Wüchner, R.; Bletzinger, K.U.; A partitioned material point method and discrete element method coupling scheme, Advanced Modeling and Simulation in Engineering Sciences, 9(16), (2022); DOI: https://doi.org/10.1186/s40323-022-00229-5
+- Chandra, B., Singer, V., Teschemacher, T., Wuechner, R., & Larese, A. (2021). Nonconforming Dirichlet boundary conditions in implicit material point method by means of penalty augmentation. Acta Geotechnica, 16(8), 2315-2335. DOI: 10.1007/s11440-020-01123-3
+- Wilson, P., Wüchner, R., & Fernando, D. (2021). Distillation of the material point method cell crossing error leading to a novel quadrature‐based C 0 remedy. International Journal for Numerical Methods in Engineering, 122(6), 1513-1537.
+- Iaconeta, I., Larese, A., Rossi, R., & Oñate, E. (2018). A stabilized mixed implicit Material Point Method for non-linear incompressible solid mechanics. *Computational Mechanics*, 1-18. DOI 10.1007/s00466-018-1647-9
+- Iaconeta, I., Larese, A., Rossi, R., & Zhiming, G. (2016). Comparison of a material point method and a Galerkin meshfree method for the simulation of cohesive-frictional materials. *Materials*, 10(10), p. 1150. doi: 10.3390/ma10101150
+-
+## Features
+
+The following features are currently available and subject to development within the MPM Application:
+- Formulation:
+  * Irreducible formulations (U displacement based)
+  * Mixed UP formulations
+
+- Element types:
+    * Updated Lagrangian elements - triangular and quadrilatera (2D) and tetrahedral and hexahedral (3D), structured and unstructured, using classical or partitioned quadrature rules (this latter limited to explicit MPM)
+    * Updated Lagrangian axis-symmetric elements - triangular and quadrilateral (2D), structured and unstructured
+    * Updated Lagrangian mixed UP elements - triangular (2D) and tetrahedral (3D), structured and unstructured, stabilized using  Variational Multiscale Stabilization or Pressure Projection techniques
+
+- Constitutive laws:
+    * Linear isotropic elastic materials - plane strain, plane stress, axis-symmetric, and 3D
+    * Hyperelastic Neo-Hookean laws - finite strain, plane strain, axis-symmetric, and 3D
+    * Elasto-plastic laws:
+        * Mohr Coulomb - finite strain, associative and non-associative, plane strain, axis-symmetric, and 3D
+        * Mohr Coulomb with Strain Softening - finite strain, associative and non-associative, plane strain, axis-symmetric, and 3D
+    * Critical state laws:
+        * Modified Cam-Clay - finite strain, plane strain, axis-symmetric, and 3D
+        * Johnson Cook Thermal Plastic (just for explicit MPM)
+
+- A set of Boundary conditions:
+    * Grid-Based Conditions (conforming): applied directly on the background nodes
+        * Neumann: Point load
+        * Neumann: Line load (a distributed load applied over a line)
+        * Neumann: Surface load (a distributed load applied over a face)
+        * Dirichlet: Slip and No slip condition on arbitrary boundary.
+    * Material Point-Based Conditions (non conforming): applied in moveable boundary particles
+        * Neumann: Moving point load
+        * Dirichlet: Imposition of displacements (homogeneous and inhomogeneous) using penalty method
+
+- Strategies and schemes:
+    * Implicit - Newmark/Bossak prediction and correction scheme for static, quasi-static, and dynamic problems
+    * Explicit
+
+- Other features:
+    * Partitioned coupling with Finite Element Method - weak and strong coupling of nonconforming discretization
+    * Partitioned coupling with the Discrete Element Method
+    * material point erase features - to delete material points outside the interest domain
+
+## License
+
+The MPM Application is OPEN SOURCE. The main code and program structure is available and aimed to grow with the need of any user willing to expand it. The BSD (Berkeley Software Distribution) licence allows to use and distribute the existing code without any restriction, but with the possibility to develop new parts of the code on an open or close basis depending on the developers.
+
+## Contact
+
+* **Antonia Larese** - *Group Leader* - [antonia.larese@unipd.it](mailto:antonia.larese@unipd.it)
+* **Veronika Singer** - *Developer* - [veronika.singer@tum.de](mailto:veronika.singer@tum.de)
+* **Laura Moreno** - *Developer* - [laura.morenomartinez@unipd.it](mailto:laura.morenomartinez@unipd.it)
```

## Comparing `KratosMPMApplication-9.5.dist-info/RECORD` & `KratosMPMApplication-9.5.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-KratosMPMApplication-9.5.dist-info/METADATA,sha256=GZkcwxKMsdcoHmQyzFCRlJ9h93FdK0lPM6aPx1Rp7ec,9084
-KratosMPMApplication-9.5.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
-KratosMPMApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosMPMApplication-9.5.dist-info/RECORD,,
-KratosMPMApplication.libs/libKratosMPMCore-b22ee70f.so,sha256=A4sutaAWXQUtZ681ef_P2zVZ1Zl-EWrMkw7MTAUV39Q,9310457
-KratosMultiphysics/MPMApplication/particle_mechanics_analysis.py,sha256=YoIkHOt-KDAL72Zcou-_OPYGDMSoD4fUACdeOwiW-p0,1461
-KratosMultiphysics/MPMApplication/mpm_vtk_output_process.py,sha256=fyMplXfx6wrqTBUu2kzHb_OuH-SsWmeFyxWN1KAADjc,5070
-KratosMultiphysics/MPMApplication/mpm_json_output_process.py,sha256=eLGXfK9Q0XVm-8eZuDL04kpI-VHRuAv1683Roy4AGVs,8063
-KratosMultiphysics/MPMApplication/particle_vtk_output_process.py,sha256=F72nUTyrSIfXIsxvm4l5PO-eRUK53GVWM9A8aee4xjk,818
-KratosMultiphysics/MPMApplication/assign_gravity_to_material_point_process.py,sha256=cIWjk_PzcJ6HdYrQPqgvCg-lXzUK9jnNXmZNtrSO30Q,2876
-KratosMultiphysics/MPMApplication/apply_mpm_slip_boundary_process.py,sha256=BmNq6SVMlVVtrJIIzvGS96kf66fjT5dkPxoGL_cyT-4,1907
-KratosMultiphysics/MPMApplication/apply_mpm_particle_dirichlet_condition_process.py,sha256=oVlyyqJGclMHaCMqbiATw2gYh4fxyslkX5FF7so8BZ4,9141
-KratosMultiphysics/MPMApplication/mpm_solver.py,sha256=X_DlR5uBJAytCplkvjXypc6UYfOhqcCvb2FeiZLSYkg,27296
-KratosMultiphysics/MPMApplication/apply_mpm_3d_rotating_dirichlet_condition_process.py,sha256=lUuPzYvk2qItKQcgBgcHVzmjbiJFfxeR4tTyhOKsOGs,6722
-KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_dirichlet_condition_process.py,sha256=3cDhjQMUEtP00HD348ovALjXKJXPPGHSQFQ9jBGJPFE,6582
-KratosMultiphysics/MPMApplication/mpm_implicit_dynamic_solver.py,sha256=MwBWg_1giWHHpGyLsobnZg3ohqAXEf_a6vCc3kWU1qI,2970
-KratosMultiphysics/MPMApplication/kratos_main_mpm.py,sha256=7a2qSMStc_vy6j7FDarS_jcSY8t87lgb-sRdvesHesI,480
-KratosMultiphysics/MPMApplication/particle_json_output_process.py,sha256=hmjDWwnIbq2PPCBNGpG7G_WnmCzcrFWTfD-irBMxbKI,728
-KratosMultiphysics/MPMApplication/mpm_explicit_solver.py,sha256=G-Wtf5NfR0FrqUyRgezH7olW1eJOLE52j7yb8r7lR2c,6302
-KratosMultiphysics/MPMApplication/apply_mpm_particle_neumann_condition_process.py,sha256=Zm15jOwrSx7gzKJP9mfjsW29C8h495BDPBnYrej95Jo,8604
-KratosMultiphysics/MPMApplication/python_solvers_wrapper_mpm.py,sha256=8t-kIbv9RKLQQ8iBaah4DArzqoICDhgWTvfh9kqG-XY,2578
-KratosMultiphysics/MPMApplication/assign_gravity_to_particle_process.py,sha256=jmEGMC1D0bNBYoRRKZ68KKk1_yGnp74hfN9g030og6s,813
-KratosMultiphysics/MPMApplication/mpm_analysis.py,sha256=M2fhElyJlAWiNR8wv1vn0T2PEvUrrjgC38fhlp4D_ps,6525
-KratosMultiphysics/MPMApplication/assign_initial_velocity_to_particle_process.py,sha256=k2pXlPKQQ11lAa3_b1HObg3Y2saLF0TtBilwt9IUZQ4,856
-KratosMultiphysics/MPMApplication/mpm_gid_output_process.py,sha256=yCkzcmgjuiF7fS4pa56ddTFqodNx09ZzbAZUvn3kYVQ,11253
-KratosMultiphysics/MPMApplication/mpm_quasi_static_solver.py,sha256=yTrkeR2ws4v4YVaT-3_UUCyyqXNwSdpcqxo7z7T_x3c,756
-KratosMultiphysics/MPMApplication/mpm_static_solver.py,sha256=HuNAy45X5xgmaV-11iE0is9B_GefpCkr-d9doA2B8CM,723
-KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_neumann_condition_process.py,sha256=EvCh-c7yaXRNk0w-dsu-c8fN__XQ3I703lS42GhR20U,5307
-KratosMultiphysics/MPMApplication/assign_initial_velocity_to_material_point_process.py,sha256=Y-DFOgjkwMPY_cbHxGFxqhMBcXP7041VLChhbybA4p4,3406
-KratosMultiphysics/MPMApplication/particle_from_json_check_result_process.py,sha256=AY6UMDkxgoyBxHHHmJS5qfTxSEWDxa72CHK8VdCzPA8,774
-KratosMultiphysics/MPMApplication/particle_gid_output_process.py,sha256=gxPcOXZtP4KmC-Pcvko59PxzkpraW9TaALU7j-DyZYI,965
-KratosMultiphysics/MPMApplication/mpm_from_json_check_result_process.py,sha256=QWavGkYeRlAiDhNalDA5r_SQHolC087Y7Hmy7nNjAkw,20995
-KratosMultiphysics/MPMApplication/__init__.py,sha256=U28oA3nw53NSsY-U8TIJEmb5dg4BjRGnfHABS3CFUK4,215
-KratosMultiphysics/MPMApplication/mpm_vtk_condition_output_process.py,sha256=LZSy9ZvOuMGRsSn194dMWQsb_jyXxb1jFsCZIUBhqs4,5301
-KratosMultiphysics/.libs/KratosMPMApplication.cpython-39-x86_64-linux-gnu.so,sha256=4Ny-XEQs49kBMGb3bkXf5IL1fOV-oHCYzze2WINpjZI,3737889
-KratosMultiphysics/.libs/libKratosMPMCore.so,sha256=G-AoFzJNrtWNTWc6xz9_5Z0RU_A6cyJnJJt6ERr3w8M,8737657
+KratosMultiphysics/.libs/KratosMPMApplication.pyd,sha256=DO6Aip6-iOBgaHVcTmBD3iv0T3W_zX_n6b6T5a9XqDM,1924096
+KratosMultiphysics/.libs/KratosMPMCore.dll,sha256=QJKdVKFXUx4cC1IN_Wc8H35B5Y_eKB0KsJFzPD-nPTI,2701824
+KratosMultiphysics/.libs/KratosMPMCore.lib,sha256=-x1Zyho8-kcmNmUcde77bPDS0sU5EM5dZLROxNT5g50,528356
+KratosMultiphysics/MPMApplication/__init__.py,sha256=TCsQq6EQly9F1wGKkGT33t1GLDFc4w9035piNAXA3Uc,221
+KratosMultiphysics/MPMApplication/apply_mpm_3d_rotating_dirichlet_condition_process.py,sha256=AJHo5v6aokc4xtptXizaKRmSYv_be8kPMy_rqvGHB_Q,6863
+KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_dirichlet_condition_process.py,sha256=OaaNquR2fr_jJx0EUkao8SaLiqBxls_u7e9LXvJPYUU,6700
+KratosMultiphysics/MPMApplication/apply_mpm_coupling_interface_neumann_condition_process.py,sha256=j4-DG2IjNjvSGSa9dbO0Otxr4BoKy3qsR5PCxdb5320,5408
+KratosMultiphysics/MPMApplication/apply_mpm_particle_dirichlet_condition_process.py,sha256=wv9lhorTZkBjE4WczM3E9K1kMWwXuwHFPArAqy_YfPI,9320
+KratosMultiphysics/MPMApplication/apply_mpm_particle_neumann_condition_process.py,sha256=apGglZe4r8RE8h8ks0Ezho7S3DXFe6YWJntRXcCSBU8,8773
+KratosMultiphysics/MPMApplication/apply_mpm_slip_boundary_process.py,sha256=UCnl-9ED1_RVaJkOn_VEHYsWVpIHhJcqZRw1PM-joEU,1947
+KratosMultiphysics/MPMApplication/assign_gravity_to_material_point_process.py,sha256=BDgMzXzkEqqyi2XeFfAC0BEkIBxbKxWFMKtlJDMVndw,2930
+KratosMultiphysics/MPMApplication/assign_gravity_to_particle_process.py,sha256=KFR1oXFymnXRqodmJpuOdiYq5AH3MjNWgwEthbvp2ac,826
+KratosMultiphysics/MPMApplication/assign_initial_velocity_to_material_point_process.py,sha256=wlrQ31ZgveKqecDfhW3HR3K-lob2DMa4h5IIMjHsCuQ,3471
+KratosMultiphysics/MPMApplication/assign_initial_velocity_to_particle_process.py,sha256=E3Ghp_6aryObITtqThYm8n7JUBU9DAy3DnOoRcZBqDo,869
+KratosMultiphysics/MPMApplication/kratos_main_mpm.py,sha256=B8Rh6ir16p1iviLINlJTJKwLKp_st_8nFCB8oLfINsU,497
+KratosMultiphysics/MPMApplication/mpm_analysis.py,sha256=M6hTiaiciUMzb4Qw1MV2YulQZs4GMmLngeWmKEcSkWE,6640
+KratosMultiphysics/MPMApplication/mpm_explicit_solver.py,sha256=DpSRzW8fdB-NWlR6GHUsZStTN74ZNb_FbrdIT0dCEMg,6430
+KratosMultiphysics/MPMApplication/mpm_from_json_check_result_process.py,sha256=5Ej5vgik4zLlFFp3HQ1OycO7_Mt_rYQBcG11uV0NbOk,21391
+KratosMultiphysics/MPMApplication/mpm_gid_output_process.py,sha256=AZRu0SlALznmOJBCc--CncU_9YauDlazMO7qlyd9b7E,11513
+KratosMultiphysics/MPMApplication/mpm_implicit_dynamic_solver.py,sha256=8P1XGn1pb_BKcacLTqE_0QbE6w8vsC9G_UdQ89i6drw,3040
+KratosMultiphysics/MPMApplication/mpm_json_output_process.py,sha256=blggxxXkD5HBx7ExxW_qhzfVM5_mBvFm8nf3t1Tr13E,8221
+KratosMultiphysics/MPMApplication/mpm_quasi_static_solver.py,sha256=nm8k56OgA5VdNtLOuosBlqlDoF95mNle1vZxMlf8z8k,778
+KratosMultiphysics/MPMApplication/mpm_solver.py,sha256=Oyv3tUGzAtPIMY4-tjusJAtgINVgSlDyl2IHtOWKvAY,27814
+KratosMultiphysics/MPMApplication/mpm_static_solver.py,sha256=xXNehA7K0vGLSRyVVb5Qc5iOp4X3ZL-e_TaGZE5IxSk,741
+KratosMultiphysics/MPMApplication/mpm_vtk_condition_output_process.py,sha256=FOgq2J4m8fFTkixcE9GAKs__fP3SGP6vNHgTId1bDgI,5415
+KratosMultiphysics/MPMApplication/mpm_vtk_output_process.py,sha256=QvNMA3Xz3EDLYdxYsXlDDHQWGn7XtJq_XFttaodDEcA,5161
+KratosMultiphysics/MPMApplication/particle_from_json_check_result_process.py,sha256=4QEJalB1g3RLF_djCJZVnHE3ZuX8rHLMFveC7md0jJ8,786
+KratosMultiphysics/MPMApplication/particle_gid_output_process.py,sha256=DuTowiqWmb2r471zDC_8FrCWY9URzJ83BWXzQE6WQpQ,980
+KratosMultiphysics/MPMApplication/particle_json_output_process.py,sha256=CWgpzwR64wIzwIzWDJHlvJ4bCKuq-A3JKFuIF3xP2JA,740
+KratosMultiphysics/MPMApplication/particle_mechanics_analysis.py,sha256=vKYMREZL1tYD1mI5xlCFaTQ84Ht9xATGL2V4jAd8QLQ,1494
+KratosMultiphysics/MPMApplication/particle_vtk_output_process.py,sha256=cx5E5iEqTczPOHmmLffl9A8HTiSkA3aML5ymBDPCpGU,829
+KratosMultiphysics/MPMApplication/python_solvers_wrapper_mpm.py,sha256=5y2s0ONssQxJbvqvbGFVVvLf03GQurUHJKtt8nCkVrs,2633
+KratosMPMApplication-9.5.1.dist-info/METADATA,sha256=9mNaVK07xqeYTJTPQb38smXtLzXS_3rRHbiIEhLPenQ,9278
+KratosMPMApplication-9.5.1.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
+KratosMPMApplication-9.5.1.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosMPMApplication-9.5.1.dist-info/RECORD,,
```

