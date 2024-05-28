# Comparing `tmp/ptwebdiscover-1.0.6.tar.gz` & `tmp/ptwebdiscover-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptwebdiscover-1.0.6.tar", last modified: Thu May  9 13:23:30 2024, max compression
+gzip compressed data, was "ptwebdiscover-1.0.7.tar", last modified: Tue May 28 11:18:50 2024, max compression
```

## Comparing `ptwebdiscover-1.0.6.tar` & `ptwebdiscover-1.0.7.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/LICENSE
--rwxr-xr-x   0 kali      (1000) kali      (1000)       40 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)     7626 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     7105 2024-05-09 13:20:59.000000 ptwebdiscover-1.0.6/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       22 2024-05-09 13:20:56.000000 ptwebdiscover-1.0.6/ptwebdiscover/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)      369 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/findings.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)      519 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/keyspace.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/__init__.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1068 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/argumentoptions.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)      192 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/findingdetail.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)      343 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/processedargumentoptions.py
--rw-r--r--   0 kali      (1000) kali      (1000)    48565 2024-04-30 07:58:41.000000 ptwebdiscover-1.0.6/ptwebdiscover/ptwebdiscover.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    11506 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/responseprocessing.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/utils/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/
--rw-r--r--   0 kali      (1000) kali      (1000)      182 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 kali      (1000) kali      (1000)     4314 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/treeshow.cpython-311.pyc
--rw-r--r--   0 kali      (1000) kali      (1000)     3949 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/url.cpython-311.pyc
--rwxr-xr-x   0 kali      (1000) kali      (1000)     9605 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/cachefile.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2069 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/treeshow.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1935 2024-05-09 13:16:29.000000 ptwebdiscover-1.0.6/ptwebdiscover/utils/url.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     7626 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      911 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       67 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       42 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2024-05-09 13:23:30.000000 ptwebdiscover-1.0.6/ptwebdiscover.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 13:23:30.635751 ptwebdiscover-1.0.6/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1043 2024-05-09 13:21:00.000000 ptwebdiscover-1.0.6/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/LICENSE
+-rwxr-xr-x   0 kali      (1000) kali      (1000)       40 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     7626 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     7105 2024-05-19 17:10:26.000000 ptwebdiscover-1.0.7/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/ptwebdiscover/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       22 2024-05-28 11:15:38.000000 ptwebdiscover-1.0.7/ptwebdiscover/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      369 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/findings.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      519 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/keyspace.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/ptwebdiscover/ptdataclasses/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/ptdataclasses/__init__.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1177 2024-05-28 11:15:51.000000 ptwebdiscover-1.0.7/ptwebdiscover/ptdataclasses/argumentoptions.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      192 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/ptdataclasses/findingdetail.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)      343 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/ptdataclasses/processedargumentoptions.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    48629 2024-05-28 11:15:51.000000 ptwebdiscover-1.0.7/ptwebdiscover/ptwebdiscover.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    11506 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/responseprocessing.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/ptwebdiscover/utils/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/ptwebdiscover/utils/__pycache__/
+-rw-r--r--   0 kali      (1000) kali      (1000)      182 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)    13651 2024-05-28 11:17:40.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/__pycache__/cachefile.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     4314 2024-05-09 13:18:18.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/__pycache__/treeshow.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     4020 2024-05-28 11:17:05.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/__pycache__/url.cpython-311.pyc
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     9605 2024-05-28 11:15:05.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/cachefile.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2069 2024-04-29 08:25:06.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/treeshow.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1981 2024-05-28 11:15:51.000000 ptwebdiscover-1.0.7/ptwebdiscover/utils/url.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/ptwebdiscover.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     7626 2024-05-28 11:18:50.000000 ptwebdiscover-1.0.7/ptwebdiscover.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      969 2024-05-28 11:18:50.000000 ptwebdiscover-1.0.7/ptwebdiscover.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-28 11:18:50.000000 ptwebdiscover-1.0.7/ptwebdiscover.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       67 2024-05-28 11:18:50.000000 ptwebdiscover-1.0.7/ptwebdiscover.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       42 2024-05-28 11:18:50.000000 ptwebdiscover-1.0.7/ptwebdiscover.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       14 2024-05-28 11:18:50.000000 ptwebdiscover-1.0.7/ptwebdiscover.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-28 11:18:50.484551 ptwebdiscover-1.0.7/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1043 2024-05-19 17:10:26.000000 ptwebdiscover-1.0.7/setup.py
```

### Comparing `ptwebdiscover-1.0.6/LICENSE` & `ptwebdiscover-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.6/PKG-INFO` & `ptwebdiscover-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptwebdiscover
-Version: 1.0.6
+Version: 1.0.7
 Summary: Web Source Discovery Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `ptwebdiscover-1.0.6/README.md` & `ptwebdiscover-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/keyspace.py` & `ptwebdiscover-1.0.7/ptwebdiscover/keyspace.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/ptdataclasses/argumentoptions.py` & `ptwebdiscover-1.0.7/ptwebdiscover/ptdataclasses/argumentoptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import dataclass
 
 
 @dataclass
 class ArgumentOptions:
     url: str
+    source: str
+    non_exist: list[str]
     charsets: list[str]
     length_min: int
     length_max: int
     wordlist: list[str]
     prefix: str
     suffix: str
     begin_with: str
@@ -46,8 +48,11 @@
     tree: bool
     output: str
     save: str
     auth: str
     json: bool
     errors: bool
     silent: bool
-    cache: bool
+    cache: bool
+    socket_address: str
+    socket_port: str
+    process_ident: str
```

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/ptwebdiscover.py` & `ptwebdiscover-1.0.7/ptwebdiscover/ptwebdiscover.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,56 +44,56 @@
 from keyspace import Keyspace
 
 from _version import __version__
 
 
 class PtWebDiscover():
     def __init__(self, args: ArgumentOptions) -> None:
-        self.args: ProcessedArgumentOptions                         = args
-        self.args.timeout                                           = args.timeout / 1000
-        self.args.content_length                                    = args.content_length * 1000
-        self.args.delay                                             = args.delay / 1000
-        self.args.is_star                                           = True if "*" in args.url else False
-        self.args.nochanged_url                                     = self.args.url
-        self.args.url                                               = ptnethelper.remove_slash_from_end_url(args.url) if not self.args.is_star else args.url
-        self.args.url                                               = Url(args.url).add_missing_scheme(self.args.scheme)
-        self.args.target                                            = Url(args.target).add_missing_scheme(self.args.scheme)
-        self.args.position, self.args.url                           = self.get_star_position(self.args.url)
-        self.args.headers                                           = ptnethelper.get_request_headers(args)
-        self.args.proxies                                           = {"http": args.proxy, "https": args.proxy}
-        self.args.charset                                           = ptcharsethelper.get_charset(["lowercase"]) if not args.charsets and not args.wordlist else ptcharsethelper.get_charset(args.charsets)
-        self.args.parse                                             = args.parse or args.parse_only
-        self.args.length_max                                        = args.length_max if args.length_max else 99 if args.wordlist else 6
-        self.args.begin_with                                        = args.begin_with if args.begin_with else ""
-        self.args.threads                                           = args.threads    if not args.delay  else 1
-        self.args.method                                            = args.method     if not (args.string_in_response or args.string_not_in_response or args.parse or args.save) else "GET"
-        self.domain                                                 = Url(self.args.url).get_domain_from_url(level=True, with_protocol=False)
-        self.domain_with_protocol                                   = Url(self.args.url).get_domain_from_url(level=True, with_protocol=True)
-        self.domain_protocol                                        = urllib.parse.urlparse(args.url).scheme
-        self.args.is_star_in_domain                                 = True if self.args.is_star and self.args.position < len(self.domain_with_protocol)+1 else False
-        self.urlpath                                                = Url(self.args.url).get_path_from_url(with_l_slash=True, without_r_slash=True)
-        self.args.auth                                              = tuple(args.auth.split(":")) if args.auth else None
-        self.ptjsonlib                                              = ptjsonlib.PtJsonLib()
-        self.use_json                                               = args.json
-        #self.ptthreads                                             = ptthreads.PtThreads(args.errors)
-        self.ptthreads                                              = ptthreads.PtThreads()
-        self.printlock                                              = printlock.PrintLock()
-        self.arraylock                                              = arraylock.ArrayLock()
-        #self.json_no                                               = self.ptjsonlib.add_json("ptwebdiscover")
-        Findings.directories                                        = arraylock.ThreadSafeArray([self.urlpath + "/"] if not self.args.is_star else [""])
+        self.args: ProcessedArgumentOptions  = args
+        self.args.timeout: int               = args.timeout / 1000
+        self.args.content_length: int        = args.content_length * 1000
+        self.args.delay: int                 = args.delay / 1000
+        self.args.is_star: bool              = True if "*" in args.url else False
+        self.args.nochanged_url: str         = self.args.url
+        self.args.url                        = ptnethelper.remove_slash_from_end_url(args.url) if not self.args.is_star else args.url
+        self.args.url                        = Url(args.url).add_missing_scheme(self.args.scheme)
+        self.args.target: str                = Url(args.target).add_missing_scheme(self.args.scheme)
+        self.args.position, self.args.url    = self.get_star_position(self.args.url)
+        self.args.headers: dict              = ptnethelper.get_request_headers(args)
+        self.args.proxies: dict              = {"http": args.proxy, "https": args.proxy}
+        self.args.charset: list              = ptcharsethelper.get_charset(["lowercase"]) if not args.charsets and not args.wordlist else ptcharsethelper.get_charset(args.charsets)
+        self.args.parse: bool                = args.parse or args.parse_only
+        self.args.length_max: int            = args.length_max if args.length_max else 99 if args.wordlist else 6
+        self.args.begin_with: str            = args.begin_with if args.begin_with else ""
+        self.args.threads: int               = args.threads if not args.delay  else 1
+        self.args.method: str                = args.method if not (args.string_in_response or args.string_not_in_response or args.parse or args.save) else "GET"
+        self.domain                          = Url(self.args.url).get_domain_from_url(level=True, with_protocol=False)
+        self.domain_with_protocol            = Url(self.args.url).get_domain_from_url(level=True, with_protocol=True)
+        self.domain_protocol                 = urllib.parse.urlparse(args.url).scheme
+        self.args.is_star_in_domain          = True if self.args.is_star and self.args.position < len(self.domain_with_protocol)+1 else False
+        self.urlpath                         = Url(self.args.url).get_path_from_url(with_l_slash=True, without_r_slash=True)
+        self.args.auth                       = tuple(args.auth.split(":")) if args.auth else None
+        self.use_json                        = args.json
+        self.ptjsonlib                       = ptjsonlib.PtJsonLib()
+        self.ptthreads                       = ptthreads.PtThreads()
+        self.printlock                       = printlock.PrintLock()
+        self.arraylock                       = arraylock.ArrayLock()
+        self.args.extensions                 = self.prepare_extensions(args) # must be placed after set of self.directories
+        Findings.directories                 = arraylock.ThreadSafeArray([self.urlpath + "/"] if not self.args.is_star else [""])
+        #self.ptthreads                      = ptthreads.PtThreads(args.errors)
         self.check_args_combinations()
-        self.args.extensions                                        = self.prepare_extensions(args) # must be placed after set of self.directories
         self.prepare_not_directories(self.args.not_directories)
 
 
     def run(self, args: ArgumentOptions) -> None:
         if not args.without_dns_cache:
             self.cache_dns()
 
-        ptnethelper.check_connectivity(self.args.proxies)
+        if not args.without_availability:
+            ptnethelper.check_connectivity(self.args.proxies)
 
         if not self.args.is_star_in_domain:
             # TODO set cookies with star in url too
             self.set_header_cookies()
 
         self.initialize_counters()
 
@@ -175,20 +175,24 @@
         ptprinthelper.clear_line_ifnot(condition = self.args.json)
         ptprinthelper.ptprint( ptprinthelper.out_title_ifnot("Check " + self.domain_with_protocol + self.directory, self.args.json))
 
         if not self.check_posibility_testing():
             self.printlock.lock_print( ptprinthelper.out_ifnot("Not posible to check this directory. Use -sy, -sn or -sc parameter.", "ERROR", self.args.json), end="\n", clear_to_eol=True)
             return
 
-        if args.wordlist or args.parse_only or args.backups_only:
+        if args.wordlist or args.source or args.parse_only or args.backups_only:
             if args.parse_only or args.backups_only:
                 Keyspace.space = 1
                 wordlist = [""]
             else:
-                Keyspace.space, wordlist = self.try_prepare_wordlist(args)
+                if args.wordlist:
+                    Keyspace.space, wordlist = self.try_prepare_wordlist(args)
+                if args.source:
+                    wordlist = [w for w in args.source]
+                    Keyspace.space = len(wordlist) * len(args.extensions)
 
             self.keyspace_for_directory = Keyspace.space
             self.ptthreads.threads(wordlist, self.dictionary_discover, self.args.threads)
         else:
             combinations = ptcharsethelper.get_combinations(self.args.charset, self.args.length_min, self.args.length_max)
             self.ptthreads.threads(combinations, self.bruteforce_discover, self.args.threads)
 
@@ -206,17 +210,15 @@
     def process_all_backups(self):
         self.prepare_backup()
         self.search_for_backup_of_all(self.domain)
 
 
     def print_results(self):
         if self.use_json:
-            nodes = []
-            for url in Findings.findings:
-                self.ptjsonlib.parse_url2nodes(url, nodes)
+            nodes: list = self.ptjsonlib.parse_urls2nodes(Findings.findings)
             self.ptjsonlib.add_nodes(nodes)
             self.ptjsonlib.set_status("finished")
             ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
         else:
             self.output_result(Findings.findings, Findings.details, Findings.technologies)
             ptprinthelper.ptprint( ptprinthelper.out_ifnot(f"Finished in {ptmisclib.time2str(time.time()-self.start_time)} - discovered: {len(Findings.findings)} items", "INFO", self.args.json))
 
@@ -681,14 +683,15 @@
             "ptwebdiscover -u https://www.example.com -e \"\" bak old php~ php.bak",
             "ptwebdiscover -u https://www.example.com -E extensions.txt",
             "ptwebdiscover -u https://www.example.com -w -sn \"Page Not Found\""
         ]},
         {"options": [
             ["-u",  "--url",                    "<url>",            "URL for test (usage of a star character as anchor)"],
             ["-ch", "--charsets",               "<charsets>",       "Specify charset fro brute force (example: lowercase,uppercase,numbers,[custom_chars])"],
+            ["-src", "--source",               "<source>",          "Check for presence of only specified <source> (eg. -src robots.txt)"],
             ["",    "",                         "",                 "Modify wordlist (lowercase,uppercase,capitalize)"],
             ["-lm", "--length-min",             "<length-min>",     "Minimal length of brute-force tested string (default 1)"],
             ["-lx", "--length-max",             "<length-max>",     "Maximal length of brute-force tested string (default 6 bf / 99 wl"],
             ["-w",  "--wordlist",               "<filename>",       "Use specified wordlist(s)"],
             ["-pf", "--prefix",                 "<string>",         "Use prefix before tested string"],
             ["-sf", "--suffix",                 "<string>",         "Use suffix after tested string"],
             ["-bw", "--begin-with",             "<string>",         "Use only words from wordlist that begin with the specified string"],
@@ -701,54 +704,58 @@
             ["-bo", "--backups-only",           "",                 "Find backup of complete website only"],
             ["-P",  "--parse",                  "",                 "Parse HTML response for URLs discovery"],
             ["-Po", "--parse-only",             "",                 "Brute force method is disabled, crawling started on specified url"],
             ["-D",  "--directory",              "",                 "Add a slash at the ends of the strings too"],
             ["-nd", "--not-directories",        "<directories>",    "Not include listed directories when recursive browse run"],
             ["-sy", "--string-in-response",     "<string>",         "Print findings only if string in response (GET method is used)"],
             ["-sn", "--string-not-in-response", "<string>",         "Print findings only if string not in response (GET method is used)"],
-            ["-sc", "--status-codes",           "<status codes>",   "Ignore response with status codes (default 404)"],
-            ["-m",  "--method",                 "<method>",         "Use said HTTP method (default: HEAD)"],
-            ["-se", "--scheme",                 "<scheme>",         "Use scheme when missing (default: http)"],
+            ["-sc", "--status-codes",           "<status-codes>",   "Ignore response with status codes (default 404)"],
             ["-d",  "--delay",                  "<miliseconds>",    "Delay before each request in seconds"],
-            ["-p",  "--proxy",                  "<proxy>",          "Use proxy (e.g. http://127.0.0.1:8080)"],
             ["-T",  "--timeout",                "<miliseconds>",    "Manually set timeout (default 10000)"],
             ["-cl", "--content-length",         "<kilobytes>",      "Max content length to download and parse (default: 1000KB)"],
+            ["-m",  "--method",                 "<method>",         "Use said HTTP method (default: HEAD)"],
+            ["-se", "--scheme",                 "<scheme>",         "Use scheme when missing (default: http)"],
+            ["-p",  "--proxy",                  "<proxy>",          "Use proxy (e.g. http://127.0.0.1:8080)"],
             ["-H",  "--headers",                "<headers>",        "Use custom headers"],
-            ["-ua", "--user-agent",             "<agent>",          "Use custom value of User-Agent header"],
+            ["-a",  "--user-agent",             "<agent>",          "Use custom value of User-Agent header"],
             ["-c",  "--cookie",                 "<cookies>",        "Use cookie (-c \"PHPSESSID=abc; any=123\")"],
-            ["-rc", "--refuse-cookies",         "",                 "Do not use cookies sets by application"],
-            ["-a",  "--auth",                   "<name:pass>",      "Use HTTP authentication"],
+            ["-A",  "--auth",                   "<name:pass>",      "Use HTTP authentication"],
+            ["-rc", "--refuse-cookies",         "",                 "Do not use cookies set by application"],
             ["-t",  "--threads",                "<threads>",        "Number of threads (default 20)"],
             ["-wd", "--without-domain",         "",                 "Output of discovered sources without domain"],
             ["-wh", "--with-headers",           "",                 "Output of discovered sources with headers"],
             ["-ip", "--include-parameters",     "",                 "Include GET parameters and anchors to output"],
             ["-tr", "--tree",                   "",                 "Output as tree"],
             ["-o",  "--output",                 "<filename>",       "Output to file"],
             ["-S",  "--save",                   "<directory>",      "Save content localy"],
             ["-wdc","--without_dns_cache",      "",                 "Do not use DNS cache (example for /etc/hosts records)"],
             ["-wa", "--without_availability",   "",                 "Do not use target availability check"],
             ["-tg", "--target",                 "<ip or host>",     "Use this target when * is in domain"],
             ["-nr", "--not-redirect",           "",                 "Do not follow redirects"],
             ["-s",  "--silent",                 "",                 "Do not show statistics in realtime"],
+            ["-C",  "--cache",                  "",                 "Cache each request response to temp file"],
+            ["-ne", "--non-exist",              "",                 "Check, if non existing pages return status code 200."],
             ["-er", "--errors",                 "",                 "Show all errors"],
-            ["-C",  "--cache",                   "",                "Cache each request response to temp file"],
             ["-v",  "--version",                "",                 "Show script version"],
             ["-h",  "--help",                   "",                 "Show this help message"],
             ["-j",  "--json",                   "",                 "Output in JSON format"],
         ]},
     ]
 
 
 def parse_args() -> ArgumentOptions:
     parser = argparse.ArgumentParser(add_help=False, usage=f"{SCRIPTNAME} <options>")
-    parser.add_argument("-u",  "--url", type=str)
+    exclusive = parser.add_mutually_exclusive_group()
+    exclusive.add_argument("-w",  "--wordlist", type=str, nargs="+")
+    exclusive.add_argument("-src", "--source", type=str, nargs="+")
+
+    parser.add_argument("-u",  "--url", type=str, required=True)
     parser.add_argument("-ch", "--charsets", type=str, nargs="+", default=[])
     parser.add_argument("-lm", "--length-min", type=int, default=1)
     parser.add_argument("-lx", "--length-max", type=int)
-    parser.add_argument("-w",  "--wordlist", type=str, nargs="+")
     parser.add_argument("-pf", "--prefix", type=str, default="")
     parser.add_argument("-sf", "--suffix", type=str, default="")
     parser.add_argument("-bw", "--begin-with", type=str)
     parser.add_argument("-b",  "--backups", action="store_true")
     parser.add_argument("-bo", "--backups-only", action="store_true")
     parser.add_argument("-e",  "--extensions", type=str, nargs="+", default=[])
     parser.add_argument("-E",  "--extensions-file", type=str)
@@ -767,32 +774,38 @@
     parser.add_argument("-d",  "--delay", type=int, default=0)
     parser.add_argument("-p",  "--proxy", type=str)
     parser.add_argument("-T",  "--timeout", type=int, default=10000)
     parser.add_argument("-cl", "--content-length", type=int, default=1000)
     parser.add_argument("-wdc","--without_dns_cache", action="store_true")
     parser.add_argument("-wa", "--without_availability", action="store_true")
     parser.add_argument("-H",  "--headers", type=ptmisclib.pairs, nargs="+")
-    parser.add_argument("-ua", "--user-agent", type=str, default="Penterep Tools")
+    parser.add_argument("-a", "--user-agent", type=str, default="Penterep Tools")
     parser.add_argument("-c",  "--cookie", type=str, default="")
     parser.add_argument("-rc", "--refuse-cookies", action="store_true")
     parser.add_argument("-nr", "--not-redirect", action="store_true", default=False)
     parser.add_argument("-tg", "--target", type=str, default="")
     parser.add_argument("-t",  "--threads", type=int, default=20)
     parser.add_argument("-wd", "--without-domain", action="store_true")
     parser.add_argument("-wh", "--with-headers", action="store_true")
     parser.add_argument("-ip", "--include-parameters", action="store_true")
     parser.add_argument("-tr", "--tree", action="store_true")
     parser.add_argument("-o",  "--output", type=str)
     parser.add_argument("-S",  "--save", type=str)
-    parser.add_argument("-a",  "--auth", type=str)
-    parser.add_argument("-j",  "--json", action="store_true")
+    parser.add_argument("-A",  "--auth", type=str)
+    parser.add_argument("-ne", "--non-exist", action="store_true")
     parser.add_argument("-er", "--errors", action="store_true")
     parser.add_argument("-s",  "--silent", action="store_true")
     parser.add_argument("-v",  "--version", action="version", version=f"{SCRIPTNAME} {__version__}")
     parser.add_argument("-C",  "--cache", action="store_true")
+    parser.add_argument("-j",  "--json", action="store_true")
+
+    parser.add_argument("--socket-address",          type=str, default=None)
+    parser.add_argument("--socket-port",             type=str, default=None)
+    parser.add_argument("--process-ident",           type=str, default=None)
+
 
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
 
     args = parser.parse_args()
     return ArgumentOptions(**vars(args))
```

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/responseprocessing.py` & `ptwebdiscover-1.0.7/ptwebdiscover/responseprocessing.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/treeshow.cpython-311.pyc` & `ptwebdiscover-1.0.7/ptwebdiscover/utils/__pycache__/treeshow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/utils/__pycache__/url.cpython-311.pyc` & `ptwebdiscover-1.0.7/ptwebdiscover/utils/__pycache__/url.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xadcc3c66 (Thu May  9 13:16:29 2024 UTC)
-files sz: 1935
+moddate:  0xe7bc5566 (Tue May 28 11:15:51 2024 UTC)
+files sz: 1981
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -27,15 +27,15 @@
      4          22 LOAD_CONST               0 (0)
                 24 LOAD_CONST               1 (None)
                 26 IMPORT_NAME              3 (urllib.parse)
                 28 STORE_NAME               4 (urllib)
    
      7          30 PUSH_NULL
                 32 LOAD_BUILD_CLASS
-                34 LOAD_CONST               3 (<code object Url, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 7>)
+                34 LOAD_CONST               3 (<code object Url, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 7>)
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('Url')
                 40 PRECALL                  2
                 44 CALL                     2
                 54 STORE_NAME               5 (Url)
                 56 LOAD_CONST               1 (None)
                 58 RETURN_VALUE
@@ -45,81 +45,85 @@
       ('tldparser',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
-            0x970065005a0164005a0264016503640264036604640484045a04640f64
-            0265036602640784055a05640265036602640884045a06640984005a0764
-            0a6503640265036604640b84045a086410640265036602640c84055a0964
-            0d6503640265036604640e84045a0a64035300
+            0x970065005a0164005a0264015a0364026504640364046604640584045a
+            056410640365046602640884055a06640365046602640984045a07640a84
+            005a08640b6504640365046604640c84045a096411640365046602640d84
+            055a0a640e6504640365046604640f84045a0b64045300
            7           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Url')
                        8 STORE_NAME               2 (__qualname__)
          
-           9          10 LOAD_CONST               1 ('url')
-                      12 LOAD_NAME                3 (str)
-                      14 LOAD_CONST               2 ('return')
-                      16 LOAD_CONST               3 (None)
-                      18 BUILD_TUPLE              4
-                      20 LOAD_CONST               4 (<code object __init__, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 9>)
-                      22 MAKE_FUNCTION            4 (annotations)
-                      24 STORE_NAME               4 (__init__)
+           8          10 LOAD_CONST               1 ('A class to represent and manipulate a URL.')
+                      12 STORE_NAME               3 (__doc__)
          
-          13          26 LOAD_CONST              15 ((True, False))
-                      28 LOAD_CONST               2 ('return')
-                      30 LOAD_NAME                3 (str)
-                      32 BUILD_TUPLE              2
-                      34 LOAD_CONST               7 (<code object get_path_from_url, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 13>)
-                      36 MAKE_FUNCTION            5 (defaults, annotations)
-                      38 STORE_NAME               5 (get_path_from_url)
+           9          14 LOAD_CONST               2 ('url')
+                      16 LOAD_NAME                4 (str)
+                      18 LOAD_CONST               3 ('return')
+                      20 LOAD_CONST               4 (None)
+                      22 BUILD_TUPLE              4
+                      24 LOAD_CONST               5 (<code object __init__, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 9>)
+                      26 MAKE_FUNCTION            4 (annotations)
+                      28 STORE_NAME               5 (__init__)
          
-          24          40 LOAD_CONST               2 ('return')
-                      42 LOAD_NAME                3 (str)
-                      44 BUILD_TUPLE              2
-                      46 LOAD_CONST               8 (<code object get_url_without_parameters, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 24>)
-                      48 MAKE_FUNCTION            4 (annotations)
-                      50 STORE_NAME               6 (get_url_without_parameters)
+          12          30 LOAD_CONST              16 ((True, False))
+                      32 LOAD_CONST               3 ('return')
+                      34 LOAD_NAME                4 (str)
+                      36 BUILD_TUPLE              2
+                      38 LOAD_CONST               8 (<code object get_path_from_url, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 12>)
+                      40 MAKE_FUNCTION            5 (defaults, annotations)
+                      42 STORE_NAME               6 (get_path_from_url)
          
-          28          52 LOAD_CONST               9 (<code object is_url_dictionary, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 28>)
-                      54 MAKE_FUNCTION            0
-                      56 STORE_NAME               7 (is_url_dictionary)
+          22          44 LOAD_CONST               3 ('return')
+                      46 LOAD_NAME                4 (str)
+                      48 BUILD_TUPLE              2
+                      50 LOAD_CONST               9 (<code object get_url_without_parameters, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 22>)
+                      52 MAKE_FUNCTION            4 (annotations)
+                      54 STORE_NAME               7 (get_url_without_parameters)
          
-          32          58 LOAD_CONST              10 ('domain_with_protocol')
-                      60 LOAD_NAME                3 (str)
-                      62 LOAD_CONST               2 ('return')
-                      64 LOAD_NAME                3 (str)
-                      66 BUILD_TUPLE              4
-                      68 LOAD_CONST              11 (<code object standardize_url, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 32>)
-                      70 MAKE_FUNCTION            4 (annotations)
-                      72 STORE_NAME               8 (standardize_url)
+          25          56 LOAD_CONST              10 (<code object is_url_dictionary, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 25>)
+                      58 MAKE_FUNCTION            0
+                      60 STORE_NAME               8 (is_url_dictionary)
          
-          40          74 LOAD_CONST              16 ((True, True))
-                      76 LOAD_CONST               2 ('return')
-                      78 LOAD_NAME                3 (str)
-                      80 BUILD_TUPLE              2
-                      82 LOAD_CONST              12 (<code object get_domain_from_url, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 40>)
-                      84 MAKE_FUNCTION            5 (defaults, annotations)
-                      86 STORE_NAME               9 (get_domain_from_url)
+          28          62 LOAD_CONST              11 ('domain_with_protocol')
+                      64 LOAD_NAME                4 (str)
+                      66 LOAD_CONST               3 ('return')
+                      68 LOAD_NAME                4 (str)
+                      70 BUILD_TUPLE              4
+                      72 LOAD_CONST              12 (<code object standardize_url, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 28>)
+                      74 MAKE_FUNCTION            4 (annotations)
+                      76 STORE_NAME               9 (standardize_url)
          
-          54          88 LOAD_CONST              13 ('scheme')
-                      90 LOAD_NAME                3 (str)
-                      92 LOAD_CONST               2 ('return')
-                      94 LOAD_NAME                3 (str)
-                      96 BUILD_TUPLE              4
-                      98 LOAD_CONST              14 (<code object add_missing_scheme, file "/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py", line 54>)
-                     100 MAKE_FUNCTION            4 (annotations)
-                     102 STORE_NAME              10 (add_missing_scheme)
-                     104 LOAD_CONST               3 (None)
-                     106 RETURN_VALUE
+          35          78 LOAD_CONST              17 ((True, True))
+                      80 LOAD_CONST               3 ('return')
+                      82 LOAD_NAME                4 (str)
+                      84 BUILD_TUPLE              2
+                      86 LOAD_CONST              13 (<code object get_domain_from_url, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 35>)
+                      88 MAKE_FUNCTION            5 (defaults, annotations)
+                      90 STORE_NAME              10 (get_domain_from_url)
+         
+          48          92 LOAD_CONST              14 ('scheme')
+                      94 LOAD_NAME                4 (str)
+                      96 LOAD_CONST               3 ('return')
+                      98 LOAD_NAME                4 (str)
+                     100 BUILD_TUPLE              4
+                     102 LOAD_CONST              15 (<code object add_missing_scheme, file "/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py", line 48>)
+                     104 MAKE_FUNCTION            4 (annotations)
+                     106 STORE_NAME              11 (add_missing_scheme)
+                     108 LOAD_CONST               4 (None)
+                     110 RETURN_VALUE
          consts
             'Url'
+            'A class to represent and manipulate a URL.'
             'url'
             'return'
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
@@ -134,15 +138,15 @@
                             18 RETURN_VALUE
                consts
                   None
                names      ('url',)
                varnames   ('self', 'url')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+               filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
                name       '__init__'
                firstlineno 9
                lnotab 0x0201
             True
             False
             code
                argcount  : 3
@@ -157,43 +161,43 @@
                   026403a6020000ab0200000000000000007d037c03a00300000000000000
                   000000000000000000000000006404a6010000ab01000000000000000064
                   056b040000000072157c03a0030000000000000000000000000000000000
                   0000006404a6010000ab0100000000000000006e0e740900000000000000
                   0000007c03a6010000ab0100000000000000007d057c01720a7c037c057c
                   0485021900000000000000000053007c037c0564067a0000007c04850219
                   0000000000000000005300
-                13           0 RESUME                   0
+                12           0 RESUME                   0
                
-                14           2 LOAD_FAST                0 (self)
+                13           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_url_without_parameters)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               3 (url)
                
-                15          42 LOAD_FAST                0 (self)
+                14          42 LOAD_FAST                0 (self)
                             44 LOAD_METHOD              1 (is_url_dictionary)
                             66 PRECALL                  0
                             70 CALL                     0
                             80 POP_JUMP_FORWARD_IF_FALSE     4 (to 90)
                             82 LOAD_FAST                2 (without_r_slash)
                             84 POP_JUMP_FORWARD_IF_FALSE     2 (to 90)
                             86 LOAD_CONST               1 (-1)
                             88 JUMP_FORWARD             1 (to 92)
                        >>   90 LOAD_CONST               0 (None)
                        >>   92 STORE_FAST               4 (out_r_slash)
                
-                16          94 LOAD_FAST                3 (url)
+                15          94 LOAD_FAST                3 (url)
                             96 LOAD_METHOD              2 (replace)
                            118 LOAD_CONST               2 ('//')
                            120 LOAD_CONST               3 ('::')
                            122 PRECALL                  2
                            126 CALL                     2
                            136 STORE_FAST               3 (url)
                
-                17         138 LOAD_FAST                3 (url)
+                16         138 LOAD_FAST                3 (url)
                            140 LOAD_METHOD              3 (find)
                            162 LOAD_CONST               4 ('/')
                            164 PRECALL                  1
                            168 CALL                     1
                            178 LOAD_CONST               5 (0)
                            180 COMPARE_OP               4 (>)
                            186 POP_JUMP_FORWARD_IF_FALSE    21 (to 230)
@@ -205,25 +209,25 @@
                            228 JUMP_FORWARD            14 (to 258)
                        >>  230 LOAD_GLOBAL              9 (NULL + len)
                            242 LOAD_FAST                3 (url)
                            244 PRECALL                  1
                            248 CALL                     1
                        >>  258 STORE_FAST               5 (domain_len)
                
-                18         260 LOAD_FAST                1 (with_l_slash)
+                17         260 LOAD_FAST                1 (with_l_slash)
                            262 POP_JUMP_FORWARD_IF_FALSE    10 (to 284)
                
-                19         264 LOAD_FAST                3 (url)
+                18         264 LOAD_FAST                3 (url)
                            266 LOAD_FAST                5 (domain_len)
                            268 LOAD_FAST                4 (out_r_slash)
                            270 BUILD_SLICE              2
                            272 BINARY_SUBSCR
                            282 RETURN_VALUE
                
-                21     >>  284 LOAD_FAST                3 (url)
+                20     >>  284 LOAD_FAST                3 (url)
                            286 LOAD_FAST                5 (domain_len)
                            288 LOAD_CONST               6 (1)
                            290 BINARY_OP                0 (+)
                            294 LOAD_FAST                4 (out_r_slash)
                            296 BUILD_SLICE              2
                            298 BINARY_SUBSCR
                            308 RETURN_VALUE
@@ -235,31 +239,31 @@
                   '/'
                   0
                   1
                names      ('get_url_without_parameters', 'is_url_dictionary', 'replace', 'find', 'len')
                varnames   ('self', 'with_l_slash', 'without_r_slash', 'url', 'out_r_slash', 'domain_len')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+               filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
                name       'get_path_from_url'
-               firstlineno 13
+               firstlineno 12
                lnotab 0x0201280134012c017a0104011402
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab01000000000000000064021900000000
                   0000000000a00100000000000000000000000000000000000000006403a6
                   010000ab0100000000000000006402190000000000000000005300
-                24           0 RESUME                   0
+                22           0 RESUME                   0
                
-                25           2 LOAD_FAST                0 (self)
+                23           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (url)
                             14 LOAD_METHOD              1 (split)
                             36 LOAD_CONST               1 ('?')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_CONST               2 (0)
                             54 BINARY_SUBSCR
@@ -275,30 +279,30 @@
                   '?'
                   0
                   '#'
                names      ('url', 'split')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+               filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
                name       'get_url_without_parameters'
-               firstlineno 24
+               firstlineno 22
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000a0010000000000000000000000000000000000
                   0000006401a6010000ab0100000000000000005300
-                28           0 RESUME                   0
+                25           0 RESUME                   0
                
-                29           2 LOAD_FAST                0 (self)
+                26           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_url_without_parameters)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 LOAD_METHOD              1 (endswith)
                             62 LOAD_CONST               1 ('/')
                             64 PRECALL                  1
                             68 CALL                     1
@@ -306,17 +310,17 @@
                consts
                   None
                   '/'
                names      ('get_url_without_parameters', 'endswith')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+               filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
                name       'is_url_dictionary'
-               firstlineno 28
+               firstlineno 25
                lnotab 0x0201
             'domain_with_protocol'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -327,38 +331,38 @@
                   010000000000000000730264017d027c02a0030000000000000000000000
                   0000000000000000006401a6010000ab01000000000000000072287c0264
                   016b030000000072227408000000000000000000006a0500000000000000
                   00a00600000000000000000000000000000000000000007c02a6010000ab
                   01000000000000000064017a0000006e1e7408000000000000000000006a
                   050000000000000000a00600000000000000000000000000000000000000
                   007c02a6010000ab0100000000000000007d037c017c037a0000005300
-                32           0 RESUME                   0
+                28           0 RESUME                   0
                
-                33           2 LOAD_FAST                0 (self)
+                29           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (url)
                             14 LOAD_GLOBAL              3 (NULL + len)
                             26 LOAD_FAST                1 (domain_with_protocol)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 LOAD_CONST               0 (None)
                             44 BUILD_SLICE              2
                             46 BINARY_SUBSCR
                             56 STORE_FAST               2 (path)
                
-                34          58 LOAD_FAST                2 (path)
+                30          58 LOAD_FAST                2 (path)
                             60 LOAD_METHOD              2 (startswith)
                             82 LOAD_CONST               1 ('/')
                             84 PRECALL                  1
                             88 CALL                     1
                             98 POP_JUMP_FORWARD_IF_TRUE     2 (to 104)
                
-                35         100 LOAD_CONST               1 ('/')
+                31         100 LOAD_CONST               1 ('/')
                            102 STORE_FAST               2 (path)
                
-                36     >>  104 LOAD_FAST                2 (path)
+                32     >>  104 LOAD_FAST                2 (path)
                            106 LOAD_METHOD              3 (endswith)
                            128 LOAD_CONST               1 ('/')
                            130 PRECALL                  1
                            134 CALL                     1
                            144 POP_JUMP_FORWARD_IF_FALSE    40 (to 226)
                            146 LOAD_FAST                2 (path)
                            148 LOAD_CONST               1 ('/')
@@ -377,28 +381,28 @@
                            238 LOAD_ATTR                5 (path)
                            248 LOAD_METHOD              6 (abspath)
                            270 LOAD_FAST                2 (path)
                            272 PRECALL                  1
                            276 CALL                     1
                        >>  286 STORE_FAST               3 (abs)
                
-                37         288 LOAD_FAST                1 (domain_with_protocol)
+                33         288 LOAD_FAST                1 (domain_with_protocol)
                            290 LOAD_FAST                3 (abs)
                            292 BINARY_OP                0 (+)
                            296 RETURN_VALUE
                consts
                   None
                   '/'
                names      ('url', 'len', 'startswith', 'endswith', 'os', 'path', 'abspath')
                varnames   ('self', 'domain_with_protocol', 'path', 'abs')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+               filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
                name       'standardize_url'
-               firstlineno 32
+               firstlineno 28
                lnotab 0x020138012a010401b801
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 3
                flags     : 3
                code
@@ -408,58 +412,58 @@
                   0300000000000000007c0272147c036a040000000000000000720a7c036a
                   04000000000000000064027a0000006e0164037d046e0264047d047c0172
                   267c047c036a0300000000000000007a0000007c036a0500000000000000
                   007a0000007c036a060000000000000000720264016e0164047a0000007c
                   036a0600000000000000007a00000053007c047c036a0500000000000000
                   007a0000007c036a060000000000000000720264016e0164047a0000007c
                   036a0600000000000000007a0000005300
-                40           0 RESUME                   0
+                35           0 RESUME                   0
                
-                41           2 LOAD_GLOBAL              1 (NULL + tldparser)
+                36           2 LOAD_GLOBAL              1 (NULL + tldparser)
                             14 LOAD_ATTR                1 (parse)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (url)
                             36 PRECALL                  1
                             40 CALL                     1
                             50 STORE_FAST               3 (extract)
                
-                42          52 LOAD_FAST                3 (extract)
+                37          52 LOAD_FAST                3 (extract)
                             54 LOAD_ATTR                3 (subdomain)
                             64 POP_JUMP_FORWARD_IF_FALSE    16 (to 98)
                
-                43          66 LOAD_FAST                3 (extract)
+                38          66 LOAD_FAST                3 (extract)
                             68 COPY                     1
                             70 LOAD_ATTR                3 (subdomain)
                             80 LOAD_CONST               1 ('.')
                             82 BINARY_OP               13 (+=)
                             86 SWAP                     2
                             88 STORE_ATTR               3 (subdomain)
                
-                44     >>   98 LOAD_FAST                2 (with_protocol)
+                39     >>   98 LOAD_FAST                2 (with_protocol)
                            100 POP_JUMP_FORWARD_IF_FALSE    20 (to 142)
                
-                45         102 LOAD_FAST                3 (extract)
+                40         102 LOAD_FAST                3 (extract)
                            104 LOAD_ATTR                4 (scheme)
                            114 POP_JUMP_FORWARD_IF_FALSE    10 (to 136)
                            116 LOAD_FAST                3 (extract)
                            118 LOAD_ATTR                4 (scheme)
                            128 LOAD_CONST               2 ('://')
                            130 BINARY_OP                0 (+)
                            134 JUMP_FORWARD             1 (to 138)
                        >>  136 LOAD_CONST               3 ('http://')
                        >>  138 STORE_FAST               4 (protocol)
                            140 JUMP_FORWARD             2 (to 146)
                
-                47     >>  142 LOAD_CONST               4 ('')
+                42     >>  142 LOAD_CONST               4 ('')
                            144 STORE_FAST               4 (protocol)
                
-                48     >>  146 LOAD_FAST                1 (level)
+                43     >>  146 LOAD_FAST                1 (level)
                            148 POP_JUMP_FORWARD_IF_FALSE    38 (to 226)
                
-                49         150 LOAD_FAST                4 (protocol)
+                44         150 LOAD_FAST                4 (protocol)
                            152 LOAD_FAST                3 (extract)
                            154 LOAD_ATTR                3 (subdomain)
                            164 BINARY_OP                0 (+)
                            168 LOAD_FAST                3 (extract)
                            170 LOAD_ATTR                5 (domain)
                            180 BINARY_OP                0 (+)
                            184 LOAD_FAST                3 (extract)
@@ -470,15 +474,15 @@
                        >>  202 LOAD_CONST               4 ('')
                        >>  204 BINARY_OP                0 (+)
                            208 LOAD_FAST                3 (extract)
                            210 LOAD_ATTR                6 (suffix)
                            220 BINARY_OP                0 (+)
                            224 RETURN_VALUE
                
-                51     >>  226 LOAD_FAST                4 (protocol)
+                46     >>  226 LOAD_FAST                4 (protocol)
                            228 LOAD_FAST                3 (extract)
                            230 LOAD_ATTR                5 (domain)
                            240 BINARY_OP                0 (+)
                            244 LOAD_FAST                3 (extract)
                            246 LOAD_ATTR                6 (suffix)
                            256 POP_JUMP_FORWARD_IF_FALSE     2 (to 262)
                            258 LOAD_CONST               1 ('.')
@@ -495,82 +499,82 @@
                   '://'
                   'http://'
                   ''
                names      ('tldparser', 'parse', 'url', 'subdomain', 'scheme', 'domain', 'suffix')
                varnames   ('self', 'level', 'with_protocol', 'extract', 'protocol')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+               filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
                name       'get_domain_from_url'
-               firstlineno 40
+               firstlineno 35
                lnotab 0x020132010e01200104012802040104014c02
             'scheme'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007400000000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000007c006a030000000000000000a6
                   010000ab0100000000000000007d027c006a03000000000000000072147c
                   026a040000000000000000730d7c0164017a0000007c006a030000000000
                   0000007a00000053007c006a0300000000000000005300
-                54           0 RESUME                   0
+                48           0 RESUME                   0
                
-                55           2 LOAD_GLOBAL              0 (urllib)
+                49           2 LOAD_GLOBAL              0 (urllib)
                             14 LOAD_ATTR                1 (parse)
                             24 LOAD_METHOD              2 (urlparse)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (url)
                             58 PRECALL                  1
                             62 CALL                     1
                             72 STORE_FAST               2 (extract)
                
-                56          74 LOAD_FAST                0 (self)
+                50          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                3 (url)
                             86 POP_JUMP_FORWARD_IF_FALSE    20 (to 128)
                             88 LOAD_FAST                2 (extract)
                             90 LOAD_ATTR                4 (scheme)
                            100 POP_JUMP_FORWARD_IF_TRUE    13 (to 128)
                
-                57         102 LOAD_FAST                1 (scheme)
+                51         102 LOAD_FAST                1 (scheme)
                            104 LOAD_CONST               1 ('://')
                            106 BINARY_OP                0 (+)
                            110 LOAD_FAST                0 (self)
                            112 LOAD_ATTR                3 (url)
                            122 BINARY_OP                0 (+)
                            126 RETURN_VALUE
                
-                59     >>  128 LOAD_FAST                0 (self)
+                53     >>  128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                3 (url)
                            140 RETURN_VALUE
                consts
                   None
                   '://'
                names      ('urllib', 'parse', 'urlparse', 'url', 'scheme')
                varnames   ('self', 'scheme', 'extract')
                freevars   ()
                cellvars   ()
-               filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+               filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
                name       'add_missing_scheme'
-               firstlineno 54
+               firstlineno 48
                lnotab 0x020148011c011a02
             (True, False)
             (True, True)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'get_path_from_url', 'get_url_without_parameters', 'is_url_dictionary', 'standardize_url', 'get_domain_from_url', 'add_missing_scheme')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', 'get_path_from_url', 'get_url_without_parameters', 'is_url_dictionary', 'standardize_url', 'get_domain_from_url', 'add_missing_scheme')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+         filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
          name       'Url'
          firstlineno 7
-         lnotab 0x0a0210040e0b0c04060410080e0e
+         lnotab 0x0a01040110030e0a0c03060310070e0d
       'Url'
    names      ('os', 'ptlibs', 'tldparser', 'urllib.parse', 'urllib', 'Url')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/kali/penterep/dkummel/ptwebdiscover/ptwebdiscover/utils/url.py'
+   filename   '/home/kali/penterep/penterep-public/ptwebdiscover/ptwebdiscover/utils/url.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108020c010803
```

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/utils/cachefile.py` & `ptwebdiscover-1.0.7/ptwebdiscover/utils/cachefile.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/utils/treeshow.py` & `ptwebdiscover-1.0.7/ptwebdiscover/utils/treeshow.py`

 * *Files identical despite different names*

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover/utils/url.py` & `ptwebdiscover-1.0.7/ptwebdiscover/utils/url.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,53 @@
 import os
 
 from ptlibs import tldparser
 import urllib.parse
 
 
 class Url:
-
+    """A class to represent and manipulate a URL."""
     def __init__(self, url: str) -> None:
         self.url = url
 
-
     def get_path_from_url(self, with_l_slash=True, without_r_slash=False) -> str:
         url = self.get_url_without_parameters()
         out_r_slash = -1 if self.is_url_dictionary() and without_r_slash else None
         url = url.replace("//", "::")
         domain_len = url.find("/") if url.find("/")>0 else len(url)
         if with_l_slash:
             return url[domain_len:out_r_slash]
         else:
             return url[domain_len+1:out_r_slash]
 
-
     def get_url_without_parameters(self) -> str:
         return self.url.split("?")[0].split("#")[0]
 
-
     def is_url_dictionary(self):
         return self.get_url_without_parameters().endswith("/")
 
-
     def standardize_url(self, domain_with_protocol: str) -> str:
         path = self.url[len(domain_with_protocol):]
         if not path.startswith("/"):
             path = "/"
         abs = os.path.abspath(path)+"/" if path.endswith("/") and path !="/" else os.path.abspath(path)
         return domain_with_protocol + abs
 
-
     def get_domain_from_url(self, level=True, with_protocol=True) -> str:
         extract = tldparser.parse(self.url)
         if extract.subdomain:
             extract.subdomain += "."
         if with_protocol:
             protocol = extract.scheme + "://" if extract.scheme else "http://"
         else:
             protocol = ""
         if level:
             return protocol + extract.subdomain + extract.domain + ("." if extract.suffix else "") + extract.suffix
         else:
             return protocol + extract.domain + ("." if extract.suffix else "") + extract.suffix
 
-
     def add_missing_scheme(self, scheme: str) -> str:
         extract = urllib.parse.urlparse(self.url)
         if self.url and not (extract.scheme):
             return scheme + "://" + self.url
         else:
             return self.url
```

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover.egg-info/PKG-INFO` & `ptwebdiscover-1.0.7/ptwebdiscover.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptwebdiscover
-Version: 1.0.6
+Version: 1.0.7
 Summary: Web Source Discovery Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `ptwebdiscover-1.0.6/ptwebdiscover.egg-info/SOURCES.txt` & `ptwebdiscover-1.0.7/ptwebdiscover.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,10 @@
 ptwebdiscover/ptdataclasses/findingdetail.py
 ptwebdiscover/ptdataclasses/processedargumentoptions.py
 ptwebdiscover/utils/__init__.py
 ptwebdiscover/utils/cachefile.py
 ptwebdiscover/utils/treeshow.py
 ptwebdiscover/utils/url.py
 ptwebdiscover/utils/__pycache__/__init__.cpython-311.pyc
+ptwebdiscover/utils/__pycache__/cachefile.cpython-311.pyc
 ptwebdiscover/utils/__pycache__/treeshow.cpython-311.pyc
 ptwebdiscover/utils/__pycache__/url.cpython-311.pyc
```

### Comparing `ptwebdiscover-1.0.6/setup.py` & `ptwebdiscover-1.0.7/setup.py`

 * *Files identical despite different names*

