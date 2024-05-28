# Comparing `tmp/theborg-1.0.6.tar.gz` & `tmp/theborg-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/theborg-1.0.6.tar", last modified: Thu Sep 28 19:34:50 2023, max compression
+gzip compressed data, was "theborg-1.0.7.tar", last modified: Tue May 28 17:13:53 2024, max compression
```

## Comparing `theborg-1.0.6.tar` & `theborg-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-09-28 19:34:50.000000 theborg-1.0.6/
--rw-r--r--   0 nidever    (503) staff       (20)     1070 2021-12-05 18:48:40.000000 theborg-1.0.6/LICENSE
--rw-r--r--   0 nidever    (503) staff       (20)       32 2021-12-07 04:32:15.000000 theborg-1.0.6/MANIFEST.in
--rw-r--r--   0 nidever    (503) staff       (20)     1046 2023-09-28 19:34:50.000000 theborg-1.0.6/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)      694 2021-12-07 04:44:59.000000 theborg-1.0.6/README.rst
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-09-28 19:34:50.000000 theborg-1.0.6/docs/
--rw-r--r--   0 nidever    (503) staff       (20)      634 2021-02-16 20:03:42.000000 theborg-1.0.6/docs/Makefile
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-09-28 19:34:50.000000 theborg-1.0.6/docs/_static/
--rw-r--r--   0 nidever    (503) staff       (20)      331 2021-02-17 00:02:55.000000 theborg-1.0.6/docs/_static/theborg.css
--rw-r--r--   0 nidever    (503) staff       (20)     7899 2021-12-07 04:46:48.000000 theborg-1.0.6/docs/conf.py
--rw-r--r--   0 nidever    (503) staff       (20)      292 2021-12-10 07:00:20.000000 theborg-1.0.6/docs/examples.rst
--rw-r--r--   0 nidever    (503) staff       (20)     3089 2021-12-10 21:19:35.000000 theborg-1.0.6/docs/gettingstarted.rst
--rw-r--r--   0 nidever    (503) staff       (20)      589 2021-12-10 05:04:55.000000 theborg-1.0.6/docs/index.rst
--rw-r--r--   0 nidever    (503) staff       (20)      436 2021-12-10 05:06:43.000000 theborg-1.0.6/docs/install.rst
--rw-r--r--   0 nidever    (503) staff       (20)      795 2021-02-16 20:03:42.000000 theborg-1.0.6/docs/make.bat
--rw-r--r--   0 nidever    (503) staff       (20)       58 2021-12-07 05:10:12.000000 theborg-1.0.6/docs/modules.rst
--rw-r--r--   0 nidever    (503) staff       (20)       69 2021-02-17 00:38:10.000000 theborg-1.0.6/docs/requirements.txt
--rw-r--r--   0 nidever    (503) staff       (20)      806 2021-12-10 06:57:31.000000 theborg-1.0.6/docs/theborg.rst
--rw-r--r--   0 nidever    (503) staff       (20)      149 2021-12-07 04:32:31.000000 theborg-1.0.6/environment.yml
--rw-r--r--   0 nidever    (503) staff       (20)       49 2021-12-07 04:29:20.000000 theborg-1.0.6/requirements-dev.txt
--rw-r--r--   0 nidever    (503) staff       (20)       48 2021-12-07 04:32:45.000000 theborg-1.0.6/requirements.txt
--rw-r--r--   0 nidever    (503) staff       (20)     1178 2023-09-28 19:34:50.000000 theborg-1.0.6/setup.cfg
--rw-r--r--   0 nidever    (503) staff       (20)      537 2023-09-28 19:34:48.000000 theborg-1.0.6/setup.py
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-09-28 19:34:50.000000 theborg-1.0.6/theborg/
--rw-r--r--   0 nidever    (503) staff       (20)       66 2023-09-28 19:34:45.000000 theborg-1.0.6/theborg/__init__.py
--rw-r--r--   0 nidever    (503) staff       (20)    15349 2021-12-10 06:44:06.000000 theborg-1.0.6/theborg/classifier.py
--rw-r--r--   0 nidever    (503) staff       (20)     3373 2023-05-19 16:01:04.000000 theborg-1.0.6/theborg/emulator.py
--rw-r--r--   0 nidever    (503) staff       (20)    26082 2023-09-28 19:34:41.000000 theborg-1.0.6/theborg/model.py
--rw-r--r--   0 nidever    (503) staff       (20)     8190 2021-12-05 23:04:59.000000 theborg-1.0.6/theborg/radam.py
-drwxr-xr-x   0 nidever    (503) staff       (20)        0 2023-09-28 19:34:50.000000 theborg-1.0.6/theborg.egg-info/
--rw-r--r--   0 nidever    (503) staff       (20)     1046 2023-09-28 19:34:49.000000 theborg-1.0.6/theborg.egg-info/PKG-INFO
--rw-r--r--   0 nidever    (503) staff       (20)      579 2023-09-28 19:34:49.000000 theborg-1.0.6/theborg.egg-info/SOURCES.txt
--rw-r--r--   0 nidever    (503) staff       (20)        1 2023-09-28 19:34:49.000000 theborg-1.0.6/theborg.egg-info/dependency_links.txt
--rw-r--r--   0 nidever    (503) staff       (20)        1 2023-09-28 19:34:49.000000 theborg-1.0.6/theborg.egg-info/not-zip-safe
--rw-r--r--   0 nidever    (503) staff       (20)      156 2023-09-28 19:34:49.000000 theborg-1.0.6/theborg.egg-info/requires.txt
--rw-r--r--   0 nidever    (503) staff       (20)        8 2023-09-28 19:34:49.000000 theborg-1.0.6/theborg.egg-info/top_level.txt
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2024-05-28 17:13:53.842494 theborg-1.0.7/
+-rw-r--r--   0 nidever    (503) staff       (20)      818 2024-03-27 15:31:13.000000 theborg-1.0.7/.readthedocs.yaml
+-rw-r--r--   0 nidever    (503) staff       (20)     1070 2021-12-05 18:48:40.000000 theborg-1.0.7/LICENSE
+-rw-r--r--   0 nidever    (503) staff       (20)       32 2021-12-07 04:32:15.000000 theborg-1.0.7/MANIFEST.in
+-rw-r--r--   0 nidever    (503) staff       (20)     1534 2024-05-28 17:13:53.842271 theborg-1.0.7/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)      694 2021-12-07 04:44:59.000000 theborg-1.0.7/README.rst
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2024-05-28 17:13:53.831992 theborg-1.0.7/docs/
+-rw-r--r--   0 nidever    (503) staff       (20)      634 2021-02-16 20:03:42.000000 theborg-1.0.7/docs/Makefile
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2024-05-28 17:13:53.832794 theborg-1.0.7/docs/_static/
+-rw-r--r--   0 nidever    (503) staff       (20)      331 2021-02-17 00:02:55.000000 theborg-1.0.7/docs/_static/theborg.css
+-rw-r--r--   0 nidever    (503) staff       (20)     7981 2024-03-27 15:37:06.000000 theborg-1.0.7/docs/conf.py
+-rw-r--r--   0 nidever    (503) staff       (20)      292 2021-12-10 07:00:20.000000 theborg-1.0.7/docs/examples.rst
+-rw-r--r--   0 nidever    (503) staff       (20)     3089 2021-12-10 21:19:35.000000 theborg-1.0.7/docs/gettingstarted.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      589 2021-12-10 05:04:55.000000 theborg-1.0.7/docs/index.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      436 2021-12-10 05:06:43.000000 theborg-1.0.7/docs/install.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      795 2021-02-16 20:03:42.000000 theborg-1.0.7/docs/make.bat
+-rw-r--r--   0 nidever    (503) staff       (20)       58 2021-12-07 05:10:12.000000 theborg-1.0.7/docs/modules.rst
+-rw-r--r--   0 nidever    (503) staff       (20)       70 2024-03-27 15:31:21.000000 theborg-1.0.7/docs/requirements.txt
+-rw-r--r--   0 nidever    (503) staff       (20)      806 2021-12-10 06:57:31.000000 theborg-1.0.7/docs/theborg.rst
+-rw-r--r--   0 nidever    (503) staff       (20)      149 2021-12-07 04:32:31.000000 theborg-1.0.7/environment.yml
+-rw-r--r--   0 nidever    (503) staff       (20)       49 2021-12-07 04:29:20.000000 theborg-1.0.7/requirements-dev.txt
+-rw-r--r--   0 nidever    (503) staff       (20)       48 2021-12-07 04:32:45.000000 theborg-1.0.7/requirements.txt
+-rw-r--r--   0 nidever    (503) staff       (20)     1178 2024-05-28 17:13:53.843484 theborg-1.0.7/setup.cfg
+-rw-r--r--   0 nidever    (503) staff       (20)      537 2024-05-28 17:13:52.000000 theborg-1.0.7/setup.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2024-05-28 17:13:53.836404 theborg-1.0.7/theborg/
+-rw-r--r--   0 nidever    (503) staff       (20)       66 2024-05-28 17:13:48.000000 theborg-1.0.7/theborg/__init__.py
+-rw-r--r--   0 nidever    (503) staff       (20)    15349 2021-12-10 06:44:06.000000 theborg-1.0.7/theborg/classifier.py
+-rw-r--r--   0 nidever    (503) staff       (20)     3487 2024-01-30 14:54:58.000000 theborg-1.0.7/theborg/emulator.py
+-rw-r--r--   0 nidever    (503) staff       (20)    26251 2024-01-30 14:54:58.000000 theborg-1.0.7/theborg/model.py
+-rw-r--r--   0 nidever    (503) staff       (20)     8190 2021-12-05 23:04:59.000000 theborg-1.0.7/theborg/radam.py
+drwxr-xr-x   0 nidever    (503) staff       (20)        0 2024-05-28 17:13:53.840181 theborg-1.0.7/theborg.egg-info/
+-rw-r--r--   0 nidever    (503) staff       (20)     1534 2024-05-28 17:13:53.000000 theborg-1.0.7/theborg.egg-info/PKG-INFO
+-rw-r--r--   0 nidever    (503) staff       (20)      597 2024-05-28 17:13:53.000000 theborg-1.0.7/theborg.egg-info/SOURCES.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        1 2024-05-28 17:13:53.000000 theborg-1.0.7/theborg.egg-info/dependency_links.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        1 2024-05-28 17:13:53.000000 theborg-1.0.7/theborg.egg-info/not-zip-safe
+-rw-r--r--   0 nidever    (503) staff       (20)      156 2024-05-28 17:13:53.000000 theborg-1.0.7/theborg.egg-info/requires.txt
+-rw-r--r--   0 nidever    (503) staff       (20)        8 2024-05-28 17:13:53.000000 theborg-1.0.7/theborg.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `theborg-1.0.6/LICENSE` & `theborg-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/README.rst` & `theborg-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/docs/Makefile` & `theborg-1.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/docs/conf.py` & `theborg-1.0.7/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,22 +74,23 @@
 copyright = '{0}, {1}'.format(
     datetime.datetime.now().year, setup_cfg['author'])
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 
-import_module(setup_cfg['name'])
-package = sys.modules[setup_cfg['name']]
+#import_module(setup_cfg['name'])
+#package = sys.modules[setup_cfg['name']]
 
 # The short X.Y version.
-version = package.__version__.split('-', 1)[0]
+#version = package.__version__.split('-', 1)[0]
+version = setup_cfg['version'].split('-', 1)[0]
 # The full version, including alpha/beta/rc tags.
-release = package.__version__
-
+#release = package.__version__
+release = setup_cfg['version']
 
 # -- Options for HTML output --------------------------------------------------
 
 # A NOTE ON HTML THEMES
 # The global astropy configuration uses a custom theme, 'bootstrap-astropy',
 # which is installed along with astropy. A different theme can be used or
 # the options for this theme can be modified by overriding some of the
```

### Comparing `theborg-1.0.6/docs/gettingstarted.rst` & `theborg-1.0.7/docs/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/docs/index.rst` & `theborg-1.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/docs/make.bat` & `theborg-1.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/docs/theborg.rst` & `theborg-1.0.7/docs/theborg.rst`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/setup.cfg` & `theborg-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 license_file = LICENSE
 url = https://github.com/dnidever/theborg
 description = Artificial Neural Network routines
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 edit_on_github = False
 github_project = dnidever/theborg
-version = 1.0.6
+version = 1.0.7
 
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.6
 setup_requires = 
 	setuptools_scm
```

### Comparing `theborg-1.0.6/setup.py` & `theborg-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 #from distutils.core import setup
 from setuptools import setup, find_packages
 
 setup(name='theborg',
-      version='1.0.6',
+      version='1.0.7',
       description='Artificial Neural Network routines',
       author='David Nidever, Yuan-Sen Ting',
       author_email='dnidever@montana.edu',
       url='https://github.com/dnidever/theborg',
       packages=find_packages(exclude=["tests"]),
       #scripts=['bin/doppler'],
       install_requires=['numpy','astropy(>=4.0)','scipy','dlnpyutils(>=1.0.3)']
```

### Comparing `theborg-1.0.6/theborg/classifier.py` & `theborg-1.0.7/theborg/classifier.py`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/theborg/emulator.py` & `theborg-1.0.7/theborg/emulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 
 #===================================================================================================
 # simple multi-layer perceptron model
 class EmulatorModel(torch.nn.Module):
     def __init__(self, dim_in, num_neurons, num_features):
         super(EmulatorModel, self).__init__()
+        if type(num_neurons) is list or type(num_neurons) is np.ndarray:
+            num_neurons = num_neurons[0]
         self.features = torch.nn.Sequential(
             torch.nn.Linear(dim_in, num_neurons),
             torch.nn.LeakyReLU(),
             torch.nn.Linear(num_neurons, num_neurons),
             torch.nn.LeakyReLU(),
             torch.nn.Linear(num_neurons, num_features),
         )
```

### Comparing `theborg-1.0.6/theborg/model.py` & `theborg-1.0.7/theborg/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,31 @@
 from . import radam
 
 
 # simple multi-layer perceptron model
 class SimpleModel(torch.nn.Module):
     def __init__(self, dim_in, num_neurons, num_features):
         super(SimpleModel, self).__init__()
+        if type(num_neurons) is list or type(num_neurons) is np.ndarray:
+             num_neurons = num_neurons[0]
         self.features = torch.nn.Sequential(
             torch.nn.Linear(dim_in, num_neurons),
             torch.nn.LeakyReLU(),
             torch.nn.Linear(num_neurons, num_neurons),
             torch.nn.LeakyReLU(),
             torch.nn.Linear(num_neurons, num_features),
         )
 
     def forward(self, x):
         return self.features(x)
 
 class MultiModel(torch.nn.Module):
     def __init__(self, dim_in, num_neurons, num_features):
         super(MultiModel, self).__init__()
-        if type(num_neurons) is int:
-            num_neurons = [num_neurons]
+        num_neurons = np.atleast_1d(num_neurons)
         flist = [torch.nn.Linear(dim_in, num_neurons[0]),torch.nn.LeakyReLU()]
         for i in range(len(num_neurons)):
             if i==len(num_neurons)-1:
                 flist.append(torch.nn.Linear(num_neurons[i], num_neurons[i]))
             else:
                 flist.append(torch.nn.Linear(num_neurons[i], num_neurons[i+1]))                
             flist.append(torch.nn.LeakyReLU())            
@@ -48,22 +49,23 @@
     def forward(self, x):
         return self.features(x)
 
     
 class Model(object):
     def __init__(self, dim_in=4, num_neurons=100, num_features=500, training_data=None, training_labels=None,
                  learning_rate=1e-4,batch_size=200,label_names=None):
-        if type(num_neurons) is int:
-            self.model = SimpleModel(dim_in, num_neurons, num_features)
+        num_neurons = np.atleast_1d(num_neurons)
+        if len(num_neurons)==1:
+            self.model = SimpleModel(dim_in, num_neurons[0], num_features)
             self.nhiddenlayers = 1
         else:
             self.model = MultiModel(dim_in, num_neurons, num_features)
-            self.nhiddenlayers = len(num_neurons)            
+            self.nhiddenlayers = len(num_neurons)
+        self.num_neurons = num_neurons            
         self.dim_in = dim_in
-        self.num_neurons = num_neurons
         self.num_features = num_features
         self.nlayers = self.nhiddenlayers+2
         self.xmin = None
         self.xmax = None
         self.num_labels = None
         if training_labels is not None:
             if np.array(training_labels).ndim != 2:
@@ -80,15 +82,15 @@
         self.label_names = label_names
         self.training_loss = []
         self.validation_loss = []
         self.training_data = training_data
         self.training_labels = training_labels
         self._best_state_dict = None
         self._hull = None
-
+        
     @property
     def device(self):
         """ Returns the device that the data is located on."""
         key0 = list(self.model.state_dict())[0]
         if key0 is not None:
             return self.model.state_dict()[key0].device
         else:
@@ -171,15 +173,15 @@
             raise ValueError(str(len(labels))+' input and expected '+str(self.num_labels))
         
         ## Input labels should be unscaled
         scaled_labels = self.scaled_labels(labels)
         
         # Check that the input labels are inside the trained parameters space
         inside = True
-        clip_labels = labels.copy()
+        clip_labels = np.atleast_1d(labels).copy()
         for i in range(self.num_labels):
             inside1 = (labels[i]>=self.xmin[i]) and (labels[i]<=self.xmax[i])
             if inside1 == False:
                 clip_labels[i] = np.minimum(np.maximum(labels[i],self.xmin[i]),self.xmax[i])
                 error = 'Input labels are outside the trained parameter space.'
                 error += ' Label {:d} = {:.3f} outside [{:.3f} to {:.3f}]'.format(i,labels[i],self.xmin[i],self.xmax[i])
             inside = inside and inside1
@@ -242,16 +244,16 @@
         # change to device value input
         if device is not None:
             for k in list(sd.keys()):
                 sd[k] = sd[k].to(device)
         newself.model.load_state_dict(sd)        
         return newself
         
-    def write(self,outfile,npz=False):
-        self.save(outfile,npz=npz)
+    def write(self,outfile,**kwargs):
+        self.save(outfile,**kwargs)
     
     def save(self,outfile,npz=False,nodata=False):
         """ Write the model to a file."""
         # save parameters and remember how we scaled the labels
         if npz:
             outdict = self.model.state_dict().copy()
             outdict['xmin'] = self.xmin
@@ -463,15 +465,15 @@
             vsi = np.arange(ndata)
             np.random.shuffle(vsi)   # shuffle
             vsi = vsi[0:int(np.round(validation_split*ndata))]  # only want validation_split
             vind = ind[vsi]
             ind = np.delete(ind,vsi)   # remove these from the training set
             validation_data = training_data[vind,:] 
             validation_labels = training_labels[vind,:]
-
+            
         # Re-initialize the model and trained data and history
         self.model = self.model.__class__(num_labels, num_neurons, num_features)
         #self.model = EmulatorModel(num_labels, num_neurons, num_features)
         self.num_labels = num_labels
         self.num_features = num_features
         self.num_neurons = num_neurons
         self.learning_rate = learning_rate
```

### Comparing `theborg-1.0.6/theborg/radam.py` & `theborg-1.0.7/theborg/radam.py`

 * *Files identical despite different names*

### Comparing `theborg-1.0.6/theborg.egg-info/SOURCES.txt` & `theborg-1.0.7/theborg.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.rst
 environment.yml
 requirements-dev.txt
 requirements.txt
 setup.cfg
```

