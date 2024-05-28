# Comparing `tmp/multiclass_interface-1.2.tar.gz` & `tmp/multiclass_interface-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiclass_interface-1.2.tar", last modified: Fri May 24 06:00:47 2024, max compression
+gzip compressed data, was "multiclass_interface-1.3.tar", last modified: Tue May 28 11:49:19 2024, max compression
```

## Comparing `multiclass_interface-1.2.tar` & `multiclass_interface-1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 multiclass_interface-1.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-24 05:52:15.000000 multiclass_interface-1.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 multiclass_interface-1.2/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/Multiclass_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-24 06:00:47.000000 multiclass_interface-1.2/Multiclass_interface.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-24 06:00:47.800943 multiclass_interface-1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 multiclass_interface-1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/multiclass_interface/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 multiclass_interface-1.2/multiclass_interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5716 2024-05-24 04:55:16.000000 multiclass_interface-1.2/multiclass_interface/mpi_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 multiclass_interface-1.2/multiclass_interface/multi_object_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 multiclass_interface-1.2/multiclass_interface/multiprocess_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 06:00:47.800943 multiclass_interface-1.2/multiclass_interface/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 05:58:40.000000 multiclass_interface-1.2/multiclass_interface/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 multiclass_interface-1.2/multiclass_interface/tests/my_test_cls.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-24 05:09:43.000000 multiclass_interface-1.2/multiclass_interface/tests/test_mpi.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 multiclass_interface-1.2/multiclass_interface/tests/test_multiclass_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 multiclass_interface-1.2/multiclass_interface/tests/test_multiprocessinterface.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-24 06:00:47.000000 multiclass_interface-1.2/multiclass_interface/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 multiclass_interface-1.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     5238 2024-05-24 05:43:55.000000 multiclass_interface-1.2/sequence_diagrams.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 06:00:47.800943 multiclass_interface-1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 multiclass_interface-1.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-24 05:52:15.000000 multiclass_interface-1.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 multiclass_interface-1.3/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/Multiclass_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-28 11:49:19.662954 multiclass_interface-1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 multiclass_interface-1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/multiclass_interface/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 multiclass_interface-1.3/multiclass_interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6088 2024-05-28 09:44:04.000000 multiclass_interface-1.3/multiclass_interface/mpi_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 multiclass_interface-1.3/multiclass_interface/multi_object_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 multiclass_interface-1.3/multiclass_interface/multiprocess_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/multiclass_interface/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 11:47:05.000000 multiclass_interface-1.3/multiclass_interface/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 multiclass_interface-1.3/multiclass_interface/tests/my_test_cls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2024-05-28 09:44:04.000000 multiclass_interface-1.3/multiclass_interface/tests/test_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 multiclass_interface-1.3/multiclass_interface/tests/test_multiclass_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 multiclass_interface-1.3/multiclass_interface/tests/test_multiprocessinterface.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-28 11:49:19.000000 multiclass_interface-1.3/multiclass_interface/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 multiclass_interface-1.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     6561 2024-05-28 10:04:03.000000 multiclass_interface-1.3/sequence_diagrams.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 11:49:19.662954 multiclass_interface-1.3/setup.cfg
```

### Comparing `multiclass_interface-1.2/.gitlab-ci.yml` & `multiclass_interface-1.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/LICENSE` & `multiclass_interface-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/Multiclass_interface.egg-info/PKG-INFO` & `multiclass_interface-1.3/Multiclass_interface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.2
+Version: 1.3
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiclass_interface-1.2/Multiclass_interface.egg-info/SOURCES.txt` & `multiclass_interface-1.3/Multiclass_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/PKG-INFO` & `multiclass_interface-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.2
+Version: 1.3
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiclass_interface-1.2/README.md` & `multiclass_interface-1.3/README.md`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/multiclass_interface/mpi_interface.py` & `multiclass_interface-1.3/multiclass_interface/mpi_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     'do_task',
     'run_task',
     'closed'}
 
 
 LOOP_UNTIL_CLOSE = True
 TERMINATE_ON_CLOSE = True
+COLLECTIVE_MPI = True
 
 
 class MPIClassInterface():
     def __init__(self, cls, args_lst):
         if len(args_lst) > size:
             if rank == 0:
                 raise Exception(f"Not enough mpi slots. Slots: {size}, Requested: {len(args_lst)}")
@@ -49,18 +50,17 @@
         else:
             class Dummy():
                 def close(self):
                     pass
             self.object = Dummy()
         self.closed = False
 
-        if rank == 0:
-            self.use_rank = np.array([True] * size)
-            self.use_rank[len(args_lst):] = False
-        elif LOOP_UNTIL_CLOSE:
+        self.use_rank = np.array([True] * size)
+        self.use_rank[len(args_lst):] = False
+        if rank > 0 and COLLECTIVE_MPI and LOOP_UNTIL_CLOSE:
             self.work_loop()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
@@ -129,21 +129,26 @@
             return (name, [get_arg(arg) for arg in args], {k: get_arg(v) for k, v in kwargs.items()})
         else:
             return ('skip', [], {})
 
     def __getattribute__(self, name):
         if name in MPIClassInterfaceAttributes:
             return object.__getattribute__(self, name)
-        elif rank > 0:
+        elif COLLECTIVE_MPI and rank > 0:
             self.work_loop()
             return lambda *args, **kwargs: 1
+        elif not self.use_rank[rank]:
+            raise ChildProcessError('MPI worker not used')
 
         def wrap(*args, **kwargs):
-            inp = [self.get_input(name, i, args, kwargs) for i in range(size)]
-            return self.run_task(inp)
+            if COLLECTIVE_MPI:
+                inp = [self.get_input(name, i, args, kwargs) for i in range(size)]
+                return self.run_task(inp)
+            else:
+                return self.do_task(name, args, kwargs)
 
         if hasattr(getattr(self.object, name), '__call__'):
             return wrap
         else:
             return wrap()
 
     def __setattr__(self, name, value):
@@ -158,19 +163,22 @@
         use_rank[slice] = True
         if np.all(self.use_rank == use_rank):
             return self
         return SubsetMPIClassInterface(self.cls, self.object, use_rank)
 
     def close(self):
         if not self.closed:
-            if rank == 0:
-                res = self.run_task([('close', [], {}) for _ in range(size)])
+            if COLLECTIVE_MPI:
+                if rank == 0:
+                    res = self.run_task([('close', [], {}) for _ in range(size)])
+                else:
+                    self.work_loop()
+                    res = None
             else:
-                self.work_loop()
-                res = None
+                res = self.do_task('close', [], {})
             self.closed = True
 
 
 class SubsetMPIClassInterface(MPIClassInterface):
     def __init__(self, cls, object, use_rank):
         self.use_rank = use_rank
         self.cls = cls
```

### Comparing `multiclass_interface-1.2/multiclass_interface/multi_object_list.py` & `multiclass_interface-1.3/multiclass_interface/multi_object_list.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/multiclass_interface/multiprocess_interface.py` & `multiclass_interface-1.3/multiclass_interface/multiprocess_interface.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/multiclass_interface/tests/my_test_cls.py` & `multiclass_interface-1.3/multiclass_interface/tests/my_test_cls.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/multiclass_interface/tests/test_mpi.py` & `multiclass_interface-1.3/multiclass_interface/tests/test_mpi.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,19 +38,36 @@
 
 
 def mpitest_mpi_ProcessClass():
 
     with ProcessClass(MyTest) as cls:
         myTest = cls(1)
         assert myTest.get_id() == 1
-    print("done, test_mpi_ProcessClass")
+    print("done, test_mpi_ProcessClass", flush=True)
+
+
+def mpitest_non_collective_mpi():
+    mpi_interface.COLLECTIVE_MPI = False
+    rank = mpi_interface.rank
+    import time
+    N = 3
+    with MPIClassInterface(MyTest, [(i + 10,) for i in range(N)]) as m:
+
+        try:
+            assert m.get_id() == rank + 10
+            assert rank < N  # rank > N will fail with ChildProcessError
+        except ChildProcessError:
+            pass
+
+    mpi_interface.COLLECTIVE_MPI = True
 
 
 def mpitest_all():
     mpi_interface.activate_mpi()
+
     mpi_interface.exit_mpi_on_close = False
     rank = mpi_interface.rank
     from multiclass_interface.tests.test_multiprocessinterface import test_attribute, test_missing_attribute, test_execption, test_setattr, test_setattr_method
     mpi_interface.TERMINATE_ON_CLOSE = False
 
     def run(f, *args):
         try:
@@ -63,17 +80,18 @@
             if rank == 0:
                 print(f"Rank {rank} done {f.__name__}", flush=True)
     for f in [mpitest_mpi_MyTest,
               mpitest_mpi_ProcessClass]:
         run(f)
 
     try:
-        with MPIClassInterface(MyTest, [(1,), (2,)]) as mpici:
+        with MPIClassInterface(MyTest, [(1,), (2,), (3,)]) as mpici:
             for f in [test_attribute, test_missing_attribute, test_execption, test_setattr, test_setattr_method]:
-                break
+
                 run(f, mpici)
 
     except ChildProcessError:
         pass
-    mpi_interface.TERMINATE_ON_CLOSE = True
+
+    run(mpitest_non_collective_mpi)
 
     print(f"Rank {rank} Done test_all")
```

### Comparing `multiclass_interface-1.2/multiclass_interface/tests/test_multiclass_list.py` & `multiclass_interface-1.3/multiclass_interface/tests/test_multiclass_list.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/multiclass_interface/tests/test_multiprocessinterface.py` & `multiclass_interface-1.3/multiclass_interface/tests/test_multiprocessinterface.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/pyproject.toml` & `multiclass_interface-1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.2/sequence_diagrams.md` & `multiclass_interface-1.3/sequence_diagrams.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# Sequence diagrams
+- [ThreadClass](#threadclass)
+- [ProcessClass](#processclass)
+- [MultiThreadClassInterface](#multithreadclassinterface)
+- [MultiProcessClassInterface](#multiprocessclassinterface)
+- [MPIClassInterface](#mpiclassinterface)
+- [MPIClassInterface(LOOP_UNTIL_CLOSE=False)](#mpiclassinterfaceloop_until_closefalse)
+- [MPIClassInterface(COLLECTIVE_MPI=False)](#mpiclassinterfacecollective_mpifalse)
+
 ## ThreadClass
 ```mermaid
 sequenceDiagram
     participant U as Main
     participant TC as ThreadClass
     
     U->>+TC: cls=A
@@ -38,15 +47,15 @@
 The `ProcessClass` is similar to the `ThreadClas` except that it uses a seprate Process instead of a Thread.
 This means:
 - More time used to spawn process
 - Changes to `os.environ['LD_LIBRARY_PATH']` are effective in the process
 - Libraries (dll/so) will have their own memory space (important if multiple instances are launched)
 - Multiple processes allows parallel execution
 
-## MultiProcessClassInterface
+## MultiThreadClassInterface
 
 ```mermaid
 sequenceDiagram
     participant U as Main
     participant TC as MultiThreadClassInterface
     
     U->>+TC: cls=A, [args1,args2])
@@ -162,15 +171,15 @@
     MPI0->>MPI2: close
     end
     MPI0->>-MPI0: 
     MPI1->>-MPI1: 
     MPI2->>-MPI2: 
 ```
 
-## MPIClassInterface
+## MPIClassInterface(LOOP_UNTIL_CLOSE=False)
 
 Setting `mpi_interface.LOOP_UNTIL_CLOSE=False` results in the following workflow
 
 ```mermaid
 sequenceDiagram
     actor U as User
     
@@ -222,7 +231,45 @@
 
     
     MPI0->>-U: [res1,res2]
     
 ```
 
 
+## MPIClassInterface(COLLECTIVE_MPI=False)
+Setting `mpi_interface.COLLECTIVE_MPI=False` results in the following workflow
+
+```mermaid
+sequenceDiagram
+    
+    participant MPI0 as MPI,rank0<br>MPIClassInterface
+    
+    
+    MPI0->>+MPI0: cls=A, [(args0),(args1)]
+    
+    
+    create participant A0
+    MPI0->>+A0: args0
+    
+    participant MPI1 as MPI,rank1<br>MPIClassInterface
+    MPI1->>+MPI1: cls=A, [(args0),(args1)]
+    create participant A1
+    MPI1->>A1: args1
+    participant MPI2 as MPI,rank2<br>MPIClassInterface
+    MPI2->>MPI2: cls=A, [(args0),(args1)]
+    
+    MPI0->>+MPI0:~a.f([args0,args1])
+    MPI1->>+MPI1:~a.f([args0,args1])
+    MPI2->>+MPI2:~a.f([args0,args1])
+    
+    
+    MPI0->>+A0: f(args0)
+    MPI1->>+A1: f(args1)
+    MPI2->>-MPI2: ChildProcessError
+    A0->>-MPI0: res0
+    A1->>-MPI1: res1
+        
+    MPI0->>-MPI0: res0
+    MPI1->>-MPI1: res1
+    
+```
+
```

