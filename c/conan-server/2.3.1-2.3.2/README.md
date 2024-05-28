# Comparing `tmp/conan-server-2.3.1.tar.gz` & `tmp/conan-server-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-server-2.3.1.tar", last modified: Thu May 16 17:41:05 2024, max compression
+gzip compressed data, was "dist/conan-server-2.3.2.tar", last modified: Tue May 28 09:10:28 2024, max compression
```

## Comparing `conan-server-2.3.1.tar` & `conan-server-2.3.2.tar`

### file list

```diff
@@ -1,430 +1,430 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.657342 conan-server-2.3.1/
--rw-r--r--   0 root         (0) root         (0)     1084 2024-05-16 17:40:48.000000 conan-server-2.3.1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-16 17:40:48.000000 conan-server-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8185 2024-05-16 17:41:05.657342 conan-server-2.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6118 2024-05-16 17:40:48.000000 conan-server-2.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.608337 conan-server-2.3.1/conan/
--rw-r--r--   0 root         (0) root         (0)      165 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.608337 conan-server-2.3.1/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2455 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)    13040 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     9460 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.611337 conan-server-2.3.1/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13263 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/command.py
--rw-r--r--   0 root         (0) root         (0)     9255 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     4793 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2714 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    11805 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3961 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)    17548 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     5596 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4808 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     5193 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     7441 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)    13412 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     6670 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.611337 conan-server-2.3.1/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7430 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    12224 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     8279 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.614338 conan-server-2.3.1/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3994 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     7489 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     4609 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)    10989 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3252 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     3157 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5914 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)    21213 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4704 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)    13371 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     7511 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4260 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3696 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/pkglist.py
--rw-r--r--   0 root         (0) root         (0)     3553 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    12835 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     6487 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     4411 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     6871 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      490 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.614338 conan-server-2.3.1/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.615338 conan-server-2.3.1/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5663 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)    15953 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.615338 conan-server-2.3.1/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.616338 conan-server-2.3.1/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6412 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.616338 conan-server-2.3.1/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.617338 conan-server-2.3.1/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21295 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/detect_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.618338 conan-server-2.3.1/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2736 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3850 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2916 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2041 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     4565 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     8212 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/local_recipes_index.py
--rw-r--r--   0 root         (0) root         (0)     2334 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12307 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.619338 conan-server-2.3.1/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11189 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.619338 conan-server-2.3.1/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3949 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     9222 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2639 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/cache/home_paths.py
--rw-r--r--   0 root         (0) root         (0)     3114 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/integrity_check.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/internal_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.620338 conan-server-2.3.1/conan/internal/runner/
--rw-r--r--   0 root         (0) root         (0)      302 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14525 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/runner/docker.py
--rw-r--r--   0 root         (0) root         (0)    12370 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/runner/ssh.py
--rw-r--r--   0 root         (0) root         (0)     6712 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/runner/wsl.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/internal/upload_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.620338 conan-server-2.3.1/conan/tools/
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.620338 conan-server-2.3.1/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.621338 conan-server-2.3.1/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12880 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16239 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5754 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.622338 conan-server-2.3.1/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4190 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11121 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2302 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    16208 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.623339 conan-server-2.3.1/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      217 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14319 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.623339 conan-server-2.3.1/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11138 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.624339 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     3944 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4563 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     4061 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5956 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14989 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    20350 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3656 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     4746 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    17034 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.624339 conan-server-2.3.1/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45120 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13891 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.625339 conan-server-2.3.1/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26546 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3601 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3561 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.626339 conan-server-2.3.1/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      535 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2672 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     7429 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)    24002 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     4177 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     6540 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.626339 conan-server-2.3.1/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.628339 conan-server-2.3.1/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6173 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2962 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    13681 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3986 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)    13632 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/gnutoolchain.py
--rw-r--r--   0 root         (0) root         (0)    27066 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/makedeps.py
--rw-r--r--   0 root         (0) root         (0)     4290 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    19100 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.628339 conan-server-2.3.1/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3387 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    23672 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)     1188 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)     8113 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.629339 conan-server-2.3.1/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6498 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.629339 conan-server-2.3.1/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.629339 conan-server-2.3.1/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4702 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5269 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    25007 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.631339 conan-server-2.3.1/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1335 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3312 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19246 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2967 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4984 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      593 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    11139 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    15069 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.631339 conan-server-2.3.1/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    10534 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.631339 conan-server-2.3.1/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2901 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9897 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.632339 conan-server-2.3.1/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13281 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.632339 conan-server-2.3.1/conan/tools/scons/
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/scons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/scons/sconsdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.632339 conan-server-2.3.1/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17993 2024-05-16 17:40:48.000000 conan-server-2.3.1/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.633340 conan-server-2.3.1/conan_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8185 2024-05-16 17:41:05.000000 conan-server-2.3.1/conan_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11473 2024-05-16 17:41:05.000000 conan-server-2.3.1/conan_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 17:41:05.000000 conan-server-2.3.1/conan_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-16 17:41:05.000000 conan-server-2.3.1/conan_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      616 2024-05-16 17:41:05.000000 conan-server-2.3.1/conan_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-16 17:41:05.000000 conan-server-2.3.1/conan_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.635340 conan-server-2.3.1/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.637340 conan-server-2.3.1/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.637340 conan-server-2.3.1/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4924 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/cache/editable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.638340 conan-server-2.3.1/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7883 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12622 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/cmd/uploader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.639340 conan-server-2.3.1/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conanfile/implementations.py
--rw-r--r--   0 root         (0) root         (0)     2138 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.639340 conan-server-2.3.1/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     7461 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7919 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     4595 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1270 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.640340 conan-server-2.3.1/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10333 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6731 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.640340 conan-server-2.3.1/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)    10455 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.642341 conan-server-2.3.1/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     6170 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     4451 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    15998 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    23157 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    22436 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     2924 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    21376 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     5186 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1895 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     7221 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     6480 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     5326 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21840 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    17007 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     5413 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    17816 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    14595 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.644341 conan-server-2.3.1/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5837 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6936 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     3945 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     2650 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/remote_credentials.py
--rw-r--r--   0 root         (0) root         (0)     5424 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)     9776 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    14934 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     9149 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/rest_client_local_recipe_index.py
--rw-r--r--   0 root         (0) root         (0)     3903 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.644341 conan-server-2.3.1/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4205 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     4223 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7419 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     3290 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.647341 conan-server-2.3.1/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20506 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    12678 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    32672 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     6302 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)    13316 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    15205 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17829 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     7155 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     8317 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    24616 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    14049 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6184 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     8643 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.647341 conan-server-2.3.1/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2198 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      251 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      191 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/requirements_runner.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.648341 conan-server-2.3.1/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4474 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.649341 conan-server-2.3.1/conans/server/
--rw-r--r--   0 root         (0) root         (0)      172 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.649341 conan-server-2.3.1/conans/server/conf/
--rw-r--r--   0 root         (0) root         (0)     9523 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2398 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/conf/default_server_conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.649341 conan-server-2.3.1/conans/server/crypto/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/crypto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.649341 conan-server-2.3.1/conans/server/crypto/jwt/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/crypto/jwt/__init__.py
--rw-r--r--   0 root         (0) root         (0)      734 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/crypto/jwt/jwt_credentials_manager.py
--rw-r--r--   0 root         (0) root         (0)     1058 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/crypto/jwt/jwt_manager.py
--rw-r--r--   0 root         (0) root         (0)     2808 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/launcher.py
--rw-r--r--   0 root         (0) root         (0)      776 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/migrate.py
--rw-r--r--   0 root         (0) root         (0)      315 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/migrations.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/plugin_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.650341 conan-server-2.3.1/conans/server/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/api_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.651342 conan-server-2.3.1/conans/server/rest/bottle_plugins/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/bottle_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2844 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/bottle_plugins/authorization_header.py
--rw-r--r--   0 root         (0) root         (0)     1545 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/bottle_plugins/http_basic_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1583 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/bottle_plugins/jwt_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1765 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/bottle_plugins/return_handler.py
--rw-r--r--   0 root         (0) root         (0)      367 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/bottle_routes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.651342 conan-server-2.3.1/conans/server/rest/controller/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.652341 conan-server-2.3.1/conans/server/rest/controller/v2/
--rw-r--r--   0 root         (0) root         (0)      316 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3147 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/v2/conan.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/v2/delete.py
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/v2/ping.py
--rw-r--r--   0 root         (0) root         (0)     3319 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/v2/revisions.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/v2/search.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/controller/v2/users.py
--rw-r--r--   0 root         (0) root         (0)     1761 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/rest/server.py
--rw-r--r--   0 root         (0) root         (0)     1869 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/revision_list.py
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/server_launcher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.652341 conan-server-2.3.1/conans/server/service/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/service/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7057 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/service/authorize.py
--rw-r--r--   0 root         (0) root         (0)      210 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/service/mime.py
--rw-r--r--   0 root         (0) root         (0)      591 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/service/user_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.652341 conan-server-2.3.1/conans/server/service/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/service/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4125 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/service/v2/search.py
--rw-r--r--   0 root         (0) root         (0)     6315 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/service/v2/service_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.653342 conan-server-2.3.1/conans/server/store/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2473 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/store/disk_adapter.py
--rw-r--r--   0 root         (0) root         (0)    13212 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/store/server_store.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.653342 conan-server-2.3.1/conans/server/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1333 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/server/utils/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.653342 conan-server-2.3.1/conans/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.654342 conan-server-2.3.1/conans/test/assets/
--rw-r--r--   0 root         (0) root         (0)      510 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1651 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/assets/autotools.py
--rw-r--r--   0 root         (0) root         (0)     3753 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/assets/cmake.py
--rw-r--r--   0 root         (0) root         (0)    17307 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/assets/genconanfile.py
--rw-r--r--   0 root         (0) root         (0)     6352 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/assets/pkg_cmake.py
--rw-r--r--   0 root         (0) root         (0)     6008 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/assets/sources.py
--rw-r--r--   0 root         (0) root         (0)    11972 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/assets/visual_project_files.py
--rw-r--r--   0 root         (0) root         (0)    13188 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.655342 conan-server-2.3.1/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     2806 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/file_server.py
--rw-r--r--   0 root         (0) root         (0)     4155 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3187 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    37579 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 17:41:05.657342 conan-server-2.3.1/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1396 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11974 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3729 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-05-16 17:40:48.000000 conan-server-2.3.1/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-16 17:40:48.000000 conan-server-2.3.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-16 17:41:05.658342 conan-server-2.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4985 2024-05-16 17:40:48.000000 conan-server-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.873769 conan-server-2.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-28 09:10:13.000000 conan-server-2.3.2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-28 09:10:13.000000 conan-server-2.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8185 2024-05-28 09:10:28.873769 conan-server-2.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6118 2024-05-28 09:10:13.000000 conan-server-2.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.830765 conan-server-2.3.2/conan/
+-rw-r--r--   0 root         (0) root         (0)      165 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.830765 conan-server-2.3.2/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)    13040 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.833765 conan-server-2.3.2/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13263 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/command.py
+-rw-r--r--   0 root         (0) root         (0)     9255 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3961 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5596 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     7441 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    13412 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.833765 conan-server-2.3.2/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7430 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    12224 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8279 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.836765 conan-server-2.3.2/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)    10989 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5914 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)    21213 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4704 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)    13371 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     7511 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/pkglist.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    12835 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     6871 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      490 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.836765 conan-server-2.3.2/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.837766 conan-server-2.3.2/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.838766 conan-server-2.3.2/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.838766 conan-server-2.3.2/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.839766 conan-server-2.3.2/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.839766 conan-server-2.3.2/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21295 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/detect_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.840766 conan-server-2.3.2/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/local_recipes_index.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.841766 conan-server-2.3.2/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11189 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.841766 conan-server-2.3.2/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     9222 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/cache/home_paths.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/integrity_check.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/internal_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.842766 conan-server-2.3.2/conan/internal/runner/
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14525 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/runner/docker.py
+-rw-r--r--   0 root         (0) root         (0)    12370 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/runner/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/runner/wsl.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/internal/upload_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.842766 conan-server-2.3.2/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.842766 conan-server-2.3.2/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.843766 conan-server-2.3.2/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12880 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16239 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.844766 conan-server-2.3.2/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11121 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    16208 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.844766 conan-server-2.3.2/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      217 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14319 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.844766 conan-server-2.3.2/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11138 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.845766 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     3944 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14989 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    20350 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     4746 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    17034 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.846766 conan-server-2.3.2/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45224 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    13891 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.846766 conan-server-2.3.2/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26546 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.847766 conan-server-2.3.2/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     7429 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    24002 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.847766 conan-server-2.3.2/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.848767 conan-server-2.3.2/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13681 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)    13632 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/gnutoolchain.py
+-rw-r--r--   0 root         (0) root         (0)    27066 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/makedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    19100 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.849767 conan-server-2.3.2/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    23672 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)     8113 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.849767 conan-server-2.3.2/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.849767 conan-server-2.3.2/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.850767 conan-server-2.3.2/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    25007 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.851767 conan-server-2.3.2/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19246 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      593 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    15163 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.851767 conan-server-2.3.2/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10534 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.852767 conan-server-2.3.2/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9897 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.852767 conan-server-2.3.2/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13281 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.852767 conan-server-2.3.2/conan/tools/scons/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/scons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/scons/sconsdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.852767 conan-server-2.3.2/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17993 2024-05-28 09:10:13.000000 conan-server-2.3.2/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.853767 conan-server-2.3.2/conan_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8185 2024-05-28 09:10:28.000000 conan-server-2.3.2/conan_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11473 2024-05-28 09:10:28.000000 conan-server-2.3.2/conan_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 09:10:28.000000 conan-server-2.3.2/conan_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-28 09:10:28.000000 conan-server-2.3.2/conan_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      616 2024-05-28 09:10:28.000000 conan-server-2.3.2/conan_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-28 09:10:28.000000 conan-server-2.3.2/conan_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.854767 conan-server-2.3.2/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.856767 conan-server-2.3.2/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.856767 conan-server-2.3.2/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/cache/editable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.857767 conan-server-2.3.2/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12622 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/cmd/uploader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.857767 conan-server-2.3.2/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conanfile/implementations.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.858767 conan-server-2.3.2/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     7461 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7919 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     4595 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.858767 conan-server-2.3.2/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6731 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.858767 conan-server-2.3.2/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)    10455 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.860768 conan-server-2.3.2/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    15998 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    23157 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    22436 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    21376 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5186 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     5326 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21840 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    17007 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    17816 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    14595 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.861768 conan-server-2.3.2/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5837 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6936 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/remote_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     5424 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)     9776 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    14934 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9282 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/rest_client_local_recipe_index.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.862768 conan-server-2.3.2/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4205 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.864768 conan-server-2.3.2/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20506 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12678 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    32796 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     6302 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    13316 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    15205 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17829 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     7155 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     8317 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    24616 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    14049 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     8643 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.865768 conan-server-2.3.2/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/requirements_runner.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.865768 conan-server-2.3.2/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.866768 conan-server-2.3.2/conans/server/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.866768 conan-server-2.3.2/conans/server/conf/
+-rw-r--r--   0 root         (0) root         (0)     9523 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/conf/default_server_conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.866768 conan-server-2.3.2/conans/server/crypto/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/crypto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.866768 conan-server-2.3.2/conans/server/crypto/jwt/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/crypto/jwt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/crypto/jwt/jwt_credentials_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/crypto/jwt/jwt_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      776 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/migrate.py
+-rw-r--r--   0 root         (0) root         (0)      315 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/migrations.py
+-rw-r--r--   0 root         (0) root         (0)      989 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/plugin_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.867768 conan-server-2.3.2/conans/server/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/api_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.867768 conan-server-2.3.2/conans/server/rest/bottle_plugins/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/bottle_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/bottle_plugins/authorization_header.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/bottle_plugins/http_basic_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/bottle_plugins/jwt_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/bottle_plugins/return_handler.py
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/bottle_routes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.868768 conan-server-2.3.2/conans/server/rest/controller/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.868768 conan-server-2.3.2/conans/server/rest/controller/v2/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/v2/conan.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/v2/delete.py
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/v2/ping.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/v2/revisions.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/v2/search.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/controller/v2/users.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/rest/server.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/revision_list.py
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/server_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.869768 conan-server-2.3.2/conans/server/service/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/service/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/service/authorize.py
+-rw-r--r--   0 root         (0) root         (0)      210 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/service/mime.py
+-rw-r--r--   0 root         (0) root         (0)      591 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/service/user_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.869768 conan-server-2.3.2/conans/server/service/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/service/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4125 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/service/v2/search.py
+-rw-r--r--   0 root         (0) root         (0)     6315 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/service/v2/service_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.869768 conan-server-2.3.2/conans/server/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/store/disk_adapter.py
+-rw-r--r--   0 root         (0) root         (0)    13212 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/store/server_store.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.870769 conan-server-2.3.2/conans/server/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/server/utils/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.870769 conan-server-2.3.2/conans/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.871769 conan-server-2.3.2/conans/test/assets/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/assets/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/assets/cmake.py
+-rw-r--r--   0 root         (0) root         (0)    17307 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/assets/genconanfile.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/assets/pkg_cmake.py
+-rw-r--r--   0 root         (0) root         (0)     6008 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/assets/sources.py
+-rw-r--r--   0 root         (0) root         (0)    11972 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/assets/visual_project_files.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2024-05-28 09:10:13.000000 conan-server-2.3.2/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.872769 conan-server-2.3.2/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/file_server.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    37579 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:10:28.873769 conan-server-2.3.2/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3729 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-28 09:10:14.000000 conan-server-2.3.2/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-28 09:10:14.000000 conan-server-2.3.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-28 09:10:28.874769 conan-server-2.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4985 2024-05-28 09:10:14.000000 conan-server-2.3.2/setup.py
```

### Comparing `conan-server-2.3.1/LICENSE.md` & `conan-server-2.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/PKG-INFO` & `conan-server-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-server
-Version: 2.3.1
+Version: 2.3.2
 Summary: Conan Server of Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Description: <picture>
           <!-- These are also used for https://github.com/conan-io/.github/blob/main/profile/README.md -->
```

### Comparing `conan-server-2.3.1/README.md` & `conan-server-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/conan_api.py` & `conan-server-2.3.2/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/model.py` & `conan-server-2.3.2/conan/api/model.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/output.py` & `conan-server-2.3.2/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/cache.py` & `conan-server-2.3.2/conan/api/subapi/cache.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/command.py` & `conan-server-2.3.2/conan/api/subapi/command.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/config.py` & `conan-server-2.3.2/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/download.py` & `conan-server-2.3.2/conan/api/subapi/download.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/export.py` & `conan-server-2.3.2/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/graph.py` & `conan-server-2.3.2/conan/api/subapi/graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/install.py` & `conan-server-2.3.2/conan/api/subapi/install.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/list.py` & `conan-server-2.3.2/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/local.py` & `conan-server-2.3.2/conan/api/subapi/local.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/lockfile.py` & `conan-server-2.3.2/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/new.py` & `conan-server-2.3.2/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/profiles.py` & `conan-server-2.3.2/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/remotes.py` & `conan-server-2.3.2/conan/api/subapi/remotes.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/remove.py` & `conan-server-2.3.2/conan/api/subapi/remove.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/search.py` & `conan-server-2.3.2/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/api/subapi/upload.py` & `conan-server-2.3.2/conan/api/subapi/upload.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/args.py` & `conan-server-2.3.2/conan/cli/args.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/cli.py` & `conan-server-2.3.2/conan/cli/cli.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/command.py` & `conan-server-2.3.2/conan/cli/command.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/build.py` & `conan-server-2.3.2/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/cache.py` & `conan-server-2.3.2/conan/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/config.py` & `conan-server-2.3.2/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/create.py` & `conan-server-2.3.2/conan/cli/commands/create.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/download.py` & `conan-server-2.3.2/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/editable.py` & `conan-server-2.3.2/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/export.py` & `conan-server-2.3.2/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/export_pkg.py` & `conan-server-2.3.2/conan/cli/commands/export_pkg.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/graph.py` & `conan-server-2.3.2/conan/cli/commands/graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/inspect.py` & `conan-server-2.3.2/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/install.py` & `conan-server-2.3.2/conan/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/list.py` & `conan-server-2.3.2/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/lock.py` & `conan-server-2.3.2/conan/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/new.py` & `conan-server-2.3.2/conan/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/pkglist.py` & `conan-server-2.3.2/conan/cli/commands/pkglist.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/profile.py` & `conan-server-2.3.2/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/remote.py` & `conan-server-2.3.2/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/remove.py` & `conan-server-2.3.2/conan/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/search.py` & `conan-server-2.3.2/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/source.py` & `conan-server-2.3.2/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/test.py` & `conan-server-2.3.2/conan/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/upload.py` & `conan-server-2.3.2/conan/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/commands/version.py` & `conan-server-2.3.2/conan/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/formatters/graph/graph.py` & `conan-server-2.3.2/conan/cli/formatters/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/formatters/graph/graph_info_text.py` & `conan-server-2.3.2/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/formatters/graph/info_graph_html.py` & `conan-server-2.3.2/conan/cli/formatters/graph/info_graph_html.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/formatters/list/binary_html_table.py` & `conan-server-2.3.2/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/formatters/list/list.py` & `conan-server-2.3.2/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/formatters/list/search_table_html.py` & `conan-server-2.3.2/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/cli/printers/graph.py` & `conan-server-2.3.2/conan/cli/printers/graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/detect_api.py` & `conan-server-2.3.2/conan/internal/api/detect_api.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/autoools_exe.py` & `conan-server-2.3.2/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/autotools_lib.py` & `conan-server-2.3.2/conan/internal/api/new/autotools_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/basic.py` & `conan-server-2.3.2/conan/internal/api/new/basic.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/bazel_exe.py` & `conan-server-2.3.2/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/bazel_lib.py` & `conan-server-2.3.2/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/cmake_exe.py` & `conan-server-2.3.2/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/cmake_lib.py` & `conan-server-2.3.2/conan/internal/api/new/cmake_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/local_recipes_index.py` & `conan-server-2.3.2/conan/internal/api/new/local_recipes_index.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/meson_exe.py` & `conan-server-2.3.2/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/meson_lib.py` & `conan-server-2.3.2/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/msbuild_exe.py` & `conan-server-2.3.2/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/api/new/msbuild_lib.py` & `conan-server-2.3.2/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/cache/cache.py` & `conan-server-2.3.2/conan/internal/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/cache/conan_reference_layout.py` & `conan-server-2.3.2/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/cache/db/cache_database.py` & `conan-server-2.3.2/conan/internal/cache/db/cache_database.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/cache/db/packages_table.py` & `conan-server-2.3.2/conan/internal/cache/db/packages_table.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/cache/db/recipes_table.py` & `conan-server-2.3.2/conan/internal/cache/db/recipes_table.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/cache/db/table.py` & `conan-server-2.3.2/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/cache/home_paths.py` & `conan-server-2.3.2/conan/internal/cache/home_paths.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/conan_app.py` & `conan-server-2.3.2/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/deploy.py` & `conan-server-2.3.2/conan/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/integrity_check.py` & `conan-server-2.3.2/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/internal_tools.py` & `conan-server-2.3.2/conan/internal/internal_tools.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/runner/docker.py` & `conan-server-2.3.2/conan/internal/runner/docker.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/runner/ssh.py` & `conan-server-2.3.2/conan/internal/runner/ssh.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/runner/wsl.py` & `conan-server-2.3.2/conan/internal/runner/wsl.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/internal/upload_metadata.py` & `conan-server-2.3.2/conan/internal/upload_metadata.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/android/utils.py` & `conan-server-2.3.2/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/apple/__init__.py` & `conan-server-2.3.2/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/apple/apple.py` & `conan-server-2.3.2/conan/tools/apple/apple.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/apple/xcodebuild.py` & `conan-server-2.3.2/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/apple/xcodedeps.py` & `conan-server-2.3.2/conan/tools/apple/xcodedeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/apple/xcodetoolchain.py` & `conan-server-2.3.2/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/build/__init__.py` & `conan-server-2.3.2/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/build/cppstd.py` & `conan-server-2.3.2/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/build/cpu.py` & `conan-server-2.3.2/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/build/cross_building.py` & `conan-server-2.3.2/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/build/flags.py` & `conan-server-2.3.2/conan/tools/build/flags.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/build/stdcpp_library.py` & `conan-server-2.3.2/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmake.py` & `conan-server-2.3.2/conan/tools/cmake/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-server-2.3.2/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/layout.py` & `conan-server-2.3.2/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/presets.py` & `conan-server-2.3.2/conan/tools/cmake/presets.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/cmake/toolchain/blocks.py` & `conan-server-2.3.2/conan/tools/cmake/toolchain/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,17 +806,18 @@
         compiler = settings.get_safe("compiler")
         if compiler == "intel-cc":
             return IntelCC(conanfile).ms_toolset
         elif compiler == "msvc":
             toolset = settings.get_safe("compiler.toolset")
             if toolset is None:
                 compiler_version = str(settings.compiler.version)
-                compiler_update = str(settings.compiler.update)
+                msvc_update = conanfile.conf.get("tools.microsoft:msvc_update")
+                compiler_update = msvc_update or settings.get_safe("compiler.update")
                 toolset = msvc_version_to_toolset_version(compiler_version)
-                if compiler_update != "None":  # It is full one(19.28), not generic 19.2X
+                if compiler_update is not None:  # It is full one(19.28), not generic 19.2X
                     # The equivalent of compiler 19.26 is toolset 14.26
                     toolset += ",version=14.{}{}".format(compiler_version[-1], compiler_update)
         elif compiler == "clang":
             if generator and "Visual" in generator:
                 if "Visual Studio 16" in generator or "Visual Studio 17" in generator:
                     toolset = "ClangCL"
                 else:
```

### Comparing `conan-server-2.3.1/conan/tools/cmake/toolchain/toolchain.py` & `conan-server-2.3.2/conan/tools/cmake/toolchain/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/env/environment.py` & `conan-server-2.3.2/conan/tools/env/environment.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/env/virtualbuildenv.py` & `conan-server-2.3.2/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/env/virtualrunenv.py` & `conan-server-2.3.2/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/files/__init__.py` & `conan-server-2.3.2/conan/tools/files/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/files/conandata.py` & `conan-server-2.3.2/conan/tools/files/conandata.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/files/copy_pattern.py` & `conan-server-2.3.2/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/files/files.py` & `conan-server-2.3.2/conan/tools/files/files.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/files/packager.py` & `conan-server-2.3.2/conan/tools/files/packager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/files/patches.py` & `conan-server-2.3.2/conan/tools/files/patches.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/files/symlinks/symlinks.py` & `conan-server-2.3.2/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/autotools.py` & `conan-server-2.3.2/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/autotoolsdeps.py` & `conan-server-2.3.2/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/autotoolstoolchain.py` & `conan-server-2.3.2/conan/tools/gnu/autotoolstoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/get_gnu_triplet.py` & `conan-server-2.3.2/conan/tools/gnu/get_gnu_triplet.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/gnudeps_flags.py` & `conan-server-2.3.2/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/gnutoolchain.py` & `conan-server-2.3.2/conan/tools/gnu/gnutoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/makedeps.py` & `conan-server-2.3.2/conan/tools/gnu/makedeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/pkgconfig.py` & `conan-server-2.3.2/conan/tools/gnu/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/gnu/pkgconfigdeps.py` & `conan-server-2.3.2/conan/tools/gnu/pkgconfigdeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/google/bazel.py` & `conan-server-2.3.2/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/google/bazeldeps.py` & `conan-server-2.3.2/conan/tools/google/bazeldeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/google/layout.py` & `conan-server-2.3.2/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/google/toolchain.py` & `conan-server-2.3.2/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/intel/intel_cc.py` & `conan-server-2.3.2/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/layout/__init__.py` & `conan-server-2.3.2/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/meson/helpers.py` & `conan-server-2.3.2/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/meson/meson.py` & `conan-server-2.3.2/conan/tools/meson/meson.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/meson/toolchain.py` & `conan-server-2.3.2/conan/tools/meson/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/__init__.py` & `conan-server-2.3.2/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/layout.py` & `conan-server-2.3.2/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/msbuild.py` & `conan-server-2.3.2/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/msbuilddeps.py` & `conan-server-2.3.2/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/nmakedeps.py` & `conan-server-2.3.2/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/nmaketoolchain.py` & `conan-server-2.3.2/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/subsystems.py` & `conan-server-2.3.2/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/toolchain.py` & `conan-server-2.3.2/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/microsoft/visual.py` & `conan-server-2.3.2/conan/tools/microsoft/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,16 @@
                             "16": "192",
                             "15": "191",
                             "14": "190",
                             "12": "180",
                             "11": "170"}.get(compiler_version)
     elif compiler == "msvc":
         compiler_version = conanfile.settings.get_safe("compiler.version")
-        compiler_update = conanfile.settings.get_safe("compiler.update")
+        msvc_update = conanfile.conf.get("tools.microsoft:msvc_update")
+        compiler_update = msvc_update or conanfile.settings.get_safe("compiler.update")
         if compiler_version and compiler_update is not None:
             compiler_version += ".{}".format(compiler_update)
 
     if compiler_version and Version(compiler_version) < version:
         if raise_invalid:
             msg = f"This package doesn't work with VS compiler version '{compiler_version}'" \
                   f", it requires at least '{version}'"
@@ -165,26 +166,26 @@
         from conan.tools.env.environment import create_env_script
         conan_vcvars_bat = f"{CONAN_VCVARS}.bat"
         create_env_script(conanfile, content, conan_vcvars_bat, scope)
         _create_deactivate_vcvars_file(conanfile, conan_vcvars_bat)
 
         is_ps1 = conanfile.conf.get("tools.env.virtualenv:powershell", check_type=bool, default=False)
         if is_ps1:
-            content_ps1 = textwrap.dedent(rf"""\
+            content_ps1 = textwrap.dedent(rf"""
             if (-not $env:VSCMD_ARG_VCVARS_VER){{
                 Push-Location "$PSScriptRoot"
                 cmd /c "conanvcvars.bat&set" |
                 foreach {{
                   if ($_ -match "=") {{
                     $v = $_.split("=", 2); set-item -force -path "ENV:\$($v[0])"  -value "$($v[1])"
                   }}
                 }}
                 Pop-Location
                 write-host conanvcvars.ps1: Activated environment}}
-            """)
+            """).strip()
             conan_vcvars_ps1 = f"{CONAN_VCVARS}.ps1"
             create_env_script(conanfile, content_ps1, conan_vcvars_ps1, scope)
             _create_deactivate_vcvars_file(conanfile, conan_vcvars_ps1)
 
 
 def _create_deactivate_vcvars_file(conanfile, filename):
     deactivate_filename = f"deactivate_{filename}"
```

### Comparing `conan-server-2.3.1/conan/tools/premake/premake.py` & `conan-server-2.3.2/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/premake/premakedeps.py` & `conan-server-2.3.2/conan/tools/premake/premakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/qbs/qbs.py` & `conan-server-2.3.2/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/qbs/qbsprofile.py` & `conan-server-2.3.2/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/scm/git.py` & `conan-server-2.3.2/conan/tools/scm/git.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/scons/sconsdeps.py` & `conan-server-2.3.2/conan/tools/scons/sconsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan/tools/system/package_manager.py` & `conan-server-2.3.2/conan/tools/system/package_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan_server.egg-info/PKG-INFO` & `conan-server-2.3.2/conan_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan-server
-Version: 2.3.1
+Version: 2.3.2
 Summary: Conan Server of Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Description: <picture>
           <!-- These are also used for https://github.com/conan-io/.github/blob/main/profile/README.md -->
```

### Comparing `conan-server-2.3.1/conan_server.egg-info/SOURCES.txt` & `conan-server-2.3.2/conan_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conan_server.egg-info/requires.txt` & `conan-server-2.3.2/conan_server.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/cache/cache.py` & `conan-server-2.3.2/conans/client/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/cache/editable.py` & `conan-server-2.3.2/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/cmd/export.py` & `conan-server-2.3.2/conans/client/cmd/export.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/cmd/uploader.py` & `conan-server-2.3.2/conans/client/cmd/uploader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conanfile/build.py` & `conan-server-2.3.2/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conanfile/configure.py` & `conan-server-2.3.2/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conanfile/implementations.py` & `conan-server-2.3.2/conans/client/conanfile/implementations.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conanfile/package.py` & `conan-server-2.3.2/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conf/__init__.py` & `conan-server-2.3.2/conans/client/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conf/config_installer.py` & `conan-server-2.3.2/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conf/detect.py` & `conan-server-2.3.2/conans/client/conf/detect.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conf/detect_vs.py` & `conan-server-2.3.2/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/conf/required_version.py` & `conan-server-2.3.2/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/downloaders/caching_file_downloader.py` & `conan-server-2.3.2/conans/client/downloaders/caching_file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/downloaders/download_cache.py` & `conan-server-2.3.2/conans/client/downloaders/download_cache.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/downloaders/file_downloader.py` & `conan-server-2.3.2/conans/client/downloaders/file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/generators/__init__.py` & `conan-server-2.3.2/conans/client/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/build_mode.py` & `conan-server-2.3.2/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/compatibility.py` & `conan-server-2.3.2/conans/client/graph/compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         return []
     base = dict(conanfile.settings.values_list)
     factors = []  # List of list, each sublist is a potential combination
     if cppstd is not None and extension_properties.get("compatibility_cppstd") is not False:
         cppstd_possible_values = supported_cppstd(conanfile)
         if cppstd_possible_values is None:
             conanfile.output.warning(f'No cppstd compatibility defined for compiler "{compiler}"')
-        else:
-            factors.append([{"compiler.cppstd": v} for v in cppstd_possible_values if v != cppstd])
+        else: # The current cppst must be included in case there is other factor
+            factors.append([{"compiler.cppstd": v} for v in cppstd_possible_values])
 
     if compiler == "msvc":
         msvc_fallback = {"194": "193"}.get(compiler_version)
         if msvc_fallback:
             factors.append([{"compiler.version": msvc_fallback}])
 
     combinations = []
```

### Comparing `conan-server-2.3.1/conans/client/graph/compute_pid.py` & `conan-server-2.3.2/conans/client/graph/compute_pid.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/graph.py` & `conan-server-2.3.2/conans/client/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/graph_binaries.py` & `conan-server-2.3.2/conans/client/graph/graph_binaries.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/graph_builder.py` & `conan-server-2.3.2/conans/client/graph/graph_builder.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/graph_error.py` & `conan-server-2.3.2/conans/client/graph/graph_error.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/install_graph.py` & `conan-server-2.3.2/conans/client/graph/install_graph.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/profile_node_definer.py` & `conan-server-2.3.2/conans/client/graph/profile_node_definer.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/provides.py` & `conan-server-2.3.2/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/proxy.py` & `conan-server-2.3.2/conans/client/graph/proxy.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/python_requires.py` & `conan-server-2.3.2/conans/client/graph/python_requires.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/graph/range_resolver.py` & `conan-server-2.3.2/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/hook_manager.py` & `conan-server-2.3.2/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/installer.py` & `conan-server-2.3.2/conans/client/installer.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/loader.py` & `conan-server-2.3.2/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/loader_txt.py` & `conan-server-2.3.2/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/migrations.py` & `conan-server-2.3.2/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/pkg_sign.py` & `conan-server-2.3.2/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/profile_loader.py` & `conan-server-2.3.2/conans/client/profile_loader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/remote_manager.py` & `conan-server-2.3.2/conans/client/remote_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/__init__.py` & `conan-server-2.3.2/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/auth_manager.py` & `conan-server-2.3.2/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/client_routes.py` & `conan-server-2.3.2/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/conan_requester.py` & `conan-server-2.3.2/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/file_uploader.py` & `conan-server-2.3.2/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/remote_credentials.py` & `conan-server-2.3.2/conans/client/rest/remote_credentials.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/rest_client.py` & `conan-server-2.3.2/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/rest_client_common.py` & `conan-server-2.3.2/conans/client/rest/rest_client_common.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest/rest_client_v2.py` & `conan-server-2.3.2/conans/client/rest/rest_client_v2.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/rest_client_local_recipe_index.py` & `conan-server-2.3.2/conans/client/rest_client_local_recipe_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,17 @@
         name_pattern = pattern.split("/", 1)[0]
         recipes_dir = os.path.join(self._base_folder, "recipes")
         recipes = os.listdir(recipes_dir)
         recipes.sort()
         ret = []
         excluded = set()
         for r in recipes:
+            if r.startswith("."):
+                # Skip hidden folders, no recipes should start with a dot
+                continue
             if not fnmatch(r, name_pattern):
                 continue
             folder = self._get_base_folder(r)
             config_yml = self._load_config_yml(folder)
             if config_yml is None:
                 raise ConanException(f"Corrupted repo, folder {r} without 'config.yml'")
             versions = config_yml["versions"]
```

### Comparing `conan-server-2.3.1/conans/client/source.py` & `conan-server-2.3.2/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/store/localdb.py` & `conan-server-2.3.2/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/subsystems.py` & `conan-server-2.3.2/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/client/userio.py` & `conan-server-2.3.2/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/conan_server.py` & `conan-server-2.3.2/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/errors.py` & `conan-server-2.3.2/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/migrations.py` & `conan-server-2.3.2/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/build_info.py` & `conan-server-2.3.2/conans/model/build_info.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/conan_file.py` & `conan-server-2.3.2/conans/model/conan_file.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/conanfile_interface.py` & `conan-server-2.3.2/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/conf.py` & `conan-server-2.3.2/conans/model/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     "tools.gnu:build_triplet": "Custom build triplet to pass to Autotools scripts",
     "tools.gnu:host_triplet": "Custom host triplet to pass to Autotools scripts",
     "tools.google.bazel:configs": "List of Bazel configurations to be used as 'bazel build --config=config1 ...'",
     "tools.google.bazel:bazelrc_path": "List of paths to bazelrc files to be used as 'bazel --bazelrc=rcpath1 ... build'",
     "tools.meson.mesontoolchain:backend": "Any Meson backend: ninja, vs, vs2010, vs2012, vs2013, vs2015, vs2017, vs2019, xcode",
     "tools.meson.mesontoolchain:extra_machine_files": "List of paths for any additional native/cross file references to be appended to the existing Conan ones",
     "tools.microsoft:winsdk_version": "Use this winsdk_version in vcvars",
+    "tools.microsoft:msvc_update": "Force the specific update irrespective of compiler.update (CMakeToolchain and VCVars)",
     "tools.microsoft.msbuild:vs_version": "Defines the IDE version (15, 16, 17) when using the msvc compiler. Necessary if compiler.version specifies a toolset that is not the IDE default",
     "tools.microsoft.msbuild:max_cpu_count": "Argument for the /m when running msvc to build parallel projects",
     "tools.microsoft.msbuild:installation_path": "VS install path, to avoid auto-detect via vswhere, like C:/Program Files (x86)/Microsoft Visual Studio/2019/Community. Use empty string to disable",
     "tools.microsoft.msbuilddeps:exclude_code_analysis": "Suppress MSBuild code analysis for patterns",
     "tools.microsoft.msbuildtoolchain:compile_options": "Dictionary with MSBuild compiler options",
     "tools.microsoft.bash:subsystem": "The subsystem to be used when conanfile.win_bash==True. Possible values: msys2, msys, cygwin, wsl, sfu",
     "tools.microsoft.bash:path": "The path to the shell to run when conanfile.win_bash==True",
```

### Comparing `conan-server-2.3.1/conans/model/dependencies.py` & `conan-server-2.3.2/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/graph_lock.py` & `conan-server-2.3.2/conans/model/graph_lock.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/info.py` & `conan-server-2.3.2/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/layout.py` & `conan-server-2.3.2/conans/model/layout.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/manifest.py` & `conan-server-2.3.2/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/options.py` & `conan-server-2.3.2/conans/model/options.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/package_ref.py` & `conan-server-2.3.2/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/pkg_type.py` & `conan-server-2.3.2/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/profile.py` & `conan-server-2.3.2/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/recipe_ref.py` & `conan-server-2.3.2/conans/model/recipe_ref.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/requires.py` & `conan-server-2.3.2/conans/model/requires.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/rest_routes.py` & `conan-server-2.3.2/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/settings.py` & `conan-server-2.3.2/conans/model/settings.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/version.py` & `conan-server-2.3.2/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/model/version_range.py` & `conan-server-2.3.2/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/paths/__init__.py` & `conan-server-2.3.2/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/search/query_parse.py` & `conan-server-2.3.2/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/search/search.py` & `conan-server-2.3.2/conans/search/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/conf/__init__.py` & `conan-server-2.3.2/conans/server/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/conf/default_server_conf.py` & `conan-server-2.3.2/conans/server/conf/default_server_conf.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/crypto/jwt/jwt_credentials_manager.py` & `conan-server-2.3.2/conans/server/crypto/jwt/jwt_credentials_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/crypto/jwt/jwt_manager.py` & `conan-server-2.3.2/conans/server/crypto/jwt/jwt_manager.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/launcher.py` & `conan-server-2.3.2/conans/server/launcher.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/migrate.py` & `conan-server-2.3.2/conans/server/migrate.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/plugin_loader.py` & `conan-server-2.3.2/conans/server/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/api_v2.py` & `conan-server-2.3.2/conans/server/rest/api_v2.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/bottle_plugins/authorization_header.py` & `conan-server-2.3.2/conans/server/rest/bottle_plugins/authorization_header.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/bottle_plugins/http_basic_authentication.py` & `conan-server-2.3.2/conans/server/rest/bottle_plugins/http_basic_authentication.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/bottle_plugins/jwt_authentication.py` & `conan-server-2.3.2/conans/server/rest/bottle_plugins/jwt_authentication.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/bottle_plugins/return_handler.py` & `conan-server-2.3.2/conans/server/rest/bottle_plugins/return_handler.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/controller/v2/conan.py` & `conan-server-2.3.2/conans/server/rest/controller/v2/conan.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/controller/v2/delete.py` & `conan-server-2.3.2/conans/server/rest/controller/v2/delete.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/controller/v2/revisions.py` & `conan-server-2.3.2/conans/server/rest/controller/v2/revisions.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/controller/v2/search.py` & `conan-server-2.3.2/conans/server/rest/controller/v2/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/controller/v2/users.py` & `conan-server-2.3.2/conans/server/rest/controller/v2/users.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/rest/server.py` & `conan-server-2.3.2/conans/server/rest/server.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/revision_list.py` & `conan-server-2.3.2/conans/server/revision_list.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/service/authorize.py` & `conan-server-2.3.2/conans/server/service/authorize.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/service/user_service.py` & `conan-server-2.3.2/conans/server/service/user_service.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/service/v2/search.py` & `conan-server-2.3.2/conans/server/service/v2/search.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/service/v2/service_v2.py` & `conan-server-2.3.2/conans/server/service/v2/service_v2.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/store/disk_adapter.py` & `conan-server-2.3.2/conans/server/store/disk_adapter.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/store/server_store.py` & `conan-server-2.3.2/conans/server/store/server_store.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/server/utils/files.py` & `conan-server-2.3.2/conans/server/utils/files.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/assets/autotools.py` & `conan-server-2.3.2/conans/test/assets/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/assets/cmake.py` & `conan-server-2.3.2/conans/test/assets/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/assets/genconanfile.py` & `conan-server-2.3.2/conans/test/assets/genconanfile.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/assets/pkg_cmake.py` & `conan-server-2.3.2/conans/test/assets/pkg_cmake.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/assets/sources.py` & `conan-server-2.3.2/conans/test/assets/sources.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/assets/visual_project_files.py` & `conan-server-2.3.2/conans/test/assets/visual_project_files.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/conftest.py` & `conan-server-2.3.2/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/artifactory.py` & `conan-server-2.3.2/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/file_server.py` & `conan-server-2.3.2/conans/test/utils/file_server.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/mocks.py` & `conan-server-2.3.2/conans/test/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/profiles.py` & `conan-server-2.3.2/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/scm.py` & `conan-server-2.3.2/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/server_launcher.py` & `conan-server-2.3.2/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/test_files.py` & `conan-server-2.3.2/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/test/utils/tools.py` & `conan-server-2.3.2/conans/test/utils/tools.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/config_parser.py` & `conan-server-2.3.2/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/dates.py` & `conan-server-2.3.2/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/encrypt.py` & `conan-server-2.3.2/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/env.py` & `conan-server-2.3.2/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/files.py` & `conan-server-2.3.2/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/locks.py` & `conan-server-2.3.2/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/runners.py` & `conan-server-2.3.2/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/sha.py` & `conan-server-2.3.2/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/conans/util/windows.py` & `conan-server-2.3.2/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-server-2.3.1/setup.py` & `conan-server-2.3.2/setup.py`

 * *Files identical despite different names*

