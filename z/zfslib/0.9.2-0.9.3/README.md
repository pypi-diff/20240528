# Comparing `tmp/zfslib-0.9.2.tar.gz` & `tmp/zfslib-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfslib-0.9.2.tar", max compression
+gzip compressed data, was "zfslib-0.9.3.tar", max compression
```

## Comparing `zfslib-0.9.2.tar` & `zfslib-0.9.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2022-04-13 20:51:01.734575 zfslib-0.9.2/LICENSE
--rw-r--r--   0        0        0     5232 2022-05-04 23:21:34.934128 zfslib-0.9.2/README.md
--rw-r--r--   0        0        0     1036 2022-06-01 01:27:08.263359 zfslib-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       21 2021-09-18 19:32:38.934906 zfslib-0.9.2/src/zfslib/__init__.py
--rw-r--r--   0        0        0    36274 2022-06-01 00:54:57.152138 zfslib-0.9.2/src/zfslib/zfslib.py
--rw-r--r--   0        0        0     5982 2022-06-01 01:30:32.848662 zfslib-0.9.2/setup.py
--rw-r--r--   0        0        0     6348 2022-06-01 01:30:32.849669 zfslib-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1109 2022-04-13 20:51:01.734575 zfslib-0.9.3/LICENSE
+-rw-r--r--   0        0        0     5232 2022-05-04 23:21:34.934128 zfslib-0.9.3/README.md
+-rw-r--r--   0        0        0     1036 2022-10-05 23:57:04.679671 zfslib-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2021-09-18 19:32:38.934906 zfslib-0.9.3/src/zfslib/__init__.py
+-rw-r--r--   0        0        0    36396 2022-10-06 00:07:40.065184 zfslib-0.9.3/src/zfslib/zfslib.py
+-rw-r--r--   0        0        0     5982 2022-10-06 00:08:57.490319 zfslib-0.9.3/setup.py
+-rw-r--r--   0        0        0     6348 2022-10-06 00:08:57.491245 zfslib-0.9.3/PKG-INFO
```

### Comparing `zfslib-0.9.2/LICENSE` & `zfslib-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zfslib-0.9.2/README.md` & `zfslib-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `zfslib-0.9.2/pyproject.toml` & `zfslib-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zfslib"
-version = "0.9.2"
+version = "0.9.3"
 description = "ZFS Utilities For Python3"
 license = "MIT"
 authors = ["Timothy C. Quinn"]
 readme = "README.md"
 homepage = "https://pypi.org/project/zfslib"
 repository = "https://github.com/JavaScriptDude/zfslib"
 classifiers = [
```

### Comparing `zfslib-0.9.2/src/zfslib/zfslib.py` & `zfslib-0.9.3/src/zfslib/zfslib.py`

 * *Files 3% similar despite different names*

```diff
@@ -357,17 +357,17 @@
     # For name, use full dataset path
     def get_dataset(self, name):
         assert not(isinstance(self, Snapshot)), "get_dataset(name) cannot be used on Snapshot Objects. Use Snapshot.dataset instead."
         ds = self.lookup(name)
         if isinstance(ds, Dataset): return ds
 
         if isinstance(self, Pool):
-            raise KeyError("Dataset '{}' not found in Pool '{}'.".format(name, self.name))
+            raise KeyError(f"Dataset '{name}' not found in Pool '{self.name}'.")
         else:
-            raise KeyError("Dataset '{}' not found in Dataset '{}'.".format(name, self.path))
+            raise KeyError(f"Dataset '{name}' not found in Dataset '{self.path}'.")
         
 
     # returns list(of str) or if with_depth == True then list(of tuple(of depth, Dataset))
     def get_all_datasets(self, with_depth=False, depth=0):
         a = []
         for c in self.children:
             if isinstance(c, Dataset):
@@ -376,16 +376,16 @@
         return a
 
 
     # if index is True return list(of tuple(int, Snapshot))
     # WARNING - Using this function to filter if snapshot contains a folder
     def get_snapshots(self, flt=True, index=False):
         if flt is True: flt = lambda _:True
-        assert inspect.isfunction(flt), "flt must either be True or a Function. Got: {}".format(type(flt))
-        assert isinstance(index, bool), "index must be a boolean. Got: {}".format(type(index))
+        assert inspect.isfunction(flt), f"flt must either be True or a Function. Got: {type(flt)}"
+        assert isinstance(index, bool), f"index must be a boolean. Got: {type(index)}"
         _ds_path = self.path
         res = []
         for idx, c in enumerate(self.children):
             if isinstance(c, Snapshot) and flt(c):
                 res.append( (idx, c) if index else c )
 
         return res
@@ -419,15 +419,15 @@
 
         def __assert(k, types, default=None, to_datetime=False):
             if k == 'find_opts':
                 v=find_opts
             else:
                 if not k in find_opts: return default
                 v = find_opts[k]
-            assert isinstance(v, types), 'Invalid type for param {}. Expecting {} but got: {}'.format(k, types, type(v))
+            assert isinstance(v, types), f'Invalid type for param {k}. Expecting {types} but got: {type(v)}'
 
             if to_datetime and not isinstance(v, datetime):
                 return datetime(v.year, v.month, v.day)
             return v
 
         find_opts = {} if find_opts is None else __assert('find_opts', (dict))
         name = __assert('name', (str))
@@ -472,15 +472,15 @@
             (dt_f, dt_t) = (datetime.now() - tdelta, datetime.now())
             f=__fil_dt
 
         elif not dt_from is None and not dt_to is None:
             if not tdelta is None:
                 raise AssertionError("tdelta cannot be specified when both dt_from and dt_to are specified")
             if dt_from >= dt_to:
-                raise AssertionError("dt_from ({}) must be < dt_to ({})".format(dt_from, dt_to))
+                raise AssertionError(f"dt_from ({dt_from}) must be < dt_to ({dt_to})")
             (dt_f, dt_t) = (dt_from, dt_to)
             f=__fil_dt
 
         else:
             f=__fil_dt
             if dt_from and dt_to and not tdelta:
                 dt_f = dt_from
@@ -554,15 +554,15 @@
         if not exclude is None and not isinstance(exclude, list):
             raise AssertionError("exclude must be a list")
 
         def __tv(k, v):
             if v is None: return None
             if isinstance(v, str): return [v]
             if isinstance(v, list): return v
-            raise AssertionError("{} can only be a str or list. Got: {}".format(k, type(v)))
+            raise AssertionError(f"{k} can only be a str or list. Got: {type(v)}")
 
 
         file_type = __tv('file_type', file_type)
         chg_type = __tv('chg_type', chg_type)
 
         cmd = self.pool.connection.command + ["zfs", "diff", "-FHt", snap_from.path]
         if snap_to:
@@ -587,16 +587,22 @@
 
         def __row(s):
             if not is_py2 and isinstance(s, bytes): s = s.decode('utf-8')
             return s.strip().split( '\t' )
 
         rows = list(map(lambda s: __row(s), stdout.splitlines()))
         diffs = []
-        for row in rows:
+        for i, row in enumerate(rows):
+            # if i == 429:
+            #     print("HERE")
             d = Diff(row, snap_left, snap_right)
+            if d.path_full.find('(on_delete_queue)') > 0:
+                # It looks to be an artefact of ZFS that does not actually exist in FS
+                # https://github.com/openzfs/zfs/blob/master/lib/libzfs/libzfs_diff.c
+                continue
             if not file_type is None and not d.file_type in file_type: continue
             if not chg_type is None and not d.chg_type in chg_type: continue
 
             if not include is None:
                 bOk=False
                 for incl in include:
                     if fnmatch.fnmatch(d.path_full, incl) \
@@ -610,14 +616,15 @@
                 bIgn = False
                 for excl in exclude:
                     if fnmatch.fnmatch(d.path_full, excl) \
                         or (not d.path_new is None and fnmatch.fnmatch(d.path_full_new, excl)):
                         bIgn = True
                         break
                 if bIgn: continue
+
             diffs.append(d)
 
         return diffs
 
 
     def _get_mountpoint(self):
         if self._mountpoint is None:
@@ -637,20 +644,20 @@
     has_mount = property(lambda self: False if self.mountpoint == 'none' else True)
 
 
     # Return relative path to resource within a dataset
     # path must be an actual path on the system being analyzed
     def get_rel_path(self, path):
         self.assertHaveMounts()
-        assert isinstance(path, str), "argument passed is not a string. Got: {}".format(type(path))
+        assert isinstance(path, str), f"argument passed is not a string. Got: {type(path)}"
         p_real = os.path.abspath( expand_user(path) )
         p_real = os.path.realpath(p_real)
         mp = self.mountpoint
         if not p_real.find(mp) == 0:
-            raise KeyError('path given is not in current dataset mountpoint {}. Path: {}'.format(mp, path))
+            raise KeyError(f'path given is not in current dataset mountpoint {mp}. Path: {path}')
         return p_real.replace(mp, '')
 
 
     def assertHaveMounts(self):
         assert self.pool.have_mounts, "Mount information not loaded. Please use Connection.load_poolset(get_mounts=True)."
 
 
@@ -686,15 +693,15 @@
 
 
     # Resolves the path to .zfs/snapshot directory
     def _get_snap_path(self):
         assert isinstance(self.parent, Dataset), \
             "This function is only available for Snapshots of Datasets not Pools"
         self.parent.assertHaveMounts()
-        return "{}/.zfs/snapshot/{}".format(self.parent.mountpoint, self.name)
+        return f"{self.parent.mountpoint}/.zfs/snapshot/{self.name}"
     snap_path = property(_get_snap_path)
 
     
 
 
     # Resolves the path to file within the .zfs/snapshot directory
     # Returns: tuple(of bool, str) where:
@@ -702,24 +709,24 @@
     # - str = Path to item if found else path to .zfs/snapshot directory
     # eg: (found, rel_path) = snap.resolve_snap_path('<some_path_on_system>')
     def resolve_snap_path(self, path):
         assert isinstance(self.parent, Dataset), \
             "This function is only available for Snapshots of Datasets not Pools"
         self.parent.assertHaveMounts()
         assert self.parent.mounted, \
-            "Parent Dataset {} is not mounted. Please verify datsset.mounted before calling this function".format(self.parent)
+            f"Parent Dataset {self.parent} is not mounted. Please verify datsset.mounted before calling this function"
 
         if path is None or not isinstance(path, str) or path.strip() == '':
             assert 0, "path must be a non-blank string"
         path = os.path.abspath( expand_user(path) )
         path_neweal = os.path.realpath(path)
         snap_path_base = self.snap_path
         ds_mp = self.dataset.mountpoint
         if path_neweal.find(ds_mp) == -1:
-            raise KeyError("Path given is not within the dataset's mountpoint of {}. Path passed: {}".format(ds_mp, path))
+            raise KeyError(f"Path given is not within the dataset's mountpoint of {ds_mp}. Path passed: {path}")
         snap_path = "{}{}".format(snap_path_base, path_neweal.replace(ds_mp, ''))
         if os.path.exists(snap_path):
             return (True, snap_path)
         else:
             return (False, snap_path_base)
 
 
@@ -758,36 +765,36 @@
     def __init__(self, row, snap_left, snap_right):
         self.no_from_snap=False
         self.to_present=False
         if isinstance(snap_left, str) and snap_left == '(na-first)':
             self.no_from_snap=True
             snap_left = None
         elif not isinstance(snap_left, Snapshot):
-            raise AssertionError("snap_left must be either a Snapshot or str('na-first'). Got: {}".format(type(snap_left)))
+            raise AssertionError(f"snap_left must be either a Snapshot or str('na-first'). Got: {type(snap_left)}")
 
         if isinstance(snap_right, str) and snap_right == '(present)':
             self.to_present=True
             snap_right = None
 
         elif not isinstance(snap_right, Snapshot):
-            raise AssertionError("snap_left must be either a Snapshot. Got: {}".format(type(snap_right)))
+            raise AssertionError(f"snap_left must be either a Snapshot. Got: {type(snap_right)}")
 
-        if not self.no_from_snap and not self.to_present and snap_left.creation >= snap_right.creation:
-            raise AssertionError("diff from creation ({}) is > or = to diff_to creation ({})".format(snap_left.creation, snap_right.creation))
+        if not self.no_from_snap and not self.to_present and snap_left.creation > snap_right.creation:
+            raise AssertionError(f"diff from creation ({snap_left.creation}) is > to diff_to creation ({snap_right.creation})")
 
         self.snap_left = snap_left
         self.snap_right = snap_right
 
         if len(row) == 4:
             (inode_ts, chg_type, file_type, path) = row
             path_new = None
         elif len(row) == 5:
             (inode_ts, chg_type, file_type, path, path_new) = row
         else:
-            raise Exception("Unexpected len: {}. Row = {}".format(len(row), row))
+            raise Exception(f"Unexpected len: {len(row)}. Row = {row}")
 
         chg_time = datetime.fromtimestamp(int(inode_ts[:inode_ts.find('.')]))
         self.chg_ts = inode_ts
         self.chg_time = chg_time
         self.chg_type = chg_type
         self.file_type = file_type
         if file_type == '/':
@@ -830,21 +837,21 @@
         path_full = self.path_full_new if self.chg_type == 'R' else self.path_full
         return "{}{}".format(snap_path, path_full.replace(self.snap_left.dataset.mountpoint, ''))
     snap_path_right = property(_get_snap_path_right)
     
     @staticmethod
     def get_file_type(s):
         assert (isinstance(s, str) and not s == ''), "argument must be a non-empty string"
-        assert s in Diff.FILE_TYPES, "ZFS Diff File type is invalid: '{}'".format(s)
+        assert s in Diff.FILE_TYPES, f"ZFS Diff File type is invalid: '{s}'"
         return Diff.FILE_TYPES[s]
 
     @staticmethod
     def get_change_type(s):
         assert (isinstance(s, str) and not s == ''), "argument must be a non-empty string"
-        assert s in Diff.CHANGE_TYPES, "ZFS Diff Change type is invalid: '{}'".format(s)
+        assert s in Diff.CHANGE_TYPES, f"ZFS Diff Change type is invalid: '{s}'"
         return Diff.CHANGE_TYPES[s]
 
     def __str__(self):
         return "<Diff> {0} [{1}][{2}] {3}{4}".format(
             self.chg_time.strftime("%Y-%m-%d %H:%M:%S")
             ,self.chg_type, self.file_type
             ,self.path_full, ('' if not self.path_full_new else ' --> '+self.path_new))
@@ -855,76 +862,76 @@
 
 
 ''' General Utilities '''
 
 # buildTimedelta()
 # Builds timedelta from string:
 # . tdelta is a timedelta -or- str(nC) where: n is an integer > 0 and C is one of:
-#   . y=year, m=month, w=week, d=day, H=hour, M=minute, s=second
+#   . Y=year, M=month, W=week, D=day, h=hour, m=minute, s=second
 # Note: month and year are imprecise and assume 30.4 and 365 days
-def buildTimedelta(tdelta):
+def buildTimedelta(tdelta) -> timedelta:
     if isinstance(tdelta, timedelta): return tdelta
     
     if not isinstance(tdelta, str):
-        raise AssertionError('tdelta must be a string')
+        raise KeyError('tdelta must be a string')
     elif len(tdelta) < 2:
-        raise AssertionError('len(tdelta) must be >= 2')
+        raise KeyError('len(tdelta) must be >= 2')
     n = tdelta[:-1]
     try:
         n = int(n)
-        if n < 1: raise AssertionError('tdelta must be > 0')
+        if n < 1: raise KeyError('tdelta must be > 0')
     except ValueError as ex:
-        raise AssertionError('Value passed for tdelta does not contain a number: {}'.format(tdelta))
+        raise KeyError(f'Value passed for tdelta does not contain a number: {tdelta}')
     
     c = tdelta[-1:]
-    if c == 'H':
+    if c == 'h':
         return timedelta(hours=n)
-    elif c == 'M':
+    elif c == 'm':
         return timedelta(minutes=n)
-    elif c == 'S':
+    elif c == 's':
         return timedelta(seconds=n)
-    elif c == 'd':
+    elif c == 'D':
         return timedelta(days=n)
-    elif c == 'm':
-        return timedelta(days=n*(365/12))
-    elif c == 'w':
+    elif c == 'W':
         return timedelta(weeks=n)
-    elif c == 'y':
+    elif c == 'M':
+        return timedelta(days=n*(365/12))
+    elif c == 'Y':
         return timedelta(days=n*365)
     else:
-        raise AssertionError('Unexpected datetime identifier, expecting one of y,m,w,d,H,M,S.')
+        raise KeyError('Unexpected datetime identifier, expecting one of Y,M,W,D,h,m,s')
 
 
 # calcDateRange()
 # Calculates a date range based on tdelta string passed
 # tdelta is a timedelta -or- str(nC) where: n is an integer > 0 and C is one of:
-# . y=year, m=month, w=week, d=day, H=hour, M=minute, s=second
+#  . Y=year, M=month, W=week, D=day, h=hour, m=minute, s=second
 # If dt_from is defined, return tuple: (dt_from, dt_from+tdelta)
 # If dt_to is defined, return tuple: (dt_from-tdelta, dt_to)
-def calcDateRange(tdelta, dt_from=None, dt_to=None):
-    if tdelta is None: raise AssertionError('tdelta is required')
+def calcDateRange(tdelta, dt_from:datetime=None, dt_to:datetime=None) -> tuple:
+    if tdelta is None: raise KeyError('tdelta is required')
     if dt_from and dt_to:
-        raise AssertionError('Only one of dt_from or dt_to must be defined')
+        raise KeyError('Only one of dt_from or dt_to must be defined')
     elif (not dt_from and not dt_to):
-        raise AssertionError('Please specify one of dt_from or dt_to')
+        raise KeyError('Please specify one of dt_from or dt_to')
     elif dt_from and not isinstance(dt_from, datetime):
-        raise AssertionError('dt_from must be  a datetime')
+        raise KeyError('dt_from must be  a datetime')
     elif dt_to and not isinstance(dt_to, datetime):
-        raise AssertionError('dt_to must be  a datetime')
+        raise KeyError('dt_to must be  a datetime')
 
     td = buildTimedelta(tdelta)
     
     if dt_from:
         return (dt_from, (dt_from + td))
     else:
         return ((dt_to - td), dt_to)
 
 
 def splitPath(s):
-    assert isinstance(s, str), "String not passed. Got: {}".format(type(s))
+    assert isinstance(s, str), f"String not passed. Got: {type(s)}"
     s = s.strip()
     assert not s == '', "Empty string passed"
     f = os.path.basename(s)
     if len(f) == 0: return ('', s[:-1] if s[-1:] == '/' else s)
     p = s[:-(len(f))-1]
     return f, p
```

### Comparing `zfslib-0.9.2/setup.py` & `zfslib-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['zfslib']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'zfslib',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'ZFS Utilities For Python3',
     'long_description': "# zfslib\n\nZFS Libraries for Python\n\nPython library for reading from ZFS Pools. Capable of reading, Pools, Datasets, Snapshots and Diffs for use by other Python Tools.\n\nThis tool presently targets Python v3.7+\n\n## Installation\n\nInstall this plugin using `pip`:\n\n    $ python3 -m pip install zfslib\n\n## Usage\n\nSee examples folder\n\n## Sample code\n\n```\n    import zfslib as zfs\n\n    # Read ZFS information from local computer\n    # For remote computer access, use certificate based ssh authentication \n    # see `examples/ex_remote.py`\n    conn = zfs.Connection(host='localhost')\n\n\n    # Load poolset. \n    # Properties can be queried here with: properties=['prop1','prop2',...]\n    # Default properties: name, creation\n    # If get_mounts=True, mountpoint and mounted are also retrieved automatically\n    # unlocking some functionality\n    # To see all available properties use: % zfs list -o foo\n    poolset = conn.load_poolset()\n\n    # Load a pool by name\n    pool = poolset.get_pool('dpool')\n    \n    # Get properties from ZFSItem's (Pool|DataSet|Snapshot)\n    # <ZFSItem>.get_property('<property>')\n    # -also-\n    # <ZFSItem>.path -> str: Full path for item\n    # <ZFSItem>.name -> str: Name of item\n    # <ZFSItem>.creation -> datetime\n    # <dataset>.mountpoint -> str\n    # <dataset|snapshot>.pool -> Pool\n    # <snapshot>.dataset -> DataSet\n    # <dataset>.dspath -> str: Dataset path excluding pool name\n    # <ZFSItem>.parent -> ZfsItem\n    # <pool|dataset>.children -> list(of ZfsItem)\n    # . Pools only contain DataSets\n    # . Datasets can contain DataSets and/or Snapshots\n\n\n    # Load dataset\n    ds = pool.get_dataset('vcmain')\n\n    # Load snapshots by with name of autosnap* that fall between \n    # the dates of 2020-12-20 and 2020-12-24\n    snapshots = ds.find_snapshots({\n        'name': 'autosnap*', 'date_from': '2020-12-20', 'date_to': '2020-12-24'\n    })\n\n    # Get all the changes file modification diffs for files that end with .py and .js \n    # excluding those in __pycache__ between the first and second snapshots\n    diffs = ds.get_diffs(\n         snapshots[0], snapshots[1]\n        ,file_type='F', chg_type='M'\n        ,include=['*.py', '*.js']\n        ,ignore=['*_pycache_*']\n    )\n\n    # Load snapshots by with name of autosnap* in the last 12 hours \n    snapshots = ds.find_snapshots({'name': 'autosnap*', 'tdelta': '12H'})\n\n    # Get Path to a file in the Snapshot folder (under mountpoint/.zfs/snapshots):\n    find_path = '<path_to_some_local_file_in_ZFS>'\n    (exists, snap_path) = snapshots[0].resolve_snap_path(find_path)\n    if exists:\n        print('snap_path: {}'.format(snap_path))\n    else: # file did not exist at time of snapshot creation\n        print('File not found in snapshot: {}'.format(find_path))\n\n```\n\n## Some Key Features\n### `<Dataset>.find_snapshots(dict)`\n```\n    # find_snapshots(dict) - Query all snapshots in Dataset\n    #  Options:\n    #  - name: Snapshot name (wildcard supported)\n    #  - contains: Path to resource (wildcard supported)\n    #  - dt_from: datetime to start\n    #  - tdelta: timedelta -or- string of nC where: n is an integer > 0 and C is one of y,m,d,H,M,S. Eg 5H = 5 Hours\n    #  - dt_to: datetime to stop \n    #  - index: (bool) - Return list(tuple(of int, snapshot, dataset)) where int is the index in current snaphot listing for dataset\n    #  Notes:\n    #  - Date searching is any combination of:\n    #      (dt_from --> dt_to) | (dt_from --> dt_from + tdelta) | (dt_to - tdelta --> dt_to) | (dt_from --> now)\n```\n\n### `<Dataset>.get_diffs()`\n```\n    # get_diffs() - Gets Diffs in snapshot or between snapshots (if snap_to is specified)\n    #               If snap_to is not specified, diff is to working copy\n    # snap_from - Left side of diff\n    # snap_to - Right side of diff. If not specified, diff is to current working version\n    # include - list of glob expressions to include (eg ['*_pycache_*'])\n    # exclude - list of glob expressions to exclude (eg ['*_pycache_*'])\n    # file_type - Filter on the following\n    #  - B       Block device\n    #  - C       Character device\n    #  - /       Directory\n    #  - >       Door\n    #  - |       Named pipe\n    #  - @       Symbolic link\n    #  - P       Event port\n    #  - =       Socket\n    #  - F       Regular file\n    # chg_type - Filter on the following:\n    #  - -       The path has been removed\n    #  - +       The path has been created\n    #  - M       The path has been modified\n    #  - R       The path has been renamed\n```\n\n### `<Snapshot>.snap_path`\n```\n    # Returns the path to read only zfs_snapshot directory (<ds_mount>/.zfs/snapshots/<snapshot>)\n```\n\n### `<Snapshot>.resolve_snap_path(path)`\n```\n    # Resolves the path to file/dir within the zfs_snapshot dir\n    # Returns: tuple(of bool, str) where:\n    # - bool = True if item is found\n    # - str = Path to item if found else path to zfs_snapshot dir\n```\n\n### `<Diff>.snap_path_left`\n```\n    # Path to resource on left side of diff in zfs_snapshot dir\n```\n\n### `<Diff>.snap_path_right`\n```\n    # Path to resource on right side of diff in .zfs_snapshot dir or working copy\n```\n\nSee `test.py` for more sample code\n\n\nCredits: This code is based heavily on [zfs-tools by Rudd-O](https://github.com/Rudd-O/zfs-tools).",
     'author': 'Timothy C. Quinn',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://pypi.org/project/zfslib',
```

### Comparing `zfslib-0.9.2/PKG-INFO` & `zfslib-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfslib
-Version: 0.9.2
+Version: 0.9.3
 Summary: ZFS Utilities For Python3
 Home-page: https://pypi.org/project/zfslib
 License: MIT
 Author: Timothy C. Quinn
 Requires-Python: >=3.7.9,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

