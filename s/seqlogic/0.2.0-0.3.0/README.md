# Comparing `tmp/seqlogic-0.2.0.tar.gz` & `tmp/seqlogic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqlogic-0.2.0.tar", last modified: Mon May 20 03:13:38 2024, max compression
+gzip compressed data, was "seqlogic-0.3.0.tar", last modified: Tue May 28 01:40:32 2024, max compression
```

## Comparing `seqlogic-0.2.0.tar` & `seqlogic-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 03:13:38.140811 seqlogic-0.2.0/
--rw-rw-rw-   0        0        0      956 2024-05-20 03:13:38.138706 seqlogic-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.2.0/README.md
--rw-rw-rw-   0        0        0      263 2024-05-20 03:11:17.000000 seqlogic-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 03:13:38.141712 seqlogic-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 03:13:38.049341 seqlogic-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-20 03:13:38.078737 seqlogic-0.2.0/src/seqlogic/
--rw-rw-rw-   0        0        0      357 2024-05-05 19:08:40.000000 seqlogic-0.2.0/src/seqlogic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 03:13:38.110716 seqlogic-0.2.0/src/seqlogic/algorithms/
--rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.2.0/src/seqlogic/algorithms/__init__.py
--rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.2.0/src/seqlogic/algorithms/aes.py
--rw-rw-rw-   0        0        0      285 2024-04-30 03:11:09.000000 seqlogic-0.2.0/src/seqlogic/algorithms/gray.py
--rw-rw-rw-   0        0        0    21662 2024-05-08 03:13:26.000000 seqlogic-0.2.0/src/seqlogic/bits.py
--rw-rw-rw-   0        0        0     8227 2024-05-20 03:10:35.000000 seqlogic-0.2.0/src/seqlogic/design.py
--rw-rw-rw-   0        0        0     2981 2024-04-01 05:33:29.000000 seqlogic-0.2.0/src/seqlogic/hier.py
--rw-rw-rw-   0        0        0    83756 2024-05-19 21:42:07.000000 seqlogic-0.2.0/src/seqlogic/lbool.py
--rw-rw-rw-   0        0        0    13223 2024-05-20 01:17:15.000000 seqlogic-0.2.0/src/seqlogic/sim.py
--rw-rw-rw-   0        0        0     1368 2024-05-05 19:08:40.000000 seqlogic-0.2.0/src/seqlogic/util.py
-drwxrwxrwx   0        0        0        0 2024-05-20 03:13:38.137713 seqlogic-0.2.0/src/seqlogic.egg-info/
--rw-rw-rw-   0        0        0      956 2024-05-20 03:13:37.000000 seqlogic-0.2.0/src/seqlogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2024-05-20 03:13:38.000000 seqlogic-0.2.0/src/seqlogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 03:13:38.000000 seqlogic-0.2.0/src/seqlogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 03:13:38.000000 seqlogic-0.2.0/src/seqlogic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-20 03:13:38.134711 seqlogic-0.2.0/tests/
--rw-rw-rw-   0        0        0     4281 2024-05-08 03:13:26.000000 seqlogic-0.2.0/tests/test_aes.py
--rw-rw-rw-   0        0        0    24103 2024-05-08 03:13:26.000000 seqlogic-0.2.0/tests/test_bits.py
--rw-rw-rw-   0        0        0     3205 2024-05-19 01:15:33.000000 seqlogic-0.2.0/tests/test_enum.py
--rw-rw-rw-   0        0        0     4731 2024-05-05 19:08:40.000000 seqlogic-0.2.0/tests/test_fsm.py
--rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.2.0/tests/test_gray.py
--rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.2.0/tests/test_hier.py
--rw-rw-rw-   0        0        0    30088 2024-05-19 21:41:57.000000 seqlogic-0.2.0/tests/test_lbool.py
--rw-rw-rw-   0        0        0     3533 2024-05-05 19:08:40.000000 seqlogic-0.2.0/tests/test_lfsr.py
--rw-rw-rw-   0        0        0    38096 2024-05-20 02:48:23.000000 seqlogic-0.2.0/tests/test_riscv.py
--rw-rw-rw-   0        0        0     4327 2024-05-05 19:08:40.000000 seqlogic-0.2.0/tests/test_sim.py
--rw-rw-rw-   0        0        0     3024 2024-05-12 18:46:32.000000 seqlogic-0.2.0/tests/test_struct.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.366601 seqlogic-0.3.0/
+-rw-rw-rw-   0        0        0      956 2024-05-28 01:40:32.362720 seqlogic-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.3.0/README.md
+-rw-rw-rw-   0        0        0      263 2024-05-28 01:39:22.000000 seqlogic-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 01:40:32.366601 seqlogic-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.280326 seqlogic-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.304640 seqlogic-0.3.0/src/seqlogic/
+-rw-rw-rw-   0        0        0      357 2024-05-27 19:30:40.000000 seqlogic-0.3.0/src/seqlogic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.334312 seqlogic-0.3.0/src/seqlogic/algorithms/
+-rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.3.0/src/seqlogic/algorithms/__init__.py
+-rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.3.0/src/seqlogic/algorithms/aes.py
+-rw-rw-rw-   0        0        0      285 2024-04-30 03:11:09.000000 seqlogic-0.3.0/src/seqlogic/algorithms/gray.py
+-rw-rw-rw-   0        0        0    21662 2024-05-08 03:13:26.000000 seqlogic-0.3.0/src/seqlogic/bits.py
+-rw-rw-rw-   0        0        0    10371 2024-05-28 01:31:22.000000 seqlogic-0.3.0/src/seqlogic/design.py
+-rw-rw-rw-   0        0        0     2962 2024-05-22 04:04:04.000000 seqlogic-0.3.0/src/seqlogic/hier.py
+-rw-rw-rw-   0        0        0    83927 2024-05-28 01:31:22.000000 seqlogic-0.3.0/src/seqlogic/lbool.py
+-rw-rw-rw-   0        0        0    13223 2024-05-20 01:17:15.000000 seqlogic-0.3.0/src/seqlogic/sim.py
+-rw-rw-rw-   0        0        0     1368 2024-05-05 19:08:40.000000 seqlogic-0.3.0/src/seqlogic/util.py
+drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.361164 seqlogic-0.3.0/src/seqlogic.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-28 01:40:32.000000 seqlogic-0.3.0/src/seqlogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 01:40:32.358161 seqlogic-0.3.0/tests/
+-rw-rw-rw-   0        0        0     4281 2024-05-08 03:13:26.000000 seqlogic-0.3.0/tests/test_aes.py
+-rw-rw-rw-   0        0        0    24103 2024-05-25 00:21:44.000000 seqlogic-0.3.0/tests/test_bits.py
+-rw-rw-rw-   0        0        0     3205 2024-05-25 00:21:32.000000 seqlogic-0.3.0/tests/test_enum.py
+-rw-rw-rw-   0        0        0     4731 2024-05-25 00:21:22.000000 seqlogic-0.3.0/tests/test_fsm.py
+-rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.3.0/tests/test_gray.py
+-rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.3.0/tests/test_hier.py
+-rw-rw-rw-   0        0        0    30042 2024-05-25 01:36:05.000000 seqlogic-0.3.0/tests/test_lbool.py
+-rw-rw-rw-   0        0        0     3533 2024-05-05 19:08:40.000000 seqlogic-0.3.0/tests/test_lfsr.py
+-rw-rw-rw-   0        0        0    30595 2024-05-28 01:31:22.000000 seqlogic-0.3.0/tests/test_riscv.py
+-rw-rw-rw-   0        0        0     4327 2024-05-25 00:20:36.000000 seqlogic-0.3.0/tests/test_sim.py
+-rw-rw-rw-   0        0        0     3024 2024-05-25 00:21:22.000000 seqlogic-0.3.0/tests/test_struct.py
```

### Comparing `seqlogic-0.2.0/PKG-INFO` & `seqlogic-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.2.0
+Version: 0.3.0
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.2.0/README.md` & `seqlogic-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/src/seqlogic/algorithms/aes.py` & `seqlogic-0.3.0/src/seqlogic/algorithms/aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/src/seqlogic/bits.py` & `seqlogic-0.3.0/src/seqlogic/bits.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/src/seqlogic/design.py` & `seqlogic-0.3.0/src/seqlogic/design.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from collections import defaultdict
 from collections.abc import Callable
 
 from vcd.writer import VarValue
 from vcd.writer import VCDWriter as VcdWriter
 
 from .hier import Branch, Leaf
-from .lbool import Vec, VecEnum, ones, zeros
-from .sim import Aggregate, Region, SimAwaitable, Singular, State, changed, get_loop
+from .lbool import Vec, VecEnum, lit2vec
+from .sim import Aggregate, Region, SimAwaitable, Singular, State, changed, get_loop, resume
 
 _item2char = {
     0b00: "x",
     0b01: "0",
     0b10: "1",
     0b11: "x",
 }
@@ -66,15 +66,15 @@
             self._procs.append((region, func, (), {}))
 
     @property
     def procs(self):
         return self._procs
 
 
-class Module(Branch, _TraceIf, _ProcIf):
+class Module(Branch, _ProcIf, _TraceIf):
     """Hierarchical, branch-level design component.
 
     A module contains:
     * Submodules
     * Ports
     * Local variables
     * Local processes
@@ -98,33 +98,122 @@
             child.dump_waves(waves, pattern)
 
     def dump_vcd(self, vcdw: VcdWriter, pattern: str):
         for child in self._children:
             assert isinstance(child, _TraceIf)
             child.dump_vcd(vcdw, pattern)
 
+    def bits(self, name: str, dtype: type, port: bool = False) -> Bits:
+        # TODO(cjdrake): Check name
+        node = Bits(name, parent=self, dtype=dtype)
+        setattr(self, f"_{name}", node)
+        if port:
+            setattr(self, name, node)
+        return node
+
+    def bit(self, name: str, port: bool = False) -> Bit:
+        # TODO(cjdrake): Check name
+        node = Bit(name, parent=self)
+        setattr(self, f"_{name}", node)
+        if port:
+            setattr(self, name, node)
+        return node
+
+    def array(self, name: str, dtype: type) -> Array:
+        # TODO(cjdrake): Check name
+        node = Array(name, parent=self, dtype=dtype)
+        setattr(self, f"_{name}", node)
+        return node
+
+    def submod(self, name: str, mod: type, **params) -> Module:
+        # TODO(cjdrake): Check name
+        node = mod(name, parent=self, **params)
+        setattr(self, f"_{name}", node)
+        return node
 
-class _TraceSingular(Leaf, _TraceIf, Singular, _ProcIf):
-    """Combine hierarchy and sim semantics for singular data types."""
+    def combi(self, y: Bits, f: Callable, *xs: Bits):
+        """Combinational logic."""
+
+        async def proc():
+            while True:
+                await changed(*xs)
+                y.next = f(*[x.value for x in xs])
+
+        self._procs.append((Region.REACTIVE, proc, (), {}))
+
+    def combis(self, ys: list[Bits], f: Callable, *xs: Bits):
+        """Combinational logic."""
+
+        async def proc():
+            while True:
+                await changed(*xs)
+                ret = f(*[x.value for x in xs])
+                assert len(ys) == len(ret)
+                for i, y in enumerate(ys):
+                    y.next = ret[i]
+
+        self._procs.append((Region.REACTIVE, proc, (), {}))
+
+    def connect(self, y: Bits, x: Bits):
+        """Connect input to output."""
+
+        async def proc():
+            while True:
+                await changed(x)
+                y.next = x.value
+
+        self._procs.append((Region.REACTIVE, proc, (), {}))
+
+    def dff_en_ar(self, q: Bits, d: Bits, en: Bit, clk: Bit, rst: Bit, rval: Vec):
+        """D Flip Flop with enable, and async reset."""
+
+        async def proc():
+            while True:
+                state = await resume(
+                    (rst, rst.is_posedge),
+                    (clk, lambda: clk.is_posedge() and rst.is_neg() and en.value == "1b1"),
+                )
+                if state is rst:
+                    q.next = rval
+                elif state is clk:
+                    q.next = d.value
+                else:
+                    assert False
+
+        self._procs.append((Region.ACTIVE, proc, (), {}))
+
+
+class Bits(Leaf, Singular, _ProcIf, _TraceIf):
+    """Leaf-level btvector design component."""
 
     def __init__(self, name: str, parent: Module, dtype: type):
         Leaf.__init__(self, name, parent)
         Singular.__init__(self, dtype.xes())
         _ProcIf.__init__(self)
         self._dtype = dtype
         self._waves_change = None
         self._vcd_change = None
 
+    # Singular => State
+    def set_next(self, value):
+        if isinstance(value, str):
+            value = lit2vec(value)
+        assert isinstance(value, self._dtype)
+        super().set_next(value)
+
+    next = property(fset=set_next)
+
     def update(self):
         if self._waves_change and self.dirty():
             self._waves_change()
         if self._vcd_change and self.dirty():
             self._vcd_change()
         super().update()
 
+    # TraceIf
     def dump_waves(self, waves: defaultdict, pattern: str):
         if re.fullmatch(pattern, self.qualname):
             t = self._sim.time
             waves[t][self] = self._value
 
             def change():
                 t = self._sim.time
@@ -139,86 +228,83 @@
                 var = vcdw.register_var(
                     scope=self._parent.scope,
                     name=self.name,
                     var_type="string",
                     init=self._value.name,
                 )
                 self._vcd_change = lambda: vcdw.change(var, self._sim.time, self._next_value.name)
-        else:
+        elif issubclass(self._dtype, Vec):
             if re.match(pattern, self.qualname):
                 var = vcdw.register_var(
                     scope=self._parent.scope,
                     name=self.name,
                     var_type="reg",
                     size=len(self._value),
                     init=_vec2vcd(self._value),
                 )
                 self._vcd_change = lambda: vcdw.change(
                     var, self._sim.time, _vec2vcd(self._next_value)
                 )
 
-    def connect(self, src):
-        """Convenience function to reduce process boilerplate."""
-
-        async def proc():
-            while True:
-                await changed(src)
-                self.next = src.value
-
-        self._procs.append((Region.REACTIVE, proc, (), {}))
-
-
-class Bits(_TraceSingular):
-    """Leaf-level bitvector design component."""
-
 
 class Bit(Bits):
     """One-bit specialization of Bits that supports edge detection."""
 
     def __init__(self, name: str, parent: Module):
         super().__init__(name, parent, dtype=Vec[1])
 
     def is_neg(self) -> bool:
         """Return True when bit is stable 0 => 0."""
-        return self._value == zeros(1) and self._next_value == zeros(1)
+        return self._value == "1b0" and self._next_value == "1b0"
 
     def is_posedge(self) -> bool:
         """Return True when bit transitions 0 => 1."""
-        return self._value == zeros(1) and self._next_value == ones(1)
+        return self._value == "1b0" and self._next_value == "1b1"
 
     def is_negedge(self) -> bool:
         """Return True when bit transition 1 => 0."""
-        return self._value == ones(1) and self._next_value == zeros(1)
+        return self._value == "1b1" and self._next_value == "1b0"
 
     def is_pos(self) -> bool:
         """Return True when bit is stable 1 => 1."""
-        return self._value == ones(1) and self._next_value == ones(1)
+        return self._value == "1b1" and self._next_value == "1b1"
 
     async def posedge(self) -> State:
         """Suspend; resume execution at signal posedge."""
         self._sim.add_event(self, self.is_posedge)
         state = await SimAwaitable()
         return state
 
     async def negedge(self) -> State:
         """Suspend; resume execution at signal negedge."""
         self._sim.add_event(self, self.is_negedge)
         state = await SimAwaitable()
         return state
 
 
-class _TraceAggregate(Leaf, _TraceIf, Aggregate, _ProcIf):
-    """Combine hierarchy and sim semantics for aggregate data types."""
+class Array(Leaf, Aggregate, _ProcIf, _TraceIf):
+    """Leaf-level array of vec/enum/struct/union design components."""
 
     def __init__(self, name: str, parent: Module, dtype: type):
         Leaf.__init__(self, name, parent)
         Aggregate.__init__(self, dtype.xes())
         _ProcIf.__init__(self)
         self._dtype = dtype
 
+    def __getitem__(self, key: int | Vec):
+        if isinstance(key, int):
+            return super().__getitem__(key)
+        if isinstance(key, Vec):
+            try:
+                i = key.to_uint()
+            except ValueError:
+                return _ArrayXPropItem(self._dtype)
+            return super().__getitem__(i)
+        assert TypeError("Expected key to be int or Vec")
+
 
 class _ArrayXPropItem:
     """Array X-Prop item helper."""
 
     def __init__(self, dtype: type):
         self._dtype = dtype
 
@@ -229,36 +315,14 @@
 
     def _set_next(self, value):
         pass
 
     next = property(fset=_set_next)
 
 
-class Array(_TraceAggregate):
-    """Leaf-level array of bitvector/enum/struct/union design components."""
-
-    def __init__(self, name: str, parent: Module, shape: tuple[int, ...], dtype: type):
-        assert len(shape) == 1
-        super().__init__(name, parent, dtype)
-
-    def __getitem__(self, key: int | Vec):
-        match key:
-            case int():
-                return super().__getitem__(key)
-            case Vec():
-                try:
-                    i = key.to_uint()
-                except ValueError:
-                    return _ArrayXPropItem(self._dtype)
-                else:
-                    return super().__getitem__(i)
-            case _:
-                assert False
-
-
 def simify(d: Module | Bits | Bit | Array):
     """Add design processes to the simulator."""
     loop = get_loop()
     for node in d.iter_bfs():
         assert isinstance(node, _ProcIf)
         for region, func, args, kwargs in node.procs:
             loop.add_proc(region, func, *args, **kwargs)
```

### Comparing `seqlogic-0.2.0/src/seqlogic/hier.py` & `seqlogic-0.3.0/src/seqlogic/hier.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,15 @@
         if parent is not None:
             parent.add_child(self)
 
     @property
     def qualname(self) -> str:
         if self._parent is None:
             return f"/{self._name}"
-        else:
-            return f"{self._parent.qualname}/{self._name}"
+        return f"{self._parent.qualname}/{self._name}"
 
     def iter_bfs(self) -> Generator[Hierarchy, None, None]:
         yield self
         for child in self._children:
             yield from child.iter_bfs()
 
     def iter_dfs(self) -> Generator[Hierarchy, None, None]:
```

### Comparing `seqlogic-0.2.0/src/seqlogic/lbool.py` & `seqlogic-0.3.0/src/seqlogic/lbool.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # PyLint/PyRight are confused by MetaClass behavior
 # pyright: reportAttributeAccessIssue=false
 
 
 from __future__ import annotations
 
 import re
-from collections.abc import Generator, Iterable
+from collections.abc import Iterable
 from functools import cached_property, partial
 
 from .util import classproperty, clog2
 
 _ITEM_BITS = 2
 _ITEM_MASK = 0b11
 
@@ -346,14 +346,20 @@
 
     @classmethod
     def dcs(cls):
         obj = object.__new__(cls)
         obj._data = (1 << cls.nbits) - 1
         return obj
 
+    @classmethod
+    def xprop(cls, sel):
+        if sel.has_x():
+            return cls.xes()
+        return cls.dcs()
+
     def __init__(self, data: int):
         """Initialize.
 
         Args:
             data: lbool items packed into an int.
 
         Raises:
@@ -362,28 +368,23 @@
         self.check_data(data)
         self._data = data
 
     def __len__(self) -> int:
         return self._n
 
     def __getitem__(self, key: int | slice) -> Vec:
-        match key:
-            case int() as i:
-                d = self._get_item(self._norm_index(i))
-                return Vec[1](d)
-            case slice() as sl:
-                i, j = self._norm_slice(sl)
-                n, d = self._get_items(i, j)
-                return Vec[n](d)
-            case _:
-                raise TypeError("Expected key to be int or slice")
-
-    def __iter__(self) -> Generator[Vec[1], None, None]:
-        for i in range(self._n):
-            yield self.__getitem__(i)
+        if isinstance(key, int):
+            i = self._norm_index(key)
+            d = self._get_item(i)
+            return Vec[1](d)
+        if isinstance(key, slice):
+            i, j = self._norm_slice(key)
+            n, d = self._get_items(i, j)
+            return Vec[n](d)
+        raise TypeError("Expected key to be int or slice")
 
     def __str__(self) -> str:
         if self._n == 0:
             return ""
         prefix = f"{self._n}b"
         chars = []
         for i in range(self._n):
@@ -398,54 +399,66 @@
     def __bool__(self) -> bool:
         return self.to_uint() != 0
 
     def __int__(self) -> int:
         return self.to_int()
 
     # Comparison
-    def _eq(self, other: Vec) -> bool:
-        return self._n == other._n and self._data == other._data
-
-    def __eq__(self, other) -> bool:
-        match other:
-            case Vec():
-                return self._eq(other)
-            case str() as lit:
-                return self._match(lit)
-            case _:
-                return False
+    def __eq__(self, obj: object) -> bool:
+        if isinstance(obj, Vec[self._n]):
+            return self._data == obj.data
+        if isinstance(obj, str):
+            n, data = _lit2vec(obj)
+            return self._n == n and self._data == data
+        return False
 
     def __hash__(self) -> int:
         return hash(self._n) ^ hash(self._data)
 
     # Bitwise Arithmetic
     def __invert__(self) -> Vec:
         return self.not_()
 
-    def __or__(self, other: Vec) -> Vec:
+    def __or__(self, other: Vec | str) -> Vec:
         return self.or_(other)
 
-    def __and__(self, other: Vec) -> Vec:
+    def __and__(self, other: Vec | str) -> Vec:
         return self.and_(other)
 
-    def __xor__(self, other: Vec) -> Vec:
+    def __xor__(self, other: Vec | str) -> Vec:
         return self.xor(other)
 
-    def __lshift__(self, n: int) -> Vec:
+    def __lshift__(self, n: int | Vec) -> Vec:
         return self.lsh(n)[0]
 
-    def __rshift__(self, n: int) -> Vec:
+    def __rlshift__(self, other: Vec | str) -> Vec:
+        v = self._to_vec(other)
+        return v.__lshift__(self)
+
+    def __rshift__(self, n: int | Vec) -> Vec:
         return self.rsh(n)[0]
 
-    def __add__(self, other: Vec) -> Vec:
+    def __rrshift__(self, other: Vec | str) -> Vec:
+        v = self._to_vec(other)
+        return v.__rshift__(self)
+
+    def __add__(self, other: Vec | str) -> Vec:
         return self.add(other, ci=_Vec0)[0]
 
-    def __sub__(self, other: Vec) -> Vec:
+    def __radd__(self, other: Vec | str) -> Vec:
+        v = self._to_vec(other)
+        return v.__add__(self)
+
+    def __sub__(self, other: Vec | str) -> Vec:
         return self.sub(other)[0]
 
+    def __rsub__(self, other: Vec | str) -> Vec:
+        v = self._to_vec(other)
+        return v.__sub__(self)
+
     def __neg__(self) -> Vec:
         return self.neg()[0]
 
     @property
     def data(self) -> int:
         """Packed items."""
         return self._data
@@ -463,65 +476,67 @@
 
         y0 = x_10
         y1 = x_01
         y = y1 | y0
 
         return Vec[self._n](y)
 
-    def nor(self, other: Vec) -> Vec:
+    def nor(self, other: Vec | str) -> Vec:
         """Bitwise lifted NOR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains NOR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
-        x1_0 = other._bit_mask[0]
+        x1_0 = v._bit_mask[0]
         x1_01 = x1_0 << 1
-        x1_1 = other._bit_mask[1]
+        x1_1 = v._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_10 | x0_10 & x1_0 | x0_10 & x1_10
         y1 = x0_01 & x1_01
         y = y1 | y0
 
         return Vec[self._n](y)
 
-    def or_(self, other: Vec) -> Vec:
+    def or_(self, other: Vec | str) -> Vec:
         """Bitwise lifted OR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains OR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
 
-        x1_0 = other._bit_mask[0]
+        x1_0 = v._bit_mask[0]
         x1_01 = x1_0 << 1
-        x1_1 = other._bit_mask[1]
+        x1_1 = v._bit_mask[1]
 
         y0 = x0_0 & x1_0
         y1 = x0_01 & x1_1 | x0_1 & x1_01 | x0_1 & x1_1
         y = y1 | y0
 
         return Vec[self._n](y)
 
@@ -532,64 +547,66 @@
             One-bit vec, data contains OR reduction.
         """
         data = _0
         for i in range(self._n):
             data = or_(data, self._get_item(i))
         return Vec[1](data)
 
-    def nand(self, other: Vec) -> Vec:
+    def nand(self, other: Vec | str) -> Vec:
         """Bitwise lifted NAND.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains NAND result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
-        x1_0 = other._bit_mask[0]
+        x1_0 = v._bit_mask[0]
         x1_01 = x1_0 << 1
-        x1_1 = other._bit_mask[1]
+        x1_1 = v._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_10 & x1_10
         y1 = x0_01 & x1_01 | x0_01 & x1_1 | x0_1 & x1_01
         y = y1 | y0
 
         return Vec[self._n](y)
 
-    def and_(self, other: Vec) -> Vec:
+    def and_(self, other: Vec | str) -> Vec:
         """Bitwise lifted AND.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains AND result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
 
         x0_0 = self._bit_mask[0]
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
-        x1_0 = other._bit_mask[0]
-        x1_1 = other._bit_mask[1]
+        x1_0 = v._bit_mask[0]
+        x1_1 = v._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_0 | x0_0 & x1_10 | x0_10 & x1_0
         y1 = x0_1 & x1_1
         y = y1 | y0
 
         return Vec[self._n](y)
@@ -601,66 +618,68 @@
             One-bit vec, data contains AND reduction.
         """
         data = _1
         for i in range(self._n):
             data = and_(data, self._get_item(i))
         return Vec[1](data)
 
-    def xnor(self, other: Vec) -> Vec:
+    def xnor(self, other: Vec | str) -> Vec:
         """Bitwise lifted XNOR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains XNOR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
-        x1_0 = other._bit_mask[0]
+        x1_0 = v._bit_mask[0]
         x1_01 = x1_0 << 1
-        x1_1 = other._bit_mask[1]
+        x1_1 = v._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_10 | x0_10 & x1_0
         y1 = x0_01 & x1_01 | x0_1 & x1_1
         y = y1 | y0
 
         return Vec[self._n](y)
 
-    def xor(self, other: Vec) -> Vec:
+    def xor(self, other: Vec | str) -> Vec:
         """Bitwise lifted XOR.
 
         Args:
             other: vec of equal length.
 
         Returns:
             vec of equal length, data contains XOR result.
 
         Raises:
             ValueError: vec lengths do not match.
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
 
         x0_0 = self._bit_mask[0]
         x0_01 = x0_0 << 1
         x0_1 = self._bit_mask[1]
         x0_10 = x0_1 >> 1
 
-        x1_0 = other._bit_mask[0]
+        x1_0 = v._bit_mask[0]
         x1_01 = x1_0 << 1
-        x1_1 = other._bit_mask[1]
+        x1_1 = v._bit_mask[1]
         x1_10 = x1_1 >> 1
 
         y0 = x0_0 & x1_0 | x0_10 & x1_10
         y1 = x0_01 & x1_1 | x0_1 & x1_01
         y = y1 | y0
 
         return Vec[self._n](y)
@@ -732,186 +751,191 @@
         if self._n == 0:
             return 0
         sign = self._get_item(self._n - 1)
         if sign == _1:
             return -(self.not_().to_uint() + 1)
         return self.to_uint()
 
-    def eq(self, other: Vec) -> Vec[1]:
+    def eq(self, other: Vec | str) -> Vec[1]:
         """Equal operator.
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of self == other
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_uint() == other.to_uint()]
+            return (_Vec0, _Vec1)[self.to_uint() == v.to_uint()]
         except ValueError:
             return _VecX
 
-    def neq(self, other: Vec) -> Vec[1]:
+    def neq(self, other: Vec | str) -> Vec[1]:
         """Not Equal operator.
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of self != other
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_uint() != other.to_uint()]
+            return (_Vec0, _Vec1)[self.to_uint() != v.to_uint()]
         except ValueError:
             return _VecX
 
-    def ltu(self, other: Vec) -> Vec[1]:
+    def ltu(self, other: Vec | str) -> Vec[1]:
         """Less than operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) < unsigned(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_uint() < other.to_uint()]
+            return (_Vec0, _Vec1)[self.to_uint() < v.to_uint()]
         except ValueError:
             return _VecX
 
-    def lteu(self, other: Vec) -> Vec[1]:
+    def lteu(self, other: Vec | str) -> Vec[1]:
         """Less than or equal operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) ≤ unsigned(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_uint() <= other.to_uint()]
+            return (_Vec0, _Vec1)[self.to_uint() <= v.to_uint()]
         except ValueError:
             return _VecX
 
-    def lt(self, other: Vec) -> Vec[1]:
+    def lt(self, other: Vec | str) -> Vec[1]:
         """Less than operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) < signed(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_int() < other.to_int()]
+            return (_Vec0, _Vec1)[self.to_int() < v.to_int()]
         except ValueError:
             return _VecX
 
-    def lte(self, other: Vec) -> Vec[1]:
+    def lte(self, other: Vec | str) -> Vec[1]:
         """Less than or equal operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) ≤ signed(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_int() <= other.to_int()]
+            return (_Vec0, _Vec1)[self.to_int() <= v.to_int()]
         except ValueError:
             return _VecX
 
-    def gtu(self, other: Vec) -> Vec[1]:
+    def gtu(self, other: Vec | str) -> Vec[1]:
         """Greater than operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) > unsigned(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_uint() > other.to_uint()]
+            return (_Vec0, _Vec1)[self.to_uint() > v.to_uint()]
         except ValueError:
             return _VecX
 
-    def gteu(self, other: Vec) -> Vec[1]:
+    def gteu(self, other: Vec | str) -> Vec[1]:
         """Greater than or equal operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of unsigned(self) ≥ unsigned(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_uint() >= other.to_uint()]
+            return (_Vec0, _Vec1)[self.to_uint() >= v.to_uint()]
         except ValueError:
             return _VecX
 
-    def gt(self, other: Vec) -> Vec[1]:
+    def gt(self, other: Vec | str) -> Vec[1]:
         """Greater than operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) > signed(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_int() > other.to_int()]
+            return (_Vec0, _Vec1)[self.to_int() > v.to_int()]
         except ValueError:
             return _VecX
 
-    def gte(self, other: Vec) -> Vec[1]:
+    def gte(self, other: Vec | str) -> Vec[1]:
         """Greater than or equal operator (signed).
 
         Args:
             other: vec of equal length.
 
         Returns:
             Vec[1] result of signed(self) ≥ signed(other)
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
         try:
-            return (_Vec0, _Vec1)[self.to_int() >= other.to_int()]
+            return (_Vec0, _Vec1)[self.to_int() >= v.to_int()]
         except ValueError:
             return _VecX
 
-    def _match(self, pattern: str | Vec) -> bool:
+    def _match(self, pattern: Vec | str) -> bool:
         """Pattern match operator."""
-        match pattern:
-            case str() as lit:
-                pattern = lit2vec(lit)
-            case Vec():
-                pass
-            case _:
-                raise TypeError("Expected pattern to be str or Vec")
+        if isinstance(pattern, str):
+            pattern = lit2vec(pattern)
 
         self.check_len(len(pattern))
 
-        # Propagate X
         if self.has_x() or pattern.has_x():
             return False
 
         for i in range(self._n):
             a = self._get_item(i)
             b = pattern._get_item(i)
             # Mismatch on (0b01, 0b10) or (0b10, 0b01)
             if a ^ b == 0b11:
                 return False
+
         return True
 
     def zext(self, n: int) -> Vec:
         """Zero extend by n bits.
 
         Args:
             n: Non-negative number of bits.
@@ -957,26 +981,21 @@
         Returns:
             vec left-shifted by n bits. If ci is provided, use it for shift
             input. Otherwise use zeros.
 
         Raises:
             ValueError: If n or ci are invalid/inconsistent.
         """
-        match n:
-            case int():
-                pass
-            case Vec():
-                if n.has_x():
-                    return self.xes(), _VecE
-                elif n.has_dc():
-                    return self.dcs(), _VecE
-                else:
-                    n = n.to_uint()
-            case _:
-                raise TypeError("Expected n to be int or Vec")
+        if isinstance(n, Vec):
+            if n.has_x():
+                return self.xes(), _VecE
+            if n.has_dc():
+                return self.dcs(), _VecE
+            n = n.to_uint()
+
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
             return self, _VecE
         if ci is None:
             ci = Vec[n](_fill(_0, n))
         elif len(ci) != n:
@@ -995,26 +1014,21 @@
         Returns:
             vec right-shifted by n bits. If ci is provided, use it for shift
             input. Otherwise use zeros.
 
         Raises:
             ValueError: If n or ci are invalid/inconsistent.
         """
-        match n:
-            case int():
-                pass
-            case Vec():
-                if n.has_x():
-                    return self.xes(), _VecE
-                elif n.has_dc():
-                    return self.dcs(), _VecE
-                else:
-                    n = n.to_uint()
-            case _:
-                raise TypeError("Expected n to be int or Vec")
+        if isinstance(n, Vec):
+            if n.has_x():
+                return self.xes(), _VecE
+            if n.has_dc():
+                return self.dcs(), _VecE
+            n = n.to_uint()
+
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
             return self, _VecE
         if ci is None:
             ci = Vec[n](_fill(_0, n))
         elif len(ci) != n:
@@ -1031,51 +1045,47 @@
 
         Returns:
             vec arithmetically right-shifted by n bits.
 
         Raises:
             ValueError: If n is invalid.
         """
-        match n:
-            case int():
-                pass
-            case Vec():
-                if n.has_x():
-                    return self.xes(), _VecE
-                elif n.has_dc():
-                    return self.dcs(), _VecE
-                else:
-                    n = n.to_uint()
-            case _:
-                raise TypeError("Expected n to be int or Vec")
+        if isinstance(n, Vec):
+            if n.has_x():
+                return self.xes(), _VecE
+            if n.has_dc():
+                return self.dcs(), _VecE
+            n = n.to_uint()
+
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
             return self, _VecE
         sign = self._get_item(self._n - 1)
         co, sh = self[:n], self[n:]
         y = Vec[self._n](sh._data | (_fill(sign, n) << sh.nbits))
         return y, co
 
-    def add(self, other: Vec, ci: Vec[1]) -> tuple[Vec, Vec[1]]:
+    def add(self, other: Vec | str, ci: Vec[1]) -> tuple[Vec, Vec[1]]:
         """Twos complement addition.
 
         Args:
             other: vec of equal length.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
 
         Raises:
             ValueError: vec lengths are invalid/inconsistent.
         """
-        self.check_len(len(other))
+        v = self._to_vec(other)
+        self.check_len(len(v))
 
         # Rename for readability
-        n, a, b = self._n, self, other
+        n, a, b = self._n, self, v
 
         if a.has_x() or b.has_x() or ci.has_x():
             return Vec[n](_fill(_X, n)), _VecX
         if a.has_dc() or b.has_dc() or ci.has_dc():
             return Vec[n](_fill(_W, n)), _VecW
 
         s = a.to_uint() + b.to_uint() + ci.to_uint()
@@ -1086,50 +1096,40 @@
             s >>= 1
 
         # Carry out is True if there is leftover sum data
         co = (_Vec0, _Vec1)[s != 0]
 
         return Vec[n](data), co
 
-    def sub(self, other: Vec) -> tuple[Vec, Vec[1]]:
+    def sub(self, other: Vec | str) -> tuple[Vec, Vec[1]]:
         """Twos complement subtraction.
 
         Args:
             other: vec of equal length.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
 
         Raises:
             ValueError: vec lengths are invalid/inconsistent.
         """
-        return self.add(other.not_(), ci=_Vec1)
+        v = self._to_vec(other)
+        return self.add(v.not_(), ci=_Vec1)
 
     def neg(self) -> tuple[Vec, Vec[1]]:
         """Twos complement negation.
 
         Computed using 0 - self.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
         """
         zero = Vec[self._n](_fill(_0, self._n))
         return zero.sub(self)
 
-    def ite(self, v1: Vec, v0: Vec | None = None) -> Vec:
-        """If then else operator."""
-        if self.has_unknown():
-            return xes(v1._n)
-        if v0 is None:
-            v0 = dcs(v1._n)
-        else:
-            if v1._n != v0._n:
-                raise ValueError("Expected matching operand lengths")
-        return v1 if self else v0
-
     def _count(self, byte_cnt: dict[int, int], item: int) -> int:
         y = 0
         n, data = self._n, self._data
 
         stride = 4
         while n >= stride:
             y += byte_cnt[data & _BYTE_MASK]
@@ -1179,14 +1179,22 @@
         """Return True if vec contains at least one DC item."""
         return self.count_dcs() != 0
 
     def has_unknown(self) -> bool:
         """Return True if vec contains at least one X/DC item."""
         return self.count_unknown() != 0
 
+    def _to_vec(self, obj: Vec | str) -> Vec:
+        if isinstance(obj, Vec[self._n]):
+            return obj
+        if isinstance(obj, str):
+            return lit2vec(obj)
+        s = f"Expected Vec[{self._n}] or lit, got {obj.__class__.__name__}"
+        raise TypeError(s)
+
     def _norm_index(self, index: int) -> int:
         a, b = -self._n, self._n
         if not a <= index < b:
             s = f"Expected index in [{a}, {b}), got {index}"
             raise IndexError(s)
         # Normalize negative start index
         if index < 0:
@@ -1417,54 +1425,52 @@
             return bools2vec([x, *rst])
         case str() as lit:
             return lit2vec(lit)
         case _:
             raise TypeError(f"Invalid input: {obj}")
 
 
-def cat(*objs: int | str | Vec) -> Vec:
+def cat(*objs: Vec | int | str) -> Vec:
     """Concatenate a sequence of vectors.
 
     Args:
-        objs: a sequence of bool/lit/vec objects.
+        objs: a sequence of vec/bool/lit objects.
 
     Returns:
         A Vec instance.
 
     Raises:
         TypeError: If input obj is invalid.
     """
     if len(objs) == 0:
         return _VecE
 
     # Convert inputs
     vs = []
     for obj in objs:
-        match obj:
-            case 0 | 1 as x:
-                vs.append((_Vec0, _Vec1)[x])
-            case str() as lit:
-                v = lit2vec(lit)
-                vs.append(v)
-            case Vec() as v:
-                vs.append(v)
-            case _:
-                raise TypeError(f"Invalid input: {obj}")
+        if isinstance(obj, Vec):
+            vs.append(obj)
+        elif obj in (0, 1):
+            vs.append((_Vec0, _Vec1)[obj])
+        elif isinstance(obj, str):
+            vs.append(lit2vec(obj))
+        else:
+            raise TypeError(f"Invalid input: {obj}")
 
     if len(vs) == 1:
         return vs[0]
 
     n, data = 0, 0
     for v in vs:
         data |= v.data << (_ITEM_BITS * n)
         n += len(v)
     return Vec[n](data)
 
 
-def rep(obj: int | str | Vec, n: int) -> Vec:
+def rep(obj: Vec | int | str, n: int) -> Vec:
     """Repeat a vector n times."""
     objs = [obj] * n
     return cat(*objs)
 
 
 def xes(n: int) -> Vec:
     """Return a vec packed with n X items."""
@@ -1546,26 +1552,26 @@
         for data, name in data2name.items():
             obj = object.__new__(enum)  # pyright: ignore[reportArgumentType]
             obj._data = data
             obj._name = name
             setattr(enum, name, obj)
 
         # Override Vec __new__ method
-        def _new(cls, arg: str | int | Vec):
-            match arg:
-                case str() as lit:
-                    n, data = _lit2vec(lit)
-                    cls.check_len(n)
-                case int() as data:
-                    cls.check_data(data)
-                case Vec() as v:
-                    n, data = len(v), v.data
-                    cls.check_len(n)
-                case _:
-                    raise TypeError("Expected arg to be str, int, or Vec")
+        def _new(cls, arg: Vec | str | int):
+            if isinstance(arg, Vec[cls._n]):
+                data = arg.data
+            elif isinstance(arg, str):
+                n, data = _lit2vec(arg)
+                cls.check_len(n)
+            elif isinstance(arg, int):
+                data = arg
+                cls.check_data(data)
+            else:
+                s = f"Expected arg to be Vec[{cls._n}], str, or int"
+                raise TypeError(s)
             try:
                 obj = getattr(cls, data2name[data])
             except KeyError:
                 obj = object.__new__(enum)  # pyright: ignore[reportArgumentType]
                 obj._data = data
                 obj._name = f"{cls.__name__}({Vec[cls._n].__str__(obj)})"
             return obj
@@ -1594,14 +1600,16 @@
     lines = []
     s = ", ".join(f"{fn}: {ft.__name__} | None = None" for fn, ft in fields)
     lines.append(f"def struct_init(self, {s}):\n")
     lines.append("    data = 0\n")
     for fn, _ in fields:
         s = f"Expected field {fn} to have {{exp}} bits, got {{got}}"
         lines.append(f"    if {fn} is not None:\n")
+        lines.append(f"        if isinstance({fn}, str):\n")
+        lines.append(f"            {fn} = lit2vec({fn})\n")
         lines.append(f"        got, exp = len({fn}), self._{fn}_size\n")
         lines.append("        if got != exp:\n")
         lines.append(f'            raise TypeError(f"{s}")\n')
         lines.append(f"        data |= {fn}.data << ({_ITEM_BITS} * self._{fn}_base)\n")
     lines.append("    self._data = data\n")
     return "".join(lines)
 
@@ -1634,15 +1642,15 @@
 
         # Create Struct class
         n = sum(field_type._n for _, field_type in fields)
         struct = super().__new__(mcs, name, bases + (Vec[n],), struct_attrs)
 
         # Override Vec __init__ method
         source = _struct_init_source(fields)
-        globals_ = {"Vec": Vec}
+        globals_ = {"Vec": Vec, "lit2vec": lit2vec}
         globals_.update({ft.__name__: ft for _, ft in fields})
         locals_ = {}
         exec(source, globals_, locals_)  # pylint: disable=exec-used
         struct.__init__ = locals_["struct_init"]
 
         # Override Vec __str__ method
         def _str(self):
```

### Comparing `seqlogic-0.2.0/src/seqlogic/sim.py` & `seqlogic-0.3.0/src/seqlogic/sim.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/src/seqlogic/util.py` & `seqlogic-0.3.0/src/seqlogic/util.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/src/seqlogic.egg-info/PKG-INFO` & `seqlogic-0.3.0/src/seqlogic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.2.0
+Version: 0.3.0
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.2.0/src/seqlogic.egg-info/SOURCES.txt` & `seqlogic-0.3.0/src/seqlogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_aes.py` & `seqlogic-0.3.0/tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_bits.py` & `seqlogic-0.3.0/tests/test_bits.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_enum.py` & `seqlogic-0.3.0/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_fsm.py` & `seqlogic-0.3.0/tests/test_fsm.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_gray.py` & `seqlogic-0.3.0/tests/test_gray.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_hier.py` & `seqlogic-0.3.0/tests/test_hier.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_lbool.py` & `seqlogic-0.3.0/tests/test_lbool.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,14 @@
 
 def test_vec_eq():
     assert Vec[0](0) == Vec[0](0)
     assert Vec[4](0b10_01_10_01) == Vec[4](0b10_01_10_01)
     assert Vec[4](0b10_01_10_01) != Vec[4](0b01_10_01_10)
     assert Vec[4](0b10_01_10_01) == "4b1010"
     assert Vec[4](0b10_01_10_01) != "4b0101"
-    assert Vec[4](0b10_01_10_01) == "4b----"
 
 
 def test_vec_hash():
     s = set()
     s.add(lbool.uint2vec(0))
     s.add(lbool.uint2vec(1))
     s.add(lbool.uint2vec(2))
```

### Comparing `seqlogic-0.2.0/tests/test_lfsr.py` & `seqlogic-0.3.0/tests/test_lfsr.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_sim.py` & `seqlogic-0.3.0/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.2.0/tests/test_struct.py` & `seqlogic-0.3.0/tests/test_struct.py`

 * *Files identical despite different names*

