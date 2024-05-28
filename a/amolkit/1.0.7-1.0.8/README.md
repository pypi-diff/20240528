# Comparing `tmp/amolkit-1.0.7.tar.gz` & `tmp/amolkit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amolkit-1.0.7.tar", last modified: Mon May 27 22:21:04 2024, max compression
+gzip compressed data, was "amolkit-1.0.8.tar", last modified: Mon May 27 23:48:13 2024, max compression
```

## Comparing `amolkit-1.0.7.tar` & `amolkit-1.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 22:21:04.413618 amolkit-1.0.7/
--rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.7/LICENSE
--rw-r--r--   0 anmol     (1000) anmol     (1000)      356 2024-05-27 22:21:04.413618 amolkit-1.0.7/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.7/README.md
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 22:21:04.413618 amolkit-1.0.7/amolkit/
--rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.7/amolkit/EleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.7/amolkit/__init__.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.7/amolkit/amolsystem.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3948 2024-05-06 05:25:28.000000 amolkit-1.0.7/amolkit/atom.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.7/amolkit/genic.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     2713 2024-05-14 21:06:09.000000 amolkit-1.0.7/amolkit/getEleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.7/amolkit/gethybridstate.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.7/amolkit/getring.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)      328 2024-05-15 19:45:36.000000 amolkit-1.0.7/amolkit/misc.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    23122 2024-05-14 21:04:52.000000 amolkit-1.0.7/amolkit/molecule.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    24779 2024-05-14 21:01:09.000000 amolkit-1.0.7/amolkit/molecule2.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.7/amolkit/moltransform.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.7/amolkit/parameter.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.7/amolkit/psf.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3803 2024-05-27 22:16:52.000000 amolkit-1.0.7/amolkit/stringmanip.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    23747 2024-05-27 22:19:11.000000 amolkit-1.0.7/amolkit/topology.py
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 22:21:04.413618 amolkit-1.0.7/amolkit.egg-info/
--rw-r--r--   0 anmol     (1000) anmol     (1000)      356 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)      501 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/SOURCES.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/dependency_links.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.7/amolkit.egg-info/not-zip-safe
--rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-05-27 22:21:04.000000 amolkit-1.0.7/amolkit.egg-info/top_level.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-05-27 22:21:04.413618 amolkit-1.0.7/setup.cfg
--rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-05-27 22:20:10.000000 amolkit-1.0.7/setup.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 23:48:13.593177 amolkit-1.0.8/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.8/LICENSE
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-27 23:48:13.593177 amolkit-1.0.8/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.8/README.md
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 23:48:13.583177 amolkit-1.0.8/amolkit/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.8/amolkit/EleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.8/amolkit/__init__.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.8/amolkit/amolsystem.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3948 2024-05-06 05:25:28.000000 amolkit-1.0.8/amolkit/atom.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.8/amolkit/genic.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2713 2024-05-14 21:06:09.000000 amolkit-1.0.8/amolkit/getEleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.8/amolkit/gethybridstate.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.8/amolkit/getring.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      328 2024-05-15 19:45:36.000000 amolkit-1.0.8/amolkit/misc.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23122 2024-05-14 21:04:52.000000 amolkit-1.0.8/amolkit/molecule.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    24779 2024-05-14 21:01:09.000000 amolkit-1.0.8/amolkit/molecule2.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.8/amolkit/moltransform.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.8/amolkit/parameter.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.8/amolkit/psf.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3803 2024-05-27 22:16:52.000000 amolkit-1.0.8/amolkit/stringmanip.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23985 2024-05-27 23:45:36.000000 amolkit-1.0.8/amolkit/topology.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 23:48:13.593177 amolkit-1.0.8/amolkit.egg-info/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      501 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.8/amolkit.egg-info/not-zip-safe
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/top_level.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-05-27 23:48:13.593177 amolkit-1.0.8/setup.cfg
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-05-27 23:48:07.000000 amolkit-1.0.8/setup.py
```

### Comparing `amolkit-1.0.7/LICENSE` & `amolkit-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/EleInfo.py` & `amolkit-1.0.8/amolkit/EleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/amolsystem.py` & `amolkit-1.0.8/amolkit/amolsystem.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/atom.py` & `amolkit-1.0.8/amolkit/atom.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/genic.py` & `amolkit-1.0.8/amolkit/genic.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/getEleInfo.py` & `amolkit-1.0.8/amolkit/getEleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/gethybridstate.py` & `amolkit-1.0.8/amolkit/gethybridstate.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/getring.py` & `amolkit-1.0.8/amolkit/getring.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/molecule.py` & `amolkit-1.0.8/amolkit/molecule.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/molecule2.py` & `amolkit-1.0.8/amolkit/molecule2.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/moltransform.py` & `amolkit-1.0.8/amolkit/moltransform.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/parameter.py` & `amolkit-1.0.8/amolkit/parameter.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/psf.py` & `amolkit-1.0.8/amolkit/psf.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/stringmanip.py` & `amolkit-1.0.8/amolkit/stringmanip.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.7/amolkit/topology.py` & `amolkit-1.0.8/amolkit/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,25 +99,25 @@
                     if found:
                         break
                     else:
                        found = False
                 elif ftype in ["RESI","PRES"] and fieldup[1] ==  topology['resname'].upper():
                     found = True
                     try:
-                        topology["rescharge"]=round(float(field[2]),3)
+                        topology["rescharge"] = round(float(field[2]),3)
                     except (ValueError,IndexError):
                         raise ValueError('Beware:: Error in detecting residue charge of '+topology['resname']+'.')
     
             if found and len(fieldup) > 0:
                 ftype = fieldup[0][0:4]
                 if ftype not in ["RING","GROU","ATOM","BOND","DOUB","TRIP","ANGL","DIHE","IMPR","DONO","ACCE","CMAP","LONE","ANIS"]: continue
                 if ftype == "RING":
                     ring=ring+1
                     #topology['atomsinring'][ring]=field[1:]
-                    topology['atomsinring'][ring]=fieldup[1:]
+                    topology['atomsinring'][ring] = fieldup[1:]
                     continue
                 elif ftype == "GROU":
                     topology['groups'].append([nat,0,0])
                     continue
                 elif ftype == "ATOM" and len(fieldup) > 3: 
                     nat = nat + 1
                     topology['atomindex_byId'][fieldup[1]] = nat
@@ -372,27 +372,35 @@
             text="read rtf card append"
         else:
             text="read rtf card"
         return text
     
     @staticmethod
     def rtf_version(version):
-        return str(version)
+        text =  str(version)
+        return text
     
     @staticmethod
     def rtf_autogenangdih(drude=True):
         if drude: 
             text = "AUTO ANGL DIHE DRUD"
         else:    
             text = "AUTO ANGL DIHE"
         return text    
     
     @staticmethod
     def rtf_comment(comment):
-        return comment
+        text = ""          
+        if comment:
+            comment = split_line(comment)
+            for h in header:
+                text += "! "+ h + "\n"
+        else:
+            text="! Written by: amolkit\n"
+        return text
     
     @staticmethod
     def rtf_resname(resname,charge,charge_penalty=0.0,param_penalty=0.0):
         text=f"RESI {resname:<10} {charge:>5.3f} ! param penalty= {param_penalty:>6.3f} ; charge penalty= {charge_penalty:>4.1f}"
         return text
     
     @staticmethod
@@ -412,19 +420,14 @@
                atomname=name,
                atomtype=topology['atomtype_byId'][name],
                charge=topology['atomcharge_byId'][name],
                penalty=topology['atompenalty_byId'][name])
         return text
 
     @staticmethod
-    def rtf_end():
-        text = "END"
-        return text
-
-    @staticmethod
     def rtf_bond(bt1,bt2):
         text=f"BOND {bt1}  {bt2}"
         return text
         
     @staticmethod
     def rtf_improper(bt1,bt2,bt3,bt4): #topology):
         text=f"IMPR {bt1}  {bt2}  {bt3}  {bt4}"
@@ -441,14 +444,20 @@
             if value[0][:4] in ["RELA", "BISE"]:
                 joined_values = " ".join(str(v) for v in value[1])
                 text += f"LONE {value[0]} {joined_values} DIST {value[2][0]:>6.4f} ANGLE {value[2][1]:>7.2f} DIHE {value[2][2]:7.2f}\n"
             elif value[0][:4] == "COLI":
                 text += f"LONE {value[0]} {value[1]} DIST {value[2][0]:>6.4f} SCAL {value[2][1]:>7.1f}\n" 
         return text
 
+    @staticmethod
+    def rtf_end():
+        text = "END"
+        return text
+
+
 def main():
     parser = argparse.ArgumentParser(description='Converts CHARMM Additve stream file into Drude stream file.')
     parser.add_argument('-r','--resi', type=str,help='Provide residue name/s for which drude str has to be created.',required=True)
     parser.add_argument('-t','--toppar', type=str,nargs='+',help='Provide file/s which contains the topology of provided residues.',required=True)
     parser.add_argument('-p','--parfile', type=str,help='Provide file/s which contains all drude parameters.',required=True)
     parser.add_argument('-walp','--wrtallprm', action='store_true',default=False,help='Insert this flag if you want to output all parameters')
     parser.add_argument('-o','--outname', type=str,help='Provide desired output name of drude str file.')
```

### Comparing `amolkit-1.0.7/setup.py` & `amolkit-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
      with open("README.md","r") as f:
           long_description=f.read()
 except:
      long_description=""
      pass
 
 setup(name='amolkit', 
-      version='1.0.7', 
+      version='1.0.8', 
       description='Library for extracting molecule information', 
       long_description=long_description,
       url='https://github.com/anmolecule/amolkit', 
       author='Anmol Kumar', 
       author_email='anmolecule@gmail.com', 
       license='BSD 3-Clause "New" or "Revised" License',
       packages=find_packages(),
```

