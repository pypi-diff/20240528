# Comparing `tmp/midea_local-1.0.3.tar.gz` & `tmp/midea_local-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midea_local-1.0.3.tar", last modified: Thu May 23 17:42:57 2024, max compression
+gzip compressed data, was "midea_local-1.0.4.tar", last modified: Tue May 28 21:57:32 2024, max compression
```

## Comparing `midea_local-1.0.3.tar` & `midea_local-1.0.4.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 17:42:49.000000 midea_local-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-23 17:42:57.129418 midea_local-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-23 17:42:49.000000 midea_local-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midea_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 17:42:57.000000 midea_local-1.0.3/midea_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/backports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/backports/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/crc8.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/devices/a1/
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/a1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/a1/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.117417 midea_local-1.0.3/midealocal/devices/ac/
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25127 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ac/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b0/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b0/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b1/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b1/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b3/
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b3/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b4/
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b4/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/b6/
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/b6/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/bf/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/bf/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/c2/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c2/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/c3/
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/c3/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ca/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/cc/
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cc/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/cd/
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cd/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.121417 midea_local-1.0.3/midealocal/devices/ce/
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ce/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/cf/
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/cf/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/da/
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/da/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/da/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/db/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/db/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/dc/
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/dc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/dc/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e1/
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e1/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e2/
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e2/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e3/
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e3/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e6/
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e6/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/e8/
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/e8/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/ea/
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ea/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/ec/
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ec/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/ed/
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/ed/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.125417 midea_local-1.0.3/midealocal/devices/fa/
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fa/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/fb/
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fb/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/fc/
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fc/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/fd/
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/fd/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x13/
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x13/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x26/
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x26/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x26/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x34/
--rw-r--r--   0 runner    (1001) docker     (127)     6137 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x34/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x34/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:42:57.129418 midea_local-1.0.3/midealocal/devices/x40/
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x40/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/devices/x40/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/discover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/packet_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9780 2024-05-23 17:42:49.000000 midea_local-1.0.3/midealocal/security.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:42:57.129418 midea_local-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-23 17:42:49.000000 midea_local-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 21:57:28.000000 midea_local-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-28 21:57:32.927553 midea_local-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-28 21:57:28.000000 midea_local-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midea_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-28 21:57:32.000000 midea_local-1.0.4/midea_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-28 21:57:32.000000 midea_local-1.0.4/midea_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:57:32.000000 midea_local-1.0.4/midea_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 21:57:32.000000 midea_local-1.0.4/midea_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 21:57:32.000000 midea_local-1.0.4/midea_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.915553 midea_local-1.0.4/midealocal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.915553 midea_local-1.0.4/midealocal/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/backports/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26761 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/crc8.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.915553 midea_local-1.0.4/midealocal/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.915553 midea_local-1.0.4/midealocal/devices/a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/a1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6432 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/a1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.915553 midea_local-1.0.4/midealocal/devices/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25360 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ac/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.915553 midea_local-1.0.4/midealocal/devices/b0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b0/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.915553 midea_local-1.0.4/midealocal/devices/b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b4/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/b6/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/bf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/bf/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/c2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/c2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/c2/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/c3/
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/c3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ca/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/cc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/cd/
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/cd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/cd/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.919553 midea_local-1.0.4/midealocal/devices/ce/
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ce/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/cf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/cf/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/da/
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/da/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/db/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/dc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/dc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/dc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/e1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e1/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/e2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e2/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/e3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e3/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/e6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e6/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/e8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/e8/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/ea/
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ea/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/ec/
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ec/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.923553 midea_local-1.0.4/midealocal/devices/ed/
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/ed/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)    13512 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fa/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/fb/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fb/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/fc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fc/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/fd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/fd/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/x13/
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x13/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/x26/
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x26/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x26/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/x34/
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x34/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x34/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:57:32.927553 midea_local-1.0.4/midealocal/devices/x40/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x40/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/devices/x40/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/discover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/packet_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-28 21:57:28.000000 midea_local-1.0.4/midealocal/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:57:32.927553 midea_local-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-28 21:57:28.000000 midea_local-1.0.4/setup.py
```

### Comparing `midea_local-1.0.3/LICENSE` & `midea_local-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.3/PKG-INFO` & `midea_local-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midea-local
-Version: 1.0.3
+Version: 1.0.4
 Summary: Control your Midea M-Smart appliances via local area network
 Home-page: https://github.com/rokam/midea-local
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,39 +13,42 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: ifaddr
 Requires-Dist: pycryptodome
 
 # Midea-local python lib
+
 [![Python build](https://github.com/rokam/midea-local/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/midea-local/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/midea-local/badges/tests.svg)
 [![Python coverage](https://raw.githubusercontent.com/rokam/midea-local/badges/coverage.svg)](https://app.codecov.io/github/rokam/midea-local)
 ![Python fake8](https://raw.githubusercontent.com/rokam/midea-local/badges/flake8.svg)
 
 Control your Midea M-Smart appliances via local area network.
 
-This library is part of https://github.com/georgezhao2010/midea_ac_lan code. It was separated to segregate responsabilities.
+This library is part of https://github.com/georgezhao2010/midea_ac_lan code. It was separated to segregate responsibilities.
 
 ⭐If this component is helpful for you, please star it, it encourages me a lot.
 
 ## Getting started
 
 ### Finding your device
+
 ```python
 from midealocal.discover import discover
 # Without knowing the ip address
 discover()
 # If you know the ip address
 discover(ip_address="203.0.113.11")
-# The device type is in hexadecimal and in midealocal/devices/TYPE
+# The device type is in hexadecimal as in midealocal/devices/TYPE
 type_code = hex(list(discover().values())[0]['type'])[2:]
 ```
 
 ### Getting data from device
+
 ```python
 from midealocal.discover import discover
 from midealocal.devices import device_selector
 
 token = '...'
 key = '...'
 
@@ -64,15 +67,14 @@
   model=d['model'],
   subtype=0,
   customize="",
 )
 
 # Connect and authenticate
 ac.connect()
-ac.authenticate()
 
 # Getting the attributes
 print(ac.attributes)
 # Setting the temperature
 ac.set_target_temperature(23.0, None)
 # Setting the swing
 ac.set_swing(False, False)
```

### Comparing `midea_local-1.0.3/README.md` & `midea_local-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # Midea-local python lib
+
 [![Python build](https://github.com/rokam/midea-local/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/midea-local/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/midea-local/badges/tests.svg)
 [![Python coverage](https://raw.githubusercontent.com/rokam/midea-local/badges/coverage.svg)](https://app.codecov.io/github/rokam/midea-local)
 ![Python fake8](https://raw.githubusercontent.com/rokam/midea-local/badges/flake8.svg)
 
 Control your Midea M-Smart appliances via local area network.
 
-This library is part of https://github.com/georgezhao2010/midea_ac_lan code. It was separated to segregate responsabilities.
+This library is part of https://github.com/georgezhao2010/midea_ac_lan code. It was separated to segregate responsibilities.
 
 ⭐If this component is helpful for you, please star it, it encourages me a lot.
 
 ## Getting started
 
 ### Finding your device
+
 ```python
 from midealocal.discover import discover
 # Without knowing the ip address
 discover()
 # If you know the ip address
 discover(ip_address="203.0.113.11")
-# The device type is in hexadecimal and in midealocal/devices/TYPE
+# The device type is in hexadecimal as in midealocal/devices/TYPE
 type_code = hex(list(discover().values())[0]['type'])[2:]
 ```
 
 ### Getting data from device
+
 ```python
 from midealocal.discover import discover
 from midealocal.devices import device_selector
 
 token = '...'
 key = '...'
 
@@ -46,15 +49,14 @@
   model=d['model'],
   subtype=0,
   customize="",
 )
 
 # Connect and authenticate
 ac.connect()
-ac.authenticate()
 
 # Getting the attributes
 print(ac.attributes)
 # Setting the temperature
 ac.set_target_temperature(23.0, None)
 # Setting the swing
 ac.set_swing(False, False)
```

### Comparing `midea_local-1.0.3/midea_local.egg-info/PKG-INFO` & `midea_local-1.0.4/midea_local.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midea-local
-Version: 1.0.3
+Version: 1.0.4
 Summary: Control your Midea M-Smart appliances via local area network
 Home-page: https://github.com/rokam/midea-local
 Author: rokam
 Author-email: lucas@mindello.com.br
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,39 +13,42 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: ifaddr
 Requires-Dist: pycryptodome
 
 # Midea-local python lib
+
 [![Python build](https://github.com/rokam/midea-local/actions/workflows/python-build.yml/badge.svg)](https://github.com/rokam/midea-local/actions/workflows/python-build.yml)
 ![Python tests](https://raw.githubusercontent.com/rokam/midea-local/badges/tests.svg)
 [![Python coverage](https://raw.githubusercontent.com/rokam/midea-local/badges/coverage.svg)](https://app.codecov.io/github/rokam/midea-local)
 ![Python fake8](https://raw.githubusercontent.com/rokam/midea-local/badges/flake8.svg)
 
 Control your Midea M-Smart appliances via local area network.
 
-This library is part of https://github.com/georgezhao2010/midea_ac_lan code. It was separated to segregate responsabilities.
+This library is part of https://github.com/georgezhao2010/midea_ac_lan code. It was separated to segregate responsibilities.
 
 ⭐If this component is helpful for you, please star it, it encourages me a lot.
 
 ## Getting started
 
 ### Finding your device
+
 ```python
 from midealocal.discover import discover
 # Without knowing the ip address
 discover()
 # If you know the ip address
 discover(ip_address="203.0.113.11")
-# The device type is in hexadecimal and in midealocal/devices/TYPE
+# The device type is in hexadecimal as in midealocal/devices/TYPE
 type_code = hex(list(discover().values())[0]['type'])[2:]
 ```
 
 ### Getting data from device
+
 ```python
 from midealocal.discover import discover
 from midealocal.devices import device_selector
 
 token = '...'
 key = '...'
 
@@ -64,15 +67,14 @@
   model=d['model'],
   subtype=0,
   customize="",
 )
 
 # Connect and authenticate
 ac.connect()
-ac.authenticate()
 
 # Getting the attributes
 print(ac.attributes)
 # Setting the temperature
 ac.set_target_temperature(23.0, None)
 # Setting the swing
 ac.set_swing(False, False)
```

### Comparing `midea_local-1.0.3/midea_local.egg-info/SOURCES.txt` & `midea_local-1.0.4/midea_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.3/midealocal/backports/enum.py` & `midea_local-1.0.4/midealocal/backports/enum.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,33 @@
 _StrEnumSelfT = TypeVar("_StrEnumSelfT", bound="StrEnum")
 
 
 class StrEnum(str, Enum):
     """Partial backport of Python 3.11's StrEnum for our basic use cases."""
 
     def __new__(
-        cls: type[_StrEnumSelfT], value: str, *args: Any, **kwargs: Any
+        cls: type[_StrEnumSelfT],
+        value: str,
+        *args: Any,
+        **kwargs: Any,
     ) -> _StrEnumSelfT:
         """Create a new StrEnum instance."""
         if not isinstance(value, str):
             raise TypeError(f"{value!r} is not a string")
         return super().__new__(cls, value, *args, **kwargs)
 
     def __str__(self) -> str:
         """Return self.value."""
         return str(self.value)
 
     @staticmethod
     def _generate_next_value_(
-        name: str, start: int, count: int, last_values: list[Any]
+        name: str,
+        start: int,
+        count: int,
+        last_values: list[Any],
     ) -> Any:
-        """
-        Make `auto()` explicitly unsupported.
+        """Make `auto()` explicitly unsupported.
         We may revisit this when it's very clear that Python 3.11's
         `StrEnum.auto()` behavior will no longer change.
         """
         raise TypeError("auto() is not supported by this implementation")
```

### Comparing `midea_local-1.0.3/midealocal/cloud.py` & `midea_local-1.0.4/midealocal/cloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,105 +1,113 @@
-import logging
-import time
+import base64
 import datetime
 import json
-import base64
+import logging
+import time
+from secrets import token_hex
 from threading import Lock
+from typing import Any, cast
+
 from aiohttp import ClientSession
-from secrets import token_hex
+
 from .security import (
     CloudSecurity,
     MeijuCloudSecurity,
-    MSmartCloudSecurity,
     MideaAirSecurity,
+    MSmartCloudSecurity,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 clouds = {
     "美的美居": {
         "class_name": "MeijuCloud",
         "app_id": "900",
         "app_key": "46579c15",
         "login_key": "ad0ee21d48a64bf49f4fb583ab76e799",
         "iot_key": bytes.fromhex(
-            format(9795516279659324117647275084689641883661667, "x")
+            format(9795516279659324117647275084689641883661667, "x"),
         ).decode(),
         "hmac_key": bytes.fromhex(
-            format(117390035944627627450677220413733956185864939010425, "x")
+            format(117390035944627627450677220413733956185864939010425, "x"),
         ).decode(),
         "api_url": "https://mp-prod.smartmidea.net/mas/v5/app/proxy?alias=",
     },
     "MSmartHome": {
         "class_name": "MSmartHomeCloud",
         "app_id": "1010",
         "app_key": "ac21b9f9cbfe4ca5a88562ef25e2b768",
         "iot_key": bytes.fromhex(format(7882822598523843940, "x")).decode(),
         "hmac_key": bytes.fromhex(
-            format(117390035944627627450677220413733956185864939010425, "x")
+            format(117390035944627627450677220413733956185864939010425, "x"),
         ).decode(),
         "api_url": "https://mp-prod.appsmb.com/mas/v5/app/proxy?alias=",
     },
     "Midea Air": {
         "class_name": "MideaAirCloud",
         "app_id": "1117",
         "app_key": "ff0cf6f5f0c3471de36341cab3f7a9af",
-        "api_url": "https://mapp.appsmb.com",
+        "api_url": "https://mapp.appsmb.com",  # codespell:ignore
     },
     "NetHome Plus": {
         "class_name": "MideaAirCloud",
         "app_id": "1017",
         "app_key": "3742e9e5842d4ad59c2db887e12449f9",
-        "api_url": "https://mapp.appsmb.com",
+        "api_url": "https://mapp.appsmb.com",  # codespell:ignore
     },
     "Ariston Clima": {
         "class_name": "MideaAirCloud",
         "app_id": "1005",
         "app_key": "434a209a5ce141c3b726de067835d7f0",
-        "api_url": "https://mapp.appsmb.com",
+        "api_url": "https://mapp.appsmb.com",  # codespell:ignore
     },
 }
 
 default_keys = {
     99: {
         "token": "ee755a84a115703768bcc7c6c13d3d629aa416f1e2fd798beb9f78cbb1381d09"
         "1cc245d7b063aad2a900e5b498fbd936c811f5d504b2e656d4f33b3bbc6d1da3",
         "key": "ed37bd31558a4b039aaf4e7a7a59aa7a75fd9101682045f69baf45d28380ae5c",
-    }
+    },
 }
 
 
 class MideaCloud:
     def __init__(
         self,
         session: ClientSession,
         security: CloudSecurity,
         app_id: str,
         app_key: str,
         account: str,
         password: str,
         api_url: str,
-    ):
+    ) -> None:
         self._device_id = CloudSecurity.get_deviceid(account)
         self._session = session
         self._security = security
         self._api_lock = Lock()
         self._app_id = app_id
         self._app_key = app_key
         self._account = account
         self._password = password
         self._api_url = api_url
-        self._access_token = None
-        self._uid = None
-        self._login_id = None
+        self._access_token: str | None = None
+        self._uid: str | None = None
+        self._login_id = ""
 
-    def _make_general_data(self):
+    def _make_general_data(self) -> dict[Any, Any]:
         return {}
 
-    async def _api_request(self, endpoint: str, data: dict, header=None) -> dict | None:
+    async def _api_request(
+        self,
+        endpoint: str,
+        data: dict[str, Any],
+        header: dict[str, Any] | None = None,
+    ) -> dict | None:
         header = header or {}
         if not data.get("reqId"):
             data.update({"reqId": token_hex(16)})
         if not data.get("stamp"):
             data.update({"stamp": datetime.datetime.now().strftime("%Y%m%d%H%M%S")})
         random = str(int(time.time()))
         url = self._api_url + endpoint
@@ -107,91 +115,105 @@
         sign = self._security.sign("", dump_data, random)
         header.update(
             {
                 "content-type": "application/json; charset=utf-8",
                 "secretVersion": "1",
                 "sign": sign,
                 "random": random,
-            }
+            },
         )
         if self._uid is not None:
             header.update({"uid": self._uid})
         if self._access_token is not None:
             header.update({"accessToken": self._access_token})
         response: dict = {"code": -1}
-        for i in range(0, 3):
+        for i in range(3):
             try:
                 with self._api_lock:
                     r = await self._session.request(
-                        "POST", url, headers=header, data=dump_data, timeout=10
+                        "POST",
+                        url,
+                        headers=header,
+                        data=dump_data,
+                        timeout=10,
                     )
                     raw = await r.read()
                     _LOGGER.debug(
-                        f"Midea cloud API url: {url}, data: {data}, response: {raw}"
+                        "Midea cloud API url: %s, data: %s, response: %s",
+                        url,
+                        data,
+                        raw,
                     )
                     response = json.loads(raw)
                     break
             except Exception as e:
-                _LOGGER.warning(f"Midea cloud API error, url: {url}, error: {repr(e)}")
+                _LOGGER.warning(
+                    "Midea cloud API error, url: %s, error: %s", url, repr(e)
+                )
         if int(response["code"]) == 0 and "data" in response:
-            return response["data"]
+            return cast(dict, response["data"])
         return None
 
     async def _get_login_id(self) -> str | None:
         data = self._make_general_data()
         data.update({"loginAccount": f"{self._account}"})
         if response := await self._api_request(
-            endpoint="/v1/user/login/id/get", data=data
+            endpoint="/v1/user/login/id/get",
+            data=data,
         ):
             return response.get("loginId")
         return None
 
     async def login(self) -> bool:
-        raise NotImplementedError()
+        raise NotImplementedError
 
-    async def get_keys(self, appliance_id: int):
+    async def get_keys(self, appliance_id: int) -> dict[int, dict[str, Any]]:
         result = {}
         for method in [1, 2]:
             udp_id = self._security.get_udp_id(appliance_id, method)
             data = self._make_general_data()
             data.update({"udpid": udp_id})
             response = await self._api_request(
-                endpoint="/v1/iot/secure/getToken", data=data
+                endpoint="/v1/iot/secure/getToken",
+                data=data,
             )
             if response and "tokenlist" in response:
                 for token in response["tokenlist"]:
                     if token["udpId"] == udp_id:
                         result[method] = {
                             "token": token["token"].lower(),
                             "key": token["key"].lower(),
                         }
         result.update(default_keys)
         return result
 
-    async def list_home(self) -> dict | None:
+    async def list_home(self) -> dict[int, Any] | None:
         return {1: "My home"}
 
-    async def list_appliances(self, home_id) -> dict | None:
-        raise NotImplementedError()
+    async def list_appliances(
+        self,
+        home_id: str | None,
+    ) -> dict[int, dict[str, Any]] | None:
+        raise NotImplementedError
 
-    async def get_device_info(self, device_id: int):
+    async def get_device_info(self, device_id: int) -> dict[str, Any] | None:
         if response := await self.list_appliances(home_id=None):
-            if device_id in response.keys():
-                return response[device_id]
+            if int(device_id) in response.keys():
+                return cast(dict, response[device_id])
         return None
 
     async def download_lua(
         self,
         path: str,
         device_type: int,
         sn: str,
         model_number: str | None,
         manufacturer_code: str = "0000",
-    ):
-        raise NotImplementedError()
+    ) -> str | None:
+        raise NotImplementedError
 
 
 class MeijuCloud(MideaCloud):
     def __init__(
         self,
         cloud_name: str,
         session: ClientSession,
@@ -217,57 +239,66 @@
             self._login_id = login_id
             stamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
             data = {
                 "iotData": {
                     "clientType": 1,
                     "deviceId": self._device_id,
                     "iampwd": self._security.encrypt_iam_password(
-                        self._login_id, self._password
+                        self._login_id,
+                        self._password,
                     ),
                     "iotAppId": self._app_id,
                     "loginAccount": self._account,
                     "password": self._security.encrypt_password(
-                        self._login_id, self._password
+                        self._login_id,
+                        self._password,
                     ),
                     "reqId": token_hex(16),
                     "stamp": stamp,
                 },
                 "data": {
                     "appKey": self._app_key,
                     "deviceId": self._device_id,
                     "platform": 2,
                 },
                 "timestamp": stamp,
                 "stamp": stamp,
             }
             if response := await self._api_request(
-                endpoint="/mj/user/login", data=data
+                endpoint="/mj/user/login",
+                data=data,
             ):
                 self._access_token = response["mdata"]["accessToken"]
                 self._security.set_aes_keys(
-                    self._security.aes_decrypt_with_fixed_key(response["key"]), None
+                    self._security.aes_decrypt_with_fixed_key(response["key"]),
+                    b"0",
                 )
 
                 return True
         return False
 
-    async def list_home(self):
+    async def list_home(self) -> dict[int, Any] | None:
         if response := await self._api_request(
-            endpoint="/v1/homegroup/list/get", data={}
+            endpoint="/v1/homegroup/list/get",
+            data={},
         ):
             homes = {}
             for home in response["homeList"]:
                 homes.update({int(home["homegroupId"]): home["name"]})
             return homes
         return None
 
-    async def list_appliances(self, home_id) -> dict | None:
+    async def list_appliances(
+        self,
+        home_id: str | None,
+    ) -> dict[int, dict[str, Any]] | None:
         data = {"homegroupId": home_id}
         if response := await self._api_request(
-            endpoint="/v1/appliance/home/list/get", data=data
+            endpoint="/v1/appliance/home/list/get",
+            data=data,
         ):
             appliances = {}
             for home in response.get("homeList") or []:
                 for room in home.get("roomList") or []:
                     for appliance in room.get("applianceList"):
                         try:
                             model_number = int(appliance.get("modelNumber", 0))
@@ -280,81 +311,79 @@
                                 self._security.aes_decrypt(appliance.get("sn"))
                                 if appliance.get("sn")
                                 else ""
                             ),
                             "sn8": appliance.get("sn8", "00000000"),
                             "model_number": model_number,
                             "manufacturer_code": appliance.get(
-                                "enterpriseCode", "0000"
+                                "enterpriseCode",
+                                "0000",
                             ),
                             "model": appliance.get("productModel"),
                             "online": appliance.get("onlineStatus") == "1",
                         }
-                        if (
-                            device_info.get("sn8") is None
-                            or len(device_info.get("sn8")) == 0
-                        ):
+                        sn8 = device_info.get("sn8")
+                        if not sn8 or len(sn8) == 0:
                             device_info["sn8"] = "00000000"
-                        if (
-                            device_info.get("model") is None
-                            or len(device_info.get("model")) == 0
-                        ):
+                        model = device_info.get("model")
+                        if not model or len(model) == 0:
                             device_info["model"] = device_info["sn8"]
                         appliances[int(appliance["applianceCode"])] = device_info
             return appliances
         return None
 
-    async def get_device_info(self, device_id: int):
+    async def get_device_info(self, device_id: int) -> dict[str, Any] | None:
         data = {"applianceCode": device_id}
         if response := await self._api_request(
-            endpoint="/v1/appliance/info/get", data=data
+            endpoint="/v1/appliance/info/get",
+            data=data,
         ):
             try:
                 model_number = int(response.get("modelNumber", 0))
-            except ValueError:
+            except (ValueError, TypeError):
                 model_number = 0
+            model_type = response.get("type")
             device_info = {
                 "name": response.get("name"),
-                "type": int(response.get("type"), 16),
-                "sn": (
-                    self._security.aes_decrypt(response.get("sn"))
-                    if response.get("sn")
-                    else ""
-                ),
+                "type": int(model_type, 16) if model_type else 0,
+                "sn": (self._security.aes_decrypt(response.get("sn") or "")),
                 "sn8": response.get("sn8", "00000000"),
                 "model_number": model_number,
                 "manufacturer_code": response.get("enterpriseCode", "0000"),
                 "model": response.get("productModel"),
                 "online": response.get("onlineStatus") == "1",
             }
-            if device_info.get("sn8") is None or len(device_info.get("sn8")) == 0:
+            sn8 = device_info.get("sn8")
+            if sn8 is None or len(sn8) == 0:
                 device_info["sn8"] = "00000000"
-            if device_info.get("model") is None or len(device_info.get("model")) == 0:
+            model = device_info.get("model")
+            if model is None or len(model) == 0:
                 device_info["model"] = device_info["sn8"]
             return device_info
         return None
 
     async def download_lua(
         self,
         path: str,
         device_type: int,
         sn: str,
         model_number: str | None,
         manufacturer_code: str = "0000",
-    ):
+    ) -> str | None:
         data = {
             "applianceSn": sn,
             "applianceType": "0x%02X" % device_type,
             "applianceMFCode": manufacturer_code,
             "version": "0",
             "iotAppId": self._app_id,
         }
         fnm = None
         if response := await self._api_request(
-            endpoint="/v1/appliance/protocol/lua/luaGet", data=data
+            endpoint="/v1/appliance/protocol/lua/luaGet",
+            data=data,
         ):
             res = await self._session.get(response["url"])
             if res.status == 200:
                 lua = await res.text()
                 if lua:
                     stream = (
                         'local bit = require "bit"\n'
@@ -385,91 +414,105 @@
             app_id=clouds[cloud_name]["app_id"],
             app_key=clouds[cloud_name]["app_key"],
             account=account,
             password=password,
             api_url=clouds[cloud_name]["api_url"],
         )
         self._auth_base = base64.b64encode(
-            f"{self._app_key}:{clouds['MSmartHome']['iot_key']}".encode("ascii")
+            f"{self._app_key}:{clouds['MSmartHome']['iot_key']}".encode("ascii"),
         ).decode("ascii")
 
-    def _make_general_data(self):
+    def _make_general_data(self) -> dict[str, Any]:
         return {
             # "appVersion": self.APP_VERSION,
             "src": self._app_id,
             "format": "2",
             "stamp": datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
             "platformId": "1",
             "deviceId": self._device_id,
             "reqId": token_hex(16),
             "uid": self._uid,
             "clientType": "1",
             "appId": self._app_id,
         }
 
-    async def _api_request(self, endpoint: str, data: dict, header=None) -> dict | None:
+    async def _api_request(
+        self,
+        endpoint: str,
+        data: dict[str, Any],
+        header: dict[str, Any] | None = None,
+    ) -> dict[str, Any] | None:
         header = header or {}
         header.update(
-            {"x-recipe-app": self._app_id, "authorization": f"Basic {self._auth_base}"}
+            {"x-recipe-app": self._app_id, "authorization": f"Basic {self._auth_base}"},
         )
 
         return await super()._api_request(endpoint, data, header)
 
-    async def _re_route(self):
+    async def _re_route(self) -> None:
         data = self._make_general_data()
         data.update({"userType": "0", "userName": f"{self._account}"})
         if response := await self._api_request(
-            endpoint="/v1/multicloud/platform/user/route", data=data
+            endpoint="/v1/multicloud/platform/user/route",
+            data=data,
         ):
             if api_url := response.get("masUrl"):
                 self._api_url = api_url
 
     async def login(self) -> bool:
         await self._re_route()
         if login_id := await self._get_login_id():
             self._login_id = login_id
             iot_data = self._make_general_data()
             iot_data.pop("uid")
             stamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
             iot_data.update(
                 {
                     "iampwd": self._security.encrypt_iam_password(
-                        self._login_id, self._password
+                        self._login_id,
+                        self._password,
                     ),
                     "loginAccount": self._account,
                     "password": self._security.encrypt_password(
-                        self._login_id, self._password
+                        self._login_id,
+                        self._password,
                     ),
                     "stamp": stamp,
-                }
+                },
             )
             data = {
                 "iotData": iot_data,
                 "data": {
                     "appKey": self._app_key,
                     "deviceId": self._device_id,
                     "platform": "2",
                 },
                 "stamp": stamp,
             }
             if response := await self._api_request(
-                endpoint="/mj/user/login", data=data
+                endpoint="/mj/user/login",
+                data=data,
             ):
                 self._uid = response["uid"]
                 self._access_token = response["mdata"]["accessToken"]
                 self._security.set_aes_keys(
-                    response["accessToken"], response["randomData"]
+                    response["accessToken"],
+                    response["randomData"],
                 )
                 return True
         return False
 
-    async def list_appliances(self, home_id) -> dict | None:
+    async def list_appliances(
+        self,
+        home_id: str | None,
+    ) -> dict[int, dict[str, Any]] | None:
         data = self._make_general_data()
         if response := await self._api_request(
-            endpoint="/v1/appliance/user/list/get", data=data
+            endpoint="/v1/appliance/user/list/get",
+            data=data,
         ):
             appliances = {}
             for appliance in response["list"]:
                 try:
                     model_number = int(appliance.get("modelNumber", 0))
                 except ValueError:
                     model_number = 0
@@ -483,48 +526,50 @@
                     ),
                     "sn8": "",
                     "model_number": model_number,
                     "manufacturer_code": appliance.get("enterpriseCode", "0000"),
                     "model": "",
                     "online": appliance.get("onlineStatus") == "1",
                 }
+                serial_num = device_info.get("sn")
                 device_info["sn8"] = (
-                    device_info.get("sn")[9:17] if len(device_info["sn"]) > 17 else ""
+                    serial_num[9:17] if (serial_num and len(serial_num) > 17) else ""
                 )
                 device_info["model"] = device_info.get("sn8")
                 appliances[int(appliance["id"])] = device_info
             return appliances
         return None
 
     async def download_lua(
         self,
         path: str,
         device_type: int,
         sn: str,
         model_number: str | None,
         manufacturer_code: str = "0000",
-    ):
+    ) -> str | None:
         data = {
             "clientType": "1",
             "appId": self._app_id,
             "format": "2",
             "deviceId": self._device_id,
             "iotAppId": self._app_id,
             "applianceMFCode": manufacturer_code,
             "applianceType": "0x%02X" % device_type,
             "modelNumber": model_number,
             "applianceSn": self._security.aes_encrypt_with_fixed_key(
-                sn.encode("ascii")
+                sn.encode("ascii"),
             ).hex(),
             "version": "0",
             "encryptedType ": "2",
         }
         fnm = None
         if response := await self._api_request(
-            endpoint="/v2/luaEncryption/luaGet", data=data
+            endpoint="/v2/luaEncryption/luaGet",
+            data=data,
         ):
             res = await self._session.get(response["url"])
             if res.status == 200:
                 lua = await res.text()
                 if lua:
                     stream = (
                         'local bit = require "bit"\n'
@@ -550,88 +595,108 @@
             security=MideaAirSecurity(login_key=clouds[cloud_name]["app_key"]),
             app_id=clouds[cloud_name]["app_id"],
             app_key=clouds[cloud_name]["app_key"],
             account=account,
             password=password,
             api_url=clouds[cloud_name]["api_url"],
         )
-        self._session_id = None
+        self._session_id: str | None = None
 
-    def _make_general_data(self):
+    def _make_general_data(self) -> dict[str, Any]:
         data = {
             "src": self._app_id,
             "format": "2",
             "stamp": datetime.datetime.now().strftime("%Y%m%d%H%M%S"),
             "deviceId": self._device_id,
             "reqId": token_hex(16),
             "clientType": "1",
             "appId": self._app_id,
         }
         if self._session_id is not None:
             data.update({"sessionId": self._session_id})
         return data
 
-    async def _api_request(self, endpoint: str, data: dict, header=None) -> dict | None:
+    async def _api_request(
+        self,
+        endpoint: str,
+        data: dict[str, Any],
+        header: dict[str, Any] | None = None,
+    ) -> dict[str, Any] | None:
         header = header or {}
         if not data.get("reqId"):
             data.update({"reqId": token_hex(16)})
         if not data.get("stamp"):
             data.update({"stamp": datetime.datetime.now().strftime("%Y%m%d%H%M%S")})
         url = self._api_url + endpoint
 
         sign = self._security.sign(url, data, "")
         data.update({"sign": sign})
         if self._uid is not None:
             header.update({"uid": self._uid})
         if self._access_token is not None:
             header.update({"accessToken": self._access_token})
         response: dict = {"code": -1}
-        for i in range(0, 3):
+        for i in range(3):
             try:
                 with self._api_lock:
                     r = await self._session.request(
-                        "POST", url, headers=header, data=data, timeout=10
+                        "POST",
+                        url,
+                        headers=header,
+                        data=data,
+                        timeout=10,
                     )
                     raw = await r.read()
                     _LOGGER.debug(
-                        f"Midea cloud API url: {url}, data: {data}, response: {raw}"
+                        "Midea cloud API url: %s, data: %s, response: %s",
+                        url,
+                        data,
+                        raw,
                     )
                     response = json.loads(raw)
                     break
             except Exception as e:
-                _LOGGER.warning(f"Midea cloud API error, url: {url}, error: {repr(e)}")
+                _LOGGER.warning(
+                    "Midea cloud API error, url: %s, error: %s", url, repr(e)
+                )
         if int(response["errorCode"]) == 0 and "result" in response:
-            return response["result"]
+            return cast(dict[str, Any], response["result"])
         return None
 
     async def login(self) -> bool:
         if login_id := await self._get_login_id():
             self._login_id = login_id
             data = self._make_general_data()
             data.update(
                 {
                     "loginAccount": self._account,
                     "password": self._security.encrypt_password(
-                        self._login_id, self._password
+                        self._login_id,
+                        self._password,
                     ),
-                }
+                },
             )
             if response := await self._api_request(
-                endpoint="/v1/user/login", data=data
+                endpoint="/v1/user/login",
+                data=data,
             ):
                 self._access_token = response["accessToken"]
                 self._uid = response["userId"]
                 self._session_id = response["sessionId"]
                 return True
         return False
 
-    async def list_appliances(self, home_id) -> dict | None:
+    async def list_appliances(
+        self,
+        home_id: str | None,
+    ) -> dict[int, dict[str, Any]] | None:
         data = self._make_general_data()
         if response := await self._api_request(
-            endpoint="/v1/appliance/user/list/get", data=data
+            endpoint="/v1/appliance/user/list/get",
+            data=data,
         ):
             appliances = {}
             for appliance in response["list"]:
                 try:
                     model_number = int(appliance.get("modelNumber", 0))
                 except ValueError:
                     model_number = 0
@@ -641,25 +706,32 @@
                     "sn": appliance.get("sn"),
                     "sn8": "",
                     "model_number": model_number,
                     "manufacturer_code": appliance.get("enterpriseCode", "0000"),
                     "model": "",
                     "online": appliance.get("onlineStatus") == "1",
                 }
+                serial_num = device_info.get("sn")
                 device_info["sn8"] = (
-                    device_info.get("sn")[9:17] if len(device_info["sn"]) > 17 else ""
+                    serial_num[9:17] if (serial_num and len(serial_num) > 17) else ""
                 )
                 device_info["model"] = device_info.get("sn8")
                 appliances[int(appliance["id"])] = device_info
             return appliances
         return None
 
 
 def get_midea_cloud(
-    cloud_name: str, session: ClientSession, account: str, password: str
+    cloud_name: str,
+    session: ClientSession,
+    account: str,
+    password: str,
 ) -> MideaCloud | None:
     cloud = None
-    if cloud_name in clouds.keys():
+    if cloud_name in clouds:
         cloud = globals()[clouds[cloud_name]["class_name"]](
-            cloud_name=cloud_name, session=session, account=account, password=password
+            cloud_name=cloud_name,
+            session=session,
+            account=account,
+            password=password,
         )
     return cloud
```

### Comparing `midea_local-1.0.3/midealocal/crc8.py` & `midea_local-1.0.4/midealocal/crc8.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,15 +257,12 @@
     0x89,
     0x6B,
     0x35,
 ]
 
 
 def calculate(data: bytearray) -> int:
-    """
-    Calculate CRC8 value of a bytearray.
-
-    """
+    """Calculate CRC8 value of a bytearray."""
     crc_value: int = 0
     for m in data:
         crc_value = crc8_854_table[crc_value ^ m]
     return crc_value
```

### Comparing `midea_local-1.0.3/midealocal/devices/__init__.py` & `midea_local-1.0.4/midealocal/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `midea_local-1.0.3/midealocal/devices/a1/__init__.py` & `midea_local-1.0.4/midealocal/devices/a1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageA1Response, MessageSet
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageA1Response, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -113,15 +116,15 @@
                     else:
                         self._attributes[status] = None
                 elif status == DeviceAttributes.water_level_set:
                     self._attributes[status] = str(value)
                 else:
                     self._attributes[status] = value
                 tank_full = self._attributes[DeviceAttributes.tank] >= int(
-                    self._attributes[DeviceAttributes.water_level_set]
+                    self._attributes[DeviceAttributes.water_level_set],
                 )
                 if (
                     self._attributes[DeviceAttributes.tank_full] is None
                     or self._attributes[DeviceAttributes.tank_full] != tank_full
                 ):
                     self._attributes[DeviceAttributes.tank_full] = tank_full
                     new_status[str(DeviceAttributes.tank_full)] = tank_full
@@ -140,23 +143,23 @@
         else:
             message.mode = 1
         message.fan_speed = (
             40
             if self._attributes[DeviceAttributes.fan_speed] is None
             else list(MideaA1Device._speeds.keys())[
                 list(MideaA1Device._speeds.values()).index(
-                    self._attributes[DeviceAttributes.fan_speed]
+                    self._attributes[DeviceAttributes.fan_speed],
                 )
             ]
         )
         message.target_humidity = self._attributes[DeviceAttributes.target_humidity]
         message.swing = self._attributes[DeviceAttributes.swing]
         message.anion = self._attributes[DeviceAttributes.anion]
         message.water_level_set = int(
-            self._attributes[DeviceAttributes.water_level_set]
+            self._attributes[DeviceAttributes.water_level_set],
         )
         return message
 
     def set_attribute(self, attr, value):
         if attr == DeviceAttributes.prompt_tone:
             self._attributes[DeviceAttributes.prompt_tone] = value
             self.update_all({DeviceAttributes.prompt_tone.value: value})
```

### Comparing `midea_local-1.0.3/midealocal/devices/a1/message.py` & `midea_local-1.0.4/midealocal/devices/a1/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import IntEnum
+
 from ...crc8 import calculate
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
     NewProtocolMessageBody,
 )
 
 
 class NewProtocolTags(IntEnum):
     light = 0x005B
 
@@ -66,15 +67,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class MessageNewProtocolQuery(MessageA1Base):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -145,15 +146,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class MessageNewProtocolSet(MessageA1Base):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -168,15 +169,15 @@
         payload = bytearray([0x00])
         if self.light is not None:
             pack_count += 1
             payload.extend(
                 NewProtocolMessageBody.pack(
                     param=NewProtocolTags.light,
                     value=bytearray([0x01 if self.light else 0x00]),
-                )
+                ),
             )
         payload[0] = pack_count
         return payload
 
 
 class A1GeneralMessageBody(MessageBody):
     def __init__(self, body):
```

### Comparing `midea_local-1.0.3/midealocal/devices/ac/__init__.py` & `midea_local-1.0.4/midealocal/devices/ac/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-import logging
 import json
+import logging
+import sys
+
 from .message import (
-    MessageQuery,
-    MessageToggleDisplay,
-    MessageNewProtocolQuery,
     MessageACResponse,
     MessageGeneralSet,
+    MessageNewProtocolQuery,
     MessageNewProtocolSet,
     MessagePowerQuery,
+    MessageQuery,
     MessageSubProtocolQuery,
     MessageSubProtocolSet,
+    MessageToggleDisplay,
 )
 
-try:
-    from enum import StrEnum
-except ImportError:
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     prompt_tone = "prompt_tone"
@@ -361,13 +364,13 @@
             try:
                 params = json.loads(customize)
                 if params and "temperature_step" in params:
                     self._temperature_step = params.get("temperature_step")
                 if params and "power_analysis_method" in params:
                     self._power_analysis_method = params.get("power_analysis_method")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"temperature_step": self._temperature_step})
 
 
 class MideaAppliance(MideaACDevice):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/ac/message.py` & `midea_local-1.0.4/midealocal/devices/ac/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from enum import IntEnum
+
+from ...crc8 import calculate
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
     NewProtocolMessageBody,
 )
-from ...crc8 import calculate
 
 BB_AC_MODES = [0, 3, 1, 2, 4, 5]
 
 
 class NewProtocolTags(IntEnum):
     indoor_humidity = 0x0015
     screen_display = 0x0017
@@ -74,15 +75,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class MessagePowerQuery(MessageACBase):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -130,15 +131,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class MessageNewProtocolQuery(MessageACBase):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -162,15 +163,17 @@
             _body.extend([param & 0xFF, param >> 8])
         return _body
 
 
 class MessageSubProtocol(MessageACBase):
     def __init__(self, protocol_version, message_type, subprotocol_query_type):
         super().__init__(
-            protocol_version=protocol_version, message_type=message_type, body_type=0xAA
+            protocol_version=protocol_version,
+            message_type=message_type,
+            body_type=0xAA,
         )
         self._subprotocol_query_type = subprotocol_query_type
 
     @property
     def _subprotocol_body(self):
         return bytes([])
 
@@ -189,15 +192,15 @@
                 6
                 + 2
                 + (len(_subprotocol_body) if _subprotocol_body is not None else 0),
                 0x00,
                 0xFF,
                 0xFF,
                 self._subprotocol_query_type,
-            ]
+            ],
         )
         if _subprotocol_body is not None:
             _body.extend(_subprotocol_body)
         return _body
 
 
 class MessageSubProtocolQuery(MessageSubProtocol):
@@ -282,15 +285,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x08,
-            ]
+            ],
         )
 
 
 class MessageGeneralSet(MessageACBase):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -371,15 +374,15 @@
                 0x00,
                 natural_wind,
                 0x00,
                 0x00,
                 0x00,
                 frost_protect,
                 comfort_mode,
-            ]
+            ],
         )
 
 
 class MessageNewProtocolSet(MessageACBase):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -399,39 +402,39 @@
         payload = bytearray([0x00])
         if self.breezeless is not None:
             pack_count += 1
             payload.extend(
                 NewProtocolMessageBody.pack(
                     param=NewProtocolTags.breezeless,
                     value=bytearray([0x01 if self.breezeless else 0x00]),
-                )
+                ),
             )
         if self.indirect_wind is not None:
             pack_count += 1
             payload.extend(
                 NewProtocolMessageBody.pack(
                     param=NewProtocolTags.indirect_wind,
                     value=bytearray([0x02 if self.indirect_wind else 0x01]),
-                )
+                ),
             )
         if self.prompt_tone is not None:
             pack_count += 1
             payload.extend(
                 NewProtocolMessageBody.pack(
                     param=NewProtocolTags.prompt_tone,
                     value=bytearray([0x01 if self.prompt_tone else 0x00]),
-                )
+                ),
             )
         if self.screen_display_alternate is not None:
             pack_count += 1
             payload.extend(
                 NewProtocolMessageBody.pack(
                     param=NewProtocolTags.screen_display,
                     value=bytearray([0x64 if self.screen_display_alternate else 0x00]),
-                )
+                ),
             )
         if self.fresh_air_1 is not None and len(self.fresh_air_1) == 2:
             pack_count += 1
             fresh_air_power = 2 if self.fresh_air_1[0] > 0 else 1
             fresh_air_fan_speed = self.fresh_air_1[1]
             payload.extend(
                 NewProtocolMessageBody.pack(
@@ -444,27 +447,27 @@
                             0x00,
                             0x00,
                             0x00,
                             0x00,
                             0x00,
                             0x00,
                             0x00,
-                        ]
+                        ],
                     ),
-                )
+                ),
             )
         if self.fresh_air_2 is not None and len(self.fresh_air_2) == 2:
             pack_count += 1
             fresh_air_power = 1 if self.fresh_air_2[0] > 0 else 0
             fresh_air_fan_speed = self.fresh_air_2[1]
             payload.extend(
                 NewProtocolMessageBody.pack(
                     param=NewProtocolTags.fresh_air_2,
                     value=bytearray([fresh_air_power, fresh_air_fan_speed, 0xFF]),
-                )
+                ),
             )
         payload[0] = pack_count
         return payload
 
 
 class XA0MessageBody(MessageBody):
     def __init__(self, body):
@@ -579,21 +582,32 @@
 
 
 class XC1MessageBody(MessageBody):
     def __init__(self, body, analysis_method=3):
         super().__init__(body)
         if body[3] == 0x44:
             self.total_energy_consumption = XC1MessageBody.parse_consumption(
-                analysis_method, body[4], body[5], body[6], body[7]
+                analysis_method,
+                body[4],
+                body[5],
+                body[6],
+                body[7],
             )
             self.current_energy_consumption = XC1MessageBody.parse_consumption(
-                analysis_method, body[12], body[13], body[14], body[15]
+                analysis_method,
+                body[12],
+                body[13],
+                body[14],
+                body[15],
             )
             self.realtime_power = XC1MessageBody.parse_power(
-                analysis_method, body[16], body[17], body[18]
+                analysis_method,
+                body[16],
+                body[17],
+                body[18],
             )
         elif body[3] == 0x40:
             pass
 
     @staticmethod
     def parse_value(byte):
         return (byte >> 4) * 10 + (byte & 0x0F)
@@ -601,15 +615,15 @@
     @staticmethod
     def parse_power(analysis_method, byte1, byte2, byte3):
         if analysis_method == 1:
             return (
                 float(
                     XC1MessageBody.parse_value(byte1) * 10000
                     + XC1MessageBody.parse_value(byte2) * 100
-                    + XC1MessageBody.parse_value(byte3)
+                    + XC1MessageBody.parse_value(byte3),
                 )
                 / 10
             )
         elif analysis_method == 2:
             return float((byte1 << 16) + (byte2 << 8) + byte3) / 10
         else:
             return float(byte1 * 10000 + byte2 * 100 + byte3) / 10
@@ -618,15 +632,15 @@
     def parse_consumption(analysis_method, byte1, byte2, byte3, byte4):
         if analysis_method == 1:
             return (
                 float(
                     XC1MessageBody.parse_value(byte1) * 1000000
                     + XC1MessageBody.parse_value(byte2) * 10000
                     + XC1MessageBody.parse_value(byte3) * 100
-                    + XC1MessageBody.parse_value(byte4)
+                    + XC1MessageBody.parse_value(byte4),
                 )
                 / 100
             )
         elif analysis_method == 2:
             return float((byte1 << 32) + (byte2 << 16) + (byte3 << 8) + byte4) / 10
         else:
             return float(byte1 * 1000000 + byte2 * 10000 + byte3 * 100 + byte4) / 100
```

### Comparing `midea_local-1.0.3/midealocal/devices/b0/__init__.py` & `midea_local-1.0.4/midealocal/devices/b0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery01, MessageB0Response
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageB0Response, MessageQuery01
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     door = "door"
```

### Comparing `midea_local-1.0.3/midealocal/devices/b0/message.py` & `midea_local-1.0.4/midealocal/devices/b0/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
 class MessageB0Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xB0,
             protocol_version=protocol_version,
```

### Comparing `midea_local-1.0.3/midealocal/devices/b1/__init__.py` & `midea_local-1.0.4/midealocal/devices/b1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageB1Response
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageB1Response, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     door = "door"
```

### Comparing `midea_local-1.0.3/midealocal/devices/b1/message.py` & `midea_local-1.0.4/midealocal/devices/b4/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
-class MessageB1Base(MessageRequest):
+class MessageB4Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
-            device_type=0xB1,
+            device_type=0xB4,
             protocol_version=protocol_version,
             message_type=message_type,
             body_type=body_type,
         )
 
     @property
     def _body(self):
         raise NotImplementedError
 
 
-class MessageQuery(MessageB1Base):
+class MessageQuery(MessageB4Base):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
             message_type=MessageType.query,
-            body_type=0x00,
+            body_type=0x01,
         )
 
     @property
     def _body(self):
         return bytearray([])
 
 
-class B1MessageBody(MessageBody):
+class B4MessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
-        self.door = (body[16] & 0x02) > 0
-        self.status = body[1]
         self.time_remaining = (
-            (0 if body[6] == 0xFF else body[6]) * 3600
-            + (0 if body[7] == 0xFF else body[7]) * 60
-            + (0 if body[8] == 0xFF else body[8])
+            (0 if body[22] == 0xFF else body[22]) * 3600
+            + (0 if body[23] == 0xFF else body[23]) * 60
+            + (0 if body[24] == 0xFF else body[24])
         )
-        self.current_temperature = body[19]
+        self.current_temperature = (body[25] << 8) + body[26]
+        if self.current_temperature == 0:
+            self.current_temperature = (body[27] << 8) + body[28]
+        self.status = body[31]
+        self.door = (body[32] & 0x02) > 0
         self.tank_ejected = (body[16] & 0x04) > 0
         self.water_shortage = (body[16] & 0x08) > 0
         self.water_change_reminder = (body[16] & 0x10) > 0
 
 
-class MessageB1Response(MessageResponse):
+class MessageB4Response(MessageResponse):
     def __init__(self, message):
         super().__init__(message)
-        if self.message_type in [MessageType.notify1, MessageType.query]:
-            self.set_body(B1MessageBody(super().body))
+        if self.message_type in [
+            MessageType.notify1,
+            MessageType.query,
+            MessageType.set,
+        ]:
+            if self.body_type == 0x01:
+                self.set_body(B4MessageBody(super().body))
         self.set_attr()
```

### Comparing `midea_local-1.0.3/midealocal/devices/b3/__init__.py` & `midea_local-1.0.4/midealocal/devices/b3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageB3Response
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageB3Response, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     top_compartment_status = "top_compartment_status"
```

### Comparing `midea_local-1.0.3/midealocal/devices/b3/message.py` & `midea_local-1.0.4/midealocal/devices/b3/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
 class MessageB3Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xB3,
             protocol_version=protocol_version,
@@ -170,12 +170,15 @@
         if (
             self.message_type == MessageType.query
             and self.body_type == 0x31
             or self.message_type == MessageType.notify1
             and self.body_type == 0x41
         ):
             self.set_body(B3MessageBody31(super().body))
-        elif self.message_type == MessageType.set and self.body_type == 0x21:
-            self.set_body(B3MessageBody21(super().body))
-        elif self.message_type == MessageType.set and self.body_type == 0x24:
+        elif (
+            self.message_type == MessageType.set
+            and self.body_type == 0x21
+            or self.message_type == MessageType.set
+            and self.body_type == 0x24
+        ):
             self.set_body(B3MessageBody21(super().body))
         self.set_attr()
```

### Comparing `midea_local-1.0.3/midealocal/devices/b4/__init__.py` & `midea_local-1.0.4/midealocal/devices/bf/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageB4Response
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageBFResponse, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     door = "door"
@@ -16,18 +19,18 @@
     time_remaining = "time_remaining"
     current_temperature = "current_temperature"
     tank_ejected = "tank_ejected"
     water_change_reminder = "water_change_reminder"
     water_shortage = "water_shortage"
 
 
-class MideaB4Device(MideaDevice):
+class MideaBFDevice(MideaDevice):
     _status = {
-        0x01: "Standby",
-        0x02: "Idle",
+        0x01: "PowerSave",
+        0x02: "Standby",
         0x03: "Working",
         0x04: "Finished",
         0x05: "Delay",
         0x06: "Paused",
     }
 
     def __init__(
@@ -42,54 +45,54 @@
         model: str,
         subtype: int,
         customize: str,
     ):
         super().__init__(
             name=name,
             device_id=device_id,
-            device_type=0xB4,
+            device_type=0xBF,
             ip_address=ip_address,
             port=port,
             token=token,
             key=key,
             protocol=protocol,
             model=model,
             subtype=subtype,
             attributes={
-                DeviceAttributes.door: False,
+                DeviceAttributes.door: None,
                 DeviceAttributes.status: None,
                 DeviceAttributes.time_remaining: None,
                 DeviceAttributes.current_temperature: None,
-                DeviceAttributes.tank_ejected: False,
-                DeviceAttributes.water_change_reminder: False,
-                DeviceAttributes.water_shortage: False,
+                DeviceAttributes.tank_ejected: None,
+                DeviceAttributes.water_change_reminder: None,
+                DeviceAttributes.water_shortage: None,
             },
         )
 
     def build_query(self):
         return [MessageQuery(self._protocol_version)]
 
     def process_message(self, msg):
-        message = MessageB4Response(msg)
+        message = MessageBFResponse(msg)
         _LOGGER.debug(f"[{self.device_id}] Received: {message}")
         new_status = {}
         for status in self._attributes.keys():
             if hasattr(message, str(status)):
                 value = getattr(message, str(status))
                 if status == DeviceAttributes.status:
-                    if value in MideaB4Device._status.keys():
+                    if value in MideaBFDevice._status.keys():
                         self._attributes[DeviceAttributes.status] = (
-                            MideaB4Device._status.get(value)
+                            MideaBFDevice._status.get(value)
                         )
                     else:
-                        self._attributes[DeviceAttributes.status] = None
+                        self._attributes[DeviceAttributes.status] = "Unknown"
                 else:
                     self._attributes[status] = value
                 new_status[str(status)] = self._attributes[status]
         return new_status
 
     def set_attribute(self, attr, value):
         pass
 
 
-class MideaAppliance(MideaB4Device):
+class MideaAppliance(MideaBFDevice):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/b4/message.py` & `midea_local-1.0.4/midealocal/devices/b1/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,52 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
-class MessageB4Base(MessageRequest):
+class MessageB1Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
-            device_type=0xB4,
+            device_type=0xB1,
             protocol_version=protocol_version,
             message_type=message_type,
             body_type=body_type,
         )
 
     @property
     def _body(self):
         raise NotImplementedError
 
 
-class MessageQuery(MessageB4Base):
+class MessageQuery(MessageB1Base):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
             message_type=MessageType.query,
-            body_type=0x01,
+            body_type=0x00,
         )
 
     @property
     def _body(self):
         return bytearray([])
 
 
-class B4MessageBody(MessageBody):
+class B1MessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
+        self.door = (body[16] & 0x02) > 0
+        self.status = body[1]
         self.time_remaining = (
-            (0 if body[22] == 0xFF else body[22]) * 3600
-            + (0 if body[23] == 0xFF else body[23]) * 60
-            + (0 if body[24] == 0xFF else body[24])
+            (0 if body[6] == 0xFF else body[6]) * 3600
+            + (0 if body[7] == 0xFF else body[7]) * 60
+            + (0 if body[8] == 0xFF else body[8])
         )
-        self.current_temperature = (body[25] << 8) + body[26]
-        if self.current_temperature == 0:
-            self.current_temperature = (body[27] << 8) + body[28]
-        self.status = body[31]
-        self.door = (body[32] & 0x02) > 0
+        self.current_temperature = body[19]
         self.tank_ejected = (body[16] & 0x04) > 0
         self.water_shortage = (body[16] & 0x08) > 0
         self.water_change_reminder = (body[16] & 0x10) > 0
 
 
-class MessageB4Response(MessageResponse):
+class MessageB1Response(MessageResponse):
     def __init__(self, message):
         super().__init__(message)
-        if self.message_type in [
-            MessageType.notify1,
-            MessageType.query,
-            MessageType.set,
-        ]:
-            if self.body_type == 0x01:
-                self.set_body(B4MessageBody(super().body))
+        if self.message_type in [MessageType.notify1, MessageType.query]:
+            self.set_body(B1MessageBody(super().body))
         self.set_attr()
```

### Comparing `midea_local-1.0.3/midealocal/devices/b6/__init__.py` & `midea_local-1.0.4/midealocal/devices/b6/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import logging
 import json
-from .message import MessageQuery, MessageB6Response, MessageSet
+import logging
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageB6Response, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -80,18 +83,18 @@
         new_status = {}
         for status in self._attributes.keys():
             if hasattr(message, str(status)):
                 value = getattr(message, str(status))
                 if status == DeviceAttributes.fan_level:
                     if value in self._speeds.keys():
                         self._attributes[DeviceAttributes.mode] = self._speeds.get(
-                            value
+                            value,
                         )
                         self._attributes[DeviceAttributes.fan_speed] = list(
-                            self._speeds.keys()
+                            self._speeds.keys(),
                         ).index(value)
                     else:
                         self._attributes[DeviceAttributes.mode] = None
                         self._attributes[DeviceAttributes.fan_speed] = 0
                     new_status[DeviceAttributes.mode.value] = self._attributes[
                         DeviceAttributes.mode
                     ]
@@ -154,15 +157,15 @@
                         speeds = {}
                         for k, v in params.get("speeds").items():
                             speeds[int(k)] = v
                         keys = sorted(speeds.keys())
                         for k in keys:
                             self._speeds[k] = speeds[k]
                     self.update_all(
-                        {"speeds": self._speeds, "default_speed": self._power_speed}
+                        {"speeds": self._speeds, "default_speed": self._power_speed},
                     )
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
 
 
 class MideaAppliance(MideaB6Device):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/b6/message.py` & `midea_local-1.0.4/midealocal/devices/b6/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageB6Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xB6,
@@ -80,15 +80,15 @@
             elif self.fan_level is not None:
                 if self.fan_level == 0:
                     value2 = 0x03
                 else:
                     value2 = 0x02
                     value3 = self.fan_level
             return bytearray(
-                [0x01, light, value2, value3, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
+                [0x01, light, value2, value3, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF],
             )
         else:
             value13 = 0xFF
             value14 = 0xFF
             value15 = 0xFF
             value16 = 0xFF
             if self.power is not None:
```

### Comparing `midea_local-1.0.3/midealocal/devices/bf/__init__.py` & `midea_local-1.0.4/midealocal/devices/b4/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageBFResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageB4Response, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     door = "door"
@@ -16,18 +19,18 @@
     time_remaining = "time_remaining"
     current_temperature = "current_temperature"
     tank_ejected = "tank_ejected"
     water_change_reminder = "water_change_reminder"
     water_shortage = "water_shortage"
 
 
-class MideaBFDevice(MideaDevice):
+class MideaB4Device(MideaDevice):
     _status = {
-        0x01: "PowerSave",
-        0x02: "Standby",
+        0x01: "Standby",
+        0x02: "Idle",
         0x03: "Working",
         0x04: "Finished",
         0x05: "Delay",
         0x06: "Paused",
     }
 
     def __init__(
@@ -42,54 +45,54 @@
         model: str,
         subtype: int,
         customize: str,
     ):
         super().__init__(
             name=name,
             device_id=device_id,
-            device_type=0xBF,
+            device_type=0xB4,
             ip_address=ip_address,
             port=port,
             token=token,
             key=key,
             protocol=protocol,
             model=model,
             subtype=subtype,
             attributes={
-                DeviceAttributes.door: None,
+                DeviceAttributes.door: False,
                 DeviceAttributes.status: None,
                 DeviceAttributes.time_remaining: None,
                 DeviceAttributes.current_temperature: None,
-                DeviceAttributes.tank_ejected: None,
-                DeviceAttributes.water_change_reminder: None,
-                DeviceAttributes.water_shortage: None,
+                DeviceAttributes.tank_ejected: False,
+                DeviceAttributes.water_change_reminder: False,
+                DeviceAttributes.water_shortage: False,
             },
         )
 
     def build_query(self):
         return [MessageQuery(self._protocol_version)]
 
     def process_message(self, msg):
-        message = MessageBFResponse(msg)
+        message = MessageB4Response(msg)
         _LOGGER.debug(f"[{self.device_id}] Received: {message}")
         new_status = {}
         for status in self._attributes.keys():
             if hasattr(message, str(status)):
                 value = getattr(message, str(status))
                 if status == DeviceAttributes.status:
-                    if value in MideaBFDevice._status.keys():
+                    if value in MideaB4Device._status.keys():
                         self._attributes[DeviceAttributes.status] = (
-                            MideaBFDevice._status.get(value)
+                            MideaB4Device._status.get(value)
                         )
                     else:
-                        self._attributes[DeviceAttributes.status] = "Unknown"
+                        self._attributes[DeviceAttributes.status] = None
                 else:
                     self._attributes[status] = value
                 new_status[str(status)] = self._attributes[status]
         return new_status
 
     def set_attribute(self, attr, value):
         pass
 
 
-class MideaAppliance(MideaBFDevice):
+class MideaAppliance(MideaB4Device):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/bf/message.py` & `midea_local-1.0.4/midealocal/devices/bf/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
 class MessageBFBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xBF,
             protocol_version=protocol_version,
```

### Comparing `midea_local-1.0.3/midealocal/devices/c2/__init__.py` & `midea_local-1.0.4/midealocal/devices/c2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import logging
 import json
-from .message import MessageQuery, MessageC2Response, MessageSet, MessagePower
+import logging
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageC2Response, MessagePower, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -129,23 +132,23 @@
                 if params and "max_dry_level" in params:
                     self._max_dry_level = params.get("max_dry_level")
                 if params and "max_water_temp_level" in params:
                     self._max_water_temp_level = params.get("max_water_temp_level")
                 if params and "max_seat_temp_level" in params:
                     self._max_seat_temp_level = params.get("max_seat_temp_level")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all(
                 {
                     "dry_level": {"max_dry_level": self._max_dry_level},
                     "water_temp_level": {
-                        "max_water_temp_level": self._max_water_temp_level
+                        "max_water_temp_level": self._max_water_temp_level,
                     },
                     "seat_temp_level": {
-                        "max_seat_temp_level": self._max_seat_temp_level
+                        "max_seat_temp_level": self._max_seat_temp_level,
                     },
-                }
+                },
             )
 
 
 class MideaAppliance(MideaC2Device):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/c2/message.py` & `midea_local-1.0.4/midealocal/devices/c2/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import IntEnum
+
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class C2MessageEnum(IntEnum):
     sensor_light = 0x01
     child_lock = 0x10
     foam_shield = 0x1F
```

### Comparing `midea_local-1.0.3/midealocal/devices/c3/__init__.py` & `midea_local-1.0.4/midealocal/devices/c3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import logging
+import sys
+
 from .message import (
-    MessageQuery,
-    MessageSetSilent,
-    MessageSetECO,
     MessageC3Response,
+    MessageQuery,
     MessageSet,
+    MessageSetECO,
+    MessageSetSilent,
 )
 
-try:
-    from enum import StrEnum
-except ImportError:
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     zone1_power = "zone1_power"
```

### Comparing `midea_local-1.0.3/midealocal/devices/c3/message.py` & `midea_local-1.0.4/midealocal/devices/c3/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageC3Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xC3,
@@ -73,15 +73,15 @@
                 zone1_power | zone2_power | dhw_power,
                 self.mode,
                 zone1_target_temp,
                 zone2_target_temp,
                 dhw_target_temp,
                 room_target_temp,
                 zone1_curve | zone2_curve | disinfect | fast_dhw,
-            ]
+            ],
         )
 
 
 class MessageSetSilent(MessageC3Base):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -93,15 +93,25 @@
 
     @property
     def _body(self):
         silent_mode = 0x01 if self.silent_mode else 0
         super_silent = 0x02 if self.super_silent else 0
 
         return bytearray(
-            [silent_mode | super_silent, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00]
+            [
+                silent_mode | super_silent,
+                0x00,
+                0x00,
+                0x00,
+                0x00,
+                0x00,
+                0x00,
+                0x00,
+                0x00,
+            ],
         )
 
 
 class MessageSetECO(MessageC3Base):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -169,15 +179,18 @@
 
         self.total_produced_energy = (
             (body[data_offset + 5] << 32)
             + (body[data_offset + 6] << 16)
             + (body[data_offset + 7] << 8)
             + (body[data_offset + 8])
         )
-        self.outdoor_temperature = int(body[data_offset + 9])
+        base_value = body[data_offset + 9]
+        self.outdoor_temperature = (
+            (base_value - 256) if base_value > 127 else base_value
+        )
 
 
 class MessageC3Response(MessageResponse):
     def __init__(self, message):
         super().__init__(message)
         if (
             self.message_type
```

### Comparing `midea_local-1.0.3/midealocal/devices/ca/__init__.py` & `midea_local-1.0.4/midealocal/devices/ca/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageCAResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageCAResponse, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     mode = "mode"
```

### Comparing `midea_local-1.0.3/midealocal/devices/ca/message.py` & `midea_local-1.0.4/midealocal/devices/ca/message.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageCABase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xCA,
```

### Comparing `midea_local-1.0.3/midealocal/devices/cc/__init__.py` & `midea_local-1.0.4/midealocal/devices/cc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageSet, MessageCCResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageCCResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -114,15 +117,15 @@
             if self._fan_speeds is None:
                 if self._attributes[DeviceAttributes.fan_speed_level]:
                     self._fan_speeds = MideaCCDevice._fan_speeds_3level
                 else:
                     self._fan_speeds = MideaCCDevice._fan_speeds_7level
             if fan_speed in self._fan_speeds.keys():
                 self._attributes[DeviceAttributes.fan_speed] = self._fan_speeds.get(
-                    fan_speed
+                    fan_speed,
                 )
             else:
                 self._attributes[DeviceAttributes.fan_speed] = None
             new_status[DeviceAttributes.fan_speed.value] = self._attributes[
                 DeviceAttributes.fan_speed
             ]
         aux_heating = (
@@ -141,15 +144,15 @@
         message.power = self._attributes[DeviceAttributes.power]
         message.mode = self._attributes[DeviceAttributes.mode]
         message.target_temperature = self._attributes[
             DeviceAttributes.target_temperature
         ]
         message.fan_speed = list(self._fan_speeds.keys())[
             list(self._fan_speeds.values()).index(
-                self._attributes[DeviceAttributes.fan_speed]
+                self._attributes[DeviceAttributes.fan_speed],
             )
         ]
         message.eco_mode = self._attributes[DeviceAttributes.eco_mode]
         message.sleep_mode = self._attributes[DeviceAttributes.sleep_mode]
         message.night_light = self._attributes[DeviceAttributes.night_light]
         message.aux_heat_status = self._attributes[DeviceAttributes.aux_heat_status]
         message.swing = self._attributes[DeviceAttributes.swing]
```

### Comparing `midea_local-1.0.3/midealocal/devices/cc/message.py` & `midea_local-1.0.4/midealocal/devices/cc/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageCCBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xCC,
@@ -101,15 +101,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class CCGeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = (body[1] & 0x80) > 0
```

### Comparing `midea_local-1.0.3/midealocal/devices/cd/__init__.py` & `midea_local-1.0.4/midealocal/devices/cd/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-import logging
 import json
-from .message import MessageQuery, MessageSet, MessageCDResponse
+import logging
+import sys
+from typing import Any
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageCDResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -60,15 +65,15 @@
                 DeviceAttributes.current_temperature: None,
                 DeviceAttributes.outdoor_temperature: None,
                 DeviceAttributes.condenser_temperature: None,
                 DeviceAttributes.compressor_temperature: None,
                 DeviceAttributes.compressor_status: None,
             },
         )
-        self._fields = {}
+        self._fields = dict[Any, Any]
         self._temperature_step = None
         self._default_temperature_step = 1
         self.set_customize(customize)
 
     @property
     def temperature_step(self):
         return self._temperature_step
@@ -81,15 +86,15 @@
         return [MessageQuery(self._protocol_version)]
 
     def process_message(self, msg):
         message = MessageCDResponse(msg)
         _LOGGER.debug(f"[{self.device_id}] Received: {message}")
         new_status = {}
         if hasattr(message, "fields"):
-            self._fields = getattr(message, "fields")
+            self._fields = message.fields
         for status in self._attributes.keys():
             if hasattr(message, str(status)):
                 value = getattr(message, str(status))
                 if status == DeviceAttributes.mode:
                     self._attributes[status] = MideaCDDevice._modes[value]
                 else:
                     self._attributes[status] = value
@@ -101,15 +106,15 @@
             DeviceAttributes.mode,
             DeviceAttributes.power,
             DeviceAttributes.target_temperature,
         ]:
             message = MessageSet(self._protocol_version)
             message.fields = self._fields
             message.mode = MideaCDDevice._modes.index(
-                self._attributes[DeviceAttributes.mode]
+                self._attributes[DeviceAttributes.mode],
             )
             message.power = self._attributes[DeviceAttributes.power]
             message.target_temperature = self._attributes[
                 DeviceAttributes.target_temperature
             ]
             if attr == DeviceAttributes.mode:
                 if value in MideaCDDevice._modes:
@@ -122,13 +127,13 @@
         self._temperature_step = self._default_temperature_step
         if customize and len(customize) > 0:
             try:
                 params = json.loads(customize)
                 if params and "temperature_step" in params:
                     self._temperature_step = params.get("temperature_step")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"temperature_step": self._temperature_step})
 
 
 class MideaAppliance(MideaCDDevice):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/cd/message.py` & `midea_local-1.0.4/midealocal/devices/cd/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageCDBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xCD,
@@ -61,15 +61,15 @@
                 power,
                 mode,
                 target_temperature,
                 self.read_field("trValue"),
                 self.read_field("openPTC"),
                 self.read_field("ptcTemp"),
                 0,  # self.read_field("byte8")
-            ]
+            ],
         )
 
 
 class CDGeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = (body[2] & 0x01) > 0
```

### Comparing `midea_local-1.0.3/midealocal/devices/ce/__init__.py` & `midea_local-1.0.4/midealocal/devices/ce/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import logging
 import json
-from .message import MessageQuery, MessageCEResponse, MessageSet
+import logging
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageCEResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -145,13 +148,13 @@
         self._speed_count = self._default_speed_count
         if customize and len(customize) > 0:
             try:
                 params = json.loads(customize)
                 if params and "speed_count" in params:
                     self._speed_count = params.get("speed_count")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"speed_count": self._speed_count})
 
 
 class MideaAppliance(MideaCEDevice):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/ce/message.py` & `midea_local-1.0.4/midealocal/devices/ce/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageFABase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xCE,
@@ -65,15 +65,15 @@
             [
                 power | 0x01,
                 self.fan_speed,
                 link_to_ac | sleep_mode | eco_mode | aux_heating | powerful_purify,
                 scheduled,
                 0x00,
                 child_lock,
-            ]
+            ],
         )
 
 
 class CEGeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = (body[1] & 0x80) > 0
```

### Comparing `midea_local-1.0.3/midealocal/devices/cf/__init__.py` & `midea_local-1.0.4/midealocal/devices/cf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageCFResponse, MessageSet
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageCFResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
```

### Comparing `midea_local-1.0.3/midealocal/devices/cf/message.py` & `midea_local-1.0.4/midealocal/devices/cf/message.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageCFBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xCF,
```

### Comparing `midea_local-1.0.3/midealocal/devices/da/__init__.py` & `midea_local-1.0.4/midealocal/devices/da/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessagePower, MessageStart, MessageDAResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageDAResponse, MessagePower, MessageQuery, MessageStart
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -111,15 +114,15 @@
             "7",
             "8",
             "Insufficient",
         ]
         softener = [
             "No",
             "Intelligent",
-            "Programed",
+            "Programed",  # codespell:ignore
             "3",
             "4",
             "5",
             "6",
             "7",
             "8",
             "Insufficient",
```

### Comparing `midea_local-1.0.3/midealocal/devices/da/message.py` & `midea_local-1.0.4/midealocal/devices/da/message.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageDABase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xDA,
```

### Comparing `midea_local-1.0.3/midealocal/devices/db/__init__.py` & `midea_local-1.0.4/midealocal/devices/db/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessagePower, MessageStart, MessageDBResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageDBResponse, MessagePower, MessageQuery, MessageStart
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
```

### Comparing `midea_local-1.0.3/midealocal/devices/db/message.py` & `midea_local-1.0.4/midealocal/devices/db/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageDBBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xDB,
@@ -64,15 +64,15 @@
                 0xFF,
                 0xFF,
                 0xFF,
                 0xFF,
                 0xFF,
                 0xFF,
                 0xFF,
-            ]
+            ],
         )
 
 
 class MessageStart(MessageDBBase):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -94,15 +94,15 @@
 class DBGeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = body[1] > 0
         self.start = True if body[2] in [2, 6] else False
         self.washing_data = body[3:16]
         self.progress = 0
-        for i in range(0, 7):
+        for i in range(7):
             if (body[16] & (1 << i)) > 0:
                 self.progress = i + 1
                 break
         if self.power:
             self.time_remaining = body[17] + (body[18] << 8)
         else:
             self.time_remaining = None
```

### Comparing `midea_local-1.0.3/midealocal/devices/dc/__init__.py` & `midea_local-1.0.4/midealocal/devices/dc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessagePower, MessageStart, MessageDCResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageDCResponse, MessagePower, MessageQuery, MessageStart
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
```

### Comparing `midea_local-1.0.3/midealocal/devices/dc/message.py` & `midea_local-1.0.4/midealocal/devices/dc/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageDCBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xDC,
@@ -70,15 +70,15 @@
 class DCGeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = body[1] > 0
         self.start = True if body[2] in [2, 6] else False
         self.washing_data = body[3:15]
         self.progress = 0
-        for i in range(0, 7):
+        for i in range(7):
             if (body[16] & (1 << i)) > 0:
                 self.progress = i + 1
                 break
         if self.power:
             self.time_remaining = body[17] + body[18] * 60
         else:
             self.time_remaining = None
```

### Comparing `midea_local-1.0.3/midealocal/devices/e1/__init__.py` & `midea_local-1.0.4/midealocal/devices/e1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import logging
+import sys
+
 from .message import (
-    MessageQuery,
+    MessageE1Response,
+    MessageLock,
     MessagePower,
+    MessageQuery,
     MessageStorage,
-    MessageLock,
-    MessageE1Response,
 )
 
-try:
-    from enum import StrEnum
-except ImportError:
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
```

### Comparing `midea_local-1.0.3/midealocal/devices/e1/message.py` & `midea_local-1.0.4/midealocal/devices/e1/message.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageE1Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xE1,
```

### Comparing `midea_local-1.0.3/midealocal/devices/e2/__init__.py` & `midea_local-1.0.4/midealocal/devices/e2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-import logging
 import json
+import logging
+import sys
+
 from .message import (
-    MessageQuery,
-    MessageSet,
     MessageE2Response,
-    MessagePower,
     MessageNewProtocolSet,
+    MessagePower,
+    MessageQuery,
+    MessageSet,
 )
 
-try:
-    from enum import StrEnum
-except ImportError:
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -127,13 +130,13 @@
         self._old_protocol = self._default_old_protocol
         if customize and len(customize) > 0:
             try:
                 params = json.loads(customize)
                 if params and "old_protocol" in params:
                     self._old_protocol = params.get("old_protocol")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"old_protocol": self._old_protocol})
 
 
 class MideaAppliance(MideaE2Device):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/e2/message.py` & `midea_local-1.0.4/midealocal/devices/e2/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageE2Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xE2,
@@ -115,15 +115,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class E2GeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = (body[2] & 0x01) > 0
```

### Comparing `midea_local-1.0.3/midealocal/devices/e3/__init__.py` & `midea_local-1.0.4/midealocal/devices/e3/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-import logging
 import json
+import logging
+import sys
+
 from .message import (
-    MessageQuery,
-    MessageSet,
+    MessageE3Response,
     MessageNewProtocolSet,
     MessagePower,
-    MessageE3Response,
+    MessageQuery,
+    MessageSet,
 )
 
-try:
-    from enum import StrEnum
-except ImportError:
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -116,25 +119,25 @@
                 message = MessagePower(self._protocol_version)
                 message.power = value
             elif self.subtype in self._old_subtypes:
                 message = self.make_message_set()
                 setattr(message, str(attr), value)
             else:
                 message = MessageNewProtocolSet(self._protocol_version)
-                setattr(message, "key", str(attr))
-                setattr(message, "value", value)
+                message.key = str(attr)
+                message.value = value
             self.build_send(message)
 
     def set_customize(self, customize):
         self._precision_halves = self._default_precision_halves
         if customize and len(customize) > 0:
             try:
                 params = json.loads(customize)
                 if params and "precision_halves" in params:
                     self._precision_halves = params.get("precision_halves")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"precision_halves": self._precision_halves})
 
 
 class MideaAppliance(MideaE3Device):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/e3/message.py` & `midea_local-1.0.4/midealocal/devices/e3/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
-
 NEW_PROTOCOL_PARAMS = {
     "zero_cold_water": 0x03,
     # "zero_cold_master": 0x12,
     "zero_cold_pulse": 0x04,
     "smart_volume": 0x07,
     "target_temperature": 0x08,
 }
@@ -98,15 +97,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class MessageNewProtocolSet(MessageE3Base):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -140,15 +139,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class E3GeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = (body[2] & 0x01) > 0
```

### Comparing `midea_local-1.0.3/midealocal/devices/e6/__init__.py` & `midea_local-1.0.4/midealocal/devices/e6/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageSet, MessageE6Response
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageE6Response, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     main_power = "main_power"
```

### Comparing `midea_local-1.0.3/midealocal/devices/e6/message.py` & `midea_local-1.0.4/midealocal/devices/e6/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageE6Base(MessageRequest):
     def __init__(self, protocol_version, message_type):
         super().__init__(
             device_type=0xE6,
@@ -23,26 +23,28 @@
     def _body(self):
         raise NotImplementedError
 
 
 class MessageQuery(MessageE6Base):
     def __init__(self, protocol_version):
         super().__init__(
-            protocol_version=protocol_version, message_type=MessageType.query
+            protocol_version=protocol_version,
+            message_type=MessageType.query,
         )
 
     @property
     def _body(self):
         return bytearray([0x01, 0x01] + [0] * 28)
 
 
 class MessageSet(MessageE6Base):
     def __init__(self, protocol_version):
         super().__init__(
-            protocol_version=protocol_version, message_type=MessageType.set
+            protocol_version=protocol_version,
+            message_type=MessageType.set,
         )
         self.main_power = None
         self.heating_temperature = None
         self.bathing_temperature = None
         self.heating_power = None
 
     @property
```

### Comparing `midea_local-1.0.3/midealocal/devices/e8/__init__.py` & `midea_local-1.0.4/midealocal/devices/e8/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageE8Response
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageE8Response, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     status = "status"
```

### Comparing `midea_local-1.0.3/midealocal/devices/e8/message.py` & `midea_local-1.0.4/midealocal/devices/e8/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
 class MessageE8Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xE8,
             protocol_version=protocol_version,
```

### Comparing `midea_local-1.0.3/midealocal/devices/ea/__init__.py` & `midea_local-1.0.4/midealocal/devices/ea/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageEAResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageEAResponse, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     cooking = "cooking"
```

### Comparing `midea_local-1.0.3/midealocal/devices/ea/message.py` & `midea_local-1.0.4/midealocal/devices/ea/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageEABase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xEA,
@@ -103,19 +103,16 @@
                     self.set_body(EABody2(super().body))
                 elif super().body[5] == 0x3D:  # 420
                     self.set_body(EABody1(super().body))
             elif (
                 self.message_type == MessageType.notify1 and super().body[5] == 0x3D
             ):  # 463
                 self.set_body(EABody1(super().body))
-        else:
-            if (
-                (self.message_type == MessageType.set and super().body[3] == 0x02)
-                or (self.message_type == MessageType.query and super().body[3] == 0x03)
-                or (
-                    self.message_type == MessageType.notify1 and super().body[3] == 0x04
-                )
-            ):  # 351
-                self.set_body(EABody3(super().body))
-            elif self.message_type == MessageType.notify1 and super().body[3] == 0x06:
-                self.mode = super().body[4] + (super().body[5] << 8)
+        elif (
+            (self.message_type == MessageType.set and super().body[3] == 0x02)
+            or (self.message_type == MessageType.query and super().body[3] == 0x03)
+            or (self.message_type == MessageType.notify1 and super().body[3] == 0x04)
+        ):  # 351
+            self.set_body(EABody3(super().body))
+        elif self.message_type == MessageType.notify1 and super().body[3] == 0x06:
+            self.mode = super().body[4] + (super().body[5] << 8)
         self.set_attr()
```

### Comparing `midea_local-1.0.3/midealocal/devices/ec/__init__.py` & `midea_local-1.0.4/midealocal/devices/ec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageECResponse
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageECResponse, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     cooking = "cooking"
```

### Comparing `midea_local-1.0.3/midealocal/devices/ec/message.py` & `midea_local-1.0.4/midealocal/devices/ec/message.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageECBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xEC,
```

### Comparing `midea_local-1.0.3/midealocal/devices/ed/__init__.py` & `midea_local-1.0.4/midealocal/devices/ed/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageEDResponse, MessageNewSet, MessageOldSet
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageEDResponse, MessageNewSet, MessageOldSet, MessageQuery
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -84,17 +87,16 @@
         return new_status
 
     def set_attribute(self, attr, value):
         message = None
         if self._use_new_set():
             if attr in [DeviceAttributes.power, DeviceAttributes.child_lock]:
                 message = MessageNewSet(self._protocol_version)
-        else:
-            if attr in []:
-                message = MessageOldSet(self._protocol_version)
+        elif attr in []:
+            message = MessageOldSet(self._protocol_version)
         if message is not None:
             setattr(message, str(attr), value)
             self.build_send(message)
 
 
 class MideaAppliance(MideaEDDevice):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/ed/message.py` & `midea_local-1.0.4/midealocal/devices/ed/message.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from enum import IntEnum
+
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class NewSetTags(IntEnum):
     power = 0x0100
     lock = 0x0201
 
 
 class EDNewSetParamPack:
     @staticmethod
     def pack(param, value, addition=0):
         return bytearray(
-            [param & 0xFF, param >> 8, value, addition & 0xFF, addition >> 8]
+            [param & 0xFF, param >> 8, value, addition & 0xFF, addition >> 8],
         )
 
 
 class MessageEDBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xED,
@@ -63,23 +64,23 @@
         payload = bytearray([0x01, 0x00])
         if self.power is not None:
             pack_count += 1
             payload.extend(
                 EDNewSetParamPack.pack(
                     param=NewSetTags.power,  # power
                     value=0x01 if self.power else 0x00,
-                )
+                ),
             )
         if self.lock is not None:
             pack_count += 1
             payload.extend(
                 EDNewSetParamPack.pack(
                     param=NewSetTags.lock,  # lock
                     value=0x01 if self.lock else 0x00,
-                )
+                ),
             )
         payload[1] = pack_count
         return payload
 
 
 class MessageOldSet(MessageEDBase):
     def __init__(self, protocol_version):
@@ -160,20 +161,18 @@
             attr = ((body[data_offset + 2] % 16) << 8) + body[data_offset + 1]
             if attr == 0x000:
                 self.child_lock = (body[data_offset + 5] & 0x01) > 0
                 self.power = (body[data_offset + 6] & 0x01) > 0
             elif attr == 0x011:
                 self.water_consumption = (
                     float(
-                        (
-                            body[data_offset + 3]
-                            + (body[data_offset + 4] << 8)
-                            + (body[data_offset + 5] << 16)
-                            + (body[data_offset + 6] << 24)
-                        )
+                        body[data_offset + 3]
+                        + (body[data_offset + 4] << 8)
+                        + (body[data_offset + 5] << 16)
+                        + (body[data_offset + 6] << 24),
                     )
                     / 1000
                 )
             elif attr == 0x013:
                 self.in_tds = body[data_offset + 3] + (body[data_offset + 4] << 8)
                 self.out_tds = body[data_offset + 5] + (body[data_offset + 6] << 8)
             elif attr == 0x10:
```

### Comparing `midea_local-1.0.3/midealocal/devices/fa/__init__.py` & `midea_local-1.0.4/midealocal/devices/fa/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import logging
 import json
-from .message import MessageQuery, MessageFAResponse, MessageSet
+import logging
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageFAResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -171,108 +174,112 @@
             ):
                 message = MessageSet(self._protocol_version, self.subtype)
                 if value == "Off" or not value:
                     message.oscillate = False
                 else:
                     message.oscillate = True
                     message.oscillation_mode = MideaFADevice._oscillation_modes.index(
-                        value
+                        value,
                     )
                     if value == "Oscillation":
                         if (
                             self._attributes[DeviceAttributes.oscillation_angle]
                             == "Off"
                         ):
                             message.oscillation_angle = 3  # 90
                         else:
                             message.oscillation_angle = (
                                 MideaFADevice._oscillation_angles.index(
-                                    self._attributes[DeviceAttributes.oscillation_angle]
+                                    self._attributes[
+                                        DeviceAttributes.oscillation_angle
+                                    ],
                                 )
                             )
                     elif value == "Tilting":
                         if self._attributes[DeviceAttributes.tilting_angle] == "Off":
                             message.tilting_angle = 3  # 90
                         else:
                             message.tilting_angle = MideaFADevice._tilting_angles.index(
-                                self._attributes[DeviceAttributes.tilting_angle]
+                                self._attributes[DeviceAttributes.tilting_angle],
                             )
                     else:
                         if (
                             self._attributes[DeviceAttributes.oscillation_angle]
                             == "Off"
                         ):
                             message.oscillation_angle = 3  # 90
                         else:
                             message.oscillation_angle = (
                                 MideaFADevice._oscillation_angles.index(
-                                    self._attributes[DeviceAttributes.oscillation_angle]
+                                    self._attributes[
+                                        DeviceAttributes.oscillation_angle
+                                    ],
                                 )
                             )
                         if self._attributes[DeviceAttributes.tilting_angle] == "Off":
                             message.tilting_angle = 3  # 90
                         else:
                             message.tilting_angle = MideaFADevice._tilting_angles.index(
-                                self._attributes[DeviceAttributes.tilting_angle]
+                                self._attributes[DeviceAttributes.tilting_angle],
                             )
             elif attr == DeviceAttributes.oscillation_angle and (
                 value in MideaFADevice._oscillation_angles or not value
             ):
                 message = MessageSet(self._protocol_version, self.subtype)
                 if value == "Off" or not value:
                     if self._attributes[DeviceAttributes.tilting_angle] == "Off":
                         message.oscillate = False
                     else:
                         message.oscillate = True
                         message.oscillation_mode = 2
                         message.tilting_angle = MideaFADevice._tilting_angles.index(
-                            self._attributes[DeviceAttributes.tilting_angle]
+                            self._attributes[DeviceAttributes.tilting_angle],
                         )
                 else:
                     message.oscillation_angle = MideaFADevice._oscillation_angles.index(
-                        value
+                        value,
                     )
                     message.oscillate = True
                     if self._attributes[DeviceAttributes.tilting_angle] == "Off":
                         message.oscillation_mode = 1
                     elif (
                         self._attributes[DeviceAttributes.oscillation_mode] == "Tilting"
                     ):
                         message.oscillation_mode = 6
                         message.tilting_angle = MideaFADevice._tilting_angles.index(
-                            self._attributes[DeviceAttributes.tilting_angle]
+                            self._attributes[DeviceAttributes.tilting_angle],
                         )
             elif attr == DeviceAttributes.tilting_angle and (
                 value in MideaFADevice._tilting_angles or not value
             ):
                 message = MessageSet(self._protocol_version, self.subtype)
                 if value == "Off" or not value:
                     if self._attributes[DeviceAttributes.oscillation_angle] == "Off":
                         message.oscillate = False
                     else:
                         message.oscillate = True
                         message.oscillation_mode = 1
                         message.oscillation_angle = (
                             MideaFADevice._oscillation_angles.index(
-                                self._attributes[DeviceAttributes.oscillation_angle]
+                                self._attributes[DeviceAttributes.oscillation_angle],
                             )
                         )
                 else:
                     message.tilting_angle = MideaFADevice._tilting_angles.index(value)
                     message.oscillate = True
                     if self._attributes[DeviceAttributes.oscillation_angle] == "Off":
                         message.oscillation_mode = 2
                     elif (
                         self._attributes[DeviceAttributes.oscillation_mode]
                         == "Oscillation"
                     ):
                         message.oscillation_mode = 6
                         message.oscillation_angle = (
                             MideaFADevice._oscillation_angles.index(
-                                self._attributes[DeviceAttributes.oscillation_angle]
+                                self._attributes[DeviceAttributes.oscillation_angle],
                             )
                         )
         return message
 
     def set_attribute(self, attr, value):
         message = None
         if attr in [
@@ -313,13 +320,13 @@
         self._speed_count = self._default_speed_count
         if customize and len(customize) > 0:
             try:
                 params = json.loads(customize)
                 if params and "speed_count" in params:
                     self._speed_count = params.get("speed_count")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"speed_count": self._speed_count})
 
 
 class MideaAppliance(MideaFADevice):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/fa/message.py` & `midea_local-1.0.4/midealocal/devices/fa/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageFABase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xFA,
@@ -73,15 +73,15 @@
                     0x00,
                     0x00,
                     0x00,
                     0x00,
                     0x00,
                     0x00,
                     0x00,
-                ]
+                ],
             )
             if self._subtype != 10:
                 _body_return[13] = 0xFF
         else:
             _body_return = bytearray(
                 [
                     0x00,
@@ -129,15 +129,15 @@
                     0x00,
                     0x00,
                     0x00,
                     0x00,
                     0x00,
                     0x00,
                     0x00,
-                ]
+                ],
             )
         if self.power is not None:
             if self.power:
                 _body_return[3] = 1
             else:
                 _body_return[3] = 0
         if self.lock is not None:
```

### Comparing `midea_local-1.0.3/midealocal/devices/fb/__init__.py` & `midea_local-1.0.4/midealocal/devices/fb/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
-from .message import MessageQuery, MessageFBResponse, MessageSet
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageFBResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
```

### Comparing `midea_local-1.0.3/midealocal/devices/fb/message.py` & `midea_local-1.0.4/midealocal/devices/fb/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageFBBase(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0xFB,
@@ -65,15 +65,15 @@
         target_temperature = (
             0
             if self.target_temperature is None
             else (
                 int(
                     (self.target_temperature + 41)
                     if -40 <= self.target_temperature <= 50
-                    else (0x80 if self.target_temperature in [0x80, 87] else 0)
+                    else (0x80 if self.target_temperature in [0x80, 87] else 0),
                 )
                 & 0xFF
             )
         )
         child_lock = (
             0xFF if self.child_lock is None else (0x01 if self.child_lock else 0x00)
         )
@@ -95,15 +95,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 child_lock,
                 0x00,
-            ]
+            ],
         )
         if self._subtype > 5:
             _return_body += bytearray([0x00, 0x00, 0x00])
         return _return_body
 
     @property
     def _body(self):
```

### Comparing `midea_local-1.0.3/midealocal/devices/fc/__init__.py` & `midea_local-1.0.4/midealocal/devices/fc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import logging
 import json
-from .message import MessageQuery, MessageFCResponse, MessageSet
+import logging
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageFCResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -122,15 +125,15 @@
                     if value in MideaFCDevice._speeds.keys():
                         self._attributes[status] = MideaFCDevice._speeds.get(value)
                     else:
                         self._attributes[status] = None
                 elif status == DeviceAttributes.screen_display:
                     if value in MideaFCDevice._screen_displays.keys():
                         self._attributes[status] = MideaFCDevice._screen_displays.get(
-                            value
+                            value,
                         )
                     else:
                         self._attributes[status] = None
                 elif status == DeviceAttributes.detect_mode:
                     if value < len(MideaFCDevice._detect_modes):
                         self._attributes[status] = MideaFCDevice._detect_modes[value]
                     else:
@@ -148,41 +151,41 @@
         message.anion = self._attributes[DeviceAttributes.anion]
         message.standby = self._attributes[DeviceAttributes.standby]
         message.screen_display = self._attributes[DeviceAttributes.screen_display]
         message.detect_mode = (
             0
             if self._attributes[DeviceAttributes.detect_mode] is None
             else MideaFCDevice._detect_modes.index(
-                self._attributes[DeviceAttributes.detect_mode]
+                self._attributes[DeviceAttributes.detect_mode],
             )
         )
         message.mode = (
             0x10
             if self._attributes[DeviceAttributes.mode] is None
             else list(MideaFCDevice._modes.keys())[
                 list(MideaFCDevice._modes.values()).index(
-                    self._attributes[DeviceAttributes.mode]
+                    self._attributes[DeviceAttributes.mode],
                 )
             ]
         )
         message.fan_speed = (
             39
             if self._attributes[DeviceAttributes.fan_speed] is None
             else list(MideaFCDevice._speeds.keys())[
                 list(MideaFCDevice._speeds.values()).index(
-                    self._attributes[DeviceAttributes.fan_speed]
+                    self._attributes[DeviceAttributes.fan_speed],
                 )
             ]
         )
         message.screen_display = (
             0
             if self._attributes[DeviceAttributes.screen_display] is None
             else list(MideaFCDevice._screen_displays.keys())[
                 list(MideaFCDevice._screen_displays.values()).index(
-                    self._attributes[DeviceAttributes.screen_display]
+                    self._attributes[DeviceAttributes.screen_display],
                 )
             ]
         )
         message.standby_detect = self._standby_detect
         return message
 
     def set_attribute(self, attr, value):
@@ -200,15 +203,15 @@
                 if value in MideaFCDevice._speeds.values():
                     message.fan_speed = list(MideaFCDevice._speeds.keys())[
                         list(MideaFCDevice._speeds.values()).index(value)
                     ]
             elif attr == DeviceAttributes.screen_display:
                 if value in MideaFCDevice._screen_displays.values():
                     message.screen_display = list(
-                        MideaFCDevice._screen_displays.keys()
+                        MideaFCDevice._screen_displays.keys(),
                     )[list(MideaFCDevice._screen_displays.values()).index(value)]
                 elif not value:
                     message.screen_display = 7
             elif attr == DeviceAttributes.detect_mode:
                 if value in MideaFCDevice._detect_modes:
                     message.detect_mode = MideaFCDevice._detect_modes.index(value)
                 elif not value:
@@ -223,13 +226,13 @@
             try:
                 params = json.loads(customize)
                 if params and "standby_detect" in params:
                     settings = params.get("standby_detect")
                     if len(settings) == 2 and settings[0] > settings[1]:
                         self._standby_detect = settings
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"standby_detect": self._standby_detect})
 
 
 class MideaAppliance(MideaFCDevice):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/fc/message.py` & `midea_local-1.0.4/midealocal/devices/fc/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ...crc8 import calculate
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageFCBase(MessageRequest):
     _message_serial = 0
 
     def __init__(self, protocol_version, message_type, body_type):
@@ -60,15 +60,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class MessageSet(MessageFCBase):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -127,15 +127,15 @@
                 detect_mode,
                 standby,
                 standby_detect_high,
                 standby_detect_low,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class FCGeneralMessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = (body[1] & 0x01) > 0
@@ -198,17 +198,16 @@
 
 
 class MessageFCResponse(MessageResponse):
     def __init__(self, message):
         super().__init__(message)
         if self.body_type in [0xB0, 0xB1]:
             pass
-        else:
-            if (
-                self.message_type
-                in [MessageType.query, MessageType.set, MessageType.notify1]
-                and self.body_type == 0xC8
-            ):
-                self.set_body(FCGeneralMessageBody(super().body))
-            elif self.message_type == MessageType.notify1 and self.body_type == 0xA0:
-                self.set_body(FCNotifyMessageBody(super().body))
+        elif (
+            self.message_type
+            in [MessageType.query, MessageType.set, MessageType.notify1]
+            and self.body_type == 0xC8
+        ):
+            self.set_body(FCGeneralMessageBody(super().body))
+        elif self.message_type == MessageType.notify1 and self.body_type == 0xA0:
+            self.set_body(FCNotifyMessageBody(super().body))
         self.set_attr()
```

### Comparing `midea_local-1.0.3/midealocal/devices/fd/__init__.py` & `midea_local-1.0.4/midealocal/devices/fd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
-from .message import MessageQuery, MessageFDResponse, MessageSet
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import MessageFDResponse, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
@@ -129,15 +131,15 @@
                     if value in self._speeds.keys():
                         self._attributes[status] = self._speeds.get(value)
                     else:
                         self._attributes[status] = None
                 elif status == DeviceAttributes.screen_display:
                     if value in MideaFDDevice._screen_displays.keys():
                         self._attributes[status] = MideaFDDevice._screen_displays.get(
-                            value
+                            value,
                         )
                     else:
                         self._attributes[status] = None
                 else:
                     self._attributes[status] = value
                 new_status[str(status)] = self._attributes[status]
         return new_status
@@ -155,24 +157,24 @@
         else:
             message.mode = 1
         message.fan_speed = (
             40
             if self._attributes[DeviceAttributes.fan_speed] is None
             else list(self._speeds.keys())[
                 list(self._speeds.values()).index(
-                    self._attributes[DeviceAttributes.fan_speed]
+                    self._attributes[DeviceAttributes.fan_speed],
                 )
             ]
         )
         message.screen_display = (
             0
             if self._attributes[DeviceAttributes.screen_display] is None
             else list(MideaFDDevice._screen_displays.keys())[
                 list(MideaFDDevice._screen_displays.values()).index(
-                    self._attributes[DeviceAttributes.screen_display]
+                    self._attributes[DeviceAttributes.screen_display],
                 )
             ]
         )
         return message
 
     def set_attribute(self, attr, value):
         if attr == DeviceAttributes.prompt_tone:
@@ -187,15 +189,15 @@
                 if value in self._speeds.values():
                     message.fan_speed = list(self._speeds.keys())[
                         list(self._speeds.values()).index(value)
                     ]
             elif attr == DeviceAttributes.screen_display:
                 if value in MideaFDDevice._screen_displays.values():
                     message.screen_display = list(
-                        MideaFDDevice._screen_displays.keys()
+                        MideaFDDevice._screen_displays.keys(),
                     )[list(MideaFDDevice._screen_displays.values()).index(value)]
                 elif not value:
                     message.screen_display = 7
             else:
                 setattr(message, str(attr), value)
             self.build_send(message)
```

### Comparing `midea_local-1.0.3/midealocal/devices/fd/message.py` & `midea_local-1.0.4/midealocal/devices/fd/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from ...crc8 import calculate
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class MessageFDBase(MessageRequest):
     _message_serial = 0
 
     def __init__(self, protocol_version, message_type, body_type):
@@ -60,15 +60,15 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class MessageSet(MessageFDBase):
     def __init__(self, protocol_version):
         super().__init__(
             protocol_version=protocol_version,
@@ -107,15 +107,15 @@
                 disinfect,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
 
 
 class FDC8MessageBody(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.power = (body[1] & 0x01) > 0
```

### Comparing `midea_local-1.0.3/midealocal/devices/x13/__init__.py` & `midea_local-1.0.4/midealocal/devices/x13/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import logging
 import json
-from .message import MessageQuery, MessageSet, Message13Response
+import logging
+import sys
 
-try:
-    from enum import StrEnum
-except ImportError:
+from .message import Message13Response, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 from ...device import MideaDevice
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     brightness = "brightness"
@@ -66,15 +69,15 @@
     def color_temp_range(self):
         return self._color_temp_range
 
     def kelvin_to_midea(self, kelvin):
         return round(
             (kelvin - self._color_temp_range[0])
             / (self._color_temp_range[1] - self._color_temp_range[0])
-            * 255
+            * 255,
         )
 
     def midea_to_kelvin(self, midea):
         return (
             round((self._color_temp_range[1] - self._color_temp_range[0]) / 255 * midea)
             + self._color_temp_range[0]
         )
@@ -123,13 +126,13 @@
         self._color_temp_range = self._default_color_temp_range
         if customize and len(customize) > 0:
             try:
                 params = json.loads(customize)
                 if params and "color_temp_range_kelvin" in params:
                     self._color_temp_range = params.get("color_temp_range_kelvin")
             except Exception as e:
-                _LOGGER.error(f"[{self.device_id}] Set customize error: {repr(e)}")
+                _LOGGER.error(f"[{self.device_id}] Set customize error: {e!r}")
             self.update_all({"color_temp_range": self._color_temp_range})
 
 
 class MideaAppliance(Midea13Device):
     pass
```

### Comparing `midea_local-1.0.3/midealocal/devices/x13/message.py` & `midea_local-1.0.4/midealocal/devices/x13/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
 class Message13Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0x13,
             protocol_version=protocol_version,
```

### Comparing `midea_local-1.0.3/midealocal/devices/x26/__init__.py` & `midea_local-1.0.4/midealocal/devices/x26/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import logging
 import math
-from .message import MessageQuery, MessageSet, Message26Response
+import sys
+from typing import Any
 
-try:
-    from enum import StrEnum
-except ImportError:
-    from ...backports.enum import StrEnum
 from ...device import MideaDevice
+from .message import Message26Response, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
+    from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     main_light = "main_light"
     night_light = "night_light"
@@ -55,15 +58,15 @@
                 DeviceAttributes.mode: None,
                 DeviceAttributes.direction: None,
                 DeviceAttributes.current_humidity: None,
                 DeviceAttributes.current_radar: None,
                 DeviceAttributes.current_temperature: None,
             },
         )
-        self._fields = {}
+        self._fields = dict[Any, Any]
 
     @staticmethod
     def _convert_to_midea_direction(direction):
         if direction == "Oscillate":
             result = 0xFD
         else:
             result = (
@@ -92,15 +95,15 @@
     def build_query(self):
         return [MessageQuery(self._protocol_version)]
 
     def process_message(self, msg):
         message = Message26Response(msg)
         _LOGGER.debug(f"[{self.device_id}] Received: {message}")
         new_status = {}
-        self._fields = getattr(message, "fields")
+        self._fields = message.fields
         for status in self._attributes.keys():
             if hasattr(message, str(status)):
                 value = getattr(message, str(status))
                 if status == DeviceAttributes.mode:
                     self._attributes[status] = Midea26Device._modes[value]
                 elif status == DeviceAttributes.direction:
                     self._attributes[status] = Midea26Device._directions[
@@ -119,18 +122,18 @@
             DeviceAttributes.direction,
         ]:
             message = MessageSet(self._protocol_version)
             message.fields = self._fields
             message.main_light = self._attributes[DeviceAttributes.main_light]
             message.night_light = self._attributes[DeviceAttributes.night_light]
             message.mode = Midea26Device._modes.index(
-                self._attributes[DeviceAttributes.mode]
+                self._attributes[DeviceAttributes.mode],
             )
             message.direction = self._convert_to_midea_direction(
-                self._attributes[DeviceAttributes.direction]
+                self._attributes[DeviceAttributes.direction],
             )
             if attr in [DeviceAttributes.main_light, DeviceAttributes.night_light]:
                 message.main_light = False
                 message.night_light = False
                 setattr(message, str(attr), value)
             elif attr == DeviceAttributes.mode:
                 message.mode = Midea26Device._modes.index(value)
```

### Comparing `midea_local-1.0.3/midealocal/devices/x26/message.py` & `midea_local-1.0.4/midealocal/devices/x26/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
 class Message26Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0x26,
             protocol_version=protocol_version,
@@ -90,15 +90,15 @@
                 self.read_field("SOFT_WIND_TEMPERATURE"),
                 self.read_field("SOFT_WIND_SPEED"),
                 self.read_field("SOFT_WIND_DIRECTION"),
                 self.read_field("WINDLESS_ENABLE"),
                 self.read_field("ANION_ENABLE"),
                 self.read_field("SMELLY_ENABLE"),
                 self.read_field("SMELLY_THRESHOLD"),
-            ]
+            ],
         )
 
 
 class Message26Body(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.fields = {}
```

### Comparing `midea_local-1.0.3/midealocal/devices/x34/__init__.py` & `midea_local-1.0.4/midealocal/devices/x34/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
+import sys
+
+from ...device import MideaDevice
 from .message import (
-    MessageQuery,
+    Message34Response,
+    MessageLock,
     MessagePower,
+    MessageQuery,
     MessageStorage,
-    MessageLock,
-    Message34Response,
 )
 
-try:
-    from enum import StrEnum
-except ImportError:
+if sys.version_info < (3, 12):
     from ...backports.enum import StrEnum
-from ...device import MideaDevice
+else:
+    from enum import StrEnum
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     power = "power"
     status = "status"
```

### Comparing `midea_local-1.0.3/midealocal/devices/x34/message.py` & `midea_local-1.0.4/midealocal/devices/x34/message.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ...message import (
-    MessageType,
+    MessageBody,
     MessageRequest,
     MessageResponse,
-    MessageBody,
+    MessageType,
 )
 
 
 class Message34Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0x34,
```

### Comparing `midea_local-1.0.3/midealocal/devices/x40/__init__.py` & `midea_local-1.0.4/midealocal/devices/x40/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import logging
 import math
-from .message import MessageQuery, MessageSet, Message40Response
+import sys
+from typing import Any
 
-try:
-    from enum import StrEnum
-except ImportError:
-    from ...backports.enum import StrEnum
 from ...device import MideaDevice
+from .message import Message40Response, MessageQuery, MessageSet
+
+if sys.version_info < (3, 12):
+    from ...backports.enum import StrEnum
+else:
+    from enum import StrEnum
+
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class DeviceAttributes(StrEnum):
     light = "light"
     fan_speed = "fan_speed"
@@ -52,15 +56,15 @@
                 DeviceAttributes.fan_speed: 0,
                 DeviceAttributes.direction: False,
                 DeviceAttributes.ventilation: False,
                 DeviceAttributes.smelly_sensor: False,
                 DeviceAttributes.current_temperature: None,
             },
         )
-        self._fields = {}
+        self._fields = dict[Any, Any]
 
     @property
     def directions(self):
         return Midea40Device._directions
 
     @staticmethod
     def _convert_to_midea_direction(direction):
@@ -85,15 +89,15 @@
     def build_query(self):
         return [MessageQuery(self._protocol_version)]
 
     def process_message(self, msg):
         message = Message40Response(msg)
         _LOGGER.debug(f"[{self.device_id}] Received: {message}")
         new_status = {}
-        self._fields = getattr(message, "fields")
+        self._fields = message.fields
         for status in self._attributes.keys():
             if hasattr(message, str(status)):
                 value = getattr(message, str(status))
                 if status == DeviceAttributes.direction:
                     self._attributes[status] = Midea40Device._directions[
                         self._convert_from_midea_direction(value)
                     ]
@@ -113,15 +117,15 @@
             message = MessageSet(self._protocol_version)
             message.fields = self._fields
             message.light = self._attributes[DeviceAttributes.light]
             message.ventilation = self._attributes[DeviceAttributes.ventilation]
             message.smelly_sensor = self._attributes[DeviceAttributes.smelly_sensor]
             message.fan_speed = self._attributes[DeviceAttributes.fan_speed]
             message.direction = self._convert_to_midea_direction(
-                self._attributes[DeviceAttributes.direction]
+                self._attributes[DeviceAttributes.direction],
             )
             if attr == DeviceAttributes.direction:
                 message.direction = self._convert_to_midea_direction(value)
             elif attr == DeviceAttributes.ventilation and message.fan_speed == 2:
                 message.fan_speed = 1
                 message.ventilation = value
             else:
```

### Comparing `midea_local-1.0.3/midealocal/devices/x40/message.py` & `midea_local-1.0.4/midealocal/devices/x40/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ...message import MessageType, MessageRequest, MessageResponse, MessageBody
+from ...message import MessageBody, MessageRequest, MessageResponse, MessageType
 
 
 class Message40Base(MessageRequest):
     def __init__(self, protocol_version, message_type, body_type):
         super().__init__(
             device_type=0x40,
             protocol_version=protocol_version,
@@ -91,15 +91,15 @@
                 self.read_field("SOFT_WIND_TEMPERATURE"),
                 self.read_field("SOFT_WIND_SPEED"),
                 self.read_field("SOFT_WIND_DIRECTION"),
                 self.read_field("WINDLESS_ENABLE"),
                 self.read_field("ANION_ENABLE"),
                 smelly_sensor,
                 self.read_field("SMELLY_THRESHOLD"),
-            ]
+            ],
         )
 
 
 class Message40Body(MessageBody):
     def __init__(self, body):
         super().__init__(body)
         self.fields = {}
```

### Comparing `midea_local-1.0.3/midealocal/discover.py` & `midea_local-1.0.4/midealocal/discover.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import socket
 import xml.etree.ElementTree as ET
 from ipaddress import IPv4Network
+from typing import Any
 
 import ifaddr
 
 from .security import LocalSecurity
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -79,15 +80,15 @@
         0x9E,
         0xB8,
         0xEC,
         0x91,
         0x8E,
         0x92,
         0xE5,
-    ]
+    ],
 )
 
 DEVICE_INFO_MSG = bytearray(
     [
         0x5A,
         0x5A,
         0x15,
@@ -140,70 +141,75 @@
         0xE4,
         0x2D,
         0x53,
         0x49,
         0x47,
         0x62,
         0xBE,
-    ]
+    ],
 )
 
 
-def discover(discover_type=None, ip_address=None):
+def discover(
+    discover_type: list | None = None,
+    ip_address: list | None = None,
+) -> dict[int, dict[str, Any]]:
     if discover_type is None:
         discover_type = []
     security = LocalSecurity()
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
     sock.settimeout(5)
     found_devices = {}
     if ip_address is None:
         addrs = enum_all_broadcast()
     else:
         addrs = [ip_address]
-    _LOGGER.debug(f"All addresses for broadcast: {addrs}")
+    _LOGGER.debug("All addresses for broadcast: %s", addrs)
     for addr in addrs:
         try:
             sock.sendto(BROADCAST_MSG, (addr, 6445))
             sock.sendto(BROADCAST_MSG, (addr, 20086))
         except Exception:
-            _LOGGER.warning(f"Can't access network {addr}")
+            _LOGGER.warning("Can't access network %s", addrs)
     while True:
         try:
             data, addr = sock.recvfrom(512)
             ip = addr[0]
-            _LOGGER.debug(f"Received response from {addr}: {data.hex()}")
+            _LOGGER.debug("Received response from %s: %s", addr, data.hex())
             if len(data) >= 104 and (
                 data[:2].hex() == "5a5a" or data[8:10].hex() == "5a5a"
             ):
                 if data[:2].hex() == "5a5a":
                     protocol = 2
                 elif data[:2].hex() == "8370":
                     protocol = 3
                     if data[8:10].hex() == "5a5a":
                         data = data[8:-16]
                 else:
                     continue
                 device_id = int.from_bytes(
-                    bytearray.fromhex(data[20:26].hex()), "little"
+                    bytearray.fromhex(data[20:26].hex()),
+                    "little",
                 )
                 if device_id in found_devices:
                     continue
                 encrypt_data = data[40:-16]
                 reply = security.aes_decrypt(encrypt_data)
-                _LOGGER.debug(f"Declassified reply: {reply.hex()}")
+                _LOGGER.debug("Declassified reply: %s", reply.hex())
                 ssid = reply[41 : 41 + reply[40]].decode("utf-8")
                 device_type = ssid.split("_")[1]
                 port = bytes2port(reply[4:8])
                 model = reply[17:25].decode("utf-8")
                 sn = reply[8:40].decode("utf-8")
             elif data[:6].hex() == "3c3f786d6c20":
                 protocol = 1
                 root = ET.fromstring(data.decode(encoding="utf-8", errors="replace"))
                 child = root.find("body/device")
+                assert child
                 m = child.attrib
                 port, sn, device_type = (
                     int(m["port"]),
                     m["apc_sn"],
                     str(hex(int(m["apc_type"])))[2:],
                 )
                 response = get_device_info(ip, int(port))
@@ -223,79 +229,83 @@
                 "port": port,
                 "model": model,
                 "sn": sn,
                 "protocol": protocol,
             }
             if len(discover_type) == 0 or device.get("type") in discover_type:
                 found_devices[device_id] = device
-                _LOGGER.debug(f"Found a supported device: {device}")
+                _LOGGER.debug("Found a supported device: %s", device)
             else:
-                _LOGGER.debug(f"Found a unsupported device: {device}")
+                _LOGGER.debug("Found a unsupported device: %s", device)
         except socket.timeout:
             break
-        except socket.error as e:
-            _LOGGER.error(f"Socket error: {repr(e)}")
+        except OSError as e:
+            _LOGGER.error("Socket error: %s", repr(e))
     return found_devices
 
 
-def get_id_from_response(response):
+def get_id_from_response(response: bytearray) -> int:
     if response[64:-16][:6].hex() == "3c3f786d6c20":
         xml = response[64:-16]
         root = ET.fromstring(xml.decode(encoding="utf-8", errors="replace"))
         child = root.find("smartDevice")
+        assert child
         m = child.attrib
         return int.from_bytes(bytearray.fromhex(m["devId"]), "little")
     else:
         return 0
 
 
-def bytes2port(paramArrayOfbyte):
+def bytes2port(paramArrayOfbyte: bytes | None) -> int:
     if paramArrayOfbyte is None:
         return 0
     b, i = 0, 0
     while b < 4:
         if b < len(paramArrayOfbyte):
             b1 = paramArrayOfbyte[b] & 0xFF
         else:
             b1 = 0
         i |= b1 << b * 8
         b += 1
     return i
 
 
-def get_device_info(device_ip, device_port: int):
+def get_device_info(device_ip: str, device_port: int) -> bytearray:
     response = bytearray(0)
     try:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
             sock.settimeout(8)
             device_address = (device_ip, device_port)
             sock.connect(device_address)
             _LOGGER.debug(
-                f"Sending to {device_ip}:{device_port} {DEVICE_INFO_MSG.hex()}"
+                "Sending to %s:%s %s", device_ip, device_port, DEVICE_INFO_MSG.hex()
             )
             sock.sendall(DEVICE_INFO_MSG)
-            response = sock.recv(512)
-    except socket.timeout:
+            response = bytearray(sock.recv(512))
+    except TimeoutError:
         _LOGGER.warning(
-            f"Connect the device {device_ip}:{device_port} timed out for 8s. "
-            f"Don't care about a small amount of this. if many maybe not support."
+            "Connect the device %s:%s timed out for 8s."
+            "Don't care about a small amount of this. if many maybe not support.",
+            device_ip,
+            device_port,
         )
-    except socket.error:
-        _LOGGER.warning(f"Can't connect to Device {device_ip}:{device_port}")
+    except OSError:
+        _LOGGER.warning("Can't connect to Device %s:%s", device_ip, device_port)
     return response
 
 
-def enum_all_broadcast():
+def enum_all_broadcast() -> list:
     nets = []
     adapters = ifaddr.get_adapters()
     for adapter in adapters:
         for ip in adapter.ips:
             if ip.is_IPv4 and ip.network_prefix < 32:
                 local_network = IPv4Network(
-                    f"{ip.ip}/{ip.network_prefix}", strict=False
+                    f"{ip.ip}/{ip.network_prefix}",
+                    strict=False,
                 )
                 if (
                     local_network.is_private
                     and not local_network.is_loopback
                     and not local_network.is_link_local
                 ):
                     addr = str(local_network.broadcast_address)
```

### Comparing `midea_local-1.0.3/midealocal/message.py` & `midea_local-1.0.4/midealocal/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from abc import ABC
 from enum import IntEnum
+from typing import SupportsIndex, cast
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class MessageLenError(Exception):
     pass
 
@@ -23,65 +24,68 @@
     notify1 = (0x04,)
     notify2 = (0x05,)
     exception = (0x06,)
     exception2 = (0x0A,)
     query_appliance = 0xA0
 
 
+NONE_VALUE = 0x00
+
+
 class MessageBase(ABC):
     HEADER_LENGTH = 10
 
-    def __init__(self):
-        self._device_type = 0x00
-        self._message_type = 0x00
-        self._body_type = 0x00
-        self._protocol_version = 0x00
+    def __init__(self) -> None:
+        self._device_type = NONE_VALUE
+        self._message_type = NONE_VALUE
+        self._body_type = NONE_VALUE
+        self._protocol_version = NONE_VALUE
 
     @staticmethod
-    def checksum(data):
-        return (~sum(data) + 1) & 0xFF
+    def checksum(data: bytes) -> SupportsIndex:
+        return cast(SupportsIndex, (~sum(data) + 1) & 0xFF)
 
     @property
-    def header(self):
+    def header(self) -> bytearray:
         raise NotImplementedError
 
     @property
-    def body(self):
+    def body(self) -> bytearray:
         raise NotImplementedError
 
     @property
-    def message_type(self):
+    def message_type(self) -> int:
         return self._message_type
 
     @message_type.setter
-    def message_type(self, value):
+    def message_type(self, value: int) -> None:
         self._message_type = value
 
     @property
-    def device_type(self):
+    def device_type(self) -> int:
         return self._device_type
 
     @device_type.setter
-    def device_type(self, value):
+    def device_type(self, value: int) -> None:
         self._device_type = value
 
     @property
-    def body_type(self):
+    def body_type(self) -> int:
         return self._body_type
 
     @body_type.setter
-    def body_type(self, value):
+    def body_type(self, value: int) -> None:
         self._body_type = value
 
     @property
-    def protocol_version(self):
+    def protocol_version(self) -> int:
         return self._protocol_version
 
     @protocol_version.setter
-    def protocol_version(self, protocol_version):
+    def protocol_version(self, protocol_version: int) -> None:
         self._protocol_version = protocol_version
 
     def __str__(self) -> str:
         output = {
             "header": self.header.hex(),
             "body": self.body.hex(),
             "message type": "%02x" % self._message_type,
@@ -89,23 +93,29 @@
                 ("%02x" % self._body_type) if self._body_type is not None else "None"
             ),
         }
         return str(output)
 
 
 class MessageRequest(MessageBase):
-    def __init__(self, device_type, protocol_version, message_type, body_type):
+    def __init__(
+        self,
+        device_type: int,
+        protocol_version: int,
+        message_type: int,
+        body_type: int,
+    ) -> None:
         super().__init__()
         self.device_type = device_type
         self.protocol_version = protocol_version
         self.message_type = message_type
         self.body_type = body_type
 
     @property
-    def header(self):
+    def header(self) -> bytearray:
         length = self.HEADER_LENGTH + len(self.body)
         return bytearray(
             [
                 # flag
                 0xAA,
                 # length
                 length,
@@ -120,153 +130,159 @@
                 0x00,
                 # frame protocol version
                 0x00,
                 # device protocol version
                 self.protocol_version,
                 # frame type
                 self.message_type,
-            ]
+            ],
         )
 
     @property
-    def _body(self):
+    def _body(self) -> bytearray:
         raise NotImplementedError
 
     @property
-    def body(self):
+    def body(self) -> bytearray:
         body = bytearray([])
         if self.body_type is not None:
             body.append(self.body_type)
         if self._body is not None:
             body.extend(self._body)
         return body
 
-    def serialize(self):
+    def serialize(self) -> bytearray:
         stream = self.header + self.body
         stream.append(MessageBase.checksum(stream[1:]))
         return stream
 
 
 class MessageQuestCustom(MessageRequest):
-    def __init__(self, device_type, protocol_version, cmd_type, cmd_body):
+    def __init__(
+        self,
+        device_type: int,
+        protocol_version: int,
+        cmd_type: int,
+        cmd_body: bytearray,
+    ) -> None:
         super().__init__(
             device_type=device_type,
             protocol_version=protocol_version,
             message_type=cmd_type,
-            body_type=None,
+            body_type=NONE_VALUE,
         )
         self._cmd_body = cmd_body
 
     @property
-    def _body(self):
+    def _body(self) -> bytearray:
         return bytearray([])
 
     @property
-    def body(self):
+    def body(self) -> bytearray:
         return self._cmd_body
 
 
 class MessageQueryAppliance(MessageRequest):
-    def __init__(self, device_type):
+    def __init__(self, device_type: int) -> None:
         super().__init__(
             device_type=device_type,
             protocol_version=0,
             message_type=MessageType.query_appliance,
-            body_type=None,
+            body_type=NONE_VALUE,
         )
 
     @property
-    def _body(self):
+    def _body(self) -> bytearray:
         return bytearray([])
 
     @property
-    def body(self):
+    def body(self) -> bytearray:
         return bytearray([0x00] * 19)
 
 
 class MessageBody:
-    def __init__(self, body):
+    def __init__(self, body: bytearray) -> None:
         self._data = body
 
     @property
-    def data(self):
+    def data(self) -> bytearray:
         return self._data
 
     @property
-    def body_type(self):
+    def body_type(self) -> int:
         return self._data[0]
 
     @staticmethod
-    def read_byte(body, byte, default_value=0):
+    def read_byte(body: bytearray, byte: int, default_value: int = 0) -> int:
         return body[byte] if len(body) > byte else default_value
 
 
 class NewProtocolMessageBody(MessageBody):
-    def __init__(self, body, bt):
+    def __init__(self, body: bytearray, bt: int) -> None:
         super().__init__(body)
         if bt == 0xB5:
             self._pack_len = 4
         else:
             self._pack_len = 5
 
     @staticmethod
-    def pack(param, value: bytearray, pack_len=4):
+    def pack(param: int, value: bytearray, pack_len: int = 4) -> bytearray:
         length = len(value)
         if pack_len == 4:
             stream = bytearray([param & 0xFF, param >> 8, length]) + value
         else:
             stream = bytearray([param & 0xFF, param >> 8, 0x00, length]) + value
         return stream
 
-    def parse(self):
+    def parse(self) -> dict[int, bytearray]:
         result = {}
         try:
             pos = 2
-            for pack in range(0, self.data[1]):
+            for pack in range(self.data[1]):
                 param = self.data[pos] + (self.data[pos + 1] << 8)
                 if self._pack_len == 5:
                     pos += 1
                 length = self.data[pos + 2]
                 if length > 0:
                     value = self.data[pos + 3 : pos + 3 + length]
                     result[param] = value
                 pos += 3 + length
         except IndexError:
             # Some device used non-standard new-protocol(美的乐享三代中央空调?)
-            _LOGGER.debug(f"Non-standard new-protocol {self.data.hex()}")
+            _LOGGER.debug("Non-standard new-protocol %s", self.data.hex())
         return result
 
 
 class MessageResponse(MessageBase):
-    def __init__(self, message):
+    def __init__(self, message: bytearray) -> None:
         super().__init__()
         if message is None or len(message) < self.HEADER_LENGTH + 1:
             raise MessageLenError
         self._header = message[: self.HEADER_LENGTH]
         self.protocol_version = self._header[-2]
         self.message_type = self._header[-1]
         self.device_type = self._header[2]
         body = message[self.HEADER_LENGTH : -1]
         self._body = MessageBody(body)
         self.body_type = self._body.body_type
 
     @property
-    def header(self):
+    def header(self) -> bytearray:
         return self._header
 
     @property
-    def body(self):
+    def body(self) -> bytearray:
         return self._body.data
 
-    def set_body(self, body: MessageBody):
+    def set_body(self, body: MessageBody) -> None:
         self._body = body
 
-    def set_attr(self):
+    def set_attr(self) -> None:
         for key in vars(self._body).keys():
             if key != "data":
                 value = getattr(self._body, key, None)
                 setattr(self, key, value)
 
 
 class MessageApplianceResponse(MessageResponse):
-    def __init__(self, message):
+    def __init__(self, message: bytearray) -> None:
         super().__init__(message)
```

### Comparing `midea_local-1.0.3/midealocal/packet_builder.py` & `midea_local-1.0.4/midealocal/packet_builder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
+from typing import cast
 
 from .security import LocalSecurity
 
 
 class PacketBuilder:
-    def __init__(self, device_id: int, command):
-        self.command = None
+    def __init__(self, device_id: int, command: bytes) -> None:
+        self.command: bytes
         self.security = LocalSecurity()
         # aa20ac00000000000003418100ff03ff000200000000000000000000000006f274
         # Init the packet with the header data.
         self.packet = bytearray(
             [
                 # 2 bytes - StaicHeader
                 0x5A,
@@ -55,40 +56,40 @@
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
                 0x00,
-            ]
+            ],
         )
         self.packet[12:20] = self.packet_time()
         self.packet[20:28] = device_id.to_bytes(8, "little")
         self.command = command
 
-    def finalize(self, msg_type=1):
+    def finalize(self, msg_type: int = 1) -> bytearray:
         if msg_type != 1:
             self.packet[3] = 0x10
             self.packet[6] = 0x7B
         else:
             self.packet.extend(self.security.aes_encrypt(self.command))
         # PacketLenght
         self.packet[4:6] = (len(self.packet) + 16).to_bytes(2, "little")
         # Append a basic checksum data(16 bytes) to the packet
         self.packet.extend(self.encode32(self.packet))
         return self.packet
 
-    def encode32(self, data: bytearray):
+    def encode32(self, data: bytearray) -> bytes:
         return self.security.encode32_data(data)
 
     @staticmethod
-    def checksum(data):
-        return (~sum(data) + 1) & 0xFF
+    def checksum(data: bytes) -> bytes:
+        return cast(bytes, (~sum(data) + 1) & 0xFF)
 
     @staticmethod
-    def packet_time():
+    def packet_time() -> bytearray:
         t = datetime.datetime.now().strftime("%Y%m%d%H%M%S%f")[:16]
         b = bytearray()
         for i in range(0, len(t), 2):
             d = int(t[i : i + 2])
             b.insert(0, d)
         return b
```

### Comparing `midea_local-1.0.3/midealocal/security.py` & `midea_local-1.0.4/midealocal/security.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,272 @@
 import hmac
 from hashlib import md5, sha256
-from typing import Any
+from typing import Any, cast
 from urllib.parse import unquote_plus, urlencode, urlparse
 
 from Crypto.Cipher import AES
 from Crypto.Random import get_random_bytes
 from Crypto.Util.Padding import pad, unpad
 from Crypto.Util.strxor import strxor
 
+Buffer = bytes | bytearray | memoryview  # alias from Crypto.Cipher.AES
+
 MSGTYPE_HANDSHAKE_REQUEST = 0x0
 MSGTYPE_HANDSHAKE_RESPONSE = 0x1
 MSGTYPE_ENCRYPTED_RESPONSE = 0x3
 MSGTYPE_ENCRYPTED_REQUEST = 0x6
 
 
 class CloudSecurity:
-    def __init__(self, login_key, iot_key, hmac_key, fixed_key=None, fixed_iv=None):
+    def __init__(
+        self,
+        login_key: str,
+        iot_key: str | None,
+        hmac_key: str | None,
+        fixed_key: int | None = None,
+        fixed_iv: int | None = None,
+    ) -> None:
         self._login_key = login_key
         self._iot_key = iot_key
         self._hmac_key = hmac_key
-        self._aes_key = None
-        self._aes_iv = None
+        self._aes_key: bytes
+        self._aes_iv: bytes
         self._fixed_key = format(fixed_key, "x").encode("ascii") if fixed_key else None
         self._fixed_iv = format(fixed_iv, "x").encode("ascii") if fixed_iv else None
 
-    def sign(self, url: str, data: Any, random: str) -> str:
-        msg = self._iot_key
+    def sign(self, url: str, data: dict[str, Any] | str, random: str) -> str | None:
+        msg: str = self._iot_key or ""
         msg += str(data)
         msg += random
+        if not self._hmac_key:
+            return None
         sign = hmac.new(self._hmac_key.encode("ascii"), msg.encode("ascii"), sha256)
         return sign.hexdigest()
 
-    def encrypt_password(self, login_id, data):
+    def encrypt_password(self, login_id: str, data: str) -> str:
         m = sha256()
         m.update(data.encode("ascii"))
         login_hash = login_id + m.hexdigest() + self._login_key
         m = sha256()
         m.update(login_hash.encode("ascii"))
         return m.hexdigest()
 
-    def encrypt_iam_password(self, login_id, data) -> str:
+    def encrypt_iam_password(self, login_id: str, data: str) -> str:
         raise NotImplementedError
 
     @staticmethod
-    def get_deviceid(username):
+    def get_deviceid(username: str) -> str:
         return sha256(f"Hello, {username}!".encode("ascii")).digest().hex()[:16]
 
     @staticmethod
-    def get_udp_id(appliance_id, method=0):
+    def get_udp_id(appliance_id: Any, method: int = 0) -> str | None:
         if method == 0:
             bytes_id = bytes(reversed(appliance_id.to_bytes(8, "big")))
         elif method == 1:
             bytes_id = appliance_id.to_bytes(6, "big")
         elif method == 2:
             bytes_id = appliance_id.to_bytes(6, "little")
         else:
             return None
         data = bytearray(sha256(bytes_id).digest())
-        for i in range(0, 16):
+        for i in range(16):
             data[i] ^= data[i + 16]
         return data[0:16].hex()
 
-    def set_aes_keys(self, key, iv):
+    def set_aes_keys(self, key: bytes | str, iv: bytes | str) -> None:
         if isinstance(key, str):
             key = key.encode("ascii")
         if isinstance(iv, str):
             iv = iv.encode("ascii")
         self._aes_key = key
         self._aes_iv = iv
 
-    def aes_encrypt_with_fixed_key(self, data):
+    def aes_encrypt_with_fixed_key(self, data: bytes) -> bytes:
         return self.aes_encrypt(data, self._fixed_key, self._fixed_iv)
 
-    def aes_decrypt_with_fixed_key(self, data):
+    def aes_decrypt_with_fixed_key(self, data: str) -> str:
         return self.aes_decrypt(data, self._fixed_key, self._fixed_iv)
 
-    def aes_encrypt(self, data, key=None, iv=None):
+    def aes_encrypt(
+        self,
+        data: str | bytes,
+        key: bytes | None = None,
+        iv: bytes | None = None,
+    ) -> bytes:
+        if len(data) == 0:
+            return b""
         if key is not None:
             aes_key = key
             aes_iv = iv
         else:
             aes_key = self._aes_key
             aes_iv = self._aes_iv
         if aes_key is None:
             raise ValueError("Encrypt need a key")
         if isinstance(data, str):
             data = bytes.fromhex(data)
-        if aes_iv is None:  # ECB
-            return AES.new(aes_key, AES.MODE_ECB).encrypt(pad(data, 16))
-        else:  # CBC
-            return AES.new(aes_key, AES.MODE_CBC, iv=aes_iv).encrypt(pad(data, 16))
+        if aes_iv is None or aes_iv == b"0":  # ECB
+            return cast(bytes, AES.new(aes_key, AES.MODE_ECB).encrypt(pad(data, 16)))
+        # CBC
+        return cast(
+            bytes,
+            AES.new(aes_key, AES.MODE_CBC, iv=aes_iv).encrypt(pad(data, 16)),
+        )
 
-    def aes_decrypt(self, data, key=None, iv=None):
+    def aes_decrypt(
+        self,
+        data: str | bytes,
+        key: bytes | None = None,
+        iv: bytes | None = None,
+    ) -> str:
+        if len(data) == 0:
+            return ""
         if key is not None:
             aes_key = key
             aes_iv = iv
         else:
             aes_key = self._aes_key
             aes_iv = self._aes_iv
         if aes_key is None:
             raise ValueError("Encrypt need a key")
         if isinstance(data, str):
             data = bytes.fromhex(data)
-        if aes_iv is None:  # ECB
-            return unpad(
-                AES.new(aes_key, AES.MODE_ECB).decrypt(data), len(aes_key)
-            ).decode()
+        if aes_iv is None or aes_iv == b"0":  # ECB
+            return cast(
+                str,
+                unpad(
+                    AES.new(aes_key, AES.MODE_ECB).decrypt(data),
+                    len(aes_key),
+                ).decode(),
+            )
         else:  # CBC
-            return unpad(
-                AES.new(aes_key, AES.MODE_CBC, iv=aes_iv).decrypt(data), len(aes_key)
-            ).decode()
+            return cast(
+                str,
+                unpad(
+                    AES.new(aes_key, AES.MODE_CBC, iv=aes_iv).decrypt(data),
+                    len(aes_key),
+                ).decode(),
+            )
 
 
 class MeijuCloudSecurity(CloudSecurity):
-    def __init__(self, login_key, iot_key, hmac_key):
+    def __init__(self, login_key: str, iot_key: str, hmac_key: str) -> None:
         super().__init__(login_key, iot_key, hmac_key, 10864842703515613082)
 
-    def encrypt_iam_password(self, login_id, data) -> str:
+    def encrypt_iam_password(self, login_id: str, data: str) -> str:
         md = md5()
         md.update(data.encode("ascii"))
         md_second = md5()
         md_second.update(md.hexdigest().encode("ascii"))
         return md_second.hexdigest()
 
 
 class MSmartCloudSecurity(CloudSecurity):
-    def __init__(self, login_key, iot_key, hmac_key):
+    def __init__(self, login_key: str, iot_key: str, hmac_key: str) -> None:
         super().__init__(
-            login_key, iot_key, hmac_key, 13101328926877700970, 16429062708050928556
+            login_key,
+            iot_key,
+            hmac_key,
+            13101328926877700970,
+            16429062708050928556,
         )
 
-    def encrypt_iam_password(self, login_id, data) -> str:
+    def encrypt_iam_password(self, login_id: str, data: str) -> str:
         md = md5()
         md.update(data.encode("ascii"))
         md_second = md5()
         md_second.update(md.hexdigest().encode("ascii"))
         login_hash = login_id + md_second.hexdigest() + self._login_key
         sha = sha256()
         sha.update(login_hash.encode("ascii"))
         return sha.hexdigest()
 
-    def set_aes_keys(self, encrypted_key, encrypted_iv):
+    def set_aes_keys(
+        self,
+        encrypted_key: str | bytes,
+        encrypted_iv: str | bytes,
+    ) -> None:
         key_digest = sha256(self._login_key.encode("ascii")).hexdigest()
         tmp_key = key_digest[:16].encode("ascii")
         tmp_iv = key_digest[16:32].encode("ascii")
         self._aes_key = self.aes_decrypt(encrypted_key, tmp_key, tmp_iv).encode("ascii")
         self._aes_iv = self.aes_decrypt(encrypted_iv, tmp_key, tmp_iv).encode("ascii")
 
 
 class MideaAirSecurity(CloudSecurity):
-    def __init__(self, login_key):
+    def __init__(self, login_key: str) -> None:
         super().__init__(login_key, None, None)
 
     def sign(self, url: str, data: Any, random: str) -> str:
         payload = unquote_plus(urlencode(sorted(data.items(), key=lambda x: x[0])))
         sha = sha256()
         sha.update((urlparse(url).path + payload + self._login_key).encode("ascii"))
         return sha.hexdigest()
 
 
 class LocalSecurity:
-    def __init__(self):
-        self.blockSize = 16
+    """Evaluate local security."""
+
+    def __init__(self) -> None:
+        """Initialize security."""
+        self.block_size = 16
         self.iv = b"\0" * 16
         self.aes_key = bytes.fromhex(
-            format(141661095494369103254425781617665632877, "x")
+            format(141661095494369103254425781617665632877, "x"),
         )
         self.salt = bytes.fromhex(
             format(
                 233912452794221312800602098970898185176935770387238278451789080441632479840061417076563,
                 "x",
-            )
+            ),
         )
-        self._tcp_key = None
+        self._tcp_key: bytes
         self._request_count = 0
         self._response_count = 0
 
-    def aes_decrypt(self, raw):
+    def aes_decrypt(self, raw: bytes) -> bytearray:
         try:
-            return unpad(
-                AES.new(self.aes_key, AES.MODE_ECB).decrypt(bytearray(raw)), 16
+            return cast(
+                bytearray,
+                unpad(AES.new(self.aes_key, AES.MODE_ECB).decrypt(bytearray(raw)), 16),
             )
         except ValueError:
             return bytearray(0)
 
-    def aes_encrypt(self, raw):
-        return AES.new(self.aes_key, AES.MODE_ECB).encrypt(bytearray(pad(raw, 16)))
+    def aes_encrypt(self, raw: bytes) -> bytes:
+        return cast(
+            bytes,
+            AES.new(self.aes_key, AES.MODE_ECB).encrypt(bytearray(pad(raw, 16))),
+        )
 
-    def aes_cbc_decrypt(self, raw, key):
-        return AES.new(key=key, mode=AES.MODE_CBC, iv=self.iv).decrypt(raw)
+    def aes_cbc_decrypt(self, raw: bytes, key: Buffer) -> bytes:
+        return cast(bytes, AES.new(key=key, mode=AES.MODE_CBC, iv=self.iv).decrypt(raw))
 
-    def aes_cbc_encrypt(self, raw, key):
-        return AES.new(key=key, mode=AES.MODE_CBC, iv=self.iv).encrypt(raw)
+    def aes_cbc_encrypt(self, raw: bytes, key: Buffer) -> bytes:
+        return cast(bytes, AES.new(key=key, mode=AES.MODE_CBC, iv=self.iv).encrypt(raw))
 
-    def encode32_data(self, raw):
+    def encode32_data(self, raw: bytes) -> bytes:
         return md5(raw + self.salt).digest()
 
-    def tcp_key(self, response, key):
+    def tcp_key(self, response: bytes, key: Buffer) -> bytes:
         if response == b"ERROR":
             raise Exception("authentication failed")
         if len(response) != 64:
             raise Exception("unexpected data length")
         payload = response[:32]
         sign = response[32:]
         plain = self.aes_cbc_decrypt(payload, key)
         if sha256(plain).digest() != sign:
             raise Exception("sign does not match")
         self._tcp_key = strxor(plain, key)
         self._request_count = 0
         self._response_count = 0
         return self._tcp_key
 
-    def encode_8370(self, data, msgtype):
+    def encode_8370(self, data: bytes, msgtype: int) -> bytes:
         header = bytearray([0x83, 0x70])
         size, padding = len(data), 0
         if msgtype in (MSGTYPE_ENCRYPTED_RESPONSE, MSGTYPE_ENCRYPTED_REQUEST):
             if (size + 2) % 16 != 0:
                 padding = 16 - (size + 2 & 0xF)
                 size += padding + 32
                 data += get_random_bytes(padding)
@@ -226,15 +277,15 @@
         if self._request_count >= 0xFFFF:
             self._request_count = 0
         if msgtype in (MSGTYPE_ENCRYPTED_RESPONSE, MSGTYPE_ENCRYPTED_REQUEST):
             sign = sha256(header + data).digest()
             data = self.aes_cbc_encrypt(raw=data, key=self._tcp_key) + sign
         return header + data
 
-    def decode_8370(self, data):
+    def decode_8370(self, data: bytes) -> tuple[list, bytes]:
         if len(data) < 6:
             return [], data
         header = data[:6]
         if header[0] != 0x83 or header[1] != 0x70:
             raise Exception("not an 8370 message")
         size = int.from_bytes(header[2:4], "big") + 8
         leftover = None
```

### Comparing `midea_local-1.0.3/setup.py` & `midea_local-1.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 #!/bin/python
 """setup midea-local."""
 
 import setuptools
 
-with open("README.md", "r", encoding="utf-8") as fh:
+with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 requires = ["aiohttp", "ifaddr", "pycryptodome"]
 
 setuptools.setup(
     name="midea-local",
-    version="1.0.3",
+    version="1.0.4",
     author="rokam",
     author_email="lucas@mindello.com.br",
     description="Control your Midea M-Smart appliances via local area network",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rokam/midea-local",
     install_requires=requires,
     packages=setuptools.find_packages(
-        include=["midealocal", "midealocal.*"], exclude=["tests", "tests.*"]
+        include=["midealocal", "midealocal.*"],
+        exclude=["tests", "tests.*"],
     ),
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

