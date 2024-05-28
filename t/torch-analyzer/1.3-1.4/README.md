# Comparing `tmp/torch_analyzer-1.3.tar.gz` & `tmp/torch_analyzer-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_analyzer-1.3.tar", last modified: Fri May 24 08:03:51 2024, max compression
+gzip compressed data, was "torch_analyzer-1.4.tar", last modified: Tue May 28 15:12:22 2024, max compression
```

## Comparing `torch_analyzer-1.3.tar` & `torch_analyzer-1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:03:51.852543 torch_analyzer-1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 08:03:46.000000 torch_analyzer-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 08:03:51.852543 torch_analyzer-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-24 08:03:46.000000 torch_analyzer-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 08:03:51.852543 torch_analyzer-1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-24 08:03:46.000000 torch_analyzer-1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:03:51.852543 torch_analyzer-1.3/torch_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-24 08:03:51.000000 torch_analyzer-1.3/torch_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 08:03:51.852543 torch_analyzer-1.3/torchanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/flops.py
--rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/flops_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/in_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/memops_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/time_mem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-24 08:03:46.000000 torch_analyzer-1.3/torchanalyzer/viser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:12:22.038859 torch_analyzer-1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 15:12:17.000000 torch_analyzer-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-28 15:12:22.038859 torch_analyzer-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-28 15:12:17.000000 torch_analyzer-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 15:12:22.038859 torch_analyzer-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-28 15:12:17.000000 torch_analyzer-1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:12:22.038859 torch_analyzer-1.4/torch_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-28 15:12:22.000000 torch_analyzer-1.4/torch_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-28 15:12:22.000000 torch_analyzer-1.4/torch_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 15:12:22.000000 torch_analyzer-1.4/torch_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 15:12:22.000000 torch_analyzer-1.4/torch_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-28 15:12:22.000000 torch_analyzer-1.4/torch_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 15:12:22.038859 torch_analyzer-1.4/torchanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/flops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/flops_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/in_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/memops_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/time_mem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-28 15:12:17.000000 torch_analyzer-1.4/torchanalyzer/viser.py
```

### Comparing `torch_analyzer-1.3/LICENSE` & `torch_analyzer-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.3/PKG-INFO` & `torch_analyzer-1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 1.3
+Version: 1.4
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_analyzer-1.3/README.md` & `torch_analyzer-1.4/README.md`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.3/setup.py` & `torch_analyzer-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     for x in f.readlines():
         requires.append(f'{x.strip()}')
 
 
 setuptools.setup(
     name="torch-analyzer",
     py_modules=["torch-analyzer"],
-    version="1.3",
+    version="1.4",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A torch model analyzer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IrisRainbowNeko/torch-analyzer",
     packages=setuptools.find_packages(),
```

### Comparing `torch_analyzer-1.3/torch_analyzer.egg-info/PKG-INFO` & `torch_analyzer-1.4/torch_analyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-analyzer
-Version: 1.3
+Version: 1.4
 Summary: A torch model analyzer
 Home-page: https://github.com/IrisRainbowNeko/torch-analyzer
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_analyzer-1.3/torchanalyzer/flops.py` & `torch_analyzer-1.4/torchanalyzer/flops.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,25 +34,39 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         for name, module in self.model.named_modules():
             module.forward = self.original_forwards[name]
 
 
 class ModelFlopsAnalyzer(ModelAnalyzer):
 
-    def analyze(self, inputs) -> List[Tuple[str, str, nn.Module, List]]:
+    def analyze(self, input_args, input_kwargs=None) -> List[Tuple[str, str, nn.Module, List]]:
+        if input_kwargs is None:
+            input_kwargs = {}
+        if not isinstance(input_args, (tuple, list)):
+            input_args = [input_args]
+
+        self.model(*input_args, **input_kwargs)
+        self.model: nn.Module
+        self.model.named_modules()
+        self.model.parameters()
+
         with (RecordFlowContext(self.model) as module_flow, ProfContext(self.model, prefix=''),
               profile(record_shapes=True, use_cuda=True) as prof):
-            out = self.model(inputs)
+            out = self.model(*input_args, **input_kwargs)
 
         self.flops_dict = self.summary_events(prof.events(), flops_op_map)
         self.flops_all = self.flops_dict['']
 
         self.memops_dict = self.summary_events(prof.events(), memops_op_map)
         self.memops_all = self.memops_dict['']
 
+        self.param_dict = {}
+        self.count_params(self.model, self.param_dict)
+        self.param_all = self.param_dict['']
+
         flow = self.add_info_to_flow(module_flow.module_record)
         return flow
 
     def summary_events(self, events, op_map):
         flops_dict = {}
         blocks = []
         for event in events:
@@ -64,14 +78,25 @@
                 if len(blocks) > 0:
                     blocks[-1][1] += block[1]
             elif event.name in op_map:
                 flops = op_map[event.name](event.input_shapes, event.concrete_inputs)
                 blocks[-1][1] += flops
         return flops_dict
 
+    def count_params(self, module, param_dict, prefix=''):
+        param_count = 0
+        for name, child in module._modules.items():
+            if child is None:
+                continue
+            submodule_prefix = prefix + ('.' if prefix else '') + name
+            param_count += self.count_params(child, param_dict, submodule_prefix)
+        param_count += sum(p.numel() for p in module.parameters(recurse=False))
+        param_dict[prefix] = param_count
+        return param_count
+
     def add_info_to_flow(self, flow):
         new_flow = []
         for i, item in enumerate(flow):
             name, io_type, module = item
             if io_type == 'i':
                 new_flow.append(item + (self.get_flops(name, module),))
             else:
@@ -80,15 +105,17 @@
 
     def get_flops(self, name, module):
         '''
         :return: [(name:str, info, color:str)]
         '''
         flops = self.flops_dict[name]
         memops = self.memops_dict[name]
+        params = self.param_dict[name]
 
         info_list = [
             # ('Layer', f'{format_time(event.cpu_time)}, {format_percent(event.cpu_time / self.cpu_time_all)}', None, Color.CYAN),
             ('FLOPs', f'{format_flops(flops)}, {format_percent(flops / self.flops_all)}', Color.CYAN),
             ('MemOPs', f'{format_flops(memops)}, {format_percent(memops / self.memops_all)}', Color.MAGENTA),
+            ('Parameters', f'{format_flops(params)}, {format_percent(params / self.param_all)}', Color.YELLOW),
         ]
 
         return {'_one_': info_list}
```

### Comparing `torch_analyzer-1.3/torchanalyzer/flops_kernel.py` & `torch_analyzer-1.4/torchanalyzer/flops_kernel.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,33 +53,33 @@
         return int(qk+softmax+att_v)
 
     return _flops(*input_shapes[:3])
 
 # -----------------------mat ops-----------------------
 def flops_addmm(input_shapes, concrete_inputs):
     @tensor_context
-    def _flops(s_v, s_mat1, s_mat2):
+    def _flops(s_v, s_mat1, s_mat2, *no_use):
         if len(s_v) > 0:
             return 2 * s_mat1[0] * s_mat1[1] * s_mat2[1] + s_mat1[0] * s_mat2[1]
         else:
             return 2 * s_mat1[0] * s_mat1[1] * s_mat2[1]
 
     return _flops(*input_shapes[:3])
 
 
 def flops_mm(input_shapes, concrete_inputs):
     @tensor_context
-    def _flops(s_mat1, s_mat2):
-        return 2 * s_mat1[0] * s_mat1[1] * s_mat2[1]
+    def _flops(s_mat1, s_mat2, *no_use):
+        return 2 * np.prod(s_mat1) * s_mat2[1]
 
     return _flops(*input_shapes)
 
 def flops_bmm(input_shapes, concrete_inputs):
     @tensor_context
-    def _flops(s_mat1, s_mat2):
+    def _flops(s_mat1, s_mat2, *no_use):
         return s_mat1[0] * 2 * s_mat1[1] * s_mat1[2] * s_mat2[2]
 
     return _flops(*input_shapes)
 
 def flops_elem_ops(input_shapes, concrete_inputs):
     if len(input_shapes[0])>len(input_shapes[1]):
         return int(np.prod(input_shapes[0]))
@@ -104,14 +104,16 @@
 
 def flops_tanh(input_shapes, concrete_inputs):
     return 8*np.prod(input_shapes[0])
 
 # -----------------------tensor ops-----------------------
 def flops_sum(input_shapes, concrete_inputs):
     s_in = np.array(input_shapes[0])
+    if len(s_in)==0:
+        return 1
     s_in[concrete_inputs[1]] -= 1
     return s_in.prod()
 
 def flops_var(input_shapes, concrete_inputs):
     return 4*np.prod(input_shapes[0])
 
 def flops_std(input_shapes, concrete_inputs):
@@ -169,14 +171,17 @@
     'aten::sigmoid': flops_sigmoid,
     # memory ops
     #'aten::transpose': flops_single_ops,
     #'aten::reshape': flops_single_ops,
     #'aten::resolve_conj': flops_single_ops,
 }
 
+def add_op(op_name, flops_counter):
+    flops_counter[op_name] = flops_counter
+
 if __name__ == '__main__':
     from torch import nn
     from torch.profiler import record_function
     class SimpleCNN(nn.Module):
         def __init__(self):
             super(SimpleCNN, self).__init__()
             self.conv1 = nn.Conv2d(1, 10, kernel_size=5, bias=False, padding=1)
```

### Comparing `torch_analyzer-1.3/torchanalyzer/in_out.py` & `torch_analyzer-1.4/torchanalyzer/in_out.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,17 +55,22 @@
 
 class ModelIOAnalyzer(ModelAnalyzer):
     def __init__(self, model):
         super().__init__(model)
         self.info_names = ['shape', 'max', 'min', 'mean']
         self.colors = [Color.CYAN, Color.GREEN, Color.YELLOW, Color.MAGENTA]
 
-    def analyze(self, inputs, prefix='layer:'):
+    def analyze(self, input_args, input_kwargs=None, prefix='layer:'):
+        if input_kwargs is None:
+            input_kwargs = {}
+        if not isinstance(input_args, (tuple, list)):
+            input_args = [input_args]
+
         with ModuleIOContext(self.model) as module_io, RecordFlowContext(self.model) as module_flow:
-            out = self.model(inputs)
+            out = self.model(*input_args, **input_kwargs)
         self.module_io = module_io
 
         flow = self.add_info_to_flow(module_flow.module_record)
         return flow
 
     def add_info_to_flow(self, flow):
         new_flow = []
```

### Comparing `torch_analyzer-1.3/torchanalyzer/memops_kernel.py` & `torch_analyzer-1.4/torchanalyzer/memops_kernel.py`

 * *Files identical despite different names*

### Comparing `torch_analyzer-1.3/torchanalyzer/time_mem.py` & `torch_analyzer-1.4/torchanalyzer/time_mem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 from typing import List, Tuple, Iterable
 
 import numpy as np
 import torch
 from torch import nn
 from torch.profiler import profile, record_function, ProfilerActivity
 
-from .base import ModelAnalyzer, RecordFlowContext
+from .base import ModelAnalyzer, RecordFlowContext, BackContext
 from .utils import Color, format_memory, format_time, format_percent
 
-from torch.autograd import Function
 
-# 方便在backward中记录Module区间
-class BackContext(Function):
-    @staticmethod
-    def forward(ctx, x, name):
-        ctx.constant = name
-        return x
-
-    @staticmethod
-    def backward(ctx, grad_outputs):
-        name = ctx.constant
-        with record_function(name):
-            return grad_outputs, None
+
 
 class ProfContext:
     def __init__(self, model, prefix='layer:', func_name='forward', with_backward=False):
         self.model = model
         self.prefix = prefix
         self.func_name = func_name
         self.original_forwards = {}
@@ -57,32 +45,39 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         for name, module in self.model.named_modules():
             setattr(module, self.func_name, self.original_forwards[name])
 
 class ModelTimeMemAnalyzer(ModelAnalyzer):
 
-    def analyze(self, inputs, prefix='layer:', with_init=True, with_backward=False) -> List[Tuple[str, str, nn.Module, List]]:
+    def analyze(self, input_args, input_kwargs=None, prefix='layer:', with_init=True, with_backward=False) -> List[Tuple[str, str, nn.Module, List]]:
+        if input_kwargs is None:
+            input_kwargs = {}
+        if not isinstance(input_args, (tuple, list)):
+            input_args = [input_args]
+
+        device = self._get_device(input_args, input_kwargs)
         if with_init:
             self.model.to('cpu')
             with ProfContext(self.model, prefix=prefix, func_name='_apply'):
                 with profile(activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA], profile_memory=True) as prof_to:
-                    self.model.to(inputs.device)
+                    self.model.to(device)
             self.filtered_events_to = {event.key[len(prefix):]: event for event in prof_to.key_averages() if
                                        event.key.startswith(prefix)}
             self.cpu_mem_all_to = max(1, self.filtered_events_to[''].cpu_memory_usage)
             self.cuda_mem_all_to = max(1, self.filtered_events_to[''].cuda_memory_usage)
 
         with RecordFlowContext(self.model) as module_flow:
-            self.model(inputs)  # warmup
+            self.model(*input_args, **input_kwargs)  # warmup
 
-        inputs.requires_grad = True # for backward
+        self._enable_grad(input_args) # for backward
+        self._enable_grad(input_kwargs) # for backward
         with ProfContext(self.model, prefix=prefix, func_name='forward', with_backward=with_backward):
             with profile(activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA], profile_memory=True) as prof:
-                out = self.model(inputs)
+                out = self.model(*input_args, **input_kwargs)
 
         if with_backward:
             out = out.mean()
             with profile(activities=[ProfilerActivity.CPU, ProfilerActivity.CUDA], profile_memory=True) as prof_back:
                 out.backward()
             # for event in prof_back.events():
             #     print(event.name, format_memory(abs(event.cuda_memory_usage)), format_time(event.cuda_time))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `torch_analyzer-1.3/torchanalyzer/utils.py` & `torch_analyzer-1.4/torchanalyzer/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+import torch
 from enum import Enum
 
 
 class Color(Enum):
     """
     控制台颜色枚举类
     """
@@ -45,12 +46,14 @@
 def format_flops(flops):
     if flops < 1000:
         return f"{flops}"
     elif flops < 1e6:
         return f"{flops / 1000:.2f} K"
     elif flops < 1e9:
         return f"{flops / 1e6:.2f} M"
+    elif flops < 1e12:
+        return f"{flops / 1e9:.2f} G"
     else:
-        return f"{flops / 1e9:.2f} T"
+        return f"{flops / 1e12:.2f} T"
 
 def format_percent(data):
     return f'{data * 100:.2f}%'
```

### Comparing `torch_analyzer-1.3/torchanalyzer/viser.py` & `torch_analyzer-1.4/torchanalyzer/viser.py`

 * *Files identical despite different names*

