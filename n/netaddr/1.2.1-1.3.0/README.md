# Comparing `tmp/netaddr-1.2.1.tar.gz` & `tmp/netaddr-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netaddr-1.2.1.tar", last modified: Sat Feb 17 20:38:11 2024, max compression
+gzip compressed data, was "netaddr-1.3.0.tar", last modified: Tue May 28 21:30:28 2024, max compression
```

## Comparing `netaddr-1.2.1.tar` & `netaddr-1.3.0.tar`

### file list

```diff
@@ -1,136 +1,125 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.793505 netaddr-1.2.1/
--rw-r--r--   0 kuba       (501) staff       (20)      241 2024-02-17 18:04:30.000000 netaddr-1.2.1/AUTHORS.rst
--rw-r--r--   0 kuba       (501) staff       (20)    57231 2024-02-17 20:37:32.000000 netaddr-1.2.1/CHANGELOG.rst
--rw-r--r--   0 kuba       (501) staff       (20)     1421 2024-02-17 18:04:30.000000 netaddr-1.2.1/COPYRIGHT.rst
--rw-r--r--   0 kuba       (501) staff       (20)     1630 2024-02-17 18:04:30.000000 netaddr-1.2.1/LICENSE.rst
--rw-r--r--   0 kuba       (501) staff       (20)      830 2024-02-17 18:04:30.000000 netaddr-1.2.1/MANIFEST.in
--rw-r--r--   0 kuba       (501) staff       (20)     2242 2024-02-17 20:32:48.000000 netaddr-1.2.1/Makefile
--rw-r--r--   0 kuba       (501) staff       (20)     5018 2024-02-17 20:38:11.793257 netaddr-1.2.1/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     1455 2024-02-17 20:32:44.000000 netaddr-1.2.1/README.rst
--rw-r--r--   0 kuba       (501) staff       (20)     1644 2024-02-17 18:04:30.000000 netaddr-1.2.1/THANKS.rst
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.757290 netaddr-1.2.1/docs/
--rw-r--r--   0 kuba       (501) staff       (20)     5577 2022-06-15 22:24:04.000000 netaddr-1.2.1/docs/Makefile
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.751875 netaddr-1.2.1/docs/build/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.751920 netaddr-1.2.1/docs/build/html/
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.758139 netaddr-1.2.1/docs/build/html/_static/
--rw-r--r--   0 kuba       (501) staff       (20)    15094 2024-02-17 20:38:10.000000 netaddr-1.2.1/docs/build/html/_static/basic.css
--rw-r--r--   0 kuba       (501) staff       (20)      508 2024-01-03 21:12:28.000000 netaddr-1.2.1/docs/build/html/_static/custom.css
--rw-r--r--   0 kuba       (501) staff       (20)     1266 2024-02-13 16:27:57.000000 netaddr-1.2.1/docs/build/html/_static/debug.css
--rw-r--r--   0 kuba       (501) staff       (20)    20744 2024-02-17 20:38:11.000000 netaddr-1.2.1/docs/build/html/_static/pygments.css
--rw-r--r--   0 kuba       (501) staff       (20)     6034 2024-02-13 16:27:57.000000 netaddr-1.2.1/docs/build/html/_static/skeleton.css
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.758386 netaddr-1.2.1/docs/build/html/_static/styles/
--rw-r--r--   0 kuba       (501) staff       (20)     5529 2024-02-13 16:27:57.000000 netaddr-1.2.1/docs/build/html/_static/styles/furo-extensions.css
--rw-r--r--   0 kuba       (501) staff       (20)    48265 2024-02-13 16:27:57.000000 netaddr-1.2.1/docs/build/html/_static/styles/furo.css
--rw-r--r--   0 kuba       (501) staff       (20)     5107 2022-06-15 22:24:04.000000 netaddr-1.2.1/docs/make.bat
--rw-r--r--   0 kuba       (501) staff       (20)    40542 2024-02-10 09:52:32.000000 netaddr-1.2.1/docs/poetry.lock
--rw-r--r--   0 kuba       (501) staff       (20)      396 2024-02-10 09:52:32.000000 netaddr-1.2.1/docs/pyproject.toml
--rw-r--r--   0 kuba       (501) staff       (20)    18191 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.760200 netaddr-1.2.1/docs/source/
--rw-r--r--   0 kuba       (501) staff       (20)     9072 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/source/api.rst
--rw-r--r--   0 kuba       (501) staff       (20)       56 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/source/authors.rst
--rw-r--r--   0 kuba       (501) staff       (20)       64 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/source/changes.rst
--rw-r--r--   0 kuba       (501) staff       (20)     9062 2024-02-17 20:37:50.000000 netaddr-1.2.1/docs/source/conf.py
--rw-r--r--   0 kuba       (501) staff       (20)       70 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/source/contributors.rst
--rw-r--r--   0 kuba       (501) staff       (20)       64 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/source/copyright.rst
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.760430 netaddr-1.2.1/docs/source/dev-how-to/
--rw-r--r--   0 kuba       (501) staff       (20)       72 2024-01-31 12:06:07.000000 netaddr-1.2.1/docs/source/dev-how-to/index.rst
--rw-r--r--   0 kuba       (501) staff       (20)     1611 2024-02-17 20:09:26.000000 netaddr-1.2.1/docs/source/dev-how-to/release.rst
--rw-r--r--   0 kuba       (501) staff       (20)      176 2024-02-08 00:01:01.000000 netaddr-1.2.1/docs/source/how-to.rst
--rw-r--r--   0 kuba       (501) staff       (20)     1991 2024-02-17 20:18:18.000000 netaddr-1.2.1/docs/source/index.rst
--rw-r--r--   0 kuba       (501) staff       (20)     1817 2024-02-17 19:09:47.000000 netaddr-1.2.1/docs/source/installation.rst
--rw-r--r--   0 kuba       (501) staff       (20)       56 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/source/license.rst
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.760708 netaddr-1.2.1/docs/source/reference/
--rw-r--r--   0 kuba       (501) staff       (20)     2647 2024-02-17 20:33:38.000000 netaddr-1.2.1/docs/source/reference/cli.rst
--rw-r--r--   0 kuba       (501) staff       (20)      566 2024-02-10 01:41:57.000000 netaddr-1.2.1/docs/source/reference/compatibility.rst
--rw-r--r--   0 kuba       (501) staff       (20)      218 2024-02-17 20:17:44.000000 netaddr-1.2.1/docs/source/reference.rst
--rw-r--r--   0 kuba       (501) staff       (20)     2965 2024-01-31 12:06:07.000000 netaddr-1.2.1/docs/source/references.rst
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.760843 netaddr-1.2.1/docs/source/static/
--rw-r--r--   0 kuba       (501) staff       (20)      508 2024-01-03 21:12:28.000000 netaddr-1.2.1/docs/source/static/custom.css
--rw-r--r--   0 kuba       (501) staff       (20)    23432 2024-02-17 18:04:30.000000 netaddr-1.2.1/docs/source/tutorial_01.rst
--rw-r--r--   0 kuba       (501) staff       (20)     5347 2024-02-08 21:43:42.000000 netaddr-1.2.1/docs/source/tutorial_02.rst
--rw-r--r--   0 kuba       (501) staff       (20)    14057 2024-02-09 22:01:12.000000 netaddr-1.2.1/docs/source/tutorial_03.rst
--rw-r--r--   0 kuba       (501) staff       (20)      240 2024-02-08 00:01:01.000000 netaddr-1.2.1/docs/source/tutorials.rst
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.761555 netaddr-1.2.1/netaddr/
--rw-r--r--   0 kuba       (501) staff       (20)     3173 2024-02-17 20:37:41.000000 netaddr-1.2.1/netaddr/__init__.py
--rwxr-xr-x   0 kuba       (501) staff       (20)     3610 2024-02-17 19:09:47.000000 netaddr-1.2.1/netaddr/cli.py
--rw-r--r--   0 kuba       (501) staff       (20)      530 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/compat.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.762662 netaddr-1.2.1/netaddr/contrib/
--rw-r--r--   0 kuba       (501) staff       (20)      569 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/contrib/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     1704 2024-02-10 09:27:55.000000 netaddr-1.2.1/netaddr/contrib/subnet_splitter.py
--rw-r--r--   0 kuba       (501) staff       (20)     5203 2024-02-08 23:12:36.000000 netaddr-1.2.1/netaddr/core.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.769882 netaddr-1.2.1/netaddr/eui/
--rw-r--r--   0 kuba       (501) staff       (20)    25219 2024-02-10 00:11:48.000000 netaddr-1.2.1/netaddr/eui/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)    95466 2024-02-17 19:49:53.000000 netaddr-1.2.1/netaddr/eui/iab.idx
--rw-r--r--   0 kuba       (501) staff       (20)  2453786 2024-02-17 19:12:46.000000 netaddr-1.2.1/netaddr/eui/iab.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)     9158 2024-02-17 19:49:53.000000 netaddr-1.2.1/netaddr/eui/ieee.py
--rw-r--r--   0 kuba       (501) staff       (20)   665453 2024-02-17 19:49:53.000000 netaddr-1.2.1/netaddr/eui/oui.idx
--rw-r--r--   0 kuba       (501) staff       (20)  5699874 2024-02-17 19:12:46.000000 netaddr-1.2.1/netaddr/eui/oui.txt
--rw-r--r--   0 kuba       (501) staff       (20)     8286 2024-02-17 18:04:30.000000 netaddr-1.2.1/netaddr/fbsocket.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.782605 netaddr-1.2.1/netaddr/ip/
--rw-r--r--   0 kuba       (501) staff       (20)    70593 2024-02-17 19:09:47.000000 netaddr-1.2.1/netaddr/ip/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)    10397 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/ip/glob.py
--rwxr-xr-x   0 kuba       (501) staff       (20)    13951 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/ip/iana.py
--rw-r--r--   0 kuba       (501) staff       (20)    76331 2023-12-18 18:30:29.000000 netaddr-1.2.1/netaddr/ip/ipv4-address-space.xml
--rw-r--r--   0 kuba       (501) staff       (20)     9646 2021-07-18 22:59:26.000000 netaddr-1.2.1/netaddr/ip/ipv6-address-space.xml
--rw-r--r--   0 kuba       (501) staff       (20)    14891 2021-07-18 23:22:40.000000 netaddr-1.2.1/netaddr/ip/ipv6-unicast-address-assignments.xml
--rw-r--r--   0 kuba       (501) staff       (20)   175116 2024-02-02 19:45:32.000000 netaddr-1.2.1/netaddr/ip/multicast-addresses.xml
--rw-r--r--   0 kuba       (501) staff       (20)     4018 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/ip/nmap.py
--rw-r--r--   0 kuba       (501) staff       (20)     1905 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/ip/rfc1924.py
--rw-r--r--   0 kuba       (501) staff       (20)    26367 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/ip/sets.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.783219 netaddr-1.2.1/netaddr/strategy/
--rw-r--r--   0 kuba       (501) staff       (20)     7453 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/strategy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     8404 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/strategy/eui48.py
--rw-r--r--   0 kuba       (501) staff       (20)     7495 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/strategy/eui64.py
--rw-r--r--   0 kuba       (501) staff       (20)     8380 2024-02-17 19:09:47.000000 netaddr-1.2.1/netaddr/strategy/ipv4.py
--rw-r--r--   0 kuba       (501) staff       (20)     7707 2024-02-17 19:09:47.000000 netaddr-1.2.1/netaddr/strategy/ipv6.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.783443 netaddr-1.2.1/netaddr/tests/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.2.1/netaddr/tests/__init__.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.783955 netaddr-1.2.1/netaddr/tests/core/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.2.1/netaddr/tests/core/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      707 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/core/test_pubsub.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.785479 netaddr-1.2.1/netaddr/tests/eui/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.2.1/netaddr/tests/eui/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      182 2022-06-15 22:24:05.000000 netaddr-1.2.1/netaddr/tests/eui/sample_iab.txt
--rw-r--r--   0 kuba       (501) staff       (20)      139 2022-06-15 22:24:05.000000 netaddr-1.2.1/netaddr/tests/eui/sample_oui.txt
--rw-r--r--   0 kuba       (501) staff       (20)     9838 2024-02-10 00:11:48.000000 netaddr-1.2.1/netaddr/tests/eui/test_eui.py
--rw-r--r--   0 kuba       (501) staff       (20)      763 2024-02-08 21:43:42.000000 netaddr-1.2.1/netaddr/tests/eui/test_ieee_parsers.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.791731 netaddr-1.2.1/netaddr/tests/ip/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.2.1/netaddr/tests/ip/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     7574 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_cidr_v4.py
--rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_cidr_v6.py
--rw-r--r--   0 kuba       (501) staff       (20)      320 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_dns.py
--rw-r--r--   0 kuba       (501) staff       (20)      625 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip.py
--rw-r--r--   0 kuba       (501) staff       (20)     4140 2024-02-10 00:11:48.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_categories.py
--rw-r--r--   0 kuba       (501) staff       (20)     1419 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_comparisons.py
--rw-r--r--   0 kuba       (501) staff       (20)     2141 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_globs.py
--rw-r--r--   0 kuba       (501) staff       (20)      547 2024-02-10 00:11:48.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_network_categories.py
--rw-r--r--   0 kuba       (501) staff       (20)     8778 2024-02-14 21:12:08.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_ranges.py
--rw-r--r--   0 kuba       (501) staff       (20)      512 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_rfc1924.py
--rw-r--r--   0 kuba       (501) staff       (20)    23222 2024-02-09 22:01:12.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_sets.py
--rw-r--r--   0 kuba       (501) staff       (20)     2268 2024-02-10 09:27:55.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_splitter.py
--rw-r--r--   0 kuba       (501) staff       (20)    14949 2024-02-17 18:04:30.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_v4.py
--rw-r--r--   0 kuba       (501) staff       (20)     1248 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_v4_v6_conversions.py
--rw-r--r--   0 kuba       (501) staff       (20)     5981 2024-02-08 21:43:42.000000 netaddr-1.2.1/netaddr/tests/ip/test_ip_v6.py
--rw-r--r--   0 kuba       (501) staff       (20)     2422 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_network_ops.py
--rw-r--r--   0 kuba       (501) staff       (20)     3710 2024-02-08 00:01:01.000000 netaddr-1.2.1/netaddr/tests/ip/test_nmap.py
--rw-r--r--   0 kuba       (501) staff       (20)     6527 2024-02-07 23:18:47.000000 netaddr-1.2.1/netaddr/tests/ip/test_old_specs.py
--rw-r--r--   0 kuba       (501) staff       (20)     5419 2024-02-08 22:42:29.000000 netaddr-1.2.1/netaddr/tests/ip/test_platform_osx.py
--rw-r--r--   0 kuba       (501) staff       (20)     1514 2024-02-17 18:04:30.000000 netaddr-1.2.1/netaddr/tests/ip/test_socket_module_fallback.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.792481 netaddr-1.2.1/netaddr/tests/strategy/
--rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.2.1/netaddr/tests/strategy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)     1382 2024-02-08 21:43:42.000000 netaddr-1.2.1/netaddr/tests/strategy/test_eui48_strategy.py
--rw-r--r--   0 kuba       (501) staff       (20)     2911 2024-02-17 19:09:47.000000 netaddr-1.2.1/netaddr/tests/strategy/test_ipv4_strategy.py
--rw-r--r--   0 kuba       (501) staff       (20)     5437 2024-02-17 19:09:47.000000 netaddr-1.2.1/netaddr/tests/strategy/test_ipv6_strategy.py
--rw-r--r--   0 kuba       (501) staff       (20)      285 2024-02-07 23:18:47.000000 netaddr-1.2.1/netaddr/tests/test_netaddr.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-02-17 20:38:11.792841 netaddr-1.2.1/netaddr.egg-info/
--rw-r--r--   0 kuba       (501) staff       (20)     5018 2024-02-17 20:38:11.000000 netaddr-1.2.1/netaddr.egg-info/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     3161 2024-02-17 20:38:11.000000 netaddr-1.2.1/netaddr.egg-info/SOURCES.txt
--rw-r--r--   0 kuba       (501) staff       (20)        1 2024-02-17 20:38:11.000000 netaddr-1.2.1/netaddr.egg-info/dependency_links.txt
--rw-r--r--   0 kuba       (501) staff       (20)       45 2024-02-17 20:38:11.000000 netaddr-1.2.1/netaddr.egg-info/entry_points.txt
--rw-r--r--   0 kuba       (501) staff       (20)       23 2024-02-17 20:38:11.000000 netaddr-1.2.1/netaddr.egg-info/requires.txt
--rw-r--r--   0 kuba       (501) staff       (20)        8 2024-02-17 20:38:11.000000 netaddr-1.2.1/netaddr.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)     3838 2024-02-17 19:09:47.000000 netaddr-1.2.1/pyproject.toml
--rw-r--r--   0 kuba       (501) staff       (20)       60 2024-02-08 22:42:29.000000 netaddr-1.2.1/pytest.ini
--rw-r--r--   0 kuba       (501) staff       (20)       93 2024-02-17 18:04:30.000000 netaddr-1.2.1/requirements-dev.in
--rw-r--r--   0 kuba       (501) staff       (20)      143 2024-02-17 18:04:30.000000 netaddr-1.2.1/requirements-dev.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2024-02-17 20:38:11.793547 netaddr-1.2.1/setup.cfg
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.990863 netaddr-1.3.0/
+-rw-r--r--   0 kuba       (501) staff       (20)      241 2024-05-20 22:42:51.000000 netaddr-1.3.0/AUTHORS.rst
+-rw-r--r--   0 kuba       (501) staff       (20)    57646 2024-05-28 21:16:50.000000 netaddr-1.3.0/CHANGELOG.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     1421 2024-05-20 22:42:51.000000 netaddr-1.3.0/COPYRIGHT.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     1630 2024-05-20 22:42:51.000000 netaddr-1.3.0/LICENSE.rst
+-rw-r--r--   0 kuba       (501) staff       (20)      830 2024-05-20 22:42:51.000000 netaddr-1.3.0/MANIFEST.in
+-rw-r--r--   0 kuba       (501) staff       (20)     2242 2024-05-20 22:42:51.000000 netaddr-1.3.0/Makefile
+-rw-r--r--   0 kuba       (501) staff       (20)     5018 2024-05-28 21:30:28.990602 netaddr-1.3.0/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     1455 2024-05-20 22:42:51.000000 netaddr-1.3.0/README.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     1644 2024-05-20 22:42:51.000000 netaddr-1.3.0/THANKS.rst
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.972829 netaddr-1.3.0/docs/
+-rw-r--r--   0 kuba       (501) staff       (20)     5577 2022-06-15 22:24:04.000000 netaddr-1.3.0/docs/Makefile
+-rw-r--r--   0 kuba       (501) staff       (20)     5107 2022-06-15 22:24:04.000000 netaddr-1.3.0/docs/make.bat
+-rw-r--r--   0 kuba       (501) staff       (20)    42134 2024-05-27 23:13:27.000000 netaddr-1.3.0/docs/poetry.lock
+-rw-r--r--   0 kuba       (501) staff       (20)      396 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/pyproject.toml
+-rw-r--r--   0 kuba       (501) staff       (20)    19041 2024-05-27 23:13:50.000000 netaddr-1.3.0/docs/requirements.txt
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.975065 netaddr-1.3.0/docs/source/
+-rw-r--r--   0 kuba       (501) staff       (20)     9072 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/api.rst
+-rw-r--r--   0 kuba       (501) staff       (20)       56 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/authors.rst
+-rw-r--r--   0 kuba       (501) staff       (20)       64 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/changes.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     9062 2024-05-28 21:20:29.000000 netaddr-1.3.0/docs/source/conf.py
+-rw-r--r--   0 kuba       (501) staff       (20)       70 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/contributors.rst
+-rw-r--r--   0 kuba       (501) staff       (20)       64 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/copyright.rst
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.975352 netaddr-1.3.0/docs/source/dev-how-to/
+-rw-r--r--   0 kuba       (501) staff       (20)       72 2024-01-31 12:06:07.000000 netaddr-1.3.0/docs/source/dev-how-to/index.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     1611 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/dev-how-to/release.rst
+-rw-r--r--   0 kuba       (501) staff       (20)      176 2024-02-08 00:01:01.000000 netaddr-1.3.0/docs/source/how-to.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     1991 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/index.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     1817 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/installation.rst
+-rw-r--r--   0 kuba       (501) staff       (20)       56 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/license.rst
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.975649 netaddr-1.3.0/docs/source/reference/
+-rw-r--r--   0 kuba       (501) staff       (20)     2647 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/reference/cli.rst
+-rw-r--r--   0 kuba       (501) staff       (20)      566 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/reference/compatibility.rst
+-rw-r--r--   0 kuba       (501) staff       (20)      218 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/reference.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     2965 2024-01-31 12:06:07.000000 netaddr-1.3.0/docs/source/references.rst
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.975781 netaddr-1.3.0/docs/source/static/
+-rw-r--r--   0 kuba       (501) staff       (20)      508 2024-01-03 21:12:28.000000 netaddr-1.3.0/docs/source/static/custom.css
+-rw-r--r--   0 kuba       (501) staff       (20)    23504 2024-05-26 23:53:14.000000 netaddr-1.3.0/docs/source/tutorial_01.rst
+-rw-r--r--   0 kuba       (501) staff       (20)     5347 2024-05-20 22:42:51.000000 netaddr-1.3.0/docs/source/tutorial_02.rst
+-rw-r--r--   0 kuba       (501) staff       (20)    14237 2024-05-26 23:53:14.000000 netaddr-1.3.0/docs/source/tutorial_03.rst
+-rw-r--r--   0 kuba       (501) staff       (20)      240 2024-02-08 00:01:01.000000 netaddr-1.3.0/docs/source/tutorials.rst
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.976445 netaddr-1.3.0/netaddr/
+-rw-r--r--   0 kuba       (501) staff       (20)     3173 2024-05-28 21:17:59.000000 netaddr-1.3.0/netaddr/__init__.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)     3610 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/cli.py
+-rw-r--r--   0 kuba       (501) staff       (20)      530 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/compat.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.977327 netaddr-1.3.0/netaddr/contrib/
+-rw-r--r--   0 kuba       (501) staff       (20)      569 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/contrib/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1704 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/contrib/subnet_splitter.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5203 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/core.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.979852 netaddr-1.3.0/netaddr/eui/
+-rw-r--r--   0 kuba       (501) staff       (20)    25219 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/eui/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)    95466 2024-02-17 19:49:53.000000 netaddr-1.3.0/netaddr/eui/iab.idx
+-rw-r--r--   0 kuba       (501) staff       (20)  2453786 2024-02-17 19:12:46.000000 netaddr-1.3.0/netaddr/eui/iab.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)     9158 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/eui/ieee.py
+-rw-r--r--   0 kuba       (501) staff       (20)   665453 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/eui/oui.idx
+-rw-r--r--   0 kuba       (501) staff       (20)  5699874 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/eui/oui.txt
+-rw-r--r--   0 kuba       (501) staff       (20)     8286 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/fbsocket.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.984647 netaddr-1.3.0/netaddr/ip/
+-rw-r--r--   0 kuba       (501) staff       (20)    71337 2024-05-28 21:16:35.000000 netaddr-1.3.0/netaddr/ip/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)    10397 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/ip/glob.py
+-rwxr-xr-x   0 kuba       (501) staff       (20)    13951 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/ip/iana.py
+-rw-r--r--   0 kuba       (501) staff       (20)    76331 2023-12-18 18:30:29.000000 netaddr-1.3.0/netaddr/ip/ipv4-address-space.xml
+-rw-r--r--   0 kuba       (501) staff       (20)     9646 2021-07-18 22:59:26.000000 netaddr-1.3.0/netaddr/ip/ipv6-address-space.xml
+-rw-r--r--   0 kuba       (501) staff       (20)    14891 2021-07-18 23:22:40.000000 netaddr-1.3.0/netaddr/ip/ipv6-unicast-address-assignments.xml
+-rw-r--r--   0 kuba       (501) staff       (20)   175116 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/ip/multicast-addresses.xml
+-rw-r--r--   0 kuba       (501) staff       (20)     4018 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/ip/nmap.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1905 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/ip/rfc1924.py
+-rw-r--r--   0 kuba       (501) staff       (20)    26367 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/ip/sets.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.985339 netaddr-1.3.0/netaddr/strategy/
+-rw-r--r--   0 kuba       (501) staff       (20)     7453 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/strategy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     8404 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/strategy/eui48.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7495 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/strategy/eui64.py
+-rw-r--r--   0 kuba       (501) staff       (20)     8420 2024-05-22 23:29:14.000000 netaddr-1.3.0/netaddr/strategy/ipv4.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7707 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/strategy/ipv6.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.985618 netaddr-1.3.0/netaddr/tests/
+-rw-r--r--   0 kuba       (501) staff       (20)      199 2024-05-26 23:53:14.000000 netaddr-1.3.0/netaddr/tests/__init__.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.985869 netaddr-1.3.0/netaddr/tests/core/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.3.0/netaddr/tests/core/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      707 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/core/test_pubsub.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.986567 netaddr-1.3.0/netaddr/tests/eui/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.3.0/netaddr/tests/eui/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      182 2022-06-15 22:24:05.000000 netaddr-1.3.0/netaddr/tests/eui/sample_iab.txt
+-rw-r--r--   0 kuba       (501) staff       (20)      139 2022-06-15 22:24:05.000000 netaddr-1.3.0/netaddr/tests/eui/sample_oui.txt
+-rw-r--r--   0 kuba       (501) staff       (20)     9838 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/eui/test_eui.py
+-rw-r--r--   0 kuba       (501) staff       (20)      763 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/eui/test_ieee_parsers.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.989430 netaddr-1.3.0/netaddr/tests/ip/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.3.0/netaddr/tests/ip/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7574 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_cidr_v4.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4673 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_cidr_v6.py
+-rw-r--r--   0 kuba       (501) staff       (20)      320 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_dns.py
+-rw-r--r--   0 kuba       (501) staff       (20)      625 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4140 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_categories.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1419 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_comparisons.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2141 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_globs.py
+-rw-r--r--   0 kuba       (501) staff       (20)      547 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_network_categories.py
+-rw-r--r--   0 kuba       (501) staff       (20)     8778 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_ranges.py
+-rw-r--r--   0 kuba       (501) staff       (20)      512 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_rfc1924.py
+-rw-r--r--   0 kuba       (501) staff       (20)    23222 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_sets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2268 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_splitter.py
+-rw-r--r--   0 kuba       (501) staff       (20)    15431 2024-05-27 23:32:01.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_v4.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1248 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_v4_v6_conversions.py
+-rw-r--r--   0 kuba       (501) staff       (20)     6097 2024-05-22 23:29:14.000000 netaddr-1.3.0/netaddr/tests/ip/test_ip_v6.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2422 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_network_ops.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3710 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_nmap.py
+-rw-r--r--   0 kuba       (501) staff       (20)     6527 2024-02-07 23:18:47.000000 netaddr-1.3.0/netaddr/tests/ip/test_old_specs.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5419 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_platform_osx.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1514 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/ip/test_socket_module_fallback.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.989937 netaddr-1.3.0/netaddr/tests/strategy/
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2024-01-13 12:25:38.000000 netaddr-1.3.0/netaddr/tests/strategy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1382 2024-05-20 22:42:51.000000 netaddr-1.3.0/netaddr/tests/strategy/test_eui48_strategy.py
+-rw-r--r--   0 kuba       (501) staff       (20)     3074 2024-05-22 23:29:14.000000 netaddr-1.3.0/netaddr/tests/strategy/test_ipv4_strategy.py
+-rw-r--r--   0 kuba       (501) staff       (20)     5730 2024-05-26 23:53:14.000000 netaddr-1.3.0/netaddr/tests/strategy/test_ipv6_strategy.py
+-rw-r--r--   0 kuba       (501) staff       (20)      285 2024-02-07 23:18:47.000000 netaddr-1.3.0/netaddr/tests/test_netaddr.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2024-05-28 21:30:28.990150 netaddr-1.3.0/netaddr.egg-info/
+-rw-r--r--   0 kuba       (501) staff       (20)     5018 2024-05-28 21:30:28.000000 netaddr-1.3.0/netaddr.egg-info/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     2893 2024-05-28 21:30:28.000000 netaddr-1.3.0/netaddr.egg-info/SOURCES.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        1 2024-05-28 21:30:28.000000 netaddr-1.3.0/netaddr.egg-info/dependency_links.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       45 2024-05-28 21:30:28.000000 netaddr-1.3.0/netaddr.egg-info/entry_points.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       23 2024-05-28 21:30:28.000000 netaddr-1.3.0/netaddr.egg-info/requires.txt
+-rw-r--r--   0 kuba       (501) staff       (20)        8 2024-05-28 21:30:28.000000 netaddr-1.3.0/netaddr.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)     3838 2024-05-20 22:42:51.000000 netaddr-1.3.0/pyproject.toml
+-rw-r--r--   0 kuba       (501) staff       (20)       60 2024-05-20 22:42:51.000000 netaddr-1.3.0/pytest.ini
+-rw-r--r--   0 kuba       (501) staff       (20)      103 2024-05-26 23:53:14.000000 netaddr-1.3.0/requirements-dev.in
+-rw-r--r--   0 kuba       (501) staff       (20)      143 2024-05-22 23:34:34.000000 netaddr-1.3.0/requirements-dev.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2024-05-28 21:30:28.990903 netaddr-1.3.0/setup.cfg
```

### Comparing `netaddr-1.2.1/CHANGELOG.rst` & `netaddr-1.3.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,31 @@
 --------------------
 NEXT_NETADDR_VERSION
 --------------------
 
 Date: not released yet
 
 --------------
+Release: 1.3.0
+--------------
+
+Date: 2024-05-28
+
+Added:
+
+* Add partial address expansion in :class:`IPNetwork` via the ``expand_partial`` switch,
+  this enables opting into pre-1.1.0 behavior
+
+Fixed:
+
+* Fix running the test suite on musl systems
+* Fix :class:`IPAddress` IPv6 parsing with :data:`ZEROFILL` enabled
+* Fix handling of the :data:`NOHOST` flag in the :class:`IPNetwork` copy constructor
+
+--------------
 Release: 1.2.1
 --------------
 
 Date: 2024-02-17
 
 Fixed:
```

### Comparing `netaddr-1.2.1/COPYRIGHT.rst` & `netaddr-1.3.0/COPYRIGHT.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/LICENSE.rst` & `netaddr-1.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/MANIFEST.in` & `netaddr-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/Makefile` & `netaddr-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/PKG-INFO` & `netaddr-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netaddr
-Version: 1.2.1
+Version: 1.3.0
 Summary: A network address manipulation library for Python
 Author-email: "David P. D. Moss" <josiah_carberry@brown.edu>, Stefan Nordhausen <stefan.nordhausen@immobilienscout24.de>
 Maintainer-email: Jakub Stasiak <jakub@stasiak.at>
 License: BSD License
 Project-URL: Documentation, https://netaddr.readthedocs.io/en/latest/
 Project-URL: Download, https://pypi.org/project/netaddr/
 Project-URL: Repository, https://github.com/netaddr/netaddr/
```

### Comparing `netaddr-1.2.1/README.rst` & `netaddr-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/THANKS.rst` & `netaddr-1.3.0/THANKS.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/Makefile` & `netaddr-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/make.bat` & `netaddr-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/poetry.lock` & `netaddr-1.3.0/docs/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is automatically @generated by Poetry 1.7.1 and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.8.2 and should not be changed by hand.
 
 [[package]]
 name = "alabaster"
 version = "0.7.13"
 description = "A configurable sidebar-enabled Sphinx theme"
 optional = false
 python-versions = ">=3.6"
@@ -190,21 +190,21 @@
 beautifulsoup4 = "*"
 pygments = ">=2.7"
 sphinx = ">=6.0,<8.0"
 sphinx-basic-ng = "*"
 
 [[package]]
 name = "idna"
-version = "3.6"
+version = "3.7"
 description = "Internationalized Domain Names in Applications (IDNA)"
 optional = false
 python-versions = ">=3.5"
 files = [
-    {file = "idna-3.6-py3-none-any.whl", hash = "sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f"},
-    {file = "idna-3.6.tar.gz", hash = "sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca"},
+    {file = "idna-3.7-py3-none-any.whl", hash = "sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0"},
+    {file = "idna-3.7.tar.gz", hash = "sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc"},
 ]
 
 [[package]]
 name = "imagesize"
 version = "1.4.1"
 description = "Getting image size from png/jpeg/jpeg2000/gif file"
 optional = false
@@ -212,21 +212,21 @@
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "jinja2"
-version = "3.1.3"
+version = "3.1.4"
 description = "A very fast and expressive template engine."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "Jinja2-3.1.3-py3-none-any.whl", hash = "sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa"},
-    {file = "Jinja2-3.1.3.tar.gz", hash = "sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90"},
+    {file = "jinja2-3.1.4-py3-none-any.whl", hash = "sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d"},
+    {file = "jinja2-3.1.4.tar.gz", hash = "sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369"},
 ]
 
 [package.dependencies]
 MarkupSafe = ">=2.0"
 
 [package.extras]
 i18n = ["Babel (>=2.7)"]
@@ -269,14 +269,24 @@
     {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2"},
     {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9"},
     {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc"},
     {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9"},
     {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac"},
     {file = "MarkupSafe-2.1.3-cp311-cp311-win32.whl", hash = "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb"},
     {file = "MarkupSafe-2.1.3-cp311-cp311-win_amd64.whl", hash = "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-win32.whl", hash = "sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007"},
+    {file = "MarkupSafe-2.1.3-cp312-cp312-win_amd64.whl", hash = "sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb"},
     {file = "MarkupSafe-2.1.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2"},
     {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b"},
     {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707"},
     {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e"},
     {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc"},
     {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48"},
     {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155"},
@@ -329,21 +339,21 @@
 
 [package.extras]
 plugins = ["importlib-metadata"]
 windows-terminal = ["colorama (>=0.4.6)"]
 
 [[package]]
 name = "requests"
-version = "2.31.0"
+version = "2.32.2"
 description = "Python HTTP for Humans."
 optional = false
-python-versions = ">=3.7"
+python-versions = ">=3.8"
 files = [
-    {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
-    {file = "requests-2.31.0.tar.gz", hash = "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"},
+    {file = "requests-2.32.2-py3-none-any.whl", hash = "sha256:fc06670dd0ed212426dfeb94fc1b983d917c4f9847c863f313c9dfaaffb7c23c"},
+    {file = "requests-2.32.2.tar.gz", hash = "sha256:dd951ff5ecf3e3b3aa26b40703ba77495dab41da839ae72ef3c8e5d8e2433289"},
 ]
 
 [package.dependencies]
 certifi = ">=2017.4.17"
 charset-normalizer = ">=2,<4"
 idna = ">=2.5,<4"
 urllib3 = ">=1.21.1,<3"
```

### Comparing `netaddr-1.2.1/docs/requirements.txt` & `netaddr-1.3.0/docs/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -106,55 +106,63 @@
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 docutils==0.20.1 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
     --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
 furo==2023.9.10 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:513092538537dc5c596691da06e3c370714ec99bc438680edc1debffb73e5bfc \
     --hash=sha256:5707530a476d2a63b8cad83b4f961f3739a69f4b058bcf38a03a39fa537195b2
-idna==3.6 ; python_version >= "3.10" and python_version < "4.0" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 ; python_version >= "3.10" and python_version < "4.0" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
 imagesize==1.4.1 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b \
     --hash=sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a
-jinja2==3.1.3 ; python_version >= "3.10" and python_version < "4.0" \
-    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
-    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+jinja2==3.1.4 ; python_version >= "3.10" and python_version < "4.0" \
+    --hash=sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369 \
+    --hash=sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d
 markupsafe==2.1.3 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
     --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
     --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
     --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
+    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
     --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
     --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
+    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
+    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
     --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
     --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
     --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
     --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
     --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
     --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
     --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
+    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
     --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
     --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
     --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
     --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
     --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
     --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
     --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
     --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
+    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
     --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
     --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
     --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
     --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
     --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
     --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
     --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
+    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
     --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
     --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
+    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
     --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
+    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
     --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
     --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
     --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
     --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
     --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
     --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
     --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
@@ -165,24 +173,26 @@
     --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
     --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
     --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
     --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
     --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
     --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
     --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2
+    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
+    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
+    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
 packaging==23.2 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
     --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
 pygments==2.17.2 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
     --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-requests==2.31.0 ; python_version >= "3.10" and python_version < "4.0" \
-    --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
-    --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
+requests==2.32.2 ; python_version >= "3.10" and python_version < "4.0" \
+    --hash=sha256:dd951ff5ecf3e3b3aa26b40703ba77495dab41da839ae72ef3c8e5d8e2433289 \
+    --hash=sha256:fc06670dd0ed212426dfeb94fc1b983d917c4f9847c863f313c9dfaaffb7c23c
 snowballstemmer==2.2.0 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
 soupsieve==2.5 ; python_version >= "3.10" and python_version < "4.0" \
     --hash=sha256:5663d5a7b3bfaeee0bc4372e7fc48f9cff4940b3eec54a6451cc5299f1097690 \
     --hash=sha256:eaa337ff55a1579b6549dc679565eac1e3d000563bcb1c8ab0d0fefbc0c2cdc7
 sphinx-basic-ng==1.0.0b2 ; python_version >= "3.10" and python_version < "4.0" \
```

### Comparing `netaddr-1.2.1/docs/source/api.rst` & `netaddr-1.3.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/conf.py` & `netaddr-1.3.0/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 copyright = '2008 David P. D. Moss, 2020 netaddr contributors'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.2.1'
+version = '1.3.0'
 # The full version, including alpha/beta/rc tags.
-release = '1.2.1'
+release = '1.3.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `netaddr-1.2.1/docs/source/dev-how-to/release.rst` & `netaddr-1.3.0/docs/source/dev-how-to/release.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/index.rst` & `netaddr-1.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/installation.rst` & `netaddr-1.3.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/reference/cli.rst` & `netaddr-1.3.0/docs/source/reference/cli.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/reference/compatibility.rst` & `netaddr-1.3.0/docs/source/reference/compatibility.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/references.rst` & `netaddr-1.3.0/docs/source/references.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/tutorial_01.rst` & `netaddr-1.3.0/docs/source/tutorial_01.rst`

 * *Files 2% similar despite different names*

```diff
@@ -194,35 +194,35 @@
 >>> ip
 IPAddress('::ffff:192.0.2.15')
 >>> ip.is_ipv4_mapped()
 True
 >>> ip.is_ipv4_compat()
 False
 
->>> IPAddress('192.0.2.15').ipv6(ipv4_compatible=True)
+>>> IPAddress('192.0.2.15').ipv6(ipv4_compatible=True)  # doctest: +SKIP
 IPAddress('::192.0.2.15')
 >>> IPAddress('192.0.2.15').ipv6(ipv4_compatible=True).is_ipv4_compat()
 True
->>> IPAddress('192.0.2.15').ipv6(True)
+>>> IPAddress('192.0.2.15').ipv6(True)  # doctest: +SKIP
 IPAddress('::192.0.2.15')
 >>> ip = IPNetwork('192.0.2.1/23')
 >>> ip.ipv4()
 IPNetwork('192.0.2.1/23')
 >>> ip.ipv6()
 IPNetwork('::ffff:192.0.2.1/119')
->>> ip.ipv6(ipv4_compatible=True)
+>>> ip.ipv6(ipv4_compatible=True)  # doctest: +SKIP
 IPNetwork('::192.0.2.1/119')
 
 ^^^^^^^^^^^^^^^^^^^^^^^
 IPv6 to IPv4 conversion
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 >>> IPNetwork('::ffff:192.0.2.1/119').ipv6()
 IPNetwork('::ffff:192.0.2.1/119')
->>> IPNetwork('::ffff:192.0.2.1/119').ipv6(ipv4_compatible=True)
+>>> IPNetwork('::ffff:192.0.2.1/119').ipv6(ipv4_compatible=True)  # doctest: +SKIP
 IPNetwork('::192.0.2.1/119')
 >>> IPNetwork('::ffff:192.0.2.1/119').ipv4()
 IPNetwork('192.0.2.1/23')
 >>> IPNetwork('::192.0.2.1/119').ipv4()
 IPNetwork('192.0.2.1/23')
 
 Note that the IP object returns IPv4 "mapped" addresses by default in preference to IPv4 "compatible" ones. This has been chosen purposefully as the latter form has been deprecated (see RFC 4291 for details).
```

### Comparing `netaddr-1.2.1/docs/source/tutorial_02.rst` & `netaddr-1.3.0/docs/source/tutorial_02.rst`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/docs/source/tutorial_03.rst` & `netaddr-1.3.0/docs/source/tutorial_03.rst`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 >>> IPSet(IPRange("10.0.0.0", "10.0.1.31"))
 IPSet(['10.0.0.0/24', '10.0.1.0/27'])
 >>> IPSet(IPRange('0.0.0.0', '255.255.255.255'))
 IPSet(['0.0.0.0/0'])
 
 You can iterate over all the IP addresses that are members of the IP set.
 
->>> for ip in IPSet(['192.0.2.0/28', '::192.0.2.0/124']):
+>>> for ip in IPSet(['192.0.2.0/28', '::ffff:192.0.2.0/124']):
 ...     print(ip)
 192.0.2.0
 192.0.2.1
 192.0.2.2
 192.0.2.3
 192.0.2.4
 192.0.2.5
@@ -59,30 +59,30 @@
 192.0.2.9
 192.0.2.10
 192.0.2.11
 192.0.2.12
 192.0.2.13
 192.0.2.14
 192.0.2.15
-::192.0.2.0
-::192.0.2.1
-::192.0.2.2
-::192.0.2.3
-::192.0.2.4
-::192.0.2.5
-::192.0.2.6
-::192.0.2.7
-::192.0.2.8
-::192.0.2.9
-::192.0.2.10
-::192.0.2.11
-::192.0.2.12
-::192.0.2.13
-::192.0.2.14
-::192.0.2.15
+::ffff:192.0.2.0
+::ffff:192.0.2.1
+::ffff:192.0.2.2
+::ffff:192.0.2.3
+::ffff:192.0.2.4
+::ffff:192.0.2.5
+::ffff:192.0.2.6
+::ffff:192.0.2.7
+::ffff:192.0.2.8
+::ffff:192.0.2.9
+::ffff:192.0.2.10
+::ffff:192.0.2.11
+::ffff:192.0.2.12
+::ffff:192.0.2.13
+::ffff:192.0.2.14
+::ffff:192.0.2.15
 
 --------------------------------
 Adding and removing set elements
 --------------------------------
 
 >>> s1 = IPSet()
 >>> s1.add('192.0.2.0')
@@ -299,53 +299,53 @@
 
 ------------------------------
 Combined IPv4 and IPv6 support
 ------------------------------
 
 In keeping with netaddr's pragmatic approach, you are free to mix and match IPv4 and IPv6 within the same data structure.
 
->>> s1 = IPSet(['192.0.2.0', '::192.0.2.0', '192.0.2.2', '::192.0.2.2'])
->>> s2 = IPSet(['192.0.2.2', '::192.0.2.2', '192.0.2.4', '::192.0.2.4'])
+>>> s1 = IPSet(['192.0.2.0', '::ffff:192.0.2.0', '192.0.2.2', '::ffff:192.0.2.2'])
+>>> s2 = IPSet(['192.0.2.2', '::ffff:192.0.2.2', '192.0.2.4', '::ffff:192.0.2.4'])
 
 >>> s1
-IPSet(['192.0.2.0/32', '192.0.2.2/32', '::192.0.2.0/128', '::192.0.2.2/128'])
+IPSet(['192.0.2.0/32', '192.0.2.2/32', '::ffff:192.0.2.0/128', '::ffff:192.0.2.2/128'])
 >>> s2
-IPSet(['192.0.2.2/32', '192.0.2.4/32', '::192.0.2.2/128', '::192.0.2.4/128'])
+IPSet(['192.0.2.2/32', '192.0.2.4/32', '::ffff:192.0.2.2/128', '::ffff:192.0.2.4/128'])
 
 ^^^^^^^^^^^^^^^^^^^^^^^
 IPv4 and IPv6 set union
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 >>> s1 | s2
-IPSet(['192.0.2.0/32', '192.0.2.2/32', '192.0.2.4/32', '::192.0.2.0/128', '::192.0.2.2/128', '::192.0.2.4/128'])
+IPSet(['192.0.2.0/32', '192.0.2.2/32', '192.0.2.4/32', '::ffff:192.0.2.0/128', '::ffff:192.0.2.2/128', '::ffff:192.0.2.4/128'])
 >>> s2 | s1
-IPSet(['192.0.2.0/32', '192.0.2.2/32', '192.0.2.4/32', '::192.0.2.0/128', '::192.0.2.2/128', '::192.0.2.4/128'])
+IPSet(['192.0.2.0/32', '192.0.2.2/32', '192.0.2.4/32', '::ffff:192.0.2.0/128', '::ffff:192.0.2.2/128', '::ffff:192.0.2.4/128'])
 
 ^^^^^^^^^^^^^^^^
 set intersection
 ^^^^^^^^^^^^^^^^
 
 >>> s1 & s2
-IPSet(['192.0.2.2/32', '::192.0.2.2/128'])
+IPSet(['192.0.2.2/32', '::ffff:192.0.2.2/128'])
 
 ^^^^^^^^^^^^^^
 set difference
 ^^^^^^^^^^^^^^
 
 >>> s1 - s2
-IPSet(['192.0.2.0/32', '::192.0.2.0/128'])
+IPSet(['192.0.2.0/32', '::ffff:192.0.2.0/128'])
 >>> s2 - s1
-IPSet(['192.0.2.4/32', '::192.0.2.4/128'])
+IPSet(['192.0.2.4/32', '::ffff:192.0.2.4/128'])
 
 ^^^^^^^^^^^^^^^^^^^^^^^^
 set symmetric difference
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
 >>> s1 ^ s2
-IPSet(['192.0.2.0/32', '192.0.2.4/32', '::192.0.2.0/128', '::192.0.2.4/128'])
+IPSet(['192.0.2.0/32', '192.0.2.4/32', '::ffff:192.0.2.0/128', '::ffff:192.0.2.4/128'])
 
 ------------------
 Disjointed IP sets
 ------------------
 
 >>> s1 = IPSet(['192.0.2.0', '192.0.2.1', '192.0.2.2'])
 >>> s2 = IPSet(['192.0.2.2', '192.0.2.3', '192.0.2.4'])
```

### Comparing `netaddr-1.2.1/netaddr/__init__.py` & `netaddr-1.3.0/netaddr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #   Copyright (c) 2008 by David P. D. Moss. All rights reserved.
 #
 #   Released under the BSD license. See the LICENSE file for details.
 # -----------------------------------------------------------------------------
 """A Python library for manipulating IP and EUI network addresses."""
 
 #: Version info (major, minor, maintenance, status)
-__version__ = '1.2.1'
+__version__ = '1.3.0'
 VERSION = tuple(int(part) for part in __version__.split('.'))
 STATUS = ''
 
 import sys as _sys
 
 if _sys.version_info[0:2] < (3, 7):
     raise RuntimeError('Python 3.7.0 or higher is required!')
```

### Comparing `netaddr-1.2.1/netaddr/cli.py` & `netaddr-1.3.0/netaddr/cli.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/compat.py` & `netaddr-1.3.0/netaddr/compat.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/contrib/__init__.py` & `netaddr-1.3.0/netaddr/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/contrib/subnet_splitter.py` & `netaddr-1.3.0/netaddr/contrib/subnet_splitter.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/core.py` & `netaddr-1.3.0/netaddr/core.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/eui/__init__.py` & `netaddr-1.3.0/netaddr/eui/__init__.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/eui/iab.idx` & `netaddr-1.3.0/netaddr/eui/iab.idx`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/eui/iab.txt` & `netaddr-1.3.0/netaddr/eui/iab.txt`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/eui/ieee.py` & `netaddr-1.3.0/netaddr/eui/ieee.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/eui/oui.idx` & `netaddr-1.3.0/netaddr/eui/oui.idx`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/eui/oui.txt` & `netaddr-1.3.0/netaddr/eui/oui.txt`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/fbsocket.py` & `netaddr-1.3.0/netaddr/fbsocket.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/__init__.py` & `netaddr-1.3.0/netaddr/ip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,22 +191,22 @@
             for cidr in IPV6_RESERVED:
                 if self in cidr:
                     return True
         return False
 
     def is_ipv4_mapped(self):
         """
-        :return: ``True`` if this IP is IPv4-compatible IPv6 address, ``False``
+        :return: ``True`` if this IP is IPv4-mapped IPv6 address, ``False``
             otherwise.
         """
         return self._module.version == 6 and (self._value >> 32) == 0xFFFF
 
     def is_ipv4_compat(self):
         """
-        :return: ``True`` if this IP is IPv4-mapped IPv6 address, ``False``
+        :return: ``True`` if this IP is IPv4-compatible IPv6 address, ``False``
             otherwise.
         """
         return self._module.version == 6 and (self._value >> 32) == 0
 
     @property
     def info(self):
         """
@@ -581,16 +581,16 @@
         return ip
 
     def ipv6(self, ipv4_compatible=False):
         """
         .. note:: The IPv4-compatible IPv6 address format is now considered \
             deprecated. See RFC 4291 or later for details.
 
-        :param ipv4_compatible: If ``True`` returns an IPv4-mapped address
-            (::ffff:x.x.x.x), an IPv4-compatible (::x.x.x.x) address
+        :param ipv4_compatible: If ``True`` returns an IPv4-compatible address
+            (::x.x.x.x), an IPv4-mapped (::ffff:x.x.x.x) address
             otherwise. Default: False (IPv4-mapped).
 
         :return: A numerically equivalent version 6 `IPAddress` object.
         """
         ip = None
         klass = self.__class__
 
@@ -872,15 +872,15 @@
         """
         Ranged IP objects always represent a sequence of at least one IP
         address and are therefore always True in the boolean context.
         """
         return True
 
 
-def parse_ip_network(module, addr, flags=0):
+def parse_ip_network(module, addr, flags=0, *, expand_partial=False):
     if isinstance(addr, tuple):
         #   CIDR integer tuple
         if len(addr) != 2:
             raise AddrFormatError('invalid %s tuple!' % module.family_name)
         value, prefixlen = addr
 
         if not (0 <= value <= module.max_int):
@@ -892,14 +892,17 @@
 
         if '/' in addr:
             val1, val2 = addr.split('/', 1)
         else:
             val1 = addr
             val2 = None
 
+        if expand_partial:
+            val1 = module.expand_partial_address(val1)
+
         ip = IPAddress(val1, module.version, flags=INET_PTON)
         value = ip._value
 
         try:
             #   Integer CIDR prefix.
             prefixlen = int(val2)
         except TypeError:
@@ -957,19 +960,23 @@
     .. versionchanged:: 1.0.0
         Removed the ``implicit_prefix`` switch that used to enable the abbreviated CIDR
         format support, use :func:`cidr_abbrev_to_verbose` if you need this behavior.
 
     .. versionchanged:: 1.1.0
         Removed partial IPv4 address support accidentally left when making 1.0.0 release.
         Use :func:`expand_partial_ipv4_address` if you need this behavior.
+
+    .. versionchanged:: 1.3.0
+        Added the expand_partial flag, which restores the previous behavior to expand
+        partial IPv4 address
     """
 
     __slots__ = ('_prefixlen',)
 
-    def __init__(self, addr, version=None, flags=0):
+    def __init__(self, addr, version=None, flags=0, *, expand_partial=False):
         """
         Constructor.
 
         :param addr: an IPv4 or IPv6 address with optional CIDR prefix,
             netmask or hostmask. May be an IP address in presentation
             (string) format, an tuple containing and integer address and a
             network prefix, or another IPAddress/IPNetwork object (copy
@@ -979,48 +986,58 @@
             and distinguishes between IPv4 and IPv6 for addresses with an
             equivalent integer value.
 
         :param flags: (optional) decides which rules are applied to the
             interpretation of the addr value. Currently only supports the
             :data:`NOHOST` option.
 
+        :param expand_partial: (optional) decides whether partial address is
+            expanded. Currently this is only effective for IPv4 address.
+
             >>> IPNetwork('1.2.3.4/24')
             IPNetwork('1.2.3.4/24')
             >>> IPNetwork('1.2.3.4/24', flags=NOHOST)
             IPNetwork('1.2.3.0/24')
+            >>> IPNetwork('10/24', expand_partial=True)
+            IPNetwork('10.0.0.0/24')
         """
         super(IPNetwork, self).__init__()
 
         if flags & ~NOHOST:
             raise ValueError('Unrecognized IPAddress flags value: %s' % (flags,))
 
         value, prefixlen, module = None, None, None
 
         if hasattr(addr, '_prefixlen'):
             #   IPNetwork object copy constructor
             value = addr._value
             module = addr._module
             prefixlen = addr._prefixlen
+            if flags & NOHOST:
+                netmask = module.prefix_to_netmask[prefixlen]
+                value = value & netmask
         elif hasattr(addr, '_value'):
             #   IPAddress object copy constructor
             value = addr._value
             module = addr._module
             prefixlen = module.width
         elif version == 4:
-            value, prefixlen = parse_ip_network(_ipv4, addr, flags=flags)
+            value, prefixlen = parse_ip_network(_ipv4, addr, flags, expand_partial=expand_partial)
             module = _ipv4
         elif version == 6:
-            value, prefixlen = parse_ip_network(_ipv6, addr, flags=flags)
+            value, prefixlen = parse_ip_network(_ipv6, addr, flags)
             module = _ipv6
         else:
             if version is not None:
                 raise ValueError('%r is an invalid IP version!' % version)
             try:
                 module = _ipv4
-                value, prefixlen = parse_ip_network(module, addr, flags)
+                value, prefixlen = parse_ip_network(
+                    module, addr, flags, expand_partial=expand_partial
+                )
             except AddrFormatError:
                 try:
                     module = _ipv6
                     value, prefixlen = parse_ip_network(module, addr, flags)
                 except AddrFormatError:
                     pass
 
@@ -1266,16 +1283,16 @@
         return ip
 
     def ipv6(self, ipv4_compatible=False):
         """
         .. note:: the IPv4-mapped IPv6 address format is now considered \
         deprecated. See RFC 4291 or later for details.
 
-        :param ipv4_compatible: If ``True`` returns an IPv4-mapped address
-            (::ffff:x.x.x.x), an IPv4-compatible (::x.x.x.x) address
+        :param ipv4_compatible: If ``True`` returns an IPv4-compatible address
+            (::x.x.x.x), an IPv4-mapped (::ffff:x.x.x.x) address
             otherwise. Default: False (IPv4-mapped).
 
         :return: A numerically equivalent version 6 `IPNetwork` object.
         """
         ip = None
         klass = self.__class__
```

### Comparing `netaddr-1.2.1/netaddr/ip/glob.py` & `netaddr-1.3.0/netaddr/ip/glob.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/iana.py` & `netaddr-1.3.0/netaddr/ip/iana.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/ipv4-address-space.xml` & `netaddr-1.3.0/netaddr/ip/ipv4-address-space.xml`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/ipv6-address-space.xml` & `netaddr-1.3.0/netaddr/ip/ipv6-address-space.xml`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/ipv6-unicast-address-assignments.xml` & `netaddr-1.3.0/netaddr/ip/ipv6-unicast-address-assignments.xml`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/multicast-addresses.xml` & `netaddr-1.3.0/netaddr/ip/multicast-addresses.xml`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/nmap.py` & `netaddr-1.3.0/netaddr/ip/nmap.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/rfc1924.py` & `netaddr-1.3.0/netaddr/ip/rfc1924.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/ip/sets.py` & `netaddr-1.3.0/netaddr/ip/sets.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/strategy/__init__.py` & `netaddr-1.3.0/netaddr/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/strategy/eui48.py` & `netaddr-1.3.0/netaddr/strategy/eui48.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/strategy/eui64.py` & `netaddr-1.3.0/netaddr/strategy/eui64.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/strategy/ipv4.py` & `netaddr-1.3.0/netaddr/strategy/ipv4.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,16 @@
     :param flags: decides which rules are applied to the interpretation of the
         addr value. Supported constants are INET_PTON and ZEROFILL. See the
         :class:`IPAddress` documentation for details.
 
     :return: The equivalent unsigned integer for a given IPv4 address.
     """
     error = AddrFormatError('%r is not a valid IPv4 address string!' % (addr,))
+    if ':' in addr:
+        raise error
     pton_mode = flags & INET_PTON or not flags & INET_ATON
     if flags & ZEROFILL:
         addr = '.'.join(['%d' % int(i) for i in addr.split('.')])
     elif pton_mode and any(len(p) > 1 and p.startswith('0') for p in addr.split('.')):
         raise error
 
     try:
```

### Comparing `netaddr-1.2.1/netaddr/strategy/ipv6.py` & `netaddr-1.3.0/netaddr/strategy/ipv6.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/core/test_pubsub.py` & `netaddr-1.3.0/netaddr/tests/core/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/eui/test_eui.py` & `netaddr-1.3.0/netaddr/tests/eui/test_eui.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/eui/test_ieee_parsers.py` & `netaddr-1.3.0/netaddr/tests/eui/test_ieee_parsers.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_cidr_v4.py` & `netaddr-1.3.0/netaddr/tests/ip/test_cidr_v4.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_cidr_v6.py` & `netaddr-1.3.0/netaddr/tests/ip/test_cidr_v6.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_categories.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_categories.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_comparisons.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_comparisons.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_globs.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_globs.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_network_categories.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_network_categories.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_ranges.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_rfc1924.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_rfc1924.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_sets.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_sets.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_splitter.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_splitter.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_v4.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_v4.py`

 * *Files 4% similar despite different names*

```diff
@@ -351,14 +351,22 @@
 
 
 def test_ipnetwork_bad_string_constructor():
     with pytest.raises(AddrFormatError):
         IPNetwork('foo')
 
 
+def test_ipnetwork_expand_partial_v4():
+    with pytest.raises(AddrFormatError):
+        IPNetwork('10/8')
+    assert IPNetwork('10/8', expand_partial=True) == IPNetwork('10.0.0.0/8')
+    assert IPNetwork('10.20/16', expand_partial=True) == IPNetwork('10.20.0.0/16')
+    assert IPNetwork('10.20.30/24', expand_partial=True) == IPNetwork('10.20.30.0/24')
+
+
 def test_ipaddress_netmask_v4():
     assert IPAddress('0.0.0.0').netmask_bits() == 0
     assert IPAddress('128.0.0.0').netmask_bits() == 1
     assert IPAddress('255.0.0.0').netmask_bits() == 8
     assert IPAddress('255.255.0.0').netmask_bits() == 16
     assert IPAddress('255.255.255.0').netmask_bits() == 24
     assert IPAddress('255.255.255.254').netmask_bits() == 31
@@ -483,7 +491,11 @@
         IPAddress('10.0.0.1'),
         IPAddress('10.0.0.2'),
         '10.0.0.3',
         '10.0.0.4',
     ]
     assert spanning_cidr(addresses) == IPNetwork('10.0.0.0/29')
     assert spanning_cidr(reversed(addresses)) == IPNetwork('10.0.0.0/29')
+
+
+def test_ipnetwork_nohost():
+    assert IPNetwork(IPNetwork('192.168.0.1/24'), flags=NOHOST).ip == IPAddress('192.168.0.0')
```

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_v4_v6_conversions.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_v4_v6_conversions.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_ip_v6.py` & `netaddr-1.3.0/netaddr/tests/ip/test_ip_v6.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pickle
 import pytest
-from netaddr import IPAddress, IPNetwork
+from netaddr import IPAddress, IPNetwork, ZEROFILL
 
 
 def test_ipaddress_v6():
     ip = IPAddress('fe80::dead:beef')
     assert ip.version == 6
     assert repr(ip) == "IPAddress('fe80::dead:beef')"
     assert str(ip) == 'fe80::dead:beef'
@@ -170,7 +170,11 @@
     assert IPNetwork('1234::').broadcast is None
 
     # Tests for /128 subnet
     assert IPNetwork('1234::/128').network == IPAddress('1234::')
     assert IPNetwork('1234::/128').broadcast is None
     assert list(IPNetwork('1234::/128')) == [IPAddress('1234::')]
     assert list(IPNetwork('1234::/128').iter_hosts()) == [IPAddress('1234::')]
+
+
+def test_ipaddress_ignores_zerofill_when_parsing_ipv6():
+    assert IPAddress('fe80::', flags=ZEROFILL)
```

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_network_ops.py` & `netaddr-1.3.0/netaddr/tests/ip/test_network_ops.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_nmap.py` & `netaddr-1.3.0/netaddr/tests/ip/test_nmap.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_old_specs.py` & `netaddr-1.3.0/netaddr/tests/ip/test_old_specs.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_platform_osx.py` & `netaddr-1.3.0/netaddr/tests/ip/test_platform_osx.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/ip/test_socket_module_fallback.py` & `netaddr-1.3.0/netaddr/tests/ip/test_socket_module_fallback.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/strategy/test_eui48_strategy.py` & `netaddr-1.3.0/netaddr/tests/strategy/test_eui48_strategy.py`

 * *Files identical despite different names*

### Comparing `netaddr-1.2.1/netaddr/tests/strategy/test_ipv4_strategy.py` & `netaddr-1.3.0/netaddr/tests/strategy/test_ipv4_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from netaddr import INET_ATON, INET_PTON, AddrFormatError
+from netaddr import INET_ATON, INET_PTON, AddrFormatError, ZEROFILL
 from netaddr.strategy import ipv4
 
 
 def test_strategy_ipv4():
     b = '11000000.00000000.00000010.00000001'
     i = 3221225985
     t = (192, 0, 2, 1)
@@ -35,14 +35,19 @@
     assert ipv4.str_to_int('0177', flags=INET_ATON) == 127
     assert ipv4.str_to_int('127.1', flags=INET_ATON) == 2130706433
     assert ipv4.str_to_int('0x7f.1', flags=INET_ATON) == 2130706433
     assert ipv4.str_to_int('0177.1', flags=INET_ATON) == 2130706433
     assert ipv4.str_to_int('127.0.0.1', flags=INET_ATON) == 2130706433
 
 
+def test_str_to_int_correctly_rejects_ipv6_with_zerofill():
+    with pytest.raises(AddrFormatError):
+        ipv4.str_to_int('fe80::', flags=ZEROFILL)
+
+
 def test_strategy_inet_pton_behaviour():
     # inet_pton() is a newer system call that supports both IPv4 and IPv6.
     # It is a lot more strict about what it deems to be a valid IPv4 address
     # and doesn't support many of the features found in inet_aton() such as
     # support for non- decimal octets, partial numbers of octets, etc.
 
     with pytest.raises(AddrFormatError):
```

### Comparing `netaddr-1.2.1/netaddr/tests/strategy/test_ipv6_strategy.py` & `netaddr-1.3.0/netaddr/tests/strategy/test_ipv6_strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import platform
 
 import pytest
 
 from netaddr import AddrFormatError
 from netaddr.strategy import ipv6
+from netaddr.tests import IS_MUSL
 
 
 def test_strategy_ipv6():
     b = '0000000000000000:0000000000000000:0000000000000000:0000000000000000:0000000000000000:0000000000000000:1111111111111111:1111111111111110'
     i = 4294967294
     t = (0, 0, 0, 0, 0, 0, 0xFFFF, 0xFFFE)
     s = '::255.255.255.254'
     p = b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xff\xff\xff\xfe'
 
     assert ipv6.bits_to_int(b) == i
     assert ipv6.int_to_bits(i) == b
 
-    assert ipv6.int_to_str(i) == s
+    # musl renders IPv4-compatible IPv6 addresses like any other IPv6 address.
+    assert ipv6.int_to_str(i) == s if not IS_MUSL else '::ffff:fffe'
     assert ipv6.str_to_int(s) == i
 
     assert ipv6.int_to_words(i) == t
     assert ipv6.words_to_int(t) == i
     assert ipv6.words_to_int(list(t)) == i
 
     assert ipv6.int_to_packed(i) == p
@@ -122,16 +124,18 @@
 def test_strategy_ipv6_string_compaction(long_form, short_form):
     int_val = ipv6.str_to_int(long_form)
     calc_short_form = ipv6.int_to_str(int_val)
     assert calc_short_form == short_form
 
 
 def test_strategy_ipv6_mapped_and_compatible_ipv4_string_formatting():
-    assert ipv6.int_to_str(0xFFFFFF) == '::0.255.255.255'
-    assert ipv6.int_to_str(0xFFFFFFFF) == '::255.255.255.255'
+    # musl renders IPv4-compatible IPv6 addresses like any other IPv6 address.
+    assert ipv6.int_to_str(0xFFFFFF) == '::0.255.255.255' if not IS_MUSL else '::ff:ffff'
+    assert ipv6.int_to_str(0xFFFFFFFF) == '::255.255.255.255' if not IS_MUSL else '::ffff:ffff'
+
     assert ipv6.int_to_str(0x1FFFFFFFF) == '::1:ffff:ffff'
     assert ipv6.int_to_str(0xFFFFFFFFFFFF) == '::ffff:255.255.255.255'
     assert ipv6.int_to_str(0xFFFEFFFFFFFF) == '::fffe:ffff:ffff'
     assert ipv6.int_to_str(0xFFFFFFFFFFFF) == '::ffff:255.255.255.255'
     assert ipv6.int_to_str(0xFFFFFFFFFFF1) == '::ffff:255.255.255.241'
     assert ipv6.int_to_str(0xFFFFFFFFFFFE) == '::ffff:255.255.255.254'
     assert ipv6.int_to_str(0xFFFFFFFFFF00) == '::ffff:255.255.255.0'
```

### Comparing `netaddr-1.2.1/netaddr.egg-info/PKG-INFO` & `netaddr-1.3.0/netaddr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netaddr
-Version: 1.2.1
+Version: 1.3.0
 Summary: A network address manipulation library for Python
 Author-email: "David P. D. Moss" <josiah_carberry@brown.edu>, Stefan Nordhausen <stefan.nordhausen@immobilienscout24.de>
 Maintainer-email: Jakub Stasiak <jakub@stasiak.at>
 License: BSD License
 Project-URL: Documentation, https://netaddr.readthedocs.io/en/latest/
 Project-URL: Download, https://pypi.org/project/netaddr/
 Project-URL: Repository, https://github.com/netaddr/netaddr/
```

### Comparing `netaddr-1.2.1/netaddr.egg-info/SOURCES.txt` & `netaddr-1.3.0/netaddr.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,21 +11,14 @@
 requirements-dev.in
 requirements-dev.txt
 docs/Makefile
 docs/make.bat
 docs/poetry.lock
 docs/pyproject.toml
 docs/requirements.txt
-docs/build/html/_static/basic.css
-docs/build/html/_static/custom.css
-docs/build/html/_static/debug.css
-docs/build/html/_static/pygments.css
-docs/build/html/_static/skeleton.css
-docs/build/html/_static/styles/furo-extensions.css
-docs/build/html/_static/styles/furo.css
 docs/source/api.rst
 docs/source/authors.rst
 docs/source/changes.rst
 docs/source/conf.py
 docs/source/contributors.rst
 docs/source/copyright.rst
 docs/source/how-to.rst
```

### Comparing `netaddr-1.2.1/pyproject.toml` & `netaddr-1.3.0/pyproject.toml`

 * *Files identical despite different names*

