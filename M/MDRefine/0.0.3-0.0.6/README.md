# Comparing `tmp/MDRefine-0.0.3.tar.gz` & `tmp/mdrefine-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDRefine-0.0.3.tar", last modified: Tue May 21 13:53:57 2024, max compression
+gzip compressed data, was "mdrefine-0.0.6.tar", last modified: Tue May 28 11:46:13 2024, max compression
```

## Comparing `MDRefine-0.0.3.tar` & `mdrefine-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:53:57.195517 MDRefine-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:53:57.191517 MDRefine-0.0.3/MDRefine/
--rw-r--r--   0 runner    (1001) docker     (127)   100236 2024-05-21 13:53:01.000000 MDRefine-0.0.3/MDRefine/Functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-21 13:53:01.000000 MDRefine-0.0.3/MDRefine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 13:53:01.000000 MDRefine-0.0.3/MDRefine/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:53:57.191517 MDRefine-0.0.3/MDRefine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 13:53:57.000000 MDRefine-0.0.3/MDRefine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 13:53:57.000000 MDRefine-0.0.3/MDRefine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:53:57.000000 MDRefine-0.0.3/MDRefine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 13:53:57.000000 MDRefine-0.0.3/MDRefine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 13:53:57.000000 MDRefine-0.0.3/MDRefine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 13:53:57.195517 MDRefine-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-21 13:53:01.000000 MDRefine-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:53:57.195517 MDRefine-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-21 13:53:01.000000 MDRefine-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:53:57.191517 MDRefine-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-21 13:53:01.000000 MDRefine-0.0.3/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:46:13.245279 mdrefine-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:46:13.245279 mdrefine-0.0.6/MDRefine/
+-rw-r--r--   0 runner    (1001) docker     (127)   102748 2024-05-28 11:43:44.000000 mdrefine-0.0.6/MDRefine/Functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 11:43:44.000000 mdrefine-0.0.6/MDRefine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-28 11:43:44.000000 mdrefine-0.0.6/MDRefine/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:46:13.245279 mdrefine-0.0.6/MDRefine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-28 11:46:13.000000 mdrefine-0.0.6/MDRefine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 11:46:13.000000 mdrefine-0.0.6/MDRefine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:46:13.000000 mdrefine-0.0.6/MDRefine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 11:46:13.000000 mdrefine-0.0.6/MDRefine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 11:46:13.000000 mdrefine-0.0.6/MDRefine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-28 11:46:13.245279 mdrefine-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-28 11:43:44.000000 mdrefine-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:46:13.245279 mdrefine-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-28 11:43:44.000000 mdrefine-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:46:13.245279 mdrefine-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 11:43:44.000000 mdrefine-0.0.6/tests/test_base.py
```

### Comparing `MDRefine-0.0.3/MDRefine/Functions.py` & `mdrefine-0.0.6/MDRefine/Functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,49 @@
-""" Tools to perform reweighting by using the fully combined approach.
-    It includes also optimization of the hyperparameters through minimization of chi2 on test set. """
-
+"""
+Tools to perform reweighting using the fully combined approach.
+It also includes optimization of the hyperparameters through minimization of chi2 on test set.
+"""
 import os
 import copy
 import time
 import pandas
-# import sys
-
-from scipy.optimize import minimize
 import numpy.random as random
-
-# if_jax = int(sys.argv[1])
-# if_jax = True
-
-# ''' if if_jax, compute derivatives through autodiff (jax.grad and similar) '''
-
-# if if_jax:
-#    print("let's use JAX!")
+from scipy.optimize import minimize
 
 import jax
 import numpy  # L-BFGS-B requires numpy arrays rather than jax.numpy for the gradient of gamma_function
 import jax.numpy as np
 from jax import config
 config.update("jax_enable_x64", True)
-#   import jax.random as random
-# else:
-#     print("do not use JAX")
-
-# import numpy as np
-# import numpy.random as random
 
 # %% A. Functions to load data:
 # %% A1. check_and_skip
 
-'''
-This function (check_and_skip) modifies input data:
-- add observables computed through forward models (if any) to data.g;
-- if hasattr(data,'selected_obs'): remove non-selected observables from data.forward_qs;
-- make the stride;
-- define data[name_sys].n_frames and data[name_sys].n_experiments.
-'''
+"""
+This function **check_and_skip** is an internal tool used in **load_data** which modifies input **data**:
+- append observables computed through forward models (if any) to data.g;
+  if hasattr(data,'selected_obs'): remove non-selected observables from data.forward_qs;
+- select frames with given **stride**;
+- count n. experiments and n. frames (data[name_sys].n_frames and data[name_sys].n_experiments)
+  and check corresponding matching.
+"""
 
 
 def check_and_skip(data, *, stride=1):
 
     output_data = {}
     output_data['global'] = data['global']
 
-    system_names = data['global'].system_names  # [k for k in data.keys() if k is not 'global']
+    system_names = data['global'].system_names
 
     for name_sys in system_names:
 
         my_data = data[name_sys]
 
-        # 1. compute observables from data.forward_qs through forward model
-        # include them in data.g
+        """ 1. compute observables from data.forward_qs through forward model and include them in data.g """
 
         if hasattr(my_data, 'forward_model') and (my_data.forward_model is not None):
             if not hasattr(my_data, 'g'):
                 my_data.g = {}
 
             if hasattr(my_data, 'selected_obs'):
                 for type_name in my_data.forward_qs.keys():
@@ -67,721 +52,729 @@
             if hasattr(my_data, 'selected_obs'):
                 selected_obs = my_data.selected_obs
             else:
                 selected_obs = None
 
             out = my_data.forward_model(np.array(data['global'].forward_coeffs_0), my_data.forward_qs, selected_obs)
             if type(out) is tuple:
-                out = out[0]  # if there are derivatives, take only forward_qs values
-            
-            if not hasattr(my_data, 'g'): my_data.g = {}
+                out = out[0]
+
+            if not hasattr(my_data, 'g'):
+                my_data.g = {}
             for name in out.keys():
                 my_data.g[name] = out[name]
 
-        # 2. check match obs,forward_qs_out with g_exp
+        """ 2. check data """
 
         b = 0
 
-        if not hasattr(my_data,'g'):
+        if not hasattr(my_data, 'g'):
 
             if not hasattr(data[name_sys[:-3]], 'gexp_DDG'):
                 print('error: missing MD data for system' % name_sys)
                 b = 1
-        if b == 1: return
+        if b == 1:
+            return
 
-        # for name_sys in system_names:
-        #     if not (name_sys in data.g.keys()) and not DDGs['if_DDGs']:
-        #         print('error: missing MD data for system %s' % name_sys)
-        #         b=1
-        #     elif (name_sys in data.g.keys()) and not set(data.gexp[name_sys].keys()) == set(data.g[name_sys].keys()):
-        #         print('error: mismatch of MD data with experimental data')
-        #         print('MD data: ',set(data.g[name_sys].keys()),' experimental data: ',set(data.gexp[name_sys].keys()))
-        #         b = 1
-        # if b == 1: return
-
-        # 3. count number of systems and number of experimental data
-        # check: same number of frames for all the systems
-
-        # if not len(data.gexp) == n_systems: print('error: different number of systems for experimental values'); return data, None, None
-        # if not len(data.g) == n_systems: print('error: different number of systems for observables'); return data, None, None
-        # if not len(data.forward_qs) == n_systems: print('error: different number of systems for forward quantities'); return data, None, None
-        # if not len(data.weights) == n_systems: print('error: different number of systems for weights'); return data, None, None
-        #if (not data.f == {}) and (not len(data.f) == n_systems): print('error: different number of systems for force field terms'); return
+        """ 3. count number of systems and number of experimental data; check: same number of frames """
 
         my_data.n_experiments = {}
-    
+
         b_error = 0
 
-        if hasattr(my_data,'gexp'):
+        if hasattr(my_data, 'gexp'):
             my_data.n_experiments = {}
             for kind in my_data.gexp.keys():
                 my_data.n_experiments[kind] = np.shape(my_data.gexp[kind])[0]
-                
-            # check same number of observables as in data.gexp
 
-            if hasattr(my_data,'g'):
+            """ check same number of observables as in data.gexp """
+
+            if hasattr(my_data, 'g'):
                 for kind in my_data.g.keys():
                     if my_data.ref[kind] == '><':
                         if not np.shape(my_data.gexp[kind+' LOWER'])[0] == np.shape(my_data.g[kind])[1]:
-                            print('error: different number of observables for (system, kind) = (%s,%s)' % (name_sys,kind)); b_error=1
+                            print('error: different number of observables for (system, kind) = (%s,%s)' % (name_sys, kind))
+                            b_error = 1
                         if not np.shape(my_data.gexp[kind+' UPPER'])[0] == np.shape(my_data.g[kind])[1]:
-                            print('error: different number of observables for (system, kind) = (%s,%s)' % (name_sys,kind)); b_error=1
+                            print('error: different number of observables for (system, kind) = (%s,%s)' % (name_sys, kind))
+                            b_error = 1
                     else:
                         if not np.shape(my_data.gexp[kind])[0] == np.shape(my_data.g[kind])[1]:
-                            print('error: different number of observables for (system, kind) = (%s,%s)' % (name_sys,kind)); b_error=1
+                            print('error: different number of observables for (system, kind) = (%s,%s)' % (name_sys, kind))
+                            b_error = 1
 
-        # check number of frames
+        """ check number of frames """
 
         n_frames = np.shape(my_data.weights)[0]
 
-        if not (hasattr(my_data,'g') or hasattr(my_data,'forward_qs') or hasattr(data[name_sys[:-3]],'gexp_DDG')):
+        if not (hasattr(my_data, 'g') or hasattr(my_data, 'forward_qs') or hasattr(data[name_sys[:-3]], 'gexp_DDG')):
             print('error: missing MD data')
         else:
 
-            if hasattr(my_data,'g'):
+            if hasattr(my_data, 'g'):
                 for kind in my_data.g.keys():
-                    if not np.shape(my_data.g[kind])[0] == n_frames: 
-                        print('error: different number of frames for observable (system,kind) = (%s,%s)' % (name_sys,kind)); b_error=1
+                    if not np.shape(my_data.g[kind])[0] == n_frames:
+                        print('error: different number of frames for observable (system,kind) = (%s,%s)' % (name_sys, kind))
+                        b_error = 1
 
-            if hasattr(my_data,'forward_qs'):
+            if hasattr(my_data, 'forward_qs'):
                 for kind in my_data.forward_qs.keys():
                     if not np.shape(my_data.forward_qs[kind])[0] == n_frames:
-                        print('error: different number of frames for forward_qs (system,kind) = (%s,%s)' % (name_sys,kind)); b_error=1
+                        print('error: different number of frames for forward_qs (system,kind) = (%s,%s)' % (name_sys, kind))
+                        b_error = 1
 
-        if hasattr(my_data,'f') and not (len(my_data.f) == n_frames):
+        if hasattr(my_data, 'f') and not (len(my_data.f) == n_frames):
             print('error: different number of frames for force field terms of system %s' % name_sys)
             b_error = 1
 
-        if b_error == 1: return
+        if b_error == 1:
+            return
 
-        # 4. do you want to skip frames? select stride (stride = 1 by default)
+        """ 4. do you want to skip frames? select stride (stride = 1 by default) """
 
         if not stride == 1:
-            if hasattr(my_data,'f'): my_data.f = my_data.f[::stride]
+            if hasattr(my_data, 'f'):
+                my_data.f = my_data.f[::stride]
             my_data.weights = my_data.weights[::stride]
             my_data.weights = my_data.weights/np.sum(my_data.weights)
-        
-            if hasattr(my_data,'g'):
+
+            if hasattr(my_data, 'g'):
                 for name in my_data.g.keys():
                     my_data.g[name] = my_data.g[name][::stride]
-            
-            if hasattr(my_data,'forward_qs'):
+
+            if hasattr(my_data, 'forward_qs'):
                 for name in my_data.forward_qs.keys():
                     my_data.forward_qs[name] = my_data.forward_qs[name][::stride]
 
-        # 5. count number of frames
+        """ 5. count number of frames """
 
         my_data.n_frames = np.shape(my_data.weights)[0]
 
         output_data[name_sys] = my_data
         del my_data
 
     if hasattr(data['global'], 'cycle_names'):
         for name in data['global'].cycle_names:
             output_data[name] = data[name]
 
-    # 6. sort n_experiments: this is needed to preserve the correct order when you will deconvolve lambdas
-    #  in the end of lossf_nested
-    # BE CAREFUL: data.g are sorted differently due to forward model
-
-    # for name_sys in data.gexp.keys():
-    #     my_dict = {}
-    #     for k in data.gexp[name_sys].keys():
-    #         my_dict[k] = n_experiments[name_sys][k]
-    #     n_experiments[name_sys] = my_dict
-    # del my_dict
-    # 
-    # data.n_experiments = n_experiments
-
     return output_data
 
 # %% A2. load_data
 
-''' WARNING: jax.numpy does not have loadtxt '''
-
-def load_data(infos, *, stride = 1):
 
-    print('loading data from directory...')
-    
-    data = {}
+"""
+This function **load_data** loads data from specified directory as indicated by the user in **infos**
+to a dictionary **data** of classes, which includes data['global'] (global properties) and data[system_name];
+for alchemical calculations, there is also data[cycle_name].
+"""
+
+
+class data_global_class:
+    def __init__(self, info_global, path_directory):
+
+        self.system_names = info_global['system_names']
+
+        if 'forward_coeffs' in info_global.keys():
+            temp = pandas.read_csv(path_directory+'%s' % info_global['forward_coeffs'], index_col=0)
+            if temp.shape[0] == 1:
+                self.forward_coeffs_0 = temp.iloc[:, 0]
+            else:
+                self.forward_coeffs_0 = temp.squeeze()
 
-    system_names = infos['global']['system_names']
-    # system_names = [k for k in infos.keys() if not k == 'global']
-    # system_names = set(infos.keys())-set(['global']) ## this would sort infos.keys(), modifying its order!!
 
-    ''' original forward-model coefficients is a global data '''
+class data_class:
+    def __init__(self, info, path_directory, name_sys):
 
-    class data_global_class:
-        def __init__(self, info_global, path_directory):
+        # 0. temperature
 
-            self.system_names = info_global['system_names']
-
-            #if not all(v is None for v in types['forward_qs'].values()):
-            # if you have forward quantities, you have also forward coefficients
-            if 'forward_coeffs' in info_global.keys():
-                temp = pandas.read_csv(path_directory+'%s' % info_global['forward_coeffs'], index_col = 0)
-                if temp.shape[0] == 1: data['global'].forward_coeffs_0 = temp.iloc[:,0]
-                else: self.forward_coeffs_0 = temp.squeeze()
+        if 'temperature' in info.keys():
+            self.temperature = info['temperature']
+        else:
+            self.temperature = 1.0
 
-    path_directory = infos['global']['path_directory'] + '/'
-    data['global'] = data_global_class(infos['global'], path_directory)
+        # 1. gexp (experimental values) and names of the observables
 
-    ''' then, separately for each system: '''
+        if 'g_exp' in info.keys():
 
-    class data_class:
-        def __init__(self, info, path_directory, name_sys):
+            self.gexp = {}
+            self.names = {}
+            self.ref = {}  # if data.gexp are boundary or puntual values
 
-            # 0. temperature (for simplicity, up to now same temperature for all the systems)
+            if info['g_exp'] is None:
+                if info['DDGs']['if_DDGs'] is False:
+                    print('error, some experimental data is missing')
+            else:
+                if info['g_exp'] == []:
+                    info['g_exp'] = [f[:-4] for f in os.listdir(path_directory+'%s/g_exp' % name_sys)]
 
-            if 'temperature' in info.keys(): self.temperature = info['temperature']
-            else: self.temperature = 1.0
-
-            # 1. gexp (experimental values) and names of the observables
-        
-            if 'g_exp' in info.keys():
-
-                self.gexp = {}
-                self.names = {}
-                self.ref = {} # if data.gexp are boundary or puntual values
-                    
-                if info['g_exp'] == None:
-                    if info['DDGs']['if_DDGs'] == False: print('error, some experimental data is missing')
-                else:
-                    if info['g_exp'] == []: info['g_exp'] = [f[:-4] for f in os.listdir(path_directory+'%s/g_exp' % name_sys)] 
+                for name in info['g_exp']:
+                    if type(name) is tuple:
+                        if len(name) == 5:
+                            for i in range(2):
+                                if name[2*i+2] == '>':
+                                    s = ' LOWER'
+                                elif name[2*i+2] == '<':
+                                    s = ' UPPER'
+                                else:
+                                    print('error in the sign of gexp')
+                                    return
+
+                                if os.path.isfile(path_directory+'%s/g_exp/%s%s.npy' % (name_sys, name[0], name[2*i+1])):
+                                    self.gexp[name[0]+s] = np.load(
+                                        path_directory+'%s/g_exp/%s%s.npy' % (name_sys, name[0], name[2*i+1]))
+                                elif os.path.isfile(path_directory+'%s/g_exp/%s%s' % (name_sys, name[0], name[2*i+1])):
+                                    self.gexp[name[0]+s] = numpy.loadtxt(
+                                        path_directory+'%s/g_exp/%s%s' % (name_sys, name[0], name[2*i+1]))
+
+                            self.ref[name[0]] = '><'
+
+                        elif name[1] == '=' or name[1] == '>' or name[1] == '<':
+                            if os.path.isfile(path_directory+'%s/g_exp/%s.npy' % (name_sys, name[0])):
+                                self.gexp[name[0]] = np.load(path_directory+'%s/g_exp/%s.npy' % (name_sys, name[0]))
+                            elif os.path.isfile(path_directory+'%s/g_exp/%s' % (name_sys, name[0])):
+                                self.gexp[name[0]] = numpy.loadtxt(path_directory+'%s/g_exp/%s' % (name_sys, name[0]))
+                            self.ref[name[0]] = name[1]
 
-                    for name in info['g_exp']:
-                        if type(name) is tuple:
-                            if len(name) == 5:
-                                for i in range(2):
-                                    if name[2*i+2] == '>': s = ' LOWER'
-                                    elif name[2*i+2] == '<': s = ' UPPER'
-                                    else: print('error in the sign of gexp'); return
-                                    
-                                    try: self.gexp[name[0]+s] = np.load(path_directory+'%s/g_exp/%s%s.npy' % (name_sys,name[0],name[2*i+1]))
-                                    except: self.gexp[name[0]+s] = np.loadtxt(path_directory+'%s/g_exp/%s%s' % (name_sys,name[0],name[2*i+1]))
-                                
-                                self.ref[name[0]] = '><'
-                            # if name[1] == '><':
-                            #     data.gexp[name_sys][name[0]+' LOWER'] = np.load(path_directory+'g_exp/%s/%s.npy' % (name_sys,name[0]))[:,:2]
-                            #     data.ref[name_sys][name[0]+' LOWER'] = '>'
-                            #     data.gexp[name_sys][name[0]+' UPPER'] = np.load(path_directory+'g_exp/%s/%s.npy' % (name_sys,name[0]))[:,2:]
-                            #     data.ref[name_sys][name[0]+ ' UPPER'] = '<'
-                            # elif name[1] == '<>':
-                            #     data.gexp[name_sys][name[0]+' LOWER'] = np.load(path_directory+'g_exp/%s/%s.npy' % (name_sys,name[0]))[:,:2]
-                            #     data.ref[name_sys][name[0]+' LOWER'] = '<'
-                            #     data.gexp[name_sys][name[0]+' UPPER'] = np.load(path_directory+'g_exp/%s/%s.npy' % (name_sys,name[0]))[:,2:]
-                            #     data.ref[name_sys][name[0]+ ' UPPER'] = '>'
-                            elif name[1] == '=' or name[1] == '>' or name[1] == '<':
-                                try: self.gexp[name[0]] = np.load(path_directory+'%s/g_exp/%s.npy' % (name_sys,name[0]))
-                                except: self.gexp[name[0]] = np.loadtxt(path_directory+'%s/g_exp/%s' % (name_sys,name[0]))
-                                self.ref[name[0]] = name[1]
-                            else: print('error on specified sign of gexp'); return
                         else:
-                            try: self.gexp[name] = np.load(path_directory+'%s/g_exp/%s.npy' % (name_sys,name))
-                            except: self.gexp[name] = np.loadtxt(path_directory+'%s/g_exp/%s' % (name_sys,name))
-                            self.ref[name] = '='
-
-                        if type(name) is tuple: name = name[0]
-                        if os.path.isfile(path_directory+'%s/names/%s.npy' % (name_sys,name)):
-                            self.names[name] = np.load(path_directory+'%s/names/%s.npy' % (name_sys,name))
-                        elif os.path.isfile(path_directory+'%s/names/%s' % (name_sys,name)):
-                            self.names[name] = np.loadtxt(path_directory+'%s/names/%s' % (name_sys,name))
-
-            # 2. g (observables)
-
-            if 'obs' in info.keys():
-
-                self.g = {}
-        
-                if info['obs'] is not None:
-                    if info['obs'] == []: info['obs'] = [f[:-4] for f in os.listdir(path_directory+'%s/observables' % name_sys)]
-                    for name in info['obs']:
-                        # if name not in data.dupl[name_sys]:
-                        # data.g[name_sys][name] = np.load(path_directory+'observables/%s/%s.npy' % (name_sys,name),mmap_mode='r')
-                        # else:
-                        #     data.g[name_sys][name+'_LOWER'] = np.load(path_directory+'observables/%s/%s.npy' % (name_sys,name),mmap_mode='r')
-                        #     data.g[name_sys][name+ '_UPPER'] = np.load(path_directory+'observables/%s/%s.npy' % (name_sys,name),mmap_mode='r')
-                        try: self.g[name] = np.load(path_directory+'%s/observables/%s.npy' % (name_sys,name), mmap_mode = 'r')
-                        except: self.g[name] = np.loadtxt(path_directory+'%s/observables/%s' % (name_sys,name))
-
-            # 3. forward_qs (quantities for the forward model) and forward_model
-        
-            if 'forward_qs' in info.keys():
-            
-                self.forward_model = info['forward_model']
-            
-                self.forward_qs = {}
-                
-                for name in info['forward_qs']:
-                    if info['forward_qs'] is not None:
-                        if info['forward_qs'] == []: info['forward_qs'] = [f[:-4] for f in os.listdir(path_directory+'%s/forward_qs' % name_sys)]
-                        for name in info['forward_qs']:
-                            try: self.forward_qs[name] = np.load(path_directory+'%s/forward_qs/%s.npy' % (name_sys,name), mmap_mode = 'r')
-                            except: self.forward_qs[name] = np.loadtxt(path_directory+'%s/forward_qs/%s' % (name_sys,name))
-
-            # 4. weights (normalized)
-
-            if os.path.isfile(path_directory+'%s/weights.npy' % name_sys):
-                try: self.weights = np.load(path_directory+'%s/weights.npy' % name_sys)
-                except: self.weights = np.loadtxt(path_directory+'%s/weights' % name_sys)
+                            print('error on specified sign of gexp')
+                            return
+
+                    else:
+                        if os.path.isfile(path_directory+'%s/g_exp/%s.npy' % (name_sys, name)):
+                            self.gexp[name] = np.load(path_directory+'%s/g_exp/%s.npy' % (name_sys, name))
+                        elif os.path.isfile(path_directory+'%s/g_exp/%s' % (name_sys, name)):
+                            self.gexp[name] = numpy.loadtxt(path_directory+'%s/g_exp/%s' % (name_sys, name))
+                        self.ref[name] = '='
+
+                    if type(name) is tuple:
+                        name = name[0]
+                    if os.path.isfile(path_directory+'%s/names/%s.npy' % (name_sys, name)):
+                        self.names[name] = np.load(path_directory+'%s/names/%s.npy' % (name_sys, name))
+                    elif os.path.isfile(path_directory+'%s/names/%s' % (name_sys, name)):
+                        self.names[name] = numpy.loadtxt(path_directory+'%s/names/%s' % (name_sys, name))
+
+        # 2. g (observables)
+
+        if 'obs' in info.keys():
+
+            self.g = {}
+
+            if info['obs'] is not None:
+                if info['obs'] == []:
+                    info['obs'] = [f[:-4] for f in os.listdir(path_directory+'%s/observables' % name_sys)]
+                for name in info['obs']:
+                    if os.path.isfile(path_directory+'%s/observables/%s.npy' % (name_sys, name)):
+                        self.g[name] = np.load(path_directory+'%s/observables/%s.npy' % (name_sys, name), mmap_mode='r')
+                    elif os.path.isfile(path_directory+'%s/observables/%s' % (name_sys, name)):
+                        self.g[name] = numpy.loadtxt(path_directory+'%s/observables/%s' % (name_sys, name))
+
+        # 3. forward_qs (quantities for the forward model) and forward_model
+
+        if 'forward_qs' in info.keys():
+
+            self.forward_model = info['forward_model']
+
+            self.forward_qs = {}
+
+            for name in info['forward_qs']:
+                if info['forward_qs'] is not None:
+                    if info['forward_qs'] == []:
+                        info['forward_qs'] = [f[:-4] for f in os.listdir(path_directory+'%s/forward_qs' % name_sys)]
+                    for name in info['forward_qs']:
+                        if os.path.isfile(path_directory+'%s/forward_qs/%s.npy' % (name_sys, name)):
+                            self.forward_qs[name] = np.load(
+                                path_directory+'%s/forward_qs/%s.npy' % (name_sys, name), mmap_mode='r')
+                        elif os.path.isfile(path_directory+'%s/forward_qs/%s' % (name_sys, name)):
+                            self.forward_qs[name] = numpy.loadtxt(path_directory+'%s/forward_qs/%s' % (name_sys, name))
+
+        # 4. weights (normalized)
+
+        if os.path.isfile(path_directory+'%s/weights.npy' % name_sys):
+            self.weights = np.load(path_directory+'%s/weights.npy' % name_sys)
+        elif os.path.isfile(path_directory+'%s/weights' % name_sys):
+            self.weights = numpy.loadtxt(path_directory+'%s/weights' % name_sys)
+        else:
+            if ('obs' in info.keys()) and not (info['obs'] is None):
+                name = list(self.g.keys())[0]
+                self.weights = np.ones(len(self.g[name]))
+            elif ('forward_qs' in info.keys()) and not (info['forward_qs'] is None):
+                name = list(self.forward_qs.keys())[0]
+                self.weights = np.ones(len(self.forward_qs[info['forward_qs'][0]]))
             else:
-                if ('obs' in info.keys()) and not (info['obs'] is None):
-                    name = list(self.g.keys())[0]
-                    self.weights = np.ones(len(self.g[name]))
-                elif ('forward_qs' in info.keys()) and not (info['forward_qs'] is None):
-                    name = list(self.forward_qs.keys())[0]
-                    self.weights = np.ones(len(self.forward_qs[info['forward_qs'][0]]))
-                else: print('error: missing MD data for %s!' % name_sys)
-
-            self.weights = self.weights/np.sum(self.weights)
-
-            # 5. f (force field correction terms) and function
-
-            if ('ff_correction' in info.keys()) and (info['ff_correction'] is not None):
-            
-                self.ff_correction = info['ff_correction']
-                self.f = {}
-
-                ff_path = path_directory + '%s/ff_terms' % name_sys
-                
-                # if info['ff_terms'] is not None:
-
-                self.f = np.load(ff_path + '.npy')
-                    # ff_terms = pandas.read_csv(ff_path, memory_map = True)
-                    # cols = ff_terms.columns
-                    # lista = []
-                    
-                    # for name_ff in info['ff_terms']: # select columns (force field correction terms)
-                    #     if name_ff in cols: # if name_ff is exactly a column of data.f
-                    #         lista.append(ff_terms[name_ff])
-                    #     else: # else, sum data.f columns starting with name_ff
-                    #         filter_col = [col for col in ff_terms.columns if col.startswith(name_ff)]
-                    #         lista.append(np.sum(np.array(ff_terms[filter_col]), axis = 1))
-                    
-                    # self.f = pandas.DataFrame(data = np.array(lista).T, columns = info['ff_terms'])
-                    # self.f = np.array(lista).T
+                print('error: missing MD data for %s!' % name_sys)
+
+        self.weights = self.weights/np.sum(self.weights)
+
+        # 5. f (force field correction terms) and function
+
+        if ('ff_correction' in info.keys()) and (info['ff_correction'] is not None):
+
+            self.ff_correction = info['ff_correction']
+            ff_path = path_directory + '%s/ff_terms' % name_sys
+            self.f = np.load(ff_path + '.npy')
+
+
+class data_cycle_class:
+    def __init__(self, cycle_name, DDGs_exp, info):
+
+        self.gexp_DDG = [DDGs_exp.loc[:, cycle_name].iloc[0], DDGs_exp.loc[:, cycle_name].iloc[1]]
+
+        if 'temperature' in info.keys():
+            self.temperature = info['temperature']
+        else:
+            self.temperature = 1.0
+
+
+def load_data(infos, *, stride=1):
+
+    print('loading data from directory...')
+
+    data = {}
+
+    system_names = infos['global']['system_names']
+
+    path_directory = infos['global']['path_directory'] + '/'
+    data['global'] = data_global_class(infos['global'], path_directory)
+
+    """ then, separately for each system: """
 
     for name_sys in system_names:
         print('loading ', name_sys)
-        if name_sys in infos.keys(): info = {**infos[name_sys], **infos['global']}
-        else: info = infos['global']
+        if name_sys in infos.keys():
+            info = {**infos[name_sys], **infos['global']}
+        else:
+            info = infos['global']
         data[name_sys] = data_class(info, path_directory, name_sys)
 
-    # 6. quantities from alchemical calculations
-
-    class data_cycle_class:
-        def __init__(self, cycle_name, DDGs_exp, info):
-            
-            self.gexp_DDG = [DDGs_exp.loc[:,cycle_name].iloc[0],DDGs_exp.loc[:,cycle_name].iloc[1]]
-
-            if 'temperature' in info.keys(): self.temperature = info['temperature']
-            else: self.temperature = 1.0
-
-    #     # DeltaE
-    #     # if types['DeltaE'][name_sys] is not None:
-    #     #     data.DeltaE[name_sys] = np.load(path_directory+'DeltaE/DeltaE_%s.npy' % name_sys)
+    # quantities from alchemical calculations
 
     if 'cycle_names' in infos['global'].keys():
 
         data['global'].cycle_names = infos['global']['cycle_names']
 
-        logZs = pandas.read_csv(path_directory+'alchemical/logZs',index_col=0)
+        logZs = pandas.read_csv(path_directory+'alchemical/logZs', index_col=0)
 
         for name in infos['global']['cycle_names']:
-            for s in ['MD','MS','AD','AS']:
+            for s in ['MD', 'MS', 'AD', 'AS']:
                 key = name+'_'+s
-                if key in logZs.index: data[key].logZ = logZs.loc[key][0]
-                else: data[key].logZ = 0.0
-        
-        DDGs_exp = pandas.read_csv(path_directory+'alchemical/DDGs',index_col=0)
+                if key in logZs.index:
+                    data[key].logZ = logZs.loc[key][0]
+                else:
+                    data[key].logZ = 0.0
+
+        DDGs_exp = pandas.read_csv(path_directory+'alchemical/DDGs', index_col=0)
 
         for name in infos['global']['cycle_names']:
-            if name in infos.keys(): info = {**infos[name], **infos['global']}
-            else: info = infos['global']
+            if name in infos.keys():
+                info = {**infos[name], **infos['global']}
+            else:
+                info = infos['global']
 
             data[name] = data_cycle_class(name, DDGs_exp, info)
 
-    # 7. check and skip frames with stride
+    # check and skip frames with stride
 
-    data = check_and_skip(data, stride = stride)
+    data = check_and_skip(data, stride=stride)
 
     def tot_n_experiments(data):
         tot = 0
         for k in system_names:
-            for item in data[k].n_experiments.values(): tot += item
+            for item in data[k].n_experiments.values():
+                tot += item
         return tot
 
     data['global'].system_names = system_names
     data['global'].tot_n_experiments = tot_n_experiments
 
     if hasattr(data['global'], 'ff_correction') and (data['global'].ff_correction == 'linear'):
         list_names_ff_pars = []
         for k in data['global'].system_names:
             if hasattr(data[k], 'f'):
                 [list_names_ff_pars.append(x) for x in data[k].f.keys() if x not in list_names_ff_pars]
         data['global'].names_ff_pars = list_names_ff_pars
-    
+
     elif 'names_ff_pars' in infos['global'].keys():
         data['global'].names_ff_pars = infos['global']['names_ff_pars']
 
     print('done')
 
     return data
 
 # %% B. Functions to compute Gamma (they act on numpy arrays):
-#%% B1. compute_js
-'''
-This function (compute_js) computes the indices (cumulative sums) for lambda corresponding to different systems and
-types of observables. BE CAREFUL TO follow always the same order: let's choose it as that of data.n_experiments.
-'''
+# %% B1. compute_js
+
+
+"""
+This function **compute_js** computes the indices (cumulative sums) for lambdas corresponding to different systems and
+types of observables. BE CAREFUL TO follow always the same order: let's choose it as that of **data.n_experiments**,
+which is a dictionary n_experiments[name_sys][name].
+"""
+
 
 def compute_js(n_experiments):
 
     js = []
 
-    for i_sys,name_sys in enumerate(n_experiments.keys()):
+    for i_sys, name_sys in enumerate(n_experiments.keys()):
         js.append([])
         for name in n_experiments[name_sys].keys():
             js[i_sys].append(n_experiments[name_sys][name])
         js[i_sys] = [0] + np.cumsum(np.array(js[i_sys])).tolist()
-    
+
     js[0] = np.array(js[0])
-    
-    if len(n_experiments.keys())>1:
-        for i_sys in range(1,len(n_experiments.keys())):
+
+    if len(n_experiments.keys()) > 1:
+        for i_sys in range(1, len(n_experiments.keys())):
             js[i_sys] = np.array(js[i_sys]) + js[i_sys-1][-1]
 
     return js
 
 # %% B2. compute_new_weights
 # to reweight given original weights and correction
 
-'''
-This function (compute_new_weights) compute the new_weights as weights*exp(-correction).
-It MODIFIES input weights and correction:
+
+"""
+This function **compute_new_weights** compute the new weights as weights*exp(-correction).
+It modifies input weights and correction:
 - weights are normalized;
-- correction is shifted by correction-= shift, shift = np.min(correction).
-'''
+- correction is shifted by correction -= shift, where shift = np.min(correction).
+It returns array **new_weights** and float **logZ**.
+"""
+
+
+def compute_new_weights(weights: np.array, correction: np.array):
 
-def compute_new_weights(weights, correction):
-    
-    correction = np.array(correction)
     weights = weights/np.sum(weights)
 
-    ''' shift is such that the physical Z is = Z/np.exp(shift) '''
+    """ shift is such that the physical Z is = Z/np.exp(shift) """
     shift = np.min(correction)
     correction -= shift
-    
+
     new_weights = np.exp(-correction)*weights
 
-    # if np.isnan(newweights).any():
-    #     print('Warning: new_weights contains none')
-    #     wh = np.argwhere(np.isnan(newweights))
-    #     newweights[wh] = 0
+    if np.isnan(new_weights).any():
+        print('Error: new_weights contains None')
+        return
 
     logZ = np.log(np.sum(new_weights))-shift
     new_weights = new_weights/np.sum(new_weights)
 
     return new_weights, logZ
 
 # %% B3. gamma_function
 
-'''
-This function (gamma_function) compute gamma function and (if if_gradient) its derivatives.
-It works directly with numpy arrays, so make sure lambdas follow the same order as g, gexp
-(let's use that of data.n_experiments).
-'''
-
-def gamma_function(lambdas, g, gexp, weights, alpha, if_gradient = False):
-    
-    correction_lambdas = np.matmul(g,lambdas)
-    newweights,logZlambda = compute_new_weights(weights,correction_lambdas)
 
-    gammaf = np.matmul(lambdas,gexp[:,0]) + 1/2*alpha*np.matmul(lambdas**2,gexp[:,1]**2) + logZlambda
+"""
+This function **gamma_function** compute value of gamma function and (if if_gradient) its derivatives and av_g.
+Make sure that lambdas follow the same order as g, gexp (let's use that of data.n_experiments).
+Parameters:
+- lambdas: a 1D array of length N; lambdas[j] is lambda value for j-th observable;
+- g: a 2D array (M x N); g[i,j] is j-th observable computed in the i-th frame;
+- gexp: a 2D array (N x 2); g[j,0] is experimental value of i-th observable, g[j,1] is the associated uncertainty;
+- weights: a 1D array of length M; w[i] is weight of i-th frame (possibly non-normalized);
+- alpha: float; value of the hyper parameter;
+- if_gradient: boolean.
+Output:
+- gammaf: float value of gamma function;
+- if if_gradient:
+    - grad: a 1D array of length N; the gradient of gamma function with respect to lambdas;
+    - av_g: a 1D array of length N; average value of j-th observable (average over new_weights).
+"""
+
+
+def gamma_function(lambdas: np.array, g: np.array, gexp: np.array, weights: np.array, alpha: float, if_gradient: bool = False):
+
+    correction_lambdas = np.matmul(g, lambdas)
+    newweights, logZlambda = compute_new_weights(weights, correction_lambdas)
+
+    gammaf = np.matmul(lambdas, gexp[:, 0]) + 1/2*alpha*np.matmul(lambdas**2, gexp[:, 1]**2) + logZlambda
 
     if if_gradient:
-        av_g = np.einsum('i,ij',newweights,g)
-        grad = -(av_g-gexp[:,0]-alpha*lambdas*gexp[:,1]**2)
+        av_g = np.einsum('i,ij', newweights, g)
+        grad = -(av_g-gexp[:, 0]-alpha*lambdas*gexp[:, 1]**2)
         grad = numpy.array(grad)
         return gammaf, grad, av_g
     else:
         return gammaf
 
 # %% B4. normalize_observables
 
-''' Since experimental observables have different units, it is better to normalize them, in order that 
-    varying any lambda by a fixed value epsilon would result in comparable effects to the ensemble.
-    This could result useful in the minimization of gamma_function. '''
 
-def normalize_observables(gexp, g, weights = None):
+"""
+This function **normalize_observables** normalize g, gexp.
+Since experimental observables have different units, it is better to normalize them, in order that
+varying any lambda by a fixed value epsilon would result in comparable effects to the ensemble.
+This results to be useful in the minimization of gamma_function.
+Input values: gexp, g (dictionaries corresponding to data[name_sys].gexp and data[name_sys].g) and weights;
+weights is by default None (equal weight for each frame), otherwise a 1D array.
+Output values: norm_g, norm_gexp (normalized g and gexp), norm_gmean, norm_gstd (reference values for normalization:
+average and standard deviation).
+"""
+
+
+def normalize_observables(gexp, g, weights=None):
 
     norm_g = {}
     norm_gexp = {}
     norm_gmean = {}
     norm_gstd = {}
 
     for name in g.keys():
         if weights is None:
-            norm_gmean[name] = np.mean(g[name], axis = 0)
-            norm_gstd[name] = np.std(g[name], axis = 0)
+            norm_gmean[name] = np.mean(g[name], axis=0)
+            norm_gstd[name] = np.std(g[name], axis=0)
         else:
-            norm_gmean[name] = np.average(g[name], axis = 0, weights = weights)
-            norm_gstd[name] = np.sqrt(np.average(g[name]**2, axis = 0, weights = weights))-norm_gmean[name]**2
+            norm_gmean[name] = np.average(g[name], axis=0, weights=weights)
+            norm_gstd[name] = np.sqrt(np.average(g[name]**2, axis=0, weights=weights))-norm_gmean[name]**2
 
-        norm_gexp[name] = np.vstack([(gexp[name][:,0]-norm_gmean[name])/norm_gstd[name], gexp[name][:,1]/norm_gstd[name]]).T
+        norm_gexp[name] = np.vstack([(gexp[name][:, 0]-norm_gmean[name])/norm_gstd[name], gexp[name][:, 1]/norm_gstd[name]]).T
         norm_g[name] = (g[name]-norm_gmean[name])/norm_gstd[name]
 
     return norm_g, norm_gexp, norm_gmean, norm_gstd
 
 # %% C. Functions to compute and minimize lossf_nested:
 # %% C1. compute_ff_correction
 
-''' This functions computes the force-field correction; names_ff_pars specifies the order of parameters in array pars.
-    BE CAREFUL to correctly match force-field correction terms to corresponding force-field parameters (through names_ff_pars). '''
 
-def compute_ff_correction(ff_correction, f, pars):#, names_ff_pars):
-    
-    if ff_correction == 'linear':
+"""
+This functions **compute_ff_correction** computes the force-field correction.
+BE CAREFUL to correctly match pars with f inside user-defined **ff_correction**.
+"""
 
-        correction_ff = np.matmul(f, pars)
 
-        # correction_ff = np.zeros(len(f))
-        # indices = [names_ff_pars.index(x) for x in f.keys()]
+def compute_ff_correction(ff_correction, f, pars):
 
-        # for i in indices:
-        #     correction_ff += pars[i]*np.array(f[names_ff_pars[i]])
-            # except: correction_ff = correction_ff.add(pars[i]*f[names_ff_pars[i]])
- 
+    if ff_correction == 'linear':
+        correction_ff = np.matmul(f, pars)
     else:
-
-        correction_ff = ff_correction(pars,f)#,False)
+        correction_ff = ff_correction(pars, f)
 
     return correction_ff
 
 # %% C2. compute_D_KL
 
-''' This function computes Kullback-Leibler divergence. '''
 
-def compute_D_KL(weights_P, correction_ff, temperature, logZ_P):#, derivatives_ff = None, *, weighted_forces = None, av_forces = None):
+"""
+This function **compute_D_KL** computes Kullback-Leibler divergence of P(x) = 1/Z P_0 (x) e^(-V(x)/T)
+w.r.t. P_0 (x), which results equal to <V>_P / T + log Z.
+Input values:
+- weights_P: 1D array for P(x);
+- correction_ff: 1D array for V(x);
+- temperature: float for T;
+- logZ_P: float for log Z.
+"""
 
-    weighted_ff = weights_P*np.array(correction_ff)
-    av_ff = np.nansum(weighted_ff,axis=0)
-    # av_ff = np.sum(weights_P[i_sys]*np.log(weights_P[i_sys]/data.weights[i_sys]))
-
-    D_KL = -(av_ff/temperature + logZ_P)
 
-    # if derivatives_ff is not None:
-    #     # if name_sys in derivatives_ff.keys():
-    #     weighted_forces = weights_P[:,None]*np.array(derivatives_ff).T
-    #     av_forces = np.sum(weighted_forces,axis=0)
+def compute_D_KL(weights_P: np.array, correction_ff: np.array, temperature: float, logZ_P: float):
 
-    #     #dav_f=-np.matmul(np.transpose(weighted_f),np.array(data.f[i_sys]))+np.outer(av_f,av_f)
-    #     derivative = (np.matmul(weighted_ff,np.array(derivatives_ff).T)-av_ff*av_forces)/temperature**2
+    weighted_ff = weights_P*np.array(correction_ff)
+    av_ff = np.nansum(weighted_ff, axis=0)
+    D_KL = -(av_ff/temperature + logZ_P)
 
-    #     return D_KL, derivative
-    
     return D_KL
 
 # %% C3. l2_regularization
 
-''' This function computes the l2 regularization specified by choice, which includes:
-    - 'plain l2' (plain l2 regularization);
-    - for alchemical calculations with charges, pars[:-1] are the charges and pars[-1] is V_eta,
-      you have constraint on charges, and there are 3 pars[4] charges:
-        - 'constraint 1';
-        - 'constraint 2' (with l2 regularization also on V_eta). '''
 
-def l2_regularization(pars, choice = 'plain l2'):
+"""
+This function **l2_regularization** computes the l2 regularization specified by **choice**, which includes:
+- 'plain l2' (plain l2 regularization);
+- ad-hoc regularization for alchemical calculations with charges (as described by Valerio Piomponi et al.):
+  pars[:-1] are the charges and pars[-1] is V_eta, you have constraint on charges, and there are 3 pars[4] charges;
+    - 'constraint 1';
+    - 'constraint 2' (with l2 regularization also on V_eta).
+Output values: lossf_reg and gradient.
+"""
+
+
+def l2_regularization(pars: np.array, choice: str = 'plain l2'):
 
     lossf_reg = None
     gradient = None
-    
+
     if choice == 'plain l2':
         lossf_reg = np.sum(pars**2)
         gradient = 2*pars
-        map = np.arange(len(pars))
 
     elif choice == 'constraint 1':
         lossf_reg = np.sum(pars[:-1]**2)+(np.sum(pars[:-1])+2*pars[4])**2
-        n = np.array([1,1,1,1,3])
+        n = np.array([1, 1, 1, 1, 3])
         gradient = 2*(pars[:-1]+(np.sum(pars[:-1])+2*pars[4])*n)
 
-        map = np.arange(len(pars)-1)
-
     elif choice == 'constraint 2':
         lossf_reg = np.sum(pars**2)+(np.sum(pars[:-1])+2*pars[4])**2
-        n = np.array([1,1,1,1,3,0])
+        n = np.array([1, 1, 1, 1, 3, 0])
         gradient = 2*(pars+(np.sum(pars[:-1])+2*pars[4])*n)
 
-        map = np.arange(len(pars))
-    
-    return lossf_reg, gradient, map
-
+    return lossf_reg, gradient
 
 # %% C4. compute_chi2
 
-''' This function computes the chi2 (for a given system). It returns: av_g (average values),
-    rel_diffs (relative differences), chi2 (for each kind of observable), tot_chi2 (total chi2 for that system).
-    If if_separate, you are distinguishing between LOWER and UPPER bounds, needed for minimizations with double bounds. '''
 
-def compute_chi2(ref, weights, g, gexp, if_separate = False):
+"""
+This function **compute_chi2** computes the chi2 (for a given system).
+Input values:
+- ref (dict for references: '=', '>', '<', '><');
+- weights (1D np.array);
+- g (dict for observables);
+- gexp (dict for experimental values);
+- if_separate (boolean, True if you are distinguishing between LOWER and UPPER bounds (name_type + ' LOWER' or
+    name_type + ' UPPER'), needed for minimizations with double bounds.)
+It returns 3 dicts with keys running over different kinds of observables and 1 float:
+- av_g (dict for average values);
+- chi2 (dict for chi2);
+- rel_diffs (dict for relative differences);
+- tot_chi2 (total chi2 for the given system).
+"""
+
+
+def compute_chi2(ref, weights, g, gexp, if_separate=False):
 
     av_g = {}
     rel_diffs = {}
     chi2 = {}
     tot_chi2 = 0
 
     for name_type in gexp.keys():
 
         if ref[name_type] == '><':
             # av_g UPPER is equal to av_g LOWER but (if if_separate) you have to distinguish them
             if if_separate:
-                av_g[name_type+' LOWER'] = np.einsum('i,ij',weights,g[name_type+' LOWER'])
+                av_g[name_type+' LOWER'] = np.einsum('i,ij', weights, g[name_type+' LOWER'])
                 av_g[name_type+' UPPER'] = av_g[name_type+' LOWER']
 
-                rel_diffs[name_type+' UPPER'] = np.maximum(av_g[name_type+' UPPER']-gexp[name_type+' UPPER'][:,0],np.zeros(len(av_g[name_type+' UPPER'])))/gexp[name_type+' UPPER'][:,1]
-                rel_diffs[name_type+' LOWER'] = np.minimum(av_g[name_type+' LOWER']-gexp[name_type+' LOWER'][:,0],np.zeros(len(av_g[name_type+' LOWER'])))/gexp[name_type+' LOWER'][:,1]
+                rel_diffs[name_type+' UPPER'] = np.maximum(
+                    av_g[name_type+' UPPER']-gexp[name_type+' UPPER'][:, 0],
+                    np.zeros(len(av_g[name_type+' UPPER'])))/gexp[name_type+' UPPER'][:, 1]
+                rel_diffs[name_type+' LOWER'] = np.minimum(
+                    av_g[name_type+' LOWER']-gexp[name_type+' LOWER'][:, 0],
+                    np.zeros(len(av_g[name_type+' LOWER'])))/gexp[name_type+' LOWER'][:, 1]
 
             else:
-                av_g[name_type] = np.einsum('i,ij',weights,g[name_type])
-                
-                rel_diffs[name_type+' UPPER'] = np.maximum(av_g[name_type]-gexp[name_type+' UPPER'][:,0],np.zeros(len(av_g[name_type])))/gexp[name_type+' UPPER'][:,1]
-                rel_diffs[name_type+' LOWER'] = np.minimum(av_g[name_type]-gexp[name_type+' LOWER'][:,0],np.zeros(len(av_g[name_type])))/gexp[name_type+' LOWER'][:,1]
+                av_g[name_type] = np.einsum('i,ij', weights, g[name_type])
+
+                rel_diffs[name_type+' UPPER'] = np.maximum(
+                    av_g[name_type]-gexp[name_type+' UPPER'][:, 0],
+                    np.zeros(len(av_g[name_type])))/gexp[name_type+' UPPER'][:, 1]
+                rel_diffs[name_type+' LOWER'] = np.minimum(
+                    av_g[name_type]-gexp[name_type+' LOWER'][:, 0],
+                    np.zeros(len(av_g[name_type])))/gexp[name_type+' LOWER'][:, 1]
 
                 # either one of the two is zero and the other non-zero
                 rel_diffs[name_type] = rel_diffs[name_type+' LOWER']+rel_diffs[name_type+' UPPER']
                 del rel_diffs[name_type+' LOWER'], rel_diffs[name_type+' UPPER']
 
         elif ref[name_type] == '=':
-            av_g[name_type] = np.einsum('i,ij',weights,g[name_type])
-            rel_diffs[name_type] = (av_g[name_type]-gexp[name_type][:,0])/gexp[name_type][:,1]
-        
+            av_g[name_type] = np.einsum('i,ij', weights, g[name_type])
+            rel_diffs[name_type] = (av_g[name_type]-gexp[name_type][:, 0])/gexp[name_type][:, 1]
+
         elif ref[name_type] == '<':
-            av_g[name_type] = np.einsum('i,ij',weights,g[name_type])
-            rel_diffs[name_type] = np.maximum(av_g[name_type]-gexp[name_type][:,0],np.zeros(len(av_g[name_type])))/gexp[name_type][:,1]
-        
+            av_g[name_type] = np.einsum('i,ij', weights, g[name_type])
+            rel_diffs[name_type] = np.maximum(
+                av_g[name_type]-gexp[name_type][:, 0], np.zeros(len(av_g[name_type])))/gexp[name_type][:, 1]
+
         elif ref[name_type] == '>':
-            av_g[name_type] = np.einsum('i,ij',weights,g[name_type])
-            rel_diffs[name_type] = np.minimum(av_g[name_type]-gexp[name_type][:,0],np.zeros(len(av_g[name_type])))/gexp[name_type][:,1]
+            av_g[name_type] = np.einsum('i,ij', weights, g[name_type])
+            rel_diffs[name_type] = np.minimum(
+                av_g[name_type]-gexp[name_type][:, 0], np.zeros(len(av_g[name_type])))/gexp[name_type][:, 1]
 
         else:
             print('error')
 
     for k in rel_diffs.keys():
         chi2[k] = np.sum(rel_diffs[k]**2)
         tot_chi2 += chi2[k]
 
     return av_g, chi2, rel_diffs, tot_chi2
 
 # %% C5. compute_DeltaDeltaG_terms
 
-''' data['global'] has attributes: cycle_names (list of cycle names);
-    for s in cycle_names: data[s] has attributes temperature of the cycle, gexp_DDG;
-    for s in cycle_names: data[s+k] for k in '_MD', '_MS', '_AD', '_AS' '''
-
-def compute_DeltaDeltaG_terms(data, logZ_P):#,weights_P,if_gradient=False,derivatives_ff=None,map_ff=None,nffs=None):
-    
-    cycle_names = data['global'].cycle_names#list(data.gexp_DDG.keys())
+
+"""
+This function **compute_DeltaDeltaG_terms** computes contribution from alchemical data about Delta Delta G
+to the loss function.
+Input values: **data** (full data dict of classes), **logZ_P** (dictionary);
+- data['global'] has attributes: cycle_names (list of cycle names);
+- for s in cycle_names: data[s] has attributes temperature (of the cycle), gexp_DDG;
+- for s in cycle_names: data[s+k] for k in '_MD', '_MS', '_AD', '_AS' has attributes temperature, logZ.
+Output values: new_av_DG (dict of reweighted averages of Delta G); chi2 (dict of contributions to chi2);
+loss (total contribution to the loss function from alchemical transformations).
+"""
+
+
+def compute_DeltaDeltaG_terms(data, logZ_P):
+
+    cycle_names = data['global'].cycle_names
 
     new_av_DG = {}
     chi2 = {}
     loss = 0
-    # if if_gradient: gradient = np.zeros(nffs)
 
     for cycle_name in cycle_names:
-        for s in ['_MD','_MS','_AD','_AS']:
-            if (cycle_name+s in logZ_P.keys()) and (not logZ_P[cycle_name+s] == 0):# and cycle_name+s in data.logZ.keys():
+        for s in ['_MD', '_MS', '_AD', '_AS']:
+            if (cycle_name+s in logZ_P.keys()) and (not logZ_P[cycle_name+s] == 0):
                 # correction only on MD
                 new_av_DG[cycle_name+s] = -data[cycle_name+s].temperature*(logZ_P[cycle_name+s]+data[cycle_name+s].logZ)
-            if cycle_name+s not in logZ_P: logZ_P[cycle_name+s] = 0
+            if cycle_name+s not in logZ_P:
+                logZ_P[cycle_name+s] = 0
 
-        DeltaDeltaG = -(logZ_P[cycle_name+'_MD']+data[cycle_name+'_MD'].logZ-logZ_P[cycle_name+'_AD']-data[cycle_name+'_AD'].logZ)
-        DeltaDeltaG += logZ_P[cycle_name+'_MS']+data[cycle_name+'_MS'].logZ-logZ_P[cycle_name+'_AS']-data[cycle_name+'_AS'].logZ
-        DeltaDeltaG = DeltaDeltaG*data[cycle_name].temperature
- 
-        chi2[cycle_name] = ((DeltaDeltaG - data[cycle_name].gexp_DDG[0])/data[cycle_name].gexp_DDG[1])**2
-        loss += 1/2*chi2[cycle_name]
+        DeltaDeltaG = -(
+            logZ_P[cycle_name+'_MD'] + data[cycle_name+'_MD'].logZ
+            - logZ_P[cycle_name+'_AD'] - data[cycle_name+'_AD'].logZ)
 
-    #     if if_gradient:
+        DeltaDeltaG += logZ_P[cycle_name+'_MS'] + data[cycle_name+'_MS'].logZ
+        - logZ_P[cycle_name+'_AS'] - data[cycle_name+'_AS'].logZ
 
-    #         vec = (DeltaDeltaG-data.gexp_DDG[cycle_name][0])/(data.gexp_DDG[cycle_name][1]**2)
+        DeltaDeltaG = DeltaDeltaG*data[cycle_name].temperature
 
-    #         s = cycle_name+'_MS' # minus
-    #         if s in derivatives_ff.keys():
-    #             if s in weights_P.keys(): w = weights_P[s]
-    #             else: w = data.weights[s]
-
-    #             av = np.matmul(w,derivatives_ff[s].T)
-    #             try: gradient[map_ff[s]]-= vec*av
-    #             except: gradient = gradient.at[np.array(map_ff[s])].add(-vec*av)
-
-    #         s = cycle_name+'_MD' # plus
-    #         if s in derivatives_ff.keys():
-    #             if s in weights_P.keys(): w = weights_P[s]
-    #             else: w = data.weights[s]
-
-    #             av = np.matmul(w,derivatives_ff[s].T)
-    #             try: gradient[map_ff[s]]+= vec*av
-    #             except: gradient = gradient.at[np.array(map_ff[s])].add(vec*av)
-
-    #         s = cycle_name+'_AS' # plus
-    #         if s in derivatives_ff.keys():
-    #             if s in weights_P.keys(): w = weights_P[s]
-    #             else: w = data.weights[s]
-
-    #             av = np.matmul(weights_P[s],derivatives_ff[s].T)
-    #             try: gradient[map_ff[s]]+= vec*av
-    #             except: gradient = gradient.at[np.array(map_ff[s])].add(vec*av)
-
-    #         s = cycle_name+'_AD' # minus
-    #         if s in derivatives_ff.keys():
-    #             if s in weights_P.keys(): w = weights_P[s]
-    #             else: w = data.weights[s]
-
-    #             av = np.matmul(weights_P[s],derivatives_ff[s].T)
-    #             try: gradient[map_ff[s]]-= vec*av
-    #             except: gradient = gradient.at[np.array(map_ff[s])].add(-vec*av)
+        chi2[cycle_name] = ((DeltaDeltaG - data[cycle_name].gexp_DDG[0])/data[cycle_name].gexp_DDG[1])**2
+        loss += 1/2*chi2[cycle_name]
 
-    # if if_gradient:
-    #     return loss,gradient,new_av_DG
     return new_av_DG, chi2, loss
 
 # %% C6. compute_details_ER
 
-''' This function computes the contribution to the loss function due to Ensemble Refinement explicitely 
-    (namely, 1/2*chi2 + alpha*D_KL) and compare this value with -alpha*Gamma, which must be equal (used to check). 
-    Its inputs are: the weights on which Ensemble Refinement acts (weights_P, those with force-field correction
-    in the fully combined refinement); the observables g (with updated forward-model coefficients); original data; 
-    lambdas; alpha. It cycles over different systems.
-    It is used to get detailed values in the end of the minimization of loss_function (not for the minimization itself,
-    since we exploit the Gamma function).
-    Be careful to use either: normalized values for lambdas and g (if hasattr(data,'normg_mean')) or non-normalized
-    (if not hasattr(data,'normg_mean')). '''
+
+"""
+This function **compute_details_ER** computes the contribution to the loss function due to Ensemble Refinement
+explicitely (namely, 1/2*chi2 + alpha*D_KL) and compare this value with -alpha*Gamma (they must be equal: check).
+It cycles over different systems. It acts in the end of the minimization of loss_function (not for the minimization
+itself, since we exploit the Gamma function).
+Be careful to use either: normalized values for lambdas and g (if hasattr(data,'normg_mean')) or non-normalized
+(if not hasattr(data,'normg_mean')).
+Inputs:
+- weights_P (dict of np.arrays): the weights on which Ensemble Refinement acts (those with force-field correction
+    in the fully combined refinement);
+- g (dict of dicts): the observables (with updated forward-model coefficients);
+- data (dict of classes): the original data;
+- lambdas (dict of np.arrays): the coefficients for Ensemble Refinement;
+- alpha (float): the hyper-parameter for Ensemble Refinement.
+Output: instance of Details_class.
+"""
+
 
 def compute_details_ER(weights_P, g, data, lambdas, alpha):
 
     if hasattr(data, 'normg_mean'):
         print('WARNING: you are using normalized observables!')
-    #     return
-    #     if_normalized = True
-    # else: if_normalized = False
-    
+
     class Details_class:
         def __init__(self):
-            self.loss_explicit = 0 # loss function computed explicitly as 1/2*chi2 + alpha*D_KL (rather than with Gamma function)
+            self.loss_explicit = 0
+            # loss_explicit is loss function computed explicitly as 1/2*chi2 + alpha*D_KL (rather than with Gamma function)
             self.weights_new = {}
             self.logZ_new = {}
             self.av_g = {}
             self.chi2 = {}
             self.D_KL_alpha = {}
             self.abs_difference = {}
 
     Details = Details_class()
 
-    system_names = data['global'].system_names#[k for k in data.keys() if k is not 'global']
+    system_names = data['global'].system_names
 
     for name_sys in system_names:
 
         flatten_g = np.hstack([g[name_sys][k] for k in data[name_sys].n_experiments.keys()])
         flatten_gexp = np.vstack([data[name_sys].gexp[k] for k in data[name_sys].n_experiments.keys()])
         correction = np.einsum('ij,j', flatten_g, lambdas[name_sys])
 
@@ -789,484 +782,585 @@
         Details.weights_new[name_sys] = out[0]
         Details.logZ_new[name_sys] = out[1]
 
         out = compute_chi2(data[name_sys].ref, Details.weights_new[name_sys], g[name_sys], data[name_sys].gexp)
         Details.av_g[name_sys] = out[0]
         Details.chi2[name_sys] = out[1]
         loss1 = 1/2*out[3]
-        
+
         Details.D_KL_alpha[name_sys] = compute_D_KL(Details.weights_new[name_sys], correction, 1, Details.logZ_new[name_sys])
         loss1 += alpha*Details.D_KL_alpha[name_sys]
         Details.loss_explicit += loss1
 
-        ''' You could also use lambdas to evaluate immediately chi2 and D_KL (if lambdas are determined from the given frames) '''
+        """ You could also use lambdas to evaluate immediately chi2 and D_KL
+        (if lambdas are determined from the given frames) """
         loss2 = -alpha*gamma_function(lambdas[name_sys], flatten_g, flatten_gexp, weights_P[name_sys], alpha)
 
         Details.abs_difference[name_sys] = np.abs(loss2-loss1)
-        
+
     return Details
 
 # %% C7. loss_function
 
-''' This function computes the fully-combined loss function to minimize, taking advantage of the inner minimization
-    with Gamma function.
-    If not np.isinf(alpha): if fixed_lambdas == None, then do the inner minimization of Gamma (in this case, you have
-    global variable lambdas, corresponding to starting point of the minimization; it is a numpy array sorted correctly - see below);
-    else lambdas is fixed (fixed_lambdas) and the Gamma function is evaluated at this value of lambda, which should
+
+"""
+This function **loss_function** computes the fully-combined loss function (to minimize),
+taking advantage of the inner minimization with Gamma function.
+
+--------------------------------------------------------------------------------------------------------------
+Input parameters:
+- pars_ff_fm: 1D np.array with parameters for force-field corrections and/or forward models;
+- data: dict of classes as organised in load_data (see above);
+- regularization: dict which can include
+    - 'force_field_reg' key: it can be a string (among 'plain l2', 'constraint 1', 'constraint 2', 'KL divergence')
+      or a user-defined function which takes as input pars_ff and returns regularization term to be multiplied by beta;
+    - 'forward_model_reg' key: a user-defined function which takes as input pars_fm and forward_coeffs_0
+      (current and reference forward-model coefficients) and returns regularization term to be multiplied by gamma;
+- alpha, beta, gamma: floats corresponding to hyperparameters of combined refinement
+  (respectively to: the ensemble, the force-field, the forward-model)
+  (np.inf by default, namely no refinement in that direction);
+- fixed_lambdas: np.array of lambdas (read below) (None by default);
+- gtol_inn: float (gtol for the inner minimization of gamma functions) (1e-3 by default);
+- if_save: bool (read below) (False by default);
+- bounds: dict of boundaries for the inner minimization (None by default).
+
+--------------------------------------------------------------------------------------------------------------
+Notes on using loss_function
+
+If not np.isinf(alpha):
+- if fixed_lambdas == None, then do the inner minimization of Gamma (in this case, you have global variable lambdas,
+    corresponding to starting point of the minimization; it is a numpy array correctly sorted - see below);
+- else: lambdas is fixed (fixed_lambdas) and the Gamma function is evaluated at this value of lambda, which must
     correspond to its point of minimum, otherwise mismatch between Gamma function and Ensemble Refinement loss).
-    If if_save: you are going to save the detailed results in the class Details.
-    The input data will not be modified by the loss_function (neither explicitely by loss_function
-    nor by inner functions: BE SURE of that if you are going to modify loss_function): for forward-model updating, 
-    you are going to define a variable g (through copy.deepcopy).
-    The order followed for lambdas is the one of data.n_experiments, which is not modified in any step.
-    The order followed for pars_ff_fm is: first force-field correction (ff), then forward model (fm); order for ff _ff: 
+
+If if_save: it will return Details class with the detailed results; otherwise, it will return loss value.
+
+The input data will not be modified by the loss_function (neither explicitely by loss_function nor by inner functions:
+BE SURE of that if you are going to modify loss_function):
+for forward-model updating, you are going to define a variable g (through copy.deepcopy).
+
+The order followed for lambdas is the one of data.n_experiments, which is not modified in any step.
+The order followed for pars_ff_fm is: first force-field correction (ff), then forward model (fm);
+order for ff _ff:
     names_ff_pars = []
     for k in system_names: [names_ff_pars.append(x) for x in data[k].f.keys() if x not in names_ff_pars];
-    order for par_fm: data.forward_coeffs_0. '''
+order for par_fm: data.forward_coeffs_0.
+"""
+
+
+def loss_function(
+    pars_ff_fm: np.array, data: dict, regularization: dict, alpha: float = np.inf, beta: float = np.inf, gamma: float = np.inf,
+        fixed_lambdas: np.array = None, gtol_inn: float = 1e-3, if_save: bool = False, bounds: dict = None):
 
-def loss_function(pars_ff_fm, data, regularization, alpha = np.inf, beta = np.inf, gamma = np.inf, fixed_lambdas = None, gtol_inn = 1e-3, if_save = False, method = 'BFGS', bounds = None):
-    
-    system_names = data['global'].system_names#[k for k in data.keys() if k is not 'global']
+    system_names = data['global'].system_names
 
-    if_fixed_lambdas = None # to avoid error in Pylint
+    if_fixed_lambdas = None  # to avoid error in Pylint
     if not np.isinf(alpha):
         if (fixed_lambdas is None):
             global lambdas
             if_fixed_lambdas = False
             if 'lambdas' not in globals():
                 lambdas = np.zeros(data['global'].tot_n_experiments(data))
         else:
             lambdas = fixed_lambdas
             if_fixed_lambdas = True
 
     if not np.isinf(beta):
         names_ff_pars = data['global'].names_ff_pars
         pars_ff = pars_ff_fm[:len(names_ff_pars)]
-    
-    pars_fm = None # to avoid error in Pylint
+
+    pars_fm = None  # to avoid error in Pylint
     if not np.isinf(gamma):
-        if np.isinf(beta): pars_fm = pars_ff_fm
-        else: pars_fm = pars_ff_fm[len(names_ff_pars):]
-    # if names_ff_pars == []: del names_ff_pars
+        if np.isinf(beta):
+            pars_fm = pars_ff_fm
+        else:
+            pars_fm = pars_ff_fm[len(names_ff_pars):]
 
     loss = 0
 
     weights_P = {}
 
     if not np.isinf(beta):
-        
+
         correction_ff = {}
         logZ_P = {}
-    
+
     g = {}
-    
+
     for name_sys in system_names:
 
-        ''' 1a. compute force-field corrections and corresponding re-weights '''
+        """ 1a. compute force-field corrections and corresponding re-weights """
 
         if not np.isinf(beta):
             if hasattr(data[name_sys], 'ff_correction'):
-                correction_ff[name_sys] = compute_ff_correction(data[name_sys].ff_correction, data[name_sys].f, pars_ff)#, names_ff_pars)
-                weights_P[name_sys], logZ_P[name_sys] = compute_new_weights(data[name_sys].weights, correction_ff[name_sys]/data[name_sys].temperature)
-            
-            else: # if beta is not infinite, but there are systems without force-field corrections:
+                correction_ff[name_sys] = compute_ff_correction(data[name_sys].ff_correction, data[name_sys].f, pars_ff)
+                weights_P[name_sys], logZ_P[name_sys] = compute_new_weights(
+                    data[name_sys].weights, correction_ff[name_sys]/data[name_sys].temperature)
+
+            else:  # if beta is not infinite, but there are systems without force-field corrections:
                 weights_P[name_sys] = data[name_sys].weights
                 logZ_P[name_sys] = 0
         else:
             weights_P[name_sys] = data[name_sys].weights
 
-        ''' 1b. if np.isinf(gamma): g is re-computed observables data.g through updated forward model
+        """ 1b. if np.isinf(gamma): g is re-computed observables data.g through updated forward model
             (notice you also have some observables directly as data.g without updating of forward model);
-            else: g is data.g (initial data.g[name_sys] if gamma == np.inf). '''
+            else: g is data.g (initial data.g[name_sys] if gamma == np.inf). """
 
         if np.isinf(gamma):
-            if hasattr(data[name_sys], 'g'): g[name_sys] = copy.deepcopy(data[name_sys].g)
+            if hasattr(data[name_sys], 'g'):
+                g[name_sys] = copy.deepcopy(data[name_sys].g)
         else:
-    
-            if hasattr(data[name_sys], 'g'): g[name_sys] = copy.deepcopy(data[name_sys].g)
-            else: g[name_sys] = {}
 
-            if hasattr(data[name_sys], 'selected_obs'): selected_obs = data[name_sys].selected_obs
-            else: selected_obs = None
+            if hasattr(data[name_sys], 'g'):
+                g[name_sys] = copy.deepcopy(data[name_sys].g)
+            else:
+                g[name_sys] = {}
+
+            if hasattr(data[name_sys], 'selected_obs'):
+                selected_obs = data[name_sys].selected_obs
+            else:
+                selected_obs = None
 
             fm_observables = data[name_sys].forward_model(pars_fm, data[name_sys].forward_qs, selected_obs)
 
             for name in fm_observables.keys():
-                
+
                 g[name_sys][name] = fm_observables[name]
-                if hasattr(data[name_sys], 'normg_mean'): g[name_sys][name] = (g[name_sys][name]-data[name_sys].normg_mean[name])/data[name_sys].normg_std[name]
+                if hasattr(data[name_sys], 'normg_mean'):
+                    g[name_sys][name] = (g[name_sys][name]-data[name_sys].normg_mean[name])/data[name_sys].normg_std[name]
 
             del fm_observables
 
         if (np.isinf(gamma) and hasattr(data[name_sys], 'g')) or not np.isinf(gamma):
             for name in data[name_sys].ref.keys():
                 if data[name_sys].ref[name] == '><':
                     g[name_sys][name+' LOWER'] = g[name_sys][name]
                     g[name_sys][name+' UPPER'] = g[name_sys][name]
                     del g[name_sys][name]
 
-    ''' 2. compute chi2 (if np.isinf(alpha)) or Gamma function (otherwise) '''
+    """ 2. compute chi2 (if np.isinf(alpha)) or Gamma function (otherwise) """
 
     if np.isinf(alpha):
 
         av_g = {}
         chi2 = {}
-        
+
         if hasattr(data['global'], 'cycle_names'):
             out = compute_DeltaDeltaG_terms(data, logZ_P)
             av_g = out[0]
             chi2 = out[1]
             loss += out[2]
 
         for name_sys in system_names:
-            if hasattr(data[name_sys],'g'):
+            if hasattr(data[name_sys], 'g'):
                 out = compute_chi2(data[name_sys].ref, weights_P[name_sys], g[name_sys], data[name_sys].gexp, True)
                 av_g[name_sys] = out[0]
                 chi2[name_sys] = out[1]
                 loss += 1/2*out[3]
 
     else:
-        
+
         my_dict = {}
-        for k in system_names: my_dict[k] = data[k].n_experiments
+        for k in system_names:
+            my_dict[k] = data[k].n_experiments
         js = compute_js(my_dict)
-        
+
         x0 = {}
         flatten_g = {}
         flatten_gexp = {}
 
-        for i_sys,name_sys in enumerate(system_names):
+        for i_sys, name_sys in enumerate(system_names):
 
             x0[name_sys] = np.array(lambdas[js[i_sys][0]:js[i_sys][-1]])
-            # x0 = np.concatenate([lambdas[name_sys][k] for k in data.n_experiments[name_sys].keys()])
             flatten_g[name_sys] = np.hstack([g[name_sys][k] for k in data[name_sys].n_experiments.keys()])
             flatten_gexp[name_sys] = np.vstack([data[name_sys].gexp[k] for k in data[name_sys].n_experiments.keys()])
-            # normg_std = np.hstack([data.normg_std[name_sys][k] for k in data.n_experiments[name_sys].keys()])
 
         gamma_value = 0
-        
+
         if if_fixed_lambdas:
             for name_sys in system_names:
-                gamma_value += gamma_function(x0[name_sys], flatten_g[name_sys], flatten_gexp[name_sys], weights_P[name_sys], alpha)
+                args = (x0[name_sys], flatten_g[name_sys], flatten_gexp[name_sys], weights_P[name_sys], alpha)
+                gamma_value += gamma_function(*args)
         else:
 
             global minis
             minis = {}
             mini_x = []
-            
+
             for name_sys in system_names:
 
-                if bounds is not None: boundaries = bounds[name_sys]
-                else: boundaries = None
+                if bounds is not None:
+                    boundaries = bounds[name_sys]
+                    method = 'L-BFGS-B'
+                else:
+                    boundaries = None
+                    method = 'BFGS'
 
                 options = {'gtol': gtol_inn}
-                if method == 'L-BFGS-B': options['ftol'] = 0
+                if method == 'L-BFGS-B':
+                    options['ftol'] = 0
+
+                args = (flatten_g[name_sys], flatten_gexp[name_sys], weights_P[name_sys], alpha, True)
+                mini = minimize(
+                    gamma_function, x0[name_sys], args=args, method=method, bounds=boundaries, jac=True, options=options)
 
-                mini = minimize(gamma_function, x0[name_sys], args = (flatten_g[name_sys], flatten_gexp[name_sys], weights_P[name_sys], alpha, True),
-                    method = method, bounds = boundaries, jac = True, options = options)
-                
                 minis[name_sys] = mini
                 mini_x.append(mini.x)
                 gamma_value += mini.fun
 
             lambdas = np.concatenate(mini_x)
 
         loss -= alpha*gamma_value
 
-    ''' 3. add regularization of force-field correction '''
-    
+    """ 3. add regularization of force-field correction """
+
     if not (np.isinf(beta) or beta == 0):
         if not isinstance(regularization['force_field_reg'], str):
             reg_ff = regularization['force_field_reg'](pars_ff)
-            loss += beta*reg_ff 
+            loss += beta*reg_ff
         elif not regularization['force_field_reg'] == 'KL divergence':
-            reg_ff = l2_regularization(pars_ff,regularization['force_field_reg'])[0]
+            reg_ff = l2_regularization(pars_ff, regularization['force_field_reg'])[0]
             loss += beta*reg_ff
         else:
             reg_ff = {}
             for name_sys in correction_ff.keys():
-                reg_ff[name_sys] = compute_D_KL(weights_P[name_sys], correction_ff[name_sys], data[name_sys].temperature, logZ_P[name_sys])
+                reg_ff[name_sys] = compute_D_KL(
+                    weights_P[name_sys], correction_ff[name_sys], data[name_sys].temperature, logZ_P[name_sys])
                 loss += beta*reg_ff[name_sys]
 
-    ''' 4. add regularization of forward-model coefficients '''
+    """ 4. add regularization of forward-model coefficients """
     if not (np.isinf(gamma) or gamma == 0):
-        reg_fm =  regularization['forward_model_reg'](pars_fm, data['global'].forward_coeffs_0)
+        reg_fm = regularization['forward_model_reg'](pars_fm, data['global'].forward_coeffs_0)
         loss += gamma*reg_fm
 
-    # print('loss function: ', loss)
-
-    ''' 5. if if_save, save values (in detail) '''
+    """ 5. if if_save, save values (in detail) """
     if if_save:
-        class Details_class: pass
+        class Details_class:
+            pass
         Details = Details_class()
 
         Details.loss = loss
 
         if not np.isinf(alpha) and not if_fixed_lambdas:
             Details.minis = minis
-        
+
         if not np.isinf(beta):
             Details.weights_P = weights_P
             Details.logZ_P = logZ_P
             Details.reg_ff = reg_ff
 
         # just with correction to the force field and to the forward model (not to the ensemble)
         if np.isinf(alpha):
             Details.av_g = av_g
             Details.chi2 = chi2
-        
-        if not np.isinf(gamma): Details.reg_fm = reg_fm
 
-        if not hasattr(Details, 'loss_explicit'): Details.loss_explicit = None # for pylint
+        if not np.isinf(gamma):
+            Details.reg_fm = reg_fm
+
+        if not hasattr(Details, 'loss_explicit'):
+            Details.loss_explicit = None  # for pylint
 
         if not np.isinf(alpha):
 
-            ''' Details_ER has attributes with names different from those of Details, as defined up to now '''
+            """ Details_ER has attributes with names different from those of Details, as defined up to now """
             dict_lambdas = {}
-            for i_sys,name_sys in enumerate(system_names):
+            for i_sys, name_sys in enumerate(system_names):
                 dict_lambdas[name_sys] = np.array(lambdas[js[i_sys][0]:js[i_sys][-1]])
-    
+
             Details_ER = compute_details_ER(weights_P, g, data, dict_lambdas, alpha)
 
             my_keys = [x for x in dir(Details_ER) if not x.startswith('__')]
-            for k in my_keys: setattr(Details, k, getattr(Details_ER, k))
+            for k in my_keys:
+                setattr(Details, k, getattr(Details_ER, k))
             del Details_ER
 
             if hasattr(Details, 'loss_explicit'):
                 if not np.isinf(beta):
-                    for name_sys in system_names: Details.loss_explicit += beta*reg_ff[name_sys]
-                if not np.isinf(gamma): Details.loss_explicit += gamma*reg_fm
-            else: print('error in loss_explicit')
+                    for name_sys in system_names:
+                        Details.loss_explicit += beta*reg_ff[name_sys]
+                if not np.isinf(gamma):
+                    Details.loss_explicit += gamma*reg_fm
+            else:
+                print('error in loss_explicit')
 
-        '''  just to improve the readability of the output: '''
+        """  just to improve the readability of the output: """
         if np.isinf(alpha):
             if np.isinf(beta) and np.isinf(gamma):
-                print('all the hyperparameters are infinite')#, namely, return original ensembles')
+                print('all the hyperparameters are infinite')  # , namely, return original ensembles')
             elif not np.isinf(beta):
                 Details.weights_new = Details.weights_P
                 Details.logZ_new = Details.logZ_P
                 del Details.weights_P, Details.logZ_P
 
         if np.isinf(alpha) and np.isinf(beta) and not np.isinf(gamma):
             Details.weights_new = {}
-            for name_sys in system_names: Details.weights_new[name_sys] = data[name_sys].weights
+            for name_sys in system_names:
+                Details.weights_new[name_sys] = data[name_sys].weights
             print('new weights are equal to original weights')
-        
-        if Details.loss_explicit is None: del Details.loss_explicit # for pylint
+
+        if Details.loss_explicit is None:
+            del Details.loss_explicit  # for pylint
 
         return Details
 
     return loss
 
 # %% C8. loss_function_and_grad
 
-''' This function evaluates loss_function and its gradient; the gradient function is computed by Jax and
-    passed as input.
-    Equivalently, you can modify the code in order to compute the gradient by hand inside loss_function
-    and then return values of loss_function value its gradient.
-    If not np.isinf(alpha), it appends also loss and lambdas to intermediates.loss and intermediates.lambdas. '''
 
-def loss_function_and_grad(pars, data, regularization, alpha, beta, gamma, gtol_inn, method, boundaries, gradient_fun):
-    
+"""
+This function **loss_function_and_grad** returns loss_function and its gradient;
+the gradient function, which is going to be evaluated, is computed by Jax and passed as input.
+If not np.isinf(alpha), it appends also loss and lambdas to intermediates.loss and intermediates.lambdas.
+
+Input parameters:
+- pars: np.array of parameters for force-field correction and forward model, respectively;
+- data, regularization: dicts (see for loss_function);
+- alpha, beta, gamma: floats (hyperparameters);
+- gtol_inn: float (see for loss_function);
+- boundaries: dict (see for loss_function);
+- gradient_fun: function (gradient of loss_function).
+
+Global: intermediates (intermediate values during minimization steps of loss_function).
+"""
+
+
+def loss_function_and_grad(
+        pars: np.array, data: dict, regularization: dict, alpha: float, beta: float, gamma: float,
+        gtol_inn: float, boundaries: dict, gradient_fun):
+
     # print('New evaluation:')
-    
-    loss = loss_function(pars, data, regularization, alpha, beta, gamma, None, gtol_inn, False, method, boundaries)
 
-    # print('loss: ', loss)
+    loss = loss_function(pars, data, regularization, alpha, beta, gamma, None, gtol_inn, False, boundaries)
 
     global intermediates
     intermediates.loss.append(loss)
     intermediates.pars.append(pars)
 
     if not np.isinf(alpha):
         try:
             intermediates.lambdas.append(lambdas)
             intermediates.minis.append(minis)
-        except: None
+        except:
+            None
 
-    ''' now evaluate the gradient w.r.t. pars at lambdas fixed (you are in the minimum: its contribute to the derivative is zero) '''
-    gradient = gradient_fun(pars, data, regularization, alpha = alpha, beta = beta, gamma = gamma, fixed_lambdas = lambdas)
+    """ now evaluate the gradient w.r.t. pars at lambdas fixed (you are in the minimum: the contribution to
+    the derivative coming from lambdas is zero) """
+    gradient = gradient_fun(pars, data, regularization, alpha=alpha, beta=beta, gamma=gamma, fixed_lambdas=lambdas)
 
+    # print('loss: ', loss)
     # print('gradient: ', gradient, '\n')
-    
+
     return loss, gradient
 
 # %% C9. deconvolve_lambdas
 
-''' If hasattr(data[name_sys],'normg_std'): also lambdas are computed with normalized data, so (if if_denormalize)
-    you go back to corresponding lambdas for non-normalized data. '''
 
-def deconvolve_lambdas(data, lambdas, if_denormalize = True):
-    
+"""
+This function **deconvolve_lambdas** deconvolves lambdas from np.array to dict of dicts (corresponding to data[name_sys].g);
+if if_denormalize, then lambdas has been computed with normalized data, so use data[name_sys].normg_std and normg_mean
+in order to go back to corresponding lambdas for non-normalized data.
+Input values: data; lambdas (np.array); if_denormalize (bool, True by default).
+The order of lambdas is the one described in compute_js.
+"""
+
+
+def deconvolve_lambdas(data, lambdas: np.array, if_denormalize: bool = True):
+
     dict_lambdas = {}
-    # list_lambdas = []
-    
+
     ns = 0
 
-    system_names = data['global'].system_names#[k for k in data.keys() if k is not 'global']
-    
+    system_names = data['global'].system_names
+
     for name_sys in system_names:
 
         dict_lambdas[name_sys] = {}
-        
+
         for name in data[name_sys].n_experiments.keys():
             dict_lambdas[name_sys][name] = lambdas[ns:(ns+data[name_sys].n_experiments[name])]
             ns += data[name_sys].n_experiments[name]
 
         if if_denormalize:
             if hasattr(data[name_sys], 'normg_std'):
                 for name in data[name_sys].ref.keys():
                     if data[name_sys].ref[name] == '><':
                         # you can sum since one of the two is zero
-                        dict_lambdas[name_sys][name] = dict_lambdas[name_sys][name+' LOWER']/data[name_sys].normg_std[name+' LOWER']
-                        dict_lambdas[name_sys][name] += dict_lambdas[name_sys][name+' UPPER']/data[name_sys].normg_std[name+' UPPER']
+                        dict_lambdas[name_sys][name] = (
+                            dict_lambdas[name_sys][name+' LOWER']/data[name_sys].normg_std[name+' LOWER'])
+
+                        dict_lambdas[name_sys][name] += (
+                            dict_lambdas[name_sys][name+' UPPER']/data[name_sys].normg_std[name+' UPPER'])
+
                         del dict_lambdas[name_sys][name+' LOWER'], dict_lambdas[name_sys][name+' UPPER']
                     else:
                         dict_lambdas[name_sys][name] = dict_lambdas[name_sys][name]/data[name_sys].normg_std[name]
-                    # list_lambdas = list_lambdas + dict_lambdas[name_sys][name]
             else:
-                print('missing normalized std values!')
+                print('Error: missing normalized std values!')
                 return
         else:
             for name in data[name_sys].ref.keys():
                 if data[name_sys].ref[name] == '><':
-                    dict_lambdas[name_sys][name] = dict_lambdas[name_sys][name+' LOWER'] + dict_lambdas[name_sys][name+' UPPER']
+                    dict_lambdas[name_sys][name] = dict_lambdas[name_sys][name+' LOWER']
+                    + dict_lambdas[name_sys][name+' UPPER']
                     del dict_lambdas[name_sys][name+' LOWER'], dict_lambdas[name_sys][name+' UPPER']
-                    # list_lambdas = list_lambdas + dict_lambdas[name_sys][name]
 
-    return dict_lambdas#, list_lambdas
+    return dict_lambdas
 
 # %% C10. minimizer
 
-''' This function minimizes loss_function'''# and do validation,
-    # both for the full data set and the selected training/test set. '''
 
-def minimizer(original_data, *, regularization = None, alpha = np.inf, beta = np.inf, gamma = np.inf, gtol = 1e-3, gtol_inn = 1e-3, data_test = None, starting_pars = None):
+"""
+This function **minimizer** minimizes loss_function on **original_data** and do **validation** on data_test (if not None).
+See Examples for further explanation.
+
+Input values:
+- original_data: data employed for minimization of loss_function (same format as data from load_data function);
+- regularization: dict (see above for loss_function);
+- alpha, beta, gamma: floats (hyperparameters for combined refinement)
+    (np.inf by default: no refinement in that direction);
+- gtol, gtol_inn: floats (gtol parameters for minimize of loss_function or inner gamma_function, respectively)
+    (1e-3 by default);
+- data_test: data employed as test set (same format as data from load_data function)
+    (None by default, namely no validation, just minimization);
+    a splitting of the full data set into training and test set is done by **select_traintest** described in the following;
+- starting_pars: np.array (pre-defined values for the starting point of loss_function minimization) (None by default).
+"""
+
+
+class intermediates_class:
+    def __init__(self, alpha):
+        self.loss = []
+        self.pars = []
+        if not np.isinf(alpha):
+            self.lambdas = []
+            self.minis = []
+
+
+def minimizer(
+        original_data, *, regularization: dict = None, alpha: float = np.inf, beta: float = np.inf, gamma: float = np.inf,
+        gtol: float = 1e-3, gtol_inn: float = 1e-3, data_test: dict = None, starting_pars: np.array = None):
 
     time1 = time.time()
 
     system_names = original_data['global'].system_names
 
-    ''' copy original_data and act only on the copy, preserving original_data '''
+    """ copy original_data and act only on the copy, preserving original_data """
 
     # data = copy.deepcopy(original_data) ## it does not work!
 
     data = {}
     for k1 in original_data.keys():
-        class my_new_class: pass
+        class my_new_class:
+            pass
         my_keys = [x for x in dir(original_data[k1]) if not x.startswith('__')]
-        for k2 in my_keys: setattr(my_new_class,k2,copy.deepcopy(getattr(original_data[k1],k2)))
+        for k2 in my_keys:
+            setattr(my_new_class, k2, copy.deepcopy(getattr(original_data[k1], k2)))
         data[k1] = my_new_class
 
-    ''' normalize observables '''
+    """ normalize observables """
     for name_sys in system_names:
         if hasattr(data[name_sys], 'g'):
             out = normalize_observables(data[name_sys].gexp, data[name_sys].g, data[name_sys].weights)
             data[name_sys].g = out[0]
             data[name_sys].gexp = out[1]
             data[name_sys].normg_mean = out[2]
             data[name_sys].normg_std = out[3]
 
-    ''' starting point for lambdas '''
+    """ starting point for lambdas """
     if not np.isinf(alpha):
-        
+
         global lambdas
 
         tot_n_exp = 0
 
         for name in system_names:
-            for item in data[name].n_experiments.values(): tot_n_exp += item
+            for item in data[name].n_experiments.values():
+                tot_n_exp += item
 
         lambdas = np.zeros(tot_n_exp)
 
-        ''' here you could duplicate lambdas for observables with both lower/upper limits '''
+        """ here you could duplicate lambdas for observables with both lower/upper limits """
 
     else:
         lambdas = None
-    
-    ''' if needed, define boundaries for minimization over lambdas '''
+
+    """ if needed, define boundaries for minimization over lambdas """
 
     if not alpha == np.inf:
 
         my_list = []
-        for k in data['global'].system_names: my_list = my_list + list(data[k].ref.values())
-        
+        for k in data['global'].system_names:
+            my_list = my_list + list(data[k].ref.values())
+
         if ('>' in my_list) or ('<' in my_list) or ('><' in my_list):
-        
-            method = 'L-BFGS-B' # 'BFGS' by default
-        
+
             bounds = {}
-        
+
             for name_sys in data['global'].system_names:
                 bounds[name_sys] = []
                 for name_type in data[name_sys].n_experiments.keys():
                     if name_type in data[name_sys].ref.keys():
                         if data[name_sys].ref[name_type] == '=':
-                            bounds[name_sys] = bounds[name_sys] + [(-np.inf,+np.inf)]*data[name_sys].g[name_type].shape[1]
+                            bounds[name_sys] = bounds[name_sys] + [(-np.inf, +np.inf)]*data[name_sys].g[name_type].shape[1]
                         elif data[name_sys].ref[name_type] == '<':
-                            bounds[name_sys] = bounds[name_sys] + [(0,+np.inf)]*data[name_sys].g[name_type].shape[1]
+                            bounds[name_sys] = bounds[name_sys] + [(0, +np.inf)]*data[name_sys].g[name_type].shape[1]
                         elif data[name_sys].ref[name_type] == '>':
-                            bounds[name_sys] = bounds[name_sys] + [(-np.inf,0)]*data[name_sys].g[name_type].shape[1]
+                            bounds[name_sys] = bounds[name_sys] + [(-np.inf, 0)]*data[name_sys].g[name_type].shape[1]
                     elif data[name_sys].ref[name_type[:-6]] == '><':
-                        bounds[name_sys] = bounds[name_sys] + [(-np.inf,0)]*data[name_sys].g[name_type].shape[1]
+                        bounds[name_sys] = bounds[name_sys] + [(-np.inf, 0)]*data[name_sys].g[name_type].shape[1]
                         # bounds = bounds + [[0,+np.inf]]*data.g[name_sys][name_type+' LOWER'].shape[1]
         else:
-            method = 'BFGS'
             bounds = None
     else:
-        method = 'BFGS'
         bounds = None
 
-    ''' minimization '''
-        
-    class intermediates_class:
-        def __init__(self, alpha):
-            self.loss = []
-            self.pars = []
-            if not np.isinf(alpha):
-                self.lambdas = []
-                self.minis = []
+    """ minimization """
 
     global intermediates
     intermediates = intermediates_class(alpha)
     global minis
 
     if (np.isinf(beta) and np.isinf(gamma)):
 
-        class Result_class: pass
+        class Result_class:
+            pass
         Result = Result_class()
-        
+
         pars_ff_fm = None
-        
-        Result.loss = loss_function(pars_ff_fm, data, regularization, alpha, beta, gamma, None, gtol_inn, False, method, bounds)
-        
+
+        Result.loss = loss_function(pars_ff_fm, data, regularization, alpha, beta, gamma, None, gtol_inn, False, bounds)
+
         # since lambdas is global, it is updated inside loss_function with optimal value
         min_lambdas = lambdas
         Result.min_lambdas = deconvolve_lambdas(data, min_lambdas)
         Result.minis = minis
 
-    else:#if not (np.isinf(beta) and np.isinf(gamma)):
+    else:
 
-        ''' starting point for the inner minimization '''
+        """ starting point for the inner minimization """
 
         if starting_pars is None:
             pars_ff_fm_0 = []
             if not np.isinf(beta):
                 names_ff_pars = data['global'].names_ff_pars
                 pars_ff_fm_0 = pars_ff_fm_0 + list(np.zeros(len(names_ff_pars)))
 
-            if not np.isinf(gamma): pars_ff_fm_0 = pars_ff_fm_0 + list(data['global'].forward_coeffs_0)
+            if not np.isinf(gamma):
+                pars_ff_fm_0 = pars_ff_fm_0 + list(data['global'].forward_coeffs_0)
             pars_ff_fm_0 = np.array(pars_ff_fm_0)
         else:
             pars_ff_fm_0 = starting_pars
 
-        ''' minimize '''
-        gradient_fun = jax.grad(loss_function, argnums = 0)
-        
-        mini = minimize(loss_function_and_grad, pars_ff_fm_0, args = (data, regularization, alpha, beta, gamma, gtol_inn, method, bounds, gradient_fun), method = 'BFGS', jac = True, options = {'gtol': gtol})
+        """ minimize """
+        gradient_fun = jax.grad(loss_function, argnums=0)
+
+        args = (data, regularization, alpha, beta, gamma, gtol_inn, bounds, gradient_fun)
+        mini = minimize(loss_function_and_grad, pars_ff_fm_0, args=args, method='BFGS', jac=True, options={'gtol': gtol})
 
         pars_ff_fm = mini.x
 
         class Result_class:
             def __init__(self, mini):
                 self.loss = mini.fun
                 self.pars = pars_ff_fm
@@ -1274,725 +1368,867 @@
 
         Result = Result_class(mini)
 
         intermediates.loss = np.array(intermediates.loss)
         intermediates.pars = np.array(intermediates.pars)
 
         if not np.isinf(alpha):
-            ''' get optimal lambdas '''
+            """ get optimal lambdas """
 
             i_min = np.argmin(intermediates.loss)
             min_lambdas = intermediates.lambdas[i_min]
             minis = intermediates.minis[i_min]
 
-            ''' denormalize and deconvolve lambdas '''
+            """ denormalize and deconvolve lambdas """
             Result.min_lambdas = deconvolve_lambdas(data, min_lambdas)
             Result.minis = minis
 
             intermediates.lambdas = np.array(intermediates.lambdas)
-            
+
         Result.intermediates = intermediates
 
-    ''' return output values '''
+    """ return output values """
 
     time2 = time.time()
-    
+
     Result.time = time2-time1
 
-    ''' use non-normalized data and non-normalized lambdas '''
+    """ use non-normalized data and non-normalized lambdas """
     if not np.isinf(alpha):
         flatten_lambda = []
         for name_sys in system_names:
-            flatten_lambda = flatten_lambda + list(np.hstack(Result.min_lambdas[name_sys][k] for k in data[name_sys].n_experiments.keys()))
+            flatten_lambda = flatten_lambda + list(
+                np.hstack(Result.min_lambdas[name_sys][k] for k in data[name_sys].n_experiments.keys()))
+
         flatten_lambda = np.array(flatten_lambda)
-    else: flatten_lambda = None
+    else:
+        flatten_lambda = None
 
-    Details = loss_function(pars_ff_fm, original_data, regularization, alpha, beta, gamma, flatten_lambda, gtol_inn, True, method, bounds)
-    if not np.isinf(alpha): del Details.loss_explicit
+    Details = loss_function(
+        pars_ff_fm, original_data, regularization, alpha, beta, gamma, flatten_lambda, gtol_inn, True, bounds)
+    if not np.isinf(alpha):
+        del Details.loss_explicit
 
-    for k in vars(Details).keys(): setattr(Result, k, getattr(Details,k))
+    for k in vars(Details).keys():
+        setattr(Result, k, getattr(Details, k))
     del Details
 
     if data_test is not None:
-        Details_test = validation(pars_ff_fm, flatten_lambda, data_test, regularization = regularization, alpha = alpha, beta = beta, gamma = gamma, which_return = 'details')
-        
+        Details_test = validation(
+            pars_ff_fm, flatten_lambda, data_test, regularization=regularization, alpha=alpha, beta=beta, gamma=gamma,
+            which_return='details')
+
         if not np.isinf(alpha):
             Details_test.loss = Details_test.loss_explicit
             del Details_test.loss_explicit
             # del Details_test.minis
-        
+
         for k in vars(Details_test).keys():
-            if not (k[-7:] == 'new_obs'): k1 = k + '_test'
-            else: k1 = k
-            setattr(Result, k1, getattr(Details_test,k))
+            if not (k[-7:] == 'new_obs'):
+                k1 = k + '_test'
+            else:
+                k1 = k
+            setattr(Result, k1, getattr(Details_test, k))
         del Details_test
 
     return Result
 
 # %% C11. select_traintest
 
-''' This function split the data set into training and test set. In particular,
-given:
+
+"""
+This function **select_traintest** splits the data set into training and test set.
+
+Input values:
 - the **data** set;
-- (required if data has attribute forward_model) **forward_model_selected**: definition of the forward model for selected observables (both train or test), which has to be defined by the user;
-- (optionally) the fraction of frames for test set **test_frames_size** and the fraction of observables for test set **test_obs_size**; each of them is a number in $(0,1)$ (same fraction for every system and for every kind of observable), by default 0.2; the **random_state** (namely, the seed, just to make same choice for different hyperparameters, otherwise it is randomly taken); if you want to specify differently, then you can insert directly the dictionaries **test_obs** and/or **test_frames**;
-- (optionally) **if_all_frames** = False by default (if True then...)
-it returns:
-- the splitting into **data_train** and **data_test**; data_test refers to: trained observables and non-trained frames (where non-specified "new"); non-trained (new) observables and non-trained/all frames (where specified "new");
-- the observables and frames (or replicas) selected for the test set **test_obs** and **test_frames** (replicas **test_rep** rather than frames if pos_replicas is not None).
-
-'''
-
-def select_traintest(data, *, test_frames_size = 0.2, test_obs_size = 0.2, random_state = None, test_frames = None, test_obs = None, if_all_frames = False, pos_replicas = None):
-    
-    ##### PART 1: IF NONE, SELECT TEST OBSERVABLES AND TEST FRAMES
+- (optionally) **test_frames_size** and **test_obs_size**: the fraction of frames for test set and
+    the fraction of observables for test set; each of them is a number in $(0,1)$ (same fraction for every system),
+    by default 0.2;
+- (optionally)**random_state** (namely, the seed, just to make same choice for different hyperparameters,
+    otherwise it is randomly taken); alternatively, you can pass the dictionaries **test_obs** and/or **test_frames**;
+- (optionally) **test_frames** and **test_obs** (dicts);
+- (optionally) **if_all_frames** (boolean, False by default; if True then use all frames for new observables in the test set);
+- (optionally) **pos_replicas** (dict for positions of replicas,
+    in order to split frames following continuous trajectories in replica exchange).
+
+Output:
+- **data_train** and **data_test**: the splitting into data_train and data_test;
+    data_test refers to:
+        trained observables and non-trained frames (where non-specified "new");
+        non-trained (new) observables and non-trained/all frames (where specified "new");
+- **test_obs** and **test_frames** (or **test_replicas**): the observables and frames (or replicas) selected for the test set
+    (replicas **test_rep** rather than frames if pos_replicas is not None).
+"""
+
 
-    system_names = data['global'].system_names#[k for k in data.keys() if k is not 'global']
+class class_test:
+    def __init__(self, data_sys, test_frames_sys, test_obs_sys, if_all_frames, data_train_sys):
+
+        # A. split weights
+        try:
+            w = data_sys.weights[test_frames_sys]
+        except:
+            w = data_sys.weights[list(test_frames_sys)]
+        self.logZ = np.log(np.sum(w))
+        self.weights = w/np.sum(w)
+        self.n_frames = np.shape(w)[0]
+
+        # B. split force-field terms
+        if hasattr(data_sys, 'f'):
+            self.ff_correction = data_sys.ff_correction
+            self.f = data_sys.f[test_frames_sys]
+
+        # C. split experimental values gexp, normg_mean and normg_std, observables g
+
+        if hasattr(data_sys, 'gexp'):
+            self.gexp_new = {}
+            self.n_experiments_new = {}
+
+            for name_type in data_sys.gexp.keys():
+
+                try:
+                    self.gexp_new[name_type] = data_sys.gexp[name_type][list(test_obs_sys[name_type])]
+                except:
+                    self.gexp_new[name_type] = data_sys.gexp[name_type][test_obs_sys[name_type]]
+
+                self.n_experiments_new[name_type] = len(test_obs_sys[name_type])
+
+        if hasattr(data_sys, 'names'):
+
+            self.names_new = {}
+
+            for name_type in data_sys.names.keys():
+                self.names_new[name_type] = data_sys.names[name_type][list(test_obs_sys[name_type])]
+
+        if hasattr(data_sys, 'g'):
+
+            self.g_new = {}
+            if if_all_frames:
+                self.g_new_old = {}
+            self.g = {}
+
+            for name_type in data_sys.g.keys():
+
+                # split g into: train, test1 (non-trained obs, all frames or only non-used ones),
+                # test2 (trained obs, non-used frames)
+                # if not test_obs[name_sys][name_type] == []:
+                self.g_new[name_type] = (data_sys.g[name_type][test_frames_sys, :].T)[test_obs_sys[name_type], :].T
+
+                if if_all_frames:  # new observables on trained frames
+                    self.g_new_old[name_type] = np.delete(
+                        data_sys.g[name_type], test_frames_sys, axis=0)[:, list(test_obs_sys[name_type])]
+
+                g3 = np.delete(data_sys.g[name_type], test_obs_sys[name_type], axis=1)
+                self.g[name_type] = g3[test_frames_sys, :]
+
+        if hasattr(data_sys, 'forward_qs'):
+
+            self.forward_qs = {}
+
+            for name_type in data_sys.forward_qs.keys():
+                self.forward_qs[name_type] = data_sys.forward_qs[name_type][list(test_frames_sys), :]
+
+            if if_all_frames:
+                self.forward_qs_trained = data_train_sys.forward_qs
+
+        if hasattr(data_sys, 'forward_model'):
+            self.forward_model = data_sys.forward_model
+
+        self.ref = data_sys.ref
+        self.selected_obs = data_train_sys.selected_obs  # same observables as in training
+        self.selected_obs_new = test_obs_sys
+
+        self.gexp = data_train_sys.gexp
+        self.n_experiments = data_train_sys.n_experiments
+        self.temperature = data_sys.temperature
+
+
+class class_train:
+    def __init__(self, data_sys, test_frames_sys, test_obs_sys):
+
+        # A. split weights
+        w = np.delete(data_sys.weights, test_frames_sys)
+        self.logZ = np.log(np.sum(w))
+        self.weights = w/np.sum(w)
+        self.n_frames = np.shape(w)[0]
+
+        # B. split force-field terms
+
+        if hasattr(data_sys, 'f'):
+            self.ff_correction = data_sys.ff_correction
+            self.f = np.delete(data_sys.f, test_frames_sys, axis=0)
+
+        # C. split experimental values gexp, normg_mean and normg_std, observables g
+
+        if hasattr(data_sys, 'gexp'):
+
+            self.gexp = {}
+            self.n_experiments = {}
+
+            for name_type in data_sys.gexp.keys():
+                self.gexp[name_type] = np.delete(data_sys.gexp[name_type], test_obs_sys[name_type], axis=0)
+                self.n_experiments[name_type] = np.shape(self.gexp[name_type])[0]
+
+        if hasattr(data_sys, 'names'):
+
+            self.names = {}
+
+            for name_type in data_sys.names.keys():
+                train_obs = list(set(np.arange(data_sys.names[name_type].shape[0]))-set(test_obs_sys[name_type]))
+                self.names[name_type] = data_sys.names[name_type][train_obs]
+
+        if hasattr(data_sys, 'g'):
+
+            self.g = {}
+
+            for name_type in data_sys.g.keys():
+                train_g = np.delete(data_sys.g[name_type], test_frames_sys, axis=0)
+                self.g[name_type] = np.delete(train_g, test_obs_sys[name_type], axis=1)
+
+        if hasattr(data_sys, 'forward_qs'):
+
+            self.forward_qs = {}
+
+            for name_type in data_sys.forward_qs.keys():
+                self.forward_qs[name_type] = np.delete(data_sys.forward_qs[name_type], test_frames_sys, axis=0)
+
+        if hasattr(data_sys, 'forward_model'):
+            self.forward_model = data_sys.forward_model
+
+        self.ref = data_sys.ref
+
+        train_obs = {}
+        for s in data_sys.n_experiments.keys():
+            train_obs[s] = list(set(np.arange(data_sys.n_experiments[s]))-set(test_obs_sys[s]))
+        self.selected_obs = train_obs
+
+        self.temperature = data_sys.temperature
+
+
+def select_traintest(
+        data, *, test_frames_size: float = 0.2, test_obs_size: float = 0.2, random_state: int = None,
+        test_frames: dict = None, test_obs: dict = None, if_all_frames: bool = False, pos_replicas: dict = None):
+
+    # PART 1: IF NONE, SELECT TEST OBSERVABLES AND TEST FRAMES
+
+    system_names = data['global'].system_names
     rng = None
 
     if (test_frames is None) or (test_obs is None):
-    
+
         if random_state is None:
-            try: random_state = random.randint(1000)
-            except: print('error: Jax requires to specify random state'); return
-            print('random_state: ',random_state)
+            # try:
+            random_state = random.randint(1000)
+            # except:
+            #     print('error: Jax requires to specify random state')
+            #     return
+            print('random_state: ', random_state)
 
-        rng = random.default_rng(seed = random_state)
+        rng = random.default_rng(seed=random_state)
         # except: key = random.PRNGKey(random_state)
 
-        if not (test_obs_size > 0 and test_obs_size < 1): print('error on test_obs_size'); return
-        if not (test_frames_size > 0 and test_frames_size < 1): print('error on test_frames_size'); return
+        if not (test_obs_size > 0 and test_obs_size < 1):
+            print('error on test_obs_size')
+            return
+        if not (test_frames_size > 0 and test_frames_size < 1):
+            print('error on test_frames_size')
+            return
         # check_consistency(test_obs_size,data.n_experiments,0,data.g)
         # check_consistency(test_frames_size,data.n_frames,1,data.g)
 
-        if test_frames is not None: print('Input random_state employed only for test_obs since test_frames are given')
-        elif test_obs is not None: print('Input random_state employed only for test_frames since test_obs are given')
-        else: print('Input random_state employed both for test_obs and test_frames')
-    
-    elif random_state is not None: print('Input random_state not employed, since both test_frames and test_obs are given')
+        if test_frames is not None:
+            print('Input random_state employed only for test_obs since test_frames are given')
+        elif test_obs is not None:
+            print('Input random_state employed only for test_frames since test_obs are given')
+        else:
+            print('Input random_state employed both for test_obs and test_frames')
+
+    elif random_state is not None:
+        print('Input random_state not employed, since both test_frames and test_obs are given')
+
+    # 1B. FRAMES TEST
 
-    ### 1B. FRAMES TEST
-    
     if test_frames is None:
 
         test_frames = {}
-        
+
         # if you have demuxed trajectories, select replicas and the corresponding frames
-        
+
         if pos_replicas is not None:
-            
+
             n_replicas = {}
             n_replicas_test = {}
             test_rep = {}
 
             for name_sys in system_names:
                 n_replicas[name_sys] = len(pos_replicas[name_sys])
                 n_replicas_test[name_sys] = np.int16(np.round(test_frames_size*n_replicas))
-                
-                test_rep[name_sys] = np.sort(rng.choice(n_replicas[name_sys],n_replicas_test[name_sys],replace = False))
-                # except: test_rep[name_sys] = random.choice(key, n_replicas[name_sys], (n_replicas_test[name_sys],), replace = False)
+
+                test_rep[name_sys] = np.sort(rng.choice(n_replicas[name_sys], n_replicas_test[name_sys], replace=False))
+                # except:
+                # test_rep[name_sys] = random.choice(key, n_replicas[name_sys], (n_replicas_test[name_sys],), replace = False)
 
                 fin = []
                 for i in range(n_replicas_test[name_sys]):
-                    fin = np.concatenate((fin,pos_replicas[name_sys][test_rep[name_sys][i]].flatten()),axis = 0)
+                    fin = np.concatenate((fin, pos_replicas[name_sys][test_rep[name_sys][i]].flatten()), axis=0)
                 test_frames[name_sys] = np.array(fin).astype(int)
                 del fin
-        
+
         else:
-            
+
             n_frames_test = {}
-            
+
             for name_sys in system_names:
                 n_frames_test[name_sys] = np.int16(np.round(test_frames_size*data[name_sys].n_frames))
-                test_frames[name_sys] = np.sort(rng.choice(data[name_sys].n_frames,n_frames_test[name_sys],replace = False))
-                # except: test_frames[name_sys] = random.choice(key, data[name_sys].n_frames,(n_frames_test[name_sys],),replace = False)
+                test_frames[name_sys] = np.sort(rng.choice(data[name_sys].n_frames, n_frames_test[name_sys], replace=False))
+                # except:
+                # test_frames[name_sys] = random.choice(key, data[name_sys].n_frames,(n_frames_test[name_sys],),
+                # replace = False)
 
-    ### 1C. OBSERVABLES TEST
+    # 1C. OBSERVABLES TEST
 
     if test_obs is None:
 
         n_obs_test = {}
         test_obs = {}
 
-        ''' here you select with the same fraction for each type of observable'''
+        """ here you select with the same fraction for each type of observable"""
         # for name_sys in data.weights.keys():
         #     n_obs_test[name_sys] = {}
         #     test_obs[name_sys] = {}
 
         #     for name_type in data.g[name_sys].keys():
         #         n_obs_test[name_sys][name_type] = np.int16(np.round(test_obs_size*data.n_experiments[name_sys][name_type]))
-        #         test_obs[name_sys][name_type] = np.sort(rng.choice(data.n_experiments[name_sys][name_type],n_obs_test[name_sys][name_type],replace = False))
+        #         test_obs[name_sys][name_type] = np.sort(rng.choice(data.n_experiments[name_sys][name_type],
+        #           n_obs_test[name_sys][name_type],replace = False))
 
-        ''' here instead you select the same fraction for each system and then take the corresponding observables (in this way, no issue for types of observables with only 1 observable '''
+        """ here instead you select the same fraction for each system and then take the corresponding observables
+        (in this way, no issue for types of observables with only 1 observable """
         for name_sys in system_names:
 
             n_obs_test[name_sys] = {}
             test_obs[name_sys] = {}
 
             n = np.sum(np.array(list(data[name_sys].n_experiments.values())))
-            vec = np.sort(rng.choice(n,np.int16(np.round(n*test_obs_size)), replace = False))
+            vec = np.sort(rng.choice(n, np.int16(np.round(n*test_obs_size)), replace=False))
             # except: vec = np.sort(jax.random.choice(key, n, (np.int16(np.round(n*test_obs_size)),), replace = False))
 
             sum = 0
             for name_type in data[name_sys].n_experiments.keys():
-                
+
                 test_obs[name_sys][name_type] = vec[(vec >= sum) & (vec < sum + data[name_sys].n_experiments[name_type])] - sum
                 n_obs_test[name_sys][name_type] = len(test_obs[name_sys][name_type])
 
                 sum += data[name_sys].n_experiments[name_type]
 
         del sum, n, vec
 
-    ##### PART 2: GIVEN test_frames and test_obs, RETURN data_test AND data_train
+    # PART 2: GIVEN test_frames and test_obs, RETURN data_test AND data_train
     # train, test1 ('non-trained' obs, all or 'non-used' frames), test2 ('trained' obs, 'non-used' frames)
 
     data_train = {}
     data_test = {}
 
-    # # global properties:
-
-    # class my_class: pass
-    
-    # my_class.forward_coeffs_0 = data['global'].forward_coeffs_0
-    
-    # data_train['global'] = my_class
-    # data_test['global'] = my_class
-
-    # del my_class # to be sure data_train['global'] and data_test['global'] will not be modified later!
+    # global properties:
 
     data_train['global'] = data['global']
     data_test['global'] = data['global']
 
     # for over different systems:
 
     for name_sys in system_names:
 
-        class class_test: pass
-        class class_train: pass
-
-        ### 2A. SPLIT WEIGHTS
-
-        try: w = data[name_sys].weights[test_frames[name_sys]]
-        except: w = data[name_sys].weights[list(test_frames[name_sys])]
-        class_test.logZ = np.log(np.sum(w))
-        class_test.weights = w/np.sum(w)
-        class_test.n_frames = np.shape(w)[0]
-        
-        w = np.delete(data[name_sys].weights,test_frames[name_sys])
-        class_train.logZ = np.log(np.sum(w))
-        class_train.weights = w/np.sum(w)
-        class_train.n_frames = np.shape(w)[0]
-
-        ### 2B. SPLIT FORCE-FIELD TERMS F
-
-        if hasattr(data[name_sys],'f'):
-
-            class_test.ff_correction = data[name_sys].ff_correction
-            class_train.ff_correction = data[name_sys].ff_correction
-
-            # class_test.f = data[name_sys].f.iloc[test_frames[name_sys]]
-            class_test.f = data[name_sys].f[test_frames[name_sys]]
-            
-            # train_frames = list(set(np.arange(data[name_sys].f.shape[0]))-set(test_frames[name_sys]))
-            # class_train.f = data[name_sys].f.iloc[train_frames]
-            class_train.f = np.delete(data[name_sys].f, test_frames[name_sys], axis = 0)
-
-        ### 2C. SPLIT EXPERIMENTAL VALUES GEXP, NORMG_MEAN AND NORMG_STD, OBSERVABLES G
-
-        if hasattr(data[name_sys],'gexp'):
-            
-            class_test.gexp_new = {}
-            class_train.gexp = {}
-            class_train.n_experiments = {}
-            class_test.n_experiments_new = {}
-
-            for name_type in data[name_sys].gexp.keys():
-
-                try: class_test.gexp_new[name_type] = data[name_sys].gexp[name_type][list(test_obs[name_sys][name_type])]
-                except: class_test.gexp_new[name_type] = data[name_sys].gexp[name_type][test_obs[name_sys][name_type]]
-                class_test.n_experiments_new[name_type] = len(test_obs[name_sys][name_type])
-
-                class_train.gexp[name_type] = np.delete(data[name_sys].gexp[name_type],test_obs[name_sys][name_type],axis=0)
-                class_train.n_experiments[name_type] = np.shape(class_train.gexp[name_type])[0]
-                
-        if hasattr(data[name_sys],'names'):
-
-            class_test.names_new = {}
-            class_train.names = {}
-
-            for name_type in data[name_sys].names.keys():
-                class_test.names_new[name_type] = data[name_sys].names[name_type][list(test_obs[name_sys][name_type])]
-                train_obs = list(set(np.arange(data[name_sys].names[name_type].shape[0]))-set(test_obs[name_sys][name_type]))
-                class_train.names[name_type] = data[name_sys].names[name_type][train_obs]
-
-        if hasattr(data[name_sys],'g'):
-
-            class_test.g_new = {}
-            if if_all_frames: class_test.g_new_old = {}
-            class_test.g = {}
-            class_train.g = {}
-
-            for name_type in data[name_sys].g.keys():
+        data_train[name_sys] = class_train(data[name_sys], test_frames[name_sys], test_obs[name_sys])
+        data_test[name_sys] = class_test(
+            data[name_sys], test_frames[name_sys], test_obs[name_sys], if_all_frames, data_train[name_sys])
 
-                # split g into: train, test1 (non-trained obs, all frames or only non-used ones), test2 (trained obs, non-used frames)
-                # if not test_obs[name_sys][name_type] == []:
-                class_test.g_new[name_type] = (data[name_sys].g[name_type][test_frames[name_sys],:].T)[test_obs[name_sys][name_type],:].T
-                
-                if if_all_frames == True: # new observables on trained frames
-                    class_test.g_new_old[name_type] = np.delete(data[name_sys].g[name_type],test_frames[name_sys],axis=0)[:,list(test_obs[name_sys][name_type])]
-    
-                g3 = np.delete(data[name_sys].g[name_type],test_obs[name_sys][name_type],axis=1)
-                class_test.g[name_type] = g3[test_frames[name_sys],:]
-
-                train_g = np.delete(data[name_sys].g[name_type],test_frames[name_sys],axis=0)
-                class_train.g[name_type] = np.delete(train_g,test_obs[name_sys][name_type],axis=1)
-
-        if hasattr(data[name_sys],'forward_qs'):
-
-            class_test.forward_qs = {}
-            class_train.forward_qs = {}
-            
-            for name_type in data[name_sys].forward_qs.keys():
-                class_test.forward_qs[name_type] = data[name_sys].forward_qs[name_type][list(test_frames[name_sys]),:]
-                class_train.forward_qs[name_type] = np.delete(data[name_sys].forward_qs[name_type],test_frames[name_sys],axis=0)
-                
-        if if_all_frames:
-            class_test.forward_qs_trained = class_train.forward_qs
-
-        if hasattr(data[name_sys],'forward_model'):
-            class_test.forward_model = data[name_sys].forward_model
-            class_train.forward_model = data[name_sys].forward_model
-
-        class_train.ref = data[name_sys].ref
-        class_test.ref = data[name_sys].ref
-
-        train_obs = {}
-        for s in data[name_sys].n_experiments.keys():
-            train_obs[s] = list(set(np.arange(data[name_sys].n_experiments[s]))-set(test_obs[name_sys][s]))
-        class_train.selected_obs = train_obs
-        class_test.selected_obs = train_obs # same observables as in training
-        class_test.selected_obs_new = test_obs[name_sys] # test observables
-
-        # same as data_train
-        class_test.gexp = class_train.gexp
-        class_test.n_experiments = class_train.n_experiments
-        class_test.temperature = data[name_sys].temperature
-        class_train.temperature = data[name_sys].temperature
-
-        # class_train.normg_std = data[name_sys].normg_std
-        # class_train.normg_mean = data[name_sys].normg_mean
-
-        # class_test.normg_std = data[name_sys].normg_std
-        # class_test.normg_mean = data[name_sys].normg_mean
-
-        data_train[name_sys] = class_train
-        data_test[name_sys] = class_test
-
-        del class_train, class_test
-
-    # ''' if some type of observables are not included in test observables, delete them to avoid empty items '''
+    # """ if some type of observables are not included in test observables, delete them to avoid empty items """
     # for name_sys in system_names:
     #     for name_type in test_obs[name_sys].keys():
     #         if len(test_obs[name_sys][name_type]) == 0:
     #             del data_test[name_sys].gexp_new[name_type]
     #             if name_type in data_test[name_sys].g_new.keys():
     #                 del data_test[name_sys].g_new[name_type]
     #                 if if_all_frames: del data_test[name_sys].g_new_old[name_type]
 
     for s1 in test_obs.keys():
         my_list1 = []
         my_list2 = []
-        
+
         for s2 in test_obs[s1].keys():
-            if len(test_obs[s1][s2]) == 0: my_list1.append(s2)
-            elif len(test_obs[s1][s2]) == data[s1].n_experiments[s2]: my_list2.append(s2)
+            if len(test_obs[s1][s2]) == 0:
+                my_list1.append(s2)
+            elif len(test_obs[s1][s2]) == data[s1].n_experiments[s2]:
+                my_list2.append(s2)
 
         for s2 in my_list1:
-            ''' no test observables of this kind '''
+            """ no test observables of this kind """
             del data_test[s1].gexp_new[s2], data_test[s1].g_new[s2], data_test[s1].n_experiments_new[s2]
-            del data_test[s1].selected_obs_new[s2]#, data_test[s1].names_new[s2]
-        
+            del data_test[s1].selected_obs_new[s2]  # , data_test[s1].names_new[s2]
+
         for s2 in my_list2:
-            ''' no training observables of this kind'''
+            """ no training observables of this kind"""
             del data_test[s1].gexp[s2], data_test[s1].g[s2], data_test[s1].n_experiments[s2]
-            del data_test[s1].selected_obs[s2]#, data_test[s1].names[s2]
+            del data_test[s1].selected_obs[s2]  # , data_test[s1].names[s2]
             del data_train[s1].gexp[s2], data_train[s1].g[s2], data_train[s1].n_experiments[s2]
-            del data_train[s1].selected_obs[s2]#, data_train[s1].names[s2]
+            del data_train[s1].selected_obs[s2]  # , data_train[s1].names[s2]
 
-        for s2 in my_list1: test_obs[s1][s2] = np.int64(np.array([]))
+        for s2 in my_list1:
+            test_obs[s1][s2] = np.int64(np.array([]))
 
-    if pos_replicas is None: return data_train, data_test, test_obs, test_frames
-    else: return data_train, data_test, test_obs, test_rep
+    if pos_replicas is None:
+        return data_train, data_test, test_obs, test_frames
+    else:
+        return data_train, data_test, test_obs, test_rep
 
 # %% C12. validation
 
-''' This function computes the chi2 on new observables, starting from original data set and optimal parameters
-    (in this way you can compute the full derivative with Jax); if hasattr(data_test, 'forward_qs_trained') and
-    you have passed also data_train, it includes also training frames. If which_return == 'validation chi2' then
-    it returns chi2 on validation data set (same observables, new frames), used to compute the derivative with Jax;
-    elif which_return == 'test chi2' then it returns chi2 on test data set (new observables), used to compute the 
-    derivative with Jax; elif which_return == 'details' then it returns a class with all the computed values. 
-    The splitting of pars_ff_fm into ff and fm is determined by data_test[name_sys].f, which has the same columns
-    as data_train[name_sys].f. '''
 
-def validation(pars_ff_fm, lambdas, data_test, *, regularization = None, alpha = np.inf, beta = np.inf, gamma = np.inf, data_train = None, which_return = 'details'):
+"""
+This function **validation** evaluates loss_function in detail over the test set; then,
+- if which_return == 'chi2 validation', it returns total chi2 on validation data set (same observables, new frames)
+    (used to compute the derivatives with Jax);
+- elif which_return == 'chi2 test', it returns total chi2 on test data set (new observables, new frames
+    or all frames if data_train is not None) (used to compute the derivatives with Jax);
+- else, it returns Validation_values class, with all the computed values.
+
+Input values:
+- pars_ff_fm: np.array for force-field and forward-model coefficients;
+- lambdas: np.array of lambdas coefficients (those for ensemble refinement);
+- data_test: dict for test data set, as given by select_traintest;
+- regularization: see above for loss_function (by default, None);
+- alpha, beta, gamma: floats for hyperparameters (by default, np.inf);
+- data_train: dict for training data set, as given by select_traintest (None by default,
+    namely use only test frames for new observables);
+- which_return: str described above (by default 'details').
+"""
+
+
+def validation(
+        pars_ff_fm, lambdas, data_test, *, regularization=None, alpha=np.inf, beta=np.inf, gamma=np.inf,
+        data_train=None, which_return='details'):
 
-    system_names = data_test['global'].system_names#[k for k in data_test.keys() if k is not 'global']
+    system_names = data_test['global'].system_names
     names_ff_pars = []
 
     if not np.isinf(beta):
         names_ff_pars = data_test['global'].names_ff_pars
-        # pars_ff = pars_ff_fm[:len(names_ff_pars)]
-    
-    pars_fm = None # to avoid error in pylint
-    if not np.isinf(gamma): pars_fm = pars_ff_fm[len(names_ff_pars):]
-    if names_ff_pars == []: del names_ff_pars
-
-    # class data_test: pass
-    # my_keys = [x for x in dir(original_data_test) if not x.startswith('__')]
-    # for k in my_keys: setattr(data_test, k, copy.deepcopy(getattr(original_data_test, k)))
-    
-    # def Validation_class(): pass
 
-    ''' Compute loss_function in detail for validating set (same observables as in training, new frames). '''
-    Validation_values = loss_function(pars_ff_fm, data_test, regularization, alpha, beta, gamma, lambdas, if_save = True)
+    pars_fm = None  # to avoid error in pylint
+    if not np.isinf(gamma):
+        pars_fm = pars_ff_fm[len(names_ff_pars):]
+    if names_ff_pars == []:
+        del names_ff_pars
+
+    """ Compute loss_function in detail for validating set (same observables as in training, new frames). """
+    Validation_values = loss_function(pars_ff_fm, data_test, regularization, alpha, beta, gamma, lambdas, if_save=True)
 
     if which_return == 'chi2 validation':
         tot_chi2 = 0
         for s1 in Validation_values.chi2.keys():
-            for item in Validation_values.chi2[s1].values(): tot_chi2 += item
+            for item in Validation_values.chi2[s1].values():
+                tot_chi2 += item
         return tot_chi2
 
-    # my_keys = [x for x in dir(Details) if not x.startswith('__')]
-
-    # s = '_test'
-    # for k in my_keys: setattr(Validation_class,k+s,getattr(Details,k))
-    # del Details
-
-    ### data_test1: non-trained observables, all or non-trained frames
-
     # let's compute firstly the average of non-trained (validating) observables on new frames
 
     Validation_values.avg_new_obs = {}
     Validation_values.chi2_new_obs = {}
 
-        # if hasattr(data_test,'selected_obs'):
-        #     for name in data_test.forward_qs.keys():
-        #         for type_name in data_test.forward_qs[name].keys():
-        #             data_test.forward_qs[name][type_name] = data_test.forward_qs[name][type_name]#[:,data_test.selected_obs[name][type_name]]
+    # if hasattr(data_test,'selected_obs'):
+    #     for name in data_test.forward_qs.keys():
+    #         for type_name in data_test.forward_qs[name].keys():
+    #             data_test.forward_qs[name][type_name] = data_test.forward_qs[name][type_name]
+    #               #[:,data_test.selected_obs[name][type_name]]
 
     g = {}
 
     for name_sys in system_names:
-        
+
         if np.isinf(gamma):
-            if hasattr(data_test[name_sys], 'g_new'): g[name_sys] = copy.deepcopy(data_test[name_sys].g_new)
+            if hasattr(data_test[name_sys], 'g_new'):
+                g[name_sys] = copy.deepcopy(data_test[name_sys].g_new)
         else:
-            if hasattr(data_test[name_sys], 'g_new'): g[name_sys] = copy.deepcopy(data_test[name_sys].g_new)
-            else: g[name_sys] = {}
+            if hasattr(data_test[name_sys], 'g_new'):
+                g[name_sys] = copy.deepcopy(data_test[name_sys].g_new)
+            else:
+                g[name_sys] = {}
 
-            if hasattr(data_test[name_sys], 'selected_obs'): selected_obs = data_test[name_sys].selected_obs_new
-            else: selected_obs = None
+            if hasattr(data_test[name_sys], 'selected_obs'):
+                selected_obs = data_test[name_sys].selected_obs_new
+            else:
+                selected_obs = None
 
             fm_observables = data_test[name_sys].forward_model(pars_fm, data_test[name_sys].forward_qs, selected_obs)
 
             for name in fm_observables.keys():
-                
+
                 g[name_sys][name] = fm_observables[name]
-                if hasattr(data_test[name_sys], 'normg_mean'): g[name_sys][name] = (g[name_sys][name]-data_test[name_sys].normg_mean[name])/data_test[name_sys].normg_std[name]
+                if hasattr(data_test[name_sys], 'normg_mean'):
+                    g[name_sys][name] = (
+                        g[name_sys][name]-data_test[name_sys].normg_mean[name])/data_test[name_sys].normg_std[name]
 
             del fm_observables
 
     for name_sys in system_names:
-        
-        out = compute_chi2(data_test[name_sys].ref, Validation_values.weights_new[name_sys], g[name_sys], data_test[name_sys].gexp_new)
+
+        args = (data_test[name_sys].ref, Validation_values.weights_new[name_sys], g[name_sys], data_test[name_sys].gexp_new)
+        out = compute_chi2(*args)
 
         Validation_values.avg_new_obs[name_sys] = out[0]
 
         if not hasattr(data_test, 'forward_qs_trained'):
-            Validation_values.chi2_new_obs[name_sys] = out[2]
+            Validation_values.chi2_new_obs[name_sys] = out[1]
 
     # then, if you want to include also trained frames for validating observables:
 
-    if hasattr(data_test, 'forward_qs_trained') and (data_train is not None): # forward qs on trained frames
+    if hasattr(data_test, 'forward_qs_trained') and (data_train is not None):  # forward qs on trained frames
 
-        Details_train = loss_function(pars_ff_fm, data_train, regularization, alpha, beta, gamma, lambdas, if_save = True)
+        Details_train = loss_function(pars_ff_fm, data_train, regularization, alpha, beta, gamma, lambdas, if_save=True)
 
         g = {}
 
         for name_sys in system_names:
             if np.isinf(gamma):
-                if hasattr(data_test[name_sys], 'g_new_old'): g[name_sys] = copy.deepcopy(data_test[name_sys].g_new_old)
+                if hasattr(data_test[name_sys], 'g_new_old'):
+                    g[name_sys] = copy.deepcopy(data_test[name_sys].g_new_old)
             else:
-                if hasattr(data_test[name_sys], 'g_new_old'): g[name_sys] = copy.deepcopy(data_test[name_sys].g_new_old)
-                else: g[name_sys] = {}
+                if hasattr(data_test[name_sys], 'g_new_old'):
+                    g[name_sys] = copy.deepcopy(data_test[name_sys].g_new_old)
+                else:
+                    g[name_sys] = {}
 
-                if hasattr(data_test[name_sys], 'selected_obs'): selected_obs = data_test[name_sys].selected_obs
-                else: selected_obs = None
+                if hasattr(data_test[name_sys], 'selected_obs'):
+                    selected_obs = data_test[name_sys].selected_obs
+                else:
+                    selected_obs = None
 
                 fm_observables = data_test[name_sys].forward_model(pars_fm, data_test[name_sys].forward_qs, selected_obs)
 
                 for name in fm_observables.keys():
-                    
+
                     g[name_sys][name] = fm_observables[name]
-                    if hasattr(data_test[name_sys], 'normg_mean'): g[name_sys][name] = (g[name_sys][name]-data_test[name_sys].normg_mean[name])/data_test[name_sys].normg_std[name]
+                    if hasattr(data_test[name_sys], 'normg_mean'):
+                        g[name_sys][name] = (
+                            g[name_sys][name]-data_test[name_sys].normg_mean[name])/data_test[name_sys].normg_std[name]
 
                 del fm_observables
 
             Validation_values.chi2_new_obs[name_sys] = {}
-            
-            out = compute_chi2(data_test.ref[name_sys], Details_train.weights_new[name_sys], g[name_sys], data_test.gexp_new[name_sys])[0]
 
-            log_fact_Z = data_test.logZ[name_sys] + Validation_values.logZ_new[name_sys] - Details_train.logZ_new[name_sys] - data_train[name_sys].logZ
+            args = (data_test.ref[name_sys], Details_train.weights_new[name_sys], g[name_sys], data_test.gexp_new[name_sys])
+            out = compute_chi2(*args)[0]
 
-            if hasattr(Validation_values,'logZ_P'): log_fact_Z += Validation_values.logZ_P_test[name_sys] - Details_train.logZ_P[name_sys]
+            log_fact_Z = data_test.logZ[name_sys] + Validation_values.logZ_new[name_sys]
+            - Details_train.logZ_new[name_sys] - data_train[name_sys].logZ
+
+            if hasattr(Validation_values, 'logZ_P'):
+                log_fact_Z += Validation_values.logZ_P_test[name_sys] - Details_train.logZ_P[name_sys]
 
             for name_type in data_test.n_experiments[name_sys].keys():
-                Validation_values.avg_new_obs[name_sys][name_type] = 1/(1+np.exp(log_fact_Z))*out[name_type] + 1/(1+np.exp(-log_fact_Z))*Validation_values.avg_new_obs[name_sys][name_type]
+                Validation_values.avg_new_obs[name_sys][name_type] = 1/(1+np.exp(log_fact_Z))*out[name_type]
+                + 1/(1+np.exp(-log_fact_Z))*Validation_values.avg_new_obs[name_sys][name_type]
 
-                Validation_values.chi2_new_obs[name_sys][name_type] = np.sum(((Validation_values.avg_new_obs[name_sys][name_type] - data_test.gexp_new[name_sys][name_type][:,0])/data_test.gexp_new[name_sys][name_type][:,1])**2)
+                Validation_values.chi2_new_obs[name_sys][name_type] = np.sum(((
+                    Validation_values.avg_new_obs[name_sys][name_type]
+                    - data_test.gexp_new[name_sys][name_type][:, 0])/data_test.gexp_new[name_sys][name_type][:, 1])**2)
 
-    if which_return == 'test chi2':
+    if which_return == 'chi2 test':
         tot_chi2 = 0
         for s1 in Validation_values.chi2_new_obs.keys():
-            for item in Validation_values.chi2_new_obs[s1].values(): tot_chi2 += item
+            for item in Validation_values.chi2_new_obs[s1].values():
+                tot_chi2 += item
         return tot_chi2
-    
     return Validation_values
 
 # %% D. (automatic) optimization of the hyper parameters through minimization of chi2
 
-''' Use implicit function theorem to compute the derivatives of the pars_ff_fm and lambdas w.r.t. hyper parameters. '''
 
-# %% D1. compute "hyper-derivatives", namely, derivatives of parameters w.r.t. hyper-parameters
+""" Use implicit function theorem to compute the derivatives of the pars_ff_fm and lambdas w.r.t. hyper parameters. """
+
+
+# %% D1. compute_hyperderivatives
 
-def compute_hyperderivatives(pars_ff_fm, lambdas, data, regularization, log10_alpha = np.inf, log10_beta = np.inf, log10_gamma = np.inf, derivatives_funs = None):
 
-    system_names = data['global'].system_names#[k for k in data.keys() if k is not 'global']
+"""
+Function **compute_hyperderivatives** computes the derivatives of parameters with respect to hyperparameters,
+which are going to be used later to compute the derivatives of chi2 w.r.t. hyperparameters.
+
+Input values:
+- pars_ff_fm: np.array for force-field and forward-model coefficients;
+- lambdas: np.array for lambdas coefficients (those for ensemble refinement);
+- data: dict for data set;
+- regularization: see above;
+- derivatives_funs: class of derivatives functions computed by Jax;
+- log10_alpha, log10_beta, log10_gamma: floats for log (in base 10) of corresponding hyperparameters
+    (np.inf by default).
+
+It returns instance of class derivatives, which includes as attributes values of derivatives required in the following:
+they include dlambdas_dlogalpha, dlambdas_dpars, dpars_dlogalpha, dpars_dlogbeta, dpars_dloggamma.
+"""
+
+
+def compute_hyperderivatives(
+        pars_ff_fm, lambdas, data, regularization, derivatives_funs,
+        log10_alpha=np.inf, log10_beta=np.inf, log10_gamma=np.inf):
+
+    system_names = data['global'].system_names
 
     if np.isinf(log10_beta) and np.isinf(log10_gamma) and not np.isinf(log10_alpha):
-    
+
         alpha = np.float64(10**log10_alpha)
 
         data_n_experiments = {}
-        for k in system_names: data_n_experiments[k] = data[k].n_experiments
+        for k in system_names:
+            data_n_experiments[k] = data[k].n_experiments
         js = compute_js(data_n_experiments)
 
-        class derivatives: pass
+        class derivatives:
+            pass
 
         derivatives.dlambdas_dlogalpha = {}
 
         for i_sys, name_sys in enumerate(system_names):
 
             my_lambdas = lambdas[js[i_sys][0]:js[i_sys][-1]]
-            g = np.hstack([data[name_sys].g[k] for k in data[name_sys].n_experiments])
-            gexp = np.vstack([data[name_sys].gexp[k] for k in data[name_sys].n_experiments])
-            
+
+            indices = np.nonzero(my_lambdas)[0]
+
+            # refs = []
+            # for name in data[name_sys].n_experiments.keys():
+            #     refs.extend(data[name_sys].ref[name]*data[name_sys].n_experiments[name])
+
+            # indices = np.array([k for k in indices if not refs[k] == '='])  # indices of lambdas on constraints
+
+            my_lambdas = my_lambdas[indices]
+            g = np.hstack([data[name_sys].g[k] for k in data[name_sys].n_experiments])[:, indices]
+            gexp = np.vstack([data[name_sys].gexp[k] for k in data[name_sys].n_experiments])[indices]
+
             my_args = (my_lambdas, g, gexp, data[name_sys].weights, alpha)
             Hess_inv = np.linalg.inv(derivatives_funs.d2gamma_dlambdas2(*my_args))
-            derivatives.dlambdas_dlogalpha[name_sys] = -np.matmul(Hess_inv, derivatives_funs.d2gamma_dlambdas_dalpha(*my_args))*alpha*np.log(10)
+
+            derivatives.dlambdas_dlogalpha[name_sys] = -np.matmul(
+                Hess_inv, derivatives_funs.d2gamma_dlambdas_dalpha(*my_args))*alpha*np.log(10)
 
     elif not (np.isinf(log10_beta) and np.isinf(log10_gamma)):
-        
+
         pars_ff_fm = np.array(pars_ff_fm)
 
-        class derivatives: pass
+        class derivatives:
+            pass
 
-        if not np.isinf(log10_alpha): alpha = np.float64(10**log10_alpha)
-        else: alpha = np.inf
+        if not np.isinf(log10_alpha):
+            alpha = np.float64(10**log10_alpha)
+        else:
+            alpha = np.inf
 
-        if not np.isinf(log10_beta): beta = np.float64(10**log10_beta)
-        else: beta = np.inf
+        if not np.isinf(log10_beta):
+            beta = np.float64(10**log10_beta)
+        else:
+            beta = np.inf
 
-        if not np.isinf(log10_gamma): gamma = np.float64(10**log10_gamma)
-        else: gamma = np.inf
+        if not np.isinf(log10_gamma):
+            gamma = np.float64(10**log10_gamma)
+        else:
+            gamma = np.inf
 
         args = (pars_ff_fm, data, regularization, alpha, beta, gamma, lambdas)
 
         if not np.isinf(alpha):
-            
+
             d2loss_dpars_dlambdas = derivatives_funs.d2loss_dpars_dlambdas(*args)
 
             data_n_experiments = {}
-            for k in system_names: data_n_experiments[k] = data[k].n_experiments
+            for k in system_names:
+                data_n_experiments[k] = data[k].n_experiments
             js = compute_js(data_n_experiments)
 
-            ''' %%%
+            """
             Here use Gamma function, in this way you do multiple inversions, rather than a single inversion
             of a very big matrix: different systems have uncorrelated Ensemble Refinement
             BUT you have to evaluate Gamma at given phi, theta !!
-            '''
-            
+            """
+
             derivatives.dlambdas_dlogalpha = {}
             derivatives.dlambdas_dpars = {}
 
-            terms = [] # terms to add to get d2loss_dmu2 deriving from lambdas contribution
+            terms = []  # terms to add to get d2loss_dmu2 deriving from lambdas contribution
             terms2 = []
 
             names_ff_pars = []
 
-            ''' compute new weights with ff correction phi '''
+            """ compute new weights with ff correction phi """
             if not np.isinf(beta):
-    
+
                 names_ff_pars = data['global'].names_ff_pars
                 pars_ff = pars_ff_fm[:len(names_ff_pars)]
 
                 correction_ff = {}
                 weights_P = {}
                 logZ_P = {}
 
                 for name in system_names:
                     if hasattr(data[name], 'ff_correction'):
-                        correction_ff[name] = compute_ff_correction(data[name].ff_correction, data[name].f, pars_ff)#, names_ff_pars)
-                        weights_P[name], logZ_P[name] = compute_new_weights(data[name].weights, correction_ff[name]/data[name].temperature)
-            
-                    else: # if beta is not infinite, but there are systems without force-field corrections:
+                        correction_ff[name] = compute_ff_correction(data[name].ff_correction, data[name].f, pars_ff)
+                        correction_ff[name] = correction_ff[name]/data[name].temperature
+                        weights_P[name], logZ_P[name] = compute_new_weights(data[name].weights, correction_ff[name])
+
+                    else:  # if beta is not infinite, but there are systems without force-field corrections:
                         weights_P[name] = data[name].weights
                         logZ_P[name] = 0
             else:
                 weights_P = {}
-                for name in system_names: weights_P[name] = data[name].weights
-            
-            ''' compute forward quantities through (new) forward coefficients theta'''
+                for name in system_names:
+                    weights_P[name] = data[name].weights
+
+            """ compute forward quantities through (new) forward coefficients theta"""
 
             pars_fm = pars_ff_fm[len(names_ff_pars):]
 
             g = {}
 
             if np.isinf(gamma):
-                
+
                 for name in system_names:
-                    if hasattr(data[name], 'g'): g[name] = copy.deepcopy(data[name].g)
+                    if hasattr(data[name], 'g'):
+                        g[name] = copy.deepcopy(data[name].g)
             else:
 
                 for name_sys in system_names:
-                    if hasattr(data[name_sys], 'g'): g[name_sys] = copy.deepcopy(data[name_sys].g)
-                    else: g[name_sys] = {}
+                    if hasattr(data[name_sys], 'g'):
+                        g[name_sys] = copy.deepcopy(data[name_sys].g)
+                    else:
+                        g[name_sys] = {}
 
-                    if hasattr(data[name_sys], 'selected_obs'): selected_obs = data[name_sys].selected_obs
-                    else: selected_obs = None
+                    if hasattr(data[name_sys], 'selected_obs'):
+                        selected_obs = data[name_sys].selected_obs
+                    else:
+                        selected_obs = None
 
                     fm_observables = data[name_sys].forward_model(pars_fm, data[name_sys].forward_qs, selected_obs)
 
-                    for name in fm_observables.keys(): g[name_sys][name] = fm_observables[name]
+                    for name in fm_observables.keys():
+                        g[name_sys][name] = fm_observables[name]
 
                     del fm_observables
 
-            ''' use observables in the initial format '''
+            """ use observables in the initial format """
             # for name_sys in system_names:
             #     for name in data[name_sys].ref.keys():
             #         if data[name_sys].ref[name] == '><':
             #             g[name_sys][name+' LOWER'] = g[name_sys][name]
             #             g[name_sys][name+' UPPER'] = g[name_sys][name]
             #             del g[name_sys][name]
 
-            ''' Compute derivatives and Hessian. '''
-            
+            """ Compute derivatives and Hessian. """
+
             for i_sys, name_sys in enumerate(system_names):
 
                 my_lambdas = lambdas[js[i_sys][0]:js[i_sys][-1]]
                 my_g = np.hstack([g[name_sys][k] for k in data[name_sys].n_experiments])
                 my_gexp = np.vstack([data[name_sys].gexp[k] for k in data[name_sys].n_experiments])
-                
+
                 my_args = (my_lambdas, my_g, my_gexp, weights_P[name_sys], alpha)
-                
+
                 Hess_inn_inv = np.linalg.inv(derivatives_funs.d2gamma_dlambdas2(*my_args))
 
-                derivatives.dlambdas_dlogalpha[name_sys] = -np.matmul(Hess_inn_inv, derivatives_funs.d2gamma_dlambdas_dalpha(*my_args))*alpha*np.log(10)
-                
-                matrix = d2loss_dpars_dlambdas[:,js[i_sys][0]:js[i_sys][-1]]
-                derivatives.dlambdas_dpars[name_sys] = +np.matmul(Hess_inn_inv, matrix.T)/alpha
-                terms.append(np.einsum('ij,jk,kl->il',matrix,Hess_inn_inv,matrix.T))
-                terms2.append(np.matmul(matrix,derivatives.dlambdas_dlogalpha[name_sys]))
+                derivatives.dlambdas_dlogalpha[name_sys] = -np.matmul(
+                    Hess_inn_inv, derivatives_funs.d2gamma_dlambdas_dalpha(*my_args))*alpha*np.log(10)
 
-            Hess = +np.sum(np.array(terms), axis = 0)/alpha + derivatives_funs.d2loss_dpars2(*args)
-            terms2 = np.sum(np.array(terms2), axis = 0)
+                matrix = d2loss_dpars_dlambdas[:, js[i_sys][0]:js[i_sys][-1]]
+                derivatives.dlambdas_dpars[name_sys] = +np.matmul(Hess_inn_inv, matrix.T)/alpha
+                terms.append(np.einsum('ij,jk,kl->il', matrix, Hess_inn_inv, matrix.T))
+                terms2.append(np.matmul(matrix, derivatives.dlambdas_dlogalpha[name_sys]))
 
-            # terms = []
+            Hess = +np.sum(np.array(terms), axis=0)/alpha + derivatives_funs.d2loss_dpars2(*args)
+            terms2 = np.sum(np.array(terms2), axis=0)
 
-            # ''' Here you can use either the derivatives of loss function or those of Gamma;
-            #     in both cases you have to compute ff re-weights and fm-updated observables;
-            #     if you use loss, this is already coded inside it, but it is repeated at any time you evaluate a derivative;
-            #     if you use Gamma, you would have to code it below inside for loop, and it would have computed just once. '''            
-            
-            # for i_sys,name_sys in enumerate(system_names):
-
-            #     lambdas_inn = np.array(lambdas[js[i_sys][0]:js[i_sys][-1]])
-                
-            #     ''' since you are evaluating the derivatives w.r.t. lambdas, you can omit regularization terms,
-            #         which do not depend on lambdas '''
-            #     my_dict = {name_sys: data[name_sys]}
-
-            #     args_inn = (pars_ff_fm, my_dict, None, alpha, 0, 0, lambdas_inn)
-
-            #     print(loss_function(*args))
-            #     print(loss_function(*args_inn))
-                
-            #     d2loss_dpars_dlambdas = derivatives_funs.d2loss_dpars_dlambdas(*args_inn)
-            #     inv_inn_Hess = np.linalg.inv(derivatives.d2loss_dlambdas2(*args_inn))
-            #     terms.append(np.einsum('ij,jk,kl->il', d2loss_dpars_dlambdas, inv_inn_Hess, d2loss_dpars_dlambdas.T))
-
-            #     ''' To compute the 2nd derivative of gamma w.r.t. lambdas, alpha, you can either:
-            #         - compute the 2nd derivative of gamma w.r.t. lambdas, alpha with Jax and then evaluate it at corresponding ff re-weights and fm-updated observables;
-            #         - exploit Gamma = -loss/alpha (loss includes calculation of ff re-weights and fm-updated observables). '''
-            #     derivatives.dlambdas_dlogalpha[name_sys] = -np.matmul(inv_inn_Hess, derivatives.d2loss_dlambdas_dalpha(*args_inn))*alpha*np.log(10)
-            #     terms2.append(np.matmul(d2loss_dpars_dlambdas,derivatives.dlambdas_dlogalpha[name_sys]))
-
-            #     derivatives.dlambdas_dpars[name_sys] = -np.matmul(inv_inn_Hess, d2loss_dpars_dlambdas.T)
-        
-            # Hess = np.sum(np.array(terms), axis = 0) + derivatives_funs.d2loss_dpars2(*args)
-            # terms2 = np.sum(np.array(terms2), axis = 0)
+        else:
+            Hess = derivatives_funs.d2loss_dpars2(*args)
 
-        else: Hess = derivatives_funs.d2loss_dpars2(*args)
-        
         inv_Hess = np.linalg.inv(Hess)
 
         if not np.isinf(alpha):
             d2loss_dpars_dlogalpha = derivatives_funs.d2loss_dpars_dalpha(*args)*alpha*np.log(10)
             derivatives.dpars_dlogalpha = -np.matmul(inv_Hess, d2loss_dpars_dlogalpha + terms2)
         if not np.isinf(beta):
             d2loss_dpars_dbeta = derivatives_funs.d2loss_dpars_dbeta(*args)
             derivatives.dpars_dlogbeta = -np.matmul(inv_Hess, d2loss_dpars_dbeta)*beta*np.log(10)
         if not np.isinf(gamma):
             d2loss_dpars_dgamma = derivatives_funs.d2loss_dpars_dgamma(*args)
             derivatives.dpars_dloggamma = -np.matmul(inv_Hess, d2loss_dpars_dgamma)*gamma*np.log(10)
-        
+
     return derivatives
 
-# %% D2. compute chi2 tot
+# %% D2. compute_chi2_tot
+
+
+"""
+Function **compute_chi2_tot** returns the total chi2 (float) for training or test data set, according to **which_set**
+(which_set = 'training' for chi2 on training set, 'validation' for chi2 on training observables but new frames,
+'test' for chi2 on test observables and new frames, through validation function).
+
+Input values:
+- pars_ff_fm, lambdas: np.arrays for (force-field + forward-model) parameters and lambdas parameters, respectively;
+- data: dict for data set;
+- regularization: dict for regularizations (see above);
+- alpha, beta, gamma: floats for hyperparameters;
+- which_set: str, as explained above.
+"""
+
 
 def compute_chi2_tot(pars_ff_fm, lambdas, data, regularization, alpha, beta, gamma, which_set):
 
     if which_set == 'training' or which_set == 'validation':
         tot_chi2 = 0
 
-        Details = loss_function(pars_ff_fm, data, regularization, alpha, beta, gamma, fixed_lambdas = lambdas, if_save = True)
+        Details = loss_function(pars_ff_fm, data, regularization, alpha, beta, gamma, fixed_lambdas=lambdas, if_save=True)
 
         for s1 in Details.chi2.keys():
-            for item in Details.chi2[s1].values(): tot_chi2 += item
-    
+            for item in Details.chi2[s1].values():
+                tot_chi2 += item
+
     elif which_set == 'test':
 
-        tot_chi2 = validation(pars_ff_fm, lambdas, data, regularization = regularization, alpha = alpha, beta = beta, gamma = gamma, which_return = 'test chi2')
+        tot_chi2 = validation(
+            pars_ff_fm, lambdas, data, regularization=regularization, alpha=alpha, beta=beta, gamma=gamma,
+            which_return='chi2 test')
 
     return tot_chi2
 
-# %% D3. put_together: apply chain rule to get derivatives of chi2 w.r.t hyper-parameters from
-# derivatives of chi2 w.r.t. parameters and derivatives of parameters w.r.t. hyper-parameters
+# %% D3. put_together
+
+
+""""
+Function **put_together** applies chain rule to get derivatives of chi2 w.r.t hyperparameters from
+derivatives of chi2 w.r.t. parameters and derivatives of parameters w.r.t. hyperparameters.
+
+Input values:
+- dchi2_dpars: np.array with derivatives of chi2 w.r.t. pars_ff_fm (force-field and forward-model parameters);
+- dchi2_dlambdas: np.array with derivatives of chi2 w.r.t. lambdas
+    (same order of lambdas in dchi2_dlambdas and in derivatives);
+- derivatives: class with derivatives of pars_ff_fm and lambdas w.r.t. hyperparameters
+    (determined in compute_hyperderivatives).
+
+Output: class whose attributes can include dchi2_dlogalpha, dchi2_dlogbeta, dchi2_dloggamma,
+depending on which hyperparameters are not fixed to infinite.
+"""
+
 
 def put_together(dchi2_dpars, dchi2_dlambdas, derivatives):
-    
-    class out_class: pass
+
+    class out_class:
+        pass
     out = out_class()
 
     if (dchi2_dpars is None) and (dchi2_dlambdas is not None):
         out.dchi2_dlogalpha = np.dot(dchi2_dlambdas, derivatives.dlambdas_dlogalpha)
 
     elif dchi2_dpars is not None:
-        
+
         vec = dchi2_dpars
 
         if dchi2_dlambdas is not None:
 
             vec += np.einsum('i,ij', dchi2_dlambdas, derivatives.dlambdas_dpars)
             temp = np.dot(dchi2_dlambdas, derivatives.dlambdas_dlogalpha)
 
@@ -2003,204 +2239,303 @@
         if hasattr(derivatives, 'dpars_dloggamma'):
             out.dchi2_dloggamma = np.dot(vec, derivatives.dpars_dloggamma)
 
     return out
 
 # %% D4. compute_hypergradient
 
-''' data_train is needed in all cases to compute derivatives of parameters w.r.t. hyper-parameters '''
 
-def compute_hypergradient(pars_ff_fm, lambdas, log10_alpha, log10_beta, log10_gamma, data_train, regularization, which_set, data_test, derivatives_funs):
+"""
+Function **compute_hypergradient** employs previously defined functions (compute_hyperderivatives, compute_chi2_tot,
+put_together) to return selected chi2 and its gradient w.r.t hyperparameters.
+
+Input values:
+- pars_ff_fm: np.array of (force-field and forward-model) parameters;
+- lambdas: dict of dicts with lambda coefficients;
+- log10_alpha, log10_beta, log10_gamma: floats for log (in base 10) of hyperparameters;
+- data_train: training data set, always required to compute derivatives of parameters w.r.t. hyper-parameters;
+- regularization: see above;
+- which_set: str, as explained for compute_chi2_tot;
+- data_test: test data set, required to compute chi2 on the test set (which_set = 'validation' or 'test')
+    (None if useless, namely for which_set = 'training');
+- derivatives_funs: derivative functions computed by Jax (they include those employed in compute_hyperderivatives
+    and dchi2_dpars and/or dchi2_dlambdas).
+"""
+
+
+def compute_hypergradient(
+        pars_ff_fm, lambdas, log10_alpha, log10_beta, log10_gamma, data_train, regularization,
+        which_set, data_test, derivatives_funs):
 
     system_names = data_train['global'].system_names
 
-    ''' compute derivatives of optimal pars w.r.t. hyper parameters '''
+    """ compute derivatives of optimal pars w.r.t. hyper parameters """
     if not np.isinf(log10_alpha):
         lambdas_vec = []
+        # refs = []
 
         for name_sys in system_names:
             for name in data_train[name_sys].n_experiments.keys():
                 lambdas_vec.append(lambdas[name_sys][name])
+                # refs.extend(data_train[name_sys].ref[name]*data_train[name_sys].n_experiments[name])
+
         lambdas_vec = np.concatenate((lambdas_vec))
-    else: lambdas_vec = None
-    
-    # use non-normalized data and lambdas
-    derivatives = compute_hyperderivatives(pars_ff_fm, lambdas_vec, data_train, regularization, log10_alpha, log10_beta, log10_gamma, derivatives_funs)
 
-    ''' compute chi2 and its derivatives w.r.t. pars'''
+        indices = np.nonzero(lambdas_vec)[0]
+        # indices = np.array([k for k in indices if not refs[k] == '='])  # indices of lambdas on constraints
+
+    else:
+        lambdas_vec = None
+
+    # use non-normalized data and lambdas
+    derivatives = compute_hyperderivatives(
+        pars_ff_fm, lambdas_vec, data_train, regularization, derivatives_funs, log10_alpha, log10_beta, log10_gamma)
 
-    # pars_lambdas = {'ff correction': {}, 'forward model': {}}
-    # for i,k in enumerate(names_ff_pars): pars_lambdas['ff correction'][k] = mini.x[i]
-    # for i,k in enumerate(my_data['global'].forward_coeffs_0.keys()): pars_lambdas['forward model'][k] = mini.x[i+len(names_ff_pars)]
+    """ compute chi2 and its derivatives w.r.t. pars"""
 
-    if which_set == 'training':  my_data = data_train
-    elif which_set == 'validation' or which_set == 'test': my_data = data_test
+    if which_set == 'training':
+        my_data = data_train
+    elif which_set == 'validation' or which_set == 'test':
+        my_data = data_test
     else:
         print('error on which_set')
         return
-    
-    my_args = (pars_ff_fm, lambdas_vec, my_data, regularization, 10**(log10_alpha), 10**(log10_beta), 10**(log10_gamma), which_set)
 
-    chi2 = compute_chi2_tot(*my_args) # so, lambdas follows order of system_names of my_data
+    my_args = (
+        pars_ff_fm, lambdas_vec, my_data, regularization, 10**(log10_alpha), 10**(log10_beta),
+        10**(log10_gamma), which_set)
+
+    chi2 = compute_chi2_tot(*my_args)  # so, lambdas follows order of system_names of my_data
 
-    if not (np.isinf(log10_beta) and np.isinf(log10_gamma)): dchi2_dpars = derivatives_funs.dchi2_dpars(*my_args)
-    else: dchi2_dpars = None
-    if not np.isinf(log10_alpha): dchi2_dlambdas = derivatives_funs.dchi2_dlambdas(*my_args)
-    else: dchi2_dlambdas = None
+    if not (np.isinf(log10_beta) and np.isinf(log10_gamma)):
+        dchi2_dpars = derivatives_funs.dchi2_dpars(*my_args)
+    else:
+        dchi2_dpars = None
+    if not np.isinf(log10_alpha):
+        dchi2_dlambdas = derivatives_funs.dchi2_dlambdas(*my_args)
+        dchi2_dlambdas = dchi2_dlambdas[indices]
+    else:
+        dchi2_dlambdas = None
 
-    ''' compute derivatives of chi2 w.r.t. hyper parameters (put together the previous two) '''
+    """ compute derivatives of chi2 w.r.t. hyper parameters (put together the previous two) """
 
     if hasattr(derivatives, 'dlambdas_dlogalpha'):
-        derivatives.dlambdas_dlogalpha = np.concatenate(([derivatives.dlambdas_dlogalpha[name_sys] for name_sys in system_names]))
+        derivatives.dlambdas_dlogalpha = np.concatenate(([
+            derivatives.dlambdas_dlogalpha[name_sys] for name_sys in system_names]))
     if hasattr(derivatives, 'dlambdas_dpars'):
-        derivatives.dlambdas_dpars = np.concatenate(([derivatives.dlambdas_dpars[name_sys] for name_sys in system_names]))
+        derivatives.dlambdas_dpars = np.concatenate(([
+            derivatives.dlambdas_dpars[name_sys] for name_sys in system_names]))
 
     gradient = put_together(dchi2_dpars, dchi2_dlambdas, derivatives)
 
-    return chi2,gradient
+    return chi2, gradient
 
-# %% D5. hyper_function: minimize loss function, compute chi2 and its gradient w.r.t hyper-parameters
-# at given hyper-parameters (alpha, beta, gamma)
+# %% D5. hyper_function
 
-def hyper_function(log10_hyperpars, map_hyperpars, data, regularization, test_obs, test_frames, which_set, derivatives_funs, starting_pars):
 
-    ''' 0. input values '''
+"""
+Function **hyper_function** determines optimal parameters by minimizing loss function at given hyperparameters;
+then, it computes chi2 and its gradient w.r.t hyperparameters (for the optimal parameters).
+
+Input values:
+- log10_hyperpars: np.array for log10 hyperparameters;
+- map_hyperpars: legend for log10_hyperparameters (they refer to alpha, beta, gamma in this order,
+    but some of them may not be present, if fixed to infinite);
+- data, regularization;
+- test_obs, test_frames: dicts of test observables and test frames indicized by seeds;
+- which_set: str (see for compute_chi2_tot);
+- derivatives_funs: derivative functions computed by Jax and employed in compute_hypergradient;
+- starting_pars: starting parameters, if user-defined; None otherwise.
+
+It returns:
+- tot_chi2: float for total chi2;
+- tot_gradient: np.array for gradient of total chi2 w.r.t hyperparameters;
+- Results: class of Results given by minimizer.
+
+Global: hyper_intermediate, in order to follow steps of minimization.
+"""
+
+
+def hyper_function(
+        log10_hyperpars, map_hyperpars, data, regularization, test_obs, test_frames, which_set, derivatives_funs,
+        starting_pars):
+
+    """ 0. input values """
 
     i = 0
     if 'alpha' in map_hyperpars:
         log10_alpha = log10_hyperpars[i]
         i += 1
-    else: log10_alpha = np.inf
+    else:
+        log10_alpha = np.inf
     if 'beta' in map_hyperpars:
         log10_beta = log10_hyperpars[i]
         i += 1
-    else: log10_beta = np.inf
+    else:
+        log10_beta = np.inf
     if 'gamma' in map_hyperpars:
         log10_gamma = log10_hyperpars[i]
-    else: log10_gamma = np.inf
+    else:
+        log10_gamma = np.inf
 
     print('\nlog10 hyperpars: ', [(map_hyperpars[i], log10_hyperpars[i]) for i in range(len(map_hyperpars))])
 
-    if not np.isinf(log10_alpha): alpha = np.float64(10**log10_alpha)
-    else: alpha = np.inf
+    if not np.isinf(log10_alpha):
+        alpha = np.float64(10**log10_alpha)
+    else:
+        alpha = np.inf
 
     names_ff_pars = []
-    
+
     if not np.isinf(log10_beta):
         beta = np.float64(10**log10_beta)
         names_ff_pars = data['global'].names_ff_pars
         pars0 = np.zeros(len(names_ff_pars))
     else:
         beta = np.inf
         pars0 = np.array([])
 
     if not np.isinf(log10_gamma):
         gamma = np.float64(10**log10_gamma)
         pars0 = np.concatenate(([pars0, np.array(data['global'].forward_coeffs_0)]))
-    else: gamma = np.inf
-        
-    ''' for each seed: '''
-    
+    else:
+        gamma = np.inf
+
+    """ for each seed: """
+
     Results = {}
     chi2 = []
-    gradient = [] # derivatives of chi2 w.r.t. (log10) hyper parameters
+    gradient = []  # derivatives of chi2 w.r.t. (log10) hyper parameters
 
     for seed in test_obs.keys():
 
-        ''' 2. minimize loss function on training set to get optimal parameters ''' 
+        """ 2. minimize loss function on training set to get optimal parameters """
 
-        out = select_traintest(data, test_frames = test_frames[seed], test_obs = test_obs[seed])
+        out = select_traintest(data, test_frames=test_frames[seed], test_obs=test_obs[seed])
         data_train = out[0]
         data_test = out[1]
 
-        mini = minimizer(data_train, regularization = regularization, alpha = alpha, beta = beta, gamma = gamma, starting_pars = starting_pars)
+        mini = minimizer(
+            data_train, regularization=regularization, alpha=alpha, beta=beta, gamma=gamma, starting_pars=starting_pars)
+
+        if hasattr(mini, 'pars'):
+            pars_ff_fm = mini.pars
+        else:
+            pars_ff_fm = None
+        if hasattr(mini, 'min_lambdas'):
+            lambdas = mini.min_lambdas
+        else:
+            lambdas = None
 
-        if hasattr(mini, 'pars'): pars_ff_fm = mini.pars
-        else: pars_ff_fm = None
-        if hasattr(mini, 'min_lambdas'): lambdas = mini.min_lambdas
-        else: lambdas = None
-        
         Results[seed] = mini
 
         # Details_train = loss_function(pars_ff_fm, data_train, regularization, alpha, beta, gamma, lambdas, if_save = True)
         # Details_test = loss_function(pars_ff_fm, data_test, regularization, alpha, beta, gamma, lambdas, if_save = True)
 
         # my_keys = [x for x in dir(Details_train) if not x.startswith('__')]
         # for k in my_keys: setattr(Results[seed], k+'_train', getattr(Details_train, k))
 
         # my_keys = [x for x in dir(Details_test) if not x.startswith('__')]
         # for k in my_keys: setattr(Results[seed], k+'_test', getattr(Details_test, k))
-        
-        out = compute_hypergradient(pars_ff_fm, lambdas, log10_alpha, log10_beta, log10_gamma, data_train, regularization, which_set, data_test, derivatives_funs)
+
+        out = compute_hypergradient(
+            pars_ff_fm, lambdas, log10_alpha, log10_beta, log10_gamma, data_train, regularization,
+            which_set, data_test, derivatives_funs)
+
         chi2.append(out[0])
         gradient.append(out[1])
 
     tot_chi2 = np.sum(np.array(chi2))
 
     tot_gradient = []
-    if 'alpha' in map_hyperpars: tot_gradient.append(np.sum(np.array([gradient[k].dchi2_dlogalpha for k in range(len(test_obs.keys()))])))
-    if 'beta' in map_hyperpars: tot_gradient.append(np.sum(np.array([gradient[k].dchi2_dlogbeta for k in range(len(test_obs.keys()))])))
-    if 'gamma' in map_hyperpars: tot_gradient.append(np.sum(np.array([gradient[k].dchi2_dloggamma for k in range(len(test_obs.keys()))])))
+
+    if 'alpha' in map_hyperpars:
+        tot_gradient.append(np.sum(np.array([gradient[k].dchi2_dlogalpha for k in range(len(test_obs.keys()))])))
+    if 'beta' in map_hyperpars:
+        tot_gradient.append(np.sum(np.array([gradient[k].dchi2_dlogbeta for k in range(len(test_obs.keys()))])))
+    if 'gamma' in map_hyperpars:
+        tot_gradient.append(np.sum(np.array([gradient[k].dchi2_dloggamma for k in range(len(test_obs.keys()))])))
 
     tot_gradient = np.array(tot_gradient)
 
     print('tot chi2: ', tot_chi2)
     print('tot gradient: ', tot_gradient)
 
     global hyper_intermediate
     hyper_intermediate.tot_chi2.append(tot_chi2)
     hyper_intermediate.tot_gradient.append(tot_gradient)
-    hyper_intermediate.log10_hyperpars.append(log10_hyperpars)#[log10_alpha,log10_beta,log10_gamma])
+    hyper_intermediate.log10_hyperpars.append(log10_hyperpars)
 
     return tot_chi2, tot_gradient, Results
 
-# %% D6. hyper_minimization: optimize hyper-parameters
+# %% D6. hyper_minimization
 
-def hyper_minimizer(data, starting_alpha = np.inf, starting_beta = np.inf, starting_gamma = np.inf, regularization = None, random_states = 1, which_set = 'validation', gtol = 0.5, starting_pars = None):
+
+"""
+This function **hyper_minimization** optimizes hyper-parameters by minimizing the selected chi2 (training, valdiation or test)
+over different splitting of the full data set into training/test set.
+
+Input values:
+- data: full data set;
+- starting_alpha, starting_beta, starting_gamma: float for starting point of respective hyperparameters
+    (np.inf by default, namely no refinement in that direction);
+- regularization (None by default);
+- random_states: used for select_traintest, it can be an integer (in this case, random_states = np.arange(random_states))
+    or a list of values;
+- which_set: str in 'training', 'validation', 'test' (as described in compute_chi2_tot) ('validation' by default);
+- gtol: float for tolerance of scipy.optimize.minimize (0.5 by default);
+- starting_pars: np.array of starting parameters pars_ff_fm for minimization (None by default).
+"""
+
+
+def hyper_minimizer(
+        data, starting_alpha=np.inf, starting_beta=np.inf, starting_gamma=np.inf, regularization=None,
+        random_states=1, which_set='validation', gtol=0.5, starting_pars=None):
 
     class hyper_intermediate_class():
         def __init__(self):
             self.tot_chi2 = []
             self.tot_gradient = []
             self.log10_hyperpars = []
 
     global hyper_intermediate
     hyper_intermediate = hyper_intermediate_class()
-    
-    if type(random_states) is int: random_states = np.arange(random_states)
 
-    ''' select training and test set (several seeds) '''
+    if type(random_states) is int:
+        random_states = np.arange(random_states)
+
+    """ select training and test set (several seeds) """
 
     test_obs = {}
     test_frames = {}
 
     for seed in random_states:
-        out = select_traintest(data, random_state = seed)
+        out = select_traintest(data, random_state=seed)
         test_obs[seed] = out[2]
         test_frames[seed] = out[3]
 
-    ''' derivatives '''
+    """ derivatives """
 
     class derivatives_funs_class:
         def __init__(self, loss_function, gamma_function):
             # self.dloss_dpars = gradient_fun
-            self.dloss_dpars = jax.grad(loss_function, argnums = 0)
-            self.d2loss_dpars2 = jax.hessian(loss_function, argnums = 0)
-            self.d2loss_dpars_dalpha = jax.jacfwd(self.dloss_dpars, argnums = 3)
-            self.d2loss_dpars_dbeta = jax.jacfwd(self.dloss_dpars, argnums = 4)
-            self.d2loss_dpars_dgamma = jax.jacfwd(self.dloss_dpars, argnums = 5)
+            self.dloss_dpars = jax.grad(loss_function, argnums=0)
+            self.d2loss_dpars2 = jax.hessian(loss_function, argnums=0)
+            self.d2loss_dpars_dalpha = jax.jacfwd(self.dloss_dpars, argnums=3)
+            self.d2loss_dpars_dbeta = jax.jacfwd(self.dloss_dpars, argnums=4)
+            self.d2loss_dpars_dgamma = jax.jacfwd(self.dloss_dpars, argnums=5)
 
             # self.d2loss_dlambdas2 = jax.hessian(loss_function, argnums = 6)
-            self.d2loss_dpars_dlambdas = jax.jacrev(self.dloss_dpars, argnums = 6)
-            self.dgamma_dlambdas = jax.grad(gamma_function, argnums = 0)
-            self.d2gamma_dlambdas_dalpha = jax.jacfwd(self.dgamma_dlambdas, argnums = 4)
-            self.d2gamma_dlambdas2 = jax.jacrev(self.dgamma_dlambdas, argnums = 0)
+            self.d2loss_dpars_dlambdas = jax.jacrev(self.dloss_dpars, argnums=6)
+            self.dgamma_dlambdas = jax.grad(gamma_function, argnums=0)
+            self.d2gamma_dlambdas_dalpha = jax.jacfwd(self.dgamma_dlambdas, argnums=4)
+            self.d2gamma_dlambdas2 = jax.jacrev(self.dgamma_dlambdas, argnums=0)
 
-            self.dchi2_dpars = jax.grad(compute_chi2_tot, argnums = 0)
-            self.dchi2_dlambdas = jax.grad(compute_chi2_tot, argnums = 1)
+            self.dchi2_dpars = jax.grad(compute_chi2_tot, argnums=0)
+            self.dchi2_dlambdas = jax.grad(compute_chi2_tot, argnums=1)
 
     derivatives_funs = derivatives_funs_class(loss_function, gamma_function)
 
     log10_hyperpars0 = []
     map_hyperpars = []
 
     if not np.isinf(starting_alpha):
@@ -2212,56 +2547,78 @@
     if not np.isinf(starting_gamma):
         log10_hyperpars0.append(np.log10(starting_gamma))
         map_hyperpars.append('gamma')
 
     # minimize
     args = (map_hyperpars, data, regularization, test_obs, test_frames, which_set, derivatives_funs, starting_pars)
 
-    # hyper_function(log10_hyperpars0, map_hyperpars, data, regularization, test_obs, test_frames, which_set, derivatives_funs, starting_pars)
+    hyper_mini = minimize(hyper_function, log10_hyperpars0, args=args, method='BFGS', jac=True, options={'gtol': gtol})
 
-    hyper_mini = minimize(hyper_function, log10_hyperpars0, args = args, method = 'BFGS', jac = True, options = {'gtol': gtol})#, 'maxfev': 20})#, 'ftol': 0.1})
-    
     hyper_intermediate.tot_chi2 = np.array(hyper_intermediate.tot_chi2)
     hyper_intermediate.tot_gradient = np.array(hyper_intermediate.tot_gradient)
     hyper_intermediate.log10_hyperpars = np.array(hyper_intermediate.log10_hyperpars)
     hyper_mini['intermediate'] = hyper_intermediate
 
     return hyper_mini
 
-# %% D7. MDRefinement: do all together
+# %% D7. MDRefinement
+
 
-def MDRefinement(infos, *, regularization = None, stride = 1, starting_alpha = np.inf, starting_beta = np.inf, starting_gamma = np.inf, random_states = 5, which_set = 'validation', gtol = 0.5):
+"""
+This function **MDRefinement** loads data, searches for the optimal hyperparameters and minimizes the whole data set
+using determined hyperparameters.
+
+Required inputs:
+- infos: dict of information to load data with load_data;
+- regularization: regularizations for force-field and forward-model corrections;
+- stride: int for stride used to load data employed in search for optimal hyperparameters
+    (for the final minimization full the whole set is employed);
+- starting_alpha, starting_beta, starting_gamma: floats for starting values of hyperparameters
+    (np.inf by default, namely no refinement in that direction);
+- random_states: see for hyper_minimizer (5 by default);
+- which_set: str in 'training', 'validation', 'test' (as described in compute_chi2_tot) ('validation' by default);
+- gtol: float for tolerance of scipy.optimize.minimize (0.5 by default).
+"""
+
+
+def MDRefinement(
+        infos: dict, *, regularization: dict = None, stride: int = 1,
+        starting_alpha: float = np.inf, starting_beta: float = np.inf, starting_gamma: float = np.inf,
+        random_states=5, which_set: str = 'validation', gtol: float = 0.5):
 
-    data = load_data(infos, stride = stride)
+    data = load_data(infos, stride=stride)
 
     print('\nsearch for optimal hyperparameters ...')
-    
+
     mini = hyper_minimizer(data, starting_alpha, starting_beta, starting_gamma, regularization, random_states, which_set, gtol)
     optimal_log10_hyperpars = mini.x
 
     i = 0
     s = ''
     if not np.isinf(starting_alpha):
         optimal_alpha = 10**optimal_log10_hyperpars[i]
         s = s + 'alpha: ' + str(optimal_alpha) + ' '
         i += 1
-    else: optimal_alpha = starting_alpha
+    else:
+        optimal_alpha = starting_alpha
     if not np.isinf(starting_beta):
         optimal_beta = 10**optimal_log10_hyperpars[i]
         s = s + 'beta: ' + str(optimal_beta) + ' '
         i += 1
-    else: optimal_beta = starting_beta
+    else:
+        optimal_beta = starting_beta
     if not np.isinf(starting_gamma):
         optimal_gamma = 10**optimal_log10_hyperpars[i]
         s = s + 'gamma: ' + str(optimal_gamma)
         # i += 1
-    else: optimal_gamma = starting_gamma
+    else:
+        optimal_gamma = starting_gamma
 
     print('\noptimal hyperparameters: ' + s)
     print('\nrefinement with optimal hyperparameters on the full data set')
-    
+
     # for the minimization with optimal hyper-parameters use full data set
     data = load_data(infos)
 
-    Result = minimizer(data, regularization = regularization, alpha = optimal_alpha, beta = optimal_beta, gamma = optimal_gamma)
+    Result = minimizer(data, regularization=regularization, alpha=optimal_alpha, beta=optimal_beta, gamma=optimal_gamma)
 
     return Result
```

### Comparing `MDRefine-0.0.3/MDRefine.egg-info/PKG-INFO` & `mdrefine-0.0.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1
-Name: MDRefine
-Version: 0.0.3
-Summary: A package to perform refinement of MD simulation trajectories.
-Home-page: https://github.com/bussilab/MDRefine
-Author: Ivan Gilardoni
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 [![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/bussilab/MDRefine)](https://github.com/bussilab/MDRefine/tags)
 [![PyPI](https://img.shields.io/pypi/v/MDRefine)](https://pypi.org/project/MDRefine/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/MDRefine)](https://pypi.org/project/MDRefine/)
 [![CI](https://github.com/bussilab/MDRefine/workflows/CI/badge.svg)](https://github.com/bussilab/MDRefine/actions?query=workflow%3ACI)
 
-A package to perform refinement of MD simulation trajectories
+A package to perform refinement of MD simulation trajectories.
+
+To install package and dependencies with pip (version from PyPI):
+
+```
+pip install bussilab
+```
+
+You can install the development version by cloning the repository and, from its root directory, type:
+
+```
+pip install -e .
+```
+
+**Note that this is still at development stage, so also the version from PyPI is not expected to be stable yet**
```

### Comparing `MDRefine-0.0.3/setup.py` & `mdrefine-0.0.6/setup.py`

 * *Files identical despite different names*

