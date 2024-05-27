# Comparing `tmp/pysembrane-0.0.1.tar.gz` & `tmp/pysembrane-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysembrane-0.0.1.tar", last modified: Wed Mar  6 01:33:03 2024, max compression
+gzip compressed data, was "pysembrane-0.0.2.tar", last modified: Mon May 27 22:17:03 2024, max compression
```

## Comparing `pysembrane-0.0.1.tar` & `pysembrane-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-06 01:33:03.481368 pysembrane-0.0.1/
--rw-rw-rw-   0        0        0      366 2024-03-06 01:33:03.480372 pysembrane-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       17 2024-02-27 05:13:45.000000 pysembrane-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-06 01:33:03.458767 pysembrane-0.0.1/pySembrane/
--rw-rw-rw-   0        0        0        0 2024-03-06 01:32:13.000000 pysembrane-0.0.1/pySembrane/__init__.py
--rw-rw-rw-   0        0        0     2014 2024-02-27 06:42:10.000000 pysembrane-0.0.1/pySembrane/calculator.py
--rw-rw-rw-   0        0        0    32030 2024-02-27 06:42:11.000000 pysembrane-0.0.1/pySembrane/simulator.py
-drwxrwxrwx   0        0        0        0 2024-03-06 01:33:03.477385 pysembrane-0.0.1/pysembrane.egg-info/
--rw-rw-rw-   0        0        0      366 2024-03-06 01:33:03.000000 pysembrane-0.0.1/pysembrane.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-03-06 01:33:03.000000 pysembrane-0.0.1/pysembrane.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-06 01:33:03.000000 pysembrane-0.0.1/pysembrane.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-03-06 01:33:03.000000 pysembrane-0.0.1/pysembrane.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-06 01:33:03.000000 pysembrane-0.0.1/pysembrane.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-06 01:33:03.482364 pysembrane-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      939 2024-03-06 01:28:27.000000 pysembrane-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:03.387622 pysembrane-0.0.2/
+-rw-rw-rw-   0        0        0      366 2024-05-27 22:17:03.386627 pysembrane-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2024-02-27 05:13:45.000000 pysembrane-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:03.371693 pysembrane-0.0.2/pySembrane/
+-rw-rw-rw-   0        0        0        0 2024-03-06 01:32:13.000000 pysembrane-0.0.2/pySembrane/__init__.py
+-rw-rw-rw-   0        0        0     2014 2024-02-27 06:42:10.000000 pysembrane-0.0.2/pySembrane/calculator.py
+-rw-rw-rw-   0        0        0    32008 2024-05-23 05:31:48.000000 pysembrane-0.0.2/pySembrane/simulator.py
+drwxrwxrwx   0        0        0        0 2024-05-27 22:17:03.382645 pysembrane-0.0.2/pysembrane.egg-info/
+-rw-rw-rw-   0        0        0      366 2024-05-27 22:17:03.000000 pysembrane-0.0.2/pysembrane.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2024-05-27 22:17:03.000000 pysembrane-0.0.2/pysembrane.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 22:17:03.000000 pysembrane-0.0.2/pysembrane.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-27 22:17:03.000000 pysembrane-0.0.2/pysembrane.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 22:17:03.000000 pysembrane-0.0.2/pysembrane.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 22:17:03.388618 pysembrane-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      939 2024-05-23 05:31:20.000000 pysembrane-0.0.2/setup.py
```

### Comparing `pysembrane-0.0.1/pySembrane/calculator.py` & `pysembrane-0.0.2/pySembrane/calculator.py`

 * *Files identical despite different names*

### Comparing `pysembrane-0.0.1/pySembrane/simulator.py` & `pysembrane-0.0.2/pySembrane/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,14 @@
                 else:
                     err = [(ffp-_factor*(J[ii,0]))/ffp for ii, ffp in enumerate(fp_0_i)]
                 err_pp = (1-Pp[-1])/Pp[-1]
                 err.append(err_pp) 
             
             tol = sum([abs(_err) for _err in err])
         
-            Kg = 0.1
             for jj, _err in enumerate(err):
                 if jj < self._n_comp:
                     fp_0_i[jj] = fp_0_i[jj]-Kg*_err*fp_0_i[jj]
                 else:
                     self._Pp_in = self._Pp_in + Kg*_err*Pp[-1]
             self._y0 = np.array(list(self._Ff_in) +list(fp_0_i)+ [self._Pf_in, self._Pp_in])                
             if abs(tol) < tolerance:
```

### Comparing `pysembrane-0.0.1/setup.py` & `pysembrane-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
         name='pysembrane',
-        version='0.0.1',
+        version='0.0.2',
         author_email='sgasga@ulsan.ac.kr',
         description='Python package for membrane based gas separation process simulations',
         long_description_content_type='text/markdown',
         url='https://nahyeonan.github.io/pySembrane',
         packages=setuptools.find_packages(),
         classifieres=[
             'Programming Language :: Python :: 3',
```

