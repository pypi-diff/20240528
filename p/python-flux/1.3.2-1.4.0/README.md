# Comparing `tmp/python_flux-1.3.2.tar.gz` & `tmp/python_flux-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.3.2.tar", max compression
+gzip compressed data, was "python_flux-1.4.0.tar", max compression
```

## Comparing `python_flux-1.3.2.tar` & `python_flux-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     8872 2024-04-26 12:27:05.738836 python_flux-1.3.2/README.rst
--rw-r--r--   0        0        0      741 2024-05-03 04:55:36.722355 python_flux-1.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.3.2/python_flux/__init__.py
--rw-r--r--   0        0        0    23483 2024-05-03 04:55:16.370351 python_flux-1.3.2/python_flux/flux.py
--rw-r--r--   0        0        0      759 2024-04-25 04:03:40.583703 python_flux-1.3.2/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1921 2024-04-25 04:03:40.584710 python_flux-1.3.2/python_flux/producers.py
--rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.3.2/python_flux/subscribers.py
--rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 python_flux-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     8872 2024-04-26 12:27:05.738836 python_flux-1.4.0/README.rst
+-rw-r--r--   0        0        0      741 2024-05-28 04:58:20.786898 python_flux-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.4.0/python_flux/__init__.py
+-rw-r--r--   0        0        0    24446 2024-05-28 04:58:20.449426 python_flux-1.4.0/python_flux/flux.py
+-rw-r--r--   0        0        0      759 2024-04-25 04:03:40.583703 python_flux-1.4.0/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1905 2024-05-28 04:58:20.449885 python_flux-1.4.0/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.4.0/python_flux/subscribers.py
+-rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 python_flux-1.4.0/PKG-INFO
```

### Comparing `python_flux-1.3.2/README.rst` & `python_flux-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.2/python_flux/flux.py` & `python_flux-1.4.0/python_flux/flux.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,22 +133,27 @@
 
         def log_error(msg, e, c):
             message = msg(e, c)
             logging.error(message)
 
         return FDoOnNext(partial(log_function, level, build_log_message), partial(log_error, build_error_message), True, self)
 
-    def parallel(self, pool_size=5, metric_function=None):
+    def parallel(self, pool_size=5, join_timeout=0.001, metric_function=None, metric_rate=10, metric_buffer_size=10):
         """
         Ejecuta la obtención de elementos del stream en paralelo
 
         :param pool_size: Pool de hilos a utilizar
-        :param metric_function: función(metrics) Esta es una función que si se setea recibe con cada elemento procesado  un bloque de métricas sobre la ejecución paralela
+        :param join_timeout: Tiempo de espera de join en segundos por cada hilo (decimal)
+        :param metric_function: función(metrics, contexto) Esta es una función que si se setea recibe con cada elemento
+        procesado un bloque de métricas sobre la ejecución paralela y el contexto del último elemento recibido
+        :param metric_rate: Cantidad de evaluaciones por segundo que se ejecuta la función metric_function.
+        Si es None se ejecuta siempre
+        :param metric_buffer_size: Tamaño del buffer utilizado para generar las métricas recibidas por metric_function
         """
-        return FParallel(pool_size, metric_function, self)
+        return FParallel(pool_size, join_timeout, metric_function, metric_rate, metric_buffer_size, self)
 
     def on_error_resume(self, resume=fu.default_error_resume, exceptions=[Exception]):
         """
         En caso de error, este paso ejecuta la función resume que debe retornar un valor
         a partir del error recibido por parámetro.
 
         :param resume: función(ex, contexto) Debe retornar el valor a substituir en el flujo.
@@ -303,18 +308,18 @@
 
     def next(self, context):
         value, e, ctx = super(FTake, self).next(context)
         if e is not None:
             return value, e, ctx
         if self.predicate is not None:
             valid, e = fu.try_or(partial(self.predicate), value, ctx)
+            if e is not None:
+                return value, e, ctx
         else:
-            valid = False
-        if e is not None:
-            return value, e, ctx
+            valid = True
         if valid:
             self.idx = self.idx + 1
         if self.idx <= self.count:
             return value, e, ctx
         else:
             return value, StopIteration(), ctx
 
@@ -387,93 +392,101 @@
         if valid:
             time.sleep(self.delay / 1000)
         return value, e, ctx
 
 
 class _Register:
 
-    def __init__(self, id):
-        self.id = id
+    def __init__(self):
         self.value = None
         self.e = None
-        self.ctx = None
+        self.start_ctx = None
+        self.end_ctx = None
+        self.thread = None
         self.elapsed_time = 0
 
-    def execute(self, sup, context):
+    def execute(self, sup):
         t = time.process_time_ns()
         sup.prepare_next()
-        self.value, self.e, self.ctx = sup.next(context)
-        self.elapsed_time = (time.process_time_ns() - t) / 1000
+        self.value, self.e, self.end_ctx = sup.next(self.start_ctx)
+        self.elapsed_time = (time.process_time_ns() - t) / 1000000
+
+    def set_thread(self, t):
+        self.thread = t
+
+    def set_start_context(self, ctx):
+        self.start_ctx = ctx
 
 
 class FParallel(Stream):
-    def __init__(self, pool, metric_func, flux):
+    def __init__(self, pool_size, join_timeout, metric_func, metric_rate, metric_buffer_size, flux):
         super().__init__(flux)
-        self.pool_size = pool
+        self.pool_size = pool_size
         self.metric_func = metric_func
-        self.jobs = {}
-        self.pool = {}
-        self.ctxs = {}
+        self.metric_rate = metric_rate
+        self.metric_buffer_size = metric_buffer_size
+        self.join_timeout = join_timeout
+        self.pool = []
         self.buffer_metrics = []
-        self.ids = 0
-        self.last_ctx_id = 0
+        self.last_metric_execution = 0
         self.waiting_to_stop = False
 
-    def show_metrics(self):
+    def show_metrics(self, now, ctx):
         if self.metric_func is not None:
             len_buffer = len(self.buffer_metrics)
-            diff_time = max(map(lambda p: p[2], self.buffer_metrics)) - min(map(lambda p: p[2], self.buffer_metrics))
-            metrics = {
-                'pool_size': self.pool_size,
-                'used_pool': len(self.pool),
-                'avg_used_pool': sum(map(lambda p: p[0], self.buffer_metrics)) / len_buffer if len_buffer > 0 else 0.0,
-                'avg_task_time_ms': sum(map(lambda p: p[1], self.buffer_metrics)) / len_buffer if len_buffer > 0 else 0.0,
-                'rate_rps': round(1000 * len(self.buffer_metrics) / diff_time if len_buffer > 0 and diff_time > 0 else 0.0, 2)
-            }
-            self.metric_func(metrics)
+            if len_buffer > 0:
+                diff_time = max(map(lambda p: p[2], self.buffer_metrics)) - min(map(lambda p: p[2], self.buffer_metrics))
+                metrics = {
+                    'pool_size': self.pool_size,
+                    'used_pool': len(self.pool),
+                    'avg_used_pool': sum(map(lambda p: p[0], self.buffer_metrics)) / len_buffer if len_buffer > 0 else 0.0,
+                    'avg_task_time_ms': sum(map(lambda p: p[1], self.buffer_metrics)) / len_buffer if len_buffer > 0 else 0.0,
+                    'rate_rps': round(1000 * len(self.buffer_metrics) / diff_time if len_buffer > 0 and diff_time > 0 else 0.0, 2)
+                }
+                if self.metric_rate is None or (now - self.last_metric_execution) > (1000 / self.metric_rate):
+                    self.metric_func(metrics, ctx)
+                    self.last_metric_execution = now
 
     def next(self, context):
         ctx = context
         while True:
             if not self.waiting_to_stop:
                 if len(self.pool) < self.pool_size:
-                    reg = _Register(self.ids)
-                    t = threading.Thread(target=reg.execute, args=[super(FParallel, self), ctx])
-                    self.jobs[self.ids] = reg
-                    self.pool[self.ids] = t
-                    self.ids = self.ids + 1
+                    reg = _Register()
+                    t = threading.Thread(target=reg.execute, args=[super(FParallel, self)])
+                    reg.set_thread(t)
+                    reg.set_start_context(ctx)
+                    self.pool.append(reg)
                     t.start()
             pools = self.pool.copy()
-            for i, t in pools.items():
+            for r in pools:
                 try:
-                    t.join(0.01)
-                    if t.is_alive():
+                    now = time.process_time_ns() / 1000000
+                    self.show_metrics(now, ctx)
+                    r.thread.join(self.join_timeout)
+                    if r.thread.is_alive():
                         continue
                     else:
-                        self.pool.pop(i)
-                        r = self.jobs.pop(i)
-                        self.ctxs[i] = r.ctx
-                        self.buffer_metrics.append((len(self.pool), r.elapsed_time, time.process_time_ns() / 1000))
-                        if len(self.buffer_metrics) >= 10:
+                        self.pool.remove(r)
+                        self.buffer_metrics.append((len(self.pool), r.elapsed_time, now))
+                        if len(self.buffer_metrics) >= self.metric_buffer_size:
                             self.buffer_metrics.pop(0)
-                        if self.last_ctx_id in self.ctxs:
-                            ctx = merge(ctx, self.ctxs.pop(self.last_ctx_id))
-                            self.last_ctx_id = self.last_ctx_id + 1
+                        if r.end_ctx is not None:
+                            ctx = merge(ctx, r.end_ctx)
                         if isinstance(r.e, StopIteration):
                             self.waiting_to_stop = True
                             if len(self.pool) == 0:
-                                self.show_metrics()
+                                self.show_metrics(now, ctx)
                                 return None, StopIteration(), ctx
                             else:
                                 continue
                         if self.waiting_to_stop:
                             if len(self.pool) == 0:
-                                self.show_metrics()
+                                self.show_metrics(now, ctx)
                                 return None, StopIteration(), ctx
-                        self.show_metrics()
                         return r.value, r.e, ctx
                 except Exception as e:
                     return None, e, ctx
 
 
 class FMap(Stream):
     def __init__(self, func, flux):
```

### Comparing `python_flux-1.3.2/python_flux/flux_utilis.py` & `python_flux-1.4.0/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.2/python_flux/producers.py` & `python_flux-1.4.0/python_flux/producers.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         except Exception as ex:
             return None, ex
 
 
 class PFromGenerator(Producer):
     def __init__(self, function_gen):
         super(PFromGenerator, self).__init__()
-        self.function_gen = LockedIterator(function_gen)
+        self.function_gen = function_gen
         self.generator = None
 
     def _next(self, context):
         if self.generator is None:
             self.generator = self.function_gen(context)
         try:
             v = next(self.generator)
```

### Comparing `python_flux-1.3.2/python_flux/subscribers.py` & `python_flux-1.4.0/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.2/PKG-INFO` & `python_flux-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.3.2
+Version: 1.4.0
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

