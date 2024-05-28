# Comparing `tmp/buckshot-roulette-0.1.0.tar.gz` & `tmp/buckshot_roulette-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buckshot-roulette-0.1.0.tar", last modified: Fri Apr 12 05:32:20 2024, max compression
+gzip compressed data, was "buckshot_roulette-0.1.1.tar", last modified: Tue May 28 16:37:50 2024, max compression
```

## Comparing `buckshot-roulette-0.1.0.tar` & `buckshot_roulette-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/buckshot_roulette/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/buckshot_roulette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/buckshot_roulette/ai.py
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/buckshot_roulette/game.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:32:20.236260 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 05:32:20.000000 buckshot-roulette-0.1.0/buckshot_roulette.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-12 05:32:15.000000 buckshot-roulette-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:32:20.240260 buckshot-roulette-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:37:50.618602 buckshot_roulette-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-28 16:37:46.000000 buckshot_roulette-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 16:37:50.618602 buckshot_roulette-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-28 16:37:46.000000 buckshot_roulette-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:37:50.618602 buckshot_roulette-0.1.1/buckshot_roulette/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-28 16:37:46.000000 buckshot_roulette-0.1.1/buckshot_roulette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-28 16:37:46.000000 buckshot_roulette-0.1.1/buckshot_roulette/ai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-05-28 16:37:46.000000 buckshot_roulette-0.1.1/buckshot_roulette/game.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:37:50.618602 buckshot_roulette-0.1.1/buckshot_roulette.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-28 16:37:50.000000 buckshot_roulette-0.1.1/buckshot_roulette.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 16:37:50.000000 buckshot_roulette-0.1.1/buckshot_roulette.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:37:50.000000 buckshot_roulette-0.1.1/buckshot_roulette.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 16:37:50.000000 buckshot_roulette-0.1.1/buckshot_roulette.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-28 16:37:46.000000 buckshot_roulette-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:37:50.618602 buckshot_roulette-0.1.1/setup.cfg
```

### Comparing `buckshot-roulette-0.1.0/LICENSE` & `buckshot_roulette-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buckshot-roulette-0.1.0/PKG-INFO` & `buckshot_roulette-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckshot-roulette
-Version: 0.1.0
+Version: 0.1.1
 Summary: Buckshot Roulette library for python, with complete game features & reasonable efficiency.
 Author: Bytestorm
 Project-URL: Homepage, https://github.com/Bytestorm5/Buckshot-Roulette-Python
 Project-URL: Issues, https://github.com/Bytestorm5/Buckshot-Roulette-Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `buckshot-roulette-0.1.0/README.md` & `buckshot_roulette-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `buckshot-roulette-0.1.0/buckshot_roulette/game.py` & `buckshot_roulette-0.1.1/buckshot_roulette/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,51 @@
         return self.__getattribute__(key)
 
     def __setitem__(self, key, value):
         self.__setattr__(key, value)
 
     def __delitem__(self, key):
         self.__setattr__(key, 0)
+    
+    def __iter__(self):
+        return ItemIterable(self)
+
+    def __str__(self):
+        items = ', '.join(f'{key}={self[key]}' for key in self if self[key] > 0)
+        return f"Items({items})"
+
+    def __repr__(self):
+        return self.__str__()
+class ItemIterable():
+    def __init__(self, data: Items):
+        self.data: Items = data
+        self.index = 0
+
+    def __iter__(self):
+        return self
+
+    def __next__(self):
+        if self.index < len(BuckshotRoulette.POSSIBLE_ITEMS):
+            while self.index < len(BuckshotRoulette.POSSIBLE_ITEMS) and self.data[BuckshotRoulette.POSSIBLE_ITEMS[self.index]] < 1:
+                self.index += 1                
+            if self.index >= len(BuckshotRoulette.POSSIBLE_ITEMS):
+                raise StopIteration
+            
+            item = BuckshotRoulette.POSSIBLE_ITEMS[self.index]
+            self.index += 1
+            return item
+        else:
+            raise StopIteration
 
 class BuckshotRoulette:
     POSSIBLE_ITEMS = ['handcuffs', 'magnifying_glass', 'beer', 'cigarettes', 'saw', 'inverter', 'burner_phone', 'meds', 'adrenaline']
     ITEM_CAPS = Items(handcuffs=1, magnifying_glass=3, beer=2, cigarettes=1, saw=3, inverter=8, burner_phone=1, meds=1, adrenaline=2)
-    def __init__(self, charge_count, total_rounds = None, live_rounds = None):
-        self.max_charges = charge_count
-        self.charges = [charge_count, charge_count]
+    def __init__(self, charge_count = None, total_rounds = None, live_rounds = None):
+        self.max_charges = charge_count if charge_count else random.randint(2, 4)
+        self.charges = [self.max_charges, self.max_charges]
         self.current_turn = 0
         
         total = total_rounds if total_rounds else random.randint(2, 8)
         live = total // 2 if live_rounds == None else live_rounds
         if live > total:
             raise ValueError("Live Rounds must be less than Total Rounds")
         
@@ -52,16 +82,16 @@
         self._skip_next = False
         
         self.chamber_public = None
         self.give_items(random.randint(2, 5))       
 
     def new_rounds(self, drop_items = True):
         total = random.randint(2, 8)
-        live = random.randint(1, total-1)
-        self._shotgun = ([True] * live) + ([False * (total - live)])
+        live = total // 2
+        self._shotgun = ([True] * live) + ([False] * (total - live))
         random.shuffle(self._shotgun)
         if drop_items:
             self.give_items(random.randint(2, 5))
     
     def give_items(self, item_count):
         for player in self.items:
             if player.item_count() == 8:
@@ -193,15 +223,15 @@
                 items.burner_phone -= 1
                 if len(self._shotgun) > 1:
                     idx = random.randint(1, len(self._shotgun)-1)
                     out_val = (idx, self._shotgun[idx])
             case 'meds':
                 items.meds -= 1
                 if random.random() > 0.5:
-                    self.charges[self.current_turn] = max(self.charges[self.current_turn] + 2, self.max_charges)
+                    self.charges[self.current_turn] = min(self.charges[self.current_turn] + 2, self.max_charges)
                 else:
                     self.charges[self.current_turn] -= 1
             case 'adrenaline':
                 items.adrenaline -= 1
                 self._active_items.adrenaline += 1
```

### Comparing `buckshot-roulette-0.1.0/buckshot_roulette.egg-info/PKG-INFO` & `buckshot_roulette-0.1.1/buckshot_roulette.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buckshot-roulette
-Version: 0.1.0
+Version: 0.1.1
 Summary: Buckshot Roulette library for python, with complete game features & reasonable efficiency.
 Author: Bytestorm
 Project-URL: Homepage, https://github.com/Bytestorm5/Buckshot-Roulette-Python
 Project-URL: Issues, https://github.com/Bytestorm5/Buckshot-Roulette-Python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `buckshot-roulette-0.1.0/pyproject.toml` & `buckshot_roulette-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "buckshot-roulette"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Bytestorm" },
 ]
 description = "Buckshot Roulette library for python, with complete game features & reasonable efficiency."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

