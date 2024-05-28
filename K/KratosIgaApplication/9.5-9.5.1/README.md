# Comparing `tmp/KratosIgaApplication-9.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/KratosIgaApplication-9.5.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,862 +1,539 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   2683404 (000000000028F20Ch)
-  Actual end-cent-dir record offset:       2683382 (000000000028F1F6h)
-  Expected end-cent-dir record offset:     2683382 (000000000028F1F6h)
+  Zip archive file size:                    983506 (00000000000F01D2h)
+  Actual end-cent-dir record offset:        983484 (00000000000F01BCh)
+  Expected end-cent-dir record offset:      983484 (00000000000F01BCh)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 23 entries.
-  The central directory is 2859 (0000000000000B2Bh) bytes long,
+  central directory contains 18 entries.
+  The central directory is 1903 (000000000000076Fh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 2680523 (000000000028E6CBh).
+  is 981581 (00000000000EFA4Dh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  KratosIgaApplication-9.5.dist-info/
+  KratosMultiphysics/.libs/KratosIgaApplication.pyd
 
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
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:54
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             35 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:36
+  32-bit CRC value (hex):                         4c7b4ffc
+  compressed size:                                258152 bytes
+  uncompressed size:                              793088 bytes
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
 
-  KratosIgaApplication-9.5.dist-info/METADATA
+  KratosMultiphysics/.libs/KratosIgaCore.dll
 
-  offset of local header from start of archive:   93
-                                                  (000000000000005Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   258231
+                                                  (000000000003F0B7h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         2ef5e028
-  compressed size:                                543 bytes
-  uncompressed size:                              1343 bytes
-  length of filename:                             43 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:36
+  32-bit CRC value (hex):                         bf2aa111
+  compressed size:                                696272 bytes
+  uncompressed size:                              1940480 bytes
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
 
-  KratosIgaApplication-9.5.dist-info/WHEEL
+  KratosMultiphysics/.libs/KratosIgaCore.lib
 
-  offset of local header from start of archive:   737
-                                                  (00000000000002E1h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   954575
+                                                  (00000000000E90CFh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         90d34e0d
-  compressed size:                                116 bytes
-  uncompressed size:                              148 bytes
-  length of filename:                             40 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:36
+  32-bit CRC value (hex):                         2f00fe4f
+  compressed size:                                16293 bytes
+  uncompressed size:                              154612 bytes
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
 
-  KratosIgaApplication-9.5.dist-info/top_level.txt
+  KratosMultiphysics/IgaApplication/__init__.py
 
-  offset of local header from start of archive:   951
-                                                  (00000000000003B7h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   970940
+                                                  (00000000000ED0BCh) bytes
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
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         f32d789f
-  compressed size:                                19 bytes
-  uncompressed size:                              19 bytes
-  length of filename:                             48 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         2bd50766
+  compressed size:                                209 bytes
+  uncompressed size:                              464 bytes
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
 
-  KratosIgaApplication-9.5.dist-info/RECORD
+  KratosMultiphysics/IgaApplication/assign_integration_points_to_background_elements_process.py
 
-  offset of local header from start of archive:   1076
-                                                  (0000000000000434h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   971224
+                                                  (00000000000ED1D8h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:54
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 UTC
-  32-bit CRC value (hex):                         8a778608
-  compressed size:                                1090 bytes
-  uncompressed size:                              2202 bytes
-  length of filename:                             41 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         2215f4c7
+  compressed size:                                246 bytes
+  uncompressed size:                              405 bytes
+  length of filename:                             93 characters
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
 
-  KratosIgaApplication.libs/
+  KratosMultiphysics/IgaApplication/assign_vector_variable_and_constraints_to_conditions_process.py
 
-  offset of local header from start of archive:   2265
-                                                  (00000000000008D9h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   971593
+                                                  (00000000000ED349h) bytes
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
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:54
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             26 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         3479d858
+  compressed size:                                1222 bytes
+  uncompressed size:                              4486 bytes
+  length of filename:                             97 characters
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
 
-  KratosIgaApplication.libs/libKratosIgaCore-9fdd436e.so
+  KratosMultiphysics/IgaApplication/iga_output_process.py
 
-  offset of local header from start of archive:   2349
-                                                  (000000000000092Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   972942
+                                                  (00000000000ED88Eh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         4448eb66
-  compressed size:                                1909586 bytes
-  uncompressed size:                              6546497 bytes
-  length of filename:                             54 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         8af0d583
+  compressed size:                                1788 bytes
+  uncompressed size:                              7646 bytes
+  length of filename:                             55 characters
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
+  KratosMultiphysics/IgaApplication/kratos_main_iga.py
 
-  offset of local header from start of archive:   1912047
-                                                  (00000000001D2CEFh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   974815
+                                                  (00000000000EDFDFh) bytes
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
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             19 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         c86c6cb4
+  compressed size:                                324 bytes
+  uncompressed size:                              725 bytes
+  length of filename:                             52 characters
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
 
-  KratosMultiphysics/IgaApplication/
+  KratosMultiphysics/IgaApplication/map_nurbs_volume_results_to_embedded_geometry_process.py
 
-  offset of local header from start of archive:   1912124
-                                                  (00000000001D2D3Ch) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   975221
+                                                  (00000000000EE175h) bytes
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
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         00000000
-  compressed size:                                0 bytes
-  uncompressed size:                              0 bytes
-  length of filename:                             34 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         6c5eba5f
+  compressed size:                                366 bytes
+  uncompressed size:                              821 bytes
+  length of filename:                             90 characters
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
 
-  KratosMultiphysics/IgaApplication/output_eigen_values_process.py
+  KratosMultiphysics/IgaApplication/nitsche_stabilization_process.py
 
-  offset of local header from start of archive:   1912216
-                                                  (00000000001D2D98h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   975707
+                                                  (00000000000EE35Bh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         de98ed96
-  compressed size:                                226 bytes
-  uncompressed size:                              373 bytes
-  length of filename:                             64 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         18dd98a6
+  compressed size:                                1380 bytes
+  uncompressed size:                              4394 bytes
+  length of filename:                             66 characters
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
 
-  KratosMultiphysics/IgaApplication/output_quadrature_domain_process.py
+  KratosMultiphysics/IgaApplication/output_eigen_values_process.py
 
-  offset of local header from start of archive:   1912564
-                                                  (00000000001D2EF4h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   977183
+                                                  (00000000000EE91Fh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         42096c9e
-  compressed size:                                323 bytes
-  uncompressed size:                              710 bytes
-  length of filename:                             69 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         0848b754
+  compressed size:                                232 bytes
+  uncompressed size:                              381 bytes
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
 
 Central directory entry #12:
 ---------------------------
 
-  KratosMultiphysics/IgaApplication/assign_integration_points_to_background_elements_process.py
+  KratosMultiphysics/IgaApplication/output_quadrature_domain_process.py
 
-  offset of local header from start of archive:   1913014
-                                                  (00000000001D30B6h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   977509
+                                                  (00000000000EEA65h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         c9382a43
-  compressed size:                                240 bytes
-  uncompressed size:                              397 bytes
-  length of filename:                             93 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         42096c9e
+  compressed size:                                323 bytes
+  uncompressed size:                              710 bytes
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
 
 Central directory entry #13:
 ---------------------------
 
-  KratosMultiphysics/IgaApplication/nitsche_stabilization_process.py
+  KratosMultiphysics/IgaApplication/set_directors_process.py
 
-  offset of local header from start of archive:   1913405
-                                                  (00000000001D323Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   977931
+                                                  (00000000000EEC0Bh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         4da7577e
-  compressed size:                                1371 bytes
-  uncompressed size:                              4308 bytes
-  length of filename:                             66 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         54526224
+  compressed size:                                623 bytes
+  uncompressed size:                              1554 bytes
+  length of filename:                             58 characters
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
 
-  KratosMultiphysics/IgaApplication/kratos_main_iga.py
+  KratosMultiphysics/IgaApplication/vtk_embedded_geometry_output_process.py
 
-  offset of local header from start of archive:   1914900
-                                                  (00000000001D3814h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   978642
+                                                  (00000000000EEED2h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         a3047a39
-  compressed size:                                314 bytes
-  uncompressed size:                              706 bytes
-  length of filename:                             52 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 12:13:56
+  32-bit CRC value (hex):                         449006db
+  compressed size:                                851 bytes
+  uncompressed size:                              2940 bytes
+  length of filename:                             73 characters
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
 
-  KratosMultiphysics/IgaApplication/map_nurbs_volume_results_to_embedded_geometry_process.py
+  KratosIgaApplication-9.5.1.dist-info/METADATA
 
-  offset of local header from start of archive:   1915324
-                                                  (00000000001D39BCh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   979596
+                                                  (00000000000EF28Ch) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         b73e38be
-  compressed size:                                358 bytes
-  uncompressed size:                              803 bytes
-  length of filename:                             90 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:36
+  32-bit CRC value (hex):                         73542e4a
+  compressed size:                                556 bytes
+  uncompressed size:                              1427 bytes
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
 
 Central directory entry #16:
 ---------------------------
 
-  KratosMultiphysics/IgaApplication/assign_vector_variable_and_constraints_to_conditions_process.py
+  KratosIgaApplication-9.5.1.dist-info/WHEEL
 
-  offset of local header from start of archive:   1915830
-                                                  (00000000001D3BB6h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   980227
+                                                  (00000000000EF503h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         9f662160
-  compressed size:                                1212 bytes
-  uncompressed size:                              4393 bytes
-  length of filename:                             97 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:36
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
 
 Central directory entry #17:
 ---------------------------
 
-  KratosMultiphysics/IgaApplication/iga_output_process.py
+  KratosIgaApplication-9.5.1.dist-info/top_level.txt
 
-  offset of local header from start of archive:   1917197
-                                                  (00000000001D410Dh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   980395
+                                                  (00000000000EF5ABh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         bde9f638
-  compressed size:                                1781 bytes
-  uncompressed size:                              7492 bytes
-  length of filename:                             55 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:36
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
 
 Central directory entry #18:
 ---------------------------
 
-  KratosMultiphysics/IgaApplication/__init__.pyi
-
-  offset of local header from start of archive:   1919091
-                                                  (00000000001D4873h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         4a74b24a
-  compressed size:                                484 bytes
-  uncompressed size:                              1789 bytes
-  length of filename:                             46 characters
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
-Central directory entry #19:
----------------------------
-
-  KratosMultiphysics/IgaApplication/vtk_embedded_geometry_output_process.py
-
-  offset of local header from start of archive:   1919679
-                                                  (00000000001D4ABFh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         d1e4b212
-  compressed size:                                840 bytes
-  uncompressed size:                              2884 bytes
-  length of filename:                             73 characters
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
-Central directory entry #20:
----------------------------
-
-  KratosMultiphysics/IgaApplication/set_directors_process.py
+  KratosIgaApplication-9.5.1.dist-info/RECORD
 
-  offset of local header from start of archive:   1920650
-                                                  (00000000001D4E8Ah) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
+  offset of local header from start of archive:   980496
+                                                  (00000000000EF610h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   2.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         42c1a03c
-  compressed size:                                613 bytes
-  uncompressed size:                              1511 bytes
-  length of filename:                             58 characters
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
-Central directory entry #21:
----------------------------
-
-  KratosMultiphysics/IgaApplication/__init__.py
-
-  offset of local header from start of archive:   1921379
-                                                  (00000000001D5163h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         6b3759a8
-  compressed size:                                206 bytes
-  uncompressed size:                              447 bytes
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
-Central directory entry #22:
----------------------------
-
-  KratosMultiphysics/.libs/
-
-  offset of local header from start of archive:   1921688
-                                                  (00000000001D5298h) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   1.0
-  compression method:                             none (stored)
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:54
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:54 UTC
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
-Central directory entry #23:
----------------------------
-
-  KratosMultiphysics/.libs/KratosIgaApplication.cpython-39-x86_64-linux-gnu.so
-
-  offset of local header from start of archive:   1921771
-                                                  (00000000001D52EBh) bytes
-  file system or operating system of origin:      Unix
-  version of encoding software:                   3.0
-  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
-  file security status:                           not encrypted
-  extended local header:                          no
-  file last modified on (DOS date/time):          2024 Apr 25 15:59:48
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 local
-  file last modified on (UT extra field modtime): 2024 Apr 25 15:59:48 UTC
-  32-bit CRC value (hex):                         8d5e8b20
-  compressed size:                                758618 bytes
-  uncompressed size:                              2164081 bytes
-  length of filename:                             76 characters
-  length of extra field:                          24 bytes
+  file last modified on (DOS date/time):          2024 May 27 13:36:36
+  32-bit CRC value (hex):                         fcb00e03
+  compressed size:                                1012 bytes
+  uncompressed size:                              2045 bytes
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
@@ -1,70 +1,55 @@
-Filename: KratosIgaApplication-9.5.dist-info/
+Filename: KratosMultiphysics/.libs/KratosIgaApplication.pyd
 Comment: 
 
-Filename: KratosIgaApplication-9.5.dist-info/METADATA
+Filename: KratosMultiphysics/.libs/KratosIgaCore.dll
 Comment: 
 
-Filename: KratosIgaApplication-9.5.dist-info/WHEEL
+Filename: KratosMultiphysics/.libs/KratosIgaCore.lib
 Comment: 
 
-Filename: KratosIgaApplication-9.5.dist-info/top_level.txt
-Comment: 
-
-Filename: KratosIgaApplication-9.5.dist-info/RECORD
-Comment: 
-
-Filename: KratosIgaApplication.libs/
-Comment: 
-
-Filename: KratosIgaApplication.libs/libKratosIgaCore-9fdd436e.so
+Filename: KratosMultiphysics/IgaApplication/__init__.py
 Comment: 
 
-Filename: KratosMultiphysics/
+Filename: KratosMultiphysics/IgaApplication/assign_integration_points_to_background_elements_process.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/
+Filename: KratosMultiphysics/IgaApplication/assign_vector_variable_and_constraints_to_conditions_process.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/output_eigen_values_process.py
+Filename: KratosMultiphysics/IgaApplication/iga_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/output_quadrature_domain_process.py
+Filename: KratosMultiphysics/IgaApplication/kratos_main_iga.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/assign_integration_points_to_background_elements_process.py
+Filename: KratosMultiphysics/IgaApplication/map_nurbs_volume_results_to_embedded_geometry_process.py
 Comment: 
 
 Filename: KratosMultiphysics/IgaApplication/nitsche_stabilization_process.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/kratos_main_iga.py
-Comment: 
-
-Filename: KratosMultiphysics/IgaApplication/map_nurbs_volume_results_to_embedded_geometry_process.py
-Comment: 
-
-Filename: KratosMultiphysics/IgaApplication/assign_vector_variable_and_constraints_to_conditions_process.py
+Filename: KratosMultiphysics/IgaApplication/output_eigen_values_process.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/iga_output_process.py
+Filename: KratosMultiphysics/IgaApplication/output_quadrature_domain_process.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/__init__.pyi
+Filename: KratosMultiphysics/IgaApplication/set_directors_process.py
 Comment: 
 
 Filename: KratosMultiphysics/IgaApplication/vtk_embedded_geometry_output_process.py
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/set_directors_process.py
+Filename: KratosIgaApplication-9.5.1.dist-info/METADATA
 Comment: 
 
-Filename: KratosMultiphysics/IgaApplication/__init__.py
+Filename: KratosIgaApplication-9.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: KratosMultiphysics/.libs/
+Filename: KratosIgaApplication-9.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: KratosMultiphysics/.libs/KratosIgaApplication.cpython-39-x86_64-linux-gnu.so
+Filename: KratosIgaApplication-9.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v1.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## KratosMultiphysics/IgaApplication/output_eigen_values_process.py

 * *Ordering differences only*

```diff
@@ -1,8 +1,8 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.IgaApplication as IGA
-
-def Factory(settings, model):
-    if not (isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    return IGA.OutputEigenValuesProcess(model, settings["Parameters"])
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.IgaApplication as IGA
+
+def Factory(settings, model):
+    if not (isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    return IGA.OutputEigenValuesProcess(model, settings["Parameters"])
```

## KratosMultiphysics/IgaApplication/assign_integration_points_to_background_elements_process.py

 * *Ordering differences only*

```diff
@@ -1,9 +1,9 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.IgaApplication as IGA
-
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.IgaApplication as IGA
+
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
     return IGA.AssignIntegrationPointsToBackgroundElementsProcess(model, settings["Parameters"])
```

## KratosMultiphysics/IgaApplication/nitsche_stabilization_process.py

 * *Ordering differences only*

```diff
@@ -1,87 +1,87 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-from KratosMultiphysics import eigen_solver_factory
-
-import KratosMultiphysics.IgaApplication as IGA
-
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    return NitscheStabilizationProcess(model, settings["Parameters"])
-
-class NitscheStabilizationProcess(KratosMultiphysics.Process):
-    """This class is used in order to compute automatically the Nitsche stabilization factor.
-
-    Only the member variables listed below should be accessed directly.
-
-    Public member variables:
-    model -- the container of the different model parts.
-    params -- Kratos parameters containing the settings.
-    """
-    def __init__(self, model, params):
-        """ The default constructor of the class
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        model -- the container of the different model parts.
-        params -- Kratos parameters containing solver settings.
-        """
-        KratosMultiphysics.Process.__init__(self)
-
-        ## Settings string in json format
-        default_parameters = KratosMultiphysics.Parameters("""{
-            "model_part_condition_name" : "",
-            "eigen_system_settings" : {
-                    "solver_type"           : "feast",
-                    "echo_level"            : 0,
-                    "tolerance"             : 1e-10,
-                    "symmetric"             : true,
-                    "e_min"                 : 0.0,
-                    "e_max"                 : 1.0e20,
-                    "number_of_eigenvalues" : 1,
-                    "subspace_size"         : 1
-            },
-            "number_of_conditions" : 1
-        }""")
-
-        ## Overwrite the default settings with user-provided parameters
-        self.params = params
-        self.params.RecursivelyValidateAndAssignDefaults(default_parameters)
-
-        self.model = model
-        self.model_part_condition = self.model[self.params["model_part_condition_name"].GetString()]
-
-        # Call the Nitsche stabilization model Part process
-        KratosMultiphysics.Process.__init__(self)
-        self.process = IGA.NitscheStabilizationModelPartProcess(self.model_part_condition)
-        self.process.ExecuteInitialize()
-
-        self.model_part = self.model.GetModelPart("IgaModelPart").GetSubModelPart("Nitsche_Stabilization_" + self.params["model_part_condition_name"].GetString()[13:])
-
-        # Define the eigenvalue size for FEAST solver
-        eigenvalue_nitsche_stabilization_size = self.model_part.ProcessInfo.GetValue(IGA.EIGENVALUE_NITSCHE_STABILIZATION_SIZE)
-        self.params["eigen_system_settings"]["subspace_size"].SetInt(eigenvalue_nitsche_stabilization_size)
-        self.params["eigen_system_settings"]["number_of_eigenvalues"].SetInt(eigenvalue_nitsche_stabilization_size)
-
-    def ExecuteInitializeSolutionStep(self):
-        # Get the model parts which divide the problem
-        current_process_info = self.model_part.ProcessInfo
-
-        # Compute the eigen values
-        eigen_linear_solver = eigen_solver_factory.ConstructSolver(self.params["eigen_system_settings"])
-        builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(eigen_linear_solver)
-        eigen_scheme = IGA.EigensolverNitscheStabilizationScheme()
-        eigen_solver = IGA.EigensolverNitscheStabilizationStrategy(self.model_part, eigen_scheme, builder_and_solver)
-        eigen_solver.Solve()
-
-        # Compute the Nitsche stabilization factor
-        eigenvalue_nitsche_stabilization_vector = current_process_info.GetValue(IGA.EIGENVALUE_NITSCHE_STABILIZATION_VECTOR)
-        nitsche_stabilization_factor= eigenvalue_nitsche_stabilization_vector[eigenvalue_nitsche_stabilization_vector.Size()-1]*4*self.params["number_of_conditions"].GetInt()
-
-        # Set the Nitsche stabilization factor
-        for prop in self.model_part_condition.Properties:
-            prop.SetValue(IGA.NITSCHE_STABILIZATION_FACTOR, nitsche_stabilization_factor)
-
-        # Reset BUILD_LEVEL to calculate the continuity enforcement matrix in coupling Nitsche condition
+# Importing the Kratos Library
+import KratosMultiphysics
+from KratosMultiphysics import eigen_solver_factory
+
+import KratosMultiphysics.IgaApplication as IGA
+
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    return NitscheStabilizationProcess(model, settings["Parameters"])
+
+class NitscheStabilizationProcess(KratosMultiphysics.Process):
+    """This class is used in order to compute automatically the Nitsche stabilization factor.
+
+    Only the member variables listed below should be accessed directly.
+
+    Public member variables:
+    model -- the container of the different model parts.
+    params -- Kratos parameters containing the settings.
+    """
+    def __init__(self, model, params):
+        """ The default constructor of the class
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        model -- the container of the different model parts.
+        params -- Kratos parameters containing solver settings.
+        """
+        KratosMultiphysics.Process.__init__(self)
+
+        ## Settings string in json format
+        default_parameters = KratosMultiphysics.Parameters("""{
+            "model_part_condition_name" : "",
+            "eigen_system_settings" : {
+                    "solver_type"           : "feast",
+                    "echo_level"            : 0,
+                    "tolerance"             : 1e-10,
+                    "symmetric"             : true,
+                    "e_min"                 : 0.0,
+                    "e_max"                 : 1.0e20,
+                    "number_of_eigenvalues" : 1,
+                    "subspace_size"         : 1
+            },
+            "number_of_conditions" : 1
+        }""")
+
+        ## Overwrite the default settings with user-provided parameters
+        self.params = params
+        self.params.RecursivelyValidateAndAssignDefaults(default_parameters)
+
+        self.model = model
+        self.model_part_condition = self.model[self.params["model_part_condition_name"].GetString()]
+
+        # Call the Nitsche stabilization model Part process
+        KratosMultiphysics.Process.__init__(self)
+        self.process = IGA.NitscheStabilizationModelPartProcess(self.model_part_condition)
+        self.process.ExecuteInitialize()
+
+        self.model_part = self.model.GetModelPart("IgaModelPart").GetSubModelPart("Nitsche_Stabilization_" + self.params["model_part_condition_name"].GetString()[13:])
+
+        # Define the eigenvalue size for FEAST solver
+        eigenvalue_nitsche_stabilization_size = self.model_part.ProcessInfo.GetValue(IGA.EIGENVALUE_NITSCHE_STABILIZATION_SIZE)
+        self.params["eigen_system_settings"]["subspace_size"].SetInt(eigenvalue_nitsche_stabilization_size)
+        self.params["eigen_system_settings"]["number_of_eigenvalues"].SetInt(eigenvalue_nitsche_stabilization_size)
+
+    def ExecuteInitializeSolutionStep(self):
+        # Get the model parts which divide the problem
+        current_process_info = self.model_part.ProcessInfo
+
+        # Compute the eigen values
+        eigen_linear_solver = eigen_solver_factory.ConstructSolver(self.params["eigen_system_settings"])
+        builder_and_solver = KratosMultiphysics.ResidualBasedBlockBuilderAndSolver(eigen_linear_solver)
+        eigen_scheme = IGA.EigensolverNitscheStabilizationScheme()
+        eigen_solver = IGA.EigensolverNitscheStabilizationStrategy(self.model_part, eigen_scheme, builder_and_solver)
+        eigen_solver.Solve()
+
+        # Compute the Nitsche stabilization factor
+        eigenvalue_nitsche_stabilization_vector = current_process_info.GetValue(IGA.EIGENVALUE_NITSCHE_STABILIZATION_VECTOR)
+        nitsche_stabilization_factor= eigenvalue_nitsche_stabilization_vector[eigenvalue_nitsche_stabilization_vector.Size()-1]*4*self.params["number_of_conditions"].GetInt()
+
+        # Set the Nitsche stabilization factor
+        for prop in self.model_part_condition.Properties:
+            prop.SetValue(IGA.NITSCHE_STABILIZATION_FACTOR, nitsche_stabilization_factor)
+
+        # Reset BUILD_LEVEL to calculate the continuity enforcement matrix in coupling Nitsche condition
         self.model_part_condition.ProcessInfo.SetValue(IGA.BUILD_LEVEL,0)
```

## KratosMultiphysics/IgaApplication/kratos_main_iga.py

 * *Ordering differences only*

```diff
@@ -1,19 +1,19 @@
-import KratosMultiphysics
-import KratosMultiphysics.IgaApplication
-from KratosMultiphysics.StructuralMechanicsApplication.structural_mechanics_analysis import StructuralMechanicsAnalysis
-
-"""
-The IgaApplication relies on the analyses and solvers of
-the StructuralMechanicsApplication. If user-scripting is
-required it is recommended to derive that class from the
-StructuralMechanicsAnalysis to do modifications.
-"""
-
-if __name__ == "__main__":
-
-    with open("ProjectParameters.json",'r') as parameter_file:
-        parameters = KratosMultiphysics.Parameters(parameter_file.read())
-
-    model = KratosMultiphysics.Model()
-    simulation = StructuralMechanicsAnalysis(model,parameters)
-    simulation.Run()
+import KratosMultiphysics
+import KratosMultiphysics.IgaApplication
+from KratosMultiphysics.StructuralMechanicsApplication.structural_mechanics_analysis import StructuralMechanicsAnalysis
+
+"""
+The IgaApplication relies on the analyses and solvers of
+the StructuralMechanicsApplication. If user-scripting is
+required it is recommended to derive that class from the
+StructuralMechanicsAnalysis to do modifications.
+"""
+
+if __name__ == "__main__":
+
+    with open("ProjectParameters.json",'r') as parameter_file:
+        parameters = KratosMultiphysics.Parameters(parameter_file.read())
+
+    model = KratosMultiphysics.Model()
+    simulation = StructuralMechanicsAnalysis(model,parameters)
+    simulation.Run()
```

## KratosMultiphysics/IgaApplication/map_nurbs_volume_results_to_embedded_geometry_process.py

 * *Ordering differences only*

```diff
@@ -1,18 +1,18 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.IgaApplication as IGA
-from KratosMultiphysics import kratos_utilities
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    return MapNurbsVolumeResultsToEmbeddedGeometryProcess(model, settings["Parameters"])
-
-class MapNurbsVolumeResultsToEmbeddedGeometryProcess(KratosMultiphysics.Process):
-    def __init__(self, model, params):
-        KratosMultiphysics.Process.__init__(self)
-        self.params = params
-        self.process = IGA.MapNurbsVolumeResultsToEmbeddedGeometryProcess(model, params)
-
-    def ExecuteBeforeOutputStep(self):
-        self.process.MapVariables()
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.IgaApplication as IGA
+from KratosMultiphysics import kratos_utilities
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    return MapNurbsVolumeResultsToEmbeddedGeometryProcess(model, settings["Parameters"])
+
+class MapNurbsVolumeResultsToEmbeddedGeometryProcess(KratosMultiphysics.Process):
+    def __init__(self, model, params):
+        KratosMultiphysics.Process.__init__(self)
+        self.params = params
+        self.process = IGA.MapNurbsVolumeResultsToEmbeddedGeometryProcess(model, params)
+
+    def ExecuteBeforeOutputStep(self):
+        self.process.MapVariables()
```

## KratosMultiphysics/IgaApplication/assign_vector_variable_and_constraints_to_conditions_process.py

 * *Ordering differences only*

```diff
@@ -1,93 +1,93 @@
-import KratosMultiphysics
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return AssignVectorVariableAndConstraintsToConditionProcess(model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class AssignVectorVariableAndConstraintsToConditionProcess(KratosMultiphysics.Process):
-    def __init__(self, model, settings ):
-        KratosMultiphysics.Process.__init__(self)
-
-        default_settings = KratosMultiphysics.Parameters("""{
-            "mesh_id"              : 0,
-            "model_part_name"      : "please_specify_model_part_name",
-            "variable_name"        : "SPECIFY_VARIABLE_NAME",
-            "interval"             : [0.0, 1e30],
-            "value"                : [10.0, "3*t", "x+y"],
-            "local_axes"           : {}
-        }""")
-
-        # detect "End" as a tag and replace it by a large number
-        if(settings.Has("interval")):
-            if(settings["interval"][1].IsString() ):
-                if(settings["interval"][1].GetString() == "End"):
-                    settings["interval"][1].SetDouble(1e30)
-                else:
-                    raise Exception("the second value of interval can be \"End\" or a number, interval currently:"+settings["interval"].PrettyPrintJsonString())
-
-        settings.ValidateAndAssignDefaults(default_settings)
-
-        variable_name = settings["variable_name"].GetString()
-        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
-        self.variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
-
-        if not variable_type == "Array" and not variable_type == "Vector":
-            err_msg  = 'Variable-type of variable: "' + variable_name + '" is incorrect ("'
-            err_msg += variable_type + '"). Must be a "Array" or "Vector"'
-            raise Exception(msg)
-
-        self.model_part = model[settings["model_part_name"].GetString()]
-
-        self.aux_processes = []
-
-        from KratosMultiphysics.assign_scalar_variable_to_conditions_process import AssignScalarVariableToConditionsProcess
-
-        # loop over components X, Y and Z
-        for index, variable_dir in enumerate(["_X", "_Y", "_Z"]):
-            variable_component_name = variable_name + variable_dir
-            flag_name = "KratosMultiphysics.IgaApplication.IgaFlags.FIX_" + variable_component_name
-            if not settings["value"][index].IsNull():
-                component_params = KratosMultiphysics.Parameters("{}")
-                component_params.AddValue("model_part_name", settings["model_part_name"])
-                component_params.AddValue("interval", settings["interval"])
-                component_params.AddValue("value",settings["value"][index])
-                component_params.AddEmptyValue("variable_name").SetString(variable_name + variable_dir)
-                component_params.AddValue("local_axes",settings["local_axes"])
-                self.aux_processes.append( AssignScalarVariableToConditionsProcess(model, component_params) )
-                KratosMultiphysics.VariableUtils().SetFlag(eval(flag_name), True, self.model_part.Conditions)
-            else:
-                KratosMultiphysics.VariableUtils().SetFlag(eval(flag_name), False, self.model_part.Conditions)
-
-    def ExecuteInitialize(self):
-        for process in self.aux_processes:
-            process.ExecuteInitialize()
-
-    def ExecuteBeforeSolutionLoop(self):
-        for process in self.aux_processes:
-            process.ExecuteBeforeSolutionLoop()
-
-    def ExecuteInitializeSolutionStep(self):
-        for process in self.aux_processes:
-            process.ExecuteInitializeSolutionStep()
-
-    def ExecuteBeforeOutputStep(self):
-        for process in self.aux_processes:
-            process.ExecuteBeforeOutputStep()
-
-    def ExecuteAfterOutputStep(self):
-        for process in self.aux_processes:
-            process.ExecuteAfterOutputStep()
-
-    def ExecuteFinalizeSolutionStep(self):
-        for process in self.aux_processes:
-            process.ExecuteFinalizeSolutionStep()
-
-    def ExecuteFinalize(self):
-        for process in self.aux_processes:
-            process.ExecuteFinalize()
-
-    def Check(self):
-        for process in self.aux_processes:
-            process.Check()
+import KratosMultiphysics
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return AssignVectorVariableAndConstraintsToConditionProcess(model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class AssignVectorVariableAndConstraintsToConditionProcess(KratosMultiphysics.Process):
+    def __init__(self, model, settings ):
+        KratosMultiphysics.Process.__init__(self)
+
+        default_settings = KratosMultiphysics.Parameters("""{
+            "mesh_id"              : 0,
+            "model_part_name"      : "please_specify_model_part_name",
+            "variable_name"        : "SPECIFY_VARIABLE_NAME",
+            "interval"             : [0.0, 1e30],
+            "value"                : [10.0, "3*t", "x+y"],
+            "local_axes"           : {}
+        }""")
+
+        # detect "End" as a tag and replace it by a large number
+        if(settings.Has("interval")):
+            if(settings["interval"][1].IsString() ):
+                if(settings["interval"][1].GetString() == "End"):
+                    settings["interval"][1].SetDouble(1e30)
+                else:
+                    raise Exception("the second value of interval can be \"End\" or a number, interval currently:"+settings["interval"].PrettyPrintJsonString())
+
+        settings.ValidateAndAssignDefaults(default_settings)
+
+        variable_name = settings["variable_name"].GetString()
+        variable_type = KratosMultiphysics.KratosGlobals.GetVariableType(variable_name)
+        self.variable = KratosMultiphysics.KratosGlobals.GetVariable(variable_name)
+
+        if not variable_type == "Array" and not variable_type == "Vector":
+            err_msg  = 'Variable-type of variable: "' + variable_name + '" is incorrect ("'
+            err_msg += variable_type + '"). Must be a "Array" or "Vector"'
+            raise Exception(msg)
+
+        self.model_part = model[settings["model_part_name"].GetString()]
+
+        self.aux_processes = []
+
+        from KratosMultiphysics.assign_scalar_variable_to_conditions_process import AssignScalarVariableToConditionsProcess
+
+        # loop over components X, Y and Z
+        for index, variable_dir in enumerate(["_X", "_Y", "_Z"]):
+            variable_component_name = variable_name + variable_dir
+            flag_name = "KratosMultiphysics.IgaApplication.IgaFlags.FIX_" + variable_component_name
+            if not settings["value"][index].IsNull():
+                component_params = KratosMultiphysics.Parameters("{}")
+                component_params.AddValue("model_part_name", settings["model_part_name"])
+                component_params.AddValue("interval", settings["interval"])
+                component_params.AddValue("value",settings["value"][index])
+                component_params.AddEmptyValue("variable_name").SetString(variable_name + variable_dir)
+                component_params.AddValue("local_axes",settings["local_axes"])
+                self.aux_processes.append( AssignScalarVariableToConditionsProcess(model, component_params) )
+                KratosMultiphysics.VariableUtils().SetFlag(eval(flag_name), True, self.model_part.Conditions)
+            else:
+                KratosMultiphysics.VariableUtils().SetFlag(eval(flag_name), False, self.model_part.Conditions)
+
+    def ExecuteInitialize(self):
+        for process in self.aux_processes:
+            process.ExecuteInitialize()
+
+    def ExecuteBeforeSolutionLoop(self):
+        for process in self.aux_processes:
+            process.ExecuteBeforeSolutionLoop()
+
+    def ExecuteInitializeSolutionStep(self):
+        for process in self.aux_processes:
+            process.ExecuteInitializeSolutionStep()
+
+    def ExecuteBeforeOutputStep(self):
+        for process in self.aux_processes:
+            process.ExecuteBeforeOutputStep()
+
+    def ExecuteAfterOutputStep(self):
+        for process in self.aux_processes:
+            process.ExecuteAfterOutputStep()
+
+    def ExecuteFinalizeSolutionStep(self):
+        for process in self.aux_processes:
+            process.ExecuteFinalizeSolutionStep()
+
+    def ExecuteFinalize(self):
+        for process in self.aux_processes:
+            process.ExecuteFinalize()
+
+    def Check(self):
+        for process in self.aux_processes:
+            process.Check()
```

## KratosMultiphysics/IgaApplication/iga_output_process.py

 * *Ordering differences only*

```diff
@@ -1,154 +1,154 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.IgaApplication
-
-import KratosMultiphysics.kratos_utilities
-
-def Factory(settings, model):
-    if not (isinstance(settings, KratosMultiphysics.Parameters)):
-        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
-    return IgaOutputProcess(model, settings["Parameters"])
-
-class IgaOutputProcess(KratosMultiphysics.Process):
-
-    def __init__(self, model, params):
-        KratosMultiphysics.Process.__init__(self)
-
-        ## Settings string in json format
-        default_parameters = KratosMultiphysics.Parameters("""{
-            "nodal_results"             : [],
-            "integration_point_results" : [],
-            "output_file_name"          : "",
-            "model_part_name"           : "",
-            "file_label"                : "step",
-            "output_control_type"       : "step",
-            "output_frequency"          : 1.0
-        }""")
-
-        ## Overwrite the default settings with user-provided parameters
-        self.params = params
-        self.params.ValidateAndAssignDefaults(default_parameters)
-
-        self.model_part = model[self.params["model_part_name"].GetString()]
-
-        self.output_file_name = self.params["output_file_name"].GetString()
-        if not self.output_file_name.endswith(".post.res"):
-            self.output_file_name += ".post.res"
-
-        self.nodal_results_scalar, self.nodal_results_vector = \
-            CreateVariablesListFromInput(self.params["nodal_results"])
-
-        self.integration_point_results_scalar, self.integration_point_results_vector = \
-            CreateVariablesListFromInput(self.params["integration_point_results"])
-
-        # Set up output frequency and format
-        output_file_label = self.params["file_label"].GetString()
-        if output_file_label == "time":
-            self.output_label_is_time = True
-        elif output_file_label == "step":
-            self.output_label_is_time = False
-        else:
-            msg = '{} Error: Unknown value "{}" read for parameter "file_label"'.format(self.__class__.__name__,output_file_label)
-            raise Exception(msg)
-
-        output_control_type = self.params["output_control_type"].GetString()
-        if output_control_type == "time":
-            self.output_control_is_time = True
-        elif output_control_type == "step":
-            self.output_control_is_time = False
-        else:
-            err_msg  = 'The requested "output_control_type" "' + output_control_type
-            err_msg += '" is not available!\nAvailable options are: "time", "step"'
-            raise Exception(err_msg)
-
-        self.output_frequency = self.params["output_frequency"].GetDouble()
-
-        self.step_count = 0
-        self.printed_step_count = 0
-        self.next_output = 0.0
-
-    def ExecuteBeforeSolutionLoop(self):
-        with open(self.output_file_name, 'w') as output_file:
-            output_file.write("Post Results File 1.0\n")
-
-    def PrintOutput(self):
-        time = GetPrettyTime(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
-        self.printed_step_count += 1
-        self.model_part.ProcessInfo[KratosMultiphysics.PRINTED_STEP] = self.printed_step_count
-        if self.output_label_is_time:
-            label = time
-        else:
-            label = self.printed_step_count
-
-        with open(self.output_file_name, 'a') as output_file:
-            for variable in self.nodal_results_scalar:
-                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Scalar OnNodes\nValues\n")
-                for node in self.model_part.Nodes:
-                    value = node.GetSolutionStepValue(variable, 0)
-                    output_file.write(str(node.Id) + "  " + str(value) + "\n")
-                output_file.write("End Values\n")
-
-            for variable in self.nodal_results_vector:
-                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Vector OnNodes\nValues\n")
-                for node in self.model_part.Nodes:
-                    value = node.GetSolutionStepValue(variable, 0)
-                    output_file.write(str(node.Id) + "  " + str(value[0]) + "  " +  str(value[1]) + "  " + str(value[2]) + "\n")
-                output_file.write("End Values\n")
-
-            for variable in self.integration_point_results_scalar:
-                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Scalar OnGaussPoints\nValues\n")
-                for element in self.model_part.Elements:
-                    value = element.CalculateOnIntegrationPoints(variable, self.model_part.ProcessInfo)[0]
-                    output_file.write(str(element.Id) + "  " + str(value) + "\n")
-                output_file.write("End Values\n")
-
-            for variable in self.integration_point_results_vector:
-                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Vector OnGaussPoints\nValues\n")
-                for element in self.model_part.Elements:
-                    value = element.CalculateOnIntegrationPoints(variable, self.model_part.ProcessInfo)[0]
-                    if( len(value) == 3):
-                        output_file.write(str(element.Id) + "  " + str(value[0]) + "  " +  str(value[1]) + "  " + str(value[2]) + "\n")
-                    elif( len(value) == 6):
-                        output_file.write(str(element.Id) + "  " + str(value[0]) + "  " +  str(value[1]) + "  " + str(value[2])  + "  " + str(value[3]) + "  " +  str(value[4]) + "  " + str(value[5]) + "\n")
-                output_file.write("End Values\n")
-
-        # Schedule next output
-        if self.output_frequency > 0.0: # Note: if == 0, we'll just always print
-            if self.output_control_is_time:
-                while GetPrettyTime(self.next_output) <= time:
-                    self.next_output += self.output_frequency
-            else:
-                while self.next_output <= self.step_count:
-                    self.next_output += self.output_frequency
-
-    def IsOutputStep(self):
-        if self.output_control_is_time:
-            time = GetPrettyTime(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
-            return (time >= GetPrettyTime(self.next_output))
-        else:
-            return ( self.step_count >= self.next_output )
-
-def GetPrettyTime(time):
-    pretty_time = "{0:.12g}".format(time)
-    pretty_time = float(pretty_time)
-    return pretty_time
-
-def CreateVariablesListFromInput(param):
-    '''Parse a list of variables from input.'''
-    scalar_variables = []
-    vector_variables = []
-    admissible_scalar_types = ["Bool", "Integer", "Unsigned Integer", "Double"]
-    admissible_vector_types = ["Array", "Vector"]
-
-    variable_list = KratosMultiphysics.kratos_utilities.GenerateVariableListFromInput(param)
-
-    # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
-    for variable in variable_list:
-        if KratosMultiphysics.KratosGlobals.GetVariableType(variable.Name()) in admissible_scalar_types:
-            scalar_variables.append(variable)
-        elif KratosMultiphysics.KratosGlobals.GetVariableType(variable.Name()) in admissible_vector_types:
-            vector_variables.append(variable)
-        else:
-            raise Exception("unsupported variables type: " + str(type(variable)))
-
-    return scalar_variables, vector_variables
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.IgaApplication
+
+import KratosMultiphysics.kratos_utilities
+
+def Factory(settings, model):
+    if not (isinstance(settings, KratosMultiphysics.Parameters)):
+        raise Exception("Expected input shall be a Parameters object, encapsulating a json string")
+    return IgaOutputProcess(model, settings["Parameters"])
+
+class IgaOutputProcess(KratosMultiphysics.Process):
+
+    def __init__(self, model, params):
+        KratosMultiphysics.Process.__init__(self)
+
+        ## Settings string in json format
+        default_parameters = KratosMultiphysics.Parameters("""{
+            "nodal_results"             : [],
+            "integration_point_results" : [],
+            "output_file_name"          : "",
+            "model_part_name"           : "",
+            "file_label"                : "step",
+            "output_control_type"       : "step",
+            "output_frequency"          : 1.0
+        }""")
+
+        ## Overwrite the default settings with user-provided parameters
+        self.params = params
+        self.params.ValidateAndAssignDefaults(default_parameters)
+
+        self.model_part = model[self.params["model_part_name"].GetString()]
+
+        self.output_file_name = self.params["output_file_name"].GetString()
+        if not self.output_file_name.endswith(".post.res"):
+            self.output_file_name += ".post.res"
+
+        self.nodal_results_scalar, self.nodal_results_vector = \
+            CreateVariablesListFromInput(self.params["nodal_results"])
+
+        self.integration_point_results_scalar, self.integration_point_results_vector = \
+            CreateVariablesListFromInput(self.params["integration_point_results"])
+
+        # Set up output frequency and format
+        output_file_label = self.params["file_label"].GetString()
+        if output_file_label == "time":
+            self.output_label_is_time = True
+        elif output_file_label == "step":
+            self.output_label_is_time = False
+        else:
+            msg = '{} Error: Unknown value "{}" read for parameter "file_label"'.format(self.__class__.__name__,output_file_label)
+            raise Exception(msg)
+
+        output_control_type = self.params["output_control_type"].GetString()
+        if output_control_type == "time":
+            self.output_control_is_time = True
+        elif output_control_type == "step":
+            self.output_control_is_time = False
+        else:
+            err_msg  = 'The requested "output_control_type" "' + output_control_type
+            err_msg += '" is not available!\nAvailable options are: "time", "step"'
+            raise Exception(err_msg)
+
+        self.output_frequency = self.params["output_frequency"].GetDouble()
+
+        self.step_count = 0
+        self.printed_step_count = 0
+        self.next_output = 0.0
+
+    def ExecuteBeforeSolutionLoop(self):
+        with open(self.output_file_name, 'w') as output_file:
+            output_file.write("Post Results File 1.0\n")
+
+    def PrintOutput(self):
+        time = GetPrettyTime(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
+        self.printed_step_count += 1
+        self.model_part.ProcessInfo[KratosMultiphysics.PRINTED_STEP] = self.printed_step_count
+        if self.output_label_is_time:
+            label = time
+        else:
+            label = self.printed_step_count
+
+        with open(self.output_file_name, 'a') as output_file:
+            for variable in self.nodal_results_scalar:
+                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Scalar OnNodes\nValues\n")
+                for node in self.model_part.Nodes:
+                    value = node.GetSolutionStepValue(variable, 0)
+                    output_file.write(str(node.Id) + "  " + str(value) + "\n")
+                output_file.write("End Values\n")
+
+            for variable in self.nodal_results_vector:
+                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Vector OnNodes\nValues\n")
+                for node in self.model_part.Nodes:
+                    value = node.GetSolutionStepValue(variable, 0)
+                    output_file.write(str(node.Id) + "  " + str(value[0]) + "  " +  str(value[1]) + "  " + str(value[2]) + "\n")
+                output_file.write("End Values\n")
+
+            for variable in self.integration_point_results_scalar:
+                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Scalar OnGaussPoints\nValues\n")
+                for element in self.model_part.Elements:
+                    value = element.CalculateOnIntegrationPoints(variable, self.model_part.ProcessInfo)[0]
+                    output_file.write(str(element.Id) + "  " + str(value) + "\n")
+                output_file.write("End Values\n")
+
+            for variable in self.integration_point_results_vector:
+                output_file.write("Result \"" + variable.Name() + "\" \"Load Case\" " + str(label) + " Vector OnGaussPoints\nValues\n")
+                for element in self.model_part.Elements:
+                    value = element.CalculateOnIntegrationPoints(variable, self.model_part.ProcessInfo)[0]
+                    if( len(value) == 3):
+                        output_file.write(str(element.Id) + "  " + str(value[0]) + "  " +  str(value[1]) + "  " + str(value[2]) + "\n")
+                    elif( len(value) == 6):
+                        output_file.write(str(element.Id) + "  " + str(value[0]) + "  " +  str(value[1]) + "  " + str(value[2])  + "  " + str(value[3]) + "  " +  str(value[4]) + "  " + str(value[5]) + "\n")
+                output_file.write("End Values\n")
+
+        # Schedule next output
+        if self.output_frequency > 0.0: # Note: if == 0, we'll just always print
+            if self.output_control_is_time:
+                while GetPrettyTime(self.next_output) <= time:
+                    self.next_output += self.output_frequency
+            else:
+                while self.next_output <= self.step_count:
+                    self.next_output += self.output_frequency
+
+    def IsOutputStep(self):
+        if self.output_control_is_time:
+            time = GetPrettyTime(self.model_part.ProcessInfo[KratosMultiphysics.TIME])
+            return (time >= GetPrettyTime(self.next_output))
+        else:
+            return ( self.step_count >= self.next_output )
+
+def GetPrettyTime(time):
+    pretty_time = "{0:.12g}".format(time)
+    pretty_time = float(pretty_time)
+    return pretty_time
+
+def CreateVariablesListFromInput(param):
+    '''Parse a list of variables from input.'''
+    scalar_variables = []
+    vector_variables = []
+    admissible_scalar_types = ["Bool", "Integer", "Unsigned Integer", "Double"]
+    admissible_vector_types = ["Array", "Vector"]
+
+    variable_list = KratosMultiphysics.kratos_utilities.GenerateVariableListFromInput(param)
+
+    # Retrieve variable name from input (a string) and request the corresponding C++ object to the kernel
+    for variable in variable_list:
+        if KratosMultiphysics.KratosGlobals.GetVariableType(variable.Name()) in admissible_scalar_types:
+            scalar_variables.append(variable)
+        elif KratosMultiphysics.KratosGlobals.GetVariableType(variable.Name()) in admissible_vector_types:
+            vector_variables.append(variable)
+        else:
+            raise Exception("unsupported variables type: " + str(type(variable)))
+
+    return scalar_variables, vector_variables
```

## KratosMultiphysics/IgaApplication/vtk_embedded_geometry_output_process.py

 * *Ordering differences only*

```diff
@@ -1,56 +1,56 @@
-import KratosMultiphysics
-from KratosMultiphysics.IgaApplication.map_nurbs_volume_results_to_embedded_geometry_process import MapNurbsVolumeResultsToEmbeddedGeometryProcess
-from KratosMultiphysics.vtk_output_process import VtkOutputProcess
-
-def Factory(settings, model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return VtkEmbeddeGeometryOutputProcess(model, settings["Parameters"])
-
-
-class VtkEmbeddeGeometryOutputProcess(KratosMultiphysics.OutputProcess):
-    def __init__(self, model, settings):
-        super().__init__()
-
-        mapping_settings = settings["mapping_parameters"]
-        vtk_settings = settings["vtk_parameters"]
-
-        # Check for invalid variable_names.
-        self.VariableCheck(vtk_settings, "nodal_flags")
-        self.VariableCheck(vtk_settings, "element_data_value_variables")
-        self.VariableCheck(vtk_settings, "element_flags")
-        self.VariableCheck(vtk_settings, "condition_data_value_variables")
-        self.VariableCheck(vtk_settings, "condition_flags")
-        self.VariableCheck(vtk_settings, "gauss_point_variables_extrapolated_to_nodes")
-
-        # Map all values to from main_model_part to embedded_model_part.
-        process_params = KratosMultiphysics.Parameters(
-        """ {
-                "main_model_part_name"                    : "",
-                "nurbs_volume_name"                       : "",
-                "embedded_model_part_name"                : "",
-                "nodal_results": [],
-                "gauss_point_results" : []
-        } """ )
-
-        process_params["main_model_part_name"].SetString(mapping_settings["main_model_part_name"].GetString())
-        process_params["nurbs_volume_name"].SetString(mapping_settings["nurbs_volume_name"].GetString())
-        process_params["embedded_model_part_name"].SetString(mapping_settings["embedded_model_part_name"].GetString())
-        process_params["nodal_results"].SetStringArray(vtk_settings["nodal_solution_step_data_variables"].GetStringArray())
-        process_params["gauss_point_results"].SetStringArray(vtk_settings["nodal_data_value_variables"].GetStringArray())
-        self.process = MapNurbsVolumeResultsToEmbeddedGeometryProcess(model, process_params)
-
-        # Create vtk output process
-        self.vtk_io = VtkOutputProcess(model, vtk_settings) # this also validates the settings
-
-    def VariableCheck(self, settings, variable_name):
-        if( settings[variable_name].size() > 0 ):
-            err_msg = "Variable '" + variable_name + "' is not available. Please use nodal_solution_step_data_variables"
-            err_msg += "or nodal_data_value_variables"
-            raise Exception(err_msg)
-
-    def PrintOutput(self):
-        self.process.ExecuteBeforeOutputStep()
-        self.vtk_io.PrintOutput()
-
-
+import KratosMultiphysics
+from KratosMultiphysics.IgaApplication.map_nurbs_volume_results_to_embedded_geometry_process import MapNurbsVolumeResultsToEmbeddedGeometryProcess
+from KratosMultiphysics.vtk_output_process import VtkOutputProcess
+
+def Factory(settings, model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return VtkEmbeddeGeometryOutputProcess(model, settings["Parameters"])
+
+
+class VtkEmbeddeGeometryOutputProcess(KratosMultiphysics.OutputProcess):
+    def __init__(self, model, settings):
+        super().__init__()
+
+        mapping_settings = settings["mapping_parameters"]
+        vtk_settings = settings["vtk_parameters"]
+
+        # Check for invalid variable_names.
+        self.VariableCheck(vtk_settings, "nodal_flags")
+        self.VariableCheck(vtk_settings, "element_data_value_variables")
+        self.VariableCheck(vtk_settings, "element_flags")
+        self.VariableCheck(vtk_settings, "condition_data_value_variables")
+        self.VariableCheck(vtk_settings, "condition_flags")
+        self.VariableCheck(vtk_settings, "gauss_point_variables_extrapolated_to_nodes")
+
+        # Map all values to from main_model_part to embedded_model_part.
+        process_params = KratosMultiphysics.Parameters(
+        """ {
+                "main_model_part_name"                    : "",
+                "nurbs_volume_name"                       : "",
+                "embedded_model_part_name"                : "",
+                "nodal_results": [],
+                "gauss_point_results" : []
+        } """ )
+
+        process_params["main_model_part_name"].SetString(mapping_settings["main_model_part_name"].GetString())
+        process_params["nurbs_volume_name"].SetString(mapping_settings["nurbs_volume_name"].GetString())
+        process_params["embedded_model_part_name"].SetString(mapping_settings["embedded_model_part_name"].GetString())
+        process_params["nodal_results"].SetStringArray(vtk_settings["nodal_solution_step_data_variables"].GetStringArray())
+        process_params["gauss_point_results"].SetStringArray(vtk_settings["nodal_data_value_variables"].GetStringArray())
+        self.process = MapNurbsVolumeResultsToEmbeddedGeometryProcess(model, process_params)
+
+        # Create vtk output process
+        self.vtk_io = VtkOutputProcess(model, vtk_settings) # this also validates the settings
+
+    def VariableCheck(self, settings, variable_name):
+        if( settings[variable_name].size() > 0 ):
+            err_msg = "Variable '" + variable_name + "' is not available. Please use nodal_solution_step_data_variables"
+            err_msg += "or nodal_data_value_variables"
+            raise Exception(err_msg)
+
+    def PrintOutput(self):
+        self.process.ExecuteBeforeOutputStep()
+        self.vtk_io.PrintOutput()
+
+
```

## KratosMultiphysics/IgaApplication/set_directors_process.py

 * *Ordering differences only*

```diff
@@ -1,44 +1,44 @@
-# Importing the Kratos Library
-import KratosMultiphysics
-import KratosMultiphysics.IgaApplication as IGA
-
-import math
-import numpy
-
-def Factory(settings, Model):
-    if not isinstance(settings, KratosMultiphysics.Parameters):
-        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
-    return SetDirectorsProcess(Model, settings["Parameters"])
-
-## All the processes python should be derived from "Process"
-class SetDirectorsProcess(KratosMultiphysics.Process):
-    """
-    Only the member variables listed below should be accessed directly.
-
-    Public member variables:
-    Model -- the container of the different model parts.
-    settings -- Kratos parameters containing solver settings.
-    """
-
-    def __init__(self, Model, settings ):
-        """ The default constructor of the class
-
-        Keyword arguments:
-        self -- It signifies an instance of a class.
-        Model -- the container of the different model parts.
-        settings -- Kratos parameters containing solver settings.
-        """
-        KratosMultiphysics.Process.__init__(self)
-
-        default_settings = KratosMultiphysics.Parameters("""
-        {
-            "model_part_name"      : "please_specify_model_part_name"
-        }
-        """)
-
-        self.model_part = Model[settings["model_part_name"].GetString()]
-
-        self.director_utilities = IGA.DirectorUtilities(self.model_part, settings)
-
-    def ExecuteInitialize(self):
+# Importing the Kratos Library
+import KratosMultiphysics
+import KratosMultiphysics.IgaApplication as IGA
+
+import math
+import numpy
+
+def Factory(settings, Model):
+    if not isinstance(settings, KratosMultiphysics.Parameters):
+        raise Exception("expected input shall be a Parameters object, encapsulating a json string")
+    return SetDirectorsProcess(Model, settings["Parameters"])
+
+## All the processes python should be derived from "Process"
+class SetDirectorsProcess(KratosMultiphysics.Process):
+    """
+    Only the member variables listed below should be accessed directly.
+
+    Public member variables:
+    Model -- the container of the different model parts.
+    settings -- Kratos parameters containing solver settings.
+    """
+
+    def __init__(self, Model, settings ):
+        """ The default constructor of the class
+
+        Keyword arguments:
+        self -- It signifies an instance of a class.
+        Model -- the container of the different model parts.
+        settings -- Kratos parameters containing solver settings.
+        """
+        KratosMultiphysics.Process.__init__(self)
+
+        default_settings = KratosMultiphysics.Parameters("""
+        {
+            "model_part_name"      : "please_specify_model_part_name"
+        }
+        """)
+
+        self.model_part = Model[settings["model_part_name"].GetString()]
+
+        self.director_utilities = IGA.DirectorUtilities(self.model_part, settings)
+
+    def ExecuteInitialize(self):
         self.director_utilities.ComputeDirectors()
```

## KratosMultiphysics/IgaApplication/__init__.py

 * *Ordering differences only*

```diff
@@ -1,17 +1,17 @@
-#
-#   KRATOS  _____________
-#          /  _/ ____/   |
-#          / // / __/ /| |
-#        _/ // /_/ / ___ |
-#       /___/\____/_/  |_| Application
-#
-#   Main authors:   Thomas Oberbichler
-#
-
-# Application dependent names and paths
-from KratosMultiphysics import _ImportApplication
-from KratosIgaApplication import *
-application = KratosIgaApplication()
-application_name = "KratosIgaApplication"
-
-_ImportApplication(application, application_name)
+#
+#   KRATOS  _____________
+#          /  _/ ____/   |
+#          / // / __/ /| |
+#        _/ // /_/ / ___ |
+#       /___/\____/_/  |_| Application
+#
+#   Main authors:   Thomas Oberbichler
+#
+
+# Application dependent names and paths
+from KratosMultiphysics import _ImportApplication
+from KratosIgaApplication import *
+application = KratosIgaApplication()
+application_name = "KratosIgaApplication"
+
+_ImportApplication(application, application_name)
```

## Comparing `KratosIgaApplication-9.5.dist-info/METADATA` & `KratosIgaApplication-9.5.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1
-Name: KratosIgaApplication
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
-
+Metadata-Version: 2.1
+Name: KratosIgaApplication
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
+
```

## Comparing `KratosIgaApplication-9.5.dist-info/RECORD` & `KratosIgaApplication-9.5.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-KratosIgaApplication-9.5.dist-info/METADATA,sha256=Hazadp_wEAMKUhwTTth4WAO7FLQwKyddv3NT09ZI5DU,1343
-KratosIgaApplication-9.5.dist-info/WHEEL,sha256=rY0Y6THYM7EImsHfF-zs67o8pQciAsMw9_YuSvftjrQ,148
-KratosIgaApplication-9.5.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
-KratosIgaApplication-9.5.dist-info/RECORD,,
-KratosMultiphysics/IgaApplication/output_eigen_values_process.py,sha256=8bR6DdAYVzxH-FPsOVNTgPjYjqyLomIc9JHvc1NMoWM,373
-KratosMultiphysics/IgaApplication/output_quadrature_domain_process.py,sha256=JJId5G4cFPZmLnOacMeHLWmhNQNyDtn8MgTyRcyWPWM,710
-KratosMultiphysics/IgaApplication/assign_integration_points_to_background_elements_process.py,sha256=ARprfdaEZ1H7vD7xLOrebJfdaft7ZXH-AzU9KvQpGD8,397
-KratosMultiphysics/IgaApplication/nitsche_stabilization_process.py,sha256=wMMY8ZivYTvCt9YZVCagEVJ8D9YXs9-aL1ei2j9I1W0,4308
-KratosMultiphysics/IgaApplication/kratos_main_iga.py,sha256=kFCodbu-FSY_ZK2v1WkvRzqrw-p0rNXZcaDPiFxTKnk,706
-KratosMultiphysics/IgaApplication/map_nurbs_volume_results_to_embedded_geometry_process.py,sha256=vSznfssSxGW7wMI2Nwk4yGnYzUe19oeZ3EgOdjPaZIs,803
-KratosMultiphysics/IgaApplication/assign_vector_variable_and_constraints_to_conditions_process.py,sha256=WnAgl3VqBWizX2DwRzfMOGvbvdUVb0Y-MwyDDg6lGsQ,4393
-KratosMultiphysics/IgaApplication/iga_output_process.py,sha256=msI0xKu1ypnVIwe-AVmGxVLAeI7c7X-FgHRSsH2Ojp4,7492
-KratosMultiphysics/IgaApplication/__init__.pyi,sha256=gpgRTTzbSm9hCUJ59gusCXcLo0y-KjelYr6CucssaC4,1789
-KratosMultiphysics/IgaApplication/vtk_embedded_geometry_output_process.py,sha256=eBa6f8mBJ3bbfnMq-8x-qJevImGabjyeNH5yT-NfZG4,2884
-KratosMultiphysics/IgaApplication/set_directors_process.py,sha256=mcDK68O5x6GIFGD8e_gxsj3HkhlCiKKWGabXFCPvaHI,1511
-KratosMultiphysics/IgaApplication/__init__.py,sha256=TRsr4b42GslJTvVLxeWJPrXS9HWcMyUgSz1hsAGqOhI,447
-KratosMultiphysics/.libs/KratosIgaApplication.cpython-39-x86_64-linux-gnu.so,sha256=a1wOk0yEI2WOF8PtgJIH0rCSpBtLQIZRy2F0K5AMRos,2164081
-KratosMultiphysics/.libs/libKratosIgaCore.so,sha256=pxW5Q8o2hXZuOSdvoH5dvJgAcNAecvPcwjnkF1--4ls,6190785
-KratosIgaApplication.libs/libKratosIgaCore-9fdd436e.so,sha256=MxRdD1r0GfuVBcU59Bx-IPsSkybTUMJ3CqREA-3PGCs,6546497
+KratosMultiphysics/.libs/KratosIgaApplication.pyd,sha256=VZ5bEN3P5DL2jHKNdR63Kd2wWnDGvg55swG1iYjvZb4,793088
+KratosMultiphysics/.libs/KratosIgaCore.dll,sha256=yR-94Y8r6-1HfosGe2MuBD1FtVz819R_-oNPBeCXry8,1940480
+KratosMultiphysics/.libs/KratosIgaCore.lib,sha256=P-WNTt4QMFOZwK_u77RdcVHp1c_2ncbbtdYHykQdrQ0,154612
+KratosMultiphysics/IgaApplication/__init__.py,sha256=ABlpaYNXV1wkbaY2YKyTQQt6dWTAHq6whHwBLTuFAi8,464
+KratosMultiphysics/IgaApplication/assign_integration_points_to_background_elements_process.py,sha256=4kq5iUHpYwI-7e0qLfaU2RZ37zHFgWzb3sKN-Dw71pA,405
+KratosMultiphysics/IgaApplication/assign_vector_variable_and_constraints_to_conditions_process.py,sha256=omIMjN30pn1Do3XbHAHmFFE0QV9JkiZuLRl94U-Y_0Y,4486
+KratosMultiphysics/IgaApplication/iga_output_process.py,sha256=dp0vQ31i6dkYoY2L15vf1qiOglq9ifmZR_MNO7i8wM8,7646
+KratosMultiphysics/IgaApplication/kratos_main_iga.py,sha256=vNNnKC-4JzkxhMc6Q7IOxd05dghkQqpOyEvZ4NIxaJU,725
+KratosMultiphysics/IgaApplication/map_nurbs_volume_results_to_embedded_geometry_process.py,sha256=v4W-tHfHjK4_Iq5iRaGMn2vqQSkej31fhIbgL8cPaWU,821
+KratosMultiphysics/IgaApplication/nitsche_stabilization_process.py,sha256=4woHm8sk3l6lAUU2tIu0ltEbp8Nt8_l27YzWZU4YiDA,4394
+KratosMultiphysics/IgaApplication/output_eigen_values_process.py,sha256=NLq0mVUW3GLEEqMUYf6d3_5Sd1SvYEBvhFd5t7GFSK4,381
+KratosMultiphysics/IgaApplication/output_quadrature_domain_process.py,sha256=JJId5G4cFPZmLnOacMeHLWmhNQNyDtn8MgTyRcyWPWM,710
+KratosMultiphysics/IgaApplication/set_directors_process.py,sha256=FLN4oNbCyFyg8_gqTVKKiYCORlGX6X_maEFDkrsEpzo,1554
+KratosMultiphysics/IgaApplication/vtk_embedded_geometry_output_process.py,sha256=z4vFYxHtBgIMHnDVskcB48WfgnK5eaurEOt6W5WLXXY,2940
+KratosIgaApplication-9.5.1.dist-info/METADATA,sha256=8_PKgpQXdBBXHvejJUX_SqSY4vZJzCgu9JLAocb_Vfk,1427
+KratosIgaApplication-9.5.1.dist-info/WHEEL,sha256=GZFS91_ufm4WrNPBaFVPB9MvOXR6bMZQhPcZRRTN5YM,100
+KratosIgaApplication-9.5.1.dist-info/top_level.txt,sha256=8Ov--opRCptLbHStjyiZUVpzN1OUU_F7c7fGmsR5cMc,19
+KratosIgaApplication-9.5.1.dist-info/RECORD,,
```

