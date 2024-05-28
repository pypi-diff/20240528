# Comparing `tmp/hexdoc_hexdebug-0.2.1.1.20.1.1.0.tar.gz` & `tmp/hexdoc_hexdebug-0.2.2.1.20.1.1.0.tar.gz`

## Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0.tar` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/gradle.properties
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/__version__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/__init__.py
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.patterns.hexdoc.json
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/empty.json
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/full.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/empty.json
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/full.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/empty.json
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/full.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/empty.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/full.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/empty.json
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/full.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/empty.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/full.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/empty.json
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/full.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/empty.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/full.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/empty.json
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/full.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/empty.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/full.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/empty.json
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/full.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/empty.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/full.json
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator/default.json
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator/modified.json
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger.png
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/evaluator.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/debug_state/debugging.png
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/evaluator/eval_state/modified.png
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/debugger.json
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/evaluator.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_templates/__init__.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/LICENSE
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.1.1.20.1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/gradle.properties
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/__gradle_version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/__version__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/py.typed
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/__init__.py
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.patterns.hexdoc.json
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0     7053 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/empty.json
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/continue/full.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/empty.json
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/in/full.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/empty.json
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/out/full.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/empty.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/over/full.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/empty.json
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/restart/full.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/empty.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/debugging/stop/full.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/empty.json
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/continue/full.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/empty.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/in/full.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/empty.json
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/out/full.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/empty.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/over/full.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/empty.json
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/restart/full.json
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/empty.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger/not_debugging/stop/full.json
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator/default.json
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/evaluator/modified.json
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger.png
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/evaluator.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/debug_state/debugging.png
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/evaluator/eval_state/modified.png
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/debugger.json
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/data/hexdebug/recipes/evaluator.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_templates/__init__.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/LICENSE
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/README.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 hexdoc_hexdebug-0.2.2.1.20.1.1.0/PKG-INFO
```

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/hexdebug.hexdoc.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6612723214285715%*

 * *Differences: {"'asset_url'": "'https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5'",*

 * * "'book_url'": "'https://hexdebug.hexxy.media/v/0.2.2+1.20.1/1.0/en_us'",*

 * * "'textures'": "{'PNGTexture': {'hexdebug:textures/item/evaluator.png': {'url': "*

 * *               "'https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/evaluator.png'}, "*

 * *               "'hexdebug:textures/item/debugge […]*

```diff
@@ -1,86 +1,86 @@
 {
-    "asset_url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc",
-    "book_url": "https://hexdebug.hexxy.media/v/0.2.1+1.20.1/1.0/en_us",
+    "asset_url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5",
+    "book_url": "https://hexdebug.hexxy.media/v/0.2.2+1.20.1/1.0/en_us",
     "textures": {
         "PNGTexture": {
             "hexdebug:textures/item/debugger.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
             },
             "hexdebug:textures/item/debugger/debug_state/debugging.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/debug_state/debugging.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/debug_state/debugging.png"
             },
             "hexdebug:textures/item/debugger/has_hex/full.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/has_hex/full.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/has_hex/full.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/continue.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/continue.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/in.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/in.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/out.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/out.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/over.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/over.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/restart.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/restart.png"
             },
             "hexdebug:textures/item/debugger/step_mode/debugging/stop.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/debugging/stop.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/continue.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/continue.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/in.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/in.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/out.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/out.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/over.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/over.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/restart.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/restart.png"
             },
             "hexdebug:textures/item/debugger/step_mode/not_debugging/stop.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger/step_mode/not_debugging/stop.png"
             },
             "hexdebug:textures/item/evaluator.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/evaluator.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/evaluator.png"
             },
             "hexdebug:textures/item/evaluator/eval_state/modified.png": {
                 "pixelated": true,
-                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/evaluator/eval_state/modified.png"
+                "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/evaluator/eval_state/modified.png"
             }
         },
         "SingleItemTexture": {
             "hexdebug:debugger": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/debugger.png"
                 }
             },
             "hexdebug:debugger/debugging/continue/empty": {
                 "inner": {
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
                 }
@@ -222,15 +222,15 @@
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
                 }
             },
             "hexdebug:evaluator": {
                 "inner": {
                     "pixelated": true,
-                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/64fc1c35eaa9581c62b06c5550d0f65812f2dcdc/Common/src/main/resources/assets/hexdebug/textures/item/evaluator.png"
+                    "url": "https://raw.githubusercontent.com/object-Object/HexDebug/604d184744524f6bd56ac9e24fb5e781bfa530e5/Common/src/main/resources/assets/hexdebug/textures/item/evaluator.png"
                 }
             },
             "hexdebug:evaluator/default": {
                 "inner": {
                     "pixelated": true,
                     "url": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAIAAACQkWg2AAAACXBIWXMAAC4jAAAuIwF4pT92AAAAJElEQVQoz2NkwAF+MPzAKs7EQCIY1UAMYMQV3hwMHKOhRD8NAPogBA/DVsDEAAAAAElFTkSuQmCC"
                 }
```

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/items/debugging.json5`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexcasting/patchouli_books/thehexbook/en_us/entries/patterns/debugging.json5`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/en_us.flatten.json5`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/lang/zh_cn.flatten.json5`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.85%*

 * *Differences: {"'text.autoconfig.hexdebug.option.client.debuggerDisplayMode'": "'调试杖显示模式'",*

 * * "'text.autoconfig.hexdebug.option.client.debuggerDisplayMode.@Tooltip'": "'更改调试杖打印下一需运行iota的时机。\\nDISABLED：不显示调试杖状态消息。\\nNOT_CONNECTED：只在调试客户端未连接时显示调试杖状态消息。\\nENABLED：一直显示调试杖状态信息。（默认）'",*

 * * "'text.autoconfig.hexdebug.option.client.showDebugClientLineNumber'": "'显示调试客户端行号'",*

 * * "'text.autoconfig.hexdebug.option.client.showDebugClientLineNumber.@Tooltip'": "'若设为true，显示调试客户端（如VSCode）的行号，通常以1起始；否则显示列表索引下标，以0起始。'",*

 * * "'text.hexdebug.debugg […]*

```diff
@@ -22,15 +22,21 @@
     "hexdebug.tooltip.debugger.step_mode.stop": "\u505c\u6b62",
     "item.hexdebug.debugger": "\u8c03\u8bd5\u6756",
     "item.hexdebug.evaluator": "\u8fd0\u884c\u6756",
     "itemGroup.hexdebug": "\u5492\u6cd5\u8c03\u8bd5",
     "text.autoconfig.hexdebug.category.client": "\u5ba2\u6237\u7aef",
     "text.autoconfig.hexdebug.option.client.debugPort": "\u8c03\u8bd5\u7aef\u53e3",
     "text.autoconfig.hexdebug.option.client.debugPort.@Tooltip": "\u5f00\u653e\u4ee5\u8fde\u63a5\u81f3\u8c03\u8bd5\u5ba2\u6237\u7aef\uff08\u5982VSCode\uff09\u7684\u7aef\u53e3\u53f7\uff081024-65535\uff09\u3002",
+    "text.autoconfig.hexdebug.option.client.debuggerDisplayMode": "\u8c03\u8bd5\u6756\u663e\u793a\u6a21\u5f0f",
+    "text.autoconfig.hexdebug.option.client.debuggerDisplayMode.@Tooltip": "\u66f4\u6539\u8c03\u8bd5\u6756\u6253\u5370\u4e0b\u4e00\u9700\u8fd0\u884ciota\u7684\u65f6\u673a\u3002\nDISABLED\uff1a\u4e0d\u663e\u793a\u8c03\u8bd5\u6756\u72b6\u6001\u6d88\u606f\u3002\nNOT_CONNECTED\uff1a\u53ea\u5728\u8c03\u8bd5\u5ba2\u6237\u7aef\u672a\u8fde\u63a5\u65f6\u663e\u793a\u8c03\u8bd5\u6756\u72b6\u6001\u6d88\u606f\u3002\nENABLED\uff1a\u4e00\u76f4\u663e\u793a\u8c03\u8bd5\u6756\u72b6\u6001\u4fe1\u606f\u3002\uff08\u9ed8\u8ba4\uff09",
     "text.autoconfig.hexdebug.option.client.openDebugPort": "\u5f00\u653e\u8c03\u8bd5\u7aef\u53e3",
     "text.autoconfig.hexdebug.option.client.openDebugPort.@Tooltip": "\u662f\u5426\u5f00\u653e\u7aef\u53e3\u3002\u82e5\u8bbe\u4e3afalse\uff0c\u8c03\u8bd5\u6756\u4f1a\u5931\u53bb\u4f5c\u7528\u3002",
+    "text.autoconfig.hexdebug.option.client.showDebugClientLineNumber": "\u663e\u793a\u8c03\u8bd5\u5ba2\u6237\u7aef\u884c\u53f7",
+    "text.autoconfig.hexdebug.option.client.showDebugClientLineNumber.@Tooltip": "\u82e5\u8bbe\u4e3atrue\uff0c\u663e\u793a\u8c03\u8bd5\u5ba2\u6237\u7aef\uff08\u5982VSCode\uff09\u7684\u884c\u53f7\uff0c\u901a\u5e38\u4ee51\u8d77\u59cb\uff1b\u5426\u5219\u663e\u793a\u5217\u8868\u7d22\u5f15\u4e0b\u6807\uff0c\u4ee50\u8d77\u59cb\u3002",
     "text.autoconfig.hexdebug.option.client.smartDebuggerSneakScroll": "\u8c03\u8bd5\u6756\u667a\u80fd\u6f5c\u884c\u6eda\u8f6e",
     "text.autoconfig.hexdebug.option.client.smartDebuggerSneakScroll.@Tooltip": "\u82e5\u5f53\u524d\u4e3b\u624b\u6301\u6709\u8c03\u8bd5\u6756\uff0c\u4e14\u672a\u5728\u8c03\u8bd5\u5492\u672f\uff0c\u5219\u4f18\u5148\u5904\u7406\u526f\u624b\u4e2d\u6cd5\u672f\u4e66\u4e00\u7c7b\u7269\u54c1\u7684\u201c\u6f5c\u884c\u6eda\u52a8\u6eda\u8f6e\u201d\u64cd\u4f5c\u3002",
     "text.autoconfig.hexdebug.title": "\u5492\u6cd5\u8c03\u8bd5\u914d\u7f6e",
     "text.hexdebug.connected": "\u8c03\u8bd5\u5ba2\u6237\u7aef\u5df2\u8fde\u63a5\uff01",
+    "text.hexdebug.debugger_stopped": "\u4e0b\u4e00\u4e2aIota\uff1a[%d] %s",
+    "text.hexdebug.no_session": "\u8c03\u8bd5\u4f1a\u8bdd\u672a\u5728\u8fd0\u884c\u3002",
     "text.hexdebug.thwack": "\u54d0\u5f53\uff01"
 }
```

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/models/item/debugger.json`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/src/hexdoc_hexdebug/_export/generated/assets/hexdebug/textures/item/debugger/has_hex/full.png`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/.gitignore` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/LICENSE` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/pyproject.toml` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/doc/README.md` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_hexdebug-0.2.1.1.20.1.1.0/PKG-INFO` & `hexdoc_hexdebug-0.2.2.1.20.1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hexdoc-hexdebug
-Version: 0.2.1.1.20.1.1.0
+Version: 0.2.2.1.20.1.1.0
 Summary: Python web book docgen and hexdoc plugin for HexDebug.
 Project-URL: Homepage, https://hexdebug.hexxy.media
 Project-URL: Source, https://github.com/object-Object/HexDebug
 Author: object-Object
 License-File: LICENSE
 Keywords: hexdoc
 Requires-Python: >=3.11
```

