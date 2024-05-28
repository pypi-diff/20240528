# Comparing `tmp/lean_dojo-1.8.2.tar.gz` & `tmp/lean_dojo-1.9.0.tar.gz`

## Comparing `lean_dojo-1.8.2.tar` & `lean_dojo-1.9.0.tar`

### file list

```diff
@@ -1,31 +1,948 @@
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/.readthedocs.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/mypy.ini
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/constants.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/container.py
--rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/utils.py
--rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/data_extraction/ExtractData.lean
--rw-r--r--   0        0        0    48595 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/data_extraction/ast.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/data_extraction/build_lean4_repo.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/data_extraction/cache.py
--rw-r--r--   0        0        0    20689 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/data_extraction/lean.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/data_extraction/trace.py
--rw-r--r--   0        0        0    43534 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/data_extraction/traced_data.py
--rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/interaction/Lean4Repl.lean
--rw-r--r--   0        0        0    18147 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/interaction/dojo.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/src/lean_dojo/interaction/parse_goals.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/__init__.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/conftest.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/data_extraction/test_trace.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/interaction/test_commands.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/interaction/test_imports.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/interaction/test_init_errors.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/interaction/test_parse_goals.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/interaction/test_sorry.py
--rw-r--r--   0        0        0    10353 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/interaction/test_tactics.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/tests/interaction/test_timeout.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/LICENSE
--rw-r--r--   0        0        0     5061 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/README.md
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     7897 2020-02-02 00:00:00.000000 lean_dojo-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/mypy.ini
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/nohup.out
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/__init__.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/constants.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/container.py
+-rw-r--r--   0        0        0     9987 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/utils.py
+-rw-r--r--   0        0        0    17695 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/data_extraction/ExtractData.lean
+-rw-r--r--   0        0        0    50220 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/data_extraction/ast.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/data_extraction/build_lean4_repo.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/data_extraction/cache.py
+-rw-r--r--   0        0        0    22650 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/data_extraction/lean.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/data_extraction/trace.py
+-rw-r--r--   0        0        0    43616 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/data_extraction/traced_data.py
+-rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/interaction/Lean4Repl.lean
+-rw-r--r--   0        0        0    18213 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/interaction/dojo.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/src/lean_dojo/interaction/parse_goals.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/data_extraction/test_trace.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/interaction/test_commands.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/interaction/test_imports.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/interaction/test_init_errors.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/interaction/test_parse_goals.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/interaction/test_sorry.py
+-rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/interaction/test_tactics.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/tests/interaction/test_timeout.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.gitignore
+-rw-r--r--   0        0        0    17754 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/ExtractData.lean
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/LICENSE
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/Lean4Example.lean
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/README.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/lake-manifest.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/lakefile.lean
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/lean-toolchain
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/lakefile.olean.trace
+-rw-r--r--   0        0        0     9160 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/LICENSE
+-rw-r--r--   0        0        0    68500 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/LICENSES
+-rwxr-xr-x   0        0        0   171397 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/bin/clang
+-rwxr-xr-x   0        0        0  3330656 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/bin/lake
+-rwxr-xr-x   0        0        0  4434480 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/bin/ld64.lld
+-rwxr-xr-x   0        0        0    49968 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/bin/lean
+-rwxr-xr-x   0        0        0    71936 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/bin/leanc
+-rwxr-xr-x   0        0        0      839 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/bin/leanmake
+-rwxr-xr-x   0        0        0   104404 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/bin/llvm-ar
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/__stddef_max_align_t.h
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/limits.h
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/stdalign.h
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/stdarg.h
+-rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/stdatomic.h
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/stdbool.h
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/stddef.h
+-rw-r--r--   0        0        0    29742 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/stdint.h
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/clang/stdnoreturn.h
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/lean/config.h
+-rw-r--r--   0        0        0    86140 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/lean/lean.h
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/lean/lean_gmp.h
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/include/lean/version.h
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/share/lean/lean.mk
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init.lean
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean.lean
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Leanc.lean
+-rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/BinderPredicates.lean
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/ByCases.lean
+-rw-r--r--   0        0        0     6710 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Classical.lean
+-rw-r--r--   0        0        0    13505 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Coe.lean
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control.lean
+-rw-r--r--   0        0        0    13544 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Conv.lean
+-rw-r--r--   0        0        0    78862 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Core.lean
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data.lean
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Dynamic.lean
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Ext.lean
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Guard.lean
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Hints.lean
+-rw-r--r--   0        0        0    51156 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Meta.lean
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/MetaTypes.lean
+-rw-r--r--   0        0        0    25435 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Notation.lean
+-rw-r--r--   0        0        0    18682 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/NotationExtra.lean
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Omega.lean
+-rw-r--r--   0        0        0   181567 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Prelude.lean
+-rw-r--r--   0        0        0    20846 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/PropLemmas.lean
+-rw-r--r--   0        0        0     9802 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/RCases.lean
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/ShareCommon.lean
+-rw-r--r--   0        0        0    13946 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/SimpLemmas.lean
+-rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Simproc.lean
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/SizeOf.lean
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/SizeOfLemmas.lean
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System.lean
+-rw-r--r--   0        0        0    62722 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Tactics.lean
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/TacticsExtra.lean
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Util.lean
+-rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/WF.lean
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/WFTactics.lean
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/Basic.lean
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/EState.lean
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/Except.lean
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/ExceptCps.lean
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/Id.lean
+-rw-r--r--   0        0        0    17278 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/Lawful.lean
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/Option.lean
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/Reader.lean
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/State.lean
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/StateCps.lean
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Control/StateRef.lean
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/AC.lean
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array.lean
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Basic.lean
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/BitVec.lean
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Bool.lean
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/ByteArray.lean
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Cast.lean
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Channel.lean
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Char.lean
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Fin.lean
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Float.lean
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/FloatArray.lean
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Format.lean
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Hashable.lean
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int.lean
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/List.lean
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat.lean
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/OfScientific.lean
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Option.lean
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Ord.lean
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Prod.lean
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Queue.lean
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Random.lean
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Range.lean
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Repr.lean
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Stream.lean
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/String.lean
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Sum.lean
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/ToString.lean
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/UInt.lean
+-rw-r--r--   0        0        0    30554 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/Basic.lean
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/BasicAux.lean
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/BinSearch.lean
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/DecidableEq.lean
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/InsertionSort.lean
+-rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/Lemmas.lean
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/Mem.lean
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/QSort.lean
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Array/Subarray.lean
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/BitVec/Basic.lean
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/BitVec/Bitblast.lean
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/BitVec/Folds.lean
+-rw-r--r--   0        0        0    24498 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/BitVec/Lemmas.lean
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/ByteArray/Basic.lean
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Char/Basic.lean
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Fin/Basic.lean
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Fin/Fold.lean
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Fin/Iterate.lean
+-rw-r--r--   0        0        0    36476 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Fin/Lemmas.lean
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Fin/Log2.lean
+-rw-r--r--   0        0        0     5578 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/FloatArray/Basic.lean
+-rw-r--r--   0        0        0    12796 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Format/Basic.lean
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Format/Instances.lean
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Format/Macro.lean
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Format/Syntax.lean
+-rw-r--r--   0        0        0     9820 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int/Basic.lean
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int/Bitwise.lean
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int/DivMod.lean
+-rw-r--r--   0        0        0    16255 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int/DivModLemmas.lean
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int/Gcd.lean
+-rw-r--r--   0        0        0    22782 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int/Lemmas.lean
+-rw-r--r--   0        0        0    20749 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Int/Order.lean
+-rw-r--r--   0        0        0    32666 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/List/Basic.lean
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/List/BasicAux.lean
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/List/Control.lean
+-rw-r--r--   0        0        0    27971 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/List/Lemmas.lean
+-rw-r--r--   0        0        0    33724 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Basic.lean
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Bitwise.lean
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Control.lean
+-rw-r--r--   0        0        0    12049 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Div.lean
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Dvd.lean
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Gcd.lean
+-rw-r--r--   0        0        0    44456 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Lemmas.lean
+-rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Linear.lean
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Log2.lean
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/MinMax.lean
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Mod.lean
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Power2.lean
+-rw-r--r--   0        0        0     6775 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/SOM.lean
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Bitwise/Basic.lean
+-rw-r--r--   0        0        0    16338 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Nat/Bitwise/Lemmas.lean
+-rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Option/Basic.lean
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Option/BasicAux.lean
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Option/Instances.lean
+-rw-r--r--   0        0        0     9474 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/Option/Lemmas.lean
+-rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/String/Basic.lean
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/String/Extra.lean
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/ToString/Basic.lean
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/ToString/Macro.lean
+-rw-r--r--   0        0        0    15504 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/UInt/Basic.lean
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Data/UInt/Log2.lean
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Omega/Coeffs.lean
+-rw-r--r--   0        0        0    15612 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Omega/Constraint.lean
+-rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Omega/Int.lean
+-rw-r--r--   0        0        0    14375 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Omega/IntList.lean
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Omega/LinearCombo.lean
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/Omega/Logic.lean
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/FilePath.lean
+-rw-r--r--   0        0        0    29775 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/IO.lean
+-rw-r--r--   0        0        0     8953 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/IOError.lean
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/Mutex.lean
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/Platform.lean
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/Promise.lean
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/ST.lean
+-rw-r--r--   0        0        0     4578 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Init/System/Uri.lean
+-rw-r--r--   0        0        0    20493 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Attributes.lean
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/AuxRecursor.lean
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Class.lean
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler.lean
+-rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/CoreM.lean
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data.lean
+-rw-r--r--   0        0        0    17173 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Declaration.lean
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/DeclarationRange.lean
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/DocString.lean
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab.lean
+-rw-r--r--   0        0        0    44635 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Environment.lean
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Eval.lean
+-rw-r--r--   0        0        0     6555 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Exception.lean
+-rw-r--r--   0        0        0    72559 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Expr.lean
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/HeadIndex.lean
+-rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Hygiene.lean
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ImportingFlag.lean
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/InternalExceptionId.lean
+-rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/KeyedDeclsAttribute.lean
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/LabelAttribute.lean
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/LazyInitExtension.lean
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Level.lean
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Linter.lean
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/LoadDynlib.lean
+-rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/LocalContext.lean
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Log.lean
+-rw-r--r--   0        0        0    17028 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Message.lean
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta.lean
+-rw-r--r--   0        0        0    69560 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/MetavarContext.lean
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Modifiers.lean
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/MonadEnv.lean
+-rw-r--r--   0        0        0     7732 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser.lean
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ParserCompiler.lean
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter.lean
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ProjFns.lean
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ReducibilityAttrs.lean
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Replay.lean
+-rw-r--r--   0        0        0    14760 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ResolveName.lean
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Runtime.lean
+-rw-r--r--   0        0        0     8549 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ScopedEnvExtension.lean
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server.lean
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Structure.lean
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/SubExpr.lean
+-rw-r--r--   0        0        0    21473 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Syntax.lean
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ToExpr.lean
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util.lean
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget.lean
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/AtMostOnce.lean
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/BorrowedAnnotation.lean
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/CSimpAttr.lean
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/ClosedTermCache.lean
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/ConstFolding.lean
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/ExportAttr.lean
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/ExternAttr.lean
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/FFI.lean
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR.lean
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/ImplementedByAttr.lean
+-rw-r--r--   0        0        0     6986 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/InitAttr.lean
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/InlineAttrs.lean
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF.lean
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/Main.lean
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/NameMangling.lean
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/NeverExtractAttr.lean
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/NoncomputableAttr.lean
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/Old.lean
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/Options.lean
+-rw-r--r--   0        0        0     5087 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/Specialize.lean
+-rw-r--r--   0        0        0    26469 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/Basic.lean
+-rw-r--r--   0        0        0    10899 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/Borrow.lean
+-rw-r--r--   0        0        0    13203 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/Boxing.lean
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/Checker.lean
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/CompilerM.lean
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/CtorLayout.lean
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/ElimDeadBranches.lean
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/ElimDeadVars.lean
+-rw-r--r--   0        0        0    26433 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/EmitC.lean
+-rw-r--r--   0        0        0    76684 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/EmitLLVM.lean
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/EmitUtil.lean
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/ExpandResetReuse.lean
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/Format.lean
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/FreeVars.lean
+-rw-r--r--   0        0        0    19176 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/LLVMBindings.lean
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/LiveVars.lean
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/NormIds.lean
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/PushProj.lean
+-rw-r--r--   0        0        0    12357 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/RC.lean
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/ResetReuse.lean
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/SimpCase.lean
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/Sorry.lean
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/IR/UnboxResult.lean
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/AlphaEqv.lean
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/AuxDeclCache.lean
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/BaseTypes.lean
+-rw-r--r--   0        0        0    25537 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Basic.lean
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Bind.lean
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/CSE.lean
+-rw-r--r--   0        0        0    12600 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Check.lean
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Closure.lean
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/CompatibleTypes.lean
+-rw-r--r--   0        0        0    18630 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/CompilerM.lean
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ConfigOptions.lean
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/DeclHash.lean
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/DependsOn.lean
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ElimDead.lean
+-rw-r--r--   0        0        0    20087 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ElimDeadBranches.lean
+-rw-r--r--   0        0        0     7887 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/FVarUtil.lean
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/FixedParams.lean
+-rw-r--r--   0        0        0    10066 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/FloatLetIn.lean
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ForEachExpr.lean
+-rw-r--r--   0        0        0    12695 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/InferType.lean
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Internalize.lean
+-rw-r--r--   0        0        0    22468 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/JoinPoints.lean
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/LCtx.lean
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/LambdaLifting.lean
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Level.lean
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Main.lean
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/MonadScope.lean
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/MonoTypes.lean
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/OtherDecl.lean
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/PassManager.lean
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Passes.lean
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/PhaseExt.lean
+-rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/PrettyPrinter.lean
+-rw-r--r--   0        0        0     7070 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Probing.lean
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/PullFunDecls.lean
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/PullLetDecls.lean
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ReduceArity.lean
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ReduceJpArity.lean
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Renaming.lean
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ScopeM.lean
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp.lean
+-rw-r--r--   0        0        0     8620 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/SpecInfo.lean
+-rw-r--r--   0        0        0    14450 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Specialize.lean
+-rw-r--r--   0        0        0     9838 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Testing.lean
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ToDecl.lean
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ToExpr.lean
+-rw-r--r--   0        0        0    28251 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ToLCNF.lean
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/ToMono.lean
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Types.lean
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Util.lean
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/Basic.lean
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/Config.lean
+-rw-r--r--   0        0        0    18034 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/ConstantFold.lean
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/DefaultAlt.lean
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/DiscrM.lean
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/FunDeclInfo.lean
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/InlineCandidate.lean
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/InlineProj.lean
+-rw-r--r--   0        0        0    12139 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/JpCases.lean
+-rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/Main.lean
+-rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/SimpM.lean
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/SimpValue.lean
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Compiler/LCNF/Simp/Used.lean
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Array.lean
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/AssocList.lean
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Format.lean
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/FuzzyMatching.lean
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/HashMap.lean
+-rw-r--r--   0        0        0     7419 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/HashSet.lean
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Json.lean
+-rw-r--r--   0        0        0    13560 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/JsonRpc.lean
+-rw-r--r--   0        0        0     8447 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/KVMap.lean
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/LBool.lean
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/LOption.lean
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp.lean
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Name.lean
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/NameMap.lean
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/NameTrie.lean
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/OpenDecl.lean
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Options.lean
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Parsec.lean
+-rw-r--r--   0        0        0    14248 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/PersistentArray.lean
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/PersistentHashMap.lean
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/PersistentHashSet.lean
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Position.lean
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/PrefixTree.lean
+-rw-r--r--   0        0        0    15461 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/RBMap.lean
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/RBTree.lean
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Rat.lean
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/SMap.lean
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/SSet.lean
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Trie.lean
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Xml.lean
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Json/Basic.lean
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Json/Elab.lean
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Json/FromToJson.lean
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Json/Parser.lean
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Json/Printer.lean
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Json/Stream.lean
+-rw-r--r--   0        0        0    16174 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Basic.lean
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Capabilities.lean
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Client.lean
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/CodeActions.lean
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Communication.lean
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Diagnostics.lean
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Extra.lean
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/InitShutdown.lean
+-rw-r--r--   0        0        0     6146 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Internal.lean
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Ipc.lean
+-rw-r--r--   0        0        0    11234 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/LanguageFeatures.lean
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/TextSync.lean
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Utf16.lean
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Lsp/Workspace.lean
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Xml/Basic.lean
+-rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Data/Xml/Parser.lean
+-rw-r--r--   0        0        0    70752 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/App.lean
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Arg.lean
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Attributes.lean
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/AutoBound.lean
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/AuxDef.lean
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/BinderPredicates.lean
+-rw-r--r--   0        0        0    32729 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Binders.lean
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/BindersUtil.lean
+-rw-r--r--   0        0        0    31000 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/BuiltinCommand.lean
+-rw-r--r--   0        0        0    22859 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/BuiltinNotation.lean
+-rw-r--r--   0        0        0    15353 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/BuiltinTerm.lean
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Calc.lean
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/CheckTactic.lean
+-rw-r--r--   0        0        0    23152 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Command.lean
+-rw-r--r--   0        0        0     9631 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/ComputedFields.lean
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Config.lean
+-rw-r--r--   0        0        0    10414 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/DeclModifiers.lean
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/DeclUtil.lean
+-rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Declaration.lean
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/DeclarationRange.lean
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/DefView.lean
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving.lean
+-rw-r--r--   0        0        0    78346 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Do.lean
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/ElabRules.lean
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Eval.lean
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Exception.lean
+-rw-r--r--   0        0        0    26071 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Extra.lean
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Frontend.lean
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/GenInjective.lean
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/GuardMsgs.lean
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Import.lean
+-rw-r--r--   0        0        0    40186 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Inductive.lean
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/InfoTree.lean
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/InheritDoc.lean
+-rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/LetRec.lean
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Level.lean
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Macro.lean
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/MacroArgUtil.lean
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/MacroRules.lean
+-rw-r--r--   0        0        0    58693 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Match.lean
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/MatchAltView.lean
+-rw-r--r--   0        0        0     7911 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/MatchExpr.lean
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Mixfix.lean
+-rw-r--r--   0        0        0    40286 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/MutualDef.lean
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Notation.lean
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Open.lean
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/ParseImportsFast.lean
+-rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PatternVar.lean
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition.lean
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Print.lean
+-rw-r--r--   0        0        0    34040 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Quotation.lean
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/RecAppSyntax.lean
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/SetOption.lean
+-rw-r--r--   0        0        0    40786 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/StructInst.lean
+-rw-r--r--   0        0        0    46120 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Structure.lean
+-rw-r--r--   0        0        0    18994 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Syntax.lean
+-rw-r--r--   0        0        0    24879 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/SyntheticMVars.lean
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic.lean
+-rw-r--r--   0        0        0    76399 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Term.lean
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Util.lean
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/BEq.lean
+-rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/Basic.lean
+-rw-r--r--   0        0        0     8976 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/DecEq.lean
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/FromToJson.lean
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/Hashable.lean
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/Inhabited.lean
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/Nonempty.lean
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/Ord.lean
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/Repr.lean
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/SizeOf.lean
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/TypeName.lean
+-rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Deriving/Util.lean
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/InfoTree/Main.lean
+-rw-r--r--   0        0        0     9572 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/InfoTree/Types.lean
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Basic.lean
+-rw-r--r--   0        0        0    16624 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Eqns.lean
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Main.lean
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/MkInhabitant.lean
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural.lean
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF.lean
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/BRecOn.lean
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/Basic.lean
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/Eqns.lean
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/FindRecArg.lean
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/IndPred.lean
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/Main.lean
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/Preprocess.lean
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/Structural/SmartUnfolding.lean
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/Eqns.lean
+-rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/Fix.lean
+-rw-r--r--   0        0        0    29288 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/GuessLex.lean
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/Ite.lean
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/Main.lean
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/PackDomain.lean
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/PackMutual.lean
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/Preprocess.lean
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/Rel.lean
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/PreDefinition/WF/TerminationHint.lean
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Quotation/Precheck.lean
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Quotation/Util.lean
+-rw-r--r--   0        0        0    16271 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Basic.lean
+-rw-r--r--   0        0        0    19642 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/BuiltinTactic.lean
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Cache.lean
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Calc.lean
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Change.lean
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Config.lean
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Congr.lean
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv.lean
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Delta.lean
+-rw-r--r--   0        0        0    19826 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/ElabTerm.lean
+-rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Ext.lean
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/FalseOrByContra.lean
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Generalize.lean
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Guard.lean
+-rw-r--r--   0        0        0    29755 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Induction.lean
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Injection.lean
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/LibrarySearch.lean
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Location.lean
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Match.lean
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Meta.lean
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/NormCast.lean
+-rw-r--r--   0        0        0     9419 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Omega.lean
+-rw-r--r--   0        0        0    25720 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/RCases.lean
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Repeat.lean
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Rewrite.lean
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/ShowTerm.lean
+-rw-r--r--   0        0        0    20371 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Simp.lean
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/SimpTrace.lean
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Simpa.lean
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Simproc.lean
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/SolveByElim.lean
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Split.lean
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Symm.lean
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Unfold.lean
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Basic.lean
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Change.lean
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Congr.lean
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Delta.lean
+-rw-r--r--   0        0        0     6093 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Pattern.lean
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Rewrite.lean
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Simp.lean
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Conv/Unfold.lean
+-rw-r--r--   0        0        0    21449 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Omega/Core.lean
+-rw-r--r--   0        0        0    26397 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Omega/Frontend.lean
+-rw-r--r--   0        0        0     5452 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Omega/MinNatAbs.lean
+-rw-r--r--   0        0        0    11000 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Elab/Tactic/Omega/OmegaM.lean
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Linter/Basic.lean
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Linter/Builtin.lean
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Linter/Deprecated.lean
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Linter/MissingDocs.lean
+-rw-r--r--   0        0        0    12443 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Linter/UnusedVariables.lean
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Linter/Util.lean
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/ACLt.lean
+-rw-r--r--   0        0        0     5918 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/AbstractMVars.lean
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/AbstractNestedProofs.lean
+-rw-r--r--   0        0        0    25891 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/AppBuilder.lean
+-rw-r--r--   0        0        0    75967 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Basic.lean
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Check.lean
+-rw-r--r--   0        0        0    15598 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Closure.lean
+-rw-r--r--   0        0        0     9465 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Coe.lean
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/CoeAttr.lean
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/CollectFVars.lean
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/CollectMVars.lean
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/CompletionName.lean
+-rw-r--r--   0        0        0    14824 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/CongrTheorems.lean
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Constructions.lean
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/CtorRecognizer.lean
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/DecLevel.lean
+-rw-r--r--   0        0        0    32644 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/DiscrTree.lean
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/DiscrTreeTypes.lean
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Eqns.lean
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Eval.lean
+-rw-r--r--   0        0        0    84880 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/ExprDefEq.lean
+-rw-r--r--   0        0        0     7885 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/ExprLens.lean
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/ExprTraverse.lean
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/ForEachExpr.lean
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/FunInfo.lean
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/GeneralizeTelescope.lean
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/GeneralizeVars.lean
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/GetUnfoldableConst.lean
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/GlobalInstances.lean
+-rw-r--r--   0        0        0    25934 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/IndPredBelow.lean
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Inductive.lean
+-rw-r--r--   0        0        0    17217 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/InferType.lean
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Injective.lean
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Instances.lean
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Iterator.lean
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/KAbstract.lean
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/KExprMap.lean
+-rw-r--r--   0        0        0    30172 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/LazyDiscrTree.lean
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/LevelDefEq.lean
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/LitValues.lean
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match.lean
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/MatchUtil.lean
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Offset.lean
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/PPGoal.lean
+-rw-r--r--   0        0        0    13476 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/RecursorInfo.lean
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Reduce.lean
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/ReduceEval.lean
+-rw-r--r--   0        0        0    23679 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/SizeOf.lean
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Structure.lean
+-rw-r--r--   0        0        0    34266 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/SynthInstance.lean
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic.lean
+-rw-r--r--   0        0        0     8399 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Transform.lean
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/TransparencyMode.lean
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/UnificationHint.lean
+-rw-r--r--   0        0        0    39782 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/WHNF.lean
+-rw-r--r--   0        0        0    14593 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/Basic.lean
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/CaseArraySizes.lean
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/CaseValues.lean
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MVarRenaming.lean
+-rw-r--r--   0        0        0    43350 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/Match.lean
+-rw-r--r--   0        0        0    34542 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MatchEqs.lean
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MatchEqsExt.lean
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MatchPatternAttr.lean
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MatcherApp.lean
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MatcherInfo.lean
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/Value.lean
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MatcherApp/Basic.lean
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Match/MatcherApp/Transform.lean
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/AC.lean
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Acyclic.lean
+-rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Apply.lean
+-rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Assert.lean
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Assumption.lean
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/AuxLemma.lean
+-rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Backtrack.lean
+-rw-r--r--   0        0        0    14356 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Cases.lean
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Cleanup.lean
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Clear.lean
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Congr.lean
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Constructor.lean
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Contradiction.lean
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Delta.lean
+-rw-r--r--   0        0        0     8411 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/ElimInfo.lean
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/FVarSubst.lean
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Generalize.lean
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/IndependentOf.lean
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Induction.lean
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Injection.lean
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Intro.lean
+-rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LibrarySearch.lean
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith.lean
+-rw-r--r--   0        0        0     7002 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/NormCast.lean
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Refl.lean
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Rename.lean
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Repeat.lean
+-rw-r--r--   0        0        0    10862 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Replace.lean
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Revert.lean
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Rewrite.lean
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp.lean
+-rw-r--r--   0        0        0    15682 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/SolveByElim.lean
+-rw-r--r--   0        0        0    15433 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Split.lean
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/SplitIf.lean
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Subst.lean
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Symm.lean
+-rw-r--r--   0        0        0    27287 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/TryThis.lean
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Unfold.lean
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/UnifyEq.lean
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Util.lean
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/AC/Main.lean
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Basic.lean
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Main.lean
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Nat.lean
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Simp.lean
+-rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Solver.lean
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Nat/Basic.lean
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Nat/Simp.lean
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/LinearArith/Nat/Solver.lean
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/Attr.lean
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs.lean
+-rw-r--r--   0        0        0    35951 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/Main.lean
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/RegisterCommand.lean
+-rw-r--r--   0        0        0    20311 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/Rewrite.lean
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/SimpAll.lean
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/SimpCongrTheorems.lean
+-rw-r--r--   0        0        0    19252 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/SimpTheorems.lean
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/Simproc.lean
+-rw-r--r--   0        0        0    20922 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/Types.lean
+-rw-r--r--   0        0        0    14623 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/BitVec.lean
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/Char.lean
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/Core.lean
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/Fin.lean
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/Int.lean
+-rw-r--r--   0        0        0     3615 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/Nat.lean
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/String.lean
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/UInt.lean
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Meta/Tactic/Simp/BuiltinSimprocs/Util.lean
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Attr.lean
+-rw-r--r--   0        0        0    78158 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Basic.lean
+-rw-r--r--   0        0        0    16857 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Command.lean
+-rw-r--r--   0        0        0    10659 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Do.lean
+-rw-r--r--   0        0        0    32923 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Extension.lean
+-rw-r--r--   0        0        0    16735 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Extra.lean
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Level.lean
+-rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Module.lean
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/StrInterpolation.lean
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Syntax.lean
+-rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Tactic.lean
+-rw-r--r--   0        0        0    40826 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Term.lean
+-rw-r--r--   0        0        0    17054 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Parser/Types.lean
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/ParserCompiler/Attribute.lean
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Basic.lean
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Delaborator.lean
+-rw-r--r--   0        0        0    22577 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Formatter.lean
+-rw-r--r--   0        0        0    29157 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Parenthesizer.lean
+-rw-r--r--   0        0        0    16916 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Delaborator/Basic.lean
+-rw-r--r--   0        0        0    49013 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Delaborator/Builtins.lean
+-rw-r--r--   0        0        0    10145 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Delaborator/Options.lean
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Delaborator/SubExpr.lean
+-rw-r--r--   0        0        0    27124 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/PrettyPrinter/Delaborator/TopDownAnalyze.lean
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/AsyncList.lean
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/CodeActions.lean
+-rw-r--r--   0        0        0    30138 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Completion.lean
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/CompletionItemData.lean
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/FileSource.lean
+-rw-r--r--   0        0        0    25944 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/FileWorker.lean
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/GoTo.lean
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/ImportCompletion.lean
+-rw-r--r--   0        0        0    17951 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/InfoUtils.lean
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/README.md
+-rw-r--r--   0        0        0    16270 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/References.lean
+-rw-r--r--   0        0        0    10954 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Requests.lean
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Rpc.lean
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Snapshots.lean
+-rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Utils.lean
+-rw-r--r--   0        0        0    39984 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Watchdog.lean
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/CodeActions/Attr.lean
+-rw-r--r--   0        0        0     7492 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/CodeActions/Basic.lean
+-rw-r--r--   0        0        0     8679 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/CodeActions/Provider.lean
+-rw-r--r--   0        0        0    29641 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/FileWorker/RequestHandling.lean
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/FileWorker/SetupFile.lean
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/FileWorker/Utils.lean
+-rw-r--r--   0        0        0     5692 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/FileWorker/WidgetRequests.lean
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Rpc/Basic.lean
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Rpc/Deriving.lean
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Server/Rpc/RequestHandling.lean
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/CollectFVars.lean
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/CollectLevelParams.lean
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/CollectMVars.lean
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/FileSetupInfo.lean
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/FindExpr.lean
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/FindLevelMVar.lean
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/FindMVar.lean
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/FoldConsts.lean
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/ForEachExpr.lean
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/ForEachExprWhere.lean
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/HasConstCache.lean
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/Heartbeats.lean
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/InstantiateLevelParams.lean
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/LakePath.lean
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/LeanOptions.lean
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/MonadBacktrack.lean
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/MonadCache.lean
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/OccursCheck.lean
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/PPExt.lean
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/Path.lean
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/Paths.lean
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/Profile.lean
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/PtrSet.lean
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/RecDepth.lean
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/Recognizers.lean
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/ReplaceExpr.lean
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/ReplaceLevel.lean
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/SCC.lean
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/ShareCommon.lean
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/Sorry.lean
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/TestExtern.lean
+-rw-r--r--   0        0        0    11994 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Util/Trace.lean
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/Basic.lean
+-rw-r--r--   0        0        0    13221 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/Diff.lean
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/InteractiveCode.lean
+-rw-r--r--   0        0        0    10079 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/InteractiveDiagnostic.lean
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/InteractiveGoal.lean
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/TaggedText.lean
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/Types.lean
+-rw-r--r--   0        0        0    18238 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/Lean/Widget/UserWidget.lean
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake.lean
+-rw-r--r--   0        0        0    28820 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/README.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/lakefile.lean
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build.lean
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI.lean
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config.lean
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL.lean
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Load.lean
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Main.lean
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Version.lean
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Actions.lean
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Common.lean
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Context.lean
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Data.lean
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Executable.lean
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Facets.lean
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Imports.lean
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Index.lean
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Info.lean
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Job.lean
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Key.lean
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Library.lean
+-rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Module.lean
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Monad.lean
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Package.lean
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Store.lean
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Targets.lean
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Topological.lean
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Build/Trace.lean
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI/Actions.lean
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI/Build.lean
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI/Error.lean
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI/Help.lean
+-rw-r--r--   0        0        0     7924 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI/Init.lean
+-rw-r--r--   0        0        0    14981 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI/Main.lean
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/CLI/Serve.lean
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Context.lean
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Defaults.lean
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Dependency.lean
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Env.lean
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/ExternLib.lean
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/ExternLibConfig.lean
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/FacetConfig.lean
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Glob.lean
+-rw-r--r--   0        0        0     9689 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/InstallPath.lean
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/LeanConfig.lean
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/LeanExe.lean
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/LeanExeConfig.lean
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/LeanLib.lean
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/LeanLibConfig.lean
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Module.lean
+-rw-r--r--   0        0        0     7773 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Monad.lean
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Opaque.lean
+-rw-r--r--   0        0        0    14239 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Package.lean
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Script.lean
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/TargetConfig.lean
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/Workspace.lean
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Config/WorkspaceConfig.lean
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Attributes.lean
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Config.lean
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/DeclUtil.lean
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Extensions.lean
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Meta.lean
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Package.lean
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Require.lean
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Script.lean
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/DSL/Targets.lean
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Load/Config.lean
+-rw-r--r--   0        0        0    10833 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Load/Elab.lean
+-rw-r--r--   0        0        0    11709 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Load/Main.lean
+-rw-r--r--   0        0        0     9168 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Load/Manifest.lean
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Load/Materialize.lean
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Load/Package.lean
+-rw-r--r--   0        0        0    11073 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Async.lean
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Binder.lean
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Casing.lean
+-rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Cli.lean
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Compare.lean
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Cycle.lean
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/DRBMap.lean
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/EStateT.lean
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/EquipT.lean
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Error.lean
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Exit.lean
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Family.lean
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Git.lean
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Lift.lean
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/List.lean
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Log.lean
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/MainM.lean
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Name.lean
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/NativeLib.lean
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Opaque.lean
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/OptionIO.lean
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/OrdHashSet.lean
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/OrderedTagAttribute.lean
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Proc.lean
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/RBArray.lean
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Store.lean
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/StoreInsts.lean
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Sugar.lean
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/Lake/Util/Task.lean
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/badImport/X.lean
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/badImport/lakefile.lean
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/badImport/Lib/A.lean
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/badImport/Lib/B.lean
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/buildArgs/Hello.lean
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/buildArgs/Main.lean
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/buildArgs/foo.lean
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/buildArgs/lakefile.lean
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/clone/test/Main.lean
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/clone/test/lakefile.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/globs/TBA.lean
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/globs/lakefile.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/globs/TBA/Eulerian.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/globs/TBA/Eulerian/A.lean
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/globs/Test/1.lean
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/globs/Test/Subtest/1.lean
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/llvm-bitcode-gen/LlvmBitcodeGen.lean
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/llvm-bitcode-gen/Main.lean
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/llvm-bitcode-gen/lakefile.lean
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/llvm-bitcode-gen/LlvmBitcodeGen/Basic.lean
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/lock/Error.lean
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/lock/Loop.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/lock/Nop.lean
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/lock/Wait.lean
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/lock/lakefile.lean
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/manifest/lakefile.lean
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/manifest/bar/lakefile.lean
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/manifest/foo/lakefile.lean
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/meta/lakefile.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/noBuild/Test.lean
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/noBuild/lakefile.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/A.lean
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/Y.lean
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/lakefile.lean
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/A/B.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/A/B/C.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/bar/X.lean
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/bar/Y.lean
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/bar/lakefile.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/foo/X.lean
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/foo/Y.lean
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/order/foo/lakefile.lean
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/postUpdate/lakefile.lean
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/postUpdate/dep/hello.lean
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/postUpdate/dep/lakefile.lean
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/precompileArgs/Foo.lean
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/precompileArgs/lakefile.lean
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/precompileArgs/Foo/Bar.lean
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/rebuild/Main.lean
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/traced_lean4-example/lean4-example/.lake/packages/lean4/src/lean/lake/tests/rebuild/lakefile.lean
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/LICENSE
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/README.md
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7854 2020-02-02 00:00:00.000000 lean_dojo-1.9.0/PKG-INFO
```

### Comparing `lean_dojo-1.8.2/.readthedocs.yaml` & `lean_dojo-1.9.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/__init__.py` & `lean_dojo-1.9.0/src/lean_dojo/__init__.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/constants.py` & `lean_dojo-1.9.0/src/lean_dojo/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,38 +10,38 @@
 from pathlib import Path
 from typing import Tuple
 from loguru import logger
 from dotenv import load_dotenv
 
 load_dotenv()
 
-__version__ = "1.8.2"
+__version__ = "1.9.0"
 
 logger.remove()
 if "VERBOSE" in os.environ or "DEBUG" in os.environ:
     logger.add(sys.stderr, level="DEBUG")
 else:
     logger.add(sys.stderr, level="INFO")
 
 CACHE_DIR = (
     Path(os.environ["CACHE_DIR"])
     if "CACHE_DIR" in os.environ
     else Path.home() / ".cache/lean_dojo"
-)
+).absolute()
 """Cache directory for storing traced repos (see :ref:`caching`).
 """
 
 REMOTE_CACHE_URL = "https://lean-dojo.s3.amazonaws.com"
 """URL of the remote cache (see :ref:`caching`)."""
 
 DISABLE_REMOTE_CACHE = "DISABLE_REMOTE_CACHE" in os.environ
 """Whether to disable remote caching (see :ref:`caching`) and build all repos locally.
 """
 
-TMP_DIR = Path(os.environ["TMP_DIR"]) if "TMP_DIR" in os.environ else None
+TMP_DIR = Path(os.environ["TMP_DIR"]).absolute() if "TMP_DIR" in os.environ else None
 """Temporary directory used by LeanDojo for storing intermediate files
 """
 
 MAX_NUM_PROCS = 32
 
 NUM_PROCS = int(os.getenv("NUM_PROCS", min(multiprocessing.cpu_count(), MAX_NUM_PROCS)))
 """Number of threads to use
```

### Comparing `lean_dojo-1.8.2/src/lean_dojo/container.py` & `lean_dojo-1.9.0/src/lean_dojo/container.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/utils.py` & `lean_dojo-1.9.0/src/lean_dojo/utils.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/data_extraction/ExtractData.lean` & `lean_dojo-1.9.0/traced_lean4-example/lean4-example/ExtractData.lean`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/data_extraction/ast.py` & `lean_dojo-1.9.0/src/lean_dojo/data_extraction/ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -388,17 +388,16 @@
         return cls(lean_file, start, end, children, name)
 
     def is_private(self) -> bool:
         return self._is_private_decl
 
     def get_proof_node(self) -> Node:
         decl_val_node = self.children[1].children[3]
-        if type(decl_val_node) in (
-            CommandDeclvalsimpleNode,
-            CommandWherestructinstNode,
+        if isinstance(
+            decl_val_node, (CommandDeclvalsimpleNode, CommandWherestructinstNode)
         ):
             return decl_val_node.children[1]
         else:
             return decl_val_node
 
     def has_tactic_proof(self) -> bool:
         node = self.get_proof_node()
@@ -438,17 +437,20 @@
         return cls(lean_file, start, end, children, name)
 
     def is_private(self) -> bool:
         return self._is_private_decl
 
     def get_proof_node(self) -> Node:
         decl_val_node = self.children[1].children[3]
-        if type(decl_val_node) in (
-            CommandDeclvalsimpleNode,
-            CommandWherestructinstNode,
+        if isinstance(
+            decl_val_node,
+            (
+                CommandDeclvalsimpleNode,
+                CommandWherestructinstNode,
+            ),
         ):
             return decl_val_node.children[1]
         else:
             return decl_val_node
 
     def has_tactic_proof(self) -> bool:
         node = self.get_proof_node()
@@ -472,25 +474,29 @@
         start, end = None, None
         children = _parse_children(node_data, lean_file)
 
         if isinstance(children[0], CommandDeclmodifiersAntiquotNode):
             name = None
         else:
             assert isinstance(children[0], CommandDeclmodifiersNode)
-            assert type(children[1]) in (
-                CommandDefNode,
-                CommandTheoremNode,
-                CommandInductiveNode,
-                CommandClassinductiveNode,
-                CommandStructureNode,
-                CommandInstanceNode,
-                CommandAbbrevNode,
-                CommandOpaqueNode,
-                CommandAxiomNode,
-                CommandExampleNode,
+            assert isinstance(
+                children[1],
+                (
+                    CommandDefNode,
+                    CommandDefinitionNode,
+                    CommandTheoremNode,
+                    CommandInductiveNode,
+                    CommandClassinductiveNode,
+                    CommandStructureNode,
+                    CommandInstanceNode,
+                    CommandAbbrevNode,
+                    CommandOpaqueNode,
+                    CommandAxiomNode,
+                    CommandExampleNode,
+                ),
             )
             name = children[1].name
 
             if children[0].is_private():
                 for child in children:
                     if isinstance(child, CommandTheoremNode):
                         object.__setattr__(child, "_is_private_decl", True)
@@ -625,15 +631,15 @@
     def from_data(
         cls, node_data: Dict[str, Any], lean_file: LeanFile
     ) -> "CommandStructureNode":
         assert node_data["info"] == "none"
         start, end = None, None
         children = _parse_children(node_data, lean_file)
 
-        assert type(children[0]) in (CommandStructuretkNode, CommandClasstkNode)
+        assert isinstance(children[0], (CommandStructuretkNode, CommandClasstkNode))
         if isinstance(children[1], CommandDeclidAntiquotNode):
             name = None
         else:
             assert isinstance(children[1], CommandDeclidNode)
             decl_id_node = children[1]
             ident_node = decl_id_node.children[0]
 
@@ -707,34 +713,40 @@
     @classmethod
     def from_data(
         cls, node_data: Dict[str, Any], lean_file: LeanFile
     ) -> "TermHoleNode":
         assert node_data["info"] == "none"
         start, end = None, None
         children = _parse_children(node_data, lean_file)
-        assert len(children) == 1 and type(children[0]) in (
-            AtomNode,
-            TokenAntiquotNode,
+        assert len(children) == 1 and isinstance(
+            children[0],
+            (
+                AtomNode,
+                TokenAntiquotNode,
+            ),
         )
         return cls(lean_file, start, end, children)
 
 
 @dataclass(frozen=True)
 class LeanBinderidentNode(Node):
     @classmethod
     def from_data(
         cls, node_data: Dict[str, Any], lean_file: LeanFile
     ) -> "LeanBinderidentNode":
         assert node_data["info"] == "none"
         start, end = None, None
         children = _parse_children(node_data, lean_file)
-        assert len(children) == 1 and type(children[0]) in (
-            TermHoleNode,
-            IdentNode,
-            IdentAntiquotNode,
+        assert len(children) == 1 and isinstance(
+            children[0],
+            (
+                TermHoleNode,
+                IdentNode,
+                IdentAntiquotNode,
+            ),
         )
         return cls(lean_file, start, end, children)
 
     def get_ident(self) -> Optional[str]:
         if isinstance(self.children[0], TermHoleNode):
             return None
         else:
@@ -797,17 +809,21 @@
         assert isinstance(children[0], CommandDeclmodifiersNode)
         assert isinstance(children[1], AtomNode) and children[1].val == "alias"
         assert isinstance(children[2], AtomNode) and children[2].val == "⟨"
         assert isinstance(children[4], AtomNode) and children[4].val == ","
         assert isinstance(children[6], AtomNode) and children[6].val == "⟩"
 
         name = []
-        assert type(children[3]) in (LeanBinderidentNode, LeanBinderidentAntiquotNode)
+        assert isinstance(
+            children[3], (LeanBinderidentNode, LeanBinderidentAntiquotNode)
+        )
         name.append(children[3].get_ident())
-        assert type(children[5]) in (LeanBinderidentNode, LeanBinderidentAntiquotNode)
+        assert isinstance(
+            children[5], (LeanBinderidentNode, LeanBinderidentAntiquotNode)
+        )
         name.append(children[5].get_ident())
         name = [n for n in name if n is not None]
 
         return cls(lean_file, start, end, children, name)
 
     @property
     def is_mutual(self) -> bool:
@@ -962,14 +978,45 @@
                 assert isinstance(ident_node, IdentAntiquotNode)
                 name = ident_node.get_ident()
 
         return cls(lean_file, start, end, children, name)
 
 
 @dataclass(frozen=True)
+class CommandDefinitionNode(Node):
+    name: str
+
+    @classmethod
+    def from_data(
+        cls, node_data: Dict[str, Any], lean_file: LeanFile
+    ) -> "CommandDefinitionNode":
+        assert node_data["info"] == "none"
+        start, end = None, None
+        children = _parse_children(node_data, lean_file)
+
+        if isinstance(children[0], TokenAntiquotNode) or isinstance(
+            children[1], CommandDeclidAntiquotNode
+        ):
+            name = None
+        else:
+            assert isinstance(children[0], AtomNode) and children[0].val == "def"
+            assert isinstance(children[1], CommandDeclidNode)
+            decl_id_node = children[1]
+            ident_node = decl_id_node.children[0]
+
+            if isinstance(ident_node, IdentNode):
+                name = ident_node.val
+            else:
+                assert isinstance(ident_node, IdentAntiquotNode)
+                name = ident_node.get_ident()
+
+        return cls(lean_file, start, end, children, name)
+
+
+@dataclass(frozen=True)
 class CommandDeclidAntiquotNode(Node):
     @classmethod
     def from_data(
         cls, node_data: Dict[str, Any], lean_file: LeanFile
     ) -> "CommandDeclidAntiquotNode":
         assert node_data["info"] == "none"
         start, end = None, None
@@ -1101,18 +1148,21 @@
             else:
                 assert isinstance(ident_node, IdentAntiquotNode)
                 name = ident_node.get_ident()
 
         if not isinstance(children[1], CommandDeclidAntiquotNode):
             assert isinstance(children[2], CommandDeclsigNode)
             decl_val_node = children[3]
-            assert type(decl_val_node) in (
-                CommandDeclvalsimpleNode,
-                CommandDeclvaleqnsNode,
-                CommandWherestructinstNode,
+            assert isinstance(
+                decl_val_node,
+                (
+                    CommandDeclvalsimpleNode,
+                    CommandDeclvaleqnsNode,
+                    CommandWherestructinstNode,
+                ),
             )
 
             if isinstance(decl_val_node, CommandDeclvalsimpleNode):
                 assert (
                     isinstance(decl_val_node.children[0], AtomNode)
                     and decl_val_node.children[0].val == ":="
                 )
@@ -1125,17 +1175,20 @@
         return cls(lean_file, start, end, children, name)
 
     def is_private(self) -> bool:
         return self._is_private_decl
 
     def get_proof_node(self) -> Node:
         decl_val_node = self.children[3]
-        if type(decl_val_node) in (
-            CommandDeclvalsimpleNode,
-            CommandWherestructinstNode,
+        if isinstance(
+            decl_val_node,
+            (
+                CommandDeclvalsimpleNode,
+                CommandWherestructinstNode,
+            ),
         ):
             return decl_val_node.children[1]
         else:
             return decl_val_node
 
     def has_tactic_proof(self) -> bool:
         node = self.get_proof_node()
@@ -1180,18 +1233,21 @@
     @classmethod
     def from_data(
         cls, node_data: Dict[str, Any], lean_file: LeanFile
     ) -> "TacticTacticseqNode":
         assert node_data["info"] == "none"
         start, end = None, None
         children = _parse_children(node_data, lean_file)
-        assert len(children) == 1 and type(children[0]) in (
-            TacticTacticseq1IndentedNode,
-            TacticTacticseqbracketedNode,
-            TacticTacticseq1IndentedAntiquotNode,
+        assert len(children) == 1 and isinstance(
+            children[0],
+            (
+                TacticTacticseq1IndentedNode,
+                TacticTacticseqbracketedNode,
+                TacticTacticseq1IndentedAntiquotNode,
+            ),
         )
         return cls(lean_file, start, end, children)
 
     def get_tactic_nodes(
         self, atomic_only: bool = False
     ) -> Generator[Node, None, None]:
         yield from self.children[0].get_tactic_nodes(atomic_only)
@@ -1269,17 +1325,20 @@
                     )
 
 
 def contains_tactic(node: Node) -> bool:
     result = False
 
     def _callback(x, _) -> bool:
-        if x is not node and type(x) in (
-            TacticTacticseq1IndentedNode,
-            TacticTacticseqbracketedNode,
+        if x is not node and isinstance(
+            x,
+            (
+                TacticTacticseq1IndentedNode,
+                TacticTacticseqbracketedNode,
+            ),
         ):
             nonlocal result
             result = True
             return True
 
     node.traverse_preorder(_callback, node_cls=None)
     return result
@@ -1491,26 +1550,27 @@
         start, end = None, None
         children = _parse_children(node_data, lean_file)
         return cls(lean_file, start, end, children, node_data["kind"])
 
 
 def is_potential_premise_lean4(node: Node) -> bool:
     """Check if ``node`` is a theorem/definition that can be used as a premise."""
-    if (isinstance(node, CommandDeclarationNode) and not node.is_example) or type(
-        node
-    ) in (
-        LemmaNode,
-        MathlibTacticLemmaNode,
-        LeanElabCommandCommandIrreducibleDefNode,
-        StdTacticAliasAliasNode,
-        StdTacticAliasAliaslrNode,
+    if (isinstance(node, CommandDeclarationNode) and not node.is_example) or isinstance(
+        node,
+        (
+            LemmaNode,
+            MathlibTacticLemmaNode,
+            LeanElabCommandCommandIrreducibleDefNode,
+            StdTacticAliasAliasNode,
+            StdTacticAliasAliaslrNode,
+        ),
     ):
         return node.name is not None
     else:
         return False
 
 
 def is_mutual_lean4(node: Node) -> bool:
     return (
-        type(node) in (IdentNode, CommandTheoremNode, StdTacticAliasAliaslrNode)
+        isinstance(node, (IdentNode, CommandTheoremNode, StdTacticAliasAliaslrNode))
         and node.is_mutual
     )
```

### Comparing `lean_dojo-1.8.2/src/lean_dojo/data_extraction/build_lean4_repo.py` & `lean_dojo-1.9.0/src/lean_dojo/data_extraction/build_lean4_repo.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/data_extraction/cache.py` & `lean_dojo-1.9.0/src/lean_dojo/data_extraction/cache.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/data_extraction/lean.py` & `lean_dojo-1.9.0/src/lean_dojo/data_extraction/lean.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import webbrowser
 from pathlib import Path
 from loguru import logger
 from functools import cache
 from github import Github, Auth
 from dataclasses import dataclass, field
 from github.Repository import Repository
-from typing import List, Dict, Any, Generator, Union, Optional, Tuple
+from typing import List, Dict, Any, Generator, Union, Optional, Tuple, Iterator
 
 from ..utils import (
     execute,
     read_url,
     url_exists,
     get_repo_info,
     working_directory,
@@ -356,18 +356,22 @@
     tag2commit: Dict[Tuple[URL, TAG], COMMIT] = field(default_factory=dict)
     lean_version: Dict[Tuple[URL, COMMIT], str] = field(default_factory=dict)
 
 
 info_cache = RepoInfoCache()
 
 
-_GIT_REQUIREMENT_REGEX = re.compile(
+_LAKEFILE_LEAN_GIT_REQUIREMENT_REGEX = re.compile(
     r"require\s+(?P<name>\S+)\s+from\s+git\s+\"(?P<url>.+?)\"(\s+@\s+\"(?P<rev>\S+)\")?"
 )
 
+_LAKEFILE_LEAN_LOCAL_REQUIREMENT_REGEX = re.compile(r"require \S+ from \"")
+
+_LAKEFILE_TOML_REQUIREMENT_REGEX = re.compile(r"(?<=\[\[require\]\]).+(?=\n\n)")
+
 
 def is_supported_version(v) -> bool:
     """Check if ``v`` is at least `v4.3.0-rc2`."""
     if not v.startswith("v"):
         return False
     v = v[1:]
     major, minor, patch = [int(_) for _ in v.split("-")[0].split(".")]
@@ -507,37 +511,50 @@
                 self.get_config("lake-manifest.json", num_retries=0)
                 if path is None
                 else json.load((Path(path) / "lake-manifest.json").open())
             )
             for pkg in lake_manifest["packages"]:
                 deps[pkg["name"]] = LeanGitRepo(pkg["url"], pkg["rev"])
         except Exception:
-            lakefile = (
-                self.get_config("lakefile.lean")
-                if path is None
-                else {"content": (Path(path) / "lakefile.lean").open().read()}
-            )
-            for name, repo in self._parse_lakefile_dependencies(lakefile["content"]):
+            for name, repo in self._parse_lakefile_dependencies(path):
                 if name not in deps:
                     deps[name] = repo
                 for dd_name, dd_repo in repo.get_dependencies().items():
                     deps[dd_name] = dd_repo
 
         return deps
 
     def _parse_lakefile_dependencies(
-        self, lakefile: str
+        self, path: Union[str, Path, None]
+    ) -> List[Tuple[str, "LeanGitRepo"]]:
+        if self.uses_lakefile_lean():
+            return self._parse_lakefile_lean_dependencies(path)
+        else:
+            return self._parse_lakefile_toml_dependencies(path)
+
+    def _parse_lakefile_lean_dependencies(
+        self, path: Union[str, Path, None]
     ) -> List[Tuple[str, "LeanGitRepo"]]:
-        _LOCAL_REQUIREMENT_REGEX = r"require \S+ from \""
-        if re.search(_LOCAL_REQUIREMENT_REGEX, lakefile):
+        lakefile = (
+            self.get_config("lakefile.lean")["content"]
+            if path is None
+            else (Path(path) / "lakefile.lean").open().read()
+        )
+
+        if _LAKEFILE_LEAN_LOCAL_REQUIREMENT_REGEX.search(lakefile):
             raise ValueError("Local dependencies are not supported.")
 
+        return self._parse_deps(_LAKEFILE_LEAN_GIT_REQUIREMENT_REGEX.finditer(lakefile))
+
+    def _parse_deps(
+        self, matches: Union[Iterator[re.Match[str]], Dict[str, str]]
+    ) -> List[Tuple[str, "LeanGitRepo"]]:
         deps = []
 
-        for m in _GIT_REQUIREMENT_REGEX.finditer(lakefile):
+        for m in matches:
             url = m["url"]
             if url.endswith(".git"):
                 url = url[:-4]
             if url.startswith("git@"):
                 url = "https://" + url[4:].replace(":", "/")
 
             rev = m["rev"]
@@ -552,14 +569,40 @@
                     commit = get_latest_commit(url)
                 assert _COMMIT_REGEX.fullmatch(commit)
 
             deps.append((m["name"], LeanGitRepo(url, commit)))
 
         return deps
 
+    def _parse_lakefile_toml_dependencies(
+        self, path: Union[str, Path, None]
+    ) -> List[Tuple[str, "LeanGitRepo"]]:
+        lakefile = (
+            self.get_config("lakefile.toml")["content"]
+            if path is None
+            else (Path(path) / "lakefile.toml").open().read()
+        )
+        matches = dict()
+
+        for requirement in _LAKEFILE_TOML_REQUIREMENT_REGEX.finditer(lakefile):
+            for line in requirement.strip().splitlines():
+                key, value = line.split("=")
+                key = key.strip()
+                value = value.strip()
+                if key == "path":
+                    raise ValueError("Local dependencies are not supported.")
+                if key == "git":
+                    matches["url"] = value
+                if key == "rev":
+                    matches["rev"] = value
+                if key == "name":
+                    matches["name"] = value
+
+        return self._parse_deps(lakefile, matches)
+
     def get_license(self) -> Optional[str]:
         """Return the content of the ``LICENSE`` file."""
         assert "github.com" in self.url, f"Unsupported URL: {self.url}"
         url = self.url.replace("github.com", "raw.githubusercontent.com")
         license_url = f"{url}/{self.commit}/LICENSE"
         try:
             return read_url(license_url)
@@ -578,14 +621,24 @@
         if filename.endswith(".toml"):
             return toml.loads(content)
         elif filename.endswith(".json"):
             return json.loads(content)
         else:
             return {"content": content}
 
+    def uses_lakefile_lean(self) -> bool:
+        """Check if the repo uses a ``lakefile.lean``."""
+        url = self._get_config_url("lakefile.lean")
+        return url_exists(url)
+
+    def uses_lakefile_toml(self) -> bool:
+        """Check if the repo uses a ``lakefile.toml``."""
+        url = self._get_config_url("lakefile.toml")
+        return url_exists(url)
+
 
 @dataclass(frozen=True)
 class Theorem:
     """Theorem in Lean.
 
     Theorems are named constants of type :code:`Prop`. They are typically defined
     using the keywords :code:`theorem` or :code:`lemma`, but it's possible to use other
```

### Comparing `lean_dojo-1.8.2/src/lean_dojo/data_extraction/trace.py` & `lean_dojo-1.9.0/src/lean_dojo/data_extraction/trace.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/src/lean_dojo/data_extraction/traced_data.py` & `lean_dojo-1.9.0/src/lean_dojo/data_extraction/traced_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,21 +340,14 @@
         raise NotImplementedError
         assert isinstance(node.children[0], AtomNode) and node.children[0].val == "by"
         assert proof.startswith("by")
         proof = proof[len("by") :].strip()
 
         return proof
 
-    def get_namespaces(self) -> Tuple[List[str], List[str]]:
-        """Return the namespaces that the theorem is located in,
-        as well as the namespaces that are merely open.
-        """
-        assert self.traced_file is not None
-        return self.traced_file.get_namespaces(self)
-
     def get_premise_full_names(self) -> List[str]:
         """Return the fully qualified names of all premises used in the proof."""
         names = []
 
         def _callback(node: IdentNode, _: List[Node]):
             if node.full_name is not None:
                 names.append(node.full_name)
@@ -380,17 +373,20 @@
 
     def _get_traced_tactics_lean4(
         self, atomic_only: bool = False
     ) -> List[TracedTactic]:
         tacs = []
 
         def _callback(node, _):
-            if type(node) not in (
-                TacticTacticseq1IndentedNode,
-                TacticTacticseqbracketedNode,
+            if not isinstance(
+                node,
+                (
+                    TacticTacticseq1IndentedNode,
+                    TacticTacticseqbracketedNode,
+                ),
             ):
                 return
             for tac_node in node.get_tactic_nodes(atomic_only):
                 if (
                     hasattr(tac_node, "state_before")
                     and tac_node.state_before is not None
                 ):
@@ -589,19 +585,21 @@
             end = Pos(line_nb=end_line_nb, column_nb=end_column_nb + 1)
             pos2premises[(start, end)] = p
 
         inside_sections_namespaces = []
 
         def _callback(node: Node, _):
             if (
-                type(node)
-                in (
-                    CommandNamespaceNode,
-                    CommandSectionNode,
-                    CommandNoncomputablesectionNode,
+                isinstance(
+                    node,
+                    (
+                        CommandNamespaceNode,
+                        CommandSectionNode,
+                        CommandNoncomputablesectionNode,
+                    ),
                 )
                 and node.name is not None
             ):
                 inside_sections_namespaces.append(node)
             elif (
                 isinstance(node, CommandEndNode)
                 and node.name is not None
@@ -618,20 +616,25 @@
                     [_qualify_name(name, prefix) for name in node.name]
                     if is_mutual_lean4(node)
                     else _qualify_name(node.name, prefix)
                 )
                 object.__setattr__(node, "full_name", full_name)
                 if isinstance(node, CommandDeclarationNode) and node.is_theorem:
                     object.__setattr__(node.get_theorem_node(), "full_name", full_name)
-            elif type(node) in (
-                TacticTacticseq1IndentedNode,
-                TacticTacticseqbracketedNode,
+            elif isinstance(
+                node,
+                (
+                    TacticTacticseq1IndentedNode,
+                    TacticTacticseqbracketedNode,
+                ),
             ):
                 for tac_node in node.get_tactic_nodes():
-                    assert type(tac_node) in (OtherNode, TacticTacticseqbracketedNode)
+                    assert isinstance(
+                        tac_node, (OtherNode, TacticTacticseqbracketedNode)
+                    )
                     if (tac_node.start, tac_node.end) not in pos2tactics:
                         continue
                     t = pos2tactics[(tac_node.start, tac_node.end)]
                     tac = get_code_without_comments(
                         lean_file, tac_node.start, tac_node.end, comments
                     )
                     tac = _fix_indentation(tac, tac_node.start.column_nb - 1)
@@ -665,15 +668,15 @@
                             line_nb=def_start_line_nb, column_nb=def_start_column_nb + 1
                         )
                         def_end = Pos(
                             line_nb=def_end_line_nb, column_nb=def_end_column_nb + 1
                         )
                         object.__setattr__(node, "def_start", def_start)
                         object.__setattr__(node, "def_end", def_end)
-            elif type(node) in (ModuleImportNode,):
+            elif isinstance(node, ModuleImportNode):
                 node_module_name = object.__getattribute__(node, "module")
                 if node_module_name is not None:
                     suffix = node_module_name.replace(".", "/")
                     for import_line in imports_data:
                         if import_line.endswith(
                             suffix + ".lean"
                         ) or import_line.endswith(suffix + "/default.lean"):
@@ -732,18 +735,21 @@
         result = None
         private_result = None
 
         def _callback(
             node: Union[CommandTheoremNode, LemmaNode, MathlibTacticLemmaNode], _
         ) -> None:
             nonlocal result, private_result
-            if type(node) not in (
-                CommandTheoremNode,
-                LemmaNode,
-                MathlibTacticLemmaNode,
+            if not isinstance(
+                node,
+                (
+                    CommandTheoremNode,
+                    LemmaNode,
+                    MathlibTacticLemmaNode,
+                ),
             ):
                 return False
             if node.full_name == thm.full_name:
                 comments = self._filter_comments(node.start, node.end)
                 t = TracedTheorem(self.root_dir, thm, node, comments, self)
                 if t.is_private:
                     private_result = t
@@ -760,18 +766,21 @@
     def get_traced_theorems(self) -> List[TracedTheorem]:
         """Return a list of traced theorem in this traced file."""
         traced_theorems = []
 
         def _callback(
             node: Union[CommandTheoremNode, LemmaNode, MathlibTacticLemmaNode], _
         ) -> None:
-            if type(node) not in (
-                CommandTheoremNode,
-                LemmaNode,
-                MathlibTacticLemmaNode,
+            if not isinstance(
+                node,
+                (
+                    CommandTheoremNode,
+                    LemmaNode,
+                    MathlibTacticLemmaNode,
+                ),
             ):
                 return False
             repo, path = self._get_repo_and_relative_path()
             thm = Theorem(repo, path, node.full_name)
             comments = self._filter_comments(node.start, node.end)
             traced_theorems.append(
                 TracedTheorem(self.root_dir, thm, node, comments, self)
```

### Comparing `lean_dojo-1.8.2/src/lean_dojo/interaction/Lean4Repl.lean` & `lean_dojo-1.9.0/src/lean_dojo/interaction/Lean4Repl.lean`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 -- REPL for interacting with Lean 4 via the command line.
+import Lean.Message
 import Lean.Elab.Tactic
 import Lean.Elab.Frontend
 
 open Lean Lean.Meta Lean.Elab Lean.Elab.Command Lean.Elab.Tactic
 
 namespace LeanDojo
 
@@ -224,15 +225,15 @@
       ts.restore
 
       try
         monadLift $ commitIfNoEx (evalTactic stx)
         let s ← getThe Core.State
         if s.messages.hasErrors then
           let messages := s.messages.toList.filter fun m => m.severity == MessageSeverity.error
-          return { error := join $ ← (messages.map Message.data).mapM fun md => md.toString }
+          return { error := join $ ← (messages.map (·.data)).mapM fun md => md.toString }
       catch ex =>
         return {error := ← ex.toMessageData.toString}
 
       pruneSolvedGoals
       if (← getGoals).isEmpty then
         validateProof
       else
```

### Comparing `lean_dojo-1.8.2/src/lean_dojo/interaction/dojo.py` & `lean_dojo-1.9.0/src/lean_dojo/interaction/dojo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import os
 import sys
 import json
 import time
 import signal
 import shutil
+import psutil
 from pathlib import Path
 from loguru import logger
 from tempfile import mkdtemp
 from shutil import ignore_patterns
 from subprocess import TimeoutExpired
 from dataclasses import dataclass, field
 from typing import Union, Tuple, List, Dict, Any, Optional
@@ -96,29 +97,18 @@
     pass
 
 
 class DojoInitError(Exception):
     pass
 
 
-def _get_all_dependencies(
-    root_dir: Path, lean_path: Path, repo: LeanGitRepo
-) -> List[Path]:
-    all_deps = []
-    stack = [lean_path]
-
-    while stack != []:
-        json_path = to_json_path(root_dir, stack.pop(), repo)
-        tf = TracedFile.from_traced_file(root_dir, json_path, repo)
-        for _, d in tf.get_direct_dependencies(repo):
-            if d not in all_deps:
-                all_deps.append(d)
-                stack.append(d)
-
-    return all_deps
+def _kill_descendants(proc: psutil.Process) -> None:
+    for child in proc.children():
+        _kill_descendants(child)
+    proc.kill()
 
 
 class Dojo:
     """Gym-like environment for programmatic interaction with Lean through tactics or commands."""
 
     entry: Union[Theorem, Tuple[LeanGitRepo, Path, int]]
     hard_timeout: Optional[float]
@@ -310,19 +300,23 @@
         assert isinstance(self.container, DockerContainer) or isinstance(
             self.container, NativeContainer
         )
         self.container.cleanup()
 
     def _cleanup_proc(self) -> None:
         """Clean up the subprocess."""
+        logger.debug(f"Cleaning up the subprocess {self.proc.pid}.")
+        _kill_descendants(psutil.Process(self.proc.pid))
+        """
         self.proc.terminate()
         try:
             self.proc.wait(timeout=0.5)
         except TimeoutExpired:
             self.proc.kill()
+        """
 
     def _cleanup_tmp_dir(self) -> None:
         """Clean up the temporary directory."""
         logger.debug("Cleaning up the temporary directory.")
         os.chdir(self.origin_dir)
         if self.tmp_dir is not None and os.path.exists(self.tmp_dir):
             shutil.rmtree(self.tmp_dir)
@@ -376,16 +370,23 @@
                 + code_before
                 + "set_option maxHeartbeats 0 in\n#lean_dojo_repl\n\n"
                 + lean_file[pos:]
             )
 
         repl_file = "Lean4Repl.lean"
         repl_dst = Path(repl_file)
-        with open("lakefile.lean", "a") as oup:
-            oup.write("\nlean_lib Lean4Repl {\n\n}\n")
+
+        if os.path.exists("lakefile.lean"):
+            with open("lakefile.lean", "a") as oup:
+                oup.write("\nlean_lib Lean4Repl {\n\n}\n")
+        else:
+            assert os.path.exists("lakefile.toml")
+            with open("lakefile.toml", "a") as oup:
+                oup.write('\n[[lean_lib]]\nname = "Lean4Repl"\n')
+
         if os.path.exists("lakefile.olean"):
             os.remove("lakefile.olean")
         if os.path.exists(".lake/lakefile.olean"):
             os.remove(".lake/lakefile.olean")
 
         # Copy the REPL code to the right directory.
         repl_src = Path(__file__).with_name(repl_file)
```

### Comparing `lean_dojo-1.8.2/src/lean_dojo/interaction/parse_goals.py` & `lean_dojo-1.9.0/src/lean_dojo/interaction/parse_goals.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/tests/conftest.py` & `lean_dojo-1.9.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 
 from lean_dojo import *
 
 
-STD4_URL = "https://github.com/leanprover/std4"
+BATTERIES_URL = "https://github.com/leanprover-community/batteries"
 AESOP_URL = "https://github.com/leanprover-community/aesop"
 MATHLIB4_URL = "https://github.com/leanprover-community/mathlib4"
 LEAN4_EXAMPLE_URL = "https://github.com/yangky11/lean4-example"
 URLS = [
-    STD4_URL,
+    BATTERIES_URL,
     AESOP_URL,
     MATHLIB4_URL,
     LEAN4_EXAMPLE_URL,
 ]
 
 
 @pytest.fixture(scope="session")
@@ -24,17 +24,17 @@
 @pytest.fixture(scope="session")
 def lean4_example_repo():
     commit = get_latest_commit(LEAN4_EXAMPLE_URL)
     return LeanGitRepo(LEAN4_EXAMPLE_URL, commit)
 
 
 @pytest.fixture(scope="session")
-def std4_repo():
-    commit = get_latest_commit(STD4_URL)
-    return LeanGitRepo(STD4_URL, commit)
+def batteries_repo():
+    commit = get_latest_commit(BATTERIES_URL)
+    return LeanGitRepo(BATTERIES_URL, commit)
 
 
 @pytest.fixture(scope="session")
 def mathlib4_repo():
     commit = "fe4454af900584467d21f4fd4fe951d29d9332a7"
     return LeanGitRepo(MATHLIB4_URL, commit)
```

### Comparing `lean_dojo-1.8.2/tests/interaction/test_commands.py` & `lean_dojo-1.9.0/tests/interaction/test_commands.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/tests/interaction/test_imports.py` & `lean_dojo-1.9.0/tests/interaction/test_imports.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/tests/interaction/test_init_errors.py` & `lean_dojo-1.9.0/tests/interaction/test_init_errors.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/tests/interaction/test_sorry.py` & `lean_dojo-1.9.0/tests/interaction/test_sorry.py`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/tests/interaction/test_tactics.py` & `lean_dojo-1.9.0/tests/interaction/test_tactics.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
             s2,
             "· suffices x ^ 2 ^ d.succ - y ^ 2 ^ d.succ = (x ^ 2 ^ d + y ^ 2 ^ d) * (x ^ 2 ^ d - y ^ 2 ^ d) by rw [this, hd, Finset.prod_range_succ, ← mul_assoc, mul_comm (x ^ 2 ^ d + y ^ 2 ^ d)]",
         )
         assert not isinstance(s3, ProofFinished)
         assert not dojo.is_successful
 
 
-def test_example_mem_nil_iff(std4_repo: LeanGitRepo) -> None:
+def test_example_mem_nil_iff(batteries_repo: LeanGitRepo) -> None:
     thm = Theorem(
-        std4_repo,
-        "Std/Data/List/Lemmas.lean",
+        batteries_repo,
+        "Batteries/Data/List/Lemmas.lean",
         "List.mem_nil_iff",
     )
     with Dojo(thm) as (dojo, s0):
         s1 = dojo.run_tac(s0, "simp")
         assert isinstance(s1, ProofFinished)
         assert dojo.is_successful
 
@@ -134,18 +134,18 @@
     )
     with Dojo(thm) as (dojo, s0):
         s1 = dojo.run_tac(s0, "rfl")
         assert isinstance(s1, ProofFinished)
         assert dojo.is_successful
 
 
-def test_example_length_le(std4_repo: LeanGitRepo) -> None:
+def test_example_length_le(batteries_repo: LeanGitRepo) -> None:
     thm = Theorem(
-        std4_repo,
-        "Std/Data/List/Lemmas.lean",
+        batteries_repo,
+        "Batteries/Data/List/Lemmas.lean",
         "List.IsSuffix.length_le",
     )
     with Dojo(thm) as (dojo, s0):
         s1 = dojo.run_tac(s0, "exact h.sublist.length_le")
         assert isinstance(s1, ProofFinished)
         assert dojo.is_successful
 
@@ -275,28 +275,14 @@
     )
     with Dojo(thm) as (dojo, s0):
         s1 = dojo.run_tac(s0, "exact Iff.rfl")
         assert isinstance(s1, ProofFinished)
         assert dojo.is_successful
 
 
-def test_example_neg_lt_sub_right_of_lt_add(std4_repo: LeanGitRepo) -> None:
-    thm = Theorem(
-        std4_repo,
-        "Std/Data/Int/Order.lean",
-        "Int.neg_lt_sub_right_of_lt_add",
-    )
-    with Dojo(thm) as (dojo, s0):
-        s1 = dojo.run_tac(
-            s0, "exact Int.lt_sub_left_of_add_lt (Int.sub_right_lt_of_lt_add h)"
-        )
-        assert isinstance(s1, ProofFinished)
-        assert dojo.is_successful
-
-
 def test_example_eq(mathlib4_repo: LeanGitRepo) -> None:
     thm = Theorem(
         mathlib4_repo,
         "Mathlib/Algebra/CharP/Basic.lean",
         "CharP.eq",
     )
     with Dojo(thm) as (dojo, s0):
```

### Comparing `lean_dojo-1.8.2/.gitignore` & `lean_dojo-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/LICENSE` & `lean_dojo-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lean_dojo-1.8.2/README.md` & `lean_dojo-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 pip install .
 ```
 
 
 ## Documentation
 
 * [Getting Started](https://leandojo.readthedocs.io/en/latest/getting-started.html)
-* Demos: [Lean 3](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo-lean3.ipynb), [Lean 4](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo-lean4.ipynb)
+* [Demo](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo-lean4.ipynb)
 * [Full documentation](https://leandojo.readthedocs.io/en/latest/index.html)
 
 
 ## Questions and Bugs
 
 * For general questions and discussions, please use [GitHub Discussions](https://github.com/lean-dojo/LeanDojo/discussions).  
 * To report a potential bug, please open an issue. In the issue, please include your OS information, the version of LeanDojo, the exact steps to reproduce the error, and complete logs in debug mode (setting the environment variable `VERBOSE` to 1). The more details you provide, the better we will be able to help you.
```

### Comparing `lean_dojo-1.8.2/pyproject.toml` & `lean_dojo-1.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "/docs",
   "/images",
   "/scripts",
 ]
 
 [project]
 name = "lean-dojo"
-version = "1.8.2"
+version = "1.9.0"
 authors = [
   { name="Kaiyu Yang", email="kaiyuy@caltech.edu" },
 ]
 description = "LeanDojo: Machine Learning for Theorem Proving in Lean"
 keywords = ["theorem proving", "machine learning", "Lean"]
 readme = "README.md"
 license = { file = "LICENSE" }
@@ -28,14 +28,16 @@
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
 ]
 dependencies = [
   "python-dotenv",
   "loguru",
   "filelock",
+  "psutil",
+  "types-psutil",
   "tqdm",
   "toml",
   "types-toml",
   "networkx",
   "lxml",
   "PyGithub",
   "ray[default] >= 2.8",
```

### Comparing `lean_dojo-1.8.2/PKG-INFO` & `lean_dojo-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lean-dojo
-Version: 1.8.2
+Version: 1.9.0
 Summary: LeanDojo: Machine Learning for Theorem Proving in Lean
 Project-URL: Homepage, https://leandojo.org/
 Project-URL: Bug Tracker, https://github.com/lean-dojo/LeanDojo/issues
 Author-email: Kaiyu Yang <kaiyuy@caltech.edu>
 License: MIT License
         
         Copyright (c) 2023 LeanDojo Team
@@ -33,19 +33,21 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: <3.12,>=3.9
 Requires-Dist: filelock
 Requires-Dist: loguru
 Requires-Dist: lxml
 Requires-Dist: networkx
+Requires-Dist: psutil
 Requires-Dist: pygithub
 Requires-Dist: python-dotenv
 Requires-Dist: ray[default]>=2.8
 Requires-Dist: toml
 Requires-Dist: tqdm
+Requires-Dist: types-psutil
 Requires-Dist: types-toml
 Provides-Extra: all
 Requires-Dist: black[jupyter]; extra == 'all'
 Requires-Dist: hatch; extra == 'all'
 Requires-Dist: ipython; extra == 'all'
 Requires-Dist: mypy; extra == 'all'
 Requires-Dist: notebook; extra == 'all'
@@ -104,15 +106,15 @@
 pip install .
 ```
 
 
 ## Documentation
 
 * [Getting Started](https://leandojo.readthedocs.io/en/latest/getting-started.html)
-* Demos: [Lean 3](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo-lean3.ipynb), [Lean 4](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo-lean4.ipynb)
+* [Demo](https://github.com/lean-dojo/LeanDojo/blob/main/scripts/demo-lean4.ipynb)
 * [Full documentation](https://leandojo.readthedocs.io/en/latest/index.html)
 
 
 ## Questions and Bugs
 
 * For general questions and discussions, please use [GitHub Discussions](https://github.com/lean-dojo/LeanDojo/discussions).  
 * To report a potential bug, please open an issue. In the issue, please include your OS information, the version of LeanDojo, the exact steps to reproduce the error, and complete logs in debug mode (setting the environment variable `VERBOSE` to 1). The more details you provide, the better we will be able to help you.
```

