# Comparing `tmp/pytuflow-0.0.8.tar.gz` & `tmp/pytuflow-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pytuflow-0.0.8.tar", last modified: Mon Feb 10 04:50:14 2020, max compression
+gzip compressed data, was "dist\pytuflow-0.0.9.tar", last modified: Mon Feb 17 05:27:04 2020, max compression
```

## Comparing `pytuflow-0.0.8.tar` & `pytuflow-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2020-02-10 04:50:14.000000 pytuflow-0.0.8/
--rw-rw-rw-   0        0        0      850 2020-02-10 04:50:14.000000 pytuflow-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      256 2019-02-11 09:22:02.000000 pytuflow-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-02-10 04:50:14.000000 pytuflow-0.0.8/pytuflow/
--rw-rw-rw-   0        0        0    35774 2020-02-10 01:50:41.000000 pytuflow-0.0.8/pytuflow/TUFLOW.py
--rw-rw-rw-   0        0        0   198277 2019-12-06 05:50:02.000000 pytuflow-0.0.8/pytuflow/TUFLOW_results.py
--rw-rw-rw-   0        0        0    33318 2019-02-08 01:19:20.000000 pytuflow-0.0.8/pytuflow/TUFLOW_results2013.py
--rw-rw-rw-   0        0        0       65 2019-02-11 09:22:31.000000 pytuflow-0.0.8/pytuflow/__init__.py
--rw-rw-rw-   0        0        0     3603 2019-02-07 08:56:06.000000 pytuflow-0.0.8/pytuflow/helper.py
-drwxrwxrwx   0        0        0        0 2020-02-10 04:50:14.000000 pytuflow-0.0.8/pytuflow.egg-info/
--rw-rw-rw-   0        0        0      850 2020-02-10 04:50:13.000000 pytuflow-0.0.8/pytuflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2020-02-10 04:50:13.000000 pytuflow-0.0.8/pytuflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-02-10 04:50:13.000000 pytuflow-0.0.8/pytuflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2020-02-10 04:50:13.000000 pytuflow-0.0.8/pytuflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-02-10 04:50:14.000000 pytuflow-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      734 2020-02-10 01:46:06.000000 pytuflow-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-02-17 05:27:04.000000 pytuflow-0.0.9/
+-rw-rw-rw-   0        0        0      850 2020-02-17 05:27:04.000000 pytuflow-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2019-02-11 09:22:02.000000 pytuflow-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-02-17 05:27:04.000000 pytuflow-0.0.9/pytuflow/
+-rw-rw-rw-   0        0        0    35746 2020-02-17 05:13:14.000000 pytuflow-0.0.9/pytuflow/TUFLOW.py
+-rw-rw-rw-   0        0        0   198482 2020-02-17 05:24:33.000000 pytuflow-0.0.9/pytuflow/TUFLOW_results.py
+-rw-rw-rw-   0        0        0    33318 2019-02-08 01:19:20.000000 pytuflow-0.0.9/pytuflow/TUFLOW_results2013.py
+-rw-rw-rw-   0        0        0       65 2019-02-11 09:22:31.000000 pytuflow-0.0.9/pytuflow/__init__.py
+-rw-rw-rw-   0        0        0     3603 2019-02-07 08:56:06.000000 pytuflow-0.0.9/pytuflow/helper.py
+drwxrwxrwx   0        0        0        0 2020-02-17 05:27:04.000000 pytuflow-0.0.9/pytuflow.egg-info/
+-rw-rw-rw-   0        0        0      850 2020-02-17 05:27:04.000000 pytuflow-0.0.9/pytuflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2020-02-17 05:27:04.000000 pytuflow-0.0.9/pytuflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-02-17 05:27:04.000000 pytuflow-0.0.9/pytuflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2020-02-17 05:27:04.000000 pytuflow-0.0.9/pytuflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-02-17 05:27:04.000000 pytuflow-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      734 2020-02-17 05:23:28.000000 pytuflow-0.0.9/setup.py
```

### Comparing `pytuflow-0.0.8/PKG-INFO` & `pytuflow-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytuflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for scripting TUFLOW time series results.
 Home-page: https://github.com/TUFLOW-Support/PyTuflow
 Author: tuflowsupport
 Author-email: support@tuflow.com
 License: UNKNOWN
 Description: # PyTuflow
```

### Comparing `pytuflow-0.0.8/pytuflow/TUFLOW.py` & `pytuflow-0.0.9/pytuflow/TUFLOW.py`

 * *Files 0% similar despite different names*

```diff
@@ -868,15 +868,15 @@
                     return self._res.LP.dist_chan_inverts[:], self._res.LP.tHmax[:]
             
         return [], []
 
 
 if __name__ == "__main__":
     # debugging
-    tpc = r"C:\_TT_Training\Completed_Models\TUFLOW\results\plot\TUT_5m_011.tpc"
+    tpc = r"D:\plot\TUT_5m_002_HPC+QuadTree+SGS.tpc"
     res = ResData()
     err, mess = res.load(tpc)
     if err:
         print(mess)
     err, mess, qmax = res.maximum("Pit1", "Q")
     if err:
         print(mess)
```

### Comparing `pytuflow-0.0.8/pytuflow/TUFLOW_results.py` & `pytuflow-0.0.9/pytuflow/TUFLOW_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,16 +244,16 @@
     def load(self, fullpath, prefix, simID):
         error = False
         message = ''
         try:
             with open(fullpath, 'r') as csvfile:
                 reader = csv.reader(csvfile, delimiter=',', quotechar='"')
                 header = next(reader)
-        except:
-            message = '"ERROR - Error reading header from: '+fullpath
+        except Exception as e:
+            message = 'ERROR - Error reading data from: {0}\n\n{1}'.format(fullpath, e)
             error = True
             return error, message
         header[0] = 'Timestep'
         header[1] = 'Time'
         self.ID.clear()
         i = 1
         nCol = 1
@@ -524,16 +524,16 @@
                         try:
                             self.EMax.append(float(row[ind_E]))
                         except:
                             self.EMax.append(float('Nan'))
             #close file
             csvfile.close()
 
-        except:
-            message = 'ERROR - Error reading data from: '+fullpath
+        except Exception as e:
+            message = 'ERROR - Error reading data from: {0}\n\n{1}'.format(fullpath, e)
             error = True
             return error, message
 
         #normal end
         self.nLocs = len(self.ID)
         self.loaded = True
         return error, message
@@ -607,16 +607,16 @@
                         try:
                             self.tVmax.append(float(row[ind_tV]))
                         except:
                             self.tVmax.append(float('Nan'))
 
             # close file
             csvfile.close()
-        except:
-            message = 'ERROR - Error reading header from: '+fullpath
+        except Exception as e:
+            message = 'ERROR - Error reading data from: {0}\n\n{1}'.format(fullpath, e)
             error = True
             return error, message
 
         # normal return
         self.nLocs = len(self.ID)
         self.loaded = True
         return error, message
@@ -660,16 +660,16 @@
                     except:
                         self.tdHmax.append(float('Nan'))
                     try:
                         self.Q.append(float(row[6]))
                     except:
                         self.Q.append(float('Nan'))
             #csvfile.close()
-        except:
-            message = 'ERROR - Error reading header from: '+fullpath
+        except Exception as e:
+            message = 'ERROR - Error reading data from: {0}\n\n{1}'.format(fullpath, e)
             error = True
             return error, message
         if len(header)>7:
             error = True
             message = 'ERROR - More than seven columns in node maximums file: '+fullpath
             return error, message
         if not (header[2].upper()=='HMAX'):
@@ -730,16 +730,16 @@
                     except:
                         self.tdQmax.append(float('Nan'))
                     try:
                         self.H.append(float(row[6]))
                     except:
                         self.H.append(float('Nan'))
             #csvfile.close()
-        except:
-            message = 'ERROR - Error reading header from: '+fullpath
+        except Exception as e:
+            message = 'ERROR - Error reading data from: {0}\n\n{1}'.format(fullpath, e)
             error = True
             return error, message
         if len(header)>7:
             error = True
             message = 'ERROR - More than 7 columns RLL_Qmx file: '+fullpath
             return error, message
         if not (header[2].upper()=='QMAX'):
@@ -804,16 +804,16 @@
                     except:
                         self.tdVolMax.append(float('Nan'))
                     try:
                         self.H.append(float(row[6]))
                     except:
                         self.H.append(float('Nan'))
             #csvfile.close()
-        except:
-            message = 'ERROR - Error reading header from: '+fullpath
+        except Exception as e:
+            message = 'ERROR - Error reading data from: {0}\n\n{1}'.format(fullpath, e)
             error = True
             return error, message
         if len(header)>7:
             error = True
             message = 'ERROR - More than 7 columns RLL_Volmx file: '+fullpath
             return error, message
         if not (header[2].upper()=='VOL MAX'):
```

### Comparing `pytuflow-0.0.8/pytuflow/TUFLOW_results2013.py` & `pytuflow-0.0.9/pytuflow/TUFLOW_results2013.py`

 * *Files identical despite different names*

### Comparing `pytuflow-0.0.8/pytuflow/helper.py` & `pytuflow-0.0.9/pytuflow/helper.py`

 * *Files identical despite different names*

### Comparing `pytuflow-0.0.8/pytuflow.egg-info/PKG-INFO` & `pytuflow-0.0.9/pytuflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytuflow
-Version: 0.0.8
+Version: 0.0.9
 Summary: Package for scripting TUFLOW time series results.
 Home-page: https://github.com/TUFLOW-Support/PyTuflow
 Author: tuflowsupport
 Author-email: support@tuflow.com
 License: UNKNOWN
 Description: # PyTuflow
```

### Comparing `pytuflow-0.0.8/setup.py` & `pytuflow-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytuflow",
-    version="0.0.8",
+    version="0.0.9",
     author="tuflowsupport",
     author_email="support@tuflow.com",
     description="Package for scripting TUFLOW time series results.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TUFLOW-Support/PyTuflow",
     packages=setuptools.find_packages(),
```

