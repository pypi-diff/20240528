# Comparing `tmp/istr_python-1.0.5.tar.gz` & `tmp/istr_python-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-1.0.5.tar", last modified: Fri May 24 12:43:15 2024, max compression
+gzip compressed data, was "istr_python-1.0.6.tar", last modified: Tue May 28 08:03:37 2024, max compression
```

## Comparing `istr_python-1.0.5.tar` & `istr_python-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 12:43:15.677451 istr_python-1.0.5/
--rw-rw-rw-   0        0        0    16546 2024-05-24 12:43:15.673514 istr_python-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    15382 2024-05-20 18:51:02.000000 istr_python-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 12:43:15.611764 istr_python-1.0.5/istr/
--rw-rw-rw-   0        0        0     1100 2024-05-14 13:17:20.000000 istr_python-1.0.5/istr/LICENSE.txt
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.5/istr/__init__.py
--rw-rw-rw-   0        0        0    18824 2024-05-24 12:42:42.000000 istr_python-1.0.5/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-05-24 12:43:15.670448 istr_python-1.0.5/istr_python.egg-info/
--rw-rw-rw-   0        0        0    16546 2024-05-24 12:43:15.000000 istr_python-1.0.5/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-05-24 12:43:15.000000 istr_python-1.0.5/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 12:43:15.000000 istr_python-1.0.5/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-24 12:43:15.000000 istr_python-1.0.5/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      711 2024-05-24 12:43:08.000000 istr_python-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-24 12:43:15.678466 istr_python-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-24 12:43:15.666446 istr_python-1.0.5/tests/
--rw-rw-rw-   0        0        0    17509 2024-05-24 12:40:11.000000 istr_python-1.0.5/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:37.101692 istr_python-1.0.6/
+-rw-rw-rw-   0        0        0    17870 2024-05-28 08:03:37.098111 istr_python-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    16653 2024-05-28 08:01:54.000000 istr_python-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:37.050061 istr_python-1.0.6/istr/
+-rw-rw-rw-   0        0        0     1100 2024-05-14 13:17:20.000000 istr_python-1.0.6/istr/LICENSE.txt
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.6/istr/__init__.py
+-rw-rw-rw-   0        0        0    19097 2024-05-28 08:02:50.000000 istr_python-1.0.6/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:37.095036 istr_python-1.0.6/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    17870 2024-05-28 08:03:37.000000 istr_python-1.0.6/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-05-28 08:03:37.000000 istr_python-1.0.6/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:03:37.000000 istr_python-1.0.6/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-28 08:03:37.000000 istr_python-1.0.6/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      711 2024-05-28 08:03:28.000000 istr_python-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:03:37.102693 istr_python-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:37.090919 istr_python-1.0.6/tests/
+-rw-rw-rw-   0        0        0    19381 2024-05-28 07:57:40.000000 istr_python-1.0.6/tests/test_istr.py
```

### Comparing `istr_python-1.0.5/PKG-INFO` & `istr_python-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -395,14 +395,66 @@
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
+#### itertools with istrs
+All methods in itertools are also available directly from istr.
+Note that the result is istr-ed (apart from groupby and tee).
+
+The following class methods are supported (provided their counterpart exists in the installed Python version's itertools):
+
+- istr.accumulate
+- istr.chain
+- istr.combinations
+- istr.combinations_with_replacement
+- istr.compress
+- istr.count
+- istr.cycle
+- istr.dropwhile
+- istr.filterfalse
+- istr.groupby (not istr-ed)
+- istr.islice
+- istr.pairwise
+- istr.permutations
+- istr.product
+- istr.repeat
+- istr.starmap
+- istr.takewhile
+- istr.tee (not istr-ed)
+- istr.zip_longest
+
+This can be handy as these methods don't have to be imported from itertools anymore.
+
+All methods have exactly the same (optional) parameters as their itertools counterpart.
+
+For example:
+
+```
+list(istr.repeat(1, 4)) ==> [istr('1'), istr('1'), istr('1'), istr('1')]
+next(istr.count(3)) ==> istr('3')
+```
+
+One more example:
+
+```
+for t in istr.permutations(range(3)):
+    print(t)
+```
+results in
+```
+(istr('0'), istr('1'), istr('2'))
+(istr('0'), istr('2'), istr('1'))
+(istr('1'), istr('0'), istr('2'))
+(istr('1'), istr('2'), istr('0'))
+(istr('2'), istr('0'), istr('1'))
+(istr('2'), istr('1'), istr('0'))
+```
 
 #### concatenate an iterable
 
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `
@@ -634,30 +686,31 @@
 _                    x         istr(20) - 3 ==> istr('17')
 *                    x         istr(20) * 3 ==> istr('60')
 /                    x         istr(20) / 3 ==> istr('6')
 //                   x         istr(20) // 3 ==> istr('6')
 %                    x         istr(20) % 3 ==> istr('2')
 divmod               x         divmod(istr(20), 3) ==> (istr('6'), istr('2'))
 **                   x         istr(2) ** 3 ==> istr('8')
-@                         x    istr(20) @ 3 ==> istr('202020')
-==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
-|                         x    istr(20) | 5 ==> istr('205')
+<=, <, >, >=         x         istr('100') > istr('2') ==> True
 abs                  x         abs(istr(-20)) ==> istr('20')
+==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
 bool                 x    x *) bool(istr(' 0 ')) ==> False | istr('') ==> False
-<=, <, >, >=         x         istr('100') > istr('2') ==> True
+@                         x    istr(20) @ 3 ==> istr('202020')
+|                         x    istr(20) | '5' ==> istr('205')
 slicing                   x    istr(12345)[1:3] ==> istr('23')
-iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
+iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')]
 len                       x    len(istr(' 20 ')) ==> 4
-count                     x    istr(100),count('0') ==> 2
+count                     x    istr(100).count('0') ==> 2
 index                     x    istr(' 100 ').index('0') ==> 2
 split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
-string format             x    f"|{istr((1234):6}|" ==> '|1234  |'
+string format             x    f"|{istr(1234):6}|" ==> '|1234  |'
 other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
                                istr('aAbBcC').islower() ==> False
                                istr('  abc   ').strip() ==> istr('abc')
+                               ...
 -----------------------------------------------------------------------------------------
 *) str is applied if is_int() is False
 
 ```
 ### Test script
 There's an extensive pytest script in the `\tests` directory.
```

### Comparing `istr_python-1.0.5/README.md` & `istr_python-1.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -382,14 +382,66 @@
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
+#### itertools with istrs
+All methods in itertools are also available directly from istr.
+Note that the result is istr-ed (apart from groupby and tee).
+
+The following class methods are supported (provided their counterpart exists in the installed Python version's itertools):
+
+- istr.accumulate
+- istr.chain
+- istr.combinations
+- istr.combinations_with_replacement
+- istr.compress
+- istr.count
+- istr.cycle
+- istr.dropwhile
+- istr.filterfalse
+- istr.groupby (not istr-ed)
+- istr.islice
+- istr.pairwise
+- istr.permutations
+- istr.product
+- istr.repeat
+- istr.starmap
+- istr.takewhile
+- istr.tee (not istr-ed)
+- istr.zip_longest
+
+This can be handy as these methods don't have to be imported from itertools anymore.
+
+All methods have exactly the same (optional) parameters as their itertools counterpart.
+
+For example:
+
+```
+list(istr.repeat(1, 4)) ==> [istr('1'), istr('1'), istr('1'), istr('1')]
+next(istr.count(3)) ==> istr('3')
+```
+
+One more example:
+
+```
+for t in istr.permutations(range(3)):
+    print(t)
+```
+results in
+```
+(istr('0'), istr('1'), istr('2'))
+(istr('0'), istr('2'), istr('1'))
+(istr('1'), istr('0'), istr('2'))
+(istr('1'), istr('2'), istr('0'))
+(istr('2'), istr('0'), istr('1'))
+(istr('2'), istr('1'), istr('0'))
+```
 
 #### concatenate an iterable
 
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `
@@ -621,30 +673,31 @@
 _                    x         istr(20) - 3 ==> istr('17')
 *                    x         istr(20) * 3 ==> istr('60')
 /                    x         istr(20) / 3 ==> istr('6')
 //                   x         istr(20) // 3 ==> istr('6')
 %                    x         istr(20) % 3 ==> istr('2')
 divmod               x         divmod(istr(20), 3) ==> (istr('6'), istr('2'))
 **                   x         istr(2) ** 3 ==> istr('8')
-@                         x    istr(20) @ 3 ==> istr('202020')
-==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
-|                         x    istr(20) | 5 ==> istr('205')
+<=, <, >, >=         x         istr('100') > istr('2') ==> True
 abs                  x         abs(istr(-20)) ==> istr('20')
+==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
 bool                 x    x *) bool(istr(' 0 ')) ==> False | istr('') ==> False
-<=, <, >, >=         x         istr('100') > istr('2') ==> True
+@                         x    istr(20) @ 3 ==> istr('202020')
+|                         x    istr(20) | '5' ==> istr('205')
 slicing                   x    istr(12345)[1:3] ==> istr('23')
-iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
+iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')]
 len                       x    len(istr(' 20 ')) ==> 4
-count                     x    istr(100),count('0') ==> 2
+count                     x    istr(100).count('0') ==> 2
 index                     x    istr(' 100 ').index('0') ==> 2
 split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
-string format             x    f"|{istr((1234):6}|" ==> '|1234  |'
+string format             x    f"|{istr(1234):6}|" ==> '|1234  |'
 other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
                                istr('aAbBcC').islower() ==> False
                                istr('  abc   ').strip() ==> istr('abc')
+                               ...
 -----------------------------------------------------------------------------------------
 *) str is applied if is_int() is False
 
 ```
 ### Test script
 There's an extensive pytest script in the `\tests` directory.
```

### Comparing `istr_python-1.0.5/istr/LICENSE.txt` & `istr_python-1.0.6/istr/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `istr_python-1.0.5/istr/istr.py` & `istr_python-1.0.6/istr/istr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 import functools
 import math
 import copy
+import itertools
 
 """
 Note: the changelog is now in changelog.md
 
 You can view the changelog on www.salabim.org/istr/changelog.html
 
 The readme can be viewed on www.salabim.org/istr/readme.html
@@ -283,15 +284,15 @@
                 return self._as_int == other._as_int
         if isinstance(other, str):
             return super().__eq__(other)
         try:
             return self._as_int == self._to_int(other)
         except Exception:
             return False
-            
+
     def __ne__(self, other):
         return not self == other
 
     def __repr__(self):
         return self._as_repr
 
     def __bool__(self):
@@ -387,14 +388,25 @@
 
     for name in (
         "capitalize casefold center expandtabs format join ljust lower lstrip partition removeprefix "
         "removesuffix replace rjust rpartition rsplit rstrip split strip swapcase title translate upper zfill"
     ).split():
         locals()[name] = functools.partialmethod(_str_method, name)
 
+    @classmethod
+    def _itertools_method(cls, name, *args, **kwargs):
+        return cls(getattr(itertools, name)(*args, **kwargs))
+
+    for name in dir(itertools):
+        if not name.startswith("__"):
+            if name in ("groupby", "tee"):
+                locals()[name] = getattr(itertools, name)
+            else:
+                locals()[name] = functools.partialmethod(_itertools_method, name)
+
     def is_int(self):
         return self._as_int is not self._nan
 
     @classmethod
     def concat(cls, iterable):
         return map(lambda x: istr("").join(x), istr(iterable))
 
@@ -535,18 +547,11 @@
 
         result = istr("".join(result))
         cls._digits_cache[key] = result
         return result
 
 
 def main():
-    print(istr.digits())
-
-    print(repr(istr.digits()))
-    print(int(istr.digits()))
-
-    with istr.base(16):
-        print(int(istr.digits()))
+    ...
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `istr_python-1.0.5/istr_python.egg-info/PKG-INFO` & `istr_python-1.0.6/istr_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 1.0.5
+Version: 1.0.6
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -395,14 +395,66 @@
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
+#### itertools with istrs
+All methods in itertools are also available directly from istr.
+Note that the result is istr-ed (apart from groupby and tee).
+
+The following class methods are supported (provided their counterpart exists in the installed Python version's itertools):
+
+- istr.accumulate
+- istr.chain
+- istr.combinations
+- istr.combinations_with_replacement
+- istr.compress
+- istr.count
+- istr.cycle
+- istr.dropwhile
+- istr.filterfalse
+- istr.groupby (not istr-ed)
+- istr.islice
+- istr.pairwise
+- istr.permutations
+- istr.product
+- istr.repeat
+- istr.starmap
+- istr.takewhile
+- istr.tee (not istr-ed)
+- istr.zip_longest
+
+This can be handy as these methods don't have to be imported from itertools anymore.
+
+All methods have exactly the same (optional) parameters as their itertools counterpart.
+
+For example:
+
+```
+list(istr.repeat(1, 4)) ==> [istr('1'), istr('1'), istr('1'), istr('1')]
+next(istr.count(3)) ==> istr('3')
+```
+
+One more example:
+
+```
+for t in istr.permutations(range(3)):
+    print(t)
+```
+results in
+```
+(istr('0'), istr('1'), istr('2'))
+(istr('0'), istr('2'), istr('1'))
+(istr('1'), istr('0'), istr('2'))
+(istr('1'), istr('2'), istr('0'))
+(istr('2'), istr('0'), istr('1'))
+(istr('2'), istr('1'), istr('0'))
+```
 
 #### concatenate an iterable
 
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
 `
@@ -634,30 +686,31 @@
 _                    x         istr(20) - 3 ==> istr('17')
 *                    x         istr(20) * 3 ==> istr('60')
 /                    x         istr(20) / 3 ==> istr('6')
 //                   x         istr(20) // 3 ==> istr('6')
 %                    x         istr(20) % 3 ==> istr('2')
 divmod               x         divmod(istr(20), 3) ==> (istr('6'), istr('2'))
 **                   x         istr(2) ** 3 ==> istr('8')
-@                         x    istr(20) @ 3 ==> istr('202020')
-==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
-|                         x    istr(20) | 5 ==> istr('205')
+<=, <, >, >=         x         istr('100') > istr('2') ==> True
 abs                  x         abs(istr(-20)) ==> istr('20')
+==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
 bool                 x    x *) bool(istr(' 0 ')) ==> False | istr('') ==> False
-<=, <, >, >=         x         istr('100') > istr('2') ==> True
+@                         x    istr(20) @ 3 ==> istr('202020')
+|                         x    istr(20) | '5' ==> istr('205')
 slicing                   x    istr(12345)[1:3] ==> istr('23')
-iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
+iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')]
 len                       x    len(istr(' 20 ')) ==> 4
-count                     x    istr(100),count('0') ==> 2
+count                     x    istr(100).count('0') ==> 2
 index                     x    istr(' 100 ').index('0') ==> 2
 split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
-string format             x    f"|{istr((1234):6}|" ==> '|1234  |'
+string format             x    f"|{istr(1234):6}|" ==> '|1234  |'
 other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
                                istr('aAbBcC').islower() ==> False
                                istr('  abc   ').strip() ==> istr('abc')
+                               ...
 -----------------------------------------------------------------------------------------
 *) str is applied if is_int() is False
 
 ```
 ### Test script
 There's an extensive pytest script in the `\tests` directory.
```

### Comparing `istr_python-1.0.5/pyproject.toml` & `istr_python-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "1.0.5"
+version = "1.0.6"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

### Comparing `istr_python-1.0.5/tests/test_istr.py` & `istr_python-1.0.6/tests/test_istr.py`

 * *Files 10% similar despite different names*

```diff
@@ -584,14 +584,37 @@
 
     with istr.base(16):
         d = istr.digits()
         assert id(d) == id(istr.digits())
     assert int(d) == 4886718345
 
 
+def test_itertools():
+    def list100(it):
+        # just iterates over the first 100 elements in the iterable
+        return [next(it) for _ in range(100)]
+
+    assert list(istr.accumulate((1, 3, 4))) == [istr("1"), istr("4"), istr("8")]
+    assert list(istr.chain(range(2), range(2, 5))) == [istr("0"), istr("1"), istr("2"), istr("3"), istr("4")]
+    assert list(istr.combinations(range(5), r=3)) == list(istr(itertools.combinations(range(5), r=3)))
+    assert list(istr.combinations_with_replacement(range(5), r=3)) == list(istr(itertools.combinations_with_replacement(range(5), r=3)))
+    assert list(istr.compress("123456", [1, 0, 1, 0, 1, 1])) == [istr("1"), istr("3"), istr("5"), istr("6")]
+    assert list100(istr.count()) == list100(istr(itertools.count()))
+    assert list100(istr.cycle(range(10))) == list100(istr(itertools.cycle(range(10))))
+    assert list(istr.dropwhile(lambda x: x < 5, [1, 4, 6, 4, 1])) == [istr("6"), istr("4"), istr("1")]
+    assert list(istr.filterfalse(lambda x: x % 2, range(10))) == [istr("0"), istr("2"), istr("4"), istr("6"), istr("8")]
+    assert list(istr.islice("123456", 2)) == [istr("1"), istr("2")]
+    assert list(istr.pairwise("1234")) == [(istr("1"), istr("2")), (istr("2"), istr("3")), (istr("3"), istr("4"))]
+    assert list(istr.permutations(range(5), 3)) == list(istr(itertools.permutations(range(5), 3)))
+    assert list(istr.product(range(5), range(4))) == list(istr(itertools.product(range(5), range(4))))
+    assert list100(istr.repeat(10)) == list100(istr(itertools.repeat(10)))
+    assert list(istr.starmap(pow, [(2, 5), (3, 2), (10, 3)])) == [istr("32"), istr("9"), istr("1000")]
+    assert list(istr.takewhile(lambda x: x < 5, [1, 4, 6, 3, 8])) == [istr("1"), istr("4")]
+    assert list(istr.zip_longest("123", "56", fillvalue="0")) == [(istr("1"), istr("5")), (istr("2"), istr("6")), (istr("3"), istr("0"))]
+
 
 def test_all_distinct():
     assert istr("abcdef").all_distinct()
     assert not istr("aabcdef").all_distinct()
     assert istr("").all_distinct()
```

