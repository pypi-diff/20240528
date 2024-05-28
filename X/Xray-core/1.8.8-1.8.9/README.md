# Comparing `tmp/Xray-core-1.8.8.tar.gz` & `tmp/Xray-core-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Xray-core-1.8.8.tar", last modified: Wed Feb 28 15:14:25 2024, max compression
+gzip compressed data, was "Xray-core-1.8.9.tar", last modified: Mon Mar 11 05:03:19 2024, max compression
```

## Comparing `Xray-core-1.8.8.tar` & `Xray-core-1.8.9.tar`

### file list

```diff
@@ -1,1115 +1,1123 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.098563 Xray-core-1.8.8/
--rw-r--r--   0 runner     (501) staff       (20)     1149 2024-02-28 15:14:14.000000 Xray-core-1.8.8/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)    16725 2024-02-28 15:14:14.000000 Xray-core-1.8.8/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      180 2024-02-28 15:14:14.000000 Xray-core-1.8.8/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     5544 2024-02-28 15:14:25.097580 Xray-core-1.8.8/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3756 2024-02-28 15:14:14.000000 Xray-core-1.8.8/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.623646 Xray-core-1.8.8/Xray_core.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     5544 2024-02-28 15:14:24.000000 Xray-core-1.8.8/Xray_core.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    35658 2024-02-28 15:14:24.000000 Xray-core-1.8.8/Xray_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-28 15:14:24.000000 Xray-core-1.8.8/Xray_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-02-28 15:14:24.000000 Xray-core-1.8.8/Xray_core.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)        5 2024-02-28 15:14:24.000000 Xray-core-1.8.8/Xray_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.623987 Xray-core-1.8.8/gobuild/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-02-28 15:14:14.000000 Xray-core-1.8.8/gobuild/.gitkeep
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.625020 Xray-core-1.8.8/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    11911 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1684 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)        7 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/VERSION
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.592602 Xray-core-1.8.8/pybind11/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.635594 Xray-core-1.8.8/pybind11/include/pybind11/
--rw-r--r--   0 runner     (501) staff       (20)    23979 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner     (501) staff       (20)     7069 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner     (501) staff       (20)    65638 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner     (501) staff       (20)     8458 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner     (501) staff       (20)      120 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner     (501) staff       (20)     2096 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.640820 Xray-core-1.8.8/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner     (501) staff       (20)    28251 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner     (501) staff       (20)    50369 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner     (501) staff       (20)     5491 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner     (501) staff       (20)    17981 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner     (501) staff       (20)    25057 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner     (501) staff       (20)    42266 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner     (501) staff       (20)     1625 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner     (501) staff       (20)    32147 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner     (501) staff       (20)    11792 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner     (501) staff       (20)     4731 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner     (501) staff       (20)     4695 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner     (501) staff       (20)     8262 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner     (501) staff       (20)     8862 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner     (501) staff       (20)    79524 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner     (501) staff       (20)     9103 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner     (501) staff       (20)     2181 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner     (501) staff       (20)   125761 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner     (501) staff       (20)    93848 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.641459 Xray-core-1.8.8/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner     (501) staff       (20)     4185 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner     (501) staff       (20)    15337 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner     (501) staff       (20)    27013 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.650320 Xray-core-1.8.8/pybind11/tools/
--rw-r--r--   0 runner     (501) staff       (20)     2350 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner     (501) staff       (20)     3105 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner     (501) staff       (20)    11103 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner     (501) staff       (20)      817 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner     (501) staff       (20)     1423 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/check-style.sh
--rw-r--r--   0 runner     (501) staff       (20)      952 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     1040 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner     (501) staff       (20)     1031 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/libsize.py
--rw-r--r--   0 runner     (501) staff       (20)     1282 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner     (501) staff       (20)      196 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner     (501) staff       (20)    13487 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner     (501) staff       (20)     6930 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner     (501) staff       (20)     8955 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner     (501) staff       (20)     8359 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner     (501) staff       (20)       94 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1965 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner     (501) staff       (20)     1139 2024-02-28 15:14:14.000000 Xray-core-1.8.8/pybind11/tools/setup_main.py.in
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-02-28 15:14:25.098833 Xray-core-1.8.8/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2810 2024-02-28 15:14:14.000000 Xray-core-1.8.8/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.650688 Xray-core-1.8.8/src/
--rw-r--r--   0 runner     (501) staff       (20)     1403 2024-02-28 15:14:14.000000 Xray-core-1.8.8/src/xray.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.651135 Xray-core-1.8.8/xray/
--rw-r--r--   0 runner     (501) staff       (20)       50 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.653851 Xray-core-1.8.8/xray-go/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.654276 Xray-core-1.8.8/xray-go/.github/
--rw-r--r--   0 runner     (501) staff       (20)      560 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.654862 Xray-core-1.8.8/xray-go/.github/docker/
--rw-r--r--   0 runner     (501) staff       (20)      907 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/.github/docker/Dockerfile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.655539 Xray-core-1.8.8/xray-go/.github/docker/files/
--rw-r--r--   0 runner     (501) staff       (20)      286 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/.github/docker/files/config.json
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.657749 Xray-core-1.8.8/xray-go/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1324 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/.github/workflows/docker.yml
--rw-r--r--   0 runner     (501) staff       (20)     6816 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/.github/workflows/release.yml
--rw-r--r--   0 runner     (501) staff       (20)      941 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/.github/workflows/test.yml
--rw-r--r--   0 runner     (501) staff       (20)      420 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     5226 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner     (501) staff       (20)    16725 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      799 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/Makefile
--rw-r--r--   0 runner     (501) staff       (20)     6730 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.658474 Xray-core-1.8.8/xray-go/app/
--rw-r--r--   0 runner     (501) staff       (20)      113 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/app.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.663058 Xray-core-1.8.8/xray-go/app/commander/
--rw-r--r--   0 runner     (501) staff       (20)     2327 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/commander/commander.go
--rw-r--r--   0 runner     (501) staff       (20)     7721 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/commander/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      681 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/commander/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      218 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/commander/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     2176 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/commander/outbound.go
--rw-r--r--   0 runner     (501) staff       (20)      585 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/commander/service.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.669333 Xray-core-1.8.8/xray-go/app/dispatcher/
--rw-r--r--   0 runner     (501) staff       (20)     6917 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      337 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/config.proto
--rw-r--r--   0 runner     (501) staff       (20)    12703 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/default.go
--rw-r--r--   0 runner     (501) staff       (20)       90 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/dispatcher.go
--rw-r--r--   0 runner     (501) staff       (20)      219 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3802 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/fakednssniffer.go
--rw-r--r--   0 runner     (501) staff       (20)     3837 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/sniffer.go
--rw-r--r--   0 runner     (501) staff       (20)      514 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/stats.go
--rw-r--r--   0 runner     (501) staff       (20)      818 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dispatcher/stats_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.679017 Xray-core-1.8.8/xray-go/app/dns/
--rw-r--r--   0 runner     (501) staff       (20)     2112 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/config.go
--rw-r--r--   0 runner     (501) staff       (20)    29979 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     2116 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     9305 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/dns.go
--rw-r--r--   0 runner     (501) staff       (20)    24669 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/dns_test.go
--rw-r--r--   0 runner     (501) staff       (20)     5826 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/dnscommon.go
--rw-r--r--   0 runner     (501) staff       (20)     4468 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/dnscommon_test.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.681863 Xray-core-1.8.8/xray-go/app/dns/fakedns/
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/fakedns/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     6312 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/fakedns/fake.go
--rw-r--r--   0 runner     (501) staff       (20)       87 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/fakedns/fakedns.go
--rw-r--r--   0 runner     (501) staff       (20)     7885 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/fakedns/fakedns.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      497 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/fakedns/fakedns.proto
--rw-r--r--   0 runner     (501) staff       (20)     5889 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/fakedns/fakedns_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3272 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/hosts.go
--rw-r--r--   0 runner     (501) staff       (20)     2527 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/hosts_test.go
--rw-r--r--   0 runner     (501) staff       (20)     8513 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver.go
--rw-r--r--   0 runner     (501) staff       (20)    10593 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_doh.go
--rw-r--r--   0 runner     (501) staff       (20)     2705 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_doh_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1206 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_fakedns.go
--rw-r--r--   0 runner     (501) staff       (20)     1512 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_local.go
--rw-r--r--   0 runner     (501) staff       (20)      590 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_local_test.go
--rw-r--r--   0 runner     (501) staff       (20)     9780 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_quic.go
--rw-r--r--   0 runner     (501) staff       (20)     2216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_quic_test.go
--rw-r--r--   0 runner     (501) staff       (20)     9104 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_tcp.go
--rw-r--r--   0 runner     (501) staff       (20)     2767 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_tcp_test.go
--rw-r--r--   0 runner     (501) staff       (20)     7088 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/dns/nameserver_udp.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.684040 Xray-core-1.8.8/xray-go/app/log/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.686690 Xray-core-1.8.8/xray-go/app/log/command/
--rw-r--r--   0 runner     (501) staff       (20)     1459 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/command/command.go
--rw-r--r--   0 runner     (501) staff       (20)      919 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/command/command_test.go
--rw-r--r--   0 runner     (501) staff       (20)     8975 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/command/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      440 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/command/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     4016 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/command/config_grpc.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/command/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     9727 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      536 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     2921 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/log.go
--rw-r--r--   0 runner     (501) staff       (20)     1527 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/log_creator.go
--rw-r--r--   0 runner     (501) staff       (20)     1282 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/log/log_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.688626 Xray-core-1.8.8/xray-go/app/metrics/
--rw-r--r--   0 runner     (501) staff       (20)     4934 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/metrics/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      383 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/metrics/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/metrics/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3132 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/metrics/metrics.go
--rw-r--r--   0 runner     (501) staff       (20)     2190 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/metrics/outbound.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.690888 Xray-core-1.8.8/xray-go/app/observatory/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.695542 Xray-core-1.8.8/xray-go/app/observatory/burst/
--rw-r--r--   0 runner     (501) staff       (20)      207 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/burst.go
--rw-r--r--   0 runner     (501) staff       (20)     2779 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/burstobserver.go
--rw-r--r--   0 runner     (501) staff       (20)    10520 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      931 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     6228 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/healthping.go
--rw-r--r--   0 runner     (501) staff       (20)     3301 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/healthping_result.go
--rw-r--r--   0 runner     (501) staff       (20)     2485 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/healthping_result_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1696 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/burst/ping.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.697579 Xray-core-1.8.8/xray-go/app/observatory/command/
--rw-r--r--   0 runner     (501) staff       (20)     1141 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/command/command.go
--rw-r--r--   0 runner     (501) staff       (20)    11323 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/command/command.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      618 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/command/command.proto
--rw-r--r--   0 runner     (501) staff       (20)     4350 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/command/command_grpc.pb.go
--rw-r--r--   0 runner     (501) staff       (20)    22974 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     2011 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      220 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      565 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/explainErrors.go
--rw-r--r--   0 runner     (501) staff       (20)       91 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/observatory.go
--rw-r--r--   0 runner     (501) staff       (20)     6035 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/observatory/observer.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.700534 Xray-core-1.8.8/xray-go/app/policy/
--rw-r--r--   0 runner     (501) staff       (20)     2520 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/policy/config.go
--rw-r--r--   0 runner     (501) staff       (20)    25190 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/policy/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1039 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/policy/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/policy/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1433 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/policy/manager.go
--rw-r--r--   0 runner     (501) staff       (20)      995 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/policy/manager_test.go
--rw-r--r--   0 runner     (501) staff       (20)      152 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/policy/policy.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.701755 Xray-core-1.8.8/xray-go/app/proxyman/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.704217 Xray-core-1.8.8/xray-go/app/proxyman/command/
--rw-r--r--   0 runner     (501) staff       (20)     4575 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/command/command.go
--rw-r--r--   0 runner     (501) staff       (20)    39310 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/command/command.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1652 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/command/command.proto
--rw-r--r--   0 runner     (501) staff       (20)    12112 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/command/command_grpc.pb.go
--rw-r--r--   0 runner     (501) staff       (20)       87 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/command/doc.go
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/command/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      758 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/config.go
--rw-r--r--   0 runner     (501) staff       (20)    43436 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     3087 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/config.proto
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.706308 Xray-core-1.8.8/xray-go/app/proxyman/inbound/
--rw-r--r--   0 runner     (501) staff       (20)     5289 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/inbound/always.go
--rw-r--r--   0 runner     (501) staff       (20)     5544 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/inbound/dynamic.go
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/inbound/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     4732 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/inbound/inbound.go
--rw-r--r--   0 runner     (501) staff       (20)    12675 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/inbound/worker.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.708130 Xray-core-1.8.8/xray-go/app/proxyman/outbound/
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/outbound/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     9264 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/outbound/handler.go
--rw-r--r--   0 runner     (501) staff       (20)     4262 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/outbound/handler_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3984 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/outbound/outbound.go
--rw-r--r--   0 runner     (501) staff       (20)     1020 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/proxyman/outbound/uot.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.710928 Xray-core-1.8.8/xray-go/app/reverse/
--rw-r--r--   0 runner     (501) staff       (20)     4440 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/bridge.go
--rw-r--r--   0 runner     (501) staff       (20)      235 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/config.go
--rw-r--r--   0 runner     (501) staff       (20)    13860 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     5552 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/portal.go
--rw-r--r--   0 runner     (501) staff       (20)      396 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/portal_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2049 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/reverse/reverse.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.718399 Xray-core-1.8.8/xray-go/app/router/
--rw-r--r--   0 runner     (501) staff       (20)     2927 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/balancing.go
--rw-r--r--   0 runner     (501) staff       (20)      882 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/balancing_override.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.721842 Xray-core-1.8.8/xray-go/app/router/command/
--rw-r--r--   0 runner     (501) staff       (20)     3963 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/command/command.go
--rw-r--r--   0 runner     (501) staff       (20)    39584 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/command/command.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     3169 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/command/command.proto
--rw-r--r--   0 runner     (501) staff       (20)     9869 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/command/command_grpc.pb.go
--rw-r--r--   0 runner     (501) staff       (20)    12280 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/command/command_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3684 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/command/config.go
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/command/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     6367 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/condition.go
--rw-r--r--   0 runner     (501) staff       (20)     2481 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/condition_geoip.go
--rw-r--r--   0 runner     (501) staff       (20)     5852 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/condition_geoip_test.go
--rw-r--r--   0 runner     (501) staff       (20)    12335 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/condition_test.go
--rw-r--r--   0 runner     (501) staff       (20)     4008 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/config.go
--rw-r--r--   0 runner     (501) staff       (20)    53331 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     4248 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3736 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/router.go
--rw-r--r--   0 runner     (501) staff       (20)     6705 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/router_test.go
--rw-r--r--   0 runner     (501) staff       (20)     5719 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/strategy_leastload.go
--rw-r--r--   0 runner     (501) staff       (20)     5152 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/strategy_leastload_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1522 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/strategy_leastping.go
--rw-r--r--   0 runner     (501) staff       (20)      438 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/strategy_random.go
--rw-r--r--   0 runner     (501) staff       (20)     2021 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/weight.go
--rw-r--r--   0 runner     (501) staff       (20)     1207 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/router/weight_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.725500 Xray-core-1.8.8/xray-go/app/stats/
--rw-r--r--   0 runner     (501) staff       (20)     4219 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/channel.go
--rw-r--r--   0 runner     (501) staff       (20)     9714 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/channel_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.727827 Xray-core-1.8.8/xray-go/app/stats/command/
--rw-r--r--   0 runner     (501) staff       (20)     3073 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/command/command.go
--rw-r--r--   0 runner     (501) staff       (20)    24726 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/command/command.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1176 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/command/command.proto
--rw-r--r--   0 runner     (501) staff       (20)     6923 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/command/command_grpc.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1875 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/command/command_test.go
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/command/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     7106 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      346 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      478 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/counter.go
--rw-r--r--   0 runner     (501) staff       (20)      664 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/counter_test.go
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3878 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/stats.go
--rw-r--r--   0 runner     (501) staff       (20)     2004 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/app/stats/stats_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.730050 Xray-core-1.8.8/xray-go/common/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.731184 Xray-core-1.8.8/xray-go/common/antireplay/
--rw-r--r--   0 runner     (501) staff       (20)      105 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/antireplay/antireplay.go
--rw-r--r--   0 runner     (501) staff       (20)      607 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/antireplay/bloomring.go
--rw-r--r--   0 runner     (501) staff       (20)     1324 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/antireplay/replayfilter.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.732194 Xray-core-1.8.8/xray-go/common/bitmask/
--rw-r--r--   0 runner     (501) staff       (20)      318 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/bitmask/byte.go
--rw-r--r--   0 runner     (501) staff       (20)      703 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/bitmask/byte_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.742801 Xray-core-1.8.8/xray-go/common/buf/
--rw-r--r--   0 runner     (501) staff       (20)      200 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/buf.go
--rw-r--r--   0 runner     (501) staff       (20)     5954 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/buffer.go
--rw-r--r--   0 runner     (501) staff       (20)     4488 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/buffer_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2973 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/copy.go
--rw-r--r--   0 runner     (501) staff       (20)     1519 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/copy_test.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3089 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/io.go
--rw-r--r--   0 runner     (501) staff       (20)     1008 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/io_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6788 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/multi_buffer.go
--rw-r--r--   0 runner     (501) staff       (20)     3788 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/multi_buffer_test.go
--rw-r--r--   0 runner     (501) staff       (20)      760 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/override.go
--rw-r--r--   0 runner     (501) staff       (20)     3819 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/reader.go
--rw-r--r--   0 runner     (501) staff       (20)     2952 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/reader_test.go
--rw-r--r--   0 runner     (501) staff       (20)      844 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/readv_posix.go
--rw-r--r--   0 runner     (501) staff       (20)     2638 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/readv_reader.go
--rw-r--r--   0 runner     (501) staff       (20)      198 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/readv_reader_wasm.go
--rw-r--r--   0 runner     (501) staff       (20)     1310 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/readv_test.go
--rw-r--r--   0 runner     (501) staff       (20)      561 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/readv_unix.go
--rw-r--r--   0 runner     (501) staff       (20)      733 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/readv_windows.go
--rw-r--r--   0 runner     (501) staff       (20)     5199 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/writer.go
--rw-r--r--   0 runner     (501) staff       (20)     2349 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/buf/writer_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.743154 Xray-core-1.8.8/xray-go/common/bytespool/
--rw-r--r--   0 runner     (501) staff       (20)     1500 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/bytespool/pool.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.743990 Xray-core-1.8.8/xray-go/common/cache/
--rw-r--r--   0 runner     (501) staff       (20)     2301 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/cache/lru.go
--rw-r--r--   0 runner     (501) staff       (20)     1394 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/cache/lru_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.744494 Xray-core-1.8.8/xray-go/common/cmdarg/
--rw-r--r--   0 runner     (501) staff       (20)      298 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/cmdarg/cmdarg.go
--rw-r--r--   0 runner     (501) staff       (20)     4437 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/common.go
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/common_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.749428 Xray-core-1.8.8/xray-go/common/crypto/
--rw-r--r--   0 runner     (501) staff       (20)     1267 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/aes.go
--rw-r--r--   0 runner     (501) staff       (20)     7900 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/auth.go
--rw-r--r--   0 runner     (501) staff       (20)     3382 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/auth_test.go
--rw-r--r--   0 runner     (501) staff       (20)      990 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/benchmark_test.go
--rw-r--r--   0 runner     (501) staff       (20)      405 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/chacha20.go
--rw-r--r--   0 runner     (501) staff       (20)     2345 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/chacha20_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3681 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/chunk.go
--rw-r--r--   0 runner     (501) staff       (20)     1060 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/chunk_test.go
--rw-r--r--   0 runner     (501) staff       (20)      199 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/crypto.go
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.751042 Xray-core-1.8.8/xray-go/common/crypto/internal/
--rw-r--r--   0 runner     (501) staff       (20)     1942 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/internal/chacha.go
--rw-r--r--   0 runner     (501) staff       (20)     3156 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/internal/chacha_core.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1832 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/internal/chacha_core_gen.go
--rw-r--r--   0 runner     (501) staff       (20)     1360 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/crypto/io.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.751909 Xray-core-1.8.8/xray-go/common/dice/
--rw-r--r--   0 runner     (501) staff       (20)     1068 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/dice/dice.go
--rw-r--r--   0 runner     (501) staff       (20)      738 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/dice/dice_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.753611 Xray-core-1.8.8/xray-go/common/drain/
--rw-r--r--   0 runner     (501) staff       (20)      187 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/drain/drain.go
--rw-r--r--   0 runner     (501) staff       (20)     1477 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/drain/drainer.go
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/drain/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.757619 Xray-core-1.8.8/xray-go/common/errors/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.758299 Xray-core-1.8.8/xray-go/common/errors/errorgen/
--rw-r--r--   0 runner     (501) staff       (20)      704 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/errors/errorgen/main.go
--rw-r--r--   0 runner     (501) staff       (20)     3723 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/errors/errors.go
--rw-r--r--   0 runner     (501) staff       (20)     1237 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/errors/errors_test.go
--rw-r--r--   0 runner     (501) staff       (20)      735 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/errors/multi_error.go
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1669 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/interfaces.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.763282 Xray-core-1.8.8/xray-go/common/log/
--rw-r--r--   0 runner     (501) staff       (20)     1369 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/access.go
--rw-r--r--   0 runner     (501) staff       (20)     1108 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/dns.go
--rw-r--r--   0 runner     (501) staff       (20)     1240 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/log.go
--rw-r--r--   0 runner     (501) staff       (20)     4648 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/log.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      317 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/log.proto
--rw-r--r--   0 runner     (501) staff       (20)      565 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/log_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3575 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/logger.go
--rw-r--r--   0 runner     (501) staff       (20)      773 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/log/logger_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.770686 Xray-core-1.8.8/xray-go/common/mux/
--rw-r--r--   0 runner     (501) staff       (20)     9235 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/client.go
--rw-r--r--   0 runner     (501) staff       (20)     2841 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/client_test.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     4073 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/frame.go
--rw-r--r--   0 runner     (501) staff       (20)      552 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/frame_test.go
--rw-r--r--   0 runner     (501) staff       (20)       83 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/mux.go
--rw-r--r--   0 runner     (501) staff       (20)     4251 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/mux_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1326 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/reader.go
--rw-r--r--   0 runner     (501) staff       (20)     8971 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/server.go
--rw-r--r--   0 runner     (501) staff       (20)     4120 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/session.go
--rw-r--r--   0 runner     (501) staff       (20)      756 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/session_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2881 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/mux/writer.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.779029 Xray-core-1.8.8/xray-go/common/net/
--rw-r--r--   0 runner     (501) staff       (20)     5118 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/address.go
--rw-r--r--   0 runner     (501) staff       (20)     6075 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/address.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      475 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/address.proto
--rw-r--r--   0 runner     (501) staff       (20)     4485 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/address_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.779614 Xray-core-1.8.8/xray-go/common/net/cnc/
--rw-r--r--   0 runner     (501) staff       (20)     3276 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/cnc/connection.go
--rw-r--r--   0 runner     (501) staff       (20)     3560 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/destination.go
--rw-r--r--   0 runner     (501) staff       (20)     6765 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/destination.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      428 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/destination.proto
--rw-r--r--   0 runner     (501) staff       (20)     2519 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/destination_test.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      229 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/net.go
--rw-r--r--   0 runner     (501) staff       (20)      423 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/network.go
--rw-r--r--   0 runner     (501) staff       (20)     7048 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/network.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      425 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/network.proto
--rw-r--r--   0 runner     (501) staff       (20)     2328 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/port.go
--rw-r--r--   0 runner     (501) staff       (20)     7084 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/port.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      513 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/port.proto
--rw-r--r--   0 runner     (501) staff       (20)      287 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/port_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1235 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/net/system.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.780615 Xray-core-1.8.8/xray-go/common/ocsp/
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/ocsp/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3094 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/ocsp/ocsp.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.781496 Xray-core-1.8.8/xray-go/common/peer/
--rw-r--r--   0 runner     (501) staff       (20)      434 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/peer/latency.go
--rw-r--r--   0 runner     (501) staff       (20)       13 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/peer/peer.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.783051 Xray-core-1.8.8/xray-go/common/platform/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.785189 Xray-core-1.8.8/xray-go/common/platform/ctlcmd/
--rw-r--r--   0 runner     (501) staff       (20)      133 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/ctlcmd/attr_other.go
--rw-r--r--   0 runner     (501) staff       (20)      172 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/ctlcmd/attr_windows.go
--rw-r--r--   0 runner     (501) staff       (20)     1188 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/ctlcmd/ctlcmd.go
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/ctlcmd/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.786105 Xray-core-1.8.8/xray-go/common/platform/filesystem/
--rw-r--r--   0 runner     (501) staff       (20)      832 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/filesystem/file.go
--rw-r--r--   0 runner     (501) staff       (20)      915 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/others.go
--rw-r--r--   0 runner     (501) staff       (20)     2260 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/platform.go
--rw-r--r--   0 runner     (501) staff       (20)     1175 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/platform_test.go
--rw-r--r--   0 runner     (501) staff       (20)      553 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/platform/windows.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.795965 Xray-core-1.8.8/xray-go/common/protocol/
--rw-r--r--   0 runner     (501) staff       (20)      239 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/account.go
--rw-r--r--   0 runner     (501) staff       (20)     5904 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/address.go
--rw-r--r--   0 runner     (501) staff       (20)     6183 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/address_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.796449 Xray-core-1.8.8/xray-go/common/protocol/bittorrent/
--rw-r--r--   0 runner     (501) staff       (20)     1908 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/bittorrent/bittorrent.go
--rw-r--r--   0 runner     (501) staff       (20)      411 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/context.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.797408 Xray-core-1.8.8/xray-go/common/protocol/dns/
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/dns/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     2592 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/dns/io.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     2490 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/headers.go
--rw-r--r--   0 runner     (501) staff       (20)     7925 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/headers.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      445 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/headers.proto
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.799713 Xray-core-1.8.8/xray-go/common/protocol/http/
--rw-r--r--   0 runner     (501) staff       (20)     1865 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/http/headers.go
--rw-r--r--   0 runner     (501) staff       (20)     2765 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/http/headers_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1591 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/http/sniff.go
--rw-r--r--   0 runner     (501) staff       (20)     3034 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/http/sniff_test.go
--rw-r--r--   0 runner     (501) staff       (20)      907 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/id.go
--rw-r--r--   0 runner     (501) staff       (20)      392 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/id_test.go
--rw-r--r--   0 runner     (501) staff       (20)      265 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/payload.go
--rw-r--r--   0 runner     (501) staff       (20)      142 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/protocol.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.801520 Xray-core-1.8.8/xray-go/common/protocol/quic/
--rw-r--r--   0 runner     (501) staff       (20)      324 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/quic/qtls_go118.go
--rw-r--r--   0 runner     (501) staff       (20)     7888 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/quic/sniff.go
--rw-r--r--   0 runner     (501) staff       (20)     1459 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/quic/sniff_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1439 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/server_picker.go
--rw-r--r--   0 runner     (501) staff       (20)     2053 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/server_picker_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2163 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/server_spec.go
--rw-r--r--   0 runner     (501) staff       (20)     7142 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/server_spec.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      459 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/server_spec.proto
--rw-r--r--   0 runner     (501) staff       (20)     1969 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/server_spec_test.go
--rw-r--r--   0 runner     (501) staff       (20)      403 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/time.go
--rw-r--r--   0 runner     (501) staff       (20)      459 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/time_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.803252 Xray-core-1.8.8/xray-go/common/protocol/tls/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.806384 Xray-core-1.8.8/xray-go/common/protocol/tls/cert/
--rw-r--r--   0 runner     (501) staff       (20)        5 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/tls/cert/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     4416 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/tls/cert/cert.go
--rw-r--r--   0 runner     (501) staff       (20)     2093 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/tls/cert/cert_test.go
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/tls/cert/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      939 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/tls/cert/privateKey.go
--rw-r--r--   0 runner     (501) staff       (20)     3199 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/tls/sniff.go
--rw-r--r--   0 runner     (501) staff       (20)     7025 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/tls/sniff_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.807331 Xray-core-1.8.8/xray-go/common/protocol/udp/
--rw-r--r--   0 runner     (501) staff       (20)      275 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/udp/packet.go
--rw-r--r--   0 runner     (501) staff       (20)       12 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/udp/udp.go
--rw-r--r--   0 runner     (501) staff       (20)      893 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/user.go
--rw-r--r--   0 runner     (501) staff       (20)     6433 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/user.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      544 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/protocol/user.proto
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.808965 Xray-core-1.8.8/xray-go/common/reflect/
--rw-r--r--   0 runner     (501) staff       (20)     3674 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/reflect/marshal.go
--rw-r--r--   0 runner     (501) staff       (20)     3303 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/reflect/marshal_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.810562 Xray-core-1.8.8/xray-go/common/retry/
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/retry/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1463 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/retry/retry.go
--rw-r--r--   0 runner     (501) staff       (20)     1894 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/retry/retry_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.814457 Xray-core-1.8.8/xray-go/common/serial/
--rw-r--r--   0 runner     (501) staff       (20)      736 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/serial.go
--rw-r--r--   0 runner     (501) staff       (20)     1676 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/serial_test.go
--rw-r--r--   0 runner     (501) staff       (20)      609 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/string.go
--rw-r--r--   0 runner     (501) staff       (20)     1049 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/string_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1334 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/typed_message.go
--rw-r--r--   0 runner     (501) staff       (20)     5786 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/typed_message.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      473 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/typed_message.proto
--rw-r--r--   0 runner     (501) staff       (20)      424 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/serial/typed_message_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.815575 Xray-core-1.8.8/xray-go/common/session/
--rw-r--r--   0 runner     (501) staff       (20)     4606 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/session/context.go
--rw-r--r--   0 runner     (501) staff       (20)     3380 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/session/session.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.817595 Xray-core-1.8.8/xray-go/common/signal/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.818232 Xray-core-1.8.8/xray-go/common/signal/done/
--rw-r--r--   0 runner     (501) staff       (20)      830 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/done/done.go
--rw-r--r--   0 runner     (501) staff       (20)      640 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/notifier.go
--rw-r--r--   0 runner     (501) staff       (20)      226 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/notifier_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.819052 Xray-core-1.8.8/xray-go/common/signal/pubsub/
--rw-r--r--   0 runner     (501) staff       (20)     1816 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/pubsub/pubsub.go
--rw-r--r--   0 runner     (501) staff       (20)      460 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/pubsub/pubsub_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.819573 Xray-core-1.8.8/xray-go/common/signal/semaphore/
--rw-r--r--   0 runner     (501) staff       (20)      522 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/semaphore/semaphore.go
--rw-r--r--   0 runner     (501) staff       (20)     1267 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/timer.go
--rw-r--r--   0 runner     (501) staff       (20)     1422 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/signal/timer_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.823246 Xray-core-1.8.8/xray-go/common/singbridge/
--rw-r--r--   0 runner     (501) staff       (20)     1249 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/destination.go
--rw-r--r--   0 runner     (501) staff       (20)     1935 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)      173 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/error.go
--rw-r--r--   0 runner     (501) staff       (20)     1520 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/handler.go
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/logger.go
--rw-r--r--   0 runner     (501) staff       (20)     1937 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/packet.go
--rw-r--r--   0 runner     (501) staff       (20)     1173 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/pipe.go
--rw-r--r--   0 runner     (501) staff       (20)     1511 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/singbridge/reader.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.828191 Xray-core-1.8.8/xray-go/common/strmatcher/
--rw-r--r--   0 runner     (501) staff       (20)     4156 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/ac_automaton_matcher.go
--rw-r--r--   0 runner     (501) staff       (20)     1136 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/benchmark_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1804 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/domain_matcher.go
--rw-r--r--   0 runner     (501) staff       (20)     1287 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/domain_matcher_test.go
--rw-r--r--   0 runner     (501) staff       (20)      494 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/full_matcher.go
--rw-r--r--   0 runner     (501) staff       (20)      909 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/full_matcher_test.go
--rw-r--r--   0 runner     (501) staff       (20)      919 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/matchers.go
--rw-r--r--   0 runner     (501) staff       (20)     1298 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/matchers_test.go
--rw-r--r--   0 runner     (501) staff       (20)     7077 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/mph_matcher.go
--rw-r--r--   0 runner     (501) staff       (20)     2659 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/strmatcher.go
--rw-r--r--   0 runner     (501) staff       (20)     4455 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/strmatcher/strmatcher_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.830437 Xray-core-1.8.8/xray-go/common/task/
--rw-r--r--   0 runner     (501) staff       (20)      192 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/task/common.go
--rw-r--r--   0 runner     (501) staff       (20)     1264 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/task/periodic.go
--rw-r--r--   0 runner     (501) staff       (20)      668 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/task/periodic_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1082 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/task/task.go
--rw-r--r--   0 runner     (501) staff       (20)     1346 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/task/task_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1080 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/type.go
--rw-r--r--   0 runner     (501) staff       (20)      797 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/type_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.831247 Xray-core-1.8.8/xray-go/common/units/
--rw-r--r--   0 runner     (501) staff       (20)     1874 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/units/bytesize.go
--rw-r--r--   0 runner     (501) staff       (20)     1218 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/units/bytesize_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.832115 Xray-core-1.8.8/xray-go/common/uuid/
--rw-r--r--   0 runner     (501) staff       (20)     2177 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/uuid/uuid.go
--rw-r--r--   0 runner     (501) staff       (20)     1823 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/uuid/uuid_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.833545 Xray-core-1.8.8/xray-go/common/xudp/
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/xudp/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     4974 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/xudp/xudp.go
--rw-r--r--   0 runner     (501) staff       (20)      787 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/common/xudp/xudp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.840140 Xray-core-1.8.8/xray-go/core/
--rw-r--r--   0 runner     (501) staff       (20)      675 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/annotations.go
--rw-r--r--   0 runner     (501) staff       (20)     4402 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/config.go
--rw-r--r--   0 runner     (501) staff       (20)    17234 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     2402 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     1537 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/context.go
--rw-r--r--   0 runner     (501) staff       (20)      280 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/context_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1335 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/core.go
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      182 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/format.go
--rw-r--r--   0 runner     (501) staff       (20)     2758 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/functions.go
--rw-r--r--   0 runner     (501) staff       (20)     4894 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/functions_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/mocks.go
--rw-r--r--   0 runner     (501) staff       (20)      233 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/proto.go
--rw-r--r--   0 runner     (501) staff       (20)     9066 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/xray.go
--rw-r--r--   0 runner     (501) staff       (20)     2404 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/core/xray_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.840934 Xray-core-1.8.8/xray-go/features/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.841875 Xray-core-1.8.8/xray-go/features/dns/
--rw-r--r--   0 runner     (501) staff       (20)     1260 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/dns/client.go
--rw-r--r--   0 runner     (501) staff       (20)      472 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/dns/fakedns.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.842630 Xray-core-1.8.8/xray-go/features/dns/localdns/
--rw-r--r--   0 runner     (501) staff       (20)     1418 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/dns/localdns/client.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/dns/localdns/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.843566 Xray-core-1.8.8/xray-go/features/extension/
--rw-r--r--   0 runner     (501) staff       (20)      108 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/extension/contextreceiver.go
--rw-r--r--   0 runner     (501) staff       (20)      295 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/extension/observatory.go
--rw-r--r--   0 runner     (501) staff       (20)      707 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/feature.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.843977 Xray-core-1.8.8/xray-go/features/inbound/
--rw-r--r--   0 runner     (501) staff       (20)     1078 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/inbound/inbound.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.844354 Xray-core-1.8.8/xray-go/features/outbound/
--rw-r--r--   0 runner     (501) staff       (20)     1212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/outbound/outbound.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.845068 Xray-core-1.8.8/xray-go/features/policy/
--rw-r--r--   0 runner     (501) staff       (20)      691 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/policy/default.go
--rw-r--r--   0 runner     (501) staff       (20)     4058 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/policy/policy.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.846730 Xray-core-1.8.8/xray-go/features/routing/
--rw-r--r--   0 runner     (501) staff       (20)      240 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/routing/balancer.go
--rw-r--r--   0 runner     (501) staff       (20)     1285 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/routing/context.go
--rw-r--r--   0 runner     (501) staff       (20)      844 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/routing/dispatcher.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.847566 Xray-core-1.8.8/xray-go/features/routing/dns/
--rw-r--r--   0 runner     (501) staff       (20)     1293 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/routing/dns/context.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/routing/dns/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1469 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/routing/router.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.847903 Xray-core-1.8.8/xray-go/features/routing/session/
--rw-r--r--   0 runner     (501) staff       (20)     3105 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/routing/session/context.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.848811 Xray-core-1.8.8/xray-go/features/stats/
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/stats/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     4445 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/features/stats/stats.go
--rw-r--r--   0 runner     (501) staff       (20)     2533 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/go.mod
--rw-r--r--   0 runner     (501) staff       (20)    30993 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/go.sum
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.609050 Xray-core-1.8.8/xray-go/infra/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.872460 Xray-core-1.8.8/xray-go/infra/conf/
--rw-r--r--   0 runner     (501) staff       (20)     1501 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/api.go
--rw-r--r--   0 runner     (501) staff       (20)     1156 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/blackhole.go
--rw-r--r--   0 runner     (501) staff       (20)      610 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/blackhole_test.go
--rw-r--r--   0 runner     (501) staff       (20)      118 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/buildable.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.608284 Xray-core-1.8.8/xray-go/infra/conf/cfgcommon/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.873528 Xray-core-1.8.8/xray-go/infra/conf/cfgcommon/duration/
--rw-r--r--   0 runner     (501) staff       (20)      557 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/cfgcommon/duration/duration.go
--rw-r--r--   0 runner     (501) staff       (20)      654 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/cfgcommon/duration/duration_test.go
--rw-r--r--   0 runner     (501) staff       (20)     5580 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/common.go
--rw-r--r--   0 runner     (501) staff       (20)     5094 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/common_test.go
--rw-r--r--   0 runner     (501) staff       (20)       84 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/conf.go
--rw-r--r--   0 runner     (501) staff       (20)    10224 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/dns.go
--rw-r--r--   0 runner     (501) staff       (20)      853 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/dns_proxy.go
--rw-r--r--   0 runner     (501) staff       (20)      638 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/dns_proxy_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3745 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/dns_test.go
--rw-r--r--   0 runner     (501) staff       (20)      754 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/dokodemo.go
--rw-r--r--   0 runner     (501) staff       (20)      794 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/dokodemo_test.go
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3408 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/fakedns.go
--rw-r--r--   0 runner     (501) staff       (20)     5592 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/freedom.go
--rw-r--r--   0 runner     (501) staff       (20)      881 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/freedom_test.go
--rw-r--r--   0 runner     (501) staff       (20)      877 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/general_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1091 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/grpc.go
--rw-r--r--   0 runner     (501) staff       (20)     2373 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/http.go
--rw-r--r--   0 runner     (501) staff       (20)      686 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/http_test.go
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/init.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.874303 Xray-core-1.8.8/xray-go/infra/conf/json/
--rw-r--r--   0 runner     (501) staff       (20)     2564 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/json/reader.go
--rw-r--r--   0 runner     (501) staff       (20)     1927 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/json/reader_test.go
--rw-r--r--   0 runner     (501) staff       (20)      719 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/lint.go
--rw-r--r--   0 runner     (501) staff       (20)     1893 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/loader.go
--rw-r--r--   0 runner     (501) staff       (20)     1439 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/log.go
--rw-r--r--   0 runner     (501) staff       (20)      292 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/loopback.go
--rw-r--r--   0 runner     (501) staff       (20)      307 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/metrics.go
--rw-r--r--   0 runner     (501) staff       (20)     1173 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/observatory.go
--rw-r--r--   0 runner     (501) staff       (20)     2355 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/policy.go
--rw-r--r--   0 runner     (501) staff       (20)      591 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/policy_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1118 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/reverse.go
--rw-r--r--   0 runner     (501) staff       (20)      815 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/reverse_test.go
--rw-r--r--   0 runner     (501) staff       (20)    17937 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/router.go
--rw-r--r--   0 runner     (501) staff       (20)     2659 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/router_strategy.go
--rw-r--r--   0 runner     (501) staff       (20)     7374 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/router_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.877652 Xray-core-1.8.8/xray-go/infra/conf/serial/
--rw-r--r--   0 runner     (501) staff       (20)     1938 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/serial/builder.go
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/serial/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3606 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/serial/loader.go
--rw-r--r--   0 runner     (501) staff       (20)     1054 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/serial/loader_test.go
--rw-r--r--   0 runner     (501) staff       (20)       86 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/serial/serial.go
--rw-r--r--   0 runner     (501) staff       (20)     7303 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/shadowsocks.go
--rw-r--r--   0 runner     (501) staff       (20)      831 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/shadowsocks_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3204 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/socks.go
--rw-r--r--   0 runner     (501) staff       (20)     1827 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/socks_test.go
--rw-r--r--   0 runner     (501) staff       (20)     3057 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/transport.go
--rw-r--r--   0 runner     (501) staff       (20)     5619 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/transport_authenticators.go
--rw-r--r--   0 runner     (501) staff       (20)    27364 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/transport_internet.go
--rw-r--r--   0 runner     (501) staff       (20)     7387 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/transport_test.go
--rw-r--r--   0 runner     (501) staff       (20)     4746 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/trojan.go
--rw-r--r--   0 runner     (501) staff       (20)     5676 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/vless.go
--rw-r--r--   0 runner     (501) staff       (20)     2658 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/vless_test.go
--rw-r--r--   0 runner     (501) staff       (20)     4340 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/vmess.go
--rw-r--r--   0 runner     (501) staff       (20)     2345 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/vmess_test.go
--rw-r--r--   0 runner     (501) staff       (20)     4056 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/wireguard.go
--rw-r--r--   0 runner     (501) staff       (20)     1393 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/wireguard_test.go
--rw-r--r--   0 runner     (501) staff       (20)    20968 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/xray.go
--rw-r--r--   0 runner     (501) staff       (20)    13294 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/conf/xray_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.878179 Xray-core-1.8.8/xray-go/infra/vformat/
--rw-r--r--   0 runner     (501) staff       (20)     4711 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/vformat/main.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.878730 Xray-core-1.8.8/xray-go/infra/vprotogen/
--rw-r--r--   0 runner     (501) staff       (20)     6562 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/infra/vprotogen/main.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.881635 Xray-core-1.8.8/xray-go/main/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.609934 Xray-core-1.8.8/xray-go/main/commands/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.884933 Xray-core-1.8.8/xray-go/main/commands/all/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.892712 Xray-core-1.8.8/xray-go/main/commands/all/api/
--rw-r--r--   0 runner     (501) staff       (20)      523 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/api.go
--rw-r--r--   0 runner     (501) staff       (20)     2467 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/balancer_info.go
--rw-r--r--   0 runner     (501) staff       (20)     1760 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/balancer_override.go
--rw-r--r--   0 runner     (501) staff       (20)     1778 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/inbounds_add.go
--rw-r--r--   0 runner     (501) staff       (20)     1778 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/inbounds_remove.go
--rw-r--r--   0 runner     (501) staff       (20)      885 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/logger_restart.go
--rw-r--r--   0 runner     (501) staff       (20)     1797 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/outbounds_add.go
--rw-r--r--   0 runner     (501) staff       (20)     1749 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/outbounds_remove.go
--rw-r--r--   0 runner     (501) staff       (20)     3683 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/shared.go
--rw-r--r--   0 runner     (501) staff       (20)     1179 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/stats_get.go
--rw-r--r--   0 runner     (501) staff       (20)     1717 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/stats_query.go
--rw-r--r--   0 runner     (501) staff       (20)      872 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/api/stats_sys.go
--rw-r--r--   0 runner     (501) staff       (20)      410 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/commands.go
--rw-r--r--   0 runner     (501) staff       (20)     2774 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/convert.go
--rw-r--r--   0 runner     (501) staff       (20)     1232 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/curve25519.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.895303 Xray-core-1.8.8/xray-go/main/commands/all/tls/
--rw-r--r--   0 runner     (501) staff       (20)     3729 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/tls/cert.go
--rw-r--r--   0 runner     (501) staff       (20)      966 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/tls/certchainhash.go
--rw-r--r--   0 runner     (501) staff       (20)     3093 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/tls/ping.go
--rw-r--r--   0 runner     (501) staff       (20)      327 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/tls/tls.go
--rw-r--r--   0 runner     (501) staff       (20)      772 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/uuid.go
--rw-r--r--   0 runner     (501) staff       (20)      589 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/wg.go
--rw-r--r--   0 runner     (501) staff       (20)      754 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/all/x25519.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.897976 Xray-core-1.8.8/xray-go/main/commands/base/
--rw-r--r--   0 runner     (501) staff       (20)     3499 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/base/command.go
--rw-r--r--   0 runner     (501) staff       (20)      481 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/base/env.go
--rw-r--r--   0 runner     (501) staff       (20)     1940 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/base/execute.go
--rw-r--r--   0 runner     (501) staff       (20)     4055 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/base/help.go
--rw-r--r--   0 runner     (501) staff       (20)      349 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/commands/base/root.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.899074 Xray-core-1.8.8/xray-go/main/confloader/
--rw-r--r--   0 runner     (501) staff       (20)      923 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/confloader/confloader.go
--rw-r--r--   0 runner     (501) staff       (20)      219 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/confloader/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.900035 Xray-core-1.8.8/xray-go/main/confloader/external/
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/confloader/external/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1881 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/confloader/external/external.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.610648 Xray-core-1.8.8/xray-go/main/distro/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.900631 Xray-core-1.8.8/xray-go/main/distro/all/
--rw-r--r--   0 runner     (501) staff       (20)     3304 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/distro/all/all.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.901537 Xray-core-1.8.8/xray-go/main/distro/debug/
--rw-r--r--   0 runner     (501) staff       (20)      109 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/distro/debug/debug.go
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.902710 Xray-core-1.8.8/xray-go/main/json/
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/json/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1286 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/json/json.go
--rw-r--r--   0 runner     (501) staff       (20)     1426 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/main.go
--rw-r--r--   0 runner     (501) staff       (20)      139 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/main_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6648 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/run.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.904074 Xray-core-1.8.8/xray-go/main/toml/
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/toml/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1286 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/toml/toml.go
--rw-r--r--   0 runner     (501) staff       (20)      505 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/version.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.905405 Xray-core-1.8.8/xray-go/main/yaml/
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/yaml/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1293 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/main/yaml/yaml.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.906465 Xray-core-1.8.8/xray-go/proxy/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.911799 Xray-core-1.8.8/xray-go/proxy/blackhole/
--rw-r--r--   0 runner     (501) staff       (20)     1369 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/blackhole/blackhole.go
--rw-r--r--   0 runner     (501) staff       (20)      896 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/blackhole/blackhole_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1111 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/blackhole/config.go
--rw-r--r--   0 runner     (501) staff       (20)     8717 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/blackhole/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      413 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/blackhole/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      543 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/blackhole/config_test.go
--rw-r--r--   0 runner     (501) staff       (20)      218 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/blackhole/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.915672 Xray-core-1.8.8/xray-go/proxy/dns/
--rw-r--r--   0 runner     (501) staff       (20)     6221 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dns/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      476 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dns/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     8342 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dns/dns.go
--rw-r--r--   0 runner     (501) staff       (20)     9341 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dns/dns_test.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dns/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.920427 Xray-core-1.8.8/xray-go/proxy/dokodemo/
--rw-r--r--   0 runner     (501) staff       (20)      305 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dokodemo/config.go
--rw-r--r--   0 runner     (501) staff       (20)     9235 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dokodemo/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      741 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dokodemo/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     8027 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dokodemo/dokodemo.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dokodemo/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1801 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dokodemo/fakeudp_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/dokodemo/fakeudp_other.go
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.924950 Xray-core-1.8.8/xray-go/proxy/freedom/
--rw-r--r--   0 runner     (501) staff       (20)     1337 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/freedom/config.go
--rw-r--r--   0 runner     (501) staff       (20)    18291 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/freedom/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1001 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/freedom/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/freedom/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)    11789 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/freedom/freedom.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.930567 Xray-core-1.8.8/xray-go/proxy/http/
--rw-r--r--   0 runner     (501) staff       (20)     9415 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/http/client.go
--rw-r--r--   0 runner     (501) staff       (20)      512 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/http/config.go
--rw-r--r--   0 runner     (501) staff       (20)    14511 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/http/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      816 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/http/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/http/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)       84 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/http/http.go
--rw-r--r--   0 runner     (501) staff       (20)     9569 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/http/server.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.934511 Xray-core-1.8.8/xray-go/proxy/loopback/
--rw-r--r--   0 runner     (501) staff       (20)       88 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/loopback/config.go
--rw-r--r--   0 runner     (501) staff       (20)     5150 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/loopback/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      292 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/loopback/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/loopback/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3211 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/loopback/loopback.go
--rw-r--r--   0 runner     (501) staff       (20)    17405 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/proxy.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.939684 Xray-core-1.8.8/xray-go/proxy/shadowsocks/
--rw-r--r--   0 runner     (501) staff       (20)     5799 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/client.go
--rw-r--r--   0 runner     (501) staff       (20)     6146 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/config.go
--rw-r--r--   0 runner     (501) staff       (20)    14546 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      815 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      897 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/config_test.go
--rw-r--r--   0 runner     (501) staff       (20)      220 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     9468 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/protocol.go
--rw-r--r--   0 runner     (501) staff       (20)     5516 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/protocol_test.go
--rw-r--r--   0 runner     (501) staff       (20)     7831 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/server.go
--rw-r--r--   0 runner     (501) staff       (20)      293 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/shadowsocks.go
--rw-r--r--   0 runner     (501) staff       (20)     2996 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks/validator.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.943726 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/
--rw-r--r--   0 runner     (501) staff       (20)      627 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/config.go
--rw-r--r--   0 runner     (501) staff       (20)    24779 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1222 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      225 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     4911 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/inbound.go
--rw-r--r--   0 runner     (501) staff       (20)     7146 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/inbound_multi.go
--rw-r--r--   0 runner     (501) staff       (20)     5661 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/inbound_relay.go
--rw-r--r--   0 runner     (501) staff       (20)     4641 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/outbound.go
--rw-r--r--   0 runner     (501) staff       (20)       96 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/shadowsocks_2022.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.947846 Xray-core-1.8.8/xray-go/proxy/socks/
--rw-r--r--   0 runner     (501) staff       (20)     6315 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/client.go
--rw-r--r--   0 runner     (501) staff       (20)      526 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/config.go
--rw-r--r--   0 runner     (501) staff       (20)    17186 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1179 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)    13429 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/protocol.go
--rw-r--r--   0 runner     (501) staff       (20)     2944 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/protocol_test.go
--rw-r--r--   0 runner     (501) staff       (20)     8076 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/server.go
--rw-r--r--   0 runner     (501) staff       (20)      153 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/socks/socks.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.952231 Xray-core-1.8.8/xray-go/proxy/trojan/
--rw-r--r--   0 runner     (501) staff       (20)     5044 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/client.go
--rw-r--r--   0 runner     (501) staff       (20)     1039 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/config.go
--rw-r--r--   0 runner     (501) staff       (20)    13473 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      694 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      215 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     5726 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/protocol.go
--rw-r--r--   0 runner     (501) staff       (20)     2352 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/protocol_test.go
--rw-r--r--   0 runner     (501) staff       (20)    15608 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/server.go
--rw-r--r--   0 runner     (501) staff       (20)       86 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/trojan.go
--rw-r--r--   0 runner     (501) staff       (20)     1230 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/trojan/validator.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.954664 Xray-core-1.8.8/xray-go/proxy/vless/
--rw-r--r--   0 runner     (501) staff       (20)     1043 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/account.go
--rw-r--r--   0 runner     (501) staff       (20)     5752 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/account.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      544 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/account.proto
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.957310 Xray-core-1.8.8/xray-go/proxy/vless/encoding/
--rw-r--r--   0 runner     (501) staff       (20)     4835 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/encoding/addons.go
--rw-r--r--   0 runner     (501) staff       (20)     5668 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/encoding/addons.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      327 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/encoding/addons.proto
--rw-r--r--   0 runner     (501) staff       (20)     7892 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/encoding/encoding.go
--rw-r--r--   0 runner     (501) staff       (20)     3286 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/encoding/encoding_test.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/encoding/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.959520 Xray-core-1.8.8/xray-go/proxy/vless/inbound/
--rw-r--r--   0 runner     (501) staff       (20)       16 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/inbound/config.go
--rw-r--r--   0 runner     (501) staff       (20)    10235 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/inbound/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      663 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/inbound/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/inbound/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)    18633 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/inbound/inbound.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.962448 Xray-core-1.8.8/xray-go/proxy/vless/outbound/
--rw-r--r--   0 runner     (501) staff       (20)       17 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/outbound/config.go
--rw-r--r--   0 runner     (501) staff       (20)     6130 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/outbound/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      393 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/outbound/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/outbound/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)    10135 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/outbound/outbound.go
--rw-r--r--   0 runner     (501) staff       (20)     1249 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/validator.go
--rw-r--r--   0 runner     (501) staff       (20)      441 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vless/vless.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.966949 Xray-core-1.8.8/xray-go/proxy/vmess/
--rw-r--r--   0 runner     (501) staff       (20)     1397 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/account.go
--rw-r--r--   0 runner     (501) staff       (20)     6722 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/account.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      596 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/account.proto
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.970868 Xray-core-1.8.8/xray-go/proxy/vmess/aead/
--rw-r--r--   0 runner     (501) staff       (20)     2740 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/aead/authid.go
--rw-r--r--   0 runner     (501) staff       (20)     3322 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/aead/authid_test.go
--rw-r--r--   0 runner     (501) staff       (20)      748 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/aead/consts.go
--rw-r--r--   0 runner     (501) staff       (20)     5214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/aead/encrypt.go
--rw-r--r--   0 runner     (501) staff       (20)     2529 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/aead/encrypt_test.go
--rw-r--r--   0 runner     (501) staff       (20)      521 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/aead/kdf.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.975077 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/
--rw-r--r--   0 runner     (501) staff       (20)     2174 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/auth.go
--rw-r--r--   0 runner     (501) staff       (20)    13755 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/client.go
--rw-r--r--   0 runner     (501) staff       (20)     3664 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/commands.go
--rw-r--r--   0 runner     (501) staff       (20)     1200 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/commands_test.go
--rw-r--r--   0 runner     (501) staff       (20)      547 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/encoding.go
--rw-r--r--   0 runner     (501) staff       (20)     3787 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/encoding_test.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)    16319 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/encoding/server.go
--rw-r--r--   0 runner     (501) staff       (20)      214 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.978293 Xray-core-1.8.8/xray-go/proxy/vmess/inbound/
--rw-r--r--   0 runner     (501) staff       (20)      208 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/inbound/config.go
--rw-r--r--   0 runner     (501) staff       (20)    10805 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/inbound/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      546 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/inbound/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/inbound/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     9906 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/inbound/inbound.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.981935 Xray-core-1.8.8/xray-go/proxy/vmess/outbound/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/outbound/command.go
--rw-r--r--   0 runner     (501) staff       (20)       17 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/outbound/config.go
--rw-r--r--   0 runner     (501) staff       (20)     6185 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/outbound/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      396 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/outbound/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/outbound/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     7808 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/outbound/outbound.go
--rw-r--r--   0 runner     (501) staff       (20)     2341 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/validator.go
--rw-r--r--   0 runner     (501) staff       (20)      624 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/validator_test.go
--rw-r--r--   0 runner     (501) staff       (20)      404 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/vmess/vmess.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.986836 Xray-core-1.8.8/xray-go/proxy/wireguard/
--rw-r--r--   0 runner     (501) staff       (20)     4823 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/bind.go
--rw-r--r--   0 runner     (501) staff       (20)     9221 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/client.go
--rw-r--r--   0 runner     (501) staff       (20)      868 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/config.go
--rw-r--r--   0 runner     (501) staff       (20)    15221 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      218 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/errors.generated.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.987164 Xray-core-1.8.8/xray-go/proxy/wireguard/gvisortun/
--rw-r--r--   0 runner     (501) staff       (20)     5829 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/gvisortun/tun.go
--rw-r--r--   0 runner     (501) staff       (20)     4715 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/server.go
--rw-r--r--   0 runner     (501) staff       (20)     4945 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/tun.go
--rw-r--r--   0 runner     (501) staff       (20)      294 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/tun_default.go
--rw-r--r--   0 runner     (501) staff       (20)     5828 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/tun_linux.go
--rw-r--r--   0 runner     (501) staff       (20)     2720 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/proxy/wireguard/wireguard.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.615309 Xray-core-1.8.8/xray-go/testing/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.988105 Xray-core-1.8.8/xray-go/testing/coverage/
--rw-r--r--   0 runner     (501) staff       (20)     1347 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/coverage/coverall
--rw-r--r--   0 runner     (501) staff       (20)     1139 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/coverage/coverall2
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.990995 Xray-core-1.8.8/xray-go/testing/mocks/
--rw-r--r--   0 runner     (501) staff       (20)     2616 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/mocks/dns.go
--rw-r--r--   0 runner     (501) staff       (20)     2234 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/mocks/io.go
--rw-r--r--   0 runner     (501) staff       (20)     1294 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/mocks/log.go
--rw-r--r--   0 runner     (501) staff       (20)     1597 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/mocks/mux.go
--rw-r--r--   0 runner     (501) staff       (20)     5670 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/mocks/outbound.go
--rw-r--r--   0 runner     (501) staff       (20)     3379 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/mocks/proxy.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.000372 Xray-core-1.8.8/xray-go/testing/scenarios/
--rw-r--r--   0 runner     (501) staff       (20)    13144 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/command_test.go
--rw-r--r--   0 runner     (501) staff       (20)     5824 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/common.go
--rw-r--r--   0 runner     (501) staff       (20)      905 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/common_coverage.go
--rw-r--r--   0 runner     (501) staff       (20)      670 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/common_regular.go
--rw-r--r--   0 runner     (501) staff       (20)     2552 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/dns_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6351 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/dokodemo_test.go
--rw-r--r--   0 runner     (501) staff       (20)    19392 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/feature_test.go
--rw-r--r--   0 runner     (501) staff       (20)     9222 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/http_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2817 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/metrics_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6746 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/policy_test.go
--rw-r--r--   0 runner     (501) staff       (20)    10001 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/reverse_test.go
--rw-r--r--   0 runner     (501) staff       (20)     6111 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/shadowsocks_2022_test.go
--rw-r--r--   0 runner     (501) staff       (20)    12812 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/shadowsocks_test.go
--rw-r--r--   0 runner     (501) staff       (20)    11796 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/socks_test.go
--rw-r--r--   0 runner     (501) staff       (20)    35148 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/tls_test.go
--rw-r--r--   0 runner     (501) staff       (20)    10641 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/transport_test.go
--rw-r--r--   0 runner     (501) staff       (20)    14588 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/vless_test.go
--rw-r--r--   0 runner     (501) staff       (20)    39891 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/scenarios/vmess_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.615662 Xray-core-1.8.8/xray-go/testing/servers/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.000885 Xray-core-1.8.8/xray-go/testing/servers/http/
--rw-r--r--   0 runner     (501) staff       (20)      806 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/servers/http/http.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.001714 Xray-core-1.8.8/xray-go/testing/servers/tcp/
--rw-r--r--   0 runner     (501) staff       (20)      416 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/servers/tcp/port.go
--rw-r--r--   0 runner     (501) staff       (20)     2437 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/servers/tcp/tcp.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.002695 Xray-core-1.8.8/xray-go/testing/servers/udp/
--rw-r--r--   0 runner     (501) staff       (20)      456 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/servers/udp/port.go
--rw-r--r--   0 runner     (501) staff       (20)     1293 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/testing/servers/udp/udp.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.003211 Xray-core-1.8.8/xray-go/transport/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.004933 Xray-core-1.8.8/xray-go/transport/global/
--rw-r--r--   0 runner     (501) staff       (20)      239 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/global/config.go
--rw-r--r--   0 runner     (501) staff       (20)     6340 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/global/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      552 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/global/config.proto
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.016834 Xray-core-1.8.8/xray-go/transport/internet/
--rw-r--r--   0 runner     (501) staff       (20)     4250 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/config.go
--rw-r--r--   0 runner     (501) staff       (20)    34916 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     2637 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     5348 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)      643 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/dialer_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.020209 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/
--rw-r--r--   0 runner     (501) staff       (20)      749 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/config.go
--rw-r--r--   0 runner     (501) staff       (20)     7156 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      814 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     1194 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/dial.go
--rw-r--r--   0 runner     (501) staff       (20)       92 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/errgen.go
--rw-r--r--   0 runner     (501) staff       (20)      221 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3289 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/listener.go
--rw-r--r--   0 runner     (501) staff       (20)     2143 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/domainsocket/listener_test.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/filelocker.go
--rw-r--r--   0 runner     (501) staff       (20)      813 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/filelocker_other.go
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/filelocker_windows.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.024301 Xray-core-1.8.8/xray-go/transport/internet/grpc/
--rw-r--r--   0 runner     (501) staff       (20)     1763 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/config.go
--rw-r--r--   0 runner     (501) staff       (20)     8620 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      382 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     2685 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/config_test.go
--rw-r--r--   0 runner     (501) staff       (20)     5888 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/dial.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.028014 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/
--rw-r--r--   0 runner     (501) staff       (20)     1912 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/customSeviceName.go
--rw-r--r--   0 runner     (501) staff       (20)       88 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/encoding.go
--rw-r--r--   0 runner     (501) staff       (20)      217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     2890 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/hunkconn.go
--rw-r--r--   0 runner     (501) staff       (20)     2776 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/multiconn.go
--rw-r--r--   0 runner     (501) staff       (20)     9247 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/stream.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      370 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/stream.proto
--rw-r--r--   0 runner     (501) staff       (20)     6127 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/stream_grpc.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)       84 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/grpc.go
--rw-r--r--   0 runner     (501) staff       (20)     4110 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/grpc/hub.go
--rw-r--r--   0 runner     (501) staff       (20)      847 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/header.go
--rw-r--r--   0 runner     (501) staff       (20)     1054 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/header_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:24.618109 Xray-core-1.8.8/xray-go/transport/internet/headers/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.029465 Xray-core-1.8.8/xray-go/transport/internet/headers/dns/
--rw-r--r--   0 runner     (501) staff       (20)     6023 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/dns/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      354 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/dns/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     2812 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/dns/dns.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.033127 Xray-core-1.8.8/xray-go/transport/internet/headers/http/
--rw-r--r--   0 runner     (501) staff       (20)     1910 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/config.go
--rw-r--r--   0 runner     (501) staff       (20)    23417 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1514 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     7328 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/http.go
--rw-r--r--   0 runner     (501) staff       (20)     6589 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/http_test.go
--rw-r--r--   0 runner     (501) staff       (20)      203 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/linkedreadRequest.go
--rw-r--r--   0 runner     (501) staff       (20)      717 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/http/resp.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.034271 Xray-core-1.8.8/xray-go/transport/internet/headers/noop/
--rw-r--r--   0 runner     (501) staff       (20)     7365 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/noop/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      362 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/noop/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      813 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/noop/noop.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.036160 Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/
--rw-r--r--   0 runner     (501) staff       (20)     7967 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      470 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      684 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/srtp.go
--rw-r--r--   0 runner     (501) staff       (20)      637 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/srtp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.037949 Xray-core-1.8.8/xray-go/transport/internet/headers/tls/
--rw-r--r--   0 runner     (501) staff       (20)     5808 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/tls/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      335 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/tls/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     1086 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/tls/dtls.go
--rw-r--r--   0 runner     (501) staff       (20)      622 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/tls/dtls_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.039733 Xray-core-1.8.8/xray-go/transport/internet/headers/utp/
--rw-r--r--   0 runner     (501) staff       (20)     6040 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/utp/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      352 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/utp/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      712 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/utp/utp.go
--rw-r--r--   0 runner     (501) staff       (20)      579 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/utp/utp_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.041673 Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/
--rw-r--r--   0 runner     (501) staff       (20)     5975 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      346 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      794 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/wechat.go
--rw-r--r--   0 runner     (501) staff       (20)      541 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/wechat_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.043393 Xray-core-1.8.8/xray-go/transport/internet/headers/wireguard/
--rw-r--r--   0 runner     (501) staff       (20)     6227 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/wireguard/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      362 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/wireguard/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      554 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/headers/wireguard/wireguard.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.047133 Xray-core-1.8.8/xray-go/transport/internet/http/
--rw-r--r--   0 runner     (501) staff       (20)      836 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/config.go
--rw-r--r--   0 runner     (501) staff       (20)     8400 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      553 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     6845 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)       84 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/http.go
--rw-r--r--   0 runner     (501) staff       (20)     2140 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/http_test.go
--rw-r--r--   0 runner     (501) staff       (20)     5417 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/http/hub.go
--rw-r--r--   0 runner     (501) staff       (20)       88 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/internet.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.058548 Xray-core-1.8.8/xray-go/transport/internet/kcp/
--rw-r--r--   0 runner     (501) staff       (20)     2517 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/config.go
--rw-r--r--   0 runner     (501) staff       (20)    26474 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     1223 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/config.proto
--rw-r--r--   0 runner     (501) staff       (20)    14828 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/connection.go
--rw-r--r--   0 runner     (501) staff       (20)      789 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/connection_test.go
--rw-r--r--   0 runner     (501) staff       (20)     1738 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/crypt.go
--rw-r--r--   0 runner     (501) staff       (20)      803 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/crypt_test.go
--rw-r--r--   0 runner     (501) staff       (20)      345 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/cryptreal.go
--rw-r--r--   0 runner     (501) staff       (20)     2452 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1853 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/io.go
--rw-r--r--   0 runner     (501) staff       (20)      653 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/io_test.go
--rw-r--r--   0 runner     (501) staff       (20)      254 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/kcp.go
--rw-r--r--   0 runner     (501) staff       (20)     2078 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/kcp_test.go
--rw-r--r--   0 runner     (501) staff       (20)     4441 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/listener.go
--rw-r--r--   0 runner     (501) staff       (20)      934 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/output.go
--rw-r--r--   0 runner     (501) staff       (20)     4941 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/receiving.go
--rw-r--r--   0 runner     (501) staff       (20)     6019 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/segment.go
--rw-r--r--   0 runner     (501) staff       (20)     2146 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/segment_test.go
--rw-r--r--   0 runner     (501) staff       (20)     7405 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/sending.go
--rw-r--r--   0 runner     (501) staff       (20)      358 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/xor.go
--rw-r--r--   0 runner     (501) staff       (20)       86 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/xor_amd64.go
--rw-r--r--   0 runner     (501) staff       (20)      752 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/kcp/xor_amd64.s
--rw-r--r--   0 runner     (501) staff       (20)      978 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/memory_settings.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.065520 Xray-core-1.8.8/xray-go/transport/internet/quic/
--rw-r--r--   0 runner     (501) staff       (20)     1024 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/config.go
--rw-r--r--   0 runner     (501) staff       (20)     7620 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      503 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     3919 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/conn.go
--rw-r--r--   0 runner     (501) staff       (20)     5717 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3605 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/hub.go
--rw-r--r--   0 runner     (501) staff       (20)      250 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/pool.go
--rw-r--r--   0 runner     (501) staff       (20)      483 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/qlogWriter.go
--rw-r--r--   0 runner     (501) staff       (20)      583 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/quic.go
--rw-r--r--   0 runner     (501) staff       (20)     4919 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/quic/quic_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.068505 Xray-core-1.8.8/xray-go/transport/internet/reality/
--rw-r--r--   0 runner     (501) staff       (20)     1473 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/reality/config.go
--rw-r--r--   0 runner     (501) staff       (20)    11995 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/reality/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      755 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/reality/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      216 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/reality/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     8620 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/reality/reality.go
--rw-r--r--   0 runner     (501) staff       (20)      419 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt.go
--rw-r--r--   0 runner     (501) staff       (20)     7670 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt_darwin.go
--rw-r--r--   0 runner     (501) staff       (20)     7894 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt_freebsd.go
--rw-r--r--   0 runner     (501) staff       (20)     7128 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      967 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt_linux_test.go
--rw-r--r--   0 runner     (501) staff       (20)      504 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt_other.go
--rw-r--r--   0 runner     (501) staff       (20)      866 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt_test.go
--rw-r--r--   0 runner     (501) staff       (20)     2811 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/sockopt_windows.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.068909 Xray-core-1.8.8/xray-go/transport/internet/stat/
--rw-r--r--   0 runner     (501) staff       (20)      592 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/stat/connection.go
--rw-r--r--   0 runner     (501) staff       (20)     5984 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/system_dialer.go
--rw-r--r--   0 runner     (501) staff       (20)     4506 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/system_listener.go
--rw-r--r--   0 runner     (501) staff       (20)      701 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/system_listener_test.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.069401 Xray-core-1.8.8/xray-go/transport/internet/tagged/
--rw-r--r--   0 runner     (501) staff       (20)      193 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tagged/tagged.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.070882 Xray-core-1.8.8/xray-go/transport/internet/tagged/taggedimpl/
--rw-r--r--   0 runner     (501) staff       (20)      219 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tagged/taggedimpl/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     1352 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tagged/taggedimpl/impl.go
--rw-r--r--   0 runner     (501) staff       (20)       90 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tagged/taggedimpl/taggedimpl.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.077073 Xray-core-1.8.8/xray-go/transport/internet/tcp/
--rw-r--r--   0 runner     (501) staff       (20)      266 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/config.go
--rw-r--r--   0 runner     (501) staff       (20)     7028 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      446 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     1932 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     4073 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/hub.go
--rw-r--r--   0 runner     (501) staff       (20)      688 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_darwin.go
--rw-r--r--   0 runner     (501) staff       (20)      690 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_freebsd.go
--rw-r--r--   0 runner     (501) staff       (20)     1352 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      777 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_linux_test.go
--rw-r--r--   0 runner     (501) staff       (20)      304 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_other.go
--rw-r--r--   0 runner     (501) staff       (20)       83 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp/tcp.go
--rw-r--r--   0 runner     (501) staff       (20)     2907 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tcp_hub.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.082912 Xray-core-1.8.8/xray-go/transport/internet/tls/
--rw-r--r--   0 runner     (501) staff       (20)    11614 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/config.go
--rw-r--r--   0 runner     (501) staff       (20)    21489 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)     2272 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      902 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/config_other.go
--rw-r--r--   0 runner     (501) staff       (20)     2530 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/config_test.go
--rw-r--r--   0 runner     (501) staff       (20)      209 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/config_windows.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     3042 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/grpc.go
--rw-r--r--   0 runner     (501) staff       (20)      946 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/pin.go
--rw-r--r--   0 runner     (501) staff       (20)    11080 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/pin_test.go
--rw-r--r--   0 runner     (501) staff       (20)     7230 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/tls.go
--rw-r--r--   0 runner     (501) staff       (20)      121 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/tls/unsafe.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.089462 Xray-core-1.8.8/xray-go/transport/internet/udp/
--rw-r--r--   0 runner     (501) staff       (20)      238 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/config.go
--rw-r--r--   0 runner     (501) staff       (20)     5217 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      297 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/config.proto
--rw-r--r--   0 runner     (501) staff       (20)      706 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)     5014 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/dispatcher.go
--rw-r--r--   0 runner     (501) staff       (20)     2176 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/dispatcher_test.go
--rw-r--r--   0 runner     (501) staff       (20)      212 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     2783 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/hub.go
--rw-r--r--   0 runner     (501) staff       (20)     1177 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/hub_darwin.go
--rw-r--r--   0 runner     (501) staff       (20)     1179 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/hub_freebsd.go
--rw-r--r--   0 runner     (501) staff       (20)      931 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/hub_linux.go
--rw-r--r--   0 runner     (501) staff       (20)      410 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/hub_other.go
--rw-r--r--   0 runner     (501) staff       (20)      111 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/udp/udp.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.094301 Xray-core-1.8.8/xray-go/transport/internet/websocket/
--rw-r--r--   0 runner     (501) staff       (20)      601 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/config.go
--rw-r--r--   0 runner     (501) staff       (20)     9533 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/config.pb.go
--rw-r--r--   0 runner     (501) staff       (20)      565 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/config.proto
--rw-r--r--   0 runner     (501) staff       (20)     2439 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/connection.go
--rw-r--r--   0 runner     (501) staff       (20)     5887 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/dialer.go
--rw-r--r--   0 runner     (501) staff       (20)     1218 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/dialer.html
--rw-r--r--   0 runner     (501) staff       (20)      218 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/errors.generated.go
--rw-r--r--   0 runner     (501) staff       (20)     4360 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/hub.go
--rw-r--r--   0 runner     (501) staff       (20)      263 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/ws.go
--rw-r--r--   0 runner     (501) staff       (20)     3736 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/internet/websocket/ws_test.go
--rw-r--r--   0 runner     (501) staff       (20)      211 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/link.go
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-02-28 15:14:25.096990 Xray-core-1.8.8/xray-go/transport/pipe/
--rw-r--r--   0 runner     (501) staff       (20)     3519 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/pipe/impl.go
--rw-r--r--   0 runner     (501) staff       (20)     1493 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/pipe/pipe.go
--rw-r--r--   0 runner     (501) staff       (20)     3502 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/pipe/pipe_test.go
--rw-r--r--   0 runner     (501) staff       (20)      955 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/pipe/reader.go
--rw-r--r--   0 runner     (501) staff       (20)      601 2024-02-28 15:14:14.000000 Xray-core-1.8.8/xray-go/transport/pipe/writer.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.134794 Xray-core-1.8.9/
+-rw-r--r--   0 runner     (501) staff       (20)     1149 2024-03-11 05:03:11.000000 Xray-core-1.8.9/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)    16725 2024-03-11 05:03:11.000000 Xray-core-1.8.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      180 2024-03-11 05:03:11.000000 Xray-core-1.8.9/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     5544 2024-03-11 05:03:19.134466 Xray-core-1.8.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3756 2024-03-11 05:03:11.000000 Xray-core-1.8.9/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.696349 Xray-core-1.8.9/Xray_core.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     5544 2024-03-11 05:03:18.000000 Xray-core-1.8.9/Xray_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    36019 2024-03-11 05:03:18.000000 Xray-core-1.8.9/Xray_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-11 05:03:18.000000 Xray-core-1.8.9/Xray_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-03-11 05:03:18.000000 Xray-core-1.8.9/Xray_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)        5 2024-03-11 05:03:18.000000 Xray-core-1.8.9/Xray_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.696932 Xray-core-1.8.9/gobuild/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-03-11 05:03:11.000000 Xray-core-1.8.9/gobuild/.gitkeep
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.698257 Xray-core-1.8.9/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    11911 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1684 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)        7 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/VERSION
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.633412 Xray-core-1.8.9/pybind11/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.707984 Xray-core-1.8.9/pybind11/include/pybind11/
+-rw-r--r--   0 runner     (501) staff       (20)    23979 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner     (501) staff       (20)     7069 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner     (501) staff       (20)    65638 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner     (501) staff       (20)     8458 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner     (501) staff       (20)      120 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     2096 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.711350 Xray-core-1.8.9/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner     (501) staff       (20)    28251 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner     (501) staff       (20)    50369 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner     (501) staff       (20)     5491 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner     (501) staff       (20)    17981 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner     (501) staff       (20)    25057 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner     (501) staff       (20)    42266 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner     (501) staff       (20)     1625 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner     (501) staff       (20)    32147 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner     (501) staff       (20)    11792 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner     (501) staff       (20)     4731 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner     (501) staff       (20)     4695 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner     (501) staff       (20)     8262 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner     (501) staff       (20)     8862 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner     (501) staff       (20)    79524 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner     (501) staff       (20)     9103 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner     (501) staff       (20)     2181 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner     (501) staff       (20)   125761 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner     (501) staff       (20)    93848 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.711787 Xray-core-1.8.9/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner     (501) staff       (20)     4185 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner     (501) staff       (20)    15337 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner     (501) staff       (20)    27013 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.720486 Xray-core-1.8.9/pybind11/tools/
+-rw-r--r--   0 runner     (501) staff       (20)     2350 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     3105 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner     (501) staff       (20)    11103 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner     (501) staff       (20)      817 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     1423 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner     (501) staff       (20)      952 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     1040 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner     (501) staff       (20)     1031 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/libsize.py
+-rw-r--r--   0 runner     (501) staff       (20)     1282 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner     (501) staff       (20)      196 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner     (501) staff       (20)    13487 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     6930 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner     (501) staff       (20)     8955 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner     (501) staff       (20)     8359 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner     (501) staff       (20)       94 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1965 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2024-03-11 05:03:11.000000 Xray-core-1.8.9/pybind11/tools/setup_main.py.in
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-03-11 05:03:19.134874 Xray-core-1.8.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2810 2024-03-11 05:03:11.000000 Xray-core-1.8.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.722256 Xray-core-1.8.9/src/
+-rw-r--r--   0 runner     (501) staff       (20)     1403 2024-03-11 05:03:11.000000 Xray-core-1.8.9/src/xray.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.763085 Xray-core-1.8.9/xray/
+-rw-r--r--   0 runner     (501) staff       (20)       50 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.766474 Xray-core-1.8.9/xray-go/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.767044 Xray-core-1.8.9/xray-go/.github/
+-rw-r--r--   0 runner     (501) staff       (20)      560 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.767446 Xray-core-1.8.9/xray-go/.github/docker/
+-rw-r--r--   0 runner     (501) staff       (20)      907 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/.github/docker/Dockerfile
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.767863 Xray-core-1.8.9/xray-go/.github/docker/files/
+-rw-r--r--   0 runner     (501) staff       (20)      286 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/.github/docker/files/config.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.769408 Xray-core-1.8.9/xray-go/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1324 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/.github/workflows/docker.yml
+-rw-r--r--   0 runner     (501) staff       (20)     6816 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/.github/workflows/release.yml
+-rw-r--r--   0 runner     (501) staff       (20)      941 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/.github/workflows/test.yml
+-rw-r--r--   0 runner     (501) staff       (20)      420 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)     5226 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner     (501) staff       (20)    16725 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      799 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)     6963 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.769782 Xray-core-1.8.9/xray-go/app/
+-rw-r--r--   0 runner     (501) staff       (20)      113 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/app.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.771990 Xray-core-1.8.9/xray-go/app/commander/
+-rw-r--r--   0 runner     (501) staff       (20)     2327 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/commander/commander.go
+-rw-r--r--   0 runner     (501) staff       (20)     7721 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/commander/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      681 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/commander/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      218 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/commander/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     2176 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/commander/outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)      585 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/commander/service.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.776488 Xray-core-1.8.9/xray-go/app/dispatcher/
+-rw-r--r--   0 runner     (501) staff       (20)     6917 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      337 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)    12703 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/default.go
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/dispatcher.go
+-rw-r--r--   0 runner     (501) staff       (20)      219 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3802 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/fakednssniffer.go
+-rw-r--r--   0 runner     (501) staff       (20)     3837 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/sniffer.go
+-rw-r--r--   0 runner     (501) staff       (20)      514 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/stats.go
+-rw-r--r--   0 runner     (501) staff       (20)      818 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dispatcher/stats_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.785519 Xray-core-1.8.9/xray-go/app/dns/
+-rw-r--r--   0 runner     (501) staff       (20)     2112 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    29979 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     2116 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     9273 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/dns.go
+-rw-r--r--   0 runner     (501) staff       (20)    24669 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/dns_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     5826 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/dnscommon.go
+-rw-r--r--   0 runner     (501) staff       (20)     4468 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/dnscommon_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.788502 Xray-core-1.8.9/xray-go/app/dns/fakedns/
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/fakedns/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     6312 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/fakedns/fake.go
+-rw-r--r--   0 runner     (501) staff       (20)       87 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/fakedns/fakedns.go
+-rw-r--r--   0 runner     (501) staff       (20)     7885 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/fakedns/fakedns.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      497 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/fakedns/fakedns.proto
+-rw-r--r--   0 runner     (501) staff       (20)     5889 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/fakedns/fakedns_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3272 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/hosts.go
+-rw-r--r--   0 runner     (501) staff       (20)     2527 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/hosts_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     8513 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver.go
+-rw-r--r--   0 runner     (501) staff       (20)    10593 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_doh.go
+-rw-r--r--   0 runner     (501) staff       (20)     2705 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_doh_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1206 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_fakedns.go
+-rw-r--r--   0 runner     (501) staff       (20)     1512 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_local.go
+-rw-r--r--   0 runner     (501) staff       (20)      590 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_local_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    10376 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_quic.go
+-rw-r--r--   0 runner     (501) staff       (20)     2216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_quic_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     9104 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_tcp.go
+-rw-r--r--   0 runner     (501) staff       (20)     2767 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_tcp_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     7088 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/dns/nameserver_udp.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.790829 Xray-core-1.8.9/xray-go/app/log/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.793127 Xray-core-1.8.9/xray-go/app/log/command/
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/command/command.go
+-rw-r--r--   0 runner     (501) staff       (20)      919 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/command/command_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     8975 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/command/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      440 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/command/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     4016 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/command/config_grpc.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/command/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     9727 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      536 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     2921 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/log.go
+-rw-r--r--   0 runner     (501) staff       (20)     1527 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/log_creator.go
+-rw-r--r--   0 runner     (501) staff       (20)     1282 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/log/log_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.795184 Xray-core-1.8.9/xray-go/app/metrics/
+-rw-r--r--   0 runner     (501) staff       (20)     4934 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/metrics/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      383 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/metrics/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/metrics/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3132 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/metrics/metrics.go
+-rw-r--r--   0 runner     (501) staff       (20)     2190 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/metrics/outbound.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.797973 Xray-core-1.8.9/xray-go/app/observatory/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.801659 Xray-core-1.8.9/xray-go/app/observatory/burst/
+-rw-r--r--   0 runner     (501) staff       (20)      207 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/burst.go
+-rw-r--r--   0 runner     (501) staff       (20)     2779 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/burstobserver.go
+-rw-r--r--   0 runner     (501) staff       (20)    10520 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      931 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     6416 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/healthping.go
+-rw-r--r--   0 runner     (501) staff       (20)     3301 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/healthping_result.go
+-rw-r--r--   0 runner     (501) staff       (20)     2485 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/healthping_result_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1696 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/burst/ping.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.803391 Xray-core-1.8.9/xray-go/app/observatory/command/
+-rw-r--r--   0 runner     (501) staff       (20)     1141 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/command/command.go
+-rw-r--r--   0 runner     (501) staff       (20)    11323 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/command/command.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      618 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/command/command.proto
+-rw-r--r--   0 runner     (501) staff       (20)     4350 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/command/command_grpc.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)    22974 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     2011 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      220 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      565 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/explainErrors.go
+-rw-r--r--   0 runner     (501) staff       (20)       91 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/observatory.go
+-rw-r--r--   0 runner     (501) staff       (20)     6035 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/observatory/observer.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.806310 Xray-core-1.8.9/xray-go/app/policy/
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/policy/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    25190 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/policy/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1039 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/policy/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/policy/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1433 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/policy/manager.go
+-rw-r--r--   0 runner     (501) staff       (20)      995 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/policy/manager_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      152 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/policy/policy.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.807497 Xray-core-1.8.9/xray-go/app/proxyman/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.809928 Xray-core-1.8.9/xray-go/app/proxyman/command/
+-rw-r--r--   0 runner     (501) staff       (20)     4575 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/command/command.go
+-rw-r--r--   0 runner     (501) staff       (20)    39310 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/command/command.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1652 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/command/command.proto
+-rw-r--r--   0 runner     (501) staff       (20)    12112 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/command/command_grpc.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)       87 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/command/doc.go
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/command/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      758 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    43436 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     3087 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/config.proto
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.811600 Xray-core-1.8.9/xray-go/app/proxyman/inbound/
+-rw-r--r--   0 runner     (501) staff       (20)     5289 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/inbound/always.go
+-rw-r--r--   0 runner     (501) staff       (20)     5544 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/inbound/dynamic.go
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/inbound/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     4732 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/inbound/inbound.go
+-rw-r--r--   0 runner     (501) staff       (20)    12675 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/inbound/worker.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.813134 Xray-core-1.8.9/xray-go/app/proxyman/outbound/
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/outbound/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     9264 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/outbound/handler.go
+-rw-r--r--   0 runner     (501) staff       (20)     4262 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/outbound/handler_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3984 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/outbound/outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     1020 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/proxyman/outbound/uot.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.816681 Xray-core-1.8.9/xray-go/app/reverse/
+-rw-r--r--   0 runner     (501) staff       (20)     4440 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/bridge.go
+-rw-r--r--   0 runner     (501) staff       (20)      235 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    13860 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     5552 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/portal.go
+-rw-r--r--   0 runner     (501) staff       (20)      396 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/portal_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2049 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/reverse/reverse.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.822754 Xray-core-1.8.9/xray-go/app/router/
+-rw-r--r--   0 runner     (501) staff       (20)     2927 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/balancing.go
+-rw-r--r--   0 runner     (501) staff       (20)      882 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/balancing_override.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.826027 Xray-core-1.8.9/xray-go/app/router/command/
+-rw-r--r--   0 runner     (501) staff       (20)     3963 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/command/command.go
+-rw-r--r--   0 runner     (501) staff       (20)    39584 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/command/command.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     3169 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/command/command.proto
+-rw-r--r--   0 runner     (501) staff       (20)     9869 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/command/command_grpc.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)    12438 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/command/command_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3684 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/command/config.go
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/command/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     6367 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/condition.go
+-rw-r--r--   0 runner     (501) staff       (20)     2481 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/condition_geoip.go
+-rw-r--r--   0 runner     (501) staff       (20)     5852 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/condition_geoip_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    12335 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/condition_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4008 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    53331 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     4248 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3736 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/router.go
+-rw-r--r--   0 runner     (501) staff       (20)     6705 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/router_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     5719 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/strategy_leastload.go
+-rw-r--r--   0 runner     (501) staff       (20)     5152 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/strategy_leastload_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1522 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/strategy_leastping.go
+-rw-r--r--   0 runner     (501) staff       (20)      438 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/strategy_random.go
+-rw-r--r--   0 runner     (501) staff       (20)     2021 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/weight.go
+-rw-r--r--   0 runner     (501) staff       (20)     1207 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/router/weight_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.829785 Xray-core-1.8.9/xray-go/app/stats/
+-rw-r--r--   0 runner     (501) staff       (20)     4219 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/channel.go
+-rw-r--r--   0 runner     (501) staff       (20)     9714 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/channel_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.832947 Xray-core-1.8.9/xray-go/app/stats/command/
+-rw-r--r--   0 runner     (501) staff       (20)     3073 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/command/command.go
+-rw-r--r--   0 runner     (501) staff       (20)    24726 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/command/command.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1176 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/command/command.proto
+-rw-r--r--   0 runner     (501) staff       (20)     6923 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/command/command_grpc.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1875 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/command/command_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/command/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     7106 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      346 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      478 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/counter.go
+-rw-r--r--   0 runner     (501) staff       (20)      664 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/counter_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3878 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/stats.go
+-rw-r--r--   0 runner     (501) staff       (20)     2004 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/app/stats/stats_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.835170 Xray-core-1.8.9/xray-go/common/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.836349 Xray-core-1.8.9/xray-go/common/antireplay/
+-rw-r--r--   0 runner     (501) staff       (20)      105 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/antireplay/antireplay.go
+-rw-r--r--   0 runner     (501) staff       (20)      607 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/antireplay/bloomring.go
+-rw-r--r--   0 runner     (501) staff       (20)     1324 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/antireplay/replayfilter.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.837025 Xray-core-1.8.9/xray-go/common/bitmask/
+-rw-r--r--   0 runner     (501) staff       (20)      318 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/bitmask/byte.go
+-rw-r--r--   0 runner     (501) staff       (20)      703 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/bitmask/byte_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.846101 Xray-core-1.8.9/xray-go/common/buf/
+-rw-r--r--   0 runner     (501) staff       (20)      200 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/buf.go
+-rw-r--r--   0 runner     (501) staff       (20)     5954 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/buffer.go
+-rw-r--r--   0 runner     (501) staff       (20)     4488 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/buffer_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2973 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/copy.go
+-rw-r--r--   0 runner     (501) staff       (20)     1519 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/copy_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3089 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/io.go
+-rw-r--r--   0 runner     (501) staff       (20)     1008 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/io_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6788 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/multi_buffer.go
+-rw-r--r--   0 runner     (501) staff       (20)     3788 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/multi_buffer_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      760 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/override.go
+-rw-r--r--   0 runner     (501) staff       (20)     3819 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/reader.go
+-rw-r--r--   0 runner     (501) staff       (20)     2952 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/reader_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      844 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/readv_posix.go
+-rw-r--r--   0 runner     (501) staff       (20)     2638 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/readv_reader.go
+-rw-r--r--   0 runner     (501) staff       (20)      198 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/readv_reader_wasm.go
+-rw-r--r--   0 runner     (501) staff       (20)     1310 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/readv_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      561 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/readv_unix.go
+-rw-r--r--   0 runner     (501) staff       (20)      733 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/readv_windows.go
+-rw-r--r--   0 runner     (501) staff       (20)     5199 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/writer.go
+-rw-r--r--   0 runner     (501) staff       (20)     2349 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/buf/writer_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.846469 Xray-core-1.8.9/xray-go/common/bytespool/
+-rw-r--r--   0 runner     (501) staff       (20)     1500 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/bytespool/pool.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.847155 Xray-core-1.8.9/xray-go/common/cache/
+-rw-r--r--   0 runner     (501) staff       (20)     2301 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/cache/lru.go
+-rw-r--r--   0 runner     (501) staff       (20)     1394 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/cache/lru_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.847532 Xray-core-1.8.9/xray-go/common/cmdarg/
+-rw-r--r--   0 runner     (501) staff       (20)      298 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/cmdarg/cmdarg.go
+-rw-r--r--   0 runner     (501) staff       (20)     4437 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/common.go
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/common_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.851814 Xray-core-1.8.9/xray-go/common/crypto/
+-rw-r--r--   0 runner     (501) staff       (20)     1267 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/aes.go
+-rw-r--r--   0 runner     (501) staff       (20)     7900 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/auth.go
+-rw-r--r--   0 runner     (501) staff       (20)     3382 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/auth_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      990 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/benchmark_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      405 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/chacha20.go
+-rw-r--r--   0 runner     (501) staff       (20)     2345 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/chacha20_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3681 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/chunk.go
+-rw-r--r--   0 runner     (501) staff       (20)     1060 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/chunk_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      199 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/crypto.go
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.852976 Xray-core-1.8.9/xray-go/common/crypto/internal/
+-rw-r--r--   0 runner     (501) staff       (20)     1942 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/internal/chacha.go
+-rw-r--r--   0 runner     (501) staff       (20)     3156 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/internal/chacha_core.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1832 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/internal/chacha_core_gen.go
+-rw-r--r--   0 runner     (501) staff       (20)     1360 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/crypto/io.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.853647 Xray-core-1.8.9/xray-go/common/dice/
+-rw-r--r--   0 runner     (501) staff       (20)     1013 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/dice/dice.go
+-rw-r--r--   0 runner     (501) staff       (20)      738 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/dice/dice_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.854750 Xray-core-1.8.9/xray-go/common/drain/
+-rw-r--r--   0 runner     (501) staff       (20)      187 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/drain/drain.go
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/drain/drainer.go
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/drain/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.855665 Xray-core-1.8.9/xray-go/common/errors/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.855958 Xray-core-1.8.9/xray-go/common/errors/errorgen/
+-rw-r--r--   0 runner     (501) staff       (20)      704 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/errors/errorgen/main.go
+-rw-r--r--   0 runner     (501) staff       (20)     3723 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/errors/errors.go
+-rw-r--r--   0 runner     (501) staff       (20)     1237 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/errors/errors_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      735 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/errors/multi_error.go
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1669 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/interfaces.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.859285 Xray-core-1.8.9/xray-go/common/log/
+-rw-r--r--   0 runner     (501) staff       (20)     1369 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/access.go
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/dns.go
+-rw-r--r--   0 runner     (501) staff       (20)     1240 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/log.go
+-rw-r--r--   0 runner     (501) staff       (20)     4648 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/log.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      317 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/log.proto
+-rw-r--r--   0 runner     (501) staff       (20)      565 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/log_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3575 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/logger.go
+-rw-r--r--   0 runner     (501) staff       (20)      773 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/log/logger_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.862618 Xray-core-1.8.9/xray-go/common/mux/
+-rw-r--r--   0 runner     (501) staff       (20)     9235 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     2841 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/client_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     4073 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/frame.go
+-rw-r--r--   0 runner     (501) staff       (20)      552 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/frame_test.go
+-rw-r--r--   0 runner     (501) staff       (20)       83 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/mux.go
+-rw-r--r--   0 runner     (501) staff       (20)     4251 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/mux_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1326 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/reader.go
+-rw-r--r--   0 runner     (501) staff       (20)     8971 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     4120 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/session.go
+-rw-r--r--   0 runner     (501) staff       (20)      756 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/session_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2881 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/mux/writer.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.871287 Xray-core-1.8.9/xray-go/common/net/
+-rw-r--r--   0 runner     (501) staff       (20)     5118 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/address.go
+-rw-r--r--   0 runner     (501) staff       (20)     6075 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/address.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      475 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/address.proto
+-rw-r--r--   0 runner     (501) staff       (20)     4485 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/address_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.871785 Xray-core-1.8.9/xray-go/common/net/cnc/
+-rw-r--r--   0 runner     (501) staff       (20)     3276 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/cnc/connection.go
+-rw-r--r--   0 runner     (501) staff       (20)     3560 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/destination.go
+-rw-r--r--   0 runner     (501) staff       (20)     6765 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/destination.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      428 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/destination.proto
+-rw-r--r--   0 runner     (501) staff       (20)     2519 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/destination_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      229 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/net.go
+-rw-r--r--   0 runner     (501) staff       (20)      423 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/network.go
+-rw-r--r--   0 runner     (501) staff       (20)     7048 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/network.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      425 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/network.proto
+-rw-r--r--   0 runner     (501) staff       (20)     2328 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/port.go
+-rw-r--r--   0 runner     (501) staff       (20)     7084 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/port.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      513 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/port.proto
+-rw-r--r--   0 runner     (501) staff       (20)      287 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/port_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1235 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/net/system.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.872843 Xray-core-1.8.9/xray-go/common/ocsp/
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/ocsp/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3094 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/ocsp/ocsp.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.873498 Xray-core-1.8.9/xray-go/common/peer/
+-rw-r--r--   0 runner     (501) staff       (20)      434 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/peer/latency.go
+-rw-r--r--   0 runner     (501) staff       (20)       13 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/peer/peer.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.874945 Xray-core-1.8.9/xray-go/common/platform/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.876390 Xray-core-1.8.9/xray-go/common/platform/ctlcmd/
+-rw-r--r--   0 runner     (501) staff       (20)      133 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/ctlcmd/attr_other.go
+-rw-r--r--   0 runner     (501) staff       (20)      172 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/ctlcmd/attr_windows.go
+-rw-r--r--   0 runner     (501) staff       (20)     1188 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/ctlcmd/ctlcmd.go
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/ctlcmd/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.876819 Xray-core-1.8.9/xray-go/common/platform/filesystem/
+-rw-r--r--   0 runner     (501) staff       (20)      832 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/filesystem/file.go
+-rw-r--r--   0 runner     (501) staff       (20)      915 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/others.go
+-rw-r--r--   0 runner     (501) staff       (20)     2260 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/platform.go
+-rw-r--r--   0 runner     (501) staff       (20)     1175 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/platform_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      553 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/platform/windows.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.885705 Xray-core-1.8.9/xray-go/common/protocol/
+-rw-r--r--   0 runner     (501) staff       (20)      239 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/account.go
+-rw-r--r--   0 runner     (501) staff       (20)     5904 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/address.go
+-rw-r--r--   0 runner     (501) staff       (20)     6183 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/address_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.886285 Xray-core-1.8.9/xray-go/common/protocol/bittorrent/
+-rw-r--r--   0 runner     (501) staff       (20)     1908 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/bittorrent/bittorrent.go
+-rw-r--r--   0 runner     (501) staff       (20)      411 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/context.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.887554 Xray-core-1.8.9/xray-go/common/protocol/dns/
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/dns/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     2592 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/dns/io.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     2490 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/headers.go
+-rw-r--r--   0 runner     (501) staff       (20)     7925 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/headers.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      445 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/headers.proto
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.889588 Xray-core-1.8.9/xray-go/common/protocol/http/
+-rw-r--r--   0 runner     (501) staff       (20)     1865 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/http/headers.go
+-rw-r--r--   0 runner     (501) staff       (20)     2765 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/http/headers_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1591 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/http/sniff.go
+-rw-r--r--   0 runner     (501) staff       (20)     3034 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/http/sniff_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      907 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/id.go
+-rw-r--r--   0 runner     (501) staff       (20)      392 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/id_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      265 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/payload.go
+-rw-r--r--   0 runner     (501) staff       (20)      142 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/protocol.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.890715 Xray-core-1.8.9/xray-go/common/protocol/quic/
+-rw-r--r--   0 runner     (501) staff       (20)      324 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/quic/qtls_go118.go
+-rw-r--r--   0 runner     (501) staff       (20)     7888 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/quic/sniff.go
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/quic/sniff_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1439 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/server_picker.go
+-rw-r--r--   0 runner     (501) staff       (20)     2053 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/server_picker_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2163 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/server_spec.go
+-rw-r--r--   0 runner     (501) staff       (20)     7142 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/server_spec.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      459 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/server_spec.proto
+-rw-r--r--   0 runner     (501) staff       (20)     1969 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/server_spec_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      403 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/time.go
+-rw-r--r--   0 runner     (501) staff       (20)      459 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/time_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.891528 Xray-core-1.8.9/xray-go/common/protocol/tls/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.893505 Xray-core-1.8.9/xray-go/common/protocol/tls/cert/
+-rw-r--r--   0 runner     (501) staff       (20)        5 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/tls/cert/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)     4416 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/tls/cert/cert.go
+-rw-r--r--   0 runner     (501) staff       (20)     2093 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/tls/cert/cert_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/tls/cert/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      939 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/tls/cert/privateKey.go
+-rw-r--r--   0 runner     (501) staff       (20)     3199 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/tls/sniff.go
+-rw-r--r--   0 runner     (501) staff       (20)     7025 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/tls/sniff_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.894286 Xray-core-1.8.9/xray-go/common/protocol/udp/
+-rw-r--r--   0 runner     (501) staff       (20)      275 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/udp/packet.go
+-rw-r--r--   0 runner     (501) staff       (20)       12 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/udp/udp.go
+-rw-r--r--   0 runner     (501) staff       (20)      893 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/user.go
+-rw-r--r--   0 runner     (501) staff       (20)     6433 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/user.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      544 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/protocol/user.proto
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.895123 Xray-core-1.8.9/xray-go/common/reflect/
+-rw-r--r--   0 runner     (501) staff       (20)     3674 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/reflect/marshal.go
+-rw-r--r--   0 runner     (501) staff       (20)     3303 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/reflect/marshal_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.896558 Xray-core-1.8.9/xray-go/common/retry/
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/retry/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1463 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/retry/retry.go
+-rw-r--r--   0 runner     (501) staff       (20)     1894 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/retry/retry_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.899738 Xray-core-1.8.9/xray-go/common/serial/
+-rw-r--r--   0 runner     (501) staff       (20)      736 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/serial.go
+-rw-r--r--   0 runner     (501) staff       (20)     1676 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/serial_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      609 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/string.go
+-rw-r--r--   0 runner     (501) staff       (20)     1049 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/string_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1334 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/typed_message.go
+-rw-r--r--   0 runner     (501) staff       (20)     5786 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/typed_message.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      473 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/typed_message.proto
+-rw-r--r--   0 runner     (501) staff       (20)      424 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/serial/typed_message_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.900868 Xray-core-1.8.9/xray-go/common/session/
+-rw-r--r--   0 runner     (501) staff       (20)     4606 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/session/context.go
+-rw-r--r--   0 runner     (501) staff       (20)     3380 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/session/session.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.902073 Xray-core-1.8.9/xray-go/common/signal/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.902434 Xray-core-1.8.9/xray-go/common/signal/done/
+-rw-r--r--   0 runner     (501) staff       (20)      830 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/done/done.go
+-rw-r--r--   0 runner     (501) staff       (20)      640 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/notifier.go
+-rw-r--r--   0 runner     (501) staff       (20)      226 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/notifier_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.902984 Xray-core-1.8.9/xray-go/common/signal/pubsub/
+-rw-r--r--   0 runner     (501) staff       (20)     1816 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/pubsub/pubsub.go
+-rw-r--r--   0 runner     (501) staff       (20)      460 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/pubsub/pubsub_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.903266 Xray-core-1.8.9/xray-go/common/signal/semaphore/
+-rw-r--r--   0 runner     (501) staff       (20)      522 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/semaphore/semaphore.go
+-rw-r--r--   0 runner     (501) staff       (20)     1267 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/timer.go
+-rw-r--r--   0 runner     (501) staff       (20)     1422 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/signal/timer_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.905859 Xray-core-1.8.9/xray-go/common/singbridge/
+-rw-r--r--   0 runner     (501) staff       (20)     1249 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/destination.go
+-rw-r--r--   0 runner     (501) staff       (20)     1935 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)      173 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/error.go
+-rw-r--r--   0 runner     (501) staff       (20)     1520 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/handler.go
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/logger.go
+-rw-r--r--   0 runner     (501) staff       (20)     1937 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/packet.go
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/pipe.go
+-rw-r--r--   0 runner     (501) staff       (20)     1511 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/singbridge/reader.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.910579 Xray-core-1.8.9/xray-go/common/strmatcher/
+-rw-r--r--   0 runner     (501) staff       (20)     4156 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/ac_automaton_matcher.go
+-rw-r--r--   0 runner     (501) staff       (20)     1136 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/benchmark_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1804 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/domain_matcher.go
+-rw-r--r--   0 runner     (501) staff       (20)     1287 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/domain_matcher_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      494 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/full_matcher.go
+-rw-r--r--   0 runner     (501) staff       (20)      909 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/full_matcher_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      919 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/matchers.go
+-rw-r--r--   0 runner     (501) staff       (20)     1298 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/matchers_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     7077 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/mph_matcher.go
+-rw-r--r--   0 runner     (501) staff       (20)     2659 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/strmatcher.go
+-rw-r--r--   0 runner     (501) staff       (20)     4455 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/strmatcher/strmatcher_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.912706 Xray-core-1.8.9/xray-go/common/task/
+-rw-r--r--   0 runner     (501) staff       (20)      192 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/task/common.go
+-rw-r--r--   0 runner     (501) staff       (20)     1264 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/task/periodic.go
+-rw-r--r--   0 runner     (501) staff       (20)      668 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/task/periodic_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1082 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/task/task.go
+-rw-r--r--   0 runner     (501) staff       (20)     1346 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/task/task_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1080 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/type.go
+-rw-r--r--   0 runner     (501) staff       (20)      797 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/type_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.913602 Xray-core-1.8.9/xray-go/common/units/
+-rw-r--r--   0 runner     (501) staff       (20)     1874 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/units/bytesize.go
+-rw-r--r--   0 runner     (501) staff       (20)     1218 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/units/bytesize_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.914471 Xray-core-1.8.9/xray-go/common/uuid/
+-rw-r--r--   0 runner     (501) staff       (20)     2177 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/uuid/uuid.go
+-rw-r--r--   0 runner     (501) staff       (20)     1823 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/uuid/uuid_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.916818 Xray-core-1.8.9/xray-go/common/xudp/
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/xudp/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/xudp/xudp.go
+-rw-r--r--   0 runner     (501) staff       (20)      787 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/common/xudp/xudp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.924177 Xray-core-1.8.9/xray-go/core/
+-rw-r--r--   0 runner     (501) staff       (20)      675 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/annotations.go
+-rw-r--r--   0 runner     (501) staff       (20)     4402 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    17234 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     2402 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     1537 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/context.go
+-rw-r--r--   0 runner     (501) staff       (20)      280 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/context_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1335 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/core.go
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      182 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/format.go
+-rw-r--r--   0 runner     (501) staff       (20)     2758 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/functions.go
+-rw-r--r--   0 runner     (501) staff       (20)     4894 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/functions_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/mocks.go
+-rw-r--r--   0 runner     (501) staff       (20)      233 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/proto.go
+-rw-r--r--   0 runner     (501) staff       (20)     9066 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/xray.go
+-rw-r--r--   0 runner     (501) staff       (20)     2404 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/core/xray_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.924974 Xray-core-1.8.9/xray-go/features/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.925987 Xray-core-1.8.9/xray-go/features/dns/
+-rw-r--r--   0 runner     (501) staff       (20)     1260 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/dns/client.go
+-rw-r--r--   0 runner     (501) staff       (20)      472 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/dns/fakedns.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.926804 Xray-core-1.8.9/xray-go/features/dns/localdns/
+-rw-r--r--   0 runner     (501) staff       (20)     1418 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/dns/localdns/client.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/dns/localdns/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.927715 Xray-core-1.8.9/xray-go/features/extension/
+-rw-r--r--   0 runner     (501) staff       (20)      108 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/extension/contextreceiver.go
+-rw-r--r--   0 runner     (501) staff       (20)      295 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/extension/observatory.go
+-rw-r--r--   0 runner     (501) staff       (20)      707 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/feature.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.928134 Xray-core-1.8.9/xray-go/features/inbound/
+-rw-r--r--   0 runner     (501) staff       (20)     1078 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/inbound/inbound.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.928510 Xray-core-1.8.9/xray-go/features/outbound/
+-rw-r--r--   0 runner     (501) staff       (20)     1212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/outbound/outbound.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.929409 Xray-core-1.8.9/xray-go/features/policy/
+-rw-r--r--   0 runner     (501) staff       (20)      691 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/policy/default.go
+-rw-r--r--   0 runner     (501) staff       (20)     4058 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/policy/policy.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.931215 Xray-core-1.8.9/xray-go/features/routing/
+-rw-r--r--   0 runner     (501) staff       (20)      240 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/routing/balancer.go
+-rw-r--r--   0 runner     (501) staff       (20)     1285 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/routing/context.go
+-rw-r--r--   0 runner     (501) staff       (20)      844 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/routing/dispatcher.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.932365 Xray-core-1.8.9/xray-go/features/routing/dns/
+-rw-r--r--   0 runner     (501) staff       (20)     1293 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/routing/dns/context.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/routing/dns/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1469 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/routing/router.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.932761 Xray-core-1.8.9/xray-go/features/routing/session/
+-rw-r--r--   0 runner     (501) staff       (20)     3105 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/routing/session/context.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.933501 Xray-core-1.8.9/xray-go/features/stats/
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/stats/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     4445 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/features/stats/stats.go
+-rw-r--r--   0 runner     (501) staff       (20)     2533 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/go.mod
+-rw-r--r--   0 runner     (501) staff       (20)    30521 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/go.sum
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.649002 Xray-core-1.8.9/xray-go/infra/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.956565 Xray-core-1.8.9/xray-go/infra/conf/
+-rw-r--r--   0 runner     (501) staff       (20)     1501 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/api.go
+-rw-r--r--   0 runner     (501) staff       (20)     1156 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/blackhole.go
+-rw-r--r--   0 runner     (501) staff       (20)      610 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/blackhole_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      118 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/buildable.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.647958 Xray-core-1.8.9/xray-go/infra/conf/cfgcommon/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.957605 Xray-core-1.8.9/xray-go/infra/conf/cfgcommon/duration/
+-rw-r--r--   0 runner     (501) staff       (20)      557 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/cfgcommon/duration/duration.go
+-rw-r--r--   0 runner     (501) staff       (20)      654 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/cfgcommon/duration/duration_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     5580 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/common.go
+-rw-r--r--   0 runner     (501) staff       (20)     5094 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/common_test.go
+-rw-r--r--   0 runner     (501) staff       (20)       84 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/conf.go
+-rw-r--r--   0 runner     (501) staff       (20)    10224 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/dns.go
+-rw-r--r--   0 runner     (501) staff       (20)      853 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/dns_proxy.go
+-rw-r--r--   0 runner     (501) staff       (20)      638 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/dns_proxy_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3745 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/dns_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      754 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/dokodemo.go
+-rw-r--r--   0 runner     (501) staff       (20)      794 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/dokodemo_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3408 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/fakedns.go
+-rw-r--r--   0 runner     (501) staff       (20)     5592 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/freedom.go
+-rw-r--r--   0 runner     (501) staff       (20)      881 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/freedom_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      877 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/general_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/grpc.go
+-rw-r--r--   0 runner     (501) staff       (20)     2373 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/http.go
+-rw-r--r--   0 runner     (501) staff       (20)      686 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/http_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/init.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.958796 Xray-core-1.8.9/xray-go/infra/conf/json/
+-rw-r--r--   0 runner     (501) staff       (20)     2564 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/json/reader.go
+-rw-r--r--   0 runner     (501) staff       (20)     1927 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/json/reader_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      719 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/lint.go
+-rw-r--r--   0 runner     (501) staff       (20)     1893 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/loader.go
+-rw-r--r--   0 runner     (501) staff       (20)     1439 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/log.go
+-rw-r--r--   0 runner     (501) staff       (20)      292 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/loopback.go
+-rw-r--r--   0 runner     (501) staff       (20)      307 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/metrics.go
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/observatory.go
+-rw-r--r--   0 runner     (501) staff       (20)     2355 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/policy.go
+-rw-r--r--   0 runner     (501) staff       (20)      591 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/policy_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1118 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/reverse.go
+-rw-r--r--   0 runner     (501) staff       (20)      815 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/reverse_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    17937 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/router.go
+-rw-r--r--   0 runner     (501) staff       (20)     2659 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/router_strategy.go
+-rw-r--r--   0 runner     (501) staff       (20)     7374 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/router_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.960731 Xray-core-1.8.9/xray-go/infra/conf/serial/
+-rw-r--r--   0 runner     (501) staff       (20)     1938 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/serial/builder.go
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/serial/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3606 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/serial/loader.go
+-rw-r--r--   0 runner     (501) staff       (20)     1054 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/serial/loader_test.go
+-rw-r--r--   0 runner     (501) staff       (20)       86 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/serial/serial.go
+-rw-r--r--   0 runner     (501) staff       (20)     7303 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/shadowsocks.go
+-rw-r--r--   0 runner     (501) staff       (20)      831 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/shadowsocks_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3204 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/socks.go
+-rw-r--r--   0 runner     (501) staff       (20)     1827 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/socks_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     3523 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/transport.go
+-rw-r--r--   0 runner     (501) staff       (20)     5619 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/transport_authenticators.go
+-rw-r--r--   0 runner     (501) staff       (20)    28383 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/transport_internet.go
+-rw-r--r--   0 runner     (501) staff       (20)     7387 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/transport_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4746 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/trojan.go
+-rw-r--r--   0 runner     (501) staff       (20)     5676 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/vless.go
+-rw-r--r--   0 runner     (501) staff       (20)     2658 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/vless_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4340 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/vmess.go
+-rw-r--r--   0 runner     (501) staff       (20)     2345 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/vmess_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4056 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/wireguard.go
+-rw-r--r--   0 runner     (501) staff       (20)     1393 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/wireguard_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    21052 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/xray.go
+-rw-r--r--   0 runner     (501) staff       (20)    13294 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/conf/xray_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.961142 Xray-core-1.8.9/xray-go/infra/vformat/
+-rw-r--r--   0 runner     (501) staff       (20)     4711 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/vformat/main.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.961712 Xray-core-1.8.9/xray-go/infra/vprotogen/
+-rw-r--r--   0 runner     (501) staff       (20)     6562 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/infra/vprotogen/main.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.964309 Xray-core-1.8.9/xray-go/main/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.650223 Xray-core-1.8.9/xray-go/main/commands/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.967528 Xray-core-1.8.9/xray-go/main/commands/all/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.974233 Xray-core-1.8.9/xray-go/main/commands/all/api/
+-rw-r--r--   0 runner     (501) staff       (20)      523 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/api.go
+-rw-r--r--   0 runner     (501) staff       (20)     2467 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/balancer_info.go
+-rw-r--r--   0 runner     (501) staff       (20)     1760 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/balancer_override.go
+-rw-r--r--   0 runner     (501) staff       (20)     1778 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/inbounds_add.go
+-rw-r--r--   0 runner     (501) staff       (20)     1778 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/inbounds_remove.go
+-rw-r--r--   0 runner     (501) staff       (20)      885 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/logger_restart.go
+-rw-r--r--   0 runner     (501) staff       (20)     1797 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/outbounds_add.go
+-rw-r--r--   0 runner     (501) staff       (20)     1749 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/outbounds_remove.go
+-rw-r--r--   0 runner     (501) staff       (20)     3768 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/shared.go
+-rw-r--r--   0 runner     (501) staff       (20)     1179 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/stats_get.go
+-rw-r--r--   0 runner     (501) staff       (20)     1717 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/stats_query.go
+-rw-r--r--   0 runner     (501) staff       (20)      872 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/api/stats_sys.go
+-rw-r--r--   0 runner     (501) staff       (20)      410 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/commands.go
+-rw-r--r--   0 runner     (501) staff       (20)     2774 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/convert.go
+-rw-r--r--   0 runner     (501) staff       (20)     1232 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/curve25519.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.976514 Xray-core-1.8.9/xray-go/main/commands/all/tls/
+-rw-r--r--   0 runner     (501) staff       (20)     3729 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/tls/cert.go
+-rw-r--r--   0 runner     (501) staff       (20)      947 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/tls/certchainhash.go
+-rw-r--r--   0 runner     (501) staff       (20)     3093 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/tls/ping.go
+-rw-r--r--   0 runner     (501) staff       (20)      327 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/tls/tls.go
+-rw-r--r--   0 runner     (501) staff       (20)      772 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/uuid.go
+-rw-r--r--   0 runner     (501) staff       (20)      589 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/wg.go
+-rw-r--r--   0 runner     (501) staff       (20)      754 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/all/x25519.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.979413 Xray-core-1.8.9/xray-go/main/commands/base/
+-rw-r--r--   0 runner     (501) staff       (20)     3499 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/base/command.go
+-rw-r--r--   0 runner     (501) staff       (20)      481 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/base/env.go
+-rw-r--r--   0 runner     (501) staff       (20)     1940 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/base/execute.go
+-rw-r--r--   0 runner     (501) staff       (20)     4055 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/base/help.go
+-rw-r--r--   0 runner     (501) staff       (20)      349 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/commands/base/root.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.980303 Xray-core-1.8.9/xray-go/main/confloader/
+-rw-r--r--   0 runner     (501) staff       (20)      923 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/confloader/confloader.go
+-rw-r--r--   0 runner     (501) staff       (20)      219 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/confloader/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.981401 Xray-core-1.8.9/xray-go/main/confloader/external/
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/confloader/external/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1881 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/confloader/external/external.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.651261 Xray-core-1.8.9/xray-go/main/distro/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.981845 Xray-core-1.8.9/xray-go/main/distro/all/
+-rw-r--r--   0 runner     (501) staff       (20)     3366 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/distro/all/all.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.982318 Xray-core-1.8.9/xray-go/main/distro/debug/
+-rw-r--r--   0 runner     (501) staff       (20)      109 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/distro/debug/debug.go
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.983351 Xray-core-1.8.9/xray-go/main/json/
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/json/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1286 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/json/json.go
+-rw-r--r--   0 runner     (501) staff       (20)     1426 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/main.go
+-rw-r--r--   0 runner     (501) staff       (20)      139 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/main_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6648 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/run.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.984499 Xray-core-1.8.9/xray-go/main/toml/
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/toml/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1286 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/toml/toml.go
+-rw-r--r--   0 runner     (501) staff       (20)      505 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/version.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.985695 Xray-core-1.8.9/xray-go/main/yaml/
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/yaml/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1293 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/main/yaml/yaml.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.986645 Xray-core-1.8.9/xray-go/proxy/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.990003 Xray-core-1.8.9/xray-go/proxy/blackhole/
+-rw-r--r--   0 runner     (501) staff       (20)     1369 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/blackhole/blackhole.go
+-rw-r--r--   0 runner     (501) staff       (20)      896 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/blackhole/blackhole_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1111 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/blackhole/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     8717 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/blackhole/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      413 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/blackhole/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      543 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/blackhole/config_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      218 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/blackhole/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.992765 Xray-core-1.8.9/xray-go/proxy/dns/
+-rw-r--r--   0 runner     (501) staff       (20)     6221 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dns/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      476 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dns/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     8342 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dns/dns.go
+-rw-r--r--   0 runner     (501) staff       (20)     9341 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dns/dns_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dns/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.995694 Xray-core-1.8.9/xray-go/proxy/dokodemo/
+-rw-r--r--   0 runner     (501) staff       (20)      305 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dokodemo/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     9235 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dokodemo/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      741 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dokodemo/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     8027 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dokodemo/dokodemo.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dokodemo/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1801 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dokodemo/fakeudp_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/dokodemo/fakeudp_other.go
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.998345 Xray-core-1.8.9/xray-go/proxy/freedom/
+-rw-r--r--   0 runner     (501) staff       (20)     1337 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/freedom/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    18291 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/freedom/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1001 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/freedom/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/freedom/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)    11789 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/freedom/freedom.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.002409 Xray-core-1.8.9/xray-go/proxy/http/
+-rw-r--r--   0 runner     (501) staff       (20)     9415 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/http/client.go
+-rw-r--r--   0 runner     (501) staff       (20)      512 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/http/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    14511 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/http/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      816 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/http/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/http/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)       84 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/http/http.go
+-rw-r--r--   0 runner     (501) staff       (20)     9569 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/http/server.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.004847 Xray-core-1.8.9/xray-go/proxy/loopback/
+-rw-r--r--   0 runner     (501) staff       (20)       88 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/loopback/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     5150 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/loopback/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      292 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/loopback/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/loopback/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3211 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/loopback/loopback.go
+-rw-r--r--   0 runner     (501) staff       (20)    17623 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/proxy.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.010506 Xray-core-1.8.9/xray-go/proxy/shadowsocks/
+-rw-r--r--   0 runner     (501) staff       (20)     5799 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     6146 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    14546 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      815 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      897 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/config_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      220 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     9468 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/protocol.go
+-rw-r--r--   0 runner     (501) staff       (20)     5516 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/protocol_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     7831 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/server.go
+-rw-r--r--   0 runner     (501) staff       (20)      293 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/shadowsocks.go
+-rw-r--r--   0 runner     (501) staff       (20)     2996 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks/validator.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.015293 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/
+-rw-r--r--   0 runner     (501) staff       (20)      627 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    24779 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1222 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      225 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     4911 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/inbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     7146 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/inbound_multi.go
+-rw-r--r--   0 runner     (501) staff       (20)     5661 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/inbound_relay.go
+-rw-r--r--   0 runner     (501) staff       (20)     4641 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)       96 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/shadowsocks_2022.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.019516 Xray-core-1.8.9/xray-go/proxy/socks/
+-rw-r--r--   0 runner     (501) staff       (20)     6315 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/client.go
+-rw-r--r--   0 runner     (501) staff       (20)      526 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    17186 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1179 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)    13429 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/protocol.go
+-rw-r--r--   0 runner     (501) staff       (20)     2944 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/protocol_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     8040 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/server.go
+-rw-r--r--   0 runner     (501) staff       (20)      153 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/socks/socks.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.023989 Xray-core-1.8.9/xray-go/proxy/trojan/
+-rw-r--r--   0 runner     (501) staff       (20)     5044 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     1039 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    13473 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      694 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      215 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     5726 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/protocol.go
+-rw-r--r--   0 runner     (501) staff       (20)     2352 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/protocol_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    15608 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/server.go
+-rw-r--r--   0 runner     (501) staff       (20)       86 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/trojan.go
+-rw-r--r--   0 runner     (501) staff       (20)     1230 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/trojan/validator.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.026815 Xray-core-1.8.9/xray-go/proxy/vless/
+-rw-r--r--   0 runner     (501) staff       (20)     1043 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/account.go
+-rw-r--r--   0 runner     (501) staff       (20)     5752 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/account.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      544 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/account.proto
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.029222 Xray-core-1.8.9/xray-go/proxy/vless/encoding/
+-rw-r--r--   0 runner     (501) staff       (20)     4835 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/encoding/addons.go
+-rw-r--r--   0 runner     (501) staff       (20)     5668 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/encoding/addons.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      327 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/encoding/addons.proto
+-rw-r--r--   0 runner     (501) staff       (20)     7892 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/encoding/encoding.go
+-rw-r--r--   0 runner     (501) staff       (20)     3286 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/encoding/encoding_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/encoding/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.031339 Xray-core-1.8.9/xray-go/proxy/vless/inbound/
+-rw-r--r--   0 runner     (501) staff       (20)       16 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/inbound/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    10235 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/inbound/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      663 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/inbound/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/inbound/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)    18633 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/inbound/inbound.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.033511 Xray-core-1.8.9/xray-go/proxy/vless/outbound/
+-rw-r--r--   0 runner     (501) staff       (20)       17 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/outbound/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     6130 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/outbound/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      393 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/outbound/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/outbound/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)    10135 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/outbound/outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     1249 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/validator.go
+-rw-r--r--   0 runner     (501) staff       (20)      441 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vless/vless.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.036580 Xray-core-1.8.9/xray-go/proxy/vmess/
+-rw-r--r--   0 runner     (501) staff       (20)     1397 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/account.go
+-rw-r--r--   0 runner     (501) staff       (20)     6722 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/account.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      596 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/account.proto
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.039187 Xray-core-1.8.9/xray-go/proxy/vmess/aead/
+-rw-r--r--   0 runner     (501) staff       (20)     2740 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/aead/authid.go
+-rw-r--r--   0 runner     (501) staff       (20)     3322 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/aead/authid_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      748 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/aead/consts.go
+-rw-r--r--   0 runner     (501) staff       (20)     5214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/aead/encrypt.go
+-rw-r--r--   0 runner     (501) staff       (20)     2529 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/aead/encrypt_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      521 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/aead/kdf.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.042114 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/
+-rw-r--r--   0 runner     (501) staff       (20)     2174 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/auth.go
+-rw-r--r--   0 runner     (501) staff       (20)    13755 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/client.go
+-rw-r--r--   0 runner     (501) staff       (20)     3664 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/commands.go
+-rw-r--r--   0 runner     (501) staff       (20)     1200 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/commands_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      547 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/encoding.go
+-rw-r--r--   0 runner     (501) staff       (20)     3787 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/encoding_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)    16319 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/encoding/server.go
+-rw-r--r--   0 runner     (501) staff       (20)      214 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.044068 Xray-core-1.8.9/xray-go/proxy/vmess/inbound/
+-rw-r--r--   0 runner     (501) staff       (20)      208 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/inbound/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    10805 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/inbound/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      546 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/inbound/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/inbound/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     9906 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/inbound/inbound.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.046017 Xray-core-1.8.9/xray-go/proxy/vmess/outbound/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/outbound/command.go
+-rw-r--r--   0 runner     (501) staff       (20)       17 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/outbound/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     6185 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/outbound/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      396 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/outbound/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/outbound/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     7808 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/outbound/outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     2341 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/validator.go
+-rw-r--r--   0 runner     (501) staff       (20)      624 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/validator_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      404 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/vmess/vmess.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.049774 Xray-core-1.8.9/xray-go/proxy/wireguard/
+-rw-r--r--   0 runner     (501) staff       (20)     4823 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/bind.go
+-rw-r--r--   0 runner     (501) staff       (20)     9221 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/client.go
+-rw-r--r--   0 runner     (501) staff       (20)      868 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    15221 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      218 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/errors.generated.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.050244 Xray-core-1.8.9/xray-go/proxy/wireguard/gvisortun/
+-rw-r--r--   0 runner     (501) staff       (20)     5829 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/gvisortun/tun.go
+-rw-r--r--   0 runner     (501) staff       (20)     4715 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/server.go
+-rw-r--r--   0 runner     (501) staff       (20)     4945 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/tun.go
+-rw-r--r--   0 runner     (501) staff       (20)      294 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/tun_default.go
+-rw-r--r--   0 runner     (501) staff       (20)     5828 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/tun_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)     2720 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/proxy/wireguard/wireguard.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.656626 Xray-core-1.8.9/xray-go/testing/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.051005 Xray-core-1.8.9/xray-go/testing/coverage/
+-rw-r--r--   0 runner     (501) staff       (20)     1347 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/coverage/coverall
+-rw-r--r--   0 runner     (501) staff       (20)     1139 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/coverage/coverall2
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.053220 Xray-core-1.8.9/xray-go/testing/mocks/
+-rw-r--r--   0 runner     (501) staff       (20)     2616 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/mocks/dns.go
+-rw-r--r--   0 runner     (501) staff       (20)     2234 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/mocks/io.go
+-rw-r--r--   0 runner     (501) staff       (20)     1294 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/mocks/log.go
+-rw-r--r--   0 runner     (501) staff       (20)     1597 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/mocks/mux.go
+-rw-r--r--   0 runner     (501) staff       (20)     5670 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/mocks/outbound.go
+-rw-r--r--   0 runner     (501) staff       (20)     3379 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/mocks/proxy.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.060471 Xray-core-1.8.9/xray-go/testing/scenarios/
+-rw-r--r--   0 runner     (501) staff       (20)    13302 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/command_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     5824 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/common.go
+-rw-r--r--   0 runner     (501) staff       (20)      905 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/common_coverage.go
+-rw-r--r--   0 runner     (501) staff       (20)      670 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/common_regular.go
+-rw-r--r--   0 runner     (501) staff       (20)     2552 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/dns_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6351 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/dokodemo_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    19392 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/feature_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     9222 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/http_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2802 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/metrics_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6746 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/policy_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    10001 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/reverse_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6111 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/shadowsocks_2022_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    12812 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/shadowsocks_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    11796 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/socks_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    35148 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/tls_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    10641 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/transport_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    14588 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/vless_test.go
+-rw-r--r--   0 runner     (501) staff       (20)    39891 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/scenarios/vmess_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.657072 Xray-core-1.8.9/xray-go/testing/servers/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.060888 Xray-core-1.8.9/xray-go/testing/servers/http/
+-rw-r--r--   0 runner     (501) staff       (20)      806 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/servers/http/http.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.061718 Xray-core-1.8.9/xray-go/testing/servers/tcp/
+-rw-r--r--   0 runner     (501) staff       (20)      416 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/servers/tcp/port.go
+-rw-r--r--   0 runner     (501) staff       (20)     2437 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/servers/tcp/tcp.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.062240 Xray-core-1.8.9/xray-go/testing/servers/udp/
+-rw-r--r--   0 runner     (501) staff       (20)      456 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/servers/udp/port.go
+-rw-r--r--   0 runner     (501) staff       (20)     1293 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/testing/servers/udp/udp.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.062641 Xray-core-1.8.9/xray-go/transport/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.063513 Xray-core-1.8.9/xray-go/transport/global/
+-rw-r--r--   0 runner     (501) staff       (20)      239 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/global/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     6340 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/global/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      552 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/global/config.proto
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.071770 Xray-core-1.8.9/xray-go/transport/internet/
+-rw-r--r--   0 runner     (501) staff       (20)     4250 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    34916 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     2637 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     5348 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)      643 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/dialer_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.074502 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/
+-rw-r--r--   0 runner     (501) staff       (20)      749 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     7156 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      814 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/dial.go
+-rw-r--r--   0 runner     (501) staff       (20)       92 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/errgen.go
+-rw-r--r--   0 runner     (501) staff       (20)      221 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3289 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/listener.go
+-rw-r--r--   0 runner     (501) staff       (20)     2143 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/domainsocket/listener_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/filelocker.go
+-rw-r--r--   0 runner     (501) staff       (20)      813 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/filelocker_other.go
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/filelocker_windows.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.077002 Xray-core-1.8.9/xray-go/transport/internet/grpc/
+-rw-r--r--   0 runner     (501) staff       (20)     1763 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     8700 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      387 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     2685 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/config_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     6263 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/dial.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.079779 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/
+-rw-r--r--   0 runner     (501) staff       (20)     1912 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/customSeviceName.go
+-rw-r--r--   0 runner     (501) staff       (20)       88 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/encoding.go
+-rw-r--r--   0 runner     (501) staff       (20)      217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     2890 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/hunkconn.go
+-rw-r--r--   0 runner     (501) staff       (20)     2776 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/multiconn.go
+-rw-r--r--   0 runner     (501) staff       (20)     9247 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/stream.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      370 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/stream.proto
+-rw-r--r--   0 runner     (501) staff       (20)     6127 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/stream_grpc.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)       84 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/grpc.go
+-rw-r--r--   0 runner     (501) staff       (20)     4110 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/grpc/hub.go
+-rw-r--r--   0 runner     (501) staff       (20)      847 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/header.go
+-rw-r--r--   0 runner     (501) staff       (20)     1054 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/header_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:18.660134 Xray-core-1.8.9/xray-go/transport/internet/headers/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.081114 Xray-core-1.8.9/xray-go/transport/internet/headers/dns/
+-rw-r--r--   0 runner     (501) staff       (20)     6023 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/dns/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      354 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/dns/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     2812 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/dns/dns.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.084114 Xray-core-1.8.9/xray-go/transport/internet/headers/http/
+-rw-r--r--   0 runner     (501) staff       (20)     1910 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    23417 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1514 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     7328 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/http.go
+-rw-r--r--   0 runner     (501) staff       (20)     6589 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/http_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      203 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/linkedreadRequest.go
+-rw-r--r--   0 runner     (501) staff       (20)      717 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/http/resp.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.085552 Xray-core-1.8.9/xray-go/transport/internet/headers/noop/
+-rw-r--r--   0 runner     (501) staff       (20)     7365 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/noop/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      362 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/noop/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      813 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/noop/noop.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.086775 Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/
+-rw-r--r--   0 runner     (501) staff       (20)     7967 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      470 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      684 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/srtp.go
+-rw-r--r--   0 runner     (501) staff       (20)      637 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/srtp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.087912 Xray-core-1.8.9/xray-go/transport/internet/headers/tls/
+-rw-r--r--   0 runner     (501) staff       (20)     5808 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/tls/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      335 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/tls/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     1086 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/tls/dtls.go
+-rw-r--r--   0 runner     (501) staff       (20)      622 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/tls/dtls_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.089274 Xray-core-1.8.9/xray-go/transport/internet/headers/utp/
+-rw-r--r--   0 runner     (501) staff       (20)     6040 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/utp/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      352 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/utp/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      712 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/utp/utp.go
+-rw-r--r--   0 runner     (501) staff       (20)      579 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/utp/utp_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.090814 Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/
+-rw-r--r--   0 runner     (501) staff       (20)     5975 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      346 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      794 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/wechat.go
+-rw-r--r--   0 runner     (501) staff       (20)      541 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/wechat_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.092008 Xray-core-1.8.9/xray-go/transport/internet/headers/wireguard/
+-rw-r--r--   0 runner     (501) staff       (20)     6227 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/wireguard/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      362 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/wireguard/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      554 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/headers/wireguard/wireguard.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.095204 Xray-core-1.8.9/xray-go/transport/internet/http/
+-rw-r--r--   0 runner     (501) staff       (20)      836 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     8400 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      553 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     6845 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)       84 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/http.go
+-rw-r--r--   0 runner     (501) staff       (20)     2140 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/http_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     5417 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/http/hub.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.098317 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/
+-rw-r--r--   0 runner     (501) staff       (20)      175 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     6928 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      417 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     2591 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)      220 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)      392 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/httpupgrade.go
+-rw-r--r--   0 runner     (501) staff       (20)     4034 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/httpupgrade/hub.go
+-rw-r--r--   0 runner     (501) staff       (20)       88 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/internet.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.107143 Xray-core-1.8.9/xray-go/transport/internet/kcp/
+-rw-r--r--   0 runner     (501) staff       (20)     2517 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    26474 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     1223 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)    14828 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/connection.go
+-rw-r--r--   0 runner     (501) staff       (20)      789 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/connection_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     1738 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/crypt.go
+-rw-r--r--   0 runner     (501) staff       (20)      803 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/crypt_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      345 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/cryptreal.go
+-rw-r--r--   0 runner     (501) staff       (20)     2452 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1853 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/io.go
+-rw-r--r--   0 runner     (501) staff       (20)      653 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/io_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      254 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/kcp.go
+-rw-r--r--   0 runner     (501) staff       (20)     2078 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/kcp_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     4441 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/listener.go
+-rw-r--r--   0 runner     (501) staff       (20)      934 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/output.go
+-rw-r--r--   0 runner     (501) staff       (20)     4941 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/receiving.go
+-rw-r--r--   0 runner     (501) staff       (20)     6019 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/segment.go
+-rw-r--r--   0 runner     (501) staff       (20)     2146 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/segment_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     7405 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/sending.go
+-rw-r--r--   0 runner     (501) staff       (20)      358 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/xor.go
+-rw-r--r--   0 runner     (501) staff       (20)       86 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/xor_amd64.go
+-rw-r--r--   0 runner     (501) staff       (20)      752 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/kcp/xor_amd64.s
+-rw-r--r--   0 runner     (501) staff       (20)      978 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/memory_settings.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.111570 Xray-core-1.8.9/xray-go/transport/internet/quic/
+-rw-r--r--   0 runner     (501) staff       (20)     1024 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     7620 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      503 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     3919 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/conn.go
+-rw-r--r--   0 runner     (501) staff       (20)     5717 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3605 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/hub.go
+-rw-r--r--   0 runner     (501) staff       (20)      250 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/pool.go
+-rw-r--r--   0 runner     (501) staff       (20)      483 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/qlogWriter.go
+-rw-r--r--   0 runner     (501) staff       (20)      583 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/quic.go
+-rw-r--r--   0 runner     (501) staff       (20)     4919 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/quic/quic_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.114339 Xray-core-1.8.9/xray-go/transport/internet/reality/
+-rw-r--r--   0 runner     (501) staff       (20)     1473 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/reality/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    11995 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/reality/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      755 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/reality/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      216 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/reality/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     8620 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/reality/reality.go
+-rw-r--r--   0 runner     (501) staff       (20)      419 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt.go
+-rw-r--r--   0 runner     (501) staff       (20)     7670 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt_darwin.go
+-rw-r--r--   0 runner     (501) staff       (20)     7894 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt_freebsd.go
+-rw-r--r--   0 runner     (501) staff       (20)     7128 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      967 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt_linux_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      504 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt_other.go
+-rw-r--r--   0 runner     (501) staff       (20)      866 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     2811 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/sockopt_windows.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.114786 Xray-core-1.8.9/xray-go/transport/internet/stat/
+-rw-r--r--   0 runner     (501) staff       (20)      592 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/stat/connection.go
+-rw-r--r--   0 runner     (501) staff       (20)     5984 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/system_dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)     4506 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/system_listener.go
+-rw-r--r--   0 runner     (501) staff       (20)      701 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/system_listener_test.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.115309 Xray-core-1.8.9/xray-go/transport/internet/tagged/
+-rw-r--r--   0 runner     (501) staff       (20)      193 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tagged/tagged.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.116789 Xray-core-1.8.9/xray-go/transport/internet/tagged/taggedimpl/
+-rw-r--r--   0 runner     (501) staff       (20)      219 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tagged/taggedimpl/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     1352 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tagged/taggedimpl/impl.go
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tagged/taggedimpl/taggedimpl.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.120691 Xray-core-1.8.9/xray-go/transport/internet/tcp/
+-rw-r--r--   0 runner     (501) staff       (20)      266 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     7028 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      446 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     1932 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     4073 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/hub.go
+-rw-r--r--   0 runner     (501) staff       (20)      688 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_darwin.go
+-rw-r--r--   0 runner     (501) staff       (20)      690 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_freebsd.go
+-rw-r--r--   0 runner     (501) staff       (20)     1352 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      777 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_linux_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      304 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_other.go
+-rw-r--r--   0 runner     (501) staff       (20)       83 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp/tcp.go
+-rw-r--r--   0 runner     (501) staff       (20)     2907 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tcp_hub.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.124876 Xray-core-1.8.9/xray-go/transport/internet/tls/
+-rw-r--r--   0 runner     (501) staff       (20)    11614 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/config.go
+-rw-r--r--   0 runner     (501) staff       (20)    21489 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)     2272 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      902 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/config_other.go
+-rw-r--r--   0 runner     (501) staff       (20)     2530 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/config_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      209 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/config_windows.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     3042 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/grpc.go
+-rw-r--r--   0 runner     (501) staff       (20)      946 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/pin.go
+-rw-r--r--   0 runner     (501) staff       (20)    11080 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/pin_test.go
+-rw-r--r--   0 runner     (501) staff       (20)     7230 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/tls.go
+-rw-r--r--   0 runner     (501) staff       (20)      121 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/tls/unsafe.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.129073 Xray-core-1.8.9/xray-go/transport/internet/udp/
+-rw-r--r--   0 runner     (501) staff       (20)      238 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     5217 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      297 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)      706 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)     5014 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/dispatcher.go
+-rw-r--r--   0 runner     (501) staff       (20)     2176 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/dispatcher_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      212 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     2783 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/hub.go
+-rw-r--r--   0 runner     (501) staff       (20)     1177 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/hub_darwin.go
+-rw-r--r--   0 runner     (501) staff       (20)     1179 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/hub_freebsd.go
+-rw-r--r--   0 runner     (501) staff       (20)      931 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/hub_linux.go
+-rw-r--r--   0 runner     (501) staff       (20)      410 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/hub_other.go
+-rw-r--r--   0 runner     (501) staff       (20)      111 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/udp/udp.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.132347 Xray-core-1.8.9/xray-go/transport/internet/websocket/
+-rw-r--r--   0 runner     (501) staff       (20)      601 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/config.go
+-rw-r--r--   0 runner     (501) staff       (20)     9533 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/config.pb.go
+-rw-r--r--   0 runner     (501) staff       (20)      565 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/config.proto
+-rw-r--r--   0 runner     (501) staff       (20)     2439 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/connection.go
+-rw-r--r--   0 runner     (501) staff       (20)     5887 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/dialer.go
+-rw-r--r--   0 runner     (501) staff       (20)     1218 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/dialer.html
+-rw-r--r--   0 runner     (501) staff       (20)      218 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/errors.generated.go
+-rw-r--r--   0 runner     (501) staff       (20)     4360 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/hub.go
+-rw-r--r--   0 runner     (501) staff       (20)      263 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/ws.go
+-rw-r--r--   0 runner     (501) staff       (20)     3736 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/internet/websocket/ws_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      211 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/link.go
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-03-11 05:03:19.134006 Xray-core-1.8.9/xray-go/transport/pipe/
+-rw-r--r--   0 runner     (501) staff       (20)     3519 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/pipe/impl.go
+-rw-r--r--   0 runner     (501) staff       (20)     1493 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/pipe/pipe.go
+-rw-r--r--   0 runner     (501) staff       (20)     3502 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/pipe/pipe_test.go
+-rw-r--r--   0 runner     (501) staff       (20)      955 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/pipe/reader.go
+-rw-r--r--   0 runner     (501) staff       (20)      601 2024-03-11 05:03:11.000000 Xray-core-1.8.9/xray-go/transport/pipe/writer.go
```

### Comparing `Xray-core-1.8.8/CMakeLists.txt` & `Xray-core-1.8.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/LICENSE` & `Xray-core-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/PKG-INFO` & `Xray-core-1.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xray-core
-Version: 1.8.8
+Version: 1.8.9
 Summary: Python bindings for Xray-core, the best v2ray-core with XTLS support.
 Home-page: https://github.com/LorenEteval/Xray-core-python
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: MPL 2.0
 Description: # Xray-core-python
```

### Comparing `Xray-core-1.8.8/README.md` & `Xray-core-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/Xray_core.egg-info/PKG-INFO` & `Xray-core-1.8.9/Xray_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xray-core
-Version: 1.8.8
+Version: 1.8.9
 Summary: Python bindings for Xray-core, the best v2ray-core with XTLS support.
 Home-page: https://github.com/LorenEteval/Xray-core-python
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: MPL 2.0
 Description: # Xray-core-python
```

### Comparing `Xray-core-1.8.8/Xray_core.egg-info/SOURCES.txt` & `Xray-core-1.8.9/Xray_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -839,14 +839,21 @@
 xray-go/transport/internet/http/config.pb.go
 xray-go/transport/internet/http/config.proto
 xray-go/transport/internet/http/dialer.go
 xray-go/transport/internet/http/errors.generated.go
 xray-go/transport/internet/http/http.go
 xray-go/transport/internet/http/http_test.go
 xray-go/transport/internet/http/hub.go
+xray-go/transport/internet/httpupgrade/config.go
+xray-go/transport/internet/httpupgrade/config.pb.go
+xray-go/transport/internet/httpupgrade/config.proto
+xray-go/transport/internet/httpupgrade/dialer.go
+xray-go/transport/internet/httpupgrade/errors.generated.go
+xray-go/transport/internet/httpupgrade/httpupgrade.go
+xray-go/transport/internet/httpupgrade/hub.go
 xray-go/transport/internet/kcp/config.go
 xray-go/transport/internet/kcp/config.pb.go
 xray-go/transport/internet/kcp/config.proto
 xray-go/transport/internet/kcp/connection.go
 xray-go/transport/internet/kcp/connection_test.go
 xray-go/transport/internet/kcp/crypt.go
 xray-go/transport/internet/kcp/crypt_test.go
```

### Comparing `Xray-core-1.8.8/pybind11/CMakeLists.txt` & `Xray-core-1.8.9/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/LICENSE` & `Xray-core-1.8.9/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/attr.h` & `Xray-core-1.8.9/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/buffer_info.h` & `Xray-core-1.8.9/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/cast.h` & `Xray-core-1.8.9/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/chrono.h` & `Xray-core-1.8.9/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/complex.h` & `Xray-core-1.8.9/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/detail/class.h` & `Xray-core-1.8.9/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/detail/common.h` & `Xray-core-1.8.9/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/detail/descr.h` & `Xray-core-1.8.9/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/detail/init.h` & `Xray-core-1.8.9/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/detail/internals.h` & `Xray-core-1.8.9/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/detail/type_caster_base.h` & `Xray-core-1.8.9/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/detail/typeid.h` & `Xray-core-1.8.9/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/eigen.h` & `Xray-core-1.8.9/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/embed.h` & `Xray-core-1.8.9/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/eval.h` & `Xray-core-1.8.9/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/functional.h` & `Xray-core-1.8.9/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/gil.h` & `Xray-core-1.8.9/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/iostream.h` & `Xray-core-1.8.9/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/numpy.h` & `Xray-core-1.8.9/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/operators.h` & `Xray-core-1.8.9/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/options.h` & `Xray-core-1.8.9/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/pybind11.h` & `Xray-core-1.8.9/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/pytypes.h` & `Xray-core-1.8.9/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/stl/filesystem.h` & `Xray-core-1.8.9/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/stl.h` & `Xray-core-1.8.9/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/include/pybind11/stl_bind.h` & `Xray-core-1.8.9/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/FindCatch.cmake` & `Xray-core-1.8.9/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/FindEigen3.cmake` & `Xray-core-1.8.9/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/FindPythonLibsNew.cmake` & `Xray-core-1.8.9/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/JoinPaths.cmake` & `Xray-core-1.8.9/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/check-style.sh` & `Xray-core-1.8.9/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/cmake_uninstall.cmake.in` & `Xray-core-1.8.9/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/codespell_ignore_lines_from_errors.py` & `Xray-core-1.8.9/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/libsize.py` & `Xray-core-1.8.9/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/make_changelog.py` & `Xray-core-1.8.9/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/pybind11Common.cmake` & `Xray-core-1.8.9/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/pybind11Config.cmake.in` & `Xray-core-1.8.9/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/pybind11NewTools.cmake` & `Xray-core-1.8.9/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/pybind11Tools.cmake` & `Xray-core-1.8.9/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/setup_global.py.in` & `Xray-core-1.8.9/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/pybind11/tools/setup_main.py.in` & `Xray-core-1.8.9/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/setup.py` & `Xray-core-1.8.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ROOT_DIR = pathlib.Path().resolve()
 PACKAGE_NAME = 'Xray-core'
 BINDING_NAME = 'xray'
 CMAKE_BUILD_CACHE = 'CMakeBuildCache'
 
 
 def getXrayCoreVersion():
-    return '1.8.8'
+    return '1.8.9'
 
 
 def runCommand(command):
     subprocess.run(command, check=True)
 
 
 def buildXrayCore():
```

### Comparing `Xray-core-1.8.8/src/xray.cpp` & `Xray-core-1.8.9/src/xray.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,10 @@
             py::arg("apiServer"), py::arg("timeout"), py::arg("myPattern"), py::arg("reset"));
 
         m.def("startFromJSON",
             &startFromJSON,
             "Start Xray client with JSON string",
             py::arg("json"));
 
-        m.attr("__version__") = "1.8.8";
+        m.attr("__version__") = "1.8.9";
     }
 }
```

### Comparing `Xray-core-1.8.8/xray-go/.github/dependabot.yml` & `Xray-core-1.8.9/xray-go/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/.github/docker/Dockerfile` & `Xray-core-1.8.9/xray-go/.github/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/.github/workflows/docker.yml` & `Xray-core-1.8.9/xray-go/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/.github/workflows/release.yml` & `Xray-core-1.8.9/xray-go/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/.github/workflows/test.yml` & `Xray-core-1.8.9/xray-go/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/CODE_OF_CONDUCT.md` & `Xray-core-1.8.9/xray-go/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/LICENSE` & `Xray-core-1.8.9/xray-go/LICENSE`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/Makefile` & `Xray-core-1.8.9/xray-go/Makefile`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/README.md` & `Xray-core-1.8.9/xray-go/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 [Project X Channel](https://t.me/projectXtls)
 
 ## Installation
 
 - Linux Script
   - [XTLS/Xray-install](https://github.com/XTLS/Xray-install)
+  - [team-cloudchaser/tempest](https://github.com/team-cloudchaser/tempest) (supports [`systemd`](https://systemd.io) and [OpenRC](https://github.com/OpenRC/openrc); Linux-only)
 - Docker
   - Official: [ghcr.io/xtls/xray-core](https://ghcr.io/xtls/xray-core) 
   - [iamybj/docker-xray](https://hub.docker.com/r/iamybj/docker-xray)
   - [teddysun/xray](https://hub.docker.com/r/teddysun/xray)
 - Web Panel
   - [X-UI-English](https://github.com/NidukaAkalanka/x-ui-english), [3X-UI](https://github.com/MHSanaei/3x-ui), [X-UI](https://github.com/alireza0/x-ui), [X-UI](https://github.com/diditra/x-ui)
   - [Xray-UI](https://github.com/qist/xray-ui), [X-UI](https://github.com/sing-web/x-ui)
@@ -97,14 +98,15 @@
   - [xray-knife](https://github.com/lilendian0x00/xray-knife)
 - Xray Wrapper
   - [XTLS/libXray](https://github.com/XTLS/libXray)
   - [xtlsapi](https://github.com/hiddify/xtlsapi)
   - [AndroidLibXrayLite](https://github.com/2dust/AndroidLibXrayLite)
   - [XrayKit](https://github.com/arror/XrayKit)
   - [Xray-core-python](https://github.com/LorenEteval/Xray-core-python)
+  - [xray-api](https://github.com/XVGuardian/xray-api)
 - [XrayR](https://github.com/XrayR-project/XrayR)
   - [XrayR-release](https://github.com/XrayR-project/XrayR-release)
   - [XrayR-V2Board](https://github.com/missuo/XrayR-V2Board)
 - [Clash.Meta](https://github.com/MetaCubeX/Clash.Meta)
   - [Clash Verge](https://github.com/zzzgydi/clash-verge)
   - [clashN](https://github.com/2dust/clashN)
   - [Clash Meta for Android](https://github.com/MetaCubeX/ClashMetaForAndroid)
```

### Comparing `Xray-core-1.8.8/xray-go/app/commander/commander.go` & `Xray-core-1.8.9/xray-go/app/commander/commander.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/commander/config.pb.go` & `Xray-core-1.8.9/xray-go/app/commander/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/commander/config.proto` & `Xray-core-1.8.9/xray-go/app/commander/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/commander/outbound.go` & `Xray-core-1.8.9/xray-go/app/commander/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/commander/service.go` & `Xray-core-1.8.9/xray-go/app/commander/service.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dispatcher/config.pb.go` & `Xray-core-1.8.9/xray-go/app/dispatcher/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dispatcher/default.go` & `Xray-core-1.8.9/xray-go/app/dispatcher/default.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dispatcher/fakednssniffer.go` & `Xray-core-1.8.9/xray-go/app/dispatcher/fakednssniffer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dispatcher/sniffer.go` & `Xray-core-1.8.9/xray-go/app/dispatcher/sniffer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dispatcher/stats.go` & `Xray-core-1.8.9/xray-go/app/dispatcher/stats.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dispatcher/stats_test.go` & `Xray-core-1.8.9/xray-go/app/dispatcher/stats_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/config.go` & `Xray-core-1.8.9/xray-go/app/dns/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/config.pb.go` & `Xray-core-1.8.9/xray-go/app/dns/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/config.proto` & `Xray-core-1.8.9/xray-go/app/dns/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/dns.go` & `Xray-core-1.8.9/xray-go/app/dns/dns.go`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,15 @@
 	option.IPv6Enable = option.IPv6Enable && s.ipOption.IPv6Enable
 
 	if !option.IPv4Enable && !option.IPv6Enable {
 		return nil, dns.ErrEmptyResponse
 	}
 
 	// Normalize the FQDN form query
-	if strings.HasSuffix(domain, ".") {
-		domain = domain[:len(domain)-1]
-	}
+	domain = strings.TrimSuffix(domain, ".")
 
 	// Static host lookup
 	switch addrs := s.hosts.Lookup(domain, option); {
 	case addrs == nil: // Domain not recorded in static host
 		break
 	case len(addrs) == 0: // Domain recorded, but no valid IP returned (e.g. IPv4 address with only IPv6 enabled)
 		return nil, dns.ErrEmptyResponse
```

### Comparing `Xray-core-1.8.8/xray-go/app/dns/dns_test.go` & `Xray-core-1.8.9/xray-go/app/dns/dns_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/dnscommon.go` & `Xray-core-1.8.9/xray-go/app/dns/dnscommon.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/dnscommon_test.go` & `Xray-core-1.8.9/xray-go/app/dns/dnscommon_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/fakedns/fake.go` & `Xray-core-1.8.9/xray-go/app/dns/fakedns/fake.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/fakedns/fakedns.pb.go` & `Xray-core-1.8.9/xray-go/app/dns/fakedns/fakedns.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/fakedns/fakedns_test.go` & `Xray-core-1.8.9/xray-go/app/dns/fakedns/fakedns_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/hosts.go` & `Xray-core-1.8.9/xray-go/app/dns/hosts.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/hosts_test.go` & `Xray-core-1.8.9/xray-go/app/dns/hosts_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_doh.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_doh.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_doh_test.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_doh_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_fakedns.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_fakedns.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_local.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_local.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_local_test.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_local_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_quic.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_quic.go`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 package dns
 
 import (
+	"bytes"
 	"context"
+	"encoding/binary"
 	"net/url"
 	"sync"
 	"sync/atomic"
 	"time"
 
 	"github.com/quic-go/quic-go"
 	"github.com/xtls/xray-core/common"
@@ -20,15 +22,15 @@
 	"github.com/xtls/xray-core/transport/internet/tls"
 	"golang.org/x/net/dns/dnsmessage"
 	"golang.org/x/net/http2"
 )
 
 // NextProtoDQ - During connection establishment, DNS/QUIC support is indicated
 // by selecting the ALPN token "dq" in the crypto handshake.
-const NextProtoDQ = "doq-i00"
+const NextProtoDQ = "doq"
 
 const handshakeTimeout = time.Second * 8
 
 // QUICNameServer implemented DNS over QUIC
 type QUICNameServer struct {
 	sync.RWMutex
 	ips           map[string]*record
@@ -190,33 +192,50 @@
 
 			b, err := dns.PackMessage(r.msg)
 			if err != nil {
 				newError("failed to pack dns query").Base(err).AtError().WriteToLog()
 				return
 			}
 
+			dnsReqBuf := buf.New()
+			binary.Write(dnsReqBuf, binary.BigEndian, uint16(b.Len()))
+			dnsReqBuf.Write(b.Bytes())
+			b.Release()
+
 			conn, err := s.openStream(dnsCtx)
 			if err != nil {
 				newError("failed to open quic connection").Base(err).AtError().WriteToLog()
 				return
 			}
 
-			_, err = conn.Write(b.Bytes())
+			_, err = conn.Write(dnsReqBuf.Bytes())
 			if err != nil {
 				newError("failed to send query").Base(err).AtError().WriteToLog()
 				return
 			}
 
 			_ = conn.Close()
 
 			respBuf := buf.New()
 			defer respBuf.Release()
-			n, err := respBuf.ReadFrom(conn)
+			n, err := respBuf.ReadFullFrom(conn, 2)
+			if err != nil && n == 0 {
+				newError("failed to read response length").Base(err).AtError().WriteToLog()
+				return
+			}
+			var length int16
+			err = binary.Read(bytes.NewReader(respBuf.Bytes()), binary.BigEndian, &length)
+			if err != nil {
+				newError("failed to parse response length").Base(err).AtError().WriteToLog()
+				return
+			}
+			respBuf.Clear()
+			n, err = respBuf.ReadFullFrom(conn, int32(length))
 			if err != nil && n == 0 {
-				newError("failed to read response").Base(err).AtError().WriteToLog()
+				newError("failed to read response length").Base(err).AtError().WriteToLog()
 				return
 			}
 
 			rec, err := parseResponse(respBuf.Bytes())
 			if err != nil {
 				newError("failed to handle response").Base(err).AtError().WriteToLog()
 				return
```

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_quic_test.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_quic_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_tcp.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_tcp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_tcp_test.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_tcp_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/dns/nameserver_udp.go` & `Xray-core-1.8.9/xray-go/app/dns/nameserver_udp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/command/command.go` & `Xray-core-1.8.9/xray-go/app/log/command/command.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/command/command_test.go` & `Xray-core-1.8.9/xray-go/app/log/command/command_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/command/config.pb.go` & `Xray-core-1.8.9/xray-go/app/log/command/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/command/config_grpc.pb.go` & `Xray-core-1.8.9/xray-go/app/log/command/config_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/config.pb.go` & `Xray-core-1.8.9/xray-go/app/log/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/config.proto` & `Xray-core-1.8.9/xray-go/app/log/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/log.go` & `Xray-core-1.8.9/xray-go/app/log/log.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/log_creator.go` & `Xray-core-1.8.9/xray-go/app/log/log_creator.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/log/log_test.go` & `Xray-core-1.8.9/xray-go/app/log/log_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/metrics/config.pb.go` & `Xray-core-1.8.9/xray-go/app/metrics/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/metrics/metrics.go` & `Xray-core-1.8.9/xray-go/app/metrics/metrics.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/metrics/outbound.go` & `Xray-core-1.8.9/xray-go/app/metrics/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/burst/burstobserver.go` & `Xray-core-1.8.9/xray-go/app/observatory/burst/burstobserver.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/burst/config.pb.go` & `Xray-core-1.8.9/xray-go/app/observatory/burst/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/burst/config.proto` & `Xray-core-1.8.9/xray-go/app/observatory/burst/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/burst/healthping.go` & `Xray-core-1.8.9/xray-go/app/observatory/burst/healthping.go`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,23 @@
 	}
 	interval := h.Settings.Interval * time.Duration(h.Settings.SamplingCount)
 	ticker := time.NewTicker(interval)
 	tickerClose := make(chan struct{})
 	h.ticker = ticker
 	h.tickerClose = tickerClose
 	go func() {
+		tags, err := selector()
+		if err != nil {
+			newError("error select outbounds for initial health check: ", err).AtWarning().WriteToLog()
+			return
+		}
+		h.Check(tags)
+	}()
+
+	go func() {
 		for {
 			go func() {
 				tags, err := selector()
 				if err != nil {
 					newError("error select outbounds for scheduled health check: ", err).AtWarning().WriteToLog()
 					return
 				}
```

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/burst/healthping_result.go` & `Xray-core-1.8.9/xray-go/app/observatory/burst/healthping_result.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/burst/healthping_result_test.go` & `Xray-core-1.8.9/xray-go/app/observatory/burst/healthping_result_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/burst/ping.go` & `Xray-core-1.8.9/xray-go/app/observatory/burst/ping.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/command/command.go` & `Xray-core-1.8.9/xray-go/app/observatory/command/command.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/command/command.pb.go` & `Xray-core-1.8.9/xray-go/app/observatory/command/command.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/command/command.proto` & `Xray-core-1.8.9/xray-go/app/observatory/command/command.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/command/command_grpc.pb.go` & `Xray-core-1.8.9/xray-go/app/observatory/command/command_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/config.pb.go` & `Xray-core-1.8.9/xray-go/app/observatory/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/config.proto` & `Xray-core-1.8.9/xray-go/app/observatory/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/explainErrors.go` & `Xray-core-1.8.9/xray-go/app/observatory/explainErrors.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/observatory/observer.go` & `Xray-core-1.8.9/xray-go/app/observatory/observer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/policy/config.go` & `Xray-core-1.8.9/xray-go/app/policy/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/policy/config.pb.go` & `Xray-core-1.8.9/xray-go/app/policy/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/policy/config.proto` & `Xray-core-1.8.9/xray-go/app/policy/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/policy/manager.go` & `Xray-core-1.8.9/xray-go/app/policy/manager.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/policy/manager_test.go` & `Xray-core-1.8.9/xray-go/app/policy/manager_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/command/command.go` & `Xray-core-1.8.9/xray-go/app/proxyman/command/command.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/command/command.pb.go` & `Xray-core-1.8.9/xray-go/app/proxyman/command/command.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/command/command.proto` & `Xray-core-1.8.9/xray-go/app/proxyman/command/command.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/command/command_grpc.pb.go` & `Xray-core-1.8.9/xray-go/app/proxyman/command/command_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/config.go` & `Xray-core-1.8.9/xray-go/app/proxyman/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/config.pb.go` & `Xray-core-1.8.9/xray-go/app/proxyman/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/config.proto` & `Xray-core-1.8.9/xray-go/app/proxyman/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/inbound/always.go` & `Xray-core-1.8.9/xray-go/app/proxyman/inbound/always.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/inbound/dynamic.go` & `Xray-core-1.8.9/xray-go/app/proxyman/inbound/dynamic.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/inbound/inbound.go` & `Xray-core-1.8.9/xray-go/app/proxyman/inbound/inbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/inbound/worker.go` & `Xray-core-1.8.9/xray-go/app/proxyman/inbound/worker.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/outbound/handler.go` & `Xray-core-1.8.9/xray-go/app/proxyman/outbound/handler.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/outbound/handler_test.go` & `Xray-core-1.8.9/xray-go/app/proxyman/outbound/handler_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/outbound/outbound.go` & `Xray-core-1.8.9/xray-go/app/proxyman/outbound/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/proxyman/outbound/uot.go` & `Xray-core-1.8.9/xray-go/app/proxyman/outbound/uot.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/reverse/bridge.go` & `Xray-core-1.8.9/xray-go/app/reverse/bridge.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/reverse/config.pb.go` & `Xray-core-1.8.9/xray-go/app/reverse/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/reverse/config.proto` & `Xray-core-1.8.9/xray-go/app/reverse/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/reverse/portal.go` & `Xray-core-1.8.9/xray-go/app/reverse/portal.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/reverse/reverse.go` & `Xray-core-1.8.9/xray-go/app/reverse/reverse.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/balancing.go` & `Xray-core-1.8.9/xray-go/app/router/balancing.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/balancing_override.go` & `Xray-core-1.8.9/xray-go/app/router/balancing_override.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/command/command.go` & `Xray-core-1.8.9/xray-go/app/router/command/command.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/command/command.pb.go` & `Xray-core-1.8.9/xray-go/app/router/command/command.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/command/command.proto` & `Xray-core-1.8.9/xray-go/app/router/command/command.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/command/command_grpc.pb.go` & `Xray-core-1.8.9/xray-go/app/router/command/command_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/command/command_test.go` & `Xray-core-1.8.9/xray-go/app/router/command/command_test.go`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	. "github.com/xtls/xray-core/app/router/command"
 	"github.com/xtls/xray-core/app/stats"
 	"github.com/xtls/xray-core/common"
 	"github.com/xtls/xray-core/common/net"
 	"github.com/xtls/xray-core/features/routing"
 	"github.com/xtls/xray-core/testing/mocks"
 	"google.golang.org/grpc"
+	"google.golang.org/grpc/credentials/insecure"
 	"google.golang.org/grpc/test/bufconn"
 )
 
 func TestServiceSubscribeRoutingStats(t *testing.T) {
 	c := stats.NewChannel(&stats.ChannelConfig{
 		SubscriberLimit: 1,
 		BufferSize:      0,
@@ -76,15 +77,15 @@
 			errCh <- err
 		}
 	}()
 
 	// Client goroutine
 	go func() {
 		defer lis.Close()
-		conn, err := grpc.DialContext(context.Background(), "bufnet", grpc.WithContextDialer(bufDialer), grpc.WithInsecure())
+		conn, err := grpc.DialContext(context.Background(), "bufnet", grpc.WithContextDialer(bufDialer), grpc.WithTransportCredentials(insecure.NewCredentials()))
 		if err != nil {
 			errCh <- err
 			return
 		}
 		defer conn.Close()
 		client := NewRoutingServiceClient(conn)
 
@@ -210,15 +211,15 @@
 			errCh <- err
 		}
 	}()
 
 	// Client goroutine
 	go func() {
 		defer lis.Close()
-		conn, err := grpc.DialContext(context.Background(), "bufnet", grpc.WithContextDialer(bufDialer), grpc.WithInsecure())
+		conn, err := grpc.DialContext(context.Background(), "bufnet", grpc.WithContextDialer(bufDialer), grpc.WithTransportCredentials(insecure.NewCredentials()))
 		if err != nil {
 			errCh <- err
 			return
 		}
 		defer conn.Close()
 		client := NewRoutingServiceClient(conn)
 
@@ -333,15 +334,15 @@
 		RegisterRoutingServiceServer(server, NewRoutingServer(r, c))
 		errCh <- server.Serve(lis)
 	}()
 
 	// Client goroutine
 	go func() {
 		defer lis.Close()
-		conn, err := grpc.DialContext(context.Background(), "bufnet", grpc.WithContextDialer(bufDialer), grpc.WithInsecure())
+		conn, err := grpc.DialContext(context.Background(), "bufnet", grpc.WithContextDialer(bufDialer), grpc.WithTransportCredentials(insecure.NewCredentials()))
 		if err != nil {
 			errCh <- err
 		}
 		defer conn.Close()
 		client := NewRoutingServiceClient(conn)
 
 		testCases := []*RoutingContext{
```

### Comparing `Xray-core-1.8.8/xray-go/app/router/command/config.go` & `Xray-core-1.8.9/xray-go/app/router/command/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/condition.go` & `Xray-core-1.8.9/xray-go/app/router/condition.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/condition_geoip.go` & `Xray-core-1.8.9/xray-go/app/router/condition_geoip.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/condition_geoip_test.go` & `Xray-core-1.8.9/xray-go/app/router/condition_geoip_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/condition_test.go` & `Xray-core-1.8.9/xray-go/app/router/condition_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/config.go` & `Xray-core-1.8.9/xray-go/app/router/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/config.pb.go` & `Xray-core-1.8.9/xray-go/app/router/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/config.proto` & `Xray-core-1.8.9/xray-go/app/router/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/router.go` & `Xray-core-1.8.9/xray-go/app/router/router.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/router_test.go` & `Xray-core-1.8.9/xray-go/app/router/router_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/strategy_leastload.go` & `Xray-core-1.8.9/xray-go/app/router/strategy_leastload.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/strategy_leastload_test.go` & `Xray-core-1.8.9/xray-go/app/router/strategy_leastload_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/strategy_leastping.go` & `Xray-core-1.8.9/xray-go/app/router/strategy_leastping.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/weight.go` & `Xray-core-1.8.9/xray-go/app/router/weight.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/router/weight_test.go` & `Xray-core-1.8.9/xray-go/app/router/weight_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/channel.go` & `Xray-core-1.8.9/xray-go/app/stats/channel.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/channel_test.go` & `Xray-core-1.8.9/xray-go/app/stats/channel_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/command/command.go` & `Xray-core-1.8.9/xray-go/app/stats/command/command.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/command/command.pb.go` & `Xray-core-1.8.9/xray-go/app/stats/command/command.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/command/command.proto` & `Xray-core-1.8.9/xray-go/app/stats/command/command.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/command/command_grpc.pb.go` & `Xray-core-1.8.9/xray-go/app/stats/command/command_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/command/command_test.go` & `Xray-core-1.8.9/xray-go/app/stats/command/command_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/config.pb.go` & `Xray-core-1.8.9/xray-go/app/stats/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/counter_test.go` & `Xray-core-1.8.9/xray-go/app/stats/counter_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/stats.go` & `Xray-core-1.8.9/xray-go/app/stats/stats.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/app/stats/stats_test.go` & `Xray-core-1.8.9/xray-go/app/stats/stats_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/antireplay/bloomring.go` & `Xray-core-1.8.9/xray-go/common/antireplay/bloomring.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/antireplay/replayfilter.go` & `Xray-core-1.8.9/xray-go/common/antireplay/replayfilter.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/bitmask/byte_test.go` & `Xray-core-1.8.9/xray-go/common/bitmask/byte_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/buffer.go` & `Xray-core-1.8.9/xray-go/common/buf/buffer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/buffer_test.go` & `Xray-core-1.8.9/xray-go/common/buf/buffer_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/copy.go` & `Xray-core-1.8.9/xray-go/common/buf/copy.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/copy_test.go` & `Xray-core-1.8.9/xray-go/common/buf/copy_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/io.go` & `Xray-core-1.8.9/xray-go/common/buf/io.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/io_test.go` & `Xray-core-1.8.9/xray-go/common/buf/io_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/multi_buffer.go` & `Xray-core-1.8.9/xray-go/common/buf/multi_buffer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/multi_buffer_test.go` & `Xray-core-1.8.9/xray-go/common/buf/multi_buffer_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/override.go` & `Xray-core-1.8.9/xray-go/common/buf/override.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/reader.go` & `Xray-core-1.8.9/xray-go/common/buf/reader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/reader_test.go` & `Xray-core-1.8.9/xray-go/common/buf/reader_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/readv_posix.go` & `Xray-core-1.8.9/xray-go/common/buf/readv_posix.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/readv_reader.go` & `Xray-core-1.8.9/xray-go/common/buf/readv_reader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/readv_test.go` & `Xray-core-1.8.9/xray-go/common/buf/readv_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/readv_unix.go` & `Xray-core-1.8.9/xray-go/common/buf/readv_unix.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/readv_windows.go` & `Xray-core-1.8.9/xray-go/common/buf/readv_windows.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/writer.go` & `Xray-core-1.8.9/xray-go/common/buf/writer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/buf/writer_test.go` & `Xray-core-1.8.9/xray-go/common/buf/writer_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/bytespool/pool.go` & `Xray-core-1.8.9/xray-go/common/bytespool/pool.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/cache/lru.go` & `Xray-core-1.8.9/xray-go/common/cache/lru.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/cache/lru_test.go` & `Xray-core-1.8.9/xray-go/common/cache/lru_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/common.go` & `Xray-core-1.8.9/xray-go/common/common.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/common_test.go` & `Xray-core-1.8.9/xray-go/common/common_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/aes.go` & `Xray-core-1.8.9/xray-go/common/crypto/aes.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/auth.go` & `Xray-core-1.8.9/xray-go/common/crypto/auth.go`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 		r.hasSize = true
 		return errSoft
 	}
 
 	if size <= buf.Size {
 		b, err := r.readBuffer(int32(size), int32(padding))
 		if err != nil {
-			return nil
+			return err
 		}
 		*mb = append(*mb, b)
 		return nil
 	}
 
 	payload := bytespool.Alloc(int32(size))
 	defer bytespool.Free(payload)
```

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/auth_test.go` & `Xray-core-1.8.9/xray-go/common/crypto/auth_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/benchmark_test.go` & `Xray-core-1.8.9/xray-go/common/crypto/benchmark_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/chacha20_test.go` & `Xray-core-1.8.9/xray-go/common/crypto/chacha20_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/chunk.go` & `Xray-core-1.8.9/xray-go/common/crypto/chunk.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/chunk_test.go` & `Xray-core-1.8.9/xray-go/common/crypto/chunk_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/internal/chacha.go` & `Xray-core-1.8.9/xray-go/common/crypto/internal/chacha.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/internal/chacha_core.generated.go` & `Xray-core-1.8.9/xray-go/common/crypto/internal/chacha_core.generated.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/internal/chacha_core_gen.go` & `Xray-core-1.8.9/xray-go/common/crypto/internal/chacha_core_gen.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/crypto/io.go` & `Xray-core-1.8.9/xray-go/common/crypto/io.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/dice/dice_test.go` & `Xray-core-1.8.9/xray-go/common/dice/dice_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/drain/drainer.go` & `Xray-core-1.8.9/xray-go/common/drain/drainer.go`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 package drain
 
 import (
 	"io"
-	"io/ioutil"
 
 	"github.com/xtls/xray-core/common/dice"
 )
 
 type BehaviorSeedLimitedDrainer struct {
 	DrainSize int
 }
@@ -32,15 +31,15 @@
 		}
 		return newError("unable to drain connection").Base(err)
 	}
 	return nil
 }
 
 func drainReadN(reader io.Reader, n int) error {
-	_, err := io.CopyN(ioutil.Discard, reader, int64(n))
+	_, err := io.CopyN(io.Discard, reader, int64(n))
 	return err
 }
 
 func WithError(drainer Drainer, reader io.Reader, err error) error {
 	drainErr := drainer.Drain(reader)
 	if drainErr == nil {
 		return err
```

### Comparing `Xray-core-1.8.8/xray-go/common/errors/errorgen/main.go` & `Xray-core-1.8.9/xray-go/common/errors/errorgen/main.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/errors/errors.go` & `Xray-core-1.8.9/xray-go/common/errors/errors.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/errors/errors_test.go` & `Xray-core-1.8.9/xray-go/common/errors/errors_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/errors/multi_error.go` & `Xray-core-1.8.9/xray-go/common/errors/multi_error.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/interfaces.go` & `Xray-core-1.8.9/xray-go/common/interfaces.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/log/access.go` & `Xray-core-1.8.9/xray-go/common/log/access.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/log/dns.go` & `Xray-core-1.8.9/xray-go/common/log/dns.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/log/log.go` & `Xray-core-1.8.9/xray-go/common/log/log.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/log/log.pb.go` & `Xray-core-1.8.9/xray-go/common/log/log.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/log/log_test.go` & `Xray-core-1.8.9/xray-go/common/log/log_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/log/logger.go` & `Xray-core-1.8.9/xray-go/common/log/logger.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/log/logger_test.go` & `Xray-core-1.8.9/xray-go/common/log/logger_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/client.go` & `Xray-core-1.8.9/xray-go/common/mux/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/client_test.go` & `Xray-core-1.8.9/xray-go/common/mux/client_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/frame.go` & `Xray-core-1.8.9/xray-go/common/mux/frame.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/frame_test.go` & `Xray-core-1.8.9/xray-go/common/mux/frame_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/mux_test.go` & `Xray-core-1.8.9/xray-go/common/mux/mux_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/reader.go` & `Xray-core-1.8.9/xray-go/common/mux/reader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/server.go` & `Xray-core-1.8.9/xray-go/common/mux/server.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/session.go` & `Xray-core-1.8.9/xray-go/common/mux/session.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/session_test.go` & `Xray-core-1.8.9/xray-go/common/mux/session_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/mux/writer.go` & `Xray-core-1.8.9/xray-go/common/mux/writer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/address.go` & `Xray-core-1.8.9/xray-go/common/net/address.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/address.pb.go` & `Xray-core-1.8.9/xray-go/common/net/address.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/address_test.go` & `Xray-core-1.8.9/xray-go/common/net/address_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/cnc/connection.go` & `Xray-core-1.8.9/xray-go/common/net/cnc/connection.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/destination.go` & `Xray-core-1.8.9/xray-go/common/net/destination.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/destination.pb.go` & `Xray-core-1.8.9/xray-go/common/net/destination.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/destination_test.go` & `Xray-core-1.8.9/xray-go/common/net/destination_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/network.pb.go` & `Xray-core-1.8.9/xray-go/common/net/network.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/port.go` & `Xray-core-1.8.9/xray-go/common/net/port.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/port.pb.go` & `Xray-core-1.8.9/xray-go/common/net/port.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/port.proto` & `Xray-core-1.8.9/xray-go/common/net/port.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/net/system.go` & `Xray-core-1.8.9/xray-go/common/net/system.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/ocsp/ocsp.go` & `Xray-core-1.8.9/xray-go/common/ocsp/ocsp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/platform/ctlcmd/ctlcmd.go` & `Xray-core-1.8.9/xray-go/common/platform/ctlcmd/ctlcmd.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/platform/filesystem/file.go` & `Xray-core-1.8.9/xray-go/common/platform/filesystem/file.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/platform/others.go` & `Xray-core-1.8.9/xray-go/common/platform/others.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/platform/platform.go` & `Xray-core-1.8.9/xray-go/common/platform/platform.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/platform/platform_test.go` & `Xray-core-1.8.9/xray-go/common/platform/platform_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/platform/windows.go` & `Xray-core-1.8.9/xray-go/common/platform/windows.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/address.go` & `Xray-core-1.8.9/xray-go/common/protocol/address.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/address_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/address_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/bittorrent/bittorrent.go` & `Xray-core-1.8.9/xray-go/common/protocol/bittorrent/bittorrent.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/dns/io.go` & `Xray-core-1.8.9/xray-go/common/protocol/dns/io.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/headers.go` & `Xray-core-1.8.9/xray-go/common/protocol/headers.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/headers.pb.go` & `Xray-core-1.8.9/xray-go/common/protocol/headers.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/http/headers.go` & `Xray-core-1.8.9/xray-go/common/protocol/http/headers.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/http/headers_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/http/headers_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/http/sniff.go` & `Xray-core-1.8.9/xray-go/common/protocol/http/sniff.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/http/sniff_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/http/sniff_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/id.go` & `Xray-core-1.8.9/xray-go/common/protocol/id.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/quic/sniff.go` & `Xray-core-1.8.9/xray-go/common/protocol/quic/sniff.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/quic/sniff_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/quic/sniff_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/server_picker.go` & `Xray-core-1.8.9/xray-go/common/protocol/server_picker.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/server_picker_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/server_picker_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/server_spec.go` & `Xray-core-1.8.9/xray-go/common/protocol/server_spec.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/server_spec.pb.go` & `Xray-core-1.8.9/xray-go/common/protocol/server_spec.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/server_spec_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/server_spec_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/tls/cert/cert.go` & `Xray-core-1.8.9/xray-go/common/protocol/tls/cert/cert.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/tls/cert/cert_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/tls/cert/cert_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/tls/cert/privateKey.go` & `Xray-core-1.8.9/xray-go/common/protocol/tls/cert/privateKey.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/tls/sniff.go` & `Xray-core-1.8.9/xray-go/common/protocol/tls/sniff.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/tls/sniff_test.go` & `Xray-core-1.8.9/xray-go/common/protocol/tls/sniff_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/user.go` & `Xray-core-1.8.9/xray-go/common/protocol/user.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/user.pb.go` & `Xray-core-1.8.9/xray-go/common/protocol/user.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/protocol/user.proto` & `Xray-core-1.8.9/xray-go/common/protocol/user.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/reflect/marshal.go` & `Xray-core-1.8.9/xray-go/common/reflect/marshal.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/reflect/marshal_test.go` & `Xray-core-1.8.9/xray-go/common/reflect/marshal_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/retry/retry.go` & `Xray-core-1.8.9/xray-go/common/retry/retry.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/retry/retry_test.go` & `Xray-core-1.8.9/xray-go/common/retry/retry_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/serial/serial.go` & `Xray-core-1.8.9/xray-go/common/serial/serial.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/serial/serial_test.go` & `Xray-core-1.8.9/xray-go/common/serial/serial_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/serial/string.go` & `Xray-core-1.8.9/xray-go/common/serial/string.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/serial/string_test.go` & `Xray-core-1.8.9/xray-go/common/serial/string_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/serial/typed_message.go` & `Xray-core-1.8.9/xray-go/common/serial/typed_message.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/serial/typed_message.pb.go` & `Xray-core-1.8.9/xray-go/common/serial/typed_message.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/session/context.go` & `Xray-core-1.8.9/xray-go/common/session/context.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/session/session.go` & `Xray-core-1.8.9/xray-go/common/session/session.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/signal/done/done.go` & `Xray-core-1.8.9/xray-go/common/signal/done/done.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/signal/notifier.go` & `Xray-core-1.8.9/xray-go/common/signal/notifier.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/signal/pubsub/pubsub.go` & `Xray-core-1.8.9/xray-go/common/signal/pubsub/pubsub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/signal/semaphore/semaphore.go` & `Xray-core-1.8.9/xray-go/common/signal/semaphore/semaphore.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/signal/timer.go` & `Xray-core-1.8.9/xray-go/common/signal/timer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/signal/timer_test.go` & `Xray-core-1.8.9/xray-go/common/signal/timer_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/singbridge/destination.go` & `Xray-core-1.8.9/xray-go/common/singbridge/destination.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/singbridge/dialer.go` & `Xray-core-1.8.9/xray-go/common/singbridge/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/singbridge/handler.go` & `Xray-core-1.8.9/xray-go/common/singbridge/handler.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/singbridge/logger.go` & `Xray-core-1.8.9/xray-go/common/singbridge/logger.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/singbridge/packet.go` & `Xray-core-1.8.9/xray-go/common/singbridge/packet.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/singbridge/pipe.go` & `Xray-core-1.8.9/xray-go/common/singbridge/pipe.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/singbridge/reader.go` & `Xray-core-1.8.9/xray-go/common/singbridge/reader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/ac_automaton_matcher.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/ac_automaton_matcher.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/benchmark_test.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/benchmark_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/domain_matcher.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/domain_matcher.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/domain_matcher_test.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/domain_matcher_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/full_matcher_test.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/full_matcher_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/matchers.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/matchers.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/matchers_test.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/matchers_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/mph_matcher.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/mph_matcher.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/strmatcher.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/strmatcher.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/strmatcher/strmatcher_test.go` & `Xray-core-1.8.9/xray-go/common/strmatcher/strmatcher_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/task/periodic.go` & `Xray-core-1.8.9/xray-go/common/task/periodic.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/task/periodic_test.go` & `Xray-core-1.8.9/xray-go/common/task/periodic_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/task/task.go` & `Xray-core-1.8.9/xray-go/common/task/task.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/task/task_test.go` & `Xray-core-1.8.9/xray-go/common/task/task_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/type.go` & `Xray-core-1.8.9/xray-go/common/type.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/type_test.go` & `Xray-core-1.8.9/xray-go/common/type_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/units/bytesize.go` & `Xray-core-1.8.9/xray-go/common/units/bytesize.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/units/bytesize_test.go` & `Xray-core-1.8.9/xray-go/common/units/bytesize_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/uuid/uuid.go` & `Xray-core-1.8.9/xray-go/common/uuid/uuid.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/uuid/uuid_test.go` & `Xray-core-1.8.9/xray-go/common/uuid/uuid_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/xudp/xudp.go` & `Xray-core-1.8.9/xray-go/common/xudp/xudp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/common/xudp/xudp_test.go` & `Xray-core-1.8.9/xray-go/common/xudp/xudp_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/annotations.go` & `Xray-core-1.8.9/xray-go/core/annotations.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/config.go` & `Xray-core-1.8.9/xray-go/core/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/config.pb.go` & `Xray-core-1.8.9/xray-go/core/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/config.proto` & `Xray-core-1.8.9/xray-go/core/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/context.go` & `Xray-core-1.8.9/xray-go/core/context.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/core.go` & `Xray-core-1.8.9/xray-go/core/core.go`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 	"github.com/xtls/xray-core/common/serial"
 )
 
 var (
 	Version_x byte = 1
 	Version_y byte = 8
-	Version_z byte = 8
+	Version_z byte = 9
 )
 
 var (
 	build    = "Custom"
 	codename = "Xray, Penetrates Everything."
 	intro    = "A unified platform for anti-censorship."
 )
```

### Comparing `Xray-core-1.8.8/xray-go/core/functions.go` & `Xray-core-1.8.9/xray-go/core/functions.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/functions_test.go` & `Xray-core-1.8.9/xray-go/core/functions_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/mocks.go` & `Xray-core-1.8.9/xray-go/core/mocks.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/xray.go` & `Xray-core-1.8.9/xray-go/core/xray.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/core/xray_test.go` & `Xray-core-1.8.9/xray-go/core/xray_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/dns/client.go` & `Xray-core-1.8.9/xray-go/features/dns/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/dns/localdns/client.go` & `Xray-core-1.8.9/xray-go/features/dns/localdns/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/feature.go` & `Xray-core-1.8.9/xray-go/features/feature.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/inbound/inbound.go` & `Xray-core-1.8.9/xray-go/features/inbound/inbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/outbound/outbound.go` & `Xray-core-1.8.9/xray-go/features/outbound/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/policy/default.go` & `Xray-core-1.8.9/xray-go/features/policy/default.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/policy/policy.go` & `Xray-core-1.8.9/xray-go/features/policy/policy.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/routing/context.go` & `Xray-core-1.8.9/xray-go/features/routing/context.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/routing/dispatcher.go` & `Xray-core-1.8.9/xray-go/features/routing/dispatcher.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/routing/dns/context.go` & `Xray-core-1.8.9/xray-go/features/routing/dns/context.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/routing/router.go` & `Xray-core-1.8.9/xray-go/features/routing/router.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/routing/session/context.go` & `Xray-core-1.8.9/xray-go/features/routing/session/context.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/features/stats/stats.go` & `Xray-core-1.8.9/xray-go/features/stats/stats.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/go.mod` & `Xray-core-1.8.9/xray-go/go.mod`

 * *Files 8% similar despite different names*

```diff
@@ -8,54 +8,54 @@
 	github.com/google/go-cmp v0.6.0
 	github.com/gorilla/websocket v1.5.1
 	github.com/miekg/dns v1.1.58
 	github.com/pelletier/go-toml v1.9.5
 	github.com/pires/go-proxyproto v0.7.0
 	github.com/quic-go/quic-go v0.41.0
 	github.com/refraction-networking/utls v1.6.3
-	github.com/sagernet/sing v0.3.2
+	github.com/sagernet/sing v0.3.6
 	github.com/sagernet/sing-shadowsocks v0.2.6
 	github.com/seiflotfy/cuckoofilter v0.0.0-20220411075957-e3b120b3f5fb
-	github.com/stretchr/testify v1.8.4
+	github.com/stretchr/testify v1.9.0
 	github.com/v2fly/ss-bloomring v0.0.0-20210312155135-28617310f63e
 	github.com/vishvananda/netlink v1.2.1-beta.2.0.20230316163032-ced5aaba43e3
 	github.com/xtls/reality v0.0.0-20231112171332-de1173cf2b19
 	go4.org/netipx v0.0.0-20231129151722-fdeea329fbba
-	golang.org/x/crypto v0.19.0
-	golang.org/x/net v0.21.0
+	golang.org/x/crypto v0.21.0
+	golang.org/x/net v0.22.0
 	golang.org/x/sync v0.6.0
-	golang.org/x/sys v0.17.0
+	golang.org/x/sys v0.18.0
 	golang.zx2c4.com/wireguard v0.0.0-20231211153847-12269c276173
-	google.golang.org/grpc v1.62.0
-	google.golang.org/protobuf v1.32.0
+	google.golang.org/grpc v1.62.1
+	google.golang.org/protobuf v1.33.0
 	gvisor.dev/gvisor v0.0.0-20231104011432-48a6d7d5bd0b
 	h12.io/socks v1.0.3
 	lukechampine.com/blake3 v1.2.1
 )
 
 require (
 	github.com/andybalholm/brotli v1.1.0 // indirect
 	github.com/cloudflare/circl v1.3.7 // indirect
 	github.com/davecgh/go-spew v1.1.1 // indirect
 	github.com/dgryski/go-metro v0.0.0-20211217172704-adc40b04c140 // indirect
 	github.com/francoispqt/gojay v1.2.13 // indirect
 	github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 // indirect
-	github.com/golang/protobuf v1.5.3 // indirect
+	github.com/golang/protobuf v1.5.4 // indirect
 	github.com/google/btree v1.1.2 // indirect
-	github.com/google/pprof v0.0.0-20240225044709-fd706174c886 // indirect
+	github.com/google/pprof v0.0.0-20240227163752-401108e1b7e7 // indirect
 	github.com/klauspost/compress v1.17.7 // indirect
 	github.com/klauspost/cpuid/v2 v2.2.7 // indirect
-	github.com/onsi/ginkgo/v2 v2.15.0 // indirect
+	github.com/onsi/ginkgo/v2 v2.16.0 // indirect
 	github.com/pmezard/go-difflib v1.0.0 // indirect
 	github.com/riobard/go-bloom v0.0.0-20200614022211-cdc8013cb5b3 // indirect
 	github.com/vishvananda/netns v0.0.4 // indirect
 	go.uber.org/mock v0.4.0 // indirect
 	golang.org/x/exp v0.0.0-20240222234643-814bf88cf225 // indirect
-	golang.org/x/mod v0.15.0 // indirect
+	golang.org/x/mod v0.16.0 // indirect
 	golang.org/x/text v0.14.0 // indirect
 	golang.org/x/time v0.5.0 // indirect
-	golang.org/x/tools v0.18.0 // indirect
+	golang.org/x/tools v0.19.0 // indirect
 	golang.zx2c4.com/wintun v0.0.0-20230126152724-0fa3db229ce2 // indirect
-	google.golang.org/genproto/googleapis/rpc v0.0.0-20240221002015-b0ce06bbee7c // indirect
+	google.golang.org/genproto/googleapis/rpc v0.0.0-20240308144416-29370a3891b7 // indirect
 	gopkg.in/yaml.v2 v2.4.0 // indirect
 	gopkg.in/yaml.v3 v3.0.1 // indirect
 )
```

### Comparing `Xray-core-1.8.8/xray-go/go.sum` & `Xray-core-1.8.9/xray-go/go.sum`

 * *Files 2% similar despite different names*

```diff
@@ -30,43 +30,41 @@
 github.com/francoispqt/gojay v1.2.13/go.mod h1:ehT5mTG4ua4581f1++1WLG0vPdaA9HaiDsoyrBGkyDY=
 github.com/fsnotify/fsnotify v1.4.7/go.mod h1:jwhsz4b93w/PPRr/qN1Yymfu8t87LnFCMoQvtojpjFo=
 github.com/ghodss/yaml v1.0.0/go.mod h1:4dBDuWmgqj2HViK6kFavaiC9ZROes6MMH2rRYeMEF04=
 github.com/ghodss/yaml v1.0.1-0.20220118164431-d8423dcdf344 h1:Arcl6UOIS/kgO2nW3A65HN+7CMjSDP/gofXL4CZt1V4=
 github.com/ghodss/yaml v1.0.1-0.20220118164431-d8423dcdf344/go.mod h1:GIjDIg/heH5DOkXY3YJ/wNhfHsQHoXGjl8G8amsYQ1I=
 github.com/gliderlabs/ssh v0.1.1/go.mod h1:U7qILu1NlMHj9FlMhZLlkCdDnU1DBEAqr0aevW3Awn0=
 github.com/go-errors/errors v1.0.1/go.mod h1:f4zRHt4oKfwPJE5k8C9vpYG+aDHdBFUsgrm6/TyX73Q=
-github.com/go-logr/logr v1.3.0 h1:2y3SDp0ZXuc6/cjLSZ+Q3ir+QB9T/iG5yYRXqsagWSY=
-github.com/go-logr/logr v1.3.0/go.mod h1:9T104GzyrTigFIr8wt5mBrctHMim0Nb2HLGrmQ40KvY=
+github.com/go-logr/logr v1.4.1 h1:pKouT5E8xu9zeFC39JXRDukb6JFQPXM5p5I91188VAQ=
+github.com/go-logr/logr v1.4.1/go.mod h1:9T104GzyrTigFIr8wt5mBrctHMim0Nb2HLGrmQ40KvY=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572 h1:tfuBGBXKqDEevZMzYi5KSi8KkcZtzBcTgAUUtapy0OI=
 github.com/go-task/slim-sprig v0.0.0-20230315185526-52ccab3ef572/go.mod h1:9Pwr4B2jHnOSGXyyzV8ROjYa2ojvAY6HCGYYfMoC3Ls=
 github.com/gogo/protobuf v1.1.1/go.mod h1:r8qH/GZQm5c6nD/R0oafs1akxWv10x8SbQlK7atdtwQ=
 github.com/golang/glog v0.0.0-20160126235308-23def4e6c14b/go.mod h1:SBH7ygxi8pfUlaOkMMuAQtPIUF8ecWP5IEl/CR7VP2Q=
 github.com/golang/lint v0.0.0-20180702182130-06c8688daad7/go.mod h1:tluoj9z5200jBnyusfRPU2LqT6J+DAorxEvtC7LHB+E=
 github.com/golang/mock v1.1.1/go.mod h1:oTYuIxOrZwtPieC+H1uAHpcLFnEyAGVDL/k47Jfbm0A=
 github.com/golang/mock v1.2.0/go.mod h1:oTYuIxOrZwtPieC+H1uAHpcLFnEyAGVDL/k47Jfbm0A=
 github.com/golang/mock v1.7.0-rc.1 h1:YojYx61/OLFsiv6Rw1Z96LpldJIy31o+UHmwAUMJ6/U=
 github.com/golang/mock v1.7.0-rc.1/go.mod h1:s42URUywIqd+OcERslBJvOjepvNymP31m3q8d/GkuRs=
 github.com/golang/protobuf v1.2.0/go.mod h1:6lQm79b+lXiMfvg/cZm0SGofjICqVBUtrP5yJMmIC1U=
 github.com/golang/protobuf v1.3.1/go.mod h1:6lQm79b+lXiMfvg/cZm0SGofjICqVBUtrP5yJMmIC1U=
-github.com/golang/protobuf v1.5.0/go.mod h1:FsONVRAS9T7sI+LIUmWTfcYkHO4aIWwzhcaSAoJOfIk=
-github.com/golang/protobuf v1.5.3 h1:KhyjKVUg7Usr/dYsdSqoFveMYd5ko72D+zANwlG1mmg=
-github.com/golang/protobuf v1.5.3/go.mod h1:XVQd3VNwM+JqD3oG2Ue2ip4fOMUkwXdXDdiuN0vRsmY=
+github.com/golang/protobuf v1.5.4 h1:i7eJL8qZTpSEXOPTxNKhASYpMn+8e5Q6AdndVa1dWek=
+github.com/golang/protobuf v1.5.4/go.mod h1:lnTiLA8Wa4RWRcIUkrtSVa5nRhsEGBg48fD6rSs7xps=
 github.com/google/btree v0.0.0-20180813153112-4030bb1f1f0c/go.mod h1:lNA+9X1NB3Zf8V7Ke586lFgjr2dZNuvo3lPJSGZ5JPQ=
 github.com/google/btree v1.1.2 h1:xf4v41cLI2Z6FxbKm+8Bu+m8ifhj15JuZ9sa0jZCMUU=
 github.com/google/btree v1.1.2/go.mod h1:qOPhT0dTNdNzV6Z/lhRX0YXUafgPLFUh+gZMl761Gm4=
 github.com/google/go-cmp v0.2.0/go.mod h1:oXzfMopK8JAjlY9xF4vHSVASa0yLyX7SntLO5aqRK0M=
-github.com/google/go-cmp v0.5.5/go.mod h1:v8dTdLbMG2kIc/vJvl+f65V22dbkXbowE6jgT/gNBxE=
 github.com/google/go-cmp v0.6.0 h1:ofyhxvXcZhMsU5ulbFiLKl/XBFqE1GSq7atu8tAmTRI=
 github.com/google/go-cmp v0.6.0/go.mod h1:17dUlkBOakJ0+DkrSSNjCkIjxS6bF9zb3elmeNGIjoY=
 github.com/google/go-github v17.0.0+incompatible/go.mod h1:zLgOLi98H3fifZn+44m+umXrS52loVEgC2AApnigrVQ=
 github.com/google/go-querystring v1.0.0/go.mod h1:odCYkC5MyYFN7vkCjXpyrEuKhc/BUO6wN/zVPAxq5ck=
 github.com/google/martian v2.1.0+incompatible/go.mod h1:9I4somxYTbIHy5NJKHRl3wXiIaQGbYVAs8BPL6v8lEs=
 github.com/google/pprof v0.0.0-20181206194817-3ea8567a2e57/go.mod h1:zfwlbNMJ+OItoe0UupaVj+oy1omPYYDuagoSzA8v9mc=
-github.com/google/pprof v0.0.0-20240225044709-fd706174c886 h1:JSJUTZTQT1Gzb2ROdAKOY3HwzBYcclS2GgumhMfHqjw=
-github.com/google/pprof v0.0.0-20240225044709-fd706174c886/go.mod h1:czg5+yv1E0ZGTi6S6vVK1mke0fV+FaUhNGcd6VRS9Ik=
+github.com/google/pprof v0.0.0-20240227163752-401108e1b7e7 h1:y3N7Bm7Y9/CtpiVkw/ZWj6lSlDF3F74SfKwfTCer72Q=
+github.com/google/pprof v0.0.0-20240227163752-401108e1b7e7/go.mod h1:czg5+yv1E0ZGTi6S6vVK1mke0fV+FaUhNGcd6VRS9Ik=
 github.com/googleapis/gax-go v2.0.0+incompatible/go.mod h1:SFVmujtThgffbyetf+mdk2eWhX2bMyUtNHzFKcPA9HY=
 github.com/googleapis/gax-go/v2 v2.0.3/go.mod h1:LLvjysVCY1JZeum8Z6l8qUty8fiNwE08qbEPm1M08qg=
 github.com/gopherjs/gopherjs v0.0.0-20181017120253-0766667cb4d1/go.mod h1:wJfORRmW1u3UXTncJ5qlYoELFm8eSnnEO6hX4iZ3EWY=
 github.com/gorilla/websocket v1.5.1 h1:gmztn0JnHVt9JZquRuzLw3g4wouNVzKL15iLr/zn/QY=
 github.com/gorilla/websocket v1.5.1/go.mod h1:x3kM2JMyaluk02fnUJpQuwD2dCS5NDG2ZHL0uE0tcaY=
 github.com/gregjones/httpcache v0.0.0-20180305231024-9cad4c3443a7/go.mod h1:FecbI9+v66THATjSRHfNgh1IVFe/9kFxbXtjV0ctIMA=
 github.com/grpc-ecosystem/grpc-gateway v1.5.0/go.mod h1:RSKVYQBd5MCa4OVpNdGskqpgL2+G+NZTnrVHpWWfpdw=
@@ -92,16 +90,16 @@
 github.com/microcosm-cc/bluemonday v1.0.1/go.mod h1:hsXNsILzKxV+sX77C5b8FSuKF00vh2OMYv+xgHpAMF4=
 github.com/miekg/dns v1.1.58 h1:ca2Hdkz+cDg/7eNF6V56jjzuZ4aCAE+DbVkILdQWG/4=
 github.com/miekg/dns v1.1.58/go.mod h1:Ypv+3b/KadlvW9vJfXOTf300O4UqaHFzFCuHz+rPkBY=
 github.com/modern-go/concurrent v0.0.0-20180306012644-bacd9c7ef1dd/go.mod h1:6dJC0mAP4ikYIbvyc7fijjWJddQyLn8Ig3JB5CqoB9Q=
 github.com/modern-go/reflect2 v1.0.1/go.mod h1:bx2lNnkwVCuqBIxFjflWJWanXIb3RllmbCylyMrvgv0=
 github.com/neelance/astrewrite v0.0.0-20160511093645-99348263ae86/go.mod h1:kHJEU3ofeGjhHklVoIGuVj85JJwZ6kWPaJwCIxgnFmo=
 github.com/neelance/sourcemap v0.0.0-20151028013722-8c68805598ab/go.mod h1:Qr6/a/Q4r9LP1IltGz7tA7iOK1WonHEYhu1HRBA7ZiM=
-github.com/onsi/ginkgo/v2 v2.15.0 h1:79HwNRBAZHOEwrczrgSOPy+eFTTlIGELKy5as+ClttY=
-github.com/onsi/ginkgo/v2 v2.15.0/go.mod h1:HlxMHtYF57y6Dpf+mc5529KKmSq9h2FpCF+/ZkwUxKM=
+github.com/onsi/ginkgo/v2 v2.16.0 h1:7q1w9frJDzninhXxjZd+Y/x54XNjG/UlRLIYPZafsPM=
+github.com/onsi/ginkgo/v2 v2.16.0/go.mod h1:llBI3WDLL9Z6taip6f33H76YcWtJv+7R3HigUjbIBOs=
 github.com/onsi/gomega v1.30.0 h1:hvMK7xYz4D3HapigLTeGdId/NcfQx1VHMJc60ew99+8=
 github.com/onsi/gomega v1.30.0/go.mod h1:9sxs+SwGrKI0+PWe4Fxa9tFQQBG5xSsSbMXOI8PPpoQ=
 github.com/openzipkin/zipkin-go v0.1.1/go.mod h1:NtoC/o8u3JlF1lSlyPNswIbeQH9bJTmOf0Erfk+hxe8=
 github.com/pelletier/go-toml v1.9.5 h1:4yBQzkHv+7BHq2PQUZF3Mx0IYxG7LsP222s7Agd3ve8=
 github.com/pelletier/go-toml v1.9.5/go.mod h1:u1nR/EPcESfeI/szUZKdtJ0xRNbUoANCkoOuaOx1Y+c=
 github.com/phayes/freeport v0.0.0-20180830031419-95f893ade6f2 h1:JhzVVoYvbOACxoUmOs6V/G4D5nPVUW73rKvXxP4XUJc=
 github.com/phayes/freeport v0.0.0-20180830031419-95f893ade6f2/go.mod h1:iIss55rKnNBTvrwdmkUpLnDpZoAHvWaiq5+iMmen4AE=
@@ -117,16 +115,16 @@
 github.com/quic-go/quic-go v0.41.0 h1:aD8MmHfgqTURWNJy48IYFg2OnxwHT3JL7ahGs73lb4k=
 github.com/quic-go/quic-go v0.41.0/go.mod h1:qCkNjqczPEvgsOnxZ0eCD14lv+B2LHlFAB++CNOh9hA=
 github.com/refraction-networking/utls v1.6.3 h1:MFOfRN35sSx6K5AZNIoESsBuBxS2LCgRilRIdHb6fDc=
 github.com/refraction-networking/utls v1.6.3/go.mod h1:yil9+7qSl+gBwJqztoQseO6Pr3h62pQoY1lXiNR/FPs=
 github.com/riobard/go-bloom v0.0.0-20200614022211-cdc8013cb5b3 h1:f/FNXud6gA3MNr8meMVVGxhp+QBTqY91tM8HjEuMjGg=
 github.com/riobard/go-bloom v0.0.0-20200614022211-cdc8013cb5b3/go.mod h1:HgjTstvQsPGkxUsCd2KWxErBblirPizecHcpD3ffK+s=
 github.com/russross/blackfriday v1.5.2/go.mod h1:JO/DiYxRf+HjHt06OyowR9PTA263kcR/rfWxYHBV53g=
-github.com/sagernet/sing v0.3.2 h1:CwWcxUBPkMvwgfe2/zUgY5oHG9qOL8Aob/evIFYK9jo=
-github.com/sagernet/sing v0.3.2/go.mod h1:qHySJ7u8po9DABtMYEkNBcOumx7ZZJf/fbv2sfTkNHE=
+github.com/sagernet/sing v0.3.6 h1:dsEdYLKBQlrxUfw1a92x0VdPvR1/BOxQ+HIMyaoEJsQ=
+github.com/sagernet/sing v0.3.6/go.mod h1:+60H3Cm91RnL9dpVGWDPHt0zTQImO9Vfqt9a4rSambI=
 github.com/sagernet/sing-shadowsocks v0.2.6 h1:xr7ylAS/q1cQYS8oxKKajhuQcchd5VJJ4K4UZrrpp0s=
 github.com/sagernet/sing-shadowsocks v0.2.6/go.mod h1:j2YZBIpWIuElPFL/5sJAj470bcn/3QQ5lxZUNKLDNAM=
 github.com/seiflotfy/cuckoofilter v0.0.0-20220411075957-e3b120b3f5fb h1:XfLJSPIOUX+osiMraVgIrMR27uMXnRJWGm1+GL8/63U=
 github.com/seiflotfy/cuckoofilter v0.0.0-20220411075957-e3b120b3f5fb/go.mod h1:bR6DqgcAl1zTcOX8/pE2Qkj9XO00eCNqmKb7lXP8EAg=
 github.com/sergi/go-diff v1.0.0/go.mod h1:0CfEIISq7TuYL3j771MWULgwwjU+GofnZX9QAmXWZgo=
 github.com/shurcooL/component v0.0.0-20170202220835-f88ec8f54cc4/go.mod h1:XhFIlyj5a1fBNx5aJTbKoIq0mNaPvOagO+HjB3EtxrY=
 github.com/shurcooL/events v0.0.0-20181021180414-410e4ca65f48/go.mod h1:5u70Mqkb5O5cxEA8nxTsgrgLehJeAw6Oc4Ab1c/P1HM=
@@ -151,16 +149,16 @@
 github.com/shurcooL/users v0.0.0-20180125191416-49c67e49c537/go.mod h1:QJTqeLYEDaXHZDBsXlPCDqdhQuJkuw4NOtaxYe3xii4=
 github.com/shurcooL/webdavfs v0.0.0-20170829043945-18c3829fa133/go.mod h1:hKmq5kWdCj2z2KEozexVbfEZIWiTjhE0+UjmZgPqehw=
 github.com/sourcegraph/annotate v0.0.0-20160123013949-f4cad6c6324d/go.mod h1:UdhH50NIW0fCiwBSr0co2m7BnFLdv4fQTgdqdJTHFeE=
 github.com/sourcegraph/syntaxhighlight v0.0.0-20170531221838-bd320f5d308e/go.mod h1:HuIsMU8RRBOtsCgI77wP899iHVBQpCmg4ErYMZB+2IA=
 github.com/stretchr/objx v0.1.0/go.mod h1:HFkY916IF+rwdDfMAkV7OtwuqBVzrE8GR6GFx+wExME=
 github.com/stretchr/testify v1.2.2/go.mod h1:a8OnRcib4nhh0OaRAV+Yts87kKdq0PP7pXfy6kDkUVs=
 github.com/stretchr/testify v1.6.1/go.mod h1:6Fq8oRcR53rry900zMqJjRRixrwX3KX962/h/Wwjteg=
-github.com/stretchr/testify v1.8.4 h1:CcVxjf3Q8PM0mHUKJCdn+eZZtm5yQwehR5yeSVQQcUk=
-github.com/stretchr/testify v1.8.4/go.mod h1:sz/lmYIOXD/1dqDmKjjqLyZ2RngseejIcXlSw2iwfAo=
+github.com/stretchr/testify v1.9.0 h1:HtqpIVDClZ4nwg75+f6Lvsy/wHu+3BoSGCbBAcpTsTg=
+github.com/stretchr/testify v1.9.0/go.mod h1:r2ic/lqez/lEtzL7wO/rwa5dbSLXVDPFyf8C91i36aY=
 github.com/tarm/serial v0.0.0-20180830185346-98f6abe2eb07/go.mod h1:kDXzergiv9cbyO7IOYJZWg1U88JhDg3PB6klq9Hg2pA=
 github.com/v2fly/ss-bloomring v0.0.0-20210312155135-28617310f63e h1:5QefA066A1tF8gHIiADmOVOV5LS43gt3ONnlEl3xkwI=
 github.com/v2fly/ss-bloomring v0.0.0-20210312155135-28617310f63e/go.mod h1:5t19P9LBIrNamL6AcMQOncg/r10y3Pc01AbHeMhwlpU=
 github.com/viant/assertly v0.4.8/go.mod h1:aGifi++jvCrUaklKEKT0BU95igDNaqkvz+49uaYMPRU=
 github.com/viant/toolbox v0.24.0/go.mod h1:OxMCG57V0PXuIP2HNQrtJf2CjqdmbrOx5EkMILuUhzM=
 github.com/vishvananda/netlink v1.2.1-beta.2.0.20230316163032-ced5aaba43e3 h1:tkMT5pTye+1NlKIXETU78NXw0fyjnaNHmJyyLyzw8+U=
 github.com/vishvananda/netlink v1.2.1-beta.2.0.20230316163032-ced5aaba43e3/go.mod h1:cAAsePK2e15YDAMJNyOpGYEWNe4sIghTY7gpz4cX/Ik=
@@ -177,38 +175,38 @@
 go4.org/netipx v0.0.0-20231129151722-fdeea329fbba h1:0b9z3AuHCjxk0x/opv64kcgZLBseWJUpBw5I82+2U4M=
 go4.org/netipx v0.0.0-20231129151722-fdeea329fbba/go.mod h1:PLyyIXexvUFg3Owu6p/WfdlivPbZJsZdgWZlrGope/Y=
 golang.org/x/build v0.0.0-20190111050920-041ab4dc3f9d/go.mod h1:OWs+y06UdEOHN4y+MfF/py+xQ/tYqIWW03b70/CG9Rw=
 golang.org/x/crypto v0.0.0-20181030102418-4d3f4d9ffa16/go.mod h1:6SG95UA2DQfeDnfUPMdvaQW0Q7yPrPDi9nlGo2tz2b4=
 golang.org/x/crypto v0.0.0-20190308221718-c2843e01d9a2/go.mod h1:djNgcEr1/C05ACkg1iLfiJU5Ep61QUkGW8qpdssI0+w=
 golang.org/x/crypto v0.0.0-20190313024323-a1f597ede03a/go.mod h1:djNgcEr1/C05ACkg1iLfiJU5Ep61QUkGW8qpdssI0+w=
 golang.org/x/crypto v0.0.0-20191011191535-87dc89f01550/go.mod h1:yigFU9vqHzYiE8UmvKecakEJjdnWj3jj499lnFckfCI=
-golang.org/x/crypto v0.19.0 h1:ENy+Az/9Y1vSrlrvBSyna3PITt4tiZLf7sgCjZBX7Wo=
-golang.org/x/crypto v0.19.0/go.mod h1:Iy9bg/ha4yyC70EfRS8jz+B6ybOBKMaSxLj6P6oBDfU=
+golang.org/x/crypto v0.21.0 h1:X31++rzVUdKhX5sWmSOFZxx8UW/ldWx55cbf08iNAMA=
+golang.org/x/crypto v0.21.0/go.mod h1:0BP7YvVV9gBbVKyeTG0Gyn+gZm94bibOW5BjDEYAOMs=
 golang.org/x/exp v0.0.0-20190121172915-509febef88a4/go.mod h1:CJ0aWSM057203Lf6IL+f9T1iT9GByDxfZKAQTCR3kQA=
 golang.org/x/exp v0.0.0-20240222234643-814bf88cf225 h1:LfspQV/FYTatPTr/3HzIcmiUFH7PGP+OQ6mgDYo3yuQ=
 golang.org/x/exp v0.0.0-20240222234643-814bf88cf225/go.mod h1:CxmFvTBINI24O/j8iY7H1xHzx2i4OsyguNBmN/uPtqc=
 golang.org/x/lint v0.0.0-20180702182130-06c8688daad7/go.mod h1:UVdnD1Gm6xHRNCYTkRU2/jEulfH38KcIWyp/GAMgvoE=
 golang.org/x/lint v0.0.0-20181026193005-c67002cb31c3/go.mod h1:UVdnD1Gm6xHRNCYTkRU2/jEulfH38KcIWyp/GAMgvoE=
 golang.org/x/lint v0.0.0-20190227174305-5b3e6a55c961/go.mod h1:wehouNa3lNwaWXcvxsM5YxQ5yQlVC4a0KAMCusXpPoU=
 golang.org/x/mod v0.5.1/go.mod h1:5OXOZSfqPIIbmVBIIKWRFfZjPR0E5r58TLhUjH0a2Ro=
-golang.org/x/mod v0.15.0 h1:SernR4v+D55NyBH2QiEQrlBAnj1ECL6AGrA5+dPaMY8=
-golang.org/x/mod v0.15.0/go.mod h1:hTbmBsO62+eylJbnUtE2MGJUyE7QWk4xUqPFrRgJ+7c=
+golang.org/x/mod v0.16.0 h1:QX4fJ0Rr5cPQCF7O9lh9Se4pmwfwskqZfq5moyldzic=
+golang.org/x/mod v0.16.0/go.mod h1:hTbmBsO62+eylJbnUtE2MGJUyE7QWk4xUqPFrRgJ+7c=
 golang.org/x/net v0.0.0-20180724234803-3673e40ba225/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20180826012351-8a410e7b638d/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20180906233101-161cd47e91fd/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20181029044818-c44066c5c816/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20181106065722-10aee1819953/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20190108225652-1e06a53dbb7e/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20190213061140-3a22650c66bd/go.mod h1:mL1N/T3taQHkDXs73rZJwtUhF3w3ftmwwsq0BUmARs4=
 golang.org/x/net v0.0.0-20190313220215-9f648a60d977/go.mod h1:t9HGtf8HONx5eT2rtn7q6eTqICYqUVnKs3thJo3Qplg=
 golang.org/x/net v0.0.0-20190404232315-eb5bcb51f2a3/go.mod h1:t9HGtf8HONx5eT2rtn7q6eTqICYqUVnKs3thJo3Qplg=
 golang.org/x/net v0.0.0-20190620200207-3b0461eec859/go.mod h1:z5CRVTTTmAJ677TzLLGU+0bjPO0LkuOLi4/5GtJWs/s=
 golang.org/x/net v0.0.0-20211015210444-4f30a5c0130f/go.mod h1:9nx3DQGgdP8bBQD5qxJ1jj9UTztislL4KSBs9R2vV5Y=
-golang.org/x/net v0.21.0 h1:AQyQV4dYCvJ7vGmJyKki9+PBdyvhkSd8EIx/qb0AYv4=
-golang.org/x/net v0.21.0/go.mod h1:bIjVDfnllIU7BJ2DNgfnXvpSvtn8VRwhlsaeUTyUS44=
+golang.org/x/net v0.22.0 h1:9sGLhx7iRIHEiX0oAJ3MRZMUCElJgy7Br1nO+AMN3Tc=
+golang.org/x/net v0.22.0/go.mod h1:JKghWKKOSdJwpW2GEx0Ja7fmaKnMsbu+MWVZTokSYmg=
 golang.org/x/oauth2 v0.0.0-20180821212333-d2e6202438be/go.mod h1:N/0e6XlmueqKjAGxoOufVs8QHGRruUQn6yWY3a++T0U=
 golang.org/x/oauth2 v0.0.0-20181017192945-9dcd33a902f4/go.mod h1:N/0e6XlmueqKjAGxoOufVs8QHGRruUQn6yWY3a++T0U=
 golang.org/x/oauth2 v0.0.0-20181203162652-d668ce993890/go.mod h1:N/0e6XlmueqKjAGxoOufVs8QHGRruUQn6yWY3a++T0U=
 golang.org/x/oauth2 v0.0.0-20190226205417-e64efc72b421/go.mod h1:gOpvHmFTYa4IltrdGE7lF6nIHvwfUNPOp7c8zoXwtLw=
 golang.org/x/perf v0.0.0-20180704124530-6e6d33e29852/go.mod h1:JLpeXjPJfIyPr5TlbXLkXWLhP8nz10XfvxElABhCtcw=
 golang.org/x/sync v0.0.0-20180314180146-1d60e4601c6f/go.mod h1:RxMgew5VJxzue5/jJTE5uejpjVlOe/izrB70Jof72aM=
 golang.org/x/sync v0.0.0-20181108010431-42b317875d0f/go.mod h1:RxMgew5VJxzue5/jJTE5uejpjVlOe/izrB70Jof72aM=
@@ -226,16 +224,16 @@
 golang.org/x/sys v0.0.0-20190412213103-97732733099d/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20200217220822-9197077df867/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20201119102817-f84b799fce68/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20210423082822-04245dca01da/go.mod h1:h1NjWce9XRLGQEsW7wpKNCjG9DtNlClVuFLEZdDNbEs=
 golang.org/x/sys v0.0.0-20211019181941-9d821ace8654/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.0.0-20220804214406-8e32c043e418/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
 golang.org/x/sys v0.5.0/go.mod h1:oPkhp1MJrh7nUepCBck5+mAzfO9JrbApNNgaTdGDITg=
-golang.org/x/sys v0.17.0 h1:25cE3gD+tdBA7lp7QfhuV+rJiE9YXTcS3VG1SqssI/Y=
-golang.org/x/sys v0.17.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
+golang.org/x/sys v0.18.0 h1:DBdB3niSjOA/O0blCZBqDefyWNYveAYMNF1Wum0DYQ4=
+golang.org/x/sys v0.18.0/go.mod h1:/VUhepiaJMQUp4+oa/7Zr1D23ma6VTLIYjOOTFZPUcA=
 golang.org/x/term v0.0.0-20201126162022-7de9c90e9dd1/go.mod h1:bj7SfCRtBDWHUb9snDiAeCFNEtKQo2Wmx5Cou7ajbmo=
 golang.org/x/text v0.3.0/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.1-0.20180807135948-17ff2d5776d2/go.mod h1:NqM8EUOU14njkJ3fqMW+pc6Ldnwhi/IjpwHt7yyuwOQ=
 golang.org/x/text v0.3.6/go.mod h1:5Zoc/QRtKVWzQhOtBMvqHzDpF6irO9z98xDceosuGiQ=
 golang.org/x/text v0.3.7/go.mod h1:u+2+/6zg+i71rQMx5EYifcz6MCKuco9NR6JIITiCfzQ=
 golang.org/x/text v0.14.0 h1:ScX5w1eTa3QqT8oi6+ziP7dTV1S2+ALU0bI+0zXKWiQ=
 golang.org/x/text v0.14.0/go.mod h1:18ZOQIKpY8NJVqYksKHtTdi31H5itFRjB5/qKTNYzSU=
@@ -246,19 +244,18 @@
 golang.org/x/tools v0.0.0-20180828015842-6cd1fcedba52/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20180917221912-90fa682c2a6e/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20181030000716-a0a13e073c7b/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20190114222345-bf090417da8b/go.mod h1:n7NCudcB/nEzxVGmLbDWY5pfWTLqBcC2KZ6jyYvM4mQ=
 golang.org/x/tools v0.0.0-20190226205152-f727befe758c/go.mod h1:9Yl7xja0Znq3iFh3HoIrodX9oNMXvdceNzlUR8zjMvY=
 golang.org/x/tools v0.0.0-20191119224855-298f0cb1881e/go.mod h1:b+2E5dAYhXwXZwtnZ6UAqBI28+e2cm9otk0dWdXHAEo=
 golang.org/x/tools v0.1.8/go.mod h1:nABZi5QlRsZVlzPpHl034qft6wpY4eDcsTt5AaioBiU=
-golang.org/x/tools v0.18.0 h1:k8NLag8AGHnn+PHbl7g43CtqZAwG60vZkLqgyZgIHgQ=
-golang.org/x/tools v0.18.0/go.mod h1:GL7B4CwcLLeo59yx/9UWWuNOW1n3VZ4f5axWfML7Lcg=
+golang.org/x/tools v0.19.0 h1:tfGCXNR1OsFG+sVdLAitlpjAvD/I6dHDKnYrpEZUHkw=
+golang.org/x/tools v0.19.0/go.mod h1:qoJWxmGSIBmAeriMx19ogtrEPrGtDbPK634QFIcLAhc=
 golang.org/x/xerrors v0.0.0-20190717185122-a985d3407aa7/go.mod h1:I/5z698sn9Ka8TeJc9MKroUUfqBBauWjQqLJ2OPfmY0=
 golang.org/x/xerrors v0.0.0-20191011141410-1b5146add898/go.mod h1:I/5z698sn9Ka8TeJc9MKroUUfqBBauWjQqLJ2OPfmY0=
-golang.org/x/xerrors v0.0.0-20191204190536-9bdfabe68543/go.mod h1:I/5z698sn9Ka8TeJc9MKroUUfqBBauWjQqLJ2OPfmY0=
 golang.org/x/xerrors v0.0.0-20200804184101-5ec99f83aff1/go.mod h1:I/5z698sn9Ka8TeJc9MKroUUfqBBauWjQqLJ2OPfmY0=
 golang.zx2c4.com/wintun v0.0.0-20230126152724-0fa3db229ce2 h1:B82qJJgjvYKsXS9jeunTOisW56dUokqW/FOteYJJ/yg=
 golang.zx2c4.com/wintun v0.0.0-20230126152724-0fa3db229ce2/go.mod h1:deeaetjYA+DHMHg+sMSMI58GrEteJUUzzw7en6TJQcI=
 golang.zx2c4.com/wireguard v0.0.0-20231211153847-12269c276173 h1:/jFs0duh4rdb8uIfPMv78iAJGcPKDeqAFnaLBropIC4=
 golang.zx2c4.com/wireguard v0.0.0-20231211153847-12269c276173/go.mod h1:tkCQ4FQXmpAgYVh++1cq16/dH4QJtmvpRv19DWGAHSA=
 google.golang.org/api v0.0.0-20180910000450-7ca32eb868bf/go.mod h1:4mhQ8q/RsB7i+udVvVy5NUi08OU8ZlA0gRVgrF7VFY0=
 google.golang.org/api v0.0.0-20181030000543-1d582fd0359e/go.mod h1:4mhQ8q/RsB7i+udVvVy5NUi08OU8ZlA0gRVgrF7VFY0=
@@ -268,26 +265,24 @@
 google.golang.org/appengine v1.3.0/go.mod h1:xpcJRLb0r/rnEns0DIKYYv+WjYCduHsrkT7/EB5XEv4=
 google.golang.org/appengine v1.4.0/go.mod h1:xpcJRLb0r/rnEns0DIKYYv+WjYCduHsrkT7/EB5XEv4=
 google.golang.org/genproto v0.0.0-20180817151627-c66870c02cf8/go.mod h1:JiN7NxoALGmiZfu7CAH4rXhgtRTLTxftemlI0sWmxmc=
 google.golang.org/genproto v0.0.0-20180831171423-11092d34479b/go.mod h1:JiN7NxoALGmiZfu7CAH4rXhgtRTLTxftemlI0sWmxmc=
 google.golang.org/genproto v0.0.0-20181029155118-b69ba1387ce2/go.mod h1:JiN7NxoALGmiZfu7CAH4rXhgtRTLTxftemlI0sWmxmc=
 google.golang.org/genproto v0.0.0-20181202183823-bd91e49a0898/go.mod h1:7Ep/1NZk928CDR8SjdVbjWNpdIf6nzjE3BTgJDr2Atg=
 google.golang.org/genproto v0.0.0-20190306203927-b5d61aea6440/go.mod h1:VzzqZJRnGkLBvHegQrXjBqPurQTc5/KpmUdxsrq26oE=
-google.golang.org/genproto/googleapis/rpc v0.0.0-20240221002015-b0ce06bbee7c h1:NUsgEN92SQQqzfA+YtqYNqYmB3DMMYLlIwUZAQFVFbo=
-google.golang.org/genproto/googleapis/rpc v0.0.0-20240221002015-b0ce06bbee7c/go.mod h1:H4O17MA/PE9BsGx3w+a+W2VOLLD1Qf7oJneAoU6WktY=
+google.golang.org/genproto/googleapis/rpc v0.0.0-20240308144416-29370a3891b7 h1:em/y72n4XlYRtayY/cVj6pnVzHa//BDA1BdoO+z9mdE=
+google.golang.org/genproto/googleapis/rpc v0.0.0-20240308144416-29370a3891b7/go.mod h1:UCOku4NytXMJuLQE5VuqA5lX3PcHCBo8pxNyvkf4xBs=
 google.golang.org/grpc v1.14.0/go.mod h1:yo6s7OP7yaDglbqo1J04qKzAhqBH6lvTonzMVmEdcZw=
 google.golang.org/grpc v1.16.0/go.mod h1:0JHn/cJsOMiMfNA9+DeHDlAU7KAAB5GDlYFpa9MZMio=
 google.golang.org/grpc v1.17.0/go.mod h1:6QZJwpn2B+Zp71q/5VxRsJ6NXXVCE5NRUHRo+f3cWCs=
 google.golang.org/grpc v1.19.0/go.mod h1:mqu4LbDTu4XGKhr4mRzUsmM4RtVoemTSY81AxZiDr8c=
-google.golang.org/grpc v1.62.0 h1:HQKZ/fa1bXkX1oFOvSjmZEUL8wLSaZTjCcLAlmZRtdk=
-google.golang.org/grpc v1.62.0/go.mod h1:IWTG0VlJLCh1SkC58F7np9ka9mx/WNkjl4PGJaiq+QE=
-google.golang.org/protobuf v1.26.0-rc.1/go.mod h1:jlhhOSvTdKEhbULTjvd4ARK9grFBp09yW+WbY/TyQbw=
-google.golang.org/protobuf v1.26.0/go.mod h1:9q0QmTI4eRPtz6boOQmLYwt+qCgq0jsYwAQnmE0givc=
-google.golang.org/protobuf v1.32.0 h1:pPC6BG5ex8PDFnkbrGU3EixyhKcQ2aDuBS36lqK/C7I=
-google.golang.org/protobuf v1.32.0/go.mod h1:c6P6GXX6sHbq/GpV6MGZEdwhWPcYBgnhAHhKbcUYpos=
+google.golang.org/grpc v1.62.1 h1:B4n+nfKzOICUXMgyrNd19h/I9oH0L1pizfk1d4zSgTk=
+google.golang.org/grpc v1.62.1/go.mod h1:IWTG0VlJLCh1SkC58F7np9ka9mx/WNkjl4PGJaiq+QE=
+google.golang.org/protobuf v1.33.0 h1:uNO2rsAINq/JlFpSdYEKIZ0uKD/R9cpdv0T+yoGwGmI=
+google.golang.org/protobuf v1.33.0/go.mod h1:c6P6GXX6sHbq/GpV6MGZEdwhWPcYBgnhAHhKbcUYpos=
 gopkg.in/check.v1 v0.0.0-20161208181325-20d25e280405/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/check.v1 v1.0.0-20180628173108-788fd7840127 h1:qIbj1fsPNlZgppZ+VLlY7N33q108Sa+fhmuc+sWQYwY=
 gopkg.in/check.v1 v1.0.0-20180628173108-788fd7840127/go.mod h1:Co6ibVJAznAaIkqp8huTwlJQCZ016jof/cbN4VW5Yz0=
 gopkg.in/inf.v0 v0.9.1/go.mod h1:cWUDdTG/fYaXco+Dcufb5Vnc6Gp2YChqWtbxRZE0mXw=
 gopkg.in/yaml.v2 v2.2.1/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
 gopkg.in/yaml.v2 v2.2.2/go.mod h1:hI93XBmqTisBFMUTm0b8Fm+jr3Dg1NNxqwp+5A1VGuI=
 gopkg.in/yaml.v2 v2.4.0 h1:D8xgwECY7CYvx+Y2n4sBz93Jn9JRvxdiyyo8CTfuKaY=
```

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/api.go` & `Xray-core-1.8.9/xray-go/infra/conf/api.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/blackhole.go` & `Xray-core-1.8.9/xray-go/infra/conf/blackhole.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/blackhole_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/blackhole_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/cfgcommon/duration/duration.go` & `Xray-core-1.8.9/xray-go/infra/conf/cfgcommon/duration/duration.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/cfgcommon/duration/duration_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/cfgcommon/duration/duration_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/common.go` & `Xray-core-1.8.9/xray-go/infra/conf/common.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/common_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/common_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/dns.go` & `Xray-core-1.8.9/xray-go/infra/conf/dns.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/dns_proxy.go` & `Xray-core-1.8.9/xray-go/infra/conf/dns_proxy.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/dns_proxy_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/dns_proxy_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/dns_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/dns_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/dokodemo.go` & `Xray-core-1.8.9/xray-go/infra/conf/dokodemo.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/dokodemo_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/dokodemo_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/fakedns.go` & `Xray-core-1.8.9/xray-go/infra/conf/fakedns.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/freedom.go` & `Xray-core-1.8.9/xray-go/infra/conf/freedom.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/freedom_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/freedom_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/general_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/general_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/grpc.go` & `Xray-core-1.8.9/xray-go/infra/conf/grpc.go`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import (
 	"github.com/xtls/xray-core/transport/internet/grpc"
 	"google.golang.org/protobuf/proto"
 )
 
 type GRPCConfig struct {
-	ServiceName         string `json:"serviceName" `
+	Authority           string `json:"authority"`
+	ServiceName         string `json:"serviceName"`
 	MultiMode           bool   `json:"multiMode"`
 	IdleTimeout         int32  `json:"idle_timeout"`
 	HealthCheckTimeout  int32  `json:"health_check_timeout"`
 	PermitWithoutStream bool   `json:"permit_without_stream"`
 	InitialWindowsSize  int32  `json:"initial_windows_size"`
 	UserAgent           string `json:"user_agent"`
 }
@@ -24,14 +25,15 @@
 	}
 	if g.InitialWindowsSize < 0 {
 		// default window size of gRPC-go
 		g.InitialWindowsSize = 0
 	}
 
 	return &grpc.Config{
+		Authority:           g.Authority,
 		ServiceName:         g.ServiceName,
 		MultiMode:           g.MultiMode,
 		IdleTimeout:         g.IdleTimeout,
 		HealthCheckTimeout:  g.HealthCheckTimeout,
 		PermitWithoutStream: g.PermitWithoutStream,
 		InitialWindowsSize:  g.InitialWindowsSize,
 		UserAgent:           g.UserAgent,
```

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/http.go` & `Xray-core-1.8.9/xray-go/infra/conf/http.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/http_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/http_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/json/reader.go` & `Xray-core-1.8.9/xray-go/infra/conf/json/reader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/json/reader_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/json/reader_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/lint.go` & `Xray-core-1.8.9/xray-go/infra/conf/lint.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/loader.go` & `Xray-core-1.8.9/xray-go/infra/conf/loader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/log.go` & `Xray-core-1.8.9/xray-go/infra/conf/log.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/observatory.go` & `Xray-core-1.8.9/xray-go/infra/conf/observatory.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/policy.go` & `Xray-core-1.8.9/xray-go/infra/conf/policy.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/policy_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/policy_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/reverse.go` & `Xray-core-1.8.9/xray-go/infra/conf/reverse.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/reverse_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/reverse_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/router.go` & `Xray-core-1.8.9/xray-go/infra/conf/router.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/router_strategy.go` & `Xray-core-1.8.9/xray-go/infra/conf/router_strategy.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/router_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/router_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/serial/builder.go` & `Xray-core-1.8.9/xray-go/infra/conf/serial/builder.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/serial/loader.go` & `Xray-core-1.8.9/xray-go/infra/conf/serial/loader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/serial/loader_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/serial/loader_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/shadowsocks.go` & `Xray-core-1.8.9/xray-go/infra/conf/shadowsocks.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/shadowsocks_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/shadowsocks_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/socks.go` & `Xray-core-1.8.9/xray-go/infra/conf/socks.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/socks_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/socks_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/transport.go` & `Xray-core-1.8.9/xray-go/infra/conf/transport.go`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import (
 	"github.com/xtls/xray-core/common/serial"
 	"github.com/xtls/xray-core/transport/global"
 	"github.com/xtls/xray-core/transport/internet"
 )
 
 type TransportConfig struct {
-	TCPConfig  *TCPConfig          `json:"tcpSettings"`
-	KCPConfig  *KCPConfig          `json:"kcpSettings"`
-	WSConfig   *WebSocketConfig    `json:"wsSettings"`
-	HTTPConfig *HTTPConfig         `json:"httpSettings"`
-	DSConfig   *DomainSocketConfig `json:"dsSettings"`
-	QUICConfig *QUICConfig         `json:"quicSettings"`
-	GRPCConfig *GRPCConfig         `json:"grpcSettings"`
-	GUNConfig  *GRPCConfig         `json:"gunSettings"`
+	TCPConfig         *TCPConfig          `json:"tcpSettings"`
+	KCPConfig         *KCPConfig          `json:"kcpSettings"`
+	WSConfig          *WebSocketConfig    `json:"wsSettings"`
+	HTTPConfig        *HTTPConfig         `json:"httpSettings"`
+	DSConfig          *DomainSocketConfig `json:"dsSettings"`
+	QUICConfig        *QUICConfig         `json:"quicSettings"`
+	GRPCConfig        *GRPCConfig         `json:"grpcSettings"`
+	GUNConfig         *GRPCConfig         `json:"gunSettings"`
+	HTTPUPGRADEConfig *HttpUpgradeConfig  `json:"httpupgradeSettings"`
 }
 
 // Build implements Buildable.
 func (c *TransportConfig) Build() (*global.Config, error) {
 	config := new(global.Config)
 
 	if c.TCPConfig != nil {
@@ -97,9 +98,20 @@
 		}
 		config.TransportSettings = append(config.TransportSettings, &internet.TransportConfig{
 			ProtocolName: "grpc",
 			Settings:     serial.ToTypedMessage(gs),
 		})
 	}
 
+	if c.HTTPUPGRADEConfig != nil {
+		hs, err := c.HTTPUPGRADEConfig.Build()
+		if err != nil {
+			return nil, newError("failed to build HttpUpgrade config").Base(err)
+		}
+		config.TransportSettings = append(config.TransportSettings, &internet.TransportConfig{
+			ProtocolName: "httpupgrade",
+			Settings:     serial.ToTypedMessage(hs),
+		})
+	}
+
 	return config, nil
 }
```

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/transport_authenticators.go` & `Xray-core-1.8.9/xray-go/infra/conf/transport_authenticators.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/transport_internet.go` & `Xray-core-1.8.9/xray-go/infra/conf/transport_internet.go`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 	"github.com/xtls/xray-core/common/platform/filesystem"
 	"github.com/xtls/xray-core/common/protocol"
 	"github.com/xtls/xray-core/common/serial"
 	"github.com/xtls/xray-core/transport/internet"
 	"github.com/xtls/xray-core/transport/internet/domainsocket"
 	httpheader "github.com/xtls/xray-core/transport/internet/headers/http"
 	"github.com/xtls/xray-core/transport/internet/http"
+	"github.com/xtls/xray-core/transport/internet/httpupgrade"
 	"github.com/xtls/xray-core/transport/internet/kcp"
 	"github.com/xtls/xray-core/transport/internet/quic"
 	"github.com/xtls/xray-core/transport/internet/reality"
 	"github.com/xtls/xray-core/transport/internet/tcp"
 	"github.com/xtls/xray-core/transport/internet/tls"
 	"github.com/xtls/xray-core/transport/internet/websocket"
 	"google.golang.org/protobuf/proto"
@@ -177,14 +178,32 @@
 	}
 	if c.AcceptProxyProtocol {
 		config.AcceptProxyProtocol = c.AcceptProxyProtocol
 	}
 	return config, nil
 }
 
+type HttpUpgradeConfig struct {
+	Path                string `json:"path"`
+	Host                string `json:"host"`
+	AcceptProxyProtocol bool   `json:"acceptProxyProtocol"`
+}
+
+// Build implements Buildable.
+func (c *HttpUpgradeConfig) Build() (proto.Message, error) {
+	config := &httpupgrade.Config{
+		Path: c.Path,
+		Host: c.Host,
+	}
+	if c.AcceptProxyProtocol {
+		config.AcceptProxyProtocol = c.AcceptProxyProtocol
+	}
+	return config, nil
+}
+
 type HTTPConfig struct {
 	Host               *StringList            `json:"host"`
 	Path               string                 `json:"path"`
 	ReadIdleTimeout    int32                  `json:"read_idle_timeout"`
 	HealthCheckTimeout int32                  `json:"health_check_timeout"`
 	Method             string                 `json:"method"`
 	Headers            map[string]*StringList `json:"headers"`
@@ -602,14 +621,16 @@
 		return "http", nil
 	case "ds", "domainsocket":
 		return "domainsocket", nil
 	case "quic":
 		return "quic", nil
 	case "grpc", "gun":
 		return "grpc", nil
+	case "httpupgrade":
+		return "httpupgrade", nil
 	default:
 		return "", newError("Config: unknown transport protocol: ", p)
 	}
 }
 
 type SocketConfig struct {
 	Mark                 int32       `json:"mark"`
@@ -702,27 +723,28 @@
 		V6Only:               c.V6only,
 		Interface:            c.Interface,
 		TcpMptcp:             c.TcpMptcp,
 	}, nil
 }
 
 type StreamConfig struct {
-	Network         *TransportProtocol  `json:"network"`
-	Security        string              `json:"security"`
-	TLSSettings     *TLSConfig          `json:"tlsSettings"`
-	REALITYSettings *REALITYConfig      `json:"realitySettings"`
-	TCPSettings     *TCPConfig          `json:"tcpSettings"`
-	KCPSettings     *KCPConfig          `json:"kcpSettings"`
-	WSSettings      *WebSocketConfig    `json:"wsSettings"`
-	HTTPSettings    *HTTPConfig         `json:"httpSettings"`
-	DSSettings      *DomainSocketConfig `json:"dsSettings"`
-	QUICSettings    *QUICConfig         `json:"quicSettings"`
-	SocketSettings  *SocketConfig       `json:"sockopt"`
-	GRPCConfig      *GRPCConfig         `json:"grpcSettings"`
-	GUNConfig       *GRPCConfig         `json:"gunSettings"`
+	Network             *TransportProtocol  `json:"network"`
+	Security            string              `json:"security"`
+	TLSSettings         *TLSConfig          `json:"tlsSettings"`
+	REALITYSettings     *REALITYConfig      `json:"realitySettings"`
+	TCPSettings         *TCPConfig          `json:"tcpSettings"`
+	KCPSettings         *KCPConfig          `json:"kcpSettings"`
+	WSSettings          *WebSocketConfig    `json:"wsSettings"`
+	HTTPSettings        *HTTPConfig         `json:"httpSettings"`
+	DSSettings          *DomainSocketConfig `json:"dsSettings"`
+	QUICSettings        *QUICConfig         `json:"quicSettings"`
+	SocketSettings      *SocketConfig       `json:"sockopt"`
+	GRPCConfig          *GRPCConfig         `json:"grpcSettings"`
+	GUNConfig           *GRPCConfig         `json:"gunSettings"`
+	HTTPUPGRADESettings *HttpUpgradeConfig  `json:"httpupgradeSettings"`
 }
 
 // Build implements Buildable.
 func (c *StreamConfig) Build() (*internet.StreamConfig, error) {
 	config := &internet.StreamConfig{
 		ProtocolName: "tcp",
 	}
@@ -835,14 +857,24 @@
 			return nil, newError("Failed to build gRPC config.").Base(err)
 		}
 		config.TransportSettings = append(config.TransportSettings, &internet.TransportConfig{
 			ProtocolName: "grpc",
 			Settings:     serial.ToTypedMessage(gs),
 		})
 	}
+	if c.HTTPUPGRADESettings != nil {
+		hs, err := c.HTTPUPGRADESettings.Build()
+		if err != nil {
+			return nil, newError("Failed to build HttpUpgrade config.").Base(err)
+		}
+		config.TransportSettings = append(config.TransportSettings, &internet.TransportConfig{
+			ProtocolName: "httpupgrade",
+			Settings:     serial.ToTypedMessage(hs),
+		})
+	}
 	if c.SocketSettings != nil {
 		ss, err := c.SocketSettings.Build()
 		if err != nil {
 			return nil, newError("Failed to build sockopt").Base(err)
 		}
 		config.SocketSettings = ss
 	}
```

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/transport_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/transport_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/trojan.go` & `Xray-core-1.8.9/xray-go/infra/conf/trojan.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/vless.go` & `Xray-core-1.8.9/xray-go/infra/conf/vless.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/vless_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/vless_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/vmess.go` & `Xray-core-1.8.9/xray-go/infra/conf/vmess.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/vmess_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/vmess_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/wireguard.go` & `Xray-core-1.8.9/xray-go/infra/conf/wireguard.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/wireguard_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/wireguard_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/xray.go` & `Xray-core-1.8.9/xray-go/infra/conf/xray.go`

 * *Files 2% similar despite different names*

```diff
@@ -540,14 +540,17 @@
 	}
 	if s.HTTPSettings == nil {
 		s.HTTPSettings = t.HTTPConfig
 	}
 	if s.DSSettings == nil {
 		s.DSSettings = t.DSConfig
 	}
+	if s.HTTPUPGRADESettings == nil {
+		s.HTTPUPGRADESettings = t.HTTPUPGRADEConfig
+	}
 }
 
 // Build implements Buildable.
 func (c *Config) Build() (*core.Config, error) {
 	if err := PostProcessConfigureFile(c); err != nil {
 		return nil, err
 	}
```

### Comparing `Xray-core-1.8.8/xray-go/infra/conf/xray_test.go` & `Xray-core-1.8.9/xray-go/infra/conf/xray_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/vformat/main.go` & `Xray-core-1.8.9/xray-go/infra/vformat/main.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/infra/vprotogen/main.go` & `Xray-core-1.8.9/xray-go/infra/vprotogen/main.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/api.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/api.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/balancer_info.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/balancer_info.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/balancer_override.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/balancer_override.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/inbounds_add.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/inbounds_add.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/inbounds_remove.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/inbounds_remove.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/logger_restart.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/logger_restart.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/outbounds_add.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/outbounds_add.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/outbounds_remove.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/outbounds_remove.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/shared.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/shared.go`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 package api
 
 import (
 	"bytes"
 	"context"
 	"fmt"
-	"google.golang.org/protobuf/encoding/protojson"
 	"io"
 	"net/http"
 	"net/url"
 	"os"
 	"reflect"
 	"strings"
 	"time"
 
+	"google.golang.org/grpc/credentials/insecure"
+	"google.golang.org/protobuf/encoding/protojson"
+
 	"github.com/xtls/xray-core/common/buf"
 	"github.com/xtls/xray-core/main/commands/base"
 	"google.golang.org/grpc"
 	"google.golang.org/protobuf/proto"
 )
 
 type serviceHandler func(ctx context.Context, conn *grpc.ClientConn, cmd *base.Command, args []string) string
@@ -47,15 +49,15 @@
 		conn.Close()
 	}
 	return
 }
 
 func dialAPIServer() (conn *grpc.ClientConn, ctx context.Context, close func()) {
 	ctx, cancel := context.WithTimeout(context.Background(), time.Duration(apiTimeout)*time.Second)
-	conn, err := grpc.DialContext(ctx, apiServerAddrPtr, grpc.WithInsecure(), grpc.WithBlock())
+	conn, err := grpc.DialContext(ctx, apiServerAddrPtr, grpc.WithTransportCredentials(insecure.NewCredentials()), grpc.WithBlock())
 	if err != nil {
 		base.Fatalf("failed to dial %s", apiServerAddrPtr)
 	}
 	close = func() {
 		cancel()
 		conn.Close()
 	}
```

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/stats_get.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/stats_get.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/stats_query.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/stats_query.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/api/stats_sys.go` & `Xray-core-1.8.9/xray-go/main/commands/all/api/stats_sys.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/convert.go` & `Xray-core-1.8.9/xray-go/main/commands/all/convert.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/curve25519.go` & `Xray-core-1.8.9/xray-go/main/commands/all/curve25519.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/tls/cert.go` & `Xray-core-1.8.9/xray-go/main/commands/all/tls/cert.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/tls/certchainhash.go` & `Xray-core-1.8.9/xray-go/main/commands/all/tls/certchainhash.go`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 package tls
 
 import (
 	"flag"
 	"fmt"
-	"io/ioutil"
+	"os"
 
 	"github.com/xtls/xray-core/main/commands/base"
 	"github.com/xtls/xray-core/transport/internet/tls"
 )
 
 var cmdCertChainHash = &base.Command{
 	UsageLine: "{{.Exec}} certChainHash",
@@ -26,16 +26,15 @@
 
 func executeCertChainHash(cmd *base.Command, args []string) {
 	fs := flag.NewFlagSet("certChainHash", flag.ContinueOnError)
 	if err := fs.Parse(args); err != nil {
 		fmt.Println(err)
 		return
 	}
-	certContent, err := ioutil.ReadFile(*input)
+	certContent, err := os.ReadFile(*input)
 	if err != nil {
 		fmt.Println(err)
 		return
 	}
 	certChainHashB64 := tls.CalculatePEMCertChainSHA256Hash(certContent)
 	fmt.Println(certChainHashB64)
-	return
 }
```

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/tls/ping.go` & `Xray-core-1.8.9/xray-go/main/commands/all/tls/ping.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/uuid.go` & `Xray-core-1.8.9/xray-go/main/commands/all/uuid.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/wg.go` & `Xray-core-1.8.9/xray-go/main/commands/all/wg.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/all/x25519.go` & `Xray-core-1.8.9/xray-go/main/commands/all/x25519.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/base/command.go` & `Xray-core-1.8.9/xray-go/main/commands/base/command.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/base/execute.go` & `Xray-core-1.8.9/xray-go/main/commands/base/execute.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/commands/base/help.go` & `Xray-core-1.8.9/xray-go/main/commands/base/help.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/confloader/confloader.go` & `Xray-core-1.8.9/xray-go/main/confloader/confloader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/confloader/external/external.go` & `Xray-core-1.8.9/xray-go/main/confloader/external/external.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/distro/all/all.go` & `Xray-core-1.8.9/xray-go/main/distro/all/all.go`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 	_ "github.com/xtls/xray-core/proxy/vmess/outbound"
 	_ "github.com/xtls/xray-core/proxy/wireguard"
 
 	// Transports
 	_ "github.com/xtls/xray-core/transport/internet/domainsocket"
 	_ "github.com/xtls/xray-core/transport/internet/grpc"
 	_ "github.com/xtls/xray-core/transport/internet/http"
+	_ "github.com/xtls/xray-core/transport/internet/httpupgrade"
 	_ "github.com/xtls/xray-core/transport/internet/kcp"
 	_ "github.com/xtls/xray-core/transport/internet/quic"
 	_ "github.com/xtls/xray-core/transport/internet/reality"
 	_ "github.com/xtls/xray-core/transport/internet/tcp"
 	_ "github.com/xtls/xray-core/transport/internet/tls"
 	_ "github.com/xtls/xray-core/transport/internet/udp"
 	_ "github.com/xtls/xray-core/transport/internet/websocket"
```

### Comparing `Xray-core-1.8.8/xray-go/main/json/json.go` & `Xray-core-1.8.9/xray-go/main/json/json.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/main.go` & `Xray-core-1.8.9/xray-go/main/main.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/run.go` & `Xray-core-1.8.9/xray-go/main/run.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/toml/toml.go` & `Xray-core-1.8.9/xray-go/main/toml/toml.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/main/yaml/yaml.go` & `Xray-core-1.8.9/xray-go/main/yaml/yaml.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/blackhole/blackhole.go` & `Xray-core-1.8.9/xray-go/proxy/blackhole/blackhole.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/blackhole/blackhole_test.go` & `Xray-core-1.8.9/xray-go/proxy/blackhole/blackhole_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/blackhole/config.go` & `Xray-core-1.8.9/xray-go/proxy/blackhole/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/blackhole/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/blackhole/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/blackhole/config_test.go` & `Xray-core-1.8.9/xray-go/proxy/blackhole/config_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/dns/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/dns/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/dns/dns.go` & `Xray-core-1.8.9/xray-go/proxy/dns/dns.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/dns/dns_test.go` & `Xray-core-1.8.9/xray-go/proxy/dns/dns_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/dokodemo/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/dokodemo/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/dokodemo/config.proto` & `Xray-core-1.8.9/xray-go/proxy/dokodemo/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/dokodemo/dokodemo.go` & `Xray-core-1.8.9/xray-go/proxy/dokodemo/dokodemo.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/dokodemo/fakeudp_linux.go` & `Xray-core-1.8.9/xray-go/proxy/dokodemo/fakeudp_linux.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/freedom/config.go` & `Xray-core-1.8.9/xray-go/proxy/freedom/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/freedom/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/freedom/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/freedom/config.proto` & `Xray-core-1.8.9/xray-go/proxy/freedom/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/freedom/freedom.go` & `Xray-core-1.8.9/xray-go/proxy/freedom/freedom.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/http/client.go` & `Xray-core-1.8.9/xray-go/proxy/http/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/http/config.go` & `Xray-core-1.8.9/xray-go/proxy/http/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/http/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/http/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/http/config.proto` & `Xray-core-1.8.9/xray-go/proxy/http/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/http/server.go` & `Xray-core-1.8.9/xray-go/proxy/http/server.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/loopback/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/loopback/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/loopback/loopback.go` & `Xray-core-1.8.9/xray-go/proxy/loopback/loopback.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/proxy.go` & `Xray-core-1.8.9/xray-go/proxy/proxy.go`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 	"io"
 	"math/big"
 	"runtime"
 	"strconv"
 	"time"
 
 	"github.com/pires/go-proxyproto"
+	"github.com/xtls/xray-core/app/dispatcher"
 	"github.com/xtls/xray-core/common/buf"
 	"github.com/xtls/xray-core/common/errors"
 	"github.com/xtls/xray-core/common/net"
 	"github.com/xtls/xray-core/common/protocol"
 	"github.com/xtls/xray-core/common/session"
 	"github.com/xtls/xray-core/common/signal"
 	"github.com/xtls/xray-core/features/routing"
@@ -474,22 +475,26 @@
 	writerConn, _, writeCounter := UnwrapRawConn(writerConn)
 	reader := buf.NewReader(readerConn)
 	if inbound := session.InboundFromContext(ctx); inbound != nil {
 		if tc, ok := writerConn.(*net.TCPConn); ok && readerConn != nil && writerConn != nil && (runtime.GOOS == "linux" || runtime.GOOS == "android") {
 			for inbound.CanSpliceCopy != 3 {
 				if inbound.CanSpliceCopy == 1 {
 					newError("CopyRawConn splice").WriteToLog(session.ExportIDToError(ctx))
+					statWriter, _ := writer.(*dispatcher.SizeStatWriter)
 					//runtime.Gosched() // necessary
 					time.Sleep(time.Millisecond) // without this, there will be a rare ssl error for freedom splice
 					w, err := tc.ReadFrom(readerConn)
 					if readCounter != nil {
-						readCounter.Add(w)
+						readCounter.Add(w) // outbound stats
 					}
 					if writeCounter != nil {
-						writeCounter.Add(w)
+						writeCounter.Add(w) // inbound stats
+					}
+					if statWriter != nil {
+						statWriter.Counter.Add(w) // user stats
 					}
 					if err != nil && errors.Cause(err) != io.EOF {
 						return err
 					}
 					return nil
 				}
 				buffer, err := reader.ReadMultiBuffer()
```

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/client.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/config.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/config.proto` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/config_test.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/config_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/protocol.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/protocol.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/protocol_test.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/protocol_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/server.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/server.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks/validator.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks/validator.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/config.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/config.proto` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/inbound.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/inbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/inbound_multi.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/inbound_multi.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/inbound_relay.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/inbound_relay.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/shadowsocks_2022/outbound.go` & `Xray-core-1.8.9/xray-go/proxy/shadowsocks_2022/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/socks/client.go` & `Xray-core-1.8.9/xray-go/proxy/socks/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/socks/config.go` & `Xray-core-1.8.9/xray-go/proxy/socks/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/socks/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/socks/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/socks/config.proto` & `Xray-core-1.8.9/xray-go/proxy/socks/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/socks/protocol.go` & `Xray-core-1.8.9/xray-go/proxy/socks/protocol.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/socks/protocol_test.go` & `Xray-core-1.8.9/xray-go/proxy/socks/protocol_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/socks/server.go` & `Xray-core-1.8.9/xray-go/proxy/socks/server.go`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 		port:         inbound.Gateway.Port,
 		localAddress: net.IPAddress(conn.LocalAddr().(*net.TCPAddr).IP),
 	}
 
 	reader := &buf.BufferedReader{Reader: buf.NewReader(conn)}
 	request, err := svrSession.Handshake(reader, conn)
 	if err != nil {
-		if inbound != nil && inbound.Source.IsValid() {
+		if inbound.Source.IsValid() {
 			log.Record(&log.AccessMessage{
 				From:   inbound.Source,
 				To:     "",
 				Status: log.AccessRejected,
 				Reason: err,
 			})
 		}
@@ -118,15 +118,15 @@
 	if err := conn.SetReadDeadline(time.Time{}); err != nil {
 		newError("failed to clear deadline").Base(err).WriteToLog(session.ExportIDToError(ctx))
 	}
 
 	if request.Command == protocol.RequestCommandTCP {
 		dest := request.Destination()
 		newError("TCP Connect request to ", dest).WriteToLog(session.ExportIDToError(ctx))
-		if inbound != nil && inbound.Source.IsValid() {
+		if inbound.Source.IsValid() {
 			ctx = log.ContextWithAccessMessage(ctx, &log.AccessMessage{
 				From:   inbound.Source,
 				To:     dest,
 				Status: log.AccessAccepted,
 				Reason: "",
 			})
 		}
```

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/client.go` & `Xray-core-1.8.9/xray-go/proxy/trojan/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/config.go` & `Xray-core-1.8.9/xray-go/proxy/trojan/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/trojan/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/config.proto` & `Xray-core-1.8.9/xray-go/proxy/trojan/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/protocol.go` & `Xray-core-1.8.9/xray-go/proxy/trojan/protocol.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/protocol_test.go` & `Xray-core-1.8.9/xray-go/proxy/trojan/protocol_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/server.go` & `Xray-core-1.8.9/xray-go/proxy/trojan/server.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/trojan/validator.go` & `Xray-core-1.8.9/xray-go/proxy/trojan/validator.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/account.go` & `Xray-core-1.8.9/xray-go/proxy/vless/account.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/account.pb.go` & `Xray-core-1.8.9/xray-go/proxy/vless/account.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/account.proto` & `Xray-core-1.8.9/xray-go/proxy/vless/account.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/encoding/addons.go` & `Xray-core-1.8.9/xray-go/proxy/vless/encoding/addons.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/encoding/addons.pb.go` & `Xray-core-1.8.9/xray-go/proxy/vless/encoding/addons.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/encoding/encoding.go` & `Xray-core-1.8.9/xray-go/proxy/vless/encoding/encoding.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/encoding/encoding_test.go` & `Xray-core-1.8.9/xray-go/proxy/vless/encoding/encoding_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/inbound/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/vless/inbound/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/inbound/config.proto` & `Xray-core-1.8.9/xray-go/proxy/vless/inbound/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/inbound/inbound.go` & `Xray-core-1.8.9/xray-go/proxy/vless/inbound/inbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/outbound/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/vless/outbound/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/outbound/outbound.go` & `Xray-core-1.8.9/xray-go/proxy/vless/outbound/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vless/validator.go` & `Xray-core-1.8.9/xray-go/proxy/vless/validator.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/account.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/account.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/account.pb.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/account.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/account.proto` & `Xray-core-1.8.9/xray-go/proxy/vmess/account.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/aead/authid.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/aead/authid.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/aead/authid_test.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/aead/authid_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/aead/consts.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/aead/consts.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/aead/encrypt.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/aead/encrypt.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/aead/encrypt_test.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/aead/encrypt_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/aead/kdf.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/aead/kdf.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/encoding/auth.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/encoding/auth.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/encoding/client.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/encoding/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/encoding/commands.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/encoding/commands.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/encoding/commands_test.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/encoding/commands_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/encoding/encoding.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/encoding/encoding.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/encoding/encoding_test.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/encoding/encoding_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/encoding/server.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/encoding/server.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/inbound/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/inbound/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/inbound/config.proto` & `Xray-core-1.8.9/xray-go/proxy/vmess/inbound/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/inbound/inbound.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/inbound/inbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/outbound/command.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/outbound/command.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/outbound/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/outbound/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/outbound/outbound.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/outbound/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/validator.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/validator.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/vmess/validator_test.go` & `Xray-core-1.8.9/xray-go/proxy/vmess/validator_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/bind.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/bind.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/client.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/client.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/config.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/config.pb.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/config.proto` & `Xray-core-1.8.9/xray-go/proxy/wireguard/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/gvisortun/tun.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/gvisortun/tun.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/server.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/server.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/tun.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/tun.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/tun_linux.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/tun_linux.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/proxy/wireguard/wireguard.go` & `Xray-core-1.8.9/xray-go/proxy/wireguard/wireguard.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/coverage/coverall` & `Xray-core-1.8.9/xray-go/testing/coverage/coverall`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/coverage/coverall2` & `Xray-core-1.8.9/xray-go/testing/coverage/coverall2`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/mocks/dns.go` & `Xray-core-1.8.9/xray-go/testing/mocks/dns.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/mocks/io.go` & `Xray-core-1.8.9/xray-go/testing/mocks/io.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/mocks/log.go` & `Xray-core-1.8.9/xray-go/testing/mocks/log.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/mocks/mux.go` & `Xray-core-1.8.9/xray-go/testing/mocks/mux.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/mocks/outbound.go` & `Xray-core-1.8.9/xray-go/testing/mocks/outbound.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/mocks/proxy.go` & `Xray-core-1.8.9/xray-go/testing/mocks/proxy.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/command_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/command_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 	"github.com/xtls/xray-core/proxy/dokodemo"
 	"github.com/xtls/xray-core/proxy/freedom"
 	"github.com/xtls/xray-core/proxy/vmess"
 	"github.com/xtls/xray-core/proxy/vmess/inbound"
 	"github.com/xtls/xray-core/proxy/vmess/outbound"
 	"github.com/xtls/xray-core/testing/servers/tcp"
 	"google.golang.org/grpc"
+	"google.golang.org/grpc/credentials/insecure"
 )
 
 func TestCommanderRemoveHandler(t *testing.T) {
 	tcpServer := tcp.Server{
 		MsgProcessor: xor,
 	}
 	dest, err := tcpServer.Start()
@@ -99,15 +100,15 @@
 	common.Must(err)
 	defer CloseAllServers(servers)
 
 	if err := testTCPConn(clientPort, 1024, time.Second*5)(); err != nil {
 		t.Fatal(err)
 	}
 
-	cmdConn, err := grpc.Dial(fmt.Sprintf("127.0.0.1:%d", cmdPort), grpc.WithInsecure(), grpc.WithBlock())
+	cmdConn, err := grpc.Dial(fmt.Sprintf("127.0.0.1:%d", cmdPort), grpc.WithTransportCredentials(insecure.NewCredentials()), grpc.WithBlock())
 	common.Must(err)
 	defer cmdConn.Close()
 
 	hsClient := command.NewHandlerServiceClient(cmdConn)
 	resp, err := hsClient.RemoveInbound(context.Background(), &command.RemoveInboundRequest{
 		Tag: "d",
 	})
@@ -266,15 +267,15 @@
 
 	if err := testTCPConn(clientPort, 1024, time.Second*5)(); err != io.EOF &&
 		/*We might wish to drain the connection*/
 		(err != nil && !strings.HasSuffix(err.Error(), "i/o timeout")) {
 		t.Fatal("expected error: ", err)
 	}
 
-	cmdConn, err := grpc.Dial(fmt.Sprintf("127.0.0.1:%d", cmdPort), grpc.WithInsecure(), grpc.WithBlock())
+	cmdConn, err := grpc.Dial(fmt.Sprintf("127.0.0.1:%d", cmdPort), grpc.WithTransportCredentials(insecure.NewCredentials()), grpc.WithBlock())
 	common.Must(err)
 	defer cmdConn.Close()
 
 	hsClient := command.NewHandlerServiceClient(cmdConn)
 	resp, err := hsClient.AlterInbound(context.Background(), &command.AlterInboundRequest{
 		Tag: "v",
 		Operation: serial.ToTypedMessage(
@@ -447,15 +448,15 @@
 	}
 	defer CloseAllServers(servers)
 
 	if err := testTCPConn(clientPort, 10240*1024, time.Second*20)(); err != nil {
 		t.Fatal(err)
 	}
 
-	cmdConn, err := grpc.Dial(fmt.Sprintf("127.0.0.1:%d", cmdPort), grpc.WithInsecure(), grpc.WithBlock())
+	cmdConn, err := grpc.Dial(fmt.Sprintf("127.0.0.1:%d", cmdPort), grpc.WithTransportCredentials(insecure.NewCredentials()), grpc.WithBlock())
 	common.Must(err)
 	defer cmdConn.Close()
 
 	const name = "user>>>test>>>traffic>>>uplink"
 	sClient := statscmd.NewStatsServiceClient(cmdConn)
 
 	sresp, err := sClient.GetStats(context.Background(), &statscmd.GetStatsRequest{
```

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/common.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/common.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/common_coverage.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/common_coverage.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/common_regular.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/common_regular.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/dns_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/dns_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/dokodemo_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/dokodemo_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/feature_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/feature_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/http_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/http_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/metrics_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/metrics_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 package scenarios
 
 import (
 	"encoding/json"
 	"fmt"
-	"io/ioutil"
+	"io"
 	"net/http"
 	"testing"
 
 	"github.com/xtls/xray-core/app/metrics"
 	"github.com/xtls/xray-core/app/proxyman"
 	"github.com/xtls/xray-core/app/router"
 	"github.com/xtls/xray-core/common"
@@ -76,15 +76,15 @@
 	common.Must(err)
 	if resp == nil {
 		t.Error("unexpected pprof nil response")
 	}
 	if resp.StatusCode != http.StatusOK {
 		t.Error("unexpected pprof status code")
 	}
-	body, err := ioutil.ReadAll(resp.Body)
+	body, err := io.ReadAll(resp.Body)
 	if err != nil {
 		t.Fatal(err)
 	}
 	if string(body)[0:len(expectedMessage)] != expectedMessage {
 		t.Error("unexpected response body from pprof handler")
 	}
 
@@ -92,15 +92,15 @@
 	common.Must(err2)
 	if resp2 == nil {
 		t.Error("unexpected expvars nil response")
 	}
 	if resp2.StatusCode != http.StatusOK {
 		t.Error("unexpected expvars status code")
 	}
-	body2, err2 := ioutil.ReadAll(resp2.Body)
+	body2, err2 := io.ReadAll(resp2.Body)
 	if err2 != nil {
 		t.Fatal(err2)
 	}
 	var json2 map[string]interface{}
 	if json.Unmarshal(body2, &json2) != nil {
 		t.Error("unexpected response body from expvars handler")
 	}
```

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/policy_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/policy_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/reverse_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/reverse_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/shadowsocks_2022_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/shadowsocks_2022_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/shadowsocks_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/shadowsocks_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/socks_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/socks_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/tls_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/tls_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/transport_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/transport_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/vless_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/vless_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/scenarios/vmess_test.go` & `Xray-core-1.8.9/xray-go/testing/scenarios/vmess_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/servers/http/http.go` & `Xray-core-1.8.9/xray-go/testing/servers/http/http.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/servers/tcp/tcp.go` & `Xray-core-1.8.9/xray-go/testing/servers/tcp/tcp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/testing/servers/udp/udp.go` & `Xray-core-1.8.9/xray-go/testing/servers/udp/udp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/global/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/global/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/global/config.proto` & `Xray-core-1.8.9/xray-go/transport/global/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/dialer_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/dialer_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/domainsocket/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/domainsocket/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/domainsocket/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/domainsocket/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/domainsocket/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/domainsocket/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/domainsocket/dial.go` & `Xray-core-1.8.9/xray-go/transport/internet/domainsocket/dial.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/domainsocket/listener.go` & `Xray-core-1.8.9/xray-go/transport/internet/domainsocket/listener.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/domainsocket/listener_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/domainsocket/listener_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/filelocker_other.go` & `Xray-core-1.8.9/xray-go/transport/internet/filelocker_other.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/config.pb.go`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 
 type Config struct {
 	state         protoimpl.MessageState
 	sizeCache     protoimpl.SizeCache
 	unknownFields protoimpl.UnknownFields
 
-	Host                string `protobuf:"bytes,1,opt,name=host,proto3" json:"host,omitempty"`
+	Authority           string `protobuf:"bytes,1,opt,name=authority,proto3" json:"authority,omitempty"`
 	ServiceName         string `protobuf:"bytes,2,opt,name=service_name,json=serviceName,proto3" json:"service_name,omitempty"`
 	MultiMode           bool   `protobuf:"varint,3,opt,name=multi_mode,json=multiMode,proto3" json:"multi_mode,omitempty"`
 	IdleTimeout         int32  `protobuf:"varint,4,opt,name=idle_timeout,json=idleTimeout,proto3" json:"idle_timeout,omitempty"`
 	HealthCheckTimeout  int32  `protobuf:"varint,5,opt,name=health_check_timeout,json=healthCheckTimeout,proto3" json:"health_check_timeout,omitempty"`
 	PermitWithoutStream bool   `protobuf:"varint,6,opt,name=permit_without_stream,json=permitWithoutStream,proto3" json:"permit_without_stream,omitempty"`
 	InitialWindowsSize  int32  `protobuf:"varint,7,opt,name=initial_windows_size,json=initialWindowsSize,proto3" json:"initial_windows_size,omitempty"`
 	UserAgent           string `protobuf:"bytes,8,opt,name=user_agent,json=userAgent,proto3" json:"user_agent,omitempty"`
@@ -63,17 +63,17 @@
 }
 
 // Deprecated: Use Config.ProtoReflect.Descriptor instead.
 func (*Config) Descriptor() ([]byte, []int) {
 	return file_transport_internet_grpc_config_proto_rawDescGZIP(), []int{0}
 }
 
-func (x *Config) GetHost() string {
+func (x *Config) GetAuthority() string {
 	if x != nil {
-		return x.Host
+		return x.Authority
 	}
 	return ""
 }
 
 func (x *Config) GetServiceName() string {
 	if x != nil {
 		return x.ServiceName
@@ -126,39 +126,39 @@
 var File_transport_internet_grpc_config_proto protoreflect.FileDescriptor
 
 var file_transport_internet_grpc_config_proto_rawDesc = []byte{
 	0x0a, 0x24, 0x74, 0x72, 0x61, 0x6e, 0x73, 0x70, 0x6f, 0x72, 0x74, 0x2f, 0x69, 0x6e, 0x74, 0x65,
 	0x72, 0x6e, 0x65, 0x74, 0x2f, 0x67, 0x72, 0x70, 0x63, 0x2f, 0x63, 0x6f, 0x6e, 0x66, 0x69, 0x67,
 	0x2e, 0x70, 0x72, 0x6f, 0x74, 0x6f, 0x12, 0x25, 0x78, 0x72, 0x61, 0x79, 0x2e, 0x74, 0x72, 0x61,
 	0x6e, 0x73, 0x70, 0x6f, 0x72, 0x74, 0x2e, 0x69, 0x6e, 0x74, 0x65, 0x72, 0x6e, 0x65, 0x74, 0x2e,
-	0x67, 0x72, 0x70, 0x63, 0x2e, 0x65, 0x6e, 0x63, 0x6f, 0x64, 0x69, 0x6e, 0x67, 0x22, 0xb8, 0x02,
-	0x0a, 0x06, 0x43, 0x6f, 0x6e, 0x66, 0x69, 0x67, 0x12, 0x12, 0x0a, 0x04, 0x68, 0x6f, 0x73, 0x74,
-	0x18, 0x01, 0x20, 0x01, 0x28, 0x09, 0x52, 0x04, 0x68, 0x6f, 0x73, 0x74, 0x12, 0x21, 0x0a, 0x0c,
-	0x73, 0x65, 0x72, 0x76, 0x69, 0x63, 0x65, 0x5f, 0x6e, 0x61, 0x6d, 0x65, 0x18, 0x02, 0x20, 0x01,
-	0x28, 0x09, 0x52, 0x0b, 0x73, 0x65, 0x72, 0x76, 0x69, 0x63, 0x65, 0x4e, 0x61, 0x6d, 0x65, 0x12,
-	0x1d, 0x0a, 0x0a, 0x6d, 0x75, 0x6c, 0x74, 0x69, 0x5f, 0x6d, 0x6f, 0x64, 0x65, 0x18, 0x03, 0x20,
-	0x01, 0x28, 0x08, 0x52, 0x09, 0x6d, 0x75, 0x6c, 0x74, 0x69, 0x4d, 0x6f, 0x64, 0x65, 0x12, 0x21,
-	0x0a, 0x0c, 0x69, 0x64, 0x6c, 0x65, 0x5f, 0x74, 0x69, 0x6d, 0x65, 0x6f, 0x75, 0x74, 0x18, 0x04,
-	0x20, 0x01, 0x28, 0x05, 0x52, 0x0b, 0x69, 0x64, 0x6c, 0x65, 0x54, 0x69, 0x6d, 0x65, 0x6f, 0x75,
-	0x74, 0x12, 0x30, 0x0a, 0x14, 0x68, 0x65, 0x61, 0x6c, 0x74, 0x68, 0x5f, 0x63, 0x68, 0x65, 0x63,
-	0x6b, 0x5f, 0x74, 0x69, 0x6d, 0x65, 0x6f, 0x75, 0x74, 0x18, 0x05, 0x20, 0x01, 0x28, 0x05, 0x52,
-	0x12, 0x68, 0x65, 0x61, 0x6c, 0x74, 0x68, 0x43, 0x68, 0x65, 0x63, 0x6b, 0x54, 0x69, 0x6d, 0x65,
-	0x6f, 0x75, 0x74, 0x12, 0x32, 0x0a, 0x15, 0x70, 0x65, 0x72, 0x6d, 0x69, 0x74, 0x5f, 0x77, 0x69,
-	0x74, 0x68, 0x6f, 0x75, 0x74, 0x5f, 0x73, 0x74, 0x72, 0x65, 0x61, 0x6d, 0x18, 0x06, 0x20, 0x01,
-	0x28, 0x08, 0x52, 0x13, 0x70, 0x65, 0x72, 0x6d, 0x69, 0x74, 0x57, 0x69, 0x74, 0x68, 0x6f, 0x75,
-	0x74, 0x53, 0x74, 0x72, 0x65, 0x61, 0x6d, 0x12, 0x30, 0x0a, 0x14, 0x69, 0x6e, 0x69, 0x74, 0x69,
-	0x61, 0x6c, 0x5f, 0x77, 0x69, 0x6e, 0x64, 0x6f, 0x77, 0x73, 0x5f, 0x73, 0x69, 0x7a, 0x65, 0x18,
-	0x07, 0x20, 0x01, 0x28, 0x05, 0x52, 0x12, 0x69, 0x6e, 0x69, 0x74, 0x69, 0x61, 0x6c, 0x57, 0x69,
-	0x6e, 0x64, 0x6f, 0x77, 0x73, 0x53, 0x69, 0x7a, 0x65, 0x12, 0x1d, 0x0a, 0x0a, 0x75, 0x73, 0x65,
-	0x72, 0x5f, 0x61, 0x67, 0x65, 0x6e, 0x74, 0x18, 0x08, 0x20, 0x01, 0x28, 0x09, 0x52, 0x09, 0x75,
-	0x73, 0x65, 0x72, 0x41, 0x67, 0x65, 0x6e, 0x74, 0x42, 0x33, 0x5a, 0x31, 0x67, 0x69, 0x74, 0x68,
-	0x75, 0x62, 0x2e, 0x63, 0x6f, 0x6d, 0x2f, 0x78, 0x74, 0x6c, 0x73, 0x2f, 0x78, 0x72, 0x61, 0x79,
-	0x2d, 0x63, 0x6f, 0x72, 0x65, 0x2f, 0x74, 0x72, 0x61, 0x6e, 0x73, 0x70, 0x6f, 0x72, 0x74, 0x2f,
-	0x69, 0x6e, 0x74, 0x65, 0x72, 0x6e, 0x65, 0x74, 0x2f, 0x67, 0x72, 0x70, 0x63, 0x62, 0x06, 0x70,
-	0x72, 0x6f, 0x74, 0x6f, 0x33,
+	0x67, 0x72, 0x70, 0x63, 0x2e, 0x65, 0x6e, 0x63, 0x6f, 0x64, 0x69, 0x6e, 0x67, 0x22, 0xc2, 0x02,
+	0x0a, 0x06, 0x43, 0x6f, 0x6e, 0x66, 0x69, 0x67, 0x12, 0x1c, 0x0a, 0x09, 0x61, 0x75, 0x74, 0x68,
+	0x6f, 0x72, 0x69, 0x74, 0x79, 0x18, 0x01, 0x20, 0x01, 0x28, 0x09, 0x52, 0x09, 0x61, 0x75, 0x74,
+	0x68, 0x6f, 0x72, 0x69, 0x74, 0x79, 0x12, 0x21, 0x0a, 0x0c, 0x73, 0x65, 0x72, 0x76, 0x69, 0x63,
+	0x65, 0x5f, 0x6e, 0x61, 0x6d, 0x65, 0x18, 0x02, 0x20, 0x01, 0x28, 0x09, 0x52, 0x0b, 0x73, 0x65,
+	0x72, 0x76, 0x69, 0x63, 0x65, 0x4e, 0x61, 0x6d, 0x65, 0x12, 0x1d, 0x0a, 0x0a, 0x6d, 0x75, 0x6c,
+	0x74, 0x69, 0x5f, 0x6d, 0x6f, 0x64, 0x65, 0x18, 0x03, 0x20, 0x01, 0x28, 0x08, 0x52, 0x09, 0x6d,
+	0x75, 0x6c, 0x74, 0x69, 0x4d, 0x6f, 0x64, 0x65, 0x12, 0x21, 0x0a, 0x0c, 0x69, 0x64, 0x6c, 0x65,
+	0x5f, 0x74, 0x69, 0x6d, 0x65, 0x6f, 0x75, 0x74, 0x18, 0x04, 0x20, 0x01, 0x28, 0x05, 0x52, 0x0b,
+	0x69, 0x64, 0x6c, 0x65, 0x54, 0x69, 0x6d, 0x65, 0x6f, 0x75, 0x74, 0x12, 0x30, 0x0a, 0x14, 0x68,
+	0x65, 0x61, 0x6c, 0x74, 0x68, 0x5f, 0x63, 0x68, 0x65, 0x63, 0x6b, 0x5f, 0x74, 0x69, 0x6d, 0x65,
+	0x6f, 0x75, 0x74, 0x18, 0x05, 0x20, 0x01, 0x28, 0x05, 0x52, 0x12, 0x68, 0x65, 0x61, 0x6c, 0x74,
+	0x68, 0x43, 0x68, 0x65, 0x63, 0x6b, 0x54, 0x69, 0x6d, 0x65, 0x6f, 0x75, 0x74, 0x12, 0x32, 0x0a,
+	0x15, 0x70, 0x65, 0x72, 0x6d, 0x69, 0x74, 0x5f, 0x77, 0x69, 0x74, 0x68, 0x6f, 0x75, 0x74, 0x5f,
+	0x73, 0x74, 0x72, 0x65, 0x61, 0x6d, 0x18, 0x06, 0x20, 0x01, 0x28, 0x08, 0x52, 0x13, 0x70, 0x65,
+	0x72, 0x6d, 0x69, 0x74, 0x57, 0x69, 0x74, 0x68, 0x6f, 0x75, 0x74, 0x53, 0x74, 0x72, 0x65, 0x61,
+	0x6d, 0x12, 0x30, 0x0a, 0x14, 0x69, 0x6e, 0x69, 0x74, 0x69, 0x61, 0x6c, 0x5f, 0x77, 0x69, 0x6e,
+	0x64, 0x6f, 0x77, 0x73, 0x5f, 0x73, 0x69, 0x7a, 0x65, 0x18, 0x07, 0x20, 0x01, 0x28, 0x05, 0x52,
+	0x12, 0x69, 0x6e, 0x69, 0x74, 0x69, 0x61, 0x6c, 0x57, 0x69, 0x6e, 0x64, 0x6f, 0x77, 0x73, 0x53,
+	0x69, 0x7a, 0x65, 0x12, 0x1d, 0x0a, 0x0a, 0x75, 0x73, 0x65, 0x72, 0x5f, 0x61, 0x67, 0x65, 0x6e,
+	0x74, 0x18, 0x08, 0x20, 0x01, 0x28, 0x09, 0x52, 0x09, 0x75, 0x73, 0x65, 0x72, 0x41, 0x67, 0x65,
+	0x6e, 0x74, 0x42, 0x33, 0x5a, 0x31, 0x67, 0x69, 0x74, 0x68, 0x75, 0x62, 0x2e, 0x63, 0x6f, 0x6d,
+	0x2f, 0x78, 0x74, 0x6c, 0x73, 0x2f, 0x78, 0x72, 0x61, 0x79, 0x2d, 0x63, 0x6f, 0x72, 0x65, 0x2f,
+	0x74, 0x72, 0x61, 0x6e, 0x73, 0x70, 0x6f, 0x72, 0x74, 0x2f, 0x69, 0x6e, 0x74, 0x65, 0x72, 0x6e,
+	0x65, 0x74, 0x2f, 0x67, 0x72, 0x70, 0x63, 0x62, 0x06, 0x70, 0x72, 0x6f, 0x74, 0x6f, 0x33,
 }
 
 var (
 	file_transport_internet_grpc_config_proto_rawDescOnce sync.Once
 	file_transport_internet_grpc_config_proto_rawDescData = file_transport_internet_grpc_config_proto_rawDesc
 )
```

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/config_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/config_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/dial.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/dial.go`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	"github.com/xtls/xray-core/transport/internet/grpc/encoding"
 	"github.com/xtls/xray-core/transport/internet/reality"
 	"github.com/xtls/xray-core/transport/internet/stat"
 	"github.com/xtls/xray-core/transport/internet/tls"
 	"google.golang.org/grpc"
 	"google.golang.org/grpc/backoff"
 	"google.golang.org/grpc/connectivity"
-	"google.golang.org/grpc/credentials"
+	"google.golang.org/grpc/credentials/insecure"
 	"google.golang.org/grpc/keepalive"
 )
 
 func Dial(ctx context.Context, dest net.Destination, streamSettings *internet.MemoryStreamConfig) (stat.Connection, error) {
 	newError("creating connection to ", dest).WriteToLog(session.ExportIDToError(ctx))
 
 	conn, err := dialgRPC(ctx, dest, streamSettings)
@@ -118,32 +118,45 @@
 			address := net.ParseAddress(rawHost)
 
 			gctx = session.ContextWithID(gctx, session.IDFromContext(ctx))
 			gctx = session.ContextWithOutbound(gctx, session.OutboundFromContext(ctx))
 			gctx = session.ContextWithTimeoutOnly(gctx, true)
 
 			c, err := internet.DialSystem(gctx, net.TCPDestination(address, port), sockopt)
-			if err == nil && realityConfig != nil {
-				return reality.UClient(c, realityConfig, gctx, dest)
+			if err == nil {
+				if tlsConfig != nil {
+					config := tlsConfig.GetTLSConfig()
+					if config.ServerName == "" && address.Family().IsDomain() {
+						config.ServerName = address.Domain()
+					}
+					if fingerprint := tls.GetFingerprint(tlsConfig.Fingerprint); fingerprint != nil {
+						return tls.UClient(c, config, fingerprint), nil
+					} else { // Fallback to normal gRPC TLS
+						return tls.Client(c, config), nil
+					}
+				}
+				if realityConfig != nil {
+					return reality.UClient(c, realityConfig, gctx, dest)
+				}
 			}
 			return c, err
 		}),
 	}
 
-	if tlsConfig != nil {
-		var transportCredential credentials.TransportCredentials
-		if fingerprint := tls.GetFingerprint(tlsConfig.Fingerprint); fingerprint != nil {
-			transportCredential = tls.NewGrpcUtls(tlsConfig.GetTLSConfig(), fingerprint)
-		} else { // Fallback to normal gRPC TLS
-			transportCredential = credentials.NewTLS(tlsConfig.GetTLSConfig())
-		}
-		dialOptions = append(dialOptions, grpc.WithTransportCredentials(transportCredential))
-	} else {
-		dialOptions = append(dialOptions, grpc.WithInsecure())
+	dialOptions = append(dialOptions, grpc.WithTransportCredentials(insecure.NewCredentials()))
+
+	authority := ""
+	if grpcSettings.Authority != "" {
+		authority = grpcSettings.Authority
+	} else if tlsConfig != nil && tlsConfig.ServerName != "" {
+		authority = tlsConfig.ServerName
+	} else if realityConfig == nil && dest.Address.Family().IsDomain() {
+		authority = dest.Address.Domain()
 	}
+	dialOptions = append(dialOptions, grpc.WithAuthority(authority))
 
 	if grpcSettings.IdleTimeout > 0 || grpcSettings.HealthCheckTimeout > 0 || grpcSettings.PermitWithoutStream {
 		dialOptions = append(dialOptions, grpc.WithKeepaliveParams(keepalive.ClientParameters{
 			Time:                time.Second * time.Duration(grpcSettings.IdleTimeout),
 			Timeout:             time.Second * time.Duration(grpcSettings.HealthCheckTimeout),
 			PermitWithoutStream: grpcSettings.PermitWithoutStream,
 		}))
```

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/customSeviceName.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/customSeviceName.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/hunkconn.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/hunkconn.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/multiconn.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/multiconn.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/stream.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/stream.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/encoding/stream_grpc.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/encoding/stream_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/grpc/hub.go` & `Xray-core-1.8.9/xray-go/transport/internet/grpc/hub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/header.go` & `Xray-core-1.8.9/xray-go/transport/internet/header.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/header_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/header_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/dns/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/dns/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/dns/dns.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/dns/dns.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/http/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/http/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/http/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/http/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/http/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/headers/http/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/http/http.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/http/http.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/http/http_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/http/http_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/http/resp.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/http/resp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/noop/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/noop/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/noop/noop.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/noop/noop.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/srtp.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/srtp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/srtp/srtp_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/srtp/srtp_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/tls/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/tls/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/tls/dtls.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/tls/dtls.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/tls/dtls_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/tls/dtls_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/utp/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/utp/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/utp/utp.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/utp/utp.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/utp/utp_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/utp/utp_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/wechat.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/wechat.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/wechat/wechat_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/wechat/wechat_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/wireguard/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/wireguard/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/headers/wireguard/wireguard.go` & `Xray-core-1.8.9/xray-go/transport/internet/headers/wireguard/wireguard.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/http/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/http/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/http/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/http/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/http/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/http/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/http/dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/http/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/http/http_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/http/http_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/http/hub.go` & `Xray-core-1.8.9/xray-go/transport/internet/http/hub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/connection.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/connection.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/connection_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/connection_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/crypt.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/crypt.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/crypt_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/crypt_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/io.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/io.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/io_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/io_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/kcp_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/kcp_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/listener.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/listener.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/output.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/output.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/receiving.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/receiving.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/segment.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/segment.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/segment_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/segment_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/sending.go` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/sending.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/kcp/xor_amd64.s` & `Xray-core-1.8.9/xray-go/transport/internet/kcp/xor_amd64.s`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/memory_settings.go` & `Xray-core-1.8.9/xray-go/transport/internet/memory_settings.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/quic/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/quic/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/quic/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/quic/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/quic/conn.go` & `Xray-core-1.8.9/xray-go/transport/internet/quic/conn.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/quic/dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/quic/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/quic/hub.go` & `Xray-core-1.8.9/xray-go/transport/internet/quic/hub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/quic/quic.go` & `Xray-core-1.8.9/xray-go/transport/internet/quic/quic.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/quic/quic_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/quic/quic_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/reality/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/reality/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/reality/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/reality/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/reality/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/reality/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/reality/reality.go` & `Xray-core-1.8.9/xray-go/transport/internet/reality/reality.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/sockopt_darwin.go` & `Xray-core-1.8.9/xray-go/transport/internet/sockopt_darwin.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/sockopt_freebsd.go` & `Xray-core-1.8.9/xray-go/transport/internet/sockopt_freebsd.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/sockopt_linux.go` & `Xray-core-1.8.9/xray-go/transport/internet/sockopt_linux.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/sockopt_linux_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/sockopt_linux_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/sockopt_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/sockopt_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/sockopt_windows.go` & `Xray-core-1.8.9/xray-go/transport/internet/sockopt_windows.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/stat/connection.go` & `Xray-core-1.8.9/xray-go/transport/internet/stat/connection.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/system_dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/system_dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/system_listener.go` & `Xray-core-1.8.9/xray-go/transport/internet/system_listener.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/system_listener_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/system_listener_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tagged/taggedimpl/impl.go` & `Xray-core-1.8.9/xray-go/transport/internet/tagged/taggedimpl/impl.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp/dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp/hub.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp/hub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_darwin.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_darwin.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_freebsd.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_freebsd.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_linux.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_linux.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp/sockopt_linux_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp/sockopt_linux_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tcp_hub.go` & `Xray-core-1.8.9/xray-go/transport/internet/tcp_hub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/tls/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/config_other.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/config_other.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/config_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/config_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/grpc.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/grpc.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/pin.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/pin.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/pin_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/pin_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/tls/tls.go` & `Xray-core-1.8.9/xray-go/transport/internet/tls/tls.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/dispatcher.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/dispatcher.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/dispatcher_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/dispatcher_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/hub.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/hub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/hub_darwin.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/hub_darwin.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/hub_freebsd.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/hub_freebsd.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/udp/hub_linux.go` & `Xray-core-1.8.9/xray-go/transport/internet/udp/hub_linux.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/config.go` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/config.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/config.pb.go` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/config.pb.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/config.proto` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/config.proto`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/connection.go` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/connection.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/dialer.go` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/dialer.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/dialer.html` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/dialer.html`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/hub.go` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/hub.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/internet/websocket/ws_test.go` & `Xray-core-1.8.9/xray-go/transport/internet/websocket/ws_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/pipe/impl.go` & `Xray-core-1.8.9/xray-go/transport/pipe/impl.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/pipe/pipe.go` & `Xray-core-1.8.9/xray-go/transport/pipe/pipe.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/pipe/pipe_test.go` & `Xray-core-1.8.9/xray-go/transport/pipe/pipe_test.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/pipe/reader.go` & `Xray-core-1.8.9/xray-go/transport/pipe/reader.go`

 * *Files identical despite different names*

### Comparing `Xray-core-1.8.8/xray-go/transport/pipe/writer.go` & `Xray-core-1.8.9/xray-go/transport/pipe/writer.go`

 * *Files identical despite different names*

