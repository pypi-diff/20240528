# Comparing `tmp/tools_hjh-2.6.6.tar.gz` & `tmp/tools_hjh-2.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.6.6.tar", last modified: Wed May 22 21:20:08 2024, max compression
+gzip compressed data, was "dist\tools_hjh-2.6.7.tar", last modified: Tue May 28 03:15:19 2024, max compression
```

## Comparing `tools_hjh-2.6.6.tar` & `tools_hjh-2.6.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 21:20:08.000000 tools_hjh-2.6.6/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.6/LICENSE
--rw-rw-rw-   0        0        0      207 2024-05-22 21:20:08.000000 tools_hjh-2.6.6/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 21:20:08.000000 tools_hjh-2.6.6/setup.cfg
--rw-rw-rw-   0        0        0      417 2024-05-22 21:19:47.000000 tools_hjh-2.6.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:20:06.000000 tools_hjh-2.6.6/tools_hjh/
--rw-rw-rw-   0        0        0     4066 2024-04-22 08:48:58.000000 tools_hjh-2.6.6/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.6/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.6/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.6/tools_hjh/HTTPRequest2.py
--rw-rw-rw-   0        0        0     8808 2024-04-29 21:48:40.000000 tools_hjh-2.6.6/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.6/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.6/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    46268 2024-04-24 01:40:14.000000 tools_hjh-2.6.6/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.6/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     3277 2024-05-22 21:17:23.000000 tools_hjh-2.6.6/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     7766 2024-05-22 13:57:46.000000 tools_hjh-2.6.6/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      539 2024-05-22 21:19:35.000000 tools_hjh-2.6.6/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 21:20:08.000000 tools_hjh-2.6.6/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-22 21:20:03.000000 tools_hjh-2.6.6/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-05-22 21:20:03.000000 tools_hjh-2.6.6/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-05-22 21:20:03.000000 tools_hjh-2.6.6/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      479 2024-05-22 21:20:04.000000 tools_hjh-2.6.6/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 21:20:03.000000 tools_hjh-2.6.6/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 03:15:18.000000 tools_hjh-2.6.7/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.7/LICENSE
+-rw-rw-rw-   0        0        0      207 2024-05-28 03:15:18.000000 tools_hjh-2.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-28 03:15:18.000000 tools_hjh-2.6.7/setup.cfg
+-rw-rw-rw-   0        0        0      417 2024-05-28 03:14:33.000000 tools_hjh-2.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:15:18.000000 tools_hjh-2.6.7/tools_hjh/
+-rw-rw-rw-   0        0        0     4066 2024-04-22 08:48:58.000000 tools_hjh-2.6.7/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.7/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.7/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.7/tools_hjh/HTTPRequest2.py
+-rw-rw-rw-   0        0        0     8808 2024-04-29 21:48:40.000000 tools_hjh-2.6.7/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.7/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.7/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    46268 2024-04-24 01:40:14.000000 tools_hjh-2.6.7/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.7/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     3316 2024-05-24 08:22:33.000000 tools_hjh-2.6.7/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     7766 2024-05-22 13:57:46.000000 tools_hjh-2.6.7/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      539 2024-05-22 21:19:35.000000 tools_hjh-2.6.7/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 03:15:18.000000 tools_hjh-2.6.7/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-28 03:15:13.000000 tools_hjh-2.6.7/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-05-28 03:15:13.000000 tools_hjh-2.6.7/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-05-28 03:15:13.000000 tools_hjh-2.6.7/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      479 2024-05-28 03:15:14.000000 tools_hjh-2.6.7/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 03:15:13.000000 tools_hjh-2.6.7/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.6.6/tools_hjh/Chrome.py` & `tools_hjh-2.6.7/tools_hjh/Chrome.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/DBConn.py` & `tools_hjh-2.6.7/tools_hjh/DBConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/HTTPRequest.py` & `tools_hjh-2.6.7/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/HTTPRequest2.py` & `tools_hjh-2.6.7/tools_hjh/HTTPRequest2.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/HTTPTools.py` & `tools_hjh-2.6.7/tools_hjh/HTTPTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/Log.py` & `tools_hjh-2.6.7/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/MemoryDB.py` & `tools_hjh-2.6.7/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/OracleTools.py` & `tools_hjh-2.6.7/tools_hjh/OracleTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/SSHConn.py` & `tools_hjh-2.6.7/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/ThreadPool.py` & `tools_hjh-2.6.7/tools_hjh/ThreadPool.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     print(name, 'begin')
     mylist.append(name)
     time.sleep(10)
     return name
 
 
 def main():
-    tp = ThreadPool(2)
-    tp.run(one, ('A',))
-    tp.run(one, ('B',))
-    tp.wait()
+    mylist = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
+    for num in mylist:
+        mylist.remove(num)
+        print('removed', num)
+    print(len(mylist))
     print(mylist)
 
 
 class ThreadPool():
     """ 维护一个线程池 """
     
     def __init__(self, size, save_result=False, while_wait_time=0.5, report=False):
@@ -45,15 +46,15 @@
             t = myThread(func, args=args, kwargs=kwargs, thread_id=thread_id, pool_status=self.pool_status, result_map=self.result_map, save_result=self.save_result, time_out=time_out)
             t.start()
             self.thread_pool.append(t)
             return thread_id
         else:
             while self.pool_status[0] >= self.size:
                 time.sleep(self.while_wait_time)
-            return self.run(func, args, kwargs)
+            return self.run(func, args, kwargs, time_out)
 
     def get_results(self):
         return self.result_map
     
     def get_result(self, num):
         return self.result_map[num]
     
@@ -89,19 +90,17 @@
             if self.time_out is None:
                 result = self.func(*self.args, **self.kwargs)
                 if self.save_result:
                     self.result_map[self.thread_id] = result
             else:
                 # 实测效率很低
                 eventlet.monkey_patch()
-                with eventlet.Timeout(self.time_out, True):
+                with eventlet.Timeout(self.time_out, False):
                     result = self.func(*self.args, **self.kwargs)
                     if self.save_result:
                         self.result_map[self.thread_id] = result
-        except:
-            pass
         finally:
             self.pool_status[0] = self.pool_status[0] - 1
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `tools_hjh-2.6.6/tools_hjh/Tools.py` & `tools_hjh-2.6.7/tools_hjh/Tools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.6/tools_hjh/__init__.py` & `tools_hjh-2.6.7/tools_hjh/__init__.py`

 * *Files identical despite different names*

