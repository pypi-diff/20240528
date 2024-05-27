# Comparing `tmp/ElPeriodic-1.2.tar.gz` & `tmp/elperiodic-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ElPeriodic-1.2.tar", last modified: Tue Dec  1 02:00:30 2020, max compression
+gzip compressed data, was "elperiodic-1.3.tar", last modified: Mon May 27 23:38:48 2024, max compression
```

## Comparing `ElPeriodic-1.2.tar` & `elperiodic-1.3.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 02:00:30.416426 ElPeriodic-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 02:00:30.412426 ElPeriodic-1.2/ElPeriodic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3194 2020-12-01 02:00:30.000000 ElPeriodic-1.2/ElPeriodic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      741 2020-12-01 02:00:30.000000 ElPeriodic-1.2/ElPeriodic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-01 02:00:30.000000 ElPeriodic-1.2/ElPeriodic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-01 02:00:30.000000 ElPeriodic-1.2/ElPeriodic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      421 2020-12-01 02:00:21.000000 ElPeriodic-1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3194 2020-12-01 02:00:30.416426 ElPeriodic-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2254 2020-12-01 02:00:21.000000 ElPeriodic-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 02:00:30.412426 ElPeriodic-1.2/python/
--rw-r--r--   0 runner    (1001) docker     (116)     5544 2020-12-01 02:00:21.000000 ElPeriodic-1.2/python/ElPeriodic.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-01 02:00:21.000000 ElPeriodic-1.2/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-01 02:00:30.416426 ElPeriodic-1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1459 2020-12-01 02:00:21.000000 ElPeriodic-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-01 02:00:30.416426 ElPeriodic-1.2/src/
--rw-r--r--   0 runner    (1001) docker     (116)      915 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/Symbol.map
--rw-r--r--   0 runner    (1001) docker     (116)     2122 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/elperiodic.h
--rw-r--r--   0 runner    (1001) docker     (116)     7571 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/periodic.c
--rw-r--r--   0 runner    (1001) docker     (116)     1977 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_band.h
--rw-r--r--   0 runner    (1001) docker     (116)     2142 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_fd.c
--rw-r--r--   0 runner    (1001) docker     (116)     1699 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_fd.h
--rw-r--r--   0 runner    (1001) docker     (116)     1642 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_inst.h
--rw-r--r--   0 runner    (1001) docker     (116)     3256 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_main.c
--rw-r--r--   0 runner    (1001) docker     (116)     1621 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_main.h
--rw-r--r--   0 runner    (1001) docker     (116)     3729 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_main_fd.c
--rw-r--r--   0 runner    (1001) docker     (116)     1574 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_main_fd.h
--rw-r--r--   0 runner    (1001) docker     (116)     3431 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_main_pfd.c
--rw-r--r--   0 runner    (1001) docker     (116)     1573 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_main_pfd.h
--rw-r--r--   0 runner    (1001) docker     (116)     1710 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_math.c
--rw-r--r--   0 runner    (1001) docker     (116)     1834 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_math.h
--rw-r--r--   0 runner    (1001) docker     (116)     2317 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_pfd.c
--rw-r--r--   0 runner    (1001) docker     (116)     1680 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_pfd.h
--rw-r--r--   0 runner    (1001) docker     (116)     1636 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_procchain.h
--rw-r--r--   0 runner    (1001) docker     (116)     2295 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_recfilter.c
--rw-r--r--   0 runner    (1001) docker     (116)     1854 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_recfilter.h
--rw-r--r--   0 runner    (1001) docker     (116)     2031 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_shmtrig.c
--rw-r--r--   0 runner    (1001) docker     (116)     1702 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_shmtrig.h
--rw-r--r--   0 runner    (1001) docker     (116)     5529 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_sign.c
--rw-r--r--   0 runner    (1001) docker     (116)     1692 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_sign.h
--rw-r--r--   0 runner    (1001) docker     (116)     1625 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_sign_ctx.h
--rw-r--r--   0 runner    (1001) docker     (116)     1572 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_sign_impl.h
--rw-r--r--   0 runner    (1001) docker     (116)     2113 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_time.h
--rw-r--r--   0 runner    (1001) docker     (116)     4331 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_timespecops.h
--rw-r--r--   0 runner    (1001) docker     (116)     1545 2020-12-01 02:00:21.000000 ElPeriodic-1.2/src/prdic_types.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:38:48.963264 elperiodic-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-27 23:38:37.000000 elperiodic-1.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-27 23:38:37.000000 elperiodic-1.3/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:38:48.963264 elperiodic-1.3/ElPeriodic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-27 23:38:48.000000 elperiodic-1.3/ElPeriodic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-27 23:38:48.000000 elperiodic-1.3/ElPeriodic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:38:48.000000 elperiodic-1.3/ElPeriodic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-27 23:38:48.000000 elperiodic-1.3/ElPeriodic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-27 23:38:37.000000 elperiodic-1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-27 23:38:48.963264 elperiodic-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-27 23:38:37.000000 elperiodic-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:38:48.955264 elperiodic-1.3/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 23:38:37.000000 elperiodic-1.3/python/ElPeriodic.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:38:37.000000 elperiodic-1.3/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 23:38:48.963264 elperiodic-1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 23:38:37.000000 elperiodic-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:38:48.963264 elperiodic-1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-27 23:38:37.000000 elperiodic-1.3/src/Symbol.map
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-27 23:38:37.000000 elperiodic-1.3/src/elperiodic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-27 23:38:37.000000 elperiodic-1.3/src/periodic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_band.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_fd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_fd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_inst.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_main.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_main.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_main_fd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_main_fd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_main_pfd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_main_pfd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_math.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_math.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_pfd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_pfd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_procchain.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_recfilter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_recfilter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_shmtrig.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_shmtrig.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_sign.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_sign.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_sign_ctx.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_sign_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_time.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_timespecops.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-27 23:38:37.000000 elperiodic-1.3/src/prdic_types.h
```

### Comparing `ElPeriodic-1.2/ElPeriodic.egg-info/PKG-INFO` & `elperiodic-1.3/ElPeriodic.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 Metadata-Version: 2.1
 Name: ElPeriodic
-Version: 1.2
+Version: 1.3
 Summary: Phase-locked userland scheduling library
 Home-page: https://github.com/sobomax/libelperiodic
 Author: Maksym Sobolyev
 Author-email: sobomax@gmail.com
-License: UNKNOWN
-Description: [![Build Status@GitHub](https://github.com/sobomax/libelperiodic/workflows/Main%20CI/badge.svg?branch=master)](https://github.com/sobomax/libelperiodic/actions?query=branch%3Amaster++)
-        [![Build Status](https://travis-ci.com/sobomax/libelperiodic.svg?branch=master)](https://travis-ci.com/sobomax/libelperiodic)
-        [![Coverage Status](https://coveralls.io/repos/github/sobomax/libelperiodic/badge.svg?branch=master)](https://coveralls.io/github/sobomax/libelperiodic?branch=master)
-        
-        # libElPeriodic
-        Library to run frequent periodic tasks.
-        
-        ## Principle of Operation
-        The libElPeriodic is designed to simplify writing control loops that are
-        expected to run at constant "tick" intervals with smallest possible overhead
-        and little or no support from the underlying run time environment.
-        
-        The library is optimized to align active periods of the control loop
-        to the set frequency (and optionally phase as well) by applying phase
-        locked loop design with a proportional phase detector and a low-pass
-        filter as an error amplifier.
-        
-        ## Usage
-        
-        Sample usage pattern is demonstrated below. The code block denoted by the square
-        brackets will be executing 125.5 times a second, untul the value returned by the
-        `is_runnable()` routine is non-zero. Provided of course that the "logic"
-        does not take more than 0.01 second to run on average and that OS scheduler
-        plays the ball.
-        
-            #include <elperiodic.h>
-        
-            extern int is_runnable(void);
-        
-            void
-            event_loop(void)
-            {
-                double frequency = 125.5; /* Hz */
-                void *elp;
-                int i;
-        
-                prd = prdic_init(freq, 0.0);
-                assert(prd != NULL);
-        
-                while (is_runnable()) {
-            //      [----------------------];
-            //      [Insert your logic here];
-            //      [----------------------];
-                    prdic_procrastinate(prd);
-                }
-                prdic_free(prd);
-            }
-        
-        ## Story
-        
-        It came about having to write the same code over and over again in multiple
-        real-time projects, ranging from game [Digger](https://github.com/sobomax/digger),
-        RTP relay server [RTPProxy](https://github.com/sippy/rtpproxy). It has also
-        been recently utilized to replace a heavy-weight (and at the time not portable
-        to Python 3) "Twisted" framework in the
-        [Python Sippy B2BUA](https://github.com/sippy/b2bua) project.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: AUTHORS
+
+[![Build Status@GitHub](https://github.com/sobomax/libelperiodic/workflows/Main%20CI/badge.svg?branch=master)](https://github.com/sobomax/libelperiodic/actions?query=branch%3Amaster++)
+[![Build Status](https://travis-ci.com/sobomax/libelperiodic.svg?branch=master)](https://travis-ci.com/sobomax/libelperiodic)
+[![Coverage Status](https://coveralls.io/repos/github/sobomax/libelperiodic/badge.svg?branch=master)](https://coveralls.io/github/sobomax/libelperiodic?branch=master)
+
+# libElPeriodic
+Library to run frequent periodic tasks.
+
+## Principle of Operation
+The libElPeriodic is designed to simplify writing control loops that are
+expected to run at constant "tick" intervals with smallest possible overhead
+and little or no support from the underlying run time environment.
+
+The library is optimized to align active periods of the control loop
+to the set frequency (and optionally phase as well) by applying phase
+locked loop design with a proportional phase detector and a low-pass
+filter as an error amplifier.
+
+## Usage
+
+Sample usage pattern is demonstrated below. The code block denoted by the square
+brackets will be executing 125.5 times a second, untul the value returned by the
+`is_runnable()` routine is non-zero. Provided of course that the "logic"
+does not take more than 0.01 second to run on average and that OS scheduler
+plays the ball.
+
+    #include <elperiodic.h>
+
+    extern int is_runnable(void);
+
+    void
+    event_loop(void)
+    {
+        double frequency = 125.5; /* Hz */
+        void *elp;
+
+        prd = prdic_init(freq, 0.0);
+        assert(prd != NULL);
+
+        while (is_runnable()) {
+    //      [----------------------];
+    //      [Insert your logic here];
+    //      [----------------------];
+            prdic_procrastinate(prd);
+        }
+        prdic_free(prd);
+    }
+
+## Story
+
+It came about having to write the same code over and over again in multiple
+real-time projects, ranging from game [Digger](https://github.com/sobomax/digger),
+RTP relay server [RTPProxy](https://github.com/sippy/rtpproxy). It has also
+been recently utilized to replace a heavy-weight (and at the time not portable
+to Python 3) "Twisted" framework in the
+[Python Sippy B2BUA](https://github.com/sippy/b2bua) project.
```

### Comparing `ElPeriodic-1.2/ElPeriodic.egg-info/SOURCES.txt` & `elperiodic-1.3/ElPeriodic.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+AUTHORS
+COPYING
 MANIFEST.in
 README.md
 setup.py
 ElPeriodic.egg-info/PKG-INFO
 ElPeriodic.egg-info/SOURCES.txt
 ElPeriodic.egg-info/dependency_links.txt
 ElPeriodic.egg-info/top_level.txt
```

### Comparing `ElPeriodic-1.2/PKG-INFO` & `elperiodic-1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,71 @@
 Metadata-Version: 2.1
 Name: ElPeriodic
-Version: 1.2
+Version: 1.3
 Summary: Phase-locked userland scheduling library
 Home-page: https://github.com/sobomax/libelperiodic
 Author: Maksym Sobolyev
 Author-email: sobomax@gmail.com
-License: UNKNOWN
-Description: [![Build Status@GitHub](https://github.com/sobomax/libelperiodic/workflows/Main%20CI/badge.svg?branch=master)](https://github.com/sobomax/libelperiodic/actions?query=branch%3Amaster++)
-        [![Build Status](https://travis-ci.com/sobomax/libelperiodic.svg?branch=master)](https://travis-ci.com/sobomax/libelperiodic)
-        [![Coverage Status](https://coveralls.io/repos/github/sobomax/libelperiodic/badge.svg?branch=master)](https://coveralls.io/github/sobomax/libelperiodic?branch=master)
-        
-        # libElPeriodic
-        Library to run frequent periodic tasks.
-        
-        ## Principle of Operation
-        The libElPeriodic is designed to simplify writing control loops that are
-        expected to run at constant "tick" intervals with smallest possible overhead
-        and little or no support from the underlying run time environment.
-        
-        The library is optimized to align active periods of the control loop
-        to the set frequency (and optionally phase as well) by applying phase
-        locked loop design with a proportional phase detector and a low-pass
-        filter as an error amplifier.
-        
-        ## Usage
-        
-        Sample usage pattern is demonstrated below. The code block denoted by the square
-        brackets will be executing 125.5 times a second, untul the value returned by the
-        `is_runnable()` routine is non-zero. Provided of course that the "logic"
-        does not take more than 0.01 second to run on average and that OS scheduler
-        plays the ball.
-        
-            #include <elperiodic.h>
-        
-            extern int is_runnable(void);
-        
-            void
-            event_loop(void)
-            {
-                double frequency = 125.5; /* Hz */
-                void *elp;
-                int i;
-        
-                prd = prdic_init(freq, 0.0);
-                assert(prd != NULL);
-        
-                while (is_runnable()) {
-            //      [----------------------];
-            //      [Insert your logic here];
-            //      [----------------------];
-                    prdic_procrastinate(prd);
-                }
-                prdic_free(prd);
-            }
-        
-        ## Story
-        
-        It came about having to write the same code over and over again in multiple
-        real-time projects, ranging from game [Digger](https://github.com/sobomax/digger),
-        RTP relay server [RTPProxy](https://github.com/sippy/rtpproxy). It has also
-        been recently utilized to replace a heavy-weight (and at the time not portable
-        to Python 3) "Twisted" framework in the
-        [Python Sippy B2BUA](https://github.com/sippy/b2bua) project.
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: AUTHORS
+
+[![Build Status@GitHub](https://github.com/sobomax/libelperiodic/workflows/Main%20CI/badge.svg?branch=master)](https://github.com/sobomax/libelperiodic/actions?query=branch%3Amaster++)
+[![Build Status](https://travis-ci.com/sobomax/libelperiodic.svg?branch=master)](https://travis-ci.com/sobomax/libelperiodic)
+[![Coverage Status](https://coveralls.io/repos/github/sobomax/libelperiodic/badge.svg?branch=master)](https://coveralls.io/github/sobomax/libelperiodic?branch=master)
+
+# libElPeriodic
+Library to run frequent periodic tasks.
+
+## Principle of Operation
+The libElPeriodic is designed to simplify writing control loops that are
+expected to run at constant "tick" intervals with smallest possible overhead
+and little or no support from the underlying run time environment.
+
+The library is optimized to align active periods of the control loop
+to the set frequency (and optionally phase as well) by applying phase
+locked loop design with a proportional phase detector and a low-pass
+filter as an error amplifier.
+
+## Usage
+
+Sample usage pattern is demonstrated below. The code block denoted by the square
+brackets will be executing 125.5 times a second, untul the value returned by the
+`is_runnable()` routine is non-zero. Provided of course that the "logic"
+does not take more than 0.01 second to run on average and that OS scheduler
+plays the ball.
+
+    #include <elperiodic.h>
+
+    extern int is_runnable(void);
+
+    void
+    event_loop(void)
+    {
+        double frequency = 125.5; /* Hz */
+        void *elp;
+
+        prd = prdic_init(freq, 0.0);
+        assert(prd != NULL);
+
+        while (is_runnable()) {
+    //      [----------------------];
+    //      [Insert your logic here];
+    //      [----------------------];
+            prdic_procrastinate(prd);
+        }
+        prdic_free(prd);
+    }
+
+## Story
+
+It came about having to write the same code over and over again in multiple
+real-time projects, ranging from game [Digger](https://github.com/sobomax/digger),
+RTP relay server [RTPProxy](https://github.com/sippy/rtpproxy). It has also
+been recently utilized to replace a heavy-weight (and at the time not portable
+to Python 3) "Twisted" framework in the
+[Python Sippy B2BUA](https://github.com/sippy/b2bua) project.
```

### Comparing `ElPeriodic-1.2/README.md` & `elperiodic-1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     extern int is_runnable(void);
 
     void
     event_loop(void)
     {
         double frequency = 125.5; /* Hz */
         void *elp;
-        int i;
 
         prd = prdic_init(freq, 0.0);
         assert(prd != NULL);
 
         while (is_runnable()) {
     //      [----------------------];
     //      [Insert your logic here];
```

### Comparing `ElPeriodic-1.2/python/ElPeriodic.py` & `elperiodic-1.3/python/ElPeriodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,18 @@
 class ElPeriodic(object):
     _hndl = None
     _elpl = None
     _cbfunc = None
 
     def __init__(self, freq, offst = 0.0):
         self._elpl = _elpl
-        self._hndl = self._elpl.prdic_init(freq, offst)
-        if not bool(self._hndl):
+        _hndl = self._elpl.prdic_init(freq, offst)
+        if not bool(_hndl):
             raise Exception('prdic_init() failed')
+        self._hndl = _hndl
 
     def procrastinate(self):
         self._elpl.prdic_procrastinate(self._hndl)
 
     def addband(self, freq_hz):
         r = self._elpl.prdic_addband(self._hndl, freq_hz)
         return int(r)
@@ -129,16 +130,17 @@
         ts = timespec()
         tv_frac, tv_sec = modf(dtime)
         ts.tv_sec = int(tv_sec)
         ts.tv_nsec = int(tv_frac * 1e+09)
         self._elpl.prdic_set_epoch(self._hndl, byref(ts))
 
     def __del__(self):
-        if bool(self._hndl):
+        if self._hndl is not None:
             self._elpl.prdic_free(self._hndl)
+            self._hndl = None
 
     def CFT_enable(self, signum, ptrcall_class = _elpl_ptrcall_bare):
         if pythonapi == None:
             raise Exception('pythonapi is None')
         r = self._elpl.prdic_CFT_enable(self._hndl, c_int(signum))
         if r != 0:
             raise Exception('prdic_CFT_enable() = %d' % (r,))
```

### Comparing `ElPeriodic-1.2/setup.py` & `elperiodic-1.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 #!/usr/bin/env python
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 from distutils.core import Extension
-import os
+from os import environ
+from sysconfig import get_platform
 
 elp_srcs = ['src/periodic.c', 'src/prdic_math.c', \
  'src/prdic_fd.c', \
  'src/prdic_pfd.c', \
  'src/prdic_main_fd.c', 'src/prdic_main_pfd.c', \
  'src/prdic_main.c', \
  'src/prdic_recfilter.c', 'src/prdic_shmtrig.c', \
  'src/prdic_sign.c']
 
+el_args = None if get_platform().startswith('macosx-') else ['-Wl,--version-script=src/Symbol.map',]
 module1 = Extension('_elperiodic', sources = elp_srcs, \
-    extra_link_args = ['-Wl,--version-script=src/Symbol.map',])
+    extra_link_args = el_args)
 
 def get_ex_mod():
-    if 'NO_PY_EXT' in os.environ:
+    if 'NO_PY_EXT' in environ:
         return None
     return [module1]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 kwargs = {
       'name':'ElPeriodic',
-      'version':'1.2',
+      'version':'1.3',
       'description':'Phase-locked userland scheduling library',
       'long_description': long_description,
       'long_description_content_type': "text/markdown",
       'author':'Maksym Sobolyev',
       'author_email':'sobomax@gmail.com',
       'url':'https://github.com/sobomax/libelperiodic',
       'packages':['elperiodic',],
```

### Comparing `ElPeriodic-1.2/src/Symbol.map` & `elperiodic-1.3/src/Symbol.map`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/elperiodic.h` & `elperiodic-1.3/src/elperiodic.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/periodic.c` & `elperiodic-1.3/src/periodic.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_band.h` & `elperiodic-1.3/src/prdic_band.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_fd.c` & `elperiodic-1.3/src/prdic_fd.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_fd.h` & `elperiodic-1.3/src/prdic_fd.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_inst.h` & `elperiodic-1.3/src/prdic_inst.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_main.c` & `elperiodic-1.3/src/prdic_main.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_main.h` & `elperiodic-1.3/src/prdic_main.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_main_fd.c` & `elperiodic-1.3/src/prdic_main_fd.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_main_fd.h` & `elperiodic-1.3/src/prdic_main_fd.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_main_pfd.c` & `elperiodic-1.3/src/prdic_main_pfd.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_main_pfd.h` & `elperiodic-1.3/src/prdic_main_pfd.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_math.c` & `elperiodic-1.3/src/prdic_math.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_math.h` & `elperiodic-1.3/src/prdic_math.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_pfd.c` & `elperiodic-1.3/src/prdic_pfd.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_pfd.h` & `elperiodic-1.3/src/prdic_pfd.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_procchain.h` & `elperiodic-1.3/src/prdic_procchain.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_recfilter.c` & `elperiodic-1.3/src/prdic_recfilter.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_recfilter.h` & `elperiodic-1.3/src/prdic_recfilter.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_shmtrig.c` & `elperiodic-1.3/src/prdic_shmtrig.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_shmtrig.h` & `elperiodic-1.3/src/prdic_shmtrig.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_sign.c` & `elperiodic-1.3/src/prdic_sign.c`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_sign.h` & `elperiodic-1.3/src/prdic_sign.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_sign_ctx.h` & `elperiodic-1.3/src/prdic_sign_ctx.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_sign_impl.h` & `elperiodic-1.3/src/prdic_sign_impl.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_time.h` & `elperiodic-1.3/src/prdic_time.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_timespecops.h` & `elperiodic-1.3/src/prdic_timespecops.h`

 * *Files identical despite different names*

### Comparing `ElPeriodic-1.2/src/prdic_types.h` & `elperiodic-1.3/src/prdic_types.h`

 * *Files identical despite different names*

