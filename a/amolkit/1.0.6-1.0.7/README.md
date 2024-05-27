# Comparing `tmp/amolkit-1.0.6.tar.gz` & `tmp/amolkit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amolkit-1.0.6.tar", last modified: Tue May 14 21:12:12 2024, max compression
+gzip compressed data, was "amolkit-1.0.7.tar", last modified: Mon May 27 22:21:04 2024, max compression
```

## Comparing `amolkit-1.0.6.tar` & `amolkit-1.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-14 21:12:12.980649 amolkit-1.0.6/
--rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.6/LICENSE
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-14 21:12:12.980649 amolkit-1.0.6/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.6/README.md
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-14 21:12:12.980649 amolkit-1.0.6/amolkit/
--rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.6/amolkit/EleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.6/amolkit/__init__.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.6/amolkit/amolsystem.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3948 2024-05-06 05:25:28.000000 amolkit-1.0.6/amolkit/atom.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.6/amolkit/genic.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     2713 2024-05-14 21:06:09.000000 amolkit-1.0.6/amolkit/getEleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.6/amolkit/gethybridstate.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.6/amolkit/getring.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)      313 2023-08-10 20:56:51.000000 amolkit-1.0.6/amolkit/misc.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    23122 2024-05-14 21:04:52.000000 amolkit-1.0.6/amolkit/molecule.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    24779 2024-05-14 21:01:09.000000 amolkit-1.0.6/amolkit/molecule2.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.6/amolkit/moltransform.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.6/amolkit/parameter.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.6/amolkit/psf.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3248 2024-05-14 21:01:31.000000 amolkit-1.0.6/amolkit/stringmanip.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    17639 2024-05-14 21:01:44.000000 amolkit-1.0.6/amolkit/topology.py
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-14 21:12:12.980649 amolkit-1.0.6/amolkit.egg-info/
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)      501 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/SOURCES.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/dependency_links.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.6/amolkit.egg-info/not-zip-safe
--rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/top_level.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-05-14 21:12:12.980649 amolkit-1.0.6/setup.cfg
--rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-05-14 21:10:22.000000 amolkit-1.0.6/setup.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 22:21:04.413618 amolkit-1.0.7/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.7/LICENSE
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      356 2024-05-27 22:21:04.413618 amolkit-1.0.7/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.7/README.md
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 22:21:04.413618 amolkit-1.0.7/amolkit/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.7/amolkit/EleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.7/amolkit/__init__.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.7/amolkit/amolsystem.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3948 2024-05-06 05:25:28.000000 amolkit-1.0.7/amolkit/atom.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.7/amolkit/genic.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2713 2024-05-14 21:06:09.000000 amolkit-1.0.7/amolkit/getEleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.7/amolkit/gethybridstate.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.7/amolkit/getring.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      328 2024-05-15 19:45:36.000000 amolkit-1.0.7/amolkit/misc.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23122 2024-05-14 21:04:52.000000 amolkit-1.0.7/amolkit/molecule.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    24779 2024-05-14 21:01:09.000000 amolkit-1.0.7/amolkit/molecule2.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.7/amolkit/moltransform.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.7/amolkit/parameter.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.7/amolkit/psf.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3803 2024-05-27 22:16:52.000000 amolkit-1.0.7/amolkit/stringmanip.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23747 2024-05-27 22:19:11.000000 amolkit-1.0.7/amolkit/topology.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 22:21:04.413618 amolkit-1.0.7/amolkit.egg-info/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      356 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      501 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.7/amolkit.egg-info/not-zip-safe
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/top_level.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-05-27 22:21:04.413618 amolkit-1.0.7/setup.cfg
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-05-27 22:20:10.000000 amolkit-1.0.7/setup.py
```

### Comparing `amolkit-1.0.6/LICENSE` & `amolkit-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/EleInfo.py` & `amolkit-1.0.7/amolkit/EleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/amolsystem.py` & `amolkit-1.0.7/amolkit/amolsystem.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/atom.py` & `amolkit-1.0.7/amolkit/atom.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/genic.py` & `amolkit-1.0.7/amolkit/genic.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/getEleInfo.py` & `amolkit-1.0.7/amolkit/getEleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/gethybridstate.py` & `amolkit-1.0.7/amolkit/gethybridstate.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/getring.py` & `amolkit-1.0.7/amolkit/getring.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/molecule.py` & `amolkit-1.0.7/amolkit/molecule.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/molecule2.py` & `amolkit-1.0.7/amolkit/molecule2.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/moltransform.py` & `amolkit-1.0.7/amolkit/moltransform.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/parameter.py` & `amolkit-1.0.7/amolkit/parameter.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/psf.py` & `amolkit-1.0.7/amolkit/psf.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.6/amolkit/stringmanip.py` & `amolkit-1.0.7/amolkit/stringmanip.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-def getPenaltyfromString(comment):
+def getPenaltyfromString(comment,penaltyId="PENALTY"):
     #Penalty is in comments. Its value is usually provided after word "penalty"
     #Will be sucessful if comment is penalty x.xx or penalty= x.xx or penalty = x.xx
     penalty = None
     cmtuplist = comment.upper().split()
     cmtuplist = list(map(lambda x:x[0:7],cmtuplist))
     cmtlist = comment.split()
-    if "PENALTY" in cmtuplist:
-        penpos = cmtuplist.index("PENALTY")
+
+    if penaltyId.upper() in cmtuplist:
+        penpos = cmtuplist.index(penaltyId.upper())
         findpenalty = cmtlist[penpos:] 
+
+    try:
+        penalty = round(float(findpenalty[1]),4)
+        comment = " ".join(cmtlist[0:penpos]+cmtlist[penpos+2:])
+    except (ValueError,IndexError):
         try:
-            penalty = round(float(findpenalty[1]),4)
-            comment = " ".join(cmtlist[0:penpos]+cmtlist[penpos+2:])
+            penalty = round(float(findpenalty[2]),4)
+            comment = " ".join(cmtlist[0:penpos]+cmtlist[penpos+3:])
         except (ValueError,IndexError):
-            try:
-                penalty = round(float(findpenalty[2]),4)
-                comment = " ".join(cmtlist[0:penpos]+cmtlist[penpos+3:])
-            except (ValueError,IndexError):
-                penalty = None
+            penalty = 0.0
     return penalty,comment
 
 def removeSym(name):
     name = re.sub('[^A-Za-z0-9]+', '', name)
     name = name[0:6].strip()
     if len(name) < 4: name=name+"".join(["F"]*(4-len(name))) 
     return (name)
@@ -90,7 +92,27 @@
 
 def updateAtomNames(iatomnames):
     update_names=renumber(list(iatomnames.values()))
     for i,nam in enumerate(update_names):
         iatomnames[i+1]=nam
     return iatomnames
 
+def split_line(line, max_length=60):
+    """Splits a line into multiple lines if its length exceeds max_length, preserving continuous word."""
+
+    if len(line) <= max_length:
+        return [line]  
+
+    splitline = []
+    words = line.split()
+    current_line = ""
+
+    for word in words:
+        if len(current_line) + len(word) + 1 > max_length:  
+            splitline.append(current_line.strip())
+            current_line = word
+        else:
+            current_line += " " + word
+
+    splitline.append(current_line.strip())
+
+    return splitline
```

### Comparing `amolkit-1.0.6/amolkit/topology.py` & `amolkit-1.0.7/amolkit/topology.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 import math
 import argparse
 from collections import OrderedDict
 from amolkit import genic
 from amolkit import getEleInfo as gei 
 from amolkit.stringmanip import getPenaltyfromString
+from amolkit.stringmanip import split_line 
 
 class Topology():
     def __init__(self): 
         """
         Constructor for the Topology class.
         """
     
@@ -38,23 +39,31 @@
         topology["fftype"]             = 'additive' 
         topology["rescharge"]          = None 
         topology['ntopatoms']          = None
         topology['natoms']             = None
         topology['first_byId']         = None
         topology['last_byId']          = None
         topology['atomindex_byId']     = OrderedDict() 
-        topology['atomname_byIdx']     = OrderedDict()
         topology['atomtype_byId']      = OrderedDict()
         topology['atomcharge_byId']    = OrderedDict()
         topology['atompenalty_byId']   = OrderedDict()
         topology['atommass_byId']      = OrderedDict()
         topology['atomele_byId']       = OrderedDict()
         topology['atomalpha_byId']     = OrderedDict()
         topology['atomthole_byId']     = OrderedDict()
         topology['atomdrudetype_byId'] = OrderedDict()
+        topology['atomname_byIdx']     = OrderedDict()
+        topology['atomtype_byIdx']     = OrderedDict()
+        topology['atomcharge_byIdx']   = OrderedDict()
+        topology['atompenalty_byIdx']  = OrderedDict()
+        topology['atommass_byIdx']     = OrderedDict()
+        topology['atomele_byIdx']      = OrderedDict()
+        topology['atomalpha_byIdx']    = OrderedDict()
+        topology['atomthole_byIdx']    = OrderedDict()
+        topology['atomdrudetype_byIdx']= OrderedDict()
         topology['atomsinring']        = OrderedDict()
         topology['groups']             = []  
         topology['atomnames']          = []    
         topology['bonds']              = []
         topology['lpbonds']            = []
         topology['angles']             = []
         topology['dihedrals']          = []
@@ -110,39 +119,51 @@
                     topology['groups'].append([nat,0,0])
                     continue
                 elif ftype == "ATOM" and len(fieldup) > 3: 
                     nat = nat + 1
                     topology['atomindex_byId'][fieldup[1]] = nat
                     topology['atomname_byIdx'][nat] = fieldup[1]    # Atomname stored as in str
                     topology['atomtype_byId'][fieldup[1]] = fieldup[2]  # Atomtype capitalized before storing
+                    topology['atomtype_byIdx'][nat] = fieldup[2]  # Atomtype capitalized before storing
                     topology['atomcharge_byId'][fieldup[1]] = float(field[3])
+                    topology['atomcharge_byIdx'][nat] = float(field[3])
                     # Using atomicmass_by_atomname, but supplying atomtype
                     # Because atomicmass_by_atomtype does a fixed conversion
                     topology['atommass_byId'][fieldup[1]] = gei.atomicmass_by_atomname(field[2],bio)
+                    topology['atommass_byIdx'][nat] = gei.atomicmass_by_atomname(field[2],bio)
                     topology['atomele_byId'][fieldup[1]] = gei.atomsymbol_by_atomname(field[2],bio)
+                    topology['atomele_byIdx'][nat] = gei.atomsymbol_by_atomname(field[2],bio)
                     topology['atomcharges'].append(float(field[3]))
-                    topology['atompenalty_byId'][fieldup[1]],_ = getPenaltyfromString(comment)
+                    penalty = comment.split()[0] if comment else str(0.0)
+                    topology['atompenalty_byId'][fieldup[1]] = penalty 
+                    topology['atompenalty_byIdx'][nat] = penalty 
     
                     if topology['atomnames'] and fieldup[1] in topology['atomnames']:
                         raise ValueError("Topology contains repeated atomname %s. Unable to load."%(field[1]))
                     else:
                         topology['atomnames'].append(fieldup[1]) 
                     
                     if any(list(map(lambda x:x in fieldup, ["ALPHA","THOLE","TYPE"]))): 
                         topology['atomalpha_byId'][fieldup[1]]=None
+                        topology['atomalpha_byIdx'][nat]=None
                         topology['atomthole_byId'][fieldup[1]]=None
+                        topology['atomthole_byIdx'][nat]=None
                         topology['atomdrudetype_byId'][fieldup[1]]='DRUD'
+                        topology['atomdrudetype_byIdx'][nat]='DRUD'
                         topology["fftype"] = "drude"
     
                     if "ALPHA" in fieldup:
                         topology['atomalpha_byId'][fieldup[1]]=float(field[fieldup.index("ALPHA")+1])
+                        topology['atomalpha_byIdx'][nat]=float(field[fieldup.index("ALPHA")+1])
                     if "THOLE" in fieldup:
                         topology['atomthole_byId'][fieldup[1]]=float(field[fieldup.index("THOLE")+1])
+                        topology['atomthole_byIdx'][nat]=float(field[fieldup.index("THOLE")+1])
                     if "TYPE" in fieldup:
                         topology['atomdrudetype_byId'][fieldup[1]]=fieldup[fieldup.index("TYPE")+1]
+                        topology['atomdrudetype_byIdx'][nat]=fieldup[fieldup.index("TYPE")+1]
     
                     continue
     
                 #Bond list dictionary of each atom is populated.
                 elif ftype in ["BOND","DOUB","TRIP"] and (len(fieldup)-1) % 2 == 0:
                     for i in range(1,len(fieldup),2):
                         ba = fieldup[i].strip("+-")
@@ -326,15 +347,22 @@
             value: The value to assign to the attribute.
         """
         setattr(self, key, value)  
 
 class WriteCharmmTopology():
     @staticmethod
     def rtf_header(header):
-        text="* %s\n* Written by: amolkit\n*\n"%(header)
+        text = ""
+        if header:
+            header=split_line(header)
+            for h in header:
+                text += "* "+ h + "\n"
+        else:
+            text="* Written by: amolkit\n"
+        text += "*\n"
         return text
     
     @staticmethod
     def rtf_ioformat(extended=True):
         if extended: text="ioformat extended"
         return text
     
@@ -359,9 +387,114 @@
         return text    
     
     @staticmethod
     def rtf_comment(comment):
         return comment
     
     @staticmethod
+    def rtf_resname(resname,charge,charge_penalty=0.0,param_penalty=0.0):
+        text=f"RESI {resname:<10} {charge:>5.3f} ! param penalty= {param_penalty:>6.3f} ; charge penalty= {charge_penalty:>4.1f}"
+        return text
+    
+    @staticmethod
+    def rtf_drudeatomline(topology,name):
+        text = "ATOM {atomname:<6} {atomtype:<8} {charge:>10.3f} ALPHA {alpha:>6.4f} THOLE {thole:>6.4f} ! PENALTY {penalty:<6}".format(
+                atomname=name,
+                atomtype=topology['atomtype_byId'][name],
+                charge=topology['atomcharge_byId'][name],
+                alpha=topology['atomalpha_byId'][name],
+                thole=topology['atomthole_byId'][name],
+                penalty=topology['atompenalty_byId'][name])
+        return text
+
+    @staticmethod
+    def rtf_additiveatomline(topology,name):
+        text = "ATOM {atomname:<6} {atomtype:<8} {charge:>10.3f} ! PENALTY {penalty:<6}".format(
+               atomname=name,
+               atomtype=topology['atomtype_byId'][name],
+               charge=topology['atomcharge_byId'][name],
+               penalty=topology['atompenalty_byId'][name])
+        return text
+
+    @staticmethod
     def rtf_end():
-        return "END\n\n"
+        text = "END"
+        return text
+
+    @staticmethod
+    def rtf_bond(bt1,bt2):
+        text=f"BOND {bt1}  {bt2}"
+        return text
+        
+    @staticmethod
+    def rtf_improper(bt1,bt2,bt3,bt4): #topology):
+        text=f"IMPR {bt1}  {bt2}  {bt3}  {bt4}"
+        return text
+
+    @staticmethod
+    def rtf_allLonepairICs(topology):
+        text = ""
+        for value in topology["lpics"]:
+            if not isinstance(value, (list, tuple)) or len(value) < 3:
+                print(f"Warning: Invalid format for lone pair IC '{key}': {value}")
+                continue  
+
+            if value[0][:4] in ["RELA", "BISE"]:
+                joined_values = " ".join(str(v) for v in value[1])
+                text += f"LONE {value[0]} {joined_values} DIST {value[2][0]:>6.4f} ANGLE {value[2][1]:>7.2f} DIHE {value[2][2]:7.2f}\n"
+            elif value[0][:4] == "COLI":
+                text += f"LONE {value[0]} {value[1]} DIST {value[2][0]:>6.4f} SCAL {value[2][1]:>7.1f}\n" 
+        return text
+
+def main():
+    parser = argparse.ArgumentParser(description='Converts CHARMM Additve stream file into Drude stream file.')
+    parser.add_argument('-r','--resi', type=str,help='Provide residue name/s for which drude str has to be created.',required=True)
+    parser.add_argument('-t','--toppar', type=str,nargs='+',help='Provide file/s which contains the topology of provided residues.',required=True)
+    parser.add_argument('-p','--parfile', type=str,help='Provide file/s which contains all drude parameters.',required=True)
+    parser.add_argument('-walp','--wrtallprm', action='store_true',default=False,help='Insert this flag if you want to output all parameters')
+    parser.add_argument('-o','--outname', type=str,help='Provide desired output name of drude str file.')
+    args = parser.parse_args()
+    #print (args.wrtallprm)
+    cgenfftodrude(args.resi,args.toppar,args.parfile,args.wrtallprm,args.outname)
+
+if __name__=="__main__":
+   main()
+
+# DO NOT DELETE
+#import os,sys
+#
+#f1=sys.argv[1]
+#f2=sys.argv[2]
+#
+#dictd={}
+#with open(f1,"r") as fin:
+#    fins = fin.readlines()
+#for line in fins:
+#    field = line.split()
+#    if len(field) > 0 and field[0] == "MASS":
+#        dictd.update({field[2]:[0.0,0.0,0,0]})
+#    
+#with open(f2,"r") as fin1:
+#    fin1s = fin1.readlines()
+#for line in fin1s:
+#    field = line.split()
+#    field = list(map(lambda x:x.strip(),field))
+#    if len(field) > 0 and field[0] == "ATOM":
+#        if "ALPHA" in field:
+#            dictd[field[2]][0] = dictd[field[2]][0] + float(field[field.index("ALPHA")+1].strip("!"))
+#            dictd[field[2]][2] = dictd[field[2]][2] + 1
+#        if "THOLE" in field:
+#            dictd[field[2]][1] = dictd[field[2]][1] + float(field[field.index("THOLE")+1].strip("!")) 
+#            dictd[field[2]][3] = dictd[field[2]][3] + 1
+#           
+#for key,value in dictd.items():
+#    if value[2] != 0:
+#        dictd[key][0] = round(value[0]/value[2],4)
+#    if value[3] != 0:
+#        dictd[key][1] = round(value[1]/value[3],4)
+#    def multiple_replace(self,dict,text):
+#        regex = re.compile("(%s)" % "|".join(map(re.escape, list(dict.keys()))))
+#        return regex.sub(lambda mo: dict[mo.string[mo.start():mo.end()]], text)
+
+#
+#NONBONDED nbxmod  5 atom vatom cdiel vdistance switch vswitch - 
+#cutnb 16.0 ctofnb 12.0 ctonnb 10.0 eps 1.0 e14fac 1.0 wmin 1.5
```

### Comparing `amolkit-1.0.6/setup.py` & `amolkit-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
      with open("README.md","r") as f:
           long_description=f.read()
 except:
      long_description=""
      pass
 
 setup(name='amolkit', 
-      version='1.0.6', 
+      version='1.0.7', 
       description='Library for extracting molecule information', 
       long_description=long_description,
       url='https://github.com/anmolecule/amolkit', 
       author='Anmol Kumar', 
       author_email='anmolecule@gmail.com', 
       license='BSD 3-Clause "New" or "Revised" License',
       packages=find_packages(),
```

