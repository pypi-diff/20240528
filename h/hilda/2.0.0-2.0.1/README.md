# Comparing `tmp/hilda-2.0.0.tar.gz` & `tmp/hilda-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hilda-2.0.0.tar", last modified: Thu May 23 11:19:32 2024, max compression
+gzip compressed data, was "hilda-2.0.1.tar", last modified: Tue May 28 06:23:37 2024, max compression
```

## Comparing `hilda-2.0.0.tar` & `hilda-2.0.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.664590 hilda-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.644590 hilda-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.648590 hilda-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-23 11:19:22.000000 hilda-2.0.0/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-23 11:19:22.000000 hilda-2.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-23 11:19:22.000000 hilda-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 11:19:22.000000 hilda-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 11:19:22.000000 hilda-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23605 2024-05-23 11:19:32.664590 hilda-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-05-23 11:19:22.000000 hilda-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.648590 hilda-2.0.0/gifs/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 11:19:22.000000 hilda-2.0.0/gifs/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 11:19:22.000000 hilda-2.0.0/gifs/ui.png
--rw-r--r--   0 runner    (1001) docker     (127)   939935 2024-05-23 11:19:22.000000 hilda-2.0.0/gifs/xpc_print_message.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.652590 hilda-2.0.0/hilda/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)   120119 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/hilda_ascii_art.html
--rw-r--r--   0 runner    (1001) docker     (127)    43606 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/hilda_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.656590 hilda-2.0.0/hilda/ipython_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ipython_extensions/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ipython_extensions/keybindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ipython_extensions/magics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/launch_lldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/lldb_entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/lldb_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.656590 hilda-2.0.0/hilda/objective_c/
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/from_ns_to_json.m
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/get_objectivec_class_by_module.m
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/get_objectivec_class_description.m
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/get_objectivec_symbol_data.m
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/lsof.m
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c/to_ns_from_json.m
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.656590 hilda-2.0.0/hilda/snippets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/boringssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/dyld.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/fs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda/snippets/mach/
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/mach/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda/snippets/macho/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/all_image_infos.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/apple_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/image_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/macho.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/macho/macho_load_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/remotepairingd.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/snippets/xpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/symbols_jar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ui/colors.json
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ui/ui_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-23 11:19:22.000000 hilda-2.0.0/hilda/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/hilda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23605 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 11:19:32.000000 hilda-2.0.0/hilda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-23 11:19:22.000000 hilda-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-23 11:19:22.000000 hilda-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:19:32.664590 hilda-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/test_hilda_client/
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_from_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_hilda_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_ns.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_rebind_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_hilda_client/test_registers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/test_snippets/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_snippets/test_xpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:19:32.660590 hilda-2.0.0/tests/test_symbols/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-23 11:19:22.000000 hilda-2.0.0/tests/test_symbols/test_symbols_jar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.636577 hilda-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.620577 hilda-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.624577 hilda-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 06:23:22.000000 hilda-2.0.1/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-28 06:23:22.000000 hilda-2.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-28 06:23:22.000000 hilda-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 06:23:22.000000 hilda-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-28 06:23:22.000000 hilda-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23605 2024-05-28 06:23:37.636577 hilda-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20910 2024-05-28 06:23:22.000000 hilda-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.624577 hilda-2.0.1/gifs/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-28 06:23:22.000000 hilda-2.0.1/gifs/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 06:23:23.000000 hilda-2.0.1/gifs/ui.png
+-rw-r--r--   0 runner    (1001) docker     (127)   939935 2024-05-28 06:23:23.000000 hilda-2.0.1/gifs/xpc_print_message.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.628577 hilda-2.0.1/hilda/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-28 06:23:37.000000 hilda-2.0.1/hilda/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120119 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/hilda_ascii_art.html
+-rw-r--r--   0 runner    (1001) docker     (127)    43486 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/hilda_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.632577 hilda-2.0.1/hilda/ipython_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/ipython_extensions/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/ipython_extensions/keybindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/ipython_extensions/magics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/launch_lldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/lldb_entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/lldb_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.632577 hilda-2.0.1/hilda/objective_c/
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c/from_ns_to_json.m
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c/get_objectivec_class_by_module.m
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c/get_objectivec_class_description.m
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c/get_objectivec_symbol_data.m
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c/lsof.m
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c/to_ns_from_json.m
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.632577 hilda-2.0.1/hilda/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/boringssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/dyld.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/fs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.632577 hilda-2.0.1/hilda/snippets/mach/
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/mach/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.632577 hilda-2.0.1/hilda/snippets/macho/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/macho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/macho/all_image_infos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/macho/apple_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/macho/image_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/macho/macho.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/macho/macho_load_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/remotepairingd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/snippets/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/symbols_jar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.636577 hilda-2.0.1/hilda/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/ui/colors.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/ui/ui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-05-28 06:23:23.000000 hilda-2.0.1/hilda/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.636577 hilda-2.0.1/hilda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23605 2024-05-28 06:23:37.000000 hilda-2.0.1/hilda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-28 06:23:37.000000 hilda-2.0.1/hilda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:23:37.000000 hilda-2.0.1/hilda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-28 06:23:37.000000 hilda-2.0.1/hilda.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 06:23:37.000000 hilda-2.0.1/hilda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 06:23:37.000000 hilda-2.0.1/hilda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-28 06:23:23.000000 hilda-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-28 06:23:23.000000 hilda-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:23:37.636577 hilda-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.636577 hilda-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.636577 hilda-2.0.1/tests/test_hilda_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_hilda_client/test_from_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_hilda_client/test_hilda_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_hilda_client/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_hilda_client/test_ns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_hilda_client/test_rebind_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_hilda_client/test_registers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.636577 hilda-2.0.1/tests/test_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_snippets/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:23:37.636577 hilda-2.0.1/tests/test_symbols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_symbols/test_objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_symbols/test_objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_symbols/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-28 06:23:23.000000 hilda-2.0.1/tests/test_symbols/test_symbols_jar.py
```

### Comparing `hilda-2.0.0/.github/workflows/python-app.yml` & `hilda-2.0.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/.github/workflows/python-publish.yml` & `hilda-2.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/.gitignore` & `hilda-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/LICENSE` & `hilda-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/PKG-INFO` & `hilda-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 2.0.0
+Version: 2.0.1
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `hilda-2.0.0/README.md` & `hilda-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/gifs/xpc_print_message.gif` & `hilda-2.0.1/gifs/xpc_print_message.gif`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/cli.py` & `hilda-2.0.1/hilda/cli.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/exceptions.py` & `hilda-2.0.1/hilda/exceptions.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/hilda_ascii_art.html` & `hilda-2.0.1/hilda/hilda_ascii_art.html`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/hilda_client.py` & `hilda-2.0.1/hilda/hilda_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,16 +336,14 @@
         is_running = self.process.GetState() == lldb.eStateRunning
         if not is_running:
             self.log_debug('already stopped')
             return
 
         if not self.process.Stop().Success():
             self.log_critical('failed to stop process')
-        else:
-            self.log_info('Process Stopped')
 
     def cont(self, *args) -> None:
         """ Continue process. """
         is_running = self.process.GetState() == lldb.eStateRunning
 
         if is_running:
             self.log_debug('already running')
@@ -353,16 +351,14 @@
 
         # bugfix:   the debugger may become in sync state, so we make sure
         #           it isn't before trying to continue
         self.debugger.SetAsync(True)
 
         if not self.process.Continue().Success():
             self.log_critical('failed to continue process')
-        else:
-            self.log_info('Process Continued')
 
     def detach(self):
         """
         Detach from process.
 
         Useful in order to exit gracefully so process doesn't get killed
         while you exit
```

### Comparing `hilda-2.0.0/hilda/ipython_extensions/events.py` & `hilda-2.0.1/hilda/ipython_extensions/events.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/ipython_extensions/keybindings.py` & `hilda-2.0.1/hilda/ipython_extensions/keybindings.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 def load_ipython_extension(ipython):
     def register_keybindings():
         hilda = ipython.user_ns['p']
         keys_mapping = {Keys.F7: hilda.step_into,
                         Keys.F8: hilda.step_over,
-                        Keys.F9: hilda.cont,
-                        Keys.F10: hilda.stop}
+                        Keys.F9: lambda _: (hilda.log_info('Sending continue'), hilda.cont()),
+                        Keys.F10: lambda _: (hilda.log_info('Sending stop'), hilda.stop())}
 
         insert_mode = ViInsertMode() | EmacsInsertMode()
         registry = ipython.pt_app.key_bindings
 
         for key, callback in keys_mapping.items():
             registry.add_binding(key, filter=(HasFocus(DEFAULT_BUFFER) & ~HasSelection() & insert_mode))(
                 callback)
```

### Comparing `hilda-2.0.0/hilda/ipython_extensions/magics.py` & `hilda-2.0.1/hilda/ipython_extensions/magics.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/launch_lldb.py` & `hilda-2.0.1/hilda/launch_lldb.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/lldb_entrypoint.py` & `hilda-2.0.1/hilda/lldb_entrypoint.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/lldb_importer.py` & `hilda-2.0.1/hilda/lldb_importer.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c/from_ns_to_json.m` & `hilda-2.0.1/hilda/objective_c/from_ns_to_json.m`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c/get_objectivec_class_by_module.m` & `hilda-2.0.1/hilda/objective_c/get_objectivec_class_by_module.m`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c/get_objectivec_class_description.m` & `hilda-2.0.1/hilda/objective_c/get_objectivec_class_description.m`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c/get_objectivec_symbol_data.m` & `hilda-2.0.1/hilda/objective_c/get_objectivec_symbol_data.m`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c/lsof.m` & `hilda-2.0.1/hilda/objective_c/lsof.m`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c/to_ns_from_json.m` & `hilda-2.0.1/hilda/objective_c/to_ns_from_json.m`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c_class.py` & `hilda-2.0.1/hilda/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/objective_c_symbol.py` & `hilda-2.0.1/hilda/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/registers.py` & `hilda-2.0.1/hilda/registers.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/boringssl.py` & `hilda-2.0.1/hilda/snippets/boringssl.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/dyld.py` & `hilda-2.0.1/hilda/snippets/dyld.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py` & `hilda-2.0.1/hilda/snippets/mach/CFRunLoopServiceMachPort_hooks.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/macho/all_image_infos.py` & `hilda-2.0.1/hilda/snippets/macho/all_image_infos.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/macho/image_info.py` & `hilda-2.0.1/hilda/snippets/macho/image_info.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/macho/macho.py` & `hilda-2.0.1/hilda/snippets/macho/macho.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/macho/macho_load_commands.py` & `hilda-2.0.1/hilda/snippets/macho/macho_load_commands.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/remotepairingd.py` & `hilda-2.0.1/hilda/snippets/remotepairingd.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/snippets/xpc.py` & `hilda-2.0.1/hilda/snippets/xpc.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/symbol.py` & `hilda-2.0.1/hilda/symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/symbols_jar.py` & `hilda-2.0.1/hilda/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/ui/ui_manager.py` & `hilda-2.0.1/hilda/ui/ui_manager.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda/ui/views.py` & `hilda-2.0.1/hilda/ui/views.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/hilda.egg-info/PKG-INFO` & `hilda-2.0.1/hilda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hilda
-Version: 2.0.0
+Version: 2.0.1
 Summary: LLDB wrapped and empowered by iPython's features
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>, netanel cohen <netanelc305@protonmail.com>
 License: Copyright (c) 2012-2023 Doron Zarhi and Metan Perelman
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `hilda-2.0.0/hilda.egg-info/SOURCES.txt` & `hilda-2.0.1/hilda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/pyproject.toml` & `hilda-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/conftest.py` & `hilda-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_hilda_client/test_from_ns.py` & `hilda-2.0.1/tests/test_hilda_client/test_from_ns.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_hilda_client/test_hilda_client.py` & `hilda-2.0.1/tests/test_hilda_client/test_hilda_client.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_hilda_client/test_monitor.py` & `hilda-2.0.1/tests/test_hilda_client/test_monitor.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_hilda_client/test_ns.py` & `hilda-2.0.1/tests/test_hilda_client/test_ns.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_hilda_client/test_registers.py` & `hilda-2.0.1/tests/test_hilda_client/test_registers.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_snippets/test_xpc.py` & `hilda-2.0.1/tests/test_snippets/test_xpc.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_symbols/test_objective_c_class.py` & `hilda-2.0.1/tests/test_symbols/test_objective_c_class.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_symbols/test_objective_c_symbol.py` & `hilda-2.0.1/tests/test_symbols/test_objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_symbols/test_symbol.py` & `hilda-2.0.1/tests/test_symbols/test_symbol.py`

 * *Files identical despite different names*

### Comparing `hilda-2.0.0/tests/test_symbols/test_symbols_jar.py` & `hilda-2.0.1/tests/test_symbols/test_symbols_jar.py`

 * *Files identical despite different names*

