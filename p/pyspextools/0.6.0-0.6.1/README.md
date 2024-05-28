# Comparing `tmp/pyspextools-0.6.0.tar.gz` & `tmp/pyspextools-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspextools-0.6.0.tar", last modified: Thu Nov 16 10:52:46 2023, max compression
+gzip compressed data, was "pyspextools-0.6.1.tar", last modified: Tue May 28 09:43:53 2024, max compression
```

## Comparing `pyspextools-0.6.0.tar` & `pyspextools-0.6.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jellep     (502) staff       (20)        0 2023-11-16 10:52:46.078063 pyspextools-0.6.0/
--rw-r--r--   0 jellep     (502) staff       (20)    10173 2022-09-01 14:22:03.000000 pyspextools-0.6.0/LICENSE.txt
--rw-r--r--   0 jellep     (502) staff       (20)      604 2023-11-16 09:23:42.000000 pyspextools-0.6.0/NOTICE
--rw-r--r--   0 jellep     (502) staff       (20)     1692 2023-11-16 10:52:46.077731 pyspextools-0.6.0/PKG-INFO
--rw-r--r--   0 jellep     (502) staff       (20)     1367 2022-09-01 14:22:03.000000 pyspextools-0.6.0/README.md
-drwxr-xr-x   0 jellep     (502) staff       (20)        0 2023-11-16 10:52:45.997357 pyspextools-0.6.0/pyspextools/
--rw-r--r--   0 jellep     (502) staff       (20)       45 2023-11-16 09:23:42.000000 pyspextools-0.6.0/pyspextools/__init__.py
--rw-r--r--   0 jellep     (502) staff       (20)     1971 2023-03-06 08:10:31.000000 pyspextools-0.6.0/pyspextools/color.py
-drwxr-xr-x   0 jellep     (502) staff       (20)        0 2023-11-16 10:52:46.009801 pyspextools-0.6.0/pyspextools/data/
--rw-r--r--   0 jellep     (502) staff       (20)       49 2022-09-01 14:22:03.000000 pyspextools-0.6.0/pyspextools/data/__init__.py
--rw-r--r--   0 jellep     (502) staff       (20)     6828 2023-03-21 14:30:52.000000 pyspextools-0.6.0/pyspextools/data/badchannels.py
--rw-r--r--   0 jellep     (502) staff       (20)     1361 2023-03-06 08:10:31.000000 pyspextools-0.6.0/pyspextools/data/response.py
-drwxr-xr-x   0 jellep     (502) staff       (20)        0 2023-11-16 10:52:46.058950 pyspextools-0.6.0/pyspextools/io/
--rw-r--r--   0 jellep     (502) staff       (20)      289 2022-09-01 14:22:03.000000 pyspextools-0.6.0/pyspextools/io/__init__.py
--rw-r--r--   0 jellep     (502) staff       (20)     5706 2023-03-06 08:10:31.000000 pyspextools-0.6.0/pyspextools/io/arf.py
--rw-r--r--   0 jellep     (502) staff       (20)    10839 2023-03-21 14:26:26.000000 pyspextools-0.6.0/pyspextools/io/convert.py
--rw-r--r--   0 jellep     (502) staff       (20)    12878 2023-11-15 09:43:48.000000 pyspextools-0.6.0/pyspextools/io/dataset.py
--rw-r--r--   0 jellep     (502) staff       (20)    22281 2023-11-09 10:26:13.000000 pyspextools-0.6.0/pyspextools/io/ogip.py
--rw-r--r--   0 jellep     (502) staff       (20)    13006 2023-11-09 12:14:37.000000 pyspextools-0.6.0/pyspextools/io/pha.py
--rw-r--r--   0 jellep     (502) staff       (20)     8030 2023-03-06 08:10:31.000000 pyspextools-0.6.0/pyspextools/io/pha2.py
--rw-r--r--   0 jellep     (502) staff       (20)     4275 2023-03-06 08:10:31.000000 pyspextools-0.6.0/pyspextools/io/region.py
--rw-r--r--   0 jellep     (502) staff       (20)    28459 2023-03-27 13:48:59.000000 pyspextools-0.6.0/pyspextools/io/res.py
--rw-r--r--   0 jellep     (502) staff       (20)    22208 2023-11-09 09:25:09.000000 pyspextools-0.6.0/pyspextools/io/rmf.py
--rw-r--r--   0 jellep     (502) staff       (20)    23228 2023-03-27 13:48:59.000000 pyspextools-0.6.0/pyspextools/io/spo.py
--rw-r--r--   0 jellep     (502) staff       (20)     6570 2023-03-06 08:10:31.000000 pyspextools-0.6.0/pyspextools/io/tg.py
--rw-r--r--   0 jellep     (502) staff       (20)     2320 2023-03-27 13:48:59.000000 pyspextools-0.6.0/pyspextools/messages.py
-drwxr-xr-x   0 jellep     (502) staff       (20)        0 2023-11-16 10:52:46.065143 pyspextools-0.6.0/pyspextools/model/
--rw-r--r--   0 jellep     (502) staff       (20)       46 2022-09-01 14:22:03.000000 pyspextools-0.6.0/pyspextools/model/__init__.py
--rw-r--r--   0 jellep     (502) staff       (20)     6355 2022-09-01 14:22:03.000000 pyspextools-0.6.0/pyspextools/model/user.py
-drwxr-xr-x   0 jellep     (502) staff       (20)        0 2023-11-16 10:52:46.002766 pyspextools-0.6.0/pyspextools.egg-info/
--rw-r--r--   0 jellep     (502) staff       (20)     1692 2023-11-16 10:52:45.000000 pyspextools-0.6.0/pyspextools.egg-info/PKG-INFO
--rw-r--r--   0 jellep     (502) staff       (20)      775 2023-11-16 10:52:45.000000 pyspextools-0.6.0/pyspextools.egg-info/SOURCES.txt
--rw-r--r--   0 jellep     (502) staff       (20)        1 2023-11-16 10:52:45.000000 pyspextools-0.6.0/pyspextools.egg-info/dependency_links.txt
--rw-r--r--   0 jellep     (502) staff       (20)       64 2023-11-16 10:52:45.000000 pyspextools-0.6.0/pyspextools.egg-info/requires.txt
--rw-r--r--   0 jellep     (502) staff       (20)       12 2023-11-16 10:52:45.000000 pyspextools-0.6.0/pyspextools.egg-info/top_level.txt
-drwxr-xr-x   0 jellep     (502) staff       (20)        0 2023-11-16 10:52:46.077285 pyspextools-0.6.0/scripts/
--rw-r--r--   0 jellep     (502) staff       (20)     4193 2023-11-09 10:26:13.000000 pyspextools-0.6.0/scripts/ogip2spex
--rw-r--r--   0 jellep     (502) staff       (20)     8057 2023-11-08 14:49:58.000000 pyspextools-0.6.0/scripts/ogipgenrsp
--rw-r--r--   0 jellep     (502) staff       (20)     4345 2023-03-06 08:10:31.000000 pyspextools-0.6.0/scripts/simres
--rw-r--r--   0 jellep     (502) staff       (20)     9330 2023-03-06 08:10:31.000000 pyspextools-0.6.0/scripts/tg2spex
--rw-r--r--   0 jellep     (502) staff       (20)       38 2023-11-16 10:52:46.078128 pyspextools-0.6.0/setup.cfg
--rw-r--r--   0 jellep     (502) staff       (20)     1910 2023-11-16 10:22:18.000000 pyspextools-0.6.0/setup.py
+drwxr-xr-x   0 jellep    (1128) hea       (4400)        0 2024-05-28 09:43:53.677346 pyspextools-0.6.1/
+-rw-r--r--   0 jellep    (1128) hea       (4400)    10173 2024-05-27 12:53:04.000000 pyspextools-0.6.1/LICENSE.txt
+-rw-r--r--   0 jellep    (1128) hea       (4400)      604 2024-05-27 12:53:04.000000 pyspextools-0.6.1/NOTICE
+-rw-r--r--   0 jellep    (1128) hea       (4400)     1692 2024-05-28 09:43:53.677346 pyspextools-0.6.1/PKG-INFO
+-rw-r--r--   0 jellep    (1128) hea       (4400)     1367 2024-05-27 12:53:04.000000 pyspextools-0.6.1/README.md
+drwxr-xr-x   0 jellep    (1128) hea       (4400)        0 2024-05-28 09:43:53.673346 pyspextools-0.6.1/pyspextools/
+-rw-r--r--   0 jellep    (1128) hea       (4400)       45 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/__init__.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     1971 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/color.py
+drwxr-xr-x   0 jellep    (1128) hea       (4400)        0 2024-05-28 09:43:53.673346 pyspextools-0.6.1/pyspextools/data/
+-rw-r--r--   0 jellep    (1128) hea       (4400)       49 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/data/__init__.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     7040 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/data/badchannels.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     1361 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/data/response.py
+drwxr-xr-x   0 jellep    (1128) hea       (4400)        0 2024-05-28 09:43:53.673346 pyspextools-0.6.1/pyspextools/io/
+-rw-r--r--   0 jellep    (1128) hea       (4400)      289 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/__init__.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     5852 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/arf.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)    11086 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/convert.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)    12878 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/dataset.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)    22281 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/ogip.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)    13006 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/pha.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     8030 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/pha2.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     4275 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/region.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)    28459 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/res.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)    22208 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/rmf.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)    23228 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/spo.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     6570 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/io/tg.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     2320 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/messages.py
+drwxr-xr-x   0 jellep    (1128) hea       (4400)        0 2024-05-28 09:43:53.673346 pyspextools-0.6.1/pyspextools/model/
+-rw-r--r--   0 jellep    (1128) hea       (4400)       46 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/model/__init__.py
+-rw-r--r--   0 jellep    (1128) hea       (4400)     6355 2024-05-27 12:53:04.000000 pyspextools-0.6.1/pyspextools/model/user.py
+drwxr-xr-x   0 jellep    (1128) hea       (4400)        0 2024-05-28 09:43:53.673346 pyspextools-0.6.1/pyspextools.egg-info/
+-rw-r--r--   0 jellep    (1128) hea       (4400)     1692 2024-05-28 09:43:53.000000 pyspextools-0.6.1/pyspextools.egg-info/PKG-INFO
+-rw-r--r--   0 jellep    (1128) hea       (4400)      775 2024-05-28 09:43:53.000000 pyspextools-0.6.1/pyspextools.egg-info/SOURCES.txt
+-rw-r--r--   0 jellep    (1128) hea       (4400)        1 2024-05-28 09:43:53.000000 pyspextools-0.6.1/pyspextools.egg-info/dependency_links.txt
+-rw-r--r--   0 jellep    (1128) hea       (4400)       64 2024-05-28 09:43:53.000000 pyspextools-0.6.1/pyspextools.egg-info/requires.txt
+-rw-r--r--   0 jellep    (1128) hea       (4400)       12 2024-05-28 09:43:53.000000 pyspextools-0.6.1/pyspextools.egg-info/top_level.txt
+drwxr-xr-x   0 jellep    (1128) hea       (4400)        0 2024-05-28 09:43:53.677346 pyspextools-0.6.1/scripts/
+-rw-r--r--   0 jellep    (1128) hea       (4400)     4193 2024-05-27 12:53:04.000000 pyspextools-0.6.1/scripts/ogip2spex
+-rw-r--r--   0 jellep    (1128) hea       (4400)     8057 2024-05-27 12:53:04.000000 pyspextools-0.6.1/scripts/ogipgenrsp
+-rw-r--r--   0 jellep    (1128) hea       (4400)     4345 2024-05-27 12:53:04.000000 pyspextools-0.6.1/scripts/simres
+-rw-r--r--   0 jellep    (1128) hea       (4400)     9330 2024-05-27 12:53:04.000000 pyspextools-0.6.1/scripts/tg2spex
+-rw-r--r--   0 jellep    (1128) hea       (4400)       38 2024-05-28 09:43:53.677346 pyspextools-0.6.1/setup.cfg
+-rw-r--r--   0 jellep    (1128) hea       (4400)     1910 2024-05-27 12:53:04.000000 pyspextools-0.6.1/setup.py
```

### Comparing `pyspextools-0.6.0/LICENSE.txt` & `pyspextools-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/NOTICE` & `pyspextools-0.6.1/NOTICE`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/PKG-INFO` & `pyspextools-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspextools
-Version: 0.6.0
+Version: 0.6.1
 Summary: SPEX Python tools
 Home-page: https://github.com/spex-xray/pyspextools
 Author: SPEX development team
 Author-email: j.de.plaa@sron.nl
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `pyspextools-0.6.0/README.md` & `pyspextools-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/color.py` & `pyspextools-0.6.1/pyspextools/color.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/data/badchannels.py` & `pyspextools-0.6.1/pyspextools/data/badchannels.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,18 +156,24 @@
     respmask = np.ones(reg.res.resp.size, dtype=bool)
 
     if respmask.size != np.sum(reg.res.nc):
         message.error("Mismatch between the number of response elements in the GROUP and RESP extensions.")
         return -1
 
     ir = 0
+
     # Loop over groups to find zero response elements and finalize channel mask
     for ie in np.arange(reg.res.eg1.size):
         ic1 = reg.res.ic1[ie]  # Original first channel of group
         ic2 = reg.res.ic2[ie]  # Original last channel of group
+        # Masking entire group if response is zero
+        #grsum = np.sum(reg.res.resp[ir:ir+reg.res.nc[ie]+1])
+        #if grsum <= 0.0:
+        #    groupmask[ie] = False
+
         for j in np.arange(reg.res.nc[ie]):
             ic = ic1 + j - 1  # -1 because Python array starts at 0, not 1
             if ic > ic2 - 1:
                 message.error("Error: Mismatch in number of channels.")
             if reg.res.resp[ir] <= 0.0:
                 chanmask[ic] = False or chanmask[ic]
             else:
@@ -185,15 +191,15 @@
 
         ic1 = reg.res.ic1[ie]  # Original first channel of group
         first = True  # Is this the first channel of the group?
         newnc = 0
 
         for j in np.arange(reg.res.nc[ie]):
             ic = ic1 + j - 1
-            if chanmask[ic]:  # If channel is good
+            if chanmask[ic] and groupmask[ie]:  # If channel is good and group is good
                 newnc = newnc + 1  # Count number of good channels in group
                 if first:  # If this is the first good bin of the group, set ic1
                     first = False
                     reg.res.ic1[ie] = np.sum(chanmask[0:ic]) + 1
             else:
                 respmask[ir] = False
```

### Comparing `pyspextools-0.6.0/pyspextools/data/response.py` & `pyspextools-0.6.1/pyspextools/data/response.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/arf.py` & `pyspextools-0.6.1/pyspextools/io/arf.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """
 
     def __init__(self):
         """Initialize an ARF object."""
 
         self.LowEnergy = np.array([], dtype=float)      # Low Energy of bin
         self.HighEnergy = np.array([], dtype=float)     # High Energy of bin
+        self.CentEnergy = np.array([], dtype=float)     # Center Energy of bin
         self.EffArea = np.array([], dtype=float)        # Effective Area of bin
 
         self.EnergyUnits = 'keV'                        # Energy units
         self.ARFUnits = 'cm2'
         self.Order = 0                                  # Grating order (for grating arrays, else 0)
         self.Grating = 0                                # Grating instrument (if available, 1 = HEG, 2 = MEG, 3 = LEG)
 
@@ -45,14 +46,15 @@
         :type arffile: str
         """
 
         (data, header) = fits.getdata(arffile, 'SPECRESP', header=True)
 
         self.LowEnergy = data['ENERG_LO']
         self.HighEnergy = data['ENERG_HI']
+        self.CentEnergy = (self.LowEnergy + self.HighEnergy) / 2.0
         self.EffArea = data['SPECRESP']
 
         self.EnergyUnits = header['TUNIT1']
 
         if header['TUNIT3'] == 'cm**2':
             self.ARFUnits = 'cm2'
         elif header['TUNIT3'] == 'cm2':
```

### Comparing `pyspextools-0.6.0/pyspextools/io/convert.py` & `pyspextools-0.6.1/pyspextools/io/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,18 @@
             res.nc[g] = rmf.matrix[matext].NumberChannelsGroup[g]
             # Add the start channel to the IC to correct for cases where we start at channel 0/1
             res.ic1[g] = rmf.matrix[matext].FirstChannelGroup[g]
             ic2 = res.ic1[g] + res.nc[g] - 1
             res.ic2[g] = ic2
 
             if input_area:
-                area = arf.EffArea[i]
+                # Interpolate the effective area in case the response energy bins do not match the arf bins
+                # Center energy of response bin
+                renergy = (res.eg1[g] + res.eg2[g]) / 2.0
+                area = np.interp(renergy, arf.CentEnergy, arf.EffArea)
             else:
                 area = 1.0
 
             for k in np.arange(res.nc[g]):
                 res.resp[m] = rmf.matrix[matext].Matrix[m] * area
                 if res.resp[m] < 0.0:
                     res.resp[m] = 0.0
```

### Comparing `pyspextools-0.6.0/pyspextools/io/dataset.py` & `pyspextools-0.6.1/pyspextools/io/dataset.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/ogip.py` & `pyspextools-0.6.1/pyspextools/io/ogip.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/pha.py` & `pyspextools-0.6.1/pyspextools/io/pha.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/pha2.py` & `pyspextools-0.6.1/pyspextools/io/pha2.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/region.py` & `pyspextools-0.6.1/pyspextools/io/region.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/res.py` & `pyspextools-0.6.1/pyspextools/io/res.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/rmf.py` & `pyspextools-0.6.1/pyspextools/io/rmf.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/spo.py` & `pyspextools-0.6.1/pyspextools/io/spo.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/io/tg.py` & `pyspextools-0.6.1/pyspextools/io/tg.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools/messages.py` & `pyspextools-0.6.1/pyspextools/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import sys
 import pyspextools
 from pyspextools.color import Colors
 
 # Set general messages for argument parsing
 docs = 'See full documentation at: https://spex-xray.github.io/pyspextools'
-version = '%(prog)s {:s} (C) 2018-2023, Jelle de Plaa, SRON Netherlands Institute for Space Research, ' \
+version = '%(prog)s {:s} (C) 2018-2024, Jelle de Plaa, SRON Netherlands Institute for Space Research, ' \
           'Apache 2.0 License'.format(pyspextools.__version__)
 
 # Initialize colors
 color = Colors()
 
 
 def set_color(setcol):
@@ -83,11 +83,11 @@
 
     :param scriptname: Name of the script being executed.
     :type scriptname: str
     """
     print("==================================")
     print(" This is {:s} version {:s}".format(scriptname, pyspextools.__version__))
     print("==================================")
-    print("(C) 2018-2023 Jelle de Plaa")
+    print("(C) 2018-2024 Jelle de Plaa")
     print("SRON Netherlands Institute for Space Research")
     print("Github: https://github.com/spex-xray/pyspextools")
     print("")
```

### Comparing `pyspextools-0.6.0/pyspextools/model/user.py` & `pyspextools-0.6.1/pyspextools/model/user.py`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/pyspextools.egg-info/PKG-INFO` & `pyspextools-0.6.1/pyspextools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspextools
-Version: 0.6.0
+Version: 0.6.1
 Summary: SPEX Python tools
 Home-page: https://github.com/spex-xray/pyspextools
 Author: SPEX development team
 Author-email: j.de.plaa@sron.nl
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: docs
```

### Comparing `pyspextools-0.6.0/pyspextools.egg-info/SOURCES.txt` & `pyspextools-0.6.1/pyspextools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/scripts/ogip2spex` & `pyspextools-0.6.1/scripts/ogip2spex`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/scripts/ogipgenrsp` & `pyspextools-0.6.1/scripts/ogipgenrsp`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/scripts/simres` & `pyspextools-0.6.1/scripts/simres`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/scripts/tg2spex` & `pyspextools-0.6.1/scripts/tg2spex`

 * *Files identical despite different names*

### Comparing `pyspextools-0.6.0/setup.py` & `pyspextools-0.6.1/setup.py`

 * *Files identical despite different names*

