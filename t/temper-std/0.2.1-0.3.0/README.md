# Comparing `tmp/temper_std-0.2.1.tar.gz` & `tmp/temper_std-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_std-0.2.1.tar", max compression
+gzip compressed data, was "temper_std-0.3.0.tar", max compression
```

## Comparing `temper_std-0.2.1.tar` & `temper_std-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      998 2024-04-23 22:22:20.795323 temper_std-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       95 2024-04-23 22:22:20.805323 temper_std-0.2.1/temper_std/__init__.py
--rw-r--r--   0        0        0      106 2024-04-23 22:22:20.805323 temper_std-0.2.1/temper_std/__init__.py.map
--rw-r--r--   0        0        0    28586 2024-04-23 22:22:22.875323 temper_std-0.2.1/temper_std/regex.py
--rw-r--r--   0        0        0    50476 2024-04-23 22:22:23.085323 temper_std-0.2.1/temper_std/regex.py.map
--rw-r--r--   0        0        0     1974 2024-04-23 22:22:21.305323 temper_std-0.2.1/temper_std/temporal.py
--rw-r--r--   0        0        0     7395 2024-04-23 22:22:21.425323 temper_std-0.2.1/temper_std/temporal.py.map
--rw-r--r--   0        0        0     7174 2024-04-23 22:22:21.635323 temper_std-0.2.1/temper_std/testing.py
--rw-r--r--   0        0        0    14155 2024-04-23 22:22:21.935323 temper_std-0.2.1/temper_std/testing.py.map
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 temper_std-0.2.1/setup.py
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 temper_std-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      998 2024-05-28 15:06:56.857437 temper_std-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-05-28 15:06:56.857437 temper_std-0.3.0/temper_std/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-28 15:06:56.927438 temper_std-0.3.0/temper_std/__init__.py.map
+-rw-r--r--   0        0        0    28960 2024-05-28 15:06:57.177438 temper_std-0.3.0/temper_std/regex.py
+-rw-r--r--   0        0        0    51301 2024-05-28 15:06:57.187438 temper_std-0.3.0/temper_std/regex.py.map
+-rw-r--r--   0        0        0     2164 2024-05-28 15:06:56.967438 temper_std-0.3.0/temper_std/temporal.py
+-rw-r--r--   0        0        0     9649 2024-05-28 15:06:56.977438 temper_std-0.3.0/temper_std/temporal.py.map
+-rw-r--r--   0        0        0     7196 2024-05-28 15:06:57.017438 temper_std-0.3.0/temper_std/testing.py
+-rw-r--r--   0        0        0    14155 2024-05-28 15:06:57.017438 temper_std-0.3.0/temper_std/testing.py.map
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 temper_std-0.3.0/PKG-INFO
```

### Comparing `temper_std-0.2.1/pyproject.toml` & `temper_std-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [project]
 name = "temper-std"
-version = "0.2.1"
+version = "0.3.0"
 description = "Optional support library provided with Temper"
 readme = ""
 requires-python = "~=3.8"
 license = {text = "Apache-2.0"}
 authors = [ "Temper Contributors" ]
 homepage = "https://temperlang.dev/"
 repository = "https://github.com/temperlang/temper"
 maintainers = [ ]
 keywords = [ ]
 classifiers = [ ]
 urls = { }
 dependencies = [
-    "temper-core == 0.2.1"
+    "temper-core == 0.3.0"
 ]
 
 [project.scripts]
 
 [project.gui-scripts]
 
 [project.entry-points]
 
 
 [tool.poetry]
 name = "temper-std"
-version = "0.2.1"
+version = "0.3.0"
 license = "Apache-2.0"
 description = "Optional support library provided with Temper"
 authors = [ "Temper Contributors" ]
 homepage = "https://temperlang.dev/"
 repository = "https://github.com/temperlang/temper"
 packages = [{ include = "temper_std" }]
 include = ["temper_std/**/*", "./**/*.pyd", "./**/*.so"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-temper-core = "0.2.1"
+temper-core = "0.3.0"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `temper_std-0.2.1/temper_std/regex.py` & `temper_std-0.3.0/temper_std/regex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,763 +1,768 @@
 from abc import ABCMeta as ABCMeta0
-from builtins import str as str1, bool as bool2, int as int5, Exception as Exception12, RuntimeError as RuntimeError14, len as len_1254, list as list_1271
+from builtins import str as str1, bool as bool2, int as int5, RuntimeError as RuntimeError8, Exception as Exception15, len as len_1262, list as list_1279
 from types import MappingProxyType as MappingProxyType3
-from typing import Callable as Callable4, Sequence as Sequence6, Optional as Optional7, Union as Union8, Any as Any9, MutableSequence as MutableSequence10
-from temper_core import cast_by_type as cast_by_type11, Label as Label13, isinstance_int as isinstance_int15, cast_by_test as cast_by_test16, list_join as list_join_1242, generic_eq as generic_eq_1245, list_builder_add as list_builder_add_1246, string_code_points as string_code_points_1249, list_get as list_get_1255, str_cat as str_cat_1265, int_to_string as int_to_string_1266
-from temper_core.regex import compiled_regex_compile_formatted as compiled_regex_compile_formatted_1238, compiled_regex_compiled_found as compiled_regex_compiled_found_1239, compiled_regex_compiled_find as compiled_regex_compiled_find_1240, compiled_regex_compiled_replace as compiled_regex_compiled_replace_1241, regex_formatter_push_capture_name as regex_formatter_push_capture_name_1247, regex_formatter_push_code_to as regex_formatter_push_code_to_1248
-class Regex(metaclass = ABCMeta0):
-  def compiled(this__8) -> 'CompiledRegex':
-    return CompiledRegex(this__8)
-  def found(this__9, text__121: 'str1') -> 'bool2':
-    return this__9.compiled().found(text__121)
-  def find(this__10, text__124: 'str1') -> 'MappingProxyType3[str1, Group]':
-    return this__10.compiled().find(text__124)
-  def replace(this__11, text__127: 'str1', format__128: 'Callable4[[MappingProxyType3[str1, Group]], str1]') -> 'str1':
-    return this__11.compiled().replace(text__127, format__128)
-class Capture(Regex):
-  name__130: 'str1'
-  item__131: 'Regex'
-  __slots__ = ('name__130', 'item__131')
-  def constructor__132(this__50, name__133: 'str1', item__134: 'Regex') -> 'None':
-    this__50.name__130 = name__133
-    this__50.item__131 = item__134
-  def __init__(this__50, name__133: 'str1', item__134: 'Regex') -> None:
-    this__50.constructor__132(name__133, item__134)
-  @property
-  def name(this__330) -> 'str1':
-    return this__330.name__130
-  @property
-  def item(this__334) -> 'Regex':
-    return this__334.item__131
-class CodePart(Regex, metaclass = ABCMeta0):
+from typing import Callable as Callable4, TypeVar as TypeVar6, Generic as Generic7, Sequence as Sequence9, Optional as Optional10, Union as Union11, Any as Any12, MutableSequence as MutableSequence13
+from temper_core import cast_by_type as cast_by_type14, Label as Label16, isinstance_int as isinstance_int17, cast_by_test as cast_by_test18, list_join as list_join_1250, generic_eq as generic_eq_1253, list_builder_add as list_builder_add_1254, string_code_points as string_code_points_1257, list_get as list_get_1263, str_cat as str_cat_1273, int_to_string as int_to_string_1274
+from temper_core.regex import regex_compile_formatted as regex_compile_formatted_1246, regex_compiled_found as regex_compiled_found_1247, regex_compiled_find as regex_compiled_find_1248, regex_compiled_replace as regex_compiled_replace_1249, regex_formatter_push_capture_name as regex_formatter_push_capture_name_1255, regex_formatter_push_code_to as regex_formatter_push_code_to_1256
+class RegexNode(metaclass = ABCMeta0):
+  def compiled(this__8) -> 'Regex':
+    return Regex(this__8)
+  def found(this__9, text__125: 'str1') -> 'bool2':
+    return this__9.compiled().found(text__125)
+  def find(this__10, text__128: 'str1') -> 'MappingProxyType3[str1, Group]':
+    return this__10.compiled().find(text__128)
+  def replace(this__11, text__131: 'str1', format__132: 'Callable4[[MappingProxyType3[str1, Group]], str1]') -> 'str1':
+    return this__11.compiled().replace(text__131, format__132)
+class Capture(RegexNode):
+  name__134: 'str1'
+  item__135: 'RegexNode'
+  __slots__ = ('name__134', 'item__135')
+  def constructor__136(this__52, name__137: 'str1', item__138: 'RegexNode') -> 'None':
+    this__52.name__134 = name__137
+    this__52.item__135 = item__138
+  def __init__(this__52, name__137: 'str1', item__138: 'RegexNode') -> None:
+    this__52.constructor__136(name__137, item__138)
+  @property
+  def name(this__336) -> 'str1':
+    return this__336.name__134
+  @property
+  def item(this__340) -> 'RegexNode':
+    return this__340.item__135
+class CodePart(RegexNode, metaclass = ABCMeta0):
   pass
 class CodePoints(CodePart):
-  value__135: 'str1'
-  __slots__ = ('value__135',)
-  def constructor__136(this__52, value__137: 'str1') -> 'None':
-    this__52.value__135 = value__137
-  def __init__(this__52, value__137: 'str1') -> None:
-    this__52.constructor__136(value__137)
-  @property
-  def value(this__310) -> 'str1':
-    return this__310.value__135
-class Special(Regex, metaclass = ABCMeta0):
+  value__139: 'str1'
+  __slots__ = ('value__139',)
+  def constructor__140(this__54, value__141: 'str1') -> 'None':
+    this__54.value__139 = value__141
+  def __init__(this__54, value__141: 'str1') -> None:
+    this__54.constructor__140(value__141)
+  @property
+  def value(this__316) -> 'str1':
+    return this__316.value__139
+class Special(RegexNode, metaclass = ABCMeta0):
   pass
 class SpecialSet(CodePart, Special, metaclass = ABCMeta0):
   pass
 class CodeRange(CodePart):
-  min__145: 'int5'
-  max__146: 'int5'
-  __slots__ = ('min__145', 'max__146')
-  def constructor__147(this__68, min__148: 'int5', max__149: 'int5') -> 'None':
-    this__68.min__145 = min__148
-    this__68.max__146 = max__149
-  def __init__(this__68, min__148: 'int5', max__149: 'int5') -> None:
-    this__68.constructor__147(min__148, max__149)
-  @property
-  def min(this__338) -> 'int5':
-    return this__338.min__145
-  @property
-  def max(this__342) -> 'int5':
-    return this__342.max__146
-class CodeSet(Regex):
-  items__150: 'Sequence6[CodePart]'
-  negated__151: 'bool2'
-  __slots__ = ('items__150', 'negated__151')
-  def constructor__152(this__70, items__153: 'Sequence6[CodePart]', negated: Optional7['bool2'] = None) -> 'None':
-    negated__154: Optional7['bool2'] = negated
-    if negated__154 is None:
-      negated__154 = False
-    this__70.items__150 = items__153
-    this__70.negated__151 = negated__154
-  def __init__(this__70, items__153: 'Sequence6[CodePart]', negated: Optional7['bool2'] = None) -> None:
-    negated__154: Optional7['bool2'] = negated
-    this__70.constructor__152(items__153, negated__154)
-  @property
-  def items(this__346) -> 'Sequence6[CodePart]':
-    return this__346.items__150
-  @property
-  def negated(this__350) -> 'bool2':
-    return this__350.negated__151
-class Or(Regex):
-  items__155: 'Sequence6[Regex]'
-  __slots__ = ('items__155',)
-  def constructor__156(this__73, items__157: 'Sequence6[Regex]') -> 'None':
-    this__73.items__155 = items__157
-  def __init__(this__73, items__157: 'Sequence6[Regex]') -> None:
-    this__73.constructor__156(items__157)
-  @property
-  def items(this__314) -> 'Sequence6[Regex]':
-    return this__314.items__155
-class Repeat(Regex):
-  item__158: 'Regex'
-  min__159: 'int5'
-  max__160: 'Union8[int5, None]'
-  reluctant__161: 'bool2'
-  __slots__ = ('item__158', 'min__159', 'max__160', 'reluctant__161')
-  def constructor__162(this__76, item__163: 'Regex', min__164: 'int5', max__165: 'Union8[int5, None]', reluctant: Optional7['bool2'] = None) -> 'None':
-    reluctant__166: Optional7['bool2'] = reluctant
-    if reluctant__166 is None:
-      reluctant__166 = False
-    this__76.item__158 = item__163
-    this__76.min__159 = min__164
-    this__76.max__160 = max__165
-    this__76.reluctant__161 = reluctant__166
-  def __init__(this__76, item__163: 'Regex', min__164: 'int5', max__165: 'Union8[int5, None]', reluctant: Optional7['bool2'] = None) -> None:
-    reluctant__166: Optional7['bool2'] = reluctant
-    this__76.constructor__162(item__163, min__164, max__165, reluctant__166)
-  @property
-  def item(this__354) -> 'Regex':
-    return this__354.item__158
-  @property
-  def min(this__358) -> 'int5':
-    return this__358.min__159
-  @property
-  def max(this__362) -> 'Union8[int5, None]':
-    return this__362.max__160
-  @property
-  def reluctant(this__366) -> 'bool2':
-    return this__366.reluctant__161
-class Sequence(Regex):
-  items__175: 'Sequence6[Regex]'
-  __slots__ = ('items__175',)
-  def constructor__176(this__82, items__177: 'Sequence6[Regex]') -> 'None':
-    this__82.items__175 = items__177
-  def __init__(this__82, items__177: 'Sequence6[Regex]') -> None:
-    this__82.constructor__176(items__177)
+  min__149: 'int5'
+  max__150: 'int5'
+  __slots__ = ('min__149', 'max__150')
+  def constructor__151(this__70, min__152: 'int5', max__153: 'int5') -> 'None':
+    this__70.min__149 = min__152
+    this__70.max__150 = max__153
+  def __init__(this__70, min__152: 'int5', max__153: 'int5') -> None:
+    this__70.constructor__151(min__152, max__153)
+  @property
+  def min(this__344) -> 'int5':
+    return this__344.min__149
+  @property
+  def max(this__348) -> 'int5':
+    return this__348.max__150
+ITEM__19 = TypeVar6('ITEM__19', covariant = True)
+class ItemizedRegex(Generic7[ITEM__19], RegexNode, metaclass = ABCMeta0):
+  @property
+  def items(this__20) -> 'Sequence9[ITEM__19]':
+    raise RuntimeError8()
+class CodeSet(ItemizedRegex[CodePart]):
+  items__156: 'Sequence9[CodePart]'
+  negated__157: 'bool2'
+  __slots__ = ('items__156', 'negated__157')
+  def constructor__158(this__74, items__159: 'Sequence9[CodePart]', negated: Optional10['bool2'] = None) -> 'None':
+    negated__160: Optional10['bool2'] = negated
+    if negated__160 is None:
+      negated__160 = False
+    this__74.items__156 = items__159
+    this__74.negated__157 = negated__160
+  def __init__(this__74, items__159: 'Sequence9[CodePart]', negated: Optional10['bool2'] = None) -> None:
+    negated__160: Optional10['bool2'] = negated
+    this__74.constructor__158(items__159, negated__160)
+  @property
+  def items(this__352) -> 'Sequence9[CodePart]':
+    return this__352.items__156
+  @property
+  def negated(this__356) -> 'bool2':
+    return this__356.negated__157
+class Or(ItemizedRegex[RegexNode]):
+  items__161: 'Sequence9[RegexNode]'
+  __slots__ = ('items__161',)
+  def constructor__162(this__77, items__163: 'Sequence9[RegexNode]') -> 'None':
+    this__77.items__161 = items__163
+  def __init__(this__77, items__163: 'Sequence9[RegexNode]') -> None:
+    this__77.constructor__162(items__163)
+  @property
+  def items(this__320) -> 'Sequence9[RegexNode]':
+    return this__320.items__161
+class Repeat(RegexNode):
+  item__164: 'RegexNode'
+  min__165: 'int5'
+  max__166: 'Union11[int5, None]'
+  reluctant__167: 'bool2'
+  __slots__ = ('item__164', 'min__165', 'max__166', 'reluctant__167')
+  def constructor__168(this__80, item__169: 'RegexNode', min__170: 'int5', max__171: 'Union11[int5, None]', reluctant: Optional10['bool2'] = None) -> 'None':
+    reluctant__172: Optional10['bool2'] = reluctant
+    if reluctant__172 is None:
+      reluctant__172 = False
+    this__80.item__164 = item__169
+    this__80.min__165 = min__170
+    this__80.max__166 = max__171
+    this__80.reluctant__167 = reluctant__172
+  def __init__(this__80, item__169: 'RegexNode', min__170: 'int5', max__171: 'Union11[int5, None]', reluctant: Optional10['bool2'] = None) -> None:
+    reluctant__172: Optional10['bool2'] = reluctant
+    this__80.constructor__168(item__169, min__170, max__171, reluctant__172)
+  @property
+  def item(this__360) -> 'RegexNode':
+    return this__360.item__164
+  @property
+  def min(this__364) -> 'int5':
+    return this__364.min__165
+  @property
+  def max(this__368) -> 'Union11[int5, None]':
+    return this__368.max__166
+  @property
+  def reluctant(this__372) -> 'bool2':
+    return this__372.reluctant__167
+class Sequence(ItemizedRegex[RegexNode]):
+  items__181: 'Sequence9[RegexNode]'
+  __slots__ = ('items__181',)
+  def constructor__182(this__86, items__183: 'Sequence9[RegexNode]') -> 'None':
+    this__86.items__181 = items__183
+  def __init__(this__86, items__183: 'Sequence9[RegexNode]') -> None:
+    this__86.constructor__182(items__183)
   @property
-  def items(this__370) -> 'Sequence6[Regex]':
-    return this__370.items__175
+  def items(this__376) -> 'Sequence9[RegexNode]':
+    return this__376.items__181
 class Group:
-  name__178: 'str1'
-  value__179: 'str1'
-  codePointsBegin__180: 'int5'
-  __slots__ = ('name__178', 'value__179', 'codePointsBegin__180')
-  def constructor__181(this__85, name__182: 'str1', value__183: 'str1', codePointsBegin__184: 'int5') -> 'None':
-    this__85.name__178 = name__182
-    this__85.value__179 = value__183
-    this__85.codePointsBegin__180 = codePointsBegin__184
-  def __init__(this__85, name__182: 'str1', value__183: 'str1', codePointsBegin__184: 'int5') -> None:
-    this__85.constructor__181(name__182, value__183, codePointsBegin__184)
-  @property
-  def name(this__298) -> 'str1':
-    return this__298.name__178
-  @property
-  def value(this__302) -> 'str1':
-    return this__302.value__179
-  @property
-  def code_points_begin(this__306) -> 'int5':
-    return this__306.codePointsBegin__180
-class RegexRefs__19:
-  codePoints__185: 'CodePoints'
-  group__186: 'Group'
-  orObject__187: 'Or'
-  __slots__ = ('codePoints__185', 'group__186', 'orObject__187')
-  def constructor__188(this__87, code_points: Optional7['CodePoints'] = None, group: Optional7['Group'] = None, or_object: Optional7['Or'] = None) -> 'None':
-    codePoints__189: Optional7['CodePoints'] = code_points
-    group__190: Optional7['Group'] = group
-    orObject__191: Optional7['Or'] = or_object
-    t_1206: 'CodePoints'
-    t_1208: 'Group'
-    t_1210: 'Or'
-    if codePoints__189 is None:
-      t_1206 = CodePoints('')
-      codePoints__189 = t_1206
-    if group__190 is None:
-      t_1208 = Group('', '', 0)
-      group__190 = t_1208
-    if orObject__191 is None:
-      t_1210 = Or(())
-      orObject__191 = t_1210
-    this__87.codePoints__185 = codePoints__189
-    this__87.group__186 = group__190
-    this__87.orObject__187 = orObject__191
-  def __init__(this__87, code_points: Optional7['CodePoints'] = None, group: Optional7['Group'] = None, or_object: Optional7['Or'] = None) -> None:
-    codePoints__189: Optional7['CodePoints'] = code_points
-    group__190: Optional7['Group'] = group
-    orObject__191: Optional7['Or'] = or_object
-    this__87.constructor__188(codePoints__189, group__190, orObject__191)
-  @property
-  def code_points(this__318) -> 'CodePoints':
-    return this__318.codePoints__185
-  @property
-  def group(this__322) -> 'Group':
-    return this__322.group__186
-  @property
-  def or_object(this__326) -> 'Or':
-    return this__326.orObject__187
-class CompiledRegex:
-  data__192: 'Regex'
-  compiled__206: 'Any9'
-  __slots__ = ('data__192', 'compiled__206')
-  def constructor__193(this__20, data__194: 'Regex') -> 'None':
-    this__20.data__192 = data__194
-    t_1080: 'str1' = this__20.format__225()
-    t_1081: 'Any9' = compiled_regex_compile_formatted_1238(this__20, t_1080)
-    this__20.compiled__206 = t_1081
-  def __init__(this__20, data__194: 'Regex') -> None:
-    this__20.constructor__193(data__194)
-  def found(this__21, text__197: 'str1') -> 'bool2':
-    return compiled_regex_compiled_found_1239(this__21, this__21.compiled__206, text__197)
-  def find(this__22, text__200: 'str1') -> 'MappingProxyType3[str1, Group]':
-    return compiled_regex_compiled_find_1240(this__22, this__22.compiled__206, text__200, regexRefs__117)
-  def replace(this__23, text__203: 'str1', format__204: 'Callable4[[MappingProxyType3[str1, Group]], str1]') -> 'str1':
-    return compiled_regex_compiled_replace_1241(this__23, this__23.compiled__206, text__203, format__204, regexRefs__117)
-  def format__225(this__28) -> 'str1':
-    return RegexFormatter__29().format(this__28.data__192)
-  @property
-  def data(this__408) -> 'Regex':
-    return this__408.data__192
-class RegexFormatter__29:
-  out__227: 'MutableSequence10[str1]'
-  __slots__ = ('out__227',)
-  def format(this__30, regex__229: 'Regex') -> 'str1':
-    this__30.pushRegex__232(regex__229)
-    t_1175: 'MutableSequence10[str1]' = this__30.out__227
-    def fn__1172(x__231: 'str1') -> 'str1':
-      return x__231
-    return list_join_1242(t_1175, '', fn__1172)
-  def pushRegex__232(this__31, regex__233: 'Regex') -> 'None':
-    t_764: 'bool2'
-    t_765: 'Capture'
-    t_768: 'bool2'
-    t_769: 'CodePoints'
-    t_772: 'bool2'
-    t_773: 'CodeRange'
-    t_776: 'bool2'
-    t_777: 'CodeSet'
-    t_780: 'bool2'
-    t_781: 'Or'
-    t_784: 'bool2'
-    t_785: 'Repeat'
-    t_788: 'bool2'
-    t_789: 'Sequence'
+  name__184: 'str1'
+  value__185: 'str1'
+  codePointsBegin__186: 'int5'
+  __slots__ = ('name__184', 'value__185', 'codePointsBegin__186')
+  def constructor__187(this__89, name__188: 'str1', value__189: 'str1', codePointsBegin__190: 'int5') -> 'None':
+    this__89.name__184 = name__188
+    this__89.value__185 = value__189
+    this__89.codePointsBegin__186 = codePointsBegin__190
+  def __init__(this__89, name__188: 'str1', value__189: 'str1', codePointsBegin__190: 'int5') -> None:
+    this__89.constructor__187(name__188, value__189, codePointsBegin__190)
+  @property
+  def name(this__304) -> 'str1':
+    return this__304.name__184
+  @property
+  def value(this__308) -> 'str1':
+    return this__308.value__185
+  @property
+  def code_points_begin(this__312) -> 'int5':
+    return this__312.codePointsBegin__186
+class RegexRefs__21:
+  codePoints__191: 'CodePoints'
+  group__192: 'Group'
+  orObject__193: 'Or'
+  __slots__ = ('codePoints__191', 'group__192', 'orObject__193')
+  def constructor__194(this__91, code_points: Optional10['CodePoints'] = None, group: Optional10['Group'] = None, or_object: Optional10['Or'] = None) -> 'None':
+    codePoints__195: Optional10['CodePoints'] = code_points
+    group__196: Optional10['Group'] = group
+    orObject__197: Optional10['Or'] = or_object
+    t_1213: 'CodePoints'
+    t_1215: 'Group'
+    t_1217: 'Or'
+    if codePoints__195 is None:
+      t_1213 = CodePoints('')
+      codePoints__195 = t_1213
+    if group__196 is None:
+      t_1215 = Group('', '', 0)
+      group__196 = t_1215
+    if orObject__197 is None:
+      t_1217 = Or(())
+      orObject__197 = t_1217
+    this__91.codePoints__191 = codePoints__195
+    this__91.group__192 = group__196
+    this__91.orObject__193 = orObject__197
+  def __init__(this__91, code_points: Optional10['CodePoints'] = None, group: Optional10['Group'] = None, or_object: Optional10['Or'] = None) -> None:
+    codePoints__195: Optional10['CodePoints'] = code_points
+    group__196: Optional10['Group'] = group
+    orObject__197: Optional10['Or'] = or_object
+    this__91.constructor__194(codePoints__195, group__196, orObject__197)
+  @property
+  def code_points(this__324) -> 'CodePoints':
+    return this__324.codePoints__191
+  @property
+  def group(this__328) -> 'Group':
+    return this__328.group__192
+  @property
+  def or_object(this__332) -> 'Or':
+    return this__332.orObject__193
+class Regex:
+  data__198: 'RegexNode'
+  compiled__212: 'Any12'
+  __slots__ = ('data__198', 'compiled__212')
+  def constructor__199(this__22, data__200: 'RegexNode') -> 'None':
+    this__22.data__198 = data__200
+    t_1087: 'str1' = this__22.format__231()
+    t_1088: 'Any12' = regex_compile_formatted_1246(this__22, t_1087)
+    this__22.compiled__212 = t_1088
+  def __init__(this__22, data__200: 'RegexNode') -> None:
+    this__22.constructor__199(data__200)
+  def found(this__23, text__203: 'str1') -> 'bool2':
+    return regex_compiled_found_1247(this__23, this__23.compiled__212, text__203)
+  def find(this__24, text__206: 'str1') -> 'MappingProxyType3[str1, Group]':
+    return regex_compiled_find_1248(this__24, this__24.compiled__212, text__206, regexRefs__121)
+  def replace(this__25, text__209: 'str1', format__210: 'Callable4[[MappingProxyType3[str1, Group]], str1]') -> 'str1':
+    return regex_compiled_replace_1249(this__25, this__25.compiled__212, text__209, format__210, regexRefs__121)
+  def format__231(this__30) -> 'str1':
+    return RegexFormatter__31().format(this__30.data__198)
+  @property
+  def data(this__414) -> 'RegexNode':
+    return this__414.data__198
+class RegexFormatter__31:
+  out__233: 'MutableSequence13[str1]'
+  __slots__ = ('out__233',)
+  def format(this__32, regex__235: 'RegexNode') -> 'str1':
+    this__32.pushRegex__238(regex__235)
+    t_1182: 'MutableSequence13[str1]' = this__32.out__233
+    def fn__1179(x__237: 'str1') -> 'str1':
+      return x__237
+    return list_join_1250(t_1182, '', fn__1179)
+  def pushRegex__238(this__33, regex__239: 'RegexNode') -> 'None':
+    t_770: 'bool2'
+    t_771: 'Capture'
+    t_774: 'bool2'
+    t_775: 'CodePoints'
+    t_778: 'bool2'
+    t_779: 'CodeRange'
+    t_782: 'bool2'
+    t_783: 'CodeSet'
+    t_786: 'bool2'
+    t_787: 'Or'
+    t_790: 'bool2'
+    t_791: 'Repeat'
+    t_794: 'bool2'
+    t_795: 'Sequence'
     try:
-      cast_by_type11(regex__233, Capture)
-      t_764 = True
-    except Exception12:
-      t_764 = False
-    with Label13() as s__1243_1244:
-      if t_764:
+      cast_by_type14(regex__239, Capture)
+      t_770 = True
+    except Exception15:
+      t_770 = False
+    with Label16() as s__1251_1252:
+      if t_770:
         try:
-          t_765 = cast_by_type11(regex__233, Capture)
-        except Exception12:
-          s__1243_1244.break_()
-        this__31.pushCapture__235(t_765)
+          t_771 = cast_by_type14(regex__239, Capture)
+        except Exception15:
+          s__1251_1252.break_()
+        this__33.pushCapture__241(t_771)
       else:
         try:
-          cast_by_type11(regex__233, CodePoints)
-          t_768 = True
-        except Exception12:
-          t_768 = False
-        if t_768:
-          try:
-            t_769 = cast_by_type11(regex__233, CodePoints)
-          except Exception12:
-            s__1243_1244.break_()
-          this__31.pushCodePoints__251(t_769, False)
+          cast_by_type14(regex__239, CodePoints)
+          t_774 = True
+        except Exception15:
+          t_774 = False
+        if t_774:
+          try:
+            t_775 = cast_by_type14(regex__239, CodePoints)
+          except Exception15:
+            s__1251_1252.break_()
+          this__33.pushCodePoints__257(t_775, False)
         else:
           try:
-            cast_by_type11(regex__233, CodeRange)
-            t_772 = True
-          except Exception12:
-            t_772 = False
-          if t_772:
+            cast_by_type14(regex__239, CodeRange)
+            t_778 = True
+          except Exception15:
+            t_778 = False
+          if t_778:
             try:
-              t_773 = cast_by_type11(regex__233, CodeRange)
-            except Exception12:
-              s__1243_1244.break_()
-            this__31.pushCodeRange__256(t_773)
+              t_779 = cast_by_type14(regex__239, CodeRange)
+            except Exception15:
+              s__1251_1252.break_()
+            this__33.pushCodeRange__262(t_779)
           else:
             try:
-              cast_by_type11(regex__233, CodeSet)
-              t_776 = True
-            except Exception12:
-              t_776 = False
-            if t_776:
+              cast_by_type14(regex__239, CodeSet)
+              t_782 = True
+            except Exception15:
+              t_782 = False
+            if t_782:
               try:
-                t_777 = cast_by_type11(regex__233, CodeSet)
-              except Exception12:
-                s__1243_1244.break_()
-              this__31.pushCodeSet__262(t_777)
+                t_783 = cast_by_type14(regex__239, CodeSet)
+              except Exception15:
+                s__1251_1252.break_()
+              this__33.pushCodeSet__268(t_783)
             else:
               try:
-                cast_by_type11(regex__233, Or)
-                t_780 = True
-              except Exception12:
-                t_780 = False
-              if t_780:
+                cast_by_type14(regex__239, Or)
+                t_786 = True
+              except Exception15:
+                t_786 = False
+              if t_786:
                 try:
-                  t_781 = cast_by_type11(regex__233, Or)
-                except Exception12:
-                  s__1243_1244.break_()
-                this__31.pushOr__274(t_781)
+                  t_787 = cast_by_type14(regex__239, Or)
+                except Exception15:
+                  s__1251_1252.break_()
+                this__33.pushOr__280(t_787)
               else:
                 try:
-                  cast_by_type11(regex__233, Repeat)
-                  t_784 = True
-                except Exception12:
-                  t_784 = False
-                if t_784:
+                  cast_by_type14(regex__239, Repeat)
+                  t_790 = True
+                except Exception15:
+                  t_790 = False
+                if t_790:
                   try:
-                    t_785 = cast_by_type11(regex__233, Repeat)
-                  except Exception12:
-                    s__1243_1244.break_()
-                  this__31.pushRepeat__278(t_785)
+                    t_791 = cast_by_type14(regex__239, Repeat)
+                  except Exception15:
+                    s__1251_1252.break_()
+                  this__33.pushRepeat__284(t_791)
                 else:
                   try:
-                    cast_by_type11(regex__233, Sequence)
-                    t_788 = True
-                  except Exception12:
-                    t_788 = False
-                  if t_788:
+                    cast_by_type14(regex__239, Sequence)
+                    t_794 = True
+                  except Exception15:
+                    t_794 = False
+                  if t_794:
                     try:
-                      t_789 = cast_by_type11(regex__233, Sequence)
-                    except Exception12:
-                      s__1243_1244.break_()
-                    this__31.pushSequence__283(t_789)
-                  elif generic_eq_1245(regex__233, begin):
+                      t_795 = cast_by_type14(regex__239, Sequence)
+                    except Exception15:
+                      s__1251_1252.break_()
+                    this__33.pushSequence__289(t_795)
+                  elif generic_eq_1253(regex__239, begin):
                     try:
-                      list_builder_add_1246(this__31.out__227, '^')
-                    except Exception12:
-                      s__1243_1244.break_()
-                  elif generic_eq_1245(regex__233, dot):
+                      list_builder_add_1254(this__33.out__233, '^')
+                    except Exception15:
+                      s__1251_1252.break_()
+                  elif generic_eq_1253(regex__239, dot):
                     try:
-                      list_builder_add_1246(this__31.out__227, '.')
-                    except Exception12:
-                      s__1243_1244.break_()
-                  elif generic_eq_1245(regex__233, end):
+                      list_builder_add_1254(this__33.out__233, '.')
+                    except Exception15:
+                      s__1251_1252.break_()
+                  elif generic_eq_1253(regex__239, end):
                     try:
-                      list_builder_add_1246(this__31.out__227, '$')
-                    except Exception12:
-                      s__1243_1244.break_()
-                  elif generic_eq_1245(regex__233, word_boundary):
+                      list_builder_add_1254(this__33.out__233, '$')
+                    except Exception15:
+                      s__1251_1252.break_()
+                  elif generic_eq_1253(regex__239, word_boundary):
                     try:
-                      list_builder_add_1246(this__31.out__227, '\\b')
-                    except Exception12:
-                      s__1243_1244.break_()
-                  elif generic_eq_1245(regex__233, digit):
+                      list_builder_add_1254(this__33.out__233, '\\b')
+                    except Exception15:
+                      s__1251_1252.break_()
+                  elif generic_eq_1253(regex__239, digit):
                     try:
-                      list_builder_add_1246(this__31.out__227, '\\d')
-                    except Exception12:
-                      s__1243_1244.break_()
-                  elif generic_eq_1245(regex__233, space):
+                      list_builder_add_1254(this__33.out__233, '\\d')
+                    except Exception15:
+                      s__1251_1252.break_()
+                  elif generic_eq_1253(regex__239, space):
                     try:
-                      list_builder_add_1246(this__31.out__227, '\\s')
-                    except Exception12:
-                      s__1243_1244.break_()
-                  elif generic_eq_1245(regex__233, word):
+                      list_builder_add_1254(this__33.out__233, '\\s')
+                    except Exception15:
+                      s__1251_1252.break_()
+                  elif generic_eq_1253(regex__239, word):
                     try:
-                      list_builder_add_1246(this__31.out__227, '\\w')
-                    except Exception12:
-                      s__1243_1244.break_()
+                      list_builder_add_1254(this__33.out__233, '\\w')
+                    except Exception15:
+                      s__1251_1252.break_()
                   else:
                     None
       return
-    raise RuntimeError14()
-  def pushCapture__235(this__32, capture__236: 'Capture') -> 'None':
-    list_builder_add_1246(this__32.out__227, '(')
-    t_759: 'MutableSequence10[str1]' = this__32.out__227
-    t_1159: 'str1' = capture__236.name
-    regex_formatter_push_capture_name_1247(this__32, t_759, t_1159)
-    t_1160: 'Regex' = capture__236.item
-    this__32.pushRegex__232(t_1160)
-    list_builder_add_1246(this__32.out__227, ')')
-  def pushCode__242(this__34, code__243: 'int5', insideCodeSet__244: 'bool2') -> 'None':
-    regex_formatter_push_code_to_1248(this__34, this__34.out__227, code__243, insideCodeSet__244)
-  def pushCodePoints__251(this__36, codePoints__252: 'CodePoints', insideCodeSet__253: 'bool2') -> 'None':
-    t_1148: 'int5'
-    t_1149: 'Any9'
-    t_1153: 'Any9' = string_code_points_1249(codePoints__252.value)
-    slice__255: 'Any9' = t_1153
+    raise RuntimeError8()
+  def pushCapture__241(this__34, capture__242: 'Capture') -> 'None':
+    list_builder_add_1254(this__34.out__233, '(')
+    t_765: 'MutableSequence13[str1]' = this__34.out__233
+    t_1166: 'str1' = capture__242.name
+    regex_formatter_push_capture_name_1255(this__34, t_765, t_1166)
+    t_1167: 'RegexNode' = capture__242.item
+    this__34.pushRegex__238(t_1167)
+    list_builder_add_1254(this__34.out__233, ')')
+  def pushCode__248(this__36, code__249: 'int5', insideCodeSet__250: 'bool2') -> 'None':
+    regex_formatter_push_code_to_1256(this__36, this__36.out__233, code__249, insideCodeSet__250)
+  def pushCodePoints__257(this__38, codePoints__258: 'CodePoints', insideCodeSet__259: 'bool2') -> 'None':
+    t_1155: 'int5'
+    t_1156: 'Any12'
+    t_1160: 'Any12' = string_code_points_1257(codePoints__258.value)
+    slice__261: 'Any12' = t_1160
     while True:
-      if not slice__255.is_empty:
-        t_1148 = slice__255.read()
-        this__36.pushCode__242(t_1148, insideCodeSet__253)
-        t_1149 = slice__255.advance(1)
-        slice__255 = t_1149
+      if not slice__261.is_empty:
+        t_1155 = slice__261.read()
+        this__38.pushCode__248(t_1155, insideCodeSet__259)
+        t_1156 = slice__261.advance(1)
+        slice__261 = t_1156
       else:
         break
-  def pushCodeRange__256(this__37, codeRange__257: 'CodeRange') -> 'None':
-    list_builder_add_1246(this__37.out__227, '[')
-    this__37.pushCodeRangeUnwrapped__259(codeRange__257)
-    list_builder_add_1246(this__37.out__227, ']')
-  def pushCodeRangeUnwrapped__259(this__38, codeRange__260: 'CodeRange') -> 'None':
-    t_1141: 'int5' = codeRange__260.min
-    this__38.pushCode__242(t_1141, True)
-    list_builder_add_1246(this__38.out__227, '-')
-    t_1143: 'int5' = codeRange__260.max
-    this__38.pushCode__242(t_1143, True)
-  def pushCodeSet__262(this__39, codeSet__263: 'CodeSet') -> 'None':
-    t_1137: 'int5'
-    t_737: 'bool2'
-    t_738: 'CodeSet'
-    t_743: 'CodePart'
-    adjusted__265: 'Regex' = this__39.adjustCodeSet__267(codeSet__263, regexRefs__117)
+  def pushCodeRange__262(this__39, codeRange__263: 'CodeRange') -> 'None':
+    list_builder_add_1254(this__39.out__233, '[')
+    this__39.pushCodeRangeUnwrapped__265(codeRange__263)
+    list_builder_add_1254(this__39.out__233, ']')
+  def pushCodeRangeUnwrapped__265(this__40, codeRange__266: 'CodeRange') -> 'None':
+    t_1148: 'int5' = codeRange__266.min
+    this__40.pushCode__248(t_1148, True)
+    list_builder_add_1254(this__40.out__233, '-')
+    t_1150: 'int5' = codeRange__266.max
+    this__40.pushCode__248(t_1150, True)
+  def pushCodeSet__268(this__41, codeSet__269: 'CodeSet') -> 'None':
+    t_1144: 'int5'
+    t_743: 'bool2'
+    t_744: 'CodeSet'
+    t_749: 'CodePart'
+    adjusted__271: 'RegexNode' = this__41.adjustCodeSet__273(codeSet__269, regexRefs__121)
     try:
-      cast_by_type11(adjusted__265, CodeSet)
-      t_737 = True
-    except Exception12:
-      t_737 = False
-    with Label13() as s__1250_1252:
-      if t_737:
-        with Label13() as s__1251_1253:
-          try:
-            t_738 = cast_by_type11(adjusted__265, CodeSet)
-            list_builder_add_1246(this__39.out__227, '[')
-          except Exception12:
-            s__1251_1253.break_()
-          if t_738.negated:
+      cast_by_type14(adjusted__271, CodeSet)
+      t_743 = True
+    except Exception15:
+      t_743 = False
+    with Label16() as s__1258_1260:
+      if t_743:
+        with Label16() as s__1259_1261:
+          try:
+            t_744 = cast_by_type14(adjusted__271, CodeSet)
+            list_builder_add_1254(this__41.out__233, '[')
+          except Exception15:
+            s__1259_1261.break_()
+          if t_744.negated:
             try:
-              list_builder_add_1246(this__39.out__227, '^')
-            except Exception12:
-              s__1251_1253.break_()
+              list_builder_add_1254(this__41.out__233, '^')
+            except Exception15:
+              s__1259_1261.break_()
           else:
             None
-          i__266: 'int5' = 0
+          i__272: 'int5' = 0
           while True:
-            t_1137 = len_1254(t_738.items)
-            if i__266 < t_1137:
+            t_1144 = len_1262(t_744.items)
+            if i__272 < t_1144:
               try:
-                t_743 = list_get_1255(t_738.items, i__266)
-              except Exception12:
-                s__1251_1253.break_()
-              this__39.pushCodeSetItem__271(t_743)
-              i__266 = i__266 + 1
+                t_749 = list_get_1263(t_744.items, i__272)
+              except Exception15:
+                s__1259_1261.break_()
+              this__41.pushCodeSetItem__277(t_749)
+              i__272 = i__272 + 1
             else:
               break
           try:
-            list_builder_add_1246(this__39.out__227, ']')
-            s__1250_1252.break_()
-          except Exception12:
+            list_builder_add_1254(this__41.out__233, ']')
+            s__1258_1260.break_()
+          except Exception15:
             pass
-        raise RuntimeError14()
-      this__39.pushRegex__232(adjusted__265)
-  def adjustCodeSet__267(this__40, codeSet__268: 'CodeSet', regexRefs__269: 'RegexRefs__19') -> 'Regex':
-    return codeSet__268
-  def pushCodeSetItem__271(this__41, codePart__272: 'CodePart') -> 'None':
-    t_724: 'bool2'
-    t_725: 'CodePoints'
-    t_728: 'bool2'
-    t_729: 'CodeRange'
-    t_732: 'bool2'
-    t_733: 'SpecialSet'
+        raise RuntimeError8()
+      this__41.pushRegex__238(adjusted__271)
+  def adjustCodeSet__273(this__42, codeSet__274: 'CodeSet', regexRefs__275: 'RegexRefs__21') -> 'RegexNode':
+    return codeSet__274
+  def pushCodeSetItem__277(this__43, codePart__278: 'CodePart') -> 'None':
+    t_730: 'bool2'
+    t_731: 'CodePoints'
+    t_734: 'bool2'
+    t_735: 'CodeRange'
+    t_738: 'bool2'
+    t_739: 'SpecialSet'
     try:
-      cast_by_type11(codePart__272, CodePoints)
-      t_724 = True
-    except Exception12:
-      t_724 = False
-    with Label13() as s__1256_1257:
-      if t_724:
+      cast_by_type14(codePart__278, CodePoints)
+      t_730 = True
+    except Exception15:
+      t_730 = False
+    with Label16() as s__1264_1265:
+      if t_730:
         try:
-          t_725 = cast_by_type11(codePart__272, CodePoints)
-        except Exception12:
-          s__1256_1257.break_()
-        this__41.pushCodePoints__251(t_725, True)
+          t_731 = cast_by_type14(codePart__278, CodePoints)
+        except Exception15:
+          s__1264_1265.break_()
+        this__43.pushCodePoints__257(t_731, True)
       else:
         try:
-          cast_by_type11(codePart__272, CodeRange)
-          t_728 = True
-        except Exception12:
-          t_728 = False
-        if t_728:
-          try:
-            t_729 = cast_by_type11(codePart__272, CodeRange)
-          except Exception12:
-            s__1256_1257.break_()
-          this__41.pushCodeRangeUnwrapped__259(t_729)
+          cast_by_type14(codePart__278, CodeRange)
+          t_734 = True
+        except Exception15:
+          t_734 = False
+        if t_734:
+          try:
+            t_735 = cast_by_type14(codePart__278, CodeRange)
+          except Exception15:
+            s__1264_1265.break_()
+          this__43.pushCodeRangeUnwrapped__265(t_735)
         else:
           try:
-            cast_by_type11(codePart__272, SpecialSet)
-            t_732 = True
-          except Exception12:
-            t_732 = False
-          if t_732:
+            cast_by_type14(codePart__278, SpecialSet)
+            t_738 = True
+          except Exception15:
+            t_738 = False
+          if t_738:
             try:
-              t_733 = cast_by_type11(codePart__272, SpecialSet)
-            except Exception12:
-              s__1256_1257.break_()
-            this__41.pushRegex__232(t_733)
+              t_739 = cast_by_type14(codePart__278, SpecialSet)
+            except Exception15:
+              s__1264_1265.break_()
+            this__43.pushRegex__238(t_739)
           else:
             None
       return
-    raise RuntimeError14()
-  def pushOr__274(this__42, or__275: 'Or') -> 'None':
-    t_1121: 'int5'
-    t_716: 'Regex'
-    t_721: 'Regex'
-    with Label13() as s__1258_1260:
-      if not (not or__275.items):
-        with Label13() as s__1259_1262:
-          try:
-            list_builder_add_1246(this__42.out__227, '(?:')
-            t_716 = list_get_1255(or__275.items, 0)
-          except Exception12:
-            s__1259_1262.break_()
-          this__42.pushRegex__232(t_716)
-          i__277: 'int5' = 1
+    raise RuntimeError8()
+  def pushOr__280(this__44, or__281: 'Or') -> 'None':
+    t_1128: 'int5'
+    t_722: 'RegexNode'
+    t_727: 'RegexNode'
+    with Label16() as s__1266_1268:
+      if not (not or__281.items):
+        with Label16() as s__1267_1270:
+          try:
+            list_builder_add_1254(this__44.out__233, '(?:')
+            t_722 = list_get_1263(or__281.items, 0)
+          except Exception15:
+            s__1267_1270.break_()
+          this__44.pushRegex__238(t_722)
+          i__283: 'int5' = 1
           while True:
-            t_1121 = len_1254(or__275.items)
-            if i__277 < t_1121:
+            t_1128 = len_1262(or__281.items)
+            if i__283 < t_1128:
               try:
-                list_builder_add_1246(this__42.out__227, '|')
-                t_721 = list_get_1255(or__275.items, i__277)
-              except Exception12:
+                list_builder_add_1254(this__44.out__233, '|')
+                t_727 = list_get_1263(or__281.items, i__283)
+              except Exception15:
                 break
-              this__42.pushRegex__232(t_721)
-              i__277 = i__277 + 1
+              this__44.pushRegex__238(t_727)
+              i__283 = i__283 + 1
             else:
               try:
-                list_builder_add_1246(this__42.out__227, ')')
-              except Exception12:
-                s__1259_1262.break_()
-              s__1258_1260.break_()
-        raise RuntimeError14()
-  def pushRepeat__278(this__43, repeat__279: 'Repeat') -> 'None':
-    t_1111: 'Regex'
-    t_703: 'bool2'
-    t_704: 'bool2'
-    t_705: 'bool2'
-    t_708: 'int5'
-    t_710: 'MutableSequence10[str1]'
-    with Label13() as s__1263_1264:
-      min__281: 'int5'
-      max__282: 'Union8[int5, None]'
+                list_builder_add_1254(this__44.out__233, ')')
+              except Exception15:
+                s__1267_1270.break_()
+              s__1266_1268.break_()
+        raise RuntimeError8()
+  def pushRepeat__284(this__45, repeat__285: 'Repeat') -> 'None':
+    t_1118: 'RegexNode'
+    t_709: 'bool2'
+    t_710: 'bool2'
+    t_711: 'bool2'
+    t_714: 'int5'
+    t_716: 'MutableSequence13[str1]'
+    with Label16() as s__1271_1272:
+      min__287: 'int5'
+      max__288: 'Union11[int5, None]'
       try:
-        list_builder_add_1246(this__43.out__227, '(?:')
-        t_1111 = repeat__279.item
-        this__43.pushRegex__232(t_1111)
-        list_builder_add_1246(this__43.out__227, ')')
-        min__281 = repeat__279.min
-        max__282 = repeat__279.max
-      except Exception12:
-        s__1263_1264.break_()
-      if min__281 == 0:
-        t_703 = max__282 == 1
+        list_builder_add_1254(this__45.out__233, '(?:')
+        t_1118 = repeat__285.item
+        this__45.pushRegex__238(t_1118)
+        list_builder_add_1254(this__45.out__233, ')')
+        min__287 = repeat__285.min
+        max__288 = repeat__285.max
+      except Exception15:
+        s__1271_1272.break_()
+      if min__287 == 0:
+        t_709 = max__288 == 1
       else:
-        t_703 = False
-      if t_703:
+        t_709 = False
+      if t_709:
         try:
-          list_builder_add_1246(this__43.out__227, '?')
-        except Exception12:
-          s__1263_1264.break_()
+          list_builder_add_1254(this__45.out__233, '?')
+        except Exception15:
+          s__1271_1272.break_()
       else:
-        if min__281 == 0:
-          t_704 = max__282 == None
+        if min__287 == 0:
+          t_710 = max__288 == None
         else:
-          t_704 = False
-        if t_704:
+          t_710 = False
+        if t_710:
           try:
-            list_builder_add_1246(this__43.out__227, '*')
-          except Exception12:
-            s__1263_1264.break_()
+            list_builder_add_1254(this__45.out__233, '*')
+          except Exception15:
+            s__1271_1272.break_()
         else:
-          if min__281 == 1:
-            t_705 = max__282 == None
+          if min__287 == 1:
+            t_711 = max__288 == None
           else:
-            t_705 = False
-          if t_705:
+            t_711 = False
+          if t_711:
             try:
-              list_builder_add_1246(this__43.out__227, '+')
-            except Exception12:
-              s__1263_1264.break_()
+              list_builder_add_1254(this__45.out__233, '+')
+            except Exception15:
+              s__1271_1272.break_()
           else:
             try:
-              list_builder_add_1246(this__43.out__227, str_cat_1265('{', int_to_string_1266(min__281)))
-            except Exception12:
-              s__1263_1264.break_()
-            if min__281 != max__282:
+              list_builder_add_1254(this__45.out__233, str_cat_1273('{', int_to_string_1274(min__287)))
+            except Exception15:
+              s__1271_1272.break_()
+            if min__287 != max__288:
               try:
-                list_builder_add_1246(this__43.out__227, ',')
-              except Exception12:
-                s__1263_1264.break_()
-              if max__282 != None:
-                t_710 = this__43.out__227
+                list_builder_add_1254(this__45.out__233, ',')
+              except Exception15:
+                s__1271_1272.break_()
+              if max__288 != None:
+                t_716 = this__45.out__233
                 try:
-                  t_708 = cast_by_test16(max__282, isinstance_int15)
-                  list_builder_add_1246(t_710, int_to_string_1266(t_708))
-                except Exception12:
-                  s__1263_1264.break_()
+                  t_714 = cast_by_test18(max__288, isinstance_int17)
+                  list_builder_add_1254(t_716, int_to_string_1274(t_714))
+                except Exception15:
+                  s__1271_1272.break_()
               else:
                 None
             else:
               None
             try:
-              list_builder_add_1246(this__43.out__227, '}')
-            except Exception12:
-              s__1263_1264.break_()
-      if repeat__279.reluctant:
+              list_builder_add_1254(this__45.out__233, '}')
+            except Exception15:
+              s__1271_1272.break_()
+      if repeat__285.reluctant:
         try:
-          list_builder_add_1246(this__43.out__227, '?')
-        except Exception12:
-          s__1263_1264.break_()
+          list_builder_add_1254(this__45.out__233, '?')
+        except Exception15:
+          s__1271_1272.break_()
       else:
         None
       return
-    raise RuntimeError14()
-  def pushSequence__283(this__44, sequence__284: 'Sequence') -> 'None':
-    t_1109: 'int5'
-    t_697: 'Regex'
-    i__286: 'int5' = 0
-    with Label13() as s__1267_1268:
+    raise RuntimeError8()
+  def pushSequence__289(this__46, sequence__290: 'Sequence') -> 'None':
+    t_1116: 'int5'
+    t_703: 'RegexNode'
+    i__292: 'int5' = 0
+    with Label16() as s__1275_1276:
       while True:
-        t_1109 = len_1254(sequence__284.items)
-        if i__286 < t_1109:
+        t_1116 = len_1262(sequence__290.items)
+        if i__292 < t_1116:
           try:
-            t_697 = list_get_1255(sequence__284.items, i__286)
-          except Exception12:
+            t_703 = list_get_1263(sequence__290.items, i__292)
+          except Exception15:
             break
-          this__44.pushRegex__232(t_697)
-          i__286 = i__286 + 1
+          this__46.pushRegex__238(t_703)
+          i__292 = i__292 + 1
         else:
-          s__1267_1268.break_()
-      raise RuntimeError14()
-  def max_code(this__45, codePart__288: 'CodePart') -> 'Union8[int5, None]':
-    return__116: 'Union8[int5, None]'
-    t_1087: 'Any9'
-    t_1089: 'Any9'
-    t_1094: 'Union8[int5, None]'
-    t_1097: 'Union8[int5, None]'
-    t_1100: 'Union8[int5, None]'
-    t_1103: 'Union8[int5, None]'
-    t_670: 'bool2'
-    t_671: 'CodePoints'
-    t_683: 'bool2'
-    t_684: 'CodeRange'
+          s__1275_1276.break_()
+      raise RuntimeError8()
+  def max_code(this__47, codePart__294: 'CodePart') -> 'Union11[int5, None]':
+    return__120: 'Union11[int5, None]'
+    t_1094: 'Any12'
+    t_1096: 'Any12'
+    t_1101: 'Union11[int5, None]'
+    t_1104: 'Union11[int5, None]'
+    t_1107: 'Union11[int5, None]'
+    t_1110: 'Union11[int5, None]'
+    t_676: 'bool2'
+    t_677: 'CodePoints'
+    t_689: 'bool2'
+    t_690: 'CodeRange'
     try:
-      cast_by_type11(codePart__288, CodePoints)
-      t_670 = True
-    except Exception12:
-      t_670 = False
-    with Label13() as s__1269_1270:
-      if t_670:
+      cast_by_type14(codePart__294, CodePoints)
+      t_676 = True
+    except Exception15:
+      t_676 = False
+    with Label16() as s__1277_1278:
+      if t_676:
         try:
-          t_671 = cast_by_type11(codePart__288, CodePoints)
-        except Exception12:
-          s__1269_1270.break_()
-        value__290: 'str1' = t_671.value
-        if not value__290:
-          return__116 = None
+          t_677 = cast_by_type14(codePart__294, CodePoints)
+        except Exception15:
+          s__1277_1278.break_()
+        value__296: 'str1' = t_677.value
+        if not value__296:
+          return__120 = None
         else:
-          max__291: 'int5' = 0
-          t_1087 = string_code_points_1249(value__290)
-          slice__292: 'Any9' = t_1087
+          max__297: 'int5' = 0
+          t_1094 = string_code_points_1257(value__296)
+          slice__298: 'Any12' = t_1094
           while True:
-            if not slice__292.is_empty:
-              next__293: 'int5' = slice__292.read()
-              if next__293 > max__291:
-                max__291 = next__293
+            if not slice__298.is_empty:
+              next__299: 'int5' = slice__298.read()
+              if next__299 > max__297:
+                max__297 = next__299
               else:
                 None
-              t_1089 = slice__292.advance(1)
-              slice__292 = t_1089
+              t_1096 = slice__298.advance(1)
+              slice__298 = t_1096
             else:
               break
-          return__116 = max__291
+          return__120 = max__297
       else:
         try:
-          cast_by_type11(codePart__288, CodeRange)
-          t_683 = True
-        except Exception12:
-          t_683 = False
-        if t_683:
-          try:
-            t_684 = cast_by_type11(codePart__288, CodeRange)
-            t_1094 = t_684.max
-            return__116 = t_1094
-          except Exception12:
-            s__1269_1270.break_()
-        elif generic_eq_1245(codePart__288, digit):
-          t_1097 = string_code_points_1249('9').read()
-          try:
-            return__116 = t_1097
-          except Exception12:
-            s__1269_1270.break_()
-        elif generic_eq_1245(codePart__288, space):
-          t_1100 = string_code_points_1249(' ').read()
-          try:
-            return__116 = t_1100
-          except Exception12:
-            s__1269_1270.break_()
-        elif generic_eq_1245(codePart__288, word):
-          t_1103 = string_code_points_1249('z').read()
-          try:
-            return__116 = t_1103
-          except Exception12:
-            s__1269_1270.break_()
+          cast_by_type14(codePart__294, CodeRange)
+          t_689 = True
+        except Exception15:
+          t_689 = False
+        if t_689:
+          try:
+            t_690 = cast_by_type14(codePart__294, CodeRange)
+            t_1101 = t_690.max
+            return__120 = t_1101
+          except Exception15:
+            s__1277_1278.break_()
+        elif generic_eq_1253(codePart__294, digit):
+          t_1104 = string_code_points_1257('9').read()
+          try:
+            return__120 = t_1104
+          except Exception15:
+            s__1277_1278.break_()
+        elif generic_eq_1253(codePart__294, space):
+          t_1107 = string_code_points_1257(' ').read()
+          try:
+            return__120 = t_1107
+          except Exception15:
+            s__1277_1278.break_()
+        elif generic_eq_1253(codePart__294, word):
+          t_1110 = string_code_points_1257('z').read()
+          try:
+            return__120 = t_1110
+          except Exception15:
+            s__1277_1278.break_()
         else:
-          return__116 = None
-      return return__116
-    raise RuntimeError14()
-  def constructor__294(this__98, out: Optional7['MutableSequence10[str1]'] = None) -> 'None':
-    out__295: Optional7['MutableSequence10[str1]'] = out
-    t_1083: 'MutableSequence10[str1]'
-    if out__295 is None:
-      t_1083 = list_1271()
-      out__295 = t_1083
-    this__98.out__227 = out__295
-  def __init__(this__98, out: Optional7['MutableSequence10[str1]'] = None) -> None:
-    out__295: Optional7['MutableSequence10[str1]'] = out
-    this__98.constructor__294(out__295)
-regexRefs__117: 'RegexRefs__19' = RegexRefs__19()
+          return__120 = None
+      return return__120
+    raise RuntimeError8()
+  def constructor__300(this__102, out: Optional10['MutableSequence13[str1]'] = None) -> 'None':
+    out__301: Optional10['MutableSequence13[str1]'] = out
+    t_1090: 'MutableSequence13[str1]'
+    if out__301 is None:
+      t_1090 = list_1279()
+      out__301 = t_1090
+    this__102.out__233 = out__301
+  def __init__(this__102, out: Optional10['MutableSequence13[str1]'] = None) -> None:
+    out__301: Optional10['MutableSequence13[str1]'] = out
+    this__102.constructor__300(out__301)
+regexRefs__121: 'RegexRefs__21' = RegexRefs__21()
 class Begin__12(Special):
   __slots__ = ()
-  def constructor__138(this__54) -> 'None':
+  def constructor__142(this__56) -> 'None':
     None
-  def __init__(this__54) -> None:
-    this__54.constructor__138()
+  def __init__(this__56) -> None:
+    this__56.constructor__142()
 begin: 'Special' = Begin__12()
 class Dot__13(Special):
   __slots__ = ()
-  def constructor__139(this__56) -> 'None':
+  def constructor__143(this__58) -> 'None':
     None
-  def __init__(this__56) -> None:
-    this__56.constructor__139()
+  def __init__(this__58) -> None:
+    this__58.constructor__143()
 dot: 'Special' = Dot__13()
 class End__14(Special):
   __slots__ = ()
-  def constructor__140(this__58) -> 'None':
+  def constructor__144(this__60) -> 'None':
     None
-  def __init__(this__58) -> None:
-    this__58.constructor__140()
+  def __init__(this__60) -> None:
+    this__60.constructor__144()
 end: 'Special' = End__14()
 class WordBoundary__15(Special):
   __slots__ = ()
-  def constructor__141(this__60) -> 'None':
+  def constructor__145(this__62) -> 'None':
     None
-  def __init__(this__60) -> None:
-    this__60.constructor__141()
+  def __init__(this__62) -> None:
+    this__62.constructor__145()
 word_boundary: 'Special' = WordBoundary__15()
 class Digit__16(SpecialSet):
   __slots__ = ()
-  def constructor__142(this__62) -> 'None':
+  def constructor__146(this__64) -> 'None':
     None
-  def __init__(this__62) -> None:
-    this__62.constructor__142()
+  def __init__(this__64) -> None:
+    this__64.constructor__146()
 digit: 'SpecialSet' = Digit__16()
 class Space__17(SpecialSet):
   __slots__ = ()
-  def constructor__143(this__64) -> 'None':
+  def constructor__147(this__66) -> 'None':
     None
-  def __init__(this__64) -> None:
-    this__64.constructor__143()
+  def __init__(this__66) -> None:
+    this__66.constructor__147()
 space: 'SpecialSet' = Space__17()
 class Word__18(SpecialSet):
   __slots__ = ()
-  def constructor__144(this__66) -> 'None':
+  def constructor__148(this__68) -> 'None':
     None
-  def __init__(this__66) -> None:
-    this__66.constructor__144()
+  def __init__(this__68) -> None:
+    this__68.constructor__148()
 word: 'SpecialSet' = Word__18()
-def entire(item__167: 'Regex') -> 'Regex':
+def entire(item__173: 'RegexNode') -> 'RegexNode':
   global begin, end
-  return Sequence((begin, item__167, end))
-def one_or_more(item__169: 'Regex', reluctant: Optional7['bool2'] = None) -> 'Repeat':
-  reluctant__170: Optional7['bool2'] = reluctant
-  if reluctant__170 is None:
-    reluctant__170 = False
-  return Repeat(item__169, 1, None, reluctant__170)
-def optional(item__172: 'Regex', reluctant: Optional7['bool2'] = None) -> 'Repeat':
-  reluctant__173: Optional7['bool2'] = reluctant
-  if reluctant__173 is None:
-    reluctant__173 = False
-  return Repeat(item__172, 0, 1, reluctant__173)
+  return Sequence((begin, item__173, end))
+def one_or_more(item__175: 'RegexNode', reluctant: Optional10['bool2'] = None) -> 'Repeat':
+  reluctant__176: Optional10['bool2'] = reluctant
+  if reluctant__176 is None:
+    reluctant__176 = False
+  return Repeat(item__175, 1, None, reluctant__176)
+def optional(item__178: 'RegexNode', reluctant: Optional10['bool2'] = None) -> 'Repeat':
+  reluctant__179: Optional10['bool2'] = reluctant
+  if reluctant__179 is None:
+    reluctant__179 = False
+  return Repeat(item__178, 0, 1, reluctant__179)
```

### Comparing `temper_std-0.2.1/temper_std/regex.py.map` & `temper_std-0.3.0/temper_std/regex.py.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7799525504151839%*

 * *Differences: {"'mappings'": "'A,gB,O,I;A,qB,G,I,I,E,I,I,K,E,G,I,I,E,Y,I,a,E,S,I,W,E,G,I,Q,E,I,I;A,kB,gB,I;A,mB,Q,I,S,E,O,I,Q,E,O,I,Q,E,Q,I,S,E,Q,I,U,E,K,I,O,E,G,I,K,E,e,I;A,wB,Y,I,c,E,K,I,O,E,c,I,gB,E,Y,I,c,E,S,I,c,E,U,I,e,E,gB,I,qB,E,kB,I,uB,E,Q,I,a,E,O,I,Y,E,a,I;A,8B,uB,I,4B,E,oB,I,yB,E,mB,I,wB,E,sB,I,2B,E,iC,I,sC,E,4B,I;AA2B4B,MAAAiD,SAAA,UAwCzB,EAAA,AAxCyB,CAAAjD,QAwCzB,EAAA;AA9BM,cAAqC,CAAA,AAA3BkD,OAA2B,IAAA,AAAzB,QAAK;AAAG,UAAI,CAAAC,KAAK,CAACD,OAAI;AAQlC,WAAuD,CAAA,AAAjDA,OAAA,EAAAE,SAAI,CAAE,OAA2C,IAAA,AAAlC,QA […]*

```diff
@@ -1,202 +1,206 @@
 {
     "file": "py/std/temper_std/regex.py",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "ABCMeta",
         "str",
         "bool",
         "int",
-        "Exception",
         "RuntimeError",
+        "Exception",
         "len",
-        "len#1254",
+        "len#1262",
         "list",
-        "list#1271",
+        "list#1279",
         "MappingProxyType",
         "Callable",
+        "TypeVar",
+        "Generic",
         "Sequence",
         "Optional",
         "Union",
         "Any",
         "MutableSequence",
         "cast_by_type",
         "Label",
         "isinstance_int",
         "cast_by_test",
         "list_join",
-        "list_join#1242",
+        "list_join#1250",
         "generic_eq",
-        "generic_eq#1245",
+        "generic_eq#1253",
         "list_builder_add",
-        "list_builder_add#1246",
+        "list_builder_add#1254",
         "string_code_points",
-        "string_code_points#1249",
+        "string_code_points#1257",
         "list_get",
-        "list_get#1255",
+        "list_get#1263",
         "str_cat",
-        "str_cat#1265",
+        "str_cat#1273",
         "int_to_string",
-        "int_to_string#1266",
-        "compiled_regex_compile_formatted",
-        "compiled_regex_compile_formatted#1238",
-        "compiled_regex_compiled_found",
-        "compiled_regex_compiled_found#1239",
-        "compiled_regex_compiled_find",
-        "compiled_regex_compiled_find#1240",
-        "compiled_regex_compiled_replace",
-        "compiled_regex_compiled_replace#1241",
+        "int_to_string#1274",
+        "regex_compile_formatted",
+        "regex_compile_formatted#1246",
+        "regex_compiled_found",
+        "regex_compiled_found#1247",
+        "regex_compiled_find",
+        "regex_compiled_find#1248",
+        "regex_compiled_replace",
+        "regex_compiled_replace#1249",
         "regex_formatter_push_capture_name",
-        "regex_formatter_push_capture_name#1247",
+        "regex_formatter_push_capture_name#1255",
         "regex_formatter_push_code_to",
-        "regex_formatter_push_code_to#1248",
-        "Regex",
+        "regex_formatter_push_code_to#1256",
+        "RegexNode",
         "this",
-        "CompiledRegex",
+        "Regex",
         "text",
         "format",
         "Capture",
         "name",
         "item",
         "constructor",
         "CodePart",
         "CodePoints",
         "value",
         "Special",
         "SpecialSet",
         "CodeRange",
         "min",
         "max",
+        "ITEM",
+        "ItemizedRegex",
         "CodeSet",
         "items",
         "negated",
         "Or",
         "Repeat",
         "reluctant",
         "Group",
         "codePointsBegin",
         "RegexRefs",
         "codePoints",
         "group",
         "orObject",
-        "t#1206",
-        "t#1208",
-        "t#1210",
+        "t#1213",
+        "t#1215",
+        "t#1217",
         "data",
         "compiled",
-        "t#1080",
-        "t#1081",
+        "t#1087",
+        "t#1088",
         "regexRefs",
         "RegexFormatter",
         "out",
         "regex",
-        "t#1175",
+        "t#1182",
         "fn",
         "x",
         "pushRegex",
-        "t#764",
-        "t#765",
-        "t#768",
-        "t#769",
-        "t#772",
-        "t#773",
-        "t#776",
-        "t#777",
-        "t#780",
-        "t#781",
-        "t#784",
-        "t#785",
-        "t#788",
-        "t#789",
-        "s__1243#1244",
+        "t#770",
+        "t#771",
+        "t#774",
+        "t#775",
+        "t#778",
+        "t#779",
+        "t#782",
+        "t#783",
+        "t#786",
+        "t#787",
+        "t#790",
+        "t#791",
+        "t#794",
+        "t#795",
+        "s__1251#1252",
         "Begin",
         "Dot",
         "End",
         "WordBoundary",
         "Digit",
         "Space",
         "Word",
         "pushCapture",
         "capture",
-        "t#759",
-        "t#1159",
-        "t#1160",
+        "t#765",
+        "t#1166",
+        "t#1167",
         "pushCode",
         "code",
         "insideCodeSet",
         "pushCodePoints",
-        "t#1148",
-        "t#1149",
-        "t#1153",
+        "t#1155",
+        "t#1156",
+        "t#1160",
         "slice",
         "pushCodeRange",
         "codeRange",
         "pushCodeRangeUnwrapped",
-        "t#1141",
-        "t#1143",
+        "t#1148",
+        "t#1150",
         "pushCodeSet",
         "codeSet",
-        "t#1137",
-        "t#737",
-        "t#738",
+        "t#1144",
         "t#743",
+        "t#744",
+        "t#749",
         "adjusted",
-        "s__1250#1252",
-        "s__1251#1253",
+        "s__1258#1260",
+        "s__1259#1261",
         "i",
         "adjustCodeSet",
         "pushCodeSetItem",
         "codePart",
-        "t#724",
-        "t#725",
-        "t#728",
-        "t#729",
-        "t#732",
-        "t#733",
-        "s__1256#1257",
+        "t#730",
+        "t#731",
+        "t#734",
+        "t#735",
+        "t#738",
+        "t#739",
+        "s__1264#1265",
         "pushOr",
         "or",
-        "t#1121",
-        "t#716",
-        "t#721",
-        "s__1258#1260",
-        "s__1259#1262",
+        "t#1128",
+        "t#722",
+        "t#727",
+        "s__1266#1268",
+        "s__1267#1270",
         "pushRepeat",
         "repeat",
-        "t#1111",
-        "t#703",
-        "t#704",
-        "t#705",
-        "t#708",
+        "t#1118",
+        "t#709",
         "t#710",
-        "s__1263#1264",
+        "t#711",
+        "t#714",
+        "t#716",
+        "s__1271#1272",
         "pushSequence",
         "sequence",
-        "t#1109",
-        "t#697",
-        "s__1267#1268",
+        "t#1116",
+        "t#703",
+        "s__1275#1276",
         "return",
-        "t#1087",
-        "t#1089",
         "t#1094",
-        "t#1097",
-        "t#1100",
-        "t#1103",
-        "t#670",
-        "t#671",
-        "t#683",
-        "t#684",
-        "s__1269#1270",
+        "t#1096",
+        "t#1101",
+        "t#1104",
+        "t#1107",
+        "t#1110",
+        "t#676",
+        "t#677",
+        "t#689",
+        "t#690",
+        "s__1277#1278",
         "next",
-        "t#1083",
+        "t#1090",
         "entire",
         "oneOrMore",
         "optional"
     ],
     "sources": [
         "std/regex.temper.md"
     ],
     "sourcesContent": [
-        "# Regex Data Model and Functionality\n\nThe structural data model for regex patterns enables direct construction, and\nthe Temper regex dialect compiles static regex text patterns to these objects.\n\nA focus here is on providing tools people can actually reach for when they need\nto do text processing. The execution should be faster on backends like Python\nthan writing raw code, and the implementation in backends like C should\napproximate what you'd like to have written manually.\n\nDue to inadequate and distinct Unicode handling in backend regex engines, the\ninitial feature set avoids character classes and properties but is still aware\nof code points. Parsing focused on limited sets of delimiters works best for\nnow.\n\nThe core feature set here focuses on both the data model and utility functions,\nsuch as matching regexes against strings.\n\n## Regex Data Model\n\nAll regexes are composed hierarchically of `Regex` nodes. Regexes are a\nsequence of component parts. For example, `/hi./` is a sequence of\n[CodePoint](#codepoint) `/h/` and `/i/` and dot `/./`.\n\nAnd perhaps the most fundamental `Regex` is the [Sequence](#sequence),\nbecause it enables multiple regex components to be strung together.\n\n```\nexport /*sealed*/ interface Regex {\n```\n\nBefore a regex is used, it must be compiled. Some helper functions compile on\nthe fly, although it is faster to reuse a pre-compiled regex.\n\n```\n  // TODO(tjp, regex): Make this into a macro behind the scenes.\n  // TODO(tjp, regex): `compiled<T>(): CompiledRegex<T>`\n  public compiled(): CompiledRegex { new CompiledRegex(this) }\n```\n\nThe simplest use of a regular expression is if it is found in a string.\nRepeatedly calling these methods on a single `Regex` instance is inefficient.\nBetter for reuse is to compile in advance.\n\n```\n  public found(text: String): Boolean { compiled().found(text) }\n```\n\nYou can also return match details or perform text replacement. The returned\ngroups map contains an entry for each key in the order defined in the regex\npattern. If no \"full\" group is defined, one is added automatically to capture\nthe full matched text.\n\nIn the future, we intend to support customized match types with fields to match\ncapture groups, statically checked where possible.\n\n```\n  // TODO(tjp, regex): Also macro because reification.\n\n  public find(text: String): Map<String, Group> | Bubble {\n    compiled().find(text)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiled().replace(text, format)\n  }\n```\n\nThat's it for what you can do with regex patterns in Temper today, but there's\nmuch more to say on what kinds of regexes can be built.\n\n```\n}\n```\n\n## Regex Item Types\n\nA `Regex` is composed of a potential variety of subtypes.\n\n### Groups\n\nMultiple types of groups exist:\n\n- [Capture](#capture) `/(?<name>...)/` to remember match groups for later use.\n- Non-capturing group syntax `/(?:...)/`, which is simply a [Regex](#regex)\n  instance in the data model.\n\n### Capture\n\nTODO(tjp, regex): Change to named captures only!\n\n`Capture` is a [group](#groups) that remembers the matched text for later\naccess. Temper supports only named matches, with current intended syntax\n`/(?name = ...)/`.\n\n```\nexport class Capture extends Regex {\n  public name: String;\n  public /*early*/ item: Regex;\n}\n```\n\n### CodePart\n\nA component of a [CodeSet][#codeset], aka character class, which applies to a\nsubset of regex data types.\n\nHere, \"code\" is short for \"code point\" although \"char\" might work better,\ndepending on expectations.\n\n```\nexport /*sealed*/ interface CodePart extends Regex {}\n```\n\n### CodePoints\n\nOne or more verbatim code points, where the sequence matters if within a\n[Regex](#regex) or not if within a [CodeSet](#codeset). Some escapes in\ntextual regex source, such as `/\\t/`, can be stored as raw code points.\n\nThe `String` here can enable more efficient storage than individual code\npoints, although the source text may require non-capture grouping. For example,\n`/(?:abc)?/` optionally matches the string `\"abc\"`, whereas `/abc?/` matches\n`\"ab\"` with an optional `\"c\"`.\n\n```\nexport class CodePoints extends CodePart {\n  public value: String;\n}\n```\n\n### Specials\n\nA number of special match forms exist. In the data model, these are empty\nclasses.\n\n- `.` - `Dot` In default mode, matches any Unicode code point except newline.\n- `^` - `Begin` in default mode matches zero-length at the beginning of a\n  string.\n- `$` - `End` in default mode matches zero-length at the end of a string.\n- `\\b` - `WordBoundary` matches zero-length at the boundary between word and\n  non-word code points. More sophisticated Unicode compliance is TBD.\n- `\\s` (negated as `\\S`) - `Space` matches any horizontal space code point.\n  Details are TBD.\n- `\\w` (negated as `\\W`) - `Word` matches any word code point. Details are TBD.\n  This is currently defined in terms of old ASCII definitions because those are\n  clear. Perhaps this will stay that way, and Unicode properties like `\\p{L}`\n  will be used for human language needs.\n- `\\X` - `GraphemeCluster` might not be supported, but [here is some discussion\n  of how to implement it](\n  https://github.com/rust-lang/regex/issues/54#issuecomment-661905060).\n\n<details>\n\n```\nexport /*sealed*/ interface Special extends Regex {}\nexport let Begin: Special = do { class Begin extends Special {}; new Begin() };\nexport let Dot: Special = do { class Dot extends Special {}; new Dot() };\nexport let End: Special = do { class End extends Special {}; new End() };\n// TODO(tjp, regex): We can't easily support this at present across backends.\n// export let GraphemeCluster = do {\n//   class GraphemeCluster extends Special {}; new GraphemeCluster()\n// };\nexport let WordBoundary: Special = do {\n  class WordBoundary extends Special {}; new WordBoundary()\n};\n\nexport /*sealed*/ interface SpecialSet extends CodePart & Special {}\nexport let Digit: SpecialSet = do {\n  class Digit extends SpecialSet {}; new Digit()\n};\nexport let Space: SpecialSet = do {\n  class Space extends SpecialSet {}; new Space()\n};\nexport let Word: SpecialSet = do {\n  class Word extends SpecialSet {}; new Word()\n};\n```\n\n</details>\n\n### CodeRange\n\nA code point range matches any code point in its inclusive bounds, such as\n`/[a-c]/`. In source, `-` is included in a code set either by escaping or by\nincluding it as the first or last character. A `CodeRange` is usually contained\ninside a [CodeSet](#codeset), and syntactically always is.\n\n```\nexport class CodeRange extends CodePart {\n  public min: Int;\n  public max: Int;\n}\n```\n\n### CodeSet\n\nA set of code points, any of which can match, such as `/[abc]/` matching any of\n`\"a\"`, `\"b\"`, or `\"c\"`. Alternatively, a negated set is the inverse of the code\npoints given, such as `/[^abc]/`, matching any code point that's not any of\nthese. This is also often called a character class.\n\nFurther, a subset of [specials](#specials) can also be used in code sets. A\nnegated code set of just a special set often has custom syntax. For example,\nnon-space can be said as either `/[^\\s]/` or `/\\S/`.\n\n```\nexport class CodeSet extends Regex {\n  public items: List<CodePart>;\n  public negated: Boolean = false;\n}\n```\n\n### Or\n\n`Or` matches any one of multiple options, such as `/ab|cd|e*/`.\n\n```\nexport class Or extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n### Repeat\n\n`Repeat` matches from an minimum to a maximum number of repeats of a\nsubregex. This can be represented in regex source in a number of ways:\n\n- `?` matches 0 or 1.\n- `*` matches 0 or more.\n- `+` matches 1 or more.\n- `{m}` matches exactly `m` repetitions.\n- `{m,n}` matches between `m` and `n`. Missing `n` is a max of infinity. For\n  example, `{0,1}` is equivalent to `?`, and `{1,}` is equivalent to `+`.\n\nBy default, repetitions are greedy, matching as many repetitions as possible.\nIn regex source, any of the above can have `?` appended to indicated reluctant\n(aka non-greedy), matching as few repetitions as possible.\n\n```\nexport class Repeat extends Regex {\n  public /*early*/ item: Regex;\n  public min: Int;\n  public max: Int | Null; // where null means infinite\n  public reluctant: Boolean = false;\n}\n```\n\nWe also have convenience builders.\n\n```\nexport let entire(item: Regex): Regex {\n  new Sequence([Begin, item, End])\n}\n\nexport let oneOrMore(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 1, max: null, reluctant }\n}\n\nexport let optional(item: Regex, reluctant: Boolean = false): Repeat {\n  { item, min: 0, max: 1, reluctant }\n}\n```\n\n### Sequence\n\n`Sequence` strings along multiple other regexes in order.\n\n```\nexport class Sequence extends Regex {\n  public /*early*/ items: List<Regex>;\n}\n```\n\n## Match Objects\n\nFor detailed match results, call `find` on a regex to get a `Map` object from\n`String` keys to `Group` values.\n\n```\n// TODO Go back to a `Match` object with `groups` as a member so we can also\n// TODO easily return metadata alongside groups? Or is simpler better?\n// export class Match { // interface ... <T = Map<String, Group>> {\n//   public let groups: Map<String, Group>;\n// }\n\nexport class Group {\n  public let name: String;\n  public let value: String;\n  public let codePointsBegin: Int;\n}\n```\n\n## Compiled Regex Objects\n\nThe compiled form of a regex is mostly opaque, but it can be cached for more\nefficient reuse than working from a source [Regex](#regex-data-model).\n\n<details>\n\n```\n// Provides a workaround for access to std/regex from extension methods.\nclass RegexRefs {\n  public let codePoints: CodePoints = new CodePoints(\"\");\n  public let group: Group = { name: \"\", value: \"\", codePointsBegin: 0 }\n  public let orObject: Or = new Or([]);\n}\n\nlet regexRefs = new RegexRefs();\n```\n\n</details>\n\n```\n// TODO(tjp, regex): Generate subtypes of this interface later.\nexport class CompiledRegex { // interface ... <T> {\n```\n\nThe source `Regex` data is still available on compiled objects in case it's\nneeded for composition or other purposes.\n\n```\n  public let data: Regex;\n\n  public constructor(data: Regex) {\n    this.data = data;\n    compiled = compileFormatted(format());\n  }\n```\n\nA compiled regex exposes many of the same capabilities as `Regex`, but they are\nmore efficient to use repeatedly.\n\n```\n  public found(text: String): Boolean { compiledFound(compiled, text) }\n\n  public find(text: String): Map<String, Group> | Bubble {\n    compiledFind(compiled, text, regexRefs)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiledReplace(compiled, text, format, regexRefs)\n  }\n```\n\nTODO(tjp, regex): Public method for replace with named references.\nTODO(tjp, regex): Any static checking?\n\n<details>\n\n```\n  let compiled: AnyValue;\n\n  // Extension functions on some backends need the private `compiled` value\n  // passed in directly.\n  @connected(\"CompiledRegex::compiledFound\")\n  compiledFound(compiled: AnyValue, text: String): Boolean;\n\n  @connected(\"CompiledRegex::compiledFind\")\n  compiledFind(\n    compiled: AnyValue, text: String, regexRefs: RegexRefs\n  ): Map<String, Group> | Bubble;\n\n  @connected(\"CompiledRegex::compileFormatted\")\n  compileFormatted(formatted: String): AnyValue;\n\n  @connected(\"CompiledRegex::compiledReplace\")\n  compiledReplace(\n    compiled: AnyValue,\n    text: String,\n    format: fn (Map<String, Group>): String,\n    regexRefs: RegexRefs,\n  ): String;\n\n  @connected(\"CompiledRegex::format\")\n  format(): String { new RegexFormatter().format(data) }\n```\n\n</details>\n\n```\n}\n```\n\n## Private implementation matters\n\nSome regex logic can be shared across backends. These features aren't directly\nexported to the user, however.\n\nThe intent is that these support features only get included in compiled Temper\ncode if usage depends on dynamically constructed regexes. If all regex building\nis done as stable values, we hope to generated backend compiled regexes purely\nat Temper compile time.\n\n### RegexFormatter\n\n<details>\n\n```\nclass RegexFormatter {\n  let out: ListBuilder<String> = new ListBuilder<String>();\n\n  public format(regex: Regex): String {\n    pushRegex(regex)\n    out.join(\"\") { (x);; x }\n  }\n\n  pushRegex(regex: Regex): Void {\n    match (regex) {\n      // Aggregate types.\n      is Capture -> pushCapture(regex);\n      is CodePoints -> pushCodePoints(regex, false);\n      is CodeRange -> pushCodeRange(regex);\n      is CodeSet -> pushCodeSet(regex);\n      is Or -> pushOr(regex);\n      is Repeat -> pushRepeat(regex);\n      is Sequence -> pushSequence(regex);\n      // Specials.\n      // Some of these will need to be customized on future backends.\n      Begin -> out.add(\"^\");\n      Dot -> out.add(\".\");\n      End -> out.add(\"$\");\n      WordBoundary -> out.add(\"\\\\b\");\n      // Special sets.\n      Digit -> out.add(\"\\\\d\");\n      Space -> out.add(\"\\\\s\");\n      Word -> out.add(\"\\\\w\");\n      // ...\n    }\n  }\n\n  pushCapture(capture: Capture): Void {\n    out.add(\"(\");\n    // TODO(tjp, regex): Consistent name validation rules for all backends???\n    // TODO(tjp, regex): Validate here or in `Capture` constructor???\n    // TODO(tjp, regex): Validate here or where against reused names???\n    pushCaptureName(out, capture.name);\n    pushRegex(capture.item);\n    out.add(\")\");\n  }\n\n  @connected(\"RegexFormatter::pushCaptureName\")\n  pushCaptureName(out: ListBuilder<String>, name: String): Void {\n    // All so far except Python use this form.\n    out.add(\"?<${name}>\");\n  }\n\n  pushCode(code: Int, insideCodeSet: Boolean): Void {\n    // Expose private property to extension.\n    pushCodeTo(out, code, insideCodeSet);\n    // TODO(tjp, regex): Implement more in Temper once we can.\n    // if (escapeCodes[code] && false) {\n    //   out.add(\"\\\\\");\n    //   // TODO(tjp, regex): How to convert back to strings?\n    // }\n  }\n\n  @connected(\"RegexFormatter::pushCodeTo\")\n  pushCodeTo(out: ListBuilder<String>, code: Int, insideCodeSet: Boolean): Void;\n\n  pushCodePoints(codePoints: CodePoints, insideCodeSet: Boolean): Void {\n    for (\n      var slice = codePoints.value.codePoints;\n      !slice.isEmpty;\n      slice = slice.advance(1)\n    ) {\n      pushCode(slice.read(), insideCodeSet);\n    }\n  }\n\n  pushCodeRange(codeRange: CodeRange): Void {\n    out.add(\"[\");\n    pushCodeRangeUnwrapped(codeRange);\n    out.add(\"]\");\n  }\n\n  pushCodeRangeUnwrapped(codeRange: CodeRange): Void {\n    pushCode(codeRange.min, true);\n    out.add(\"-\");\n    pushCode(codeRange.max, true);\n  }\n\n  pushCodeSet(codeSet: CodeSet): Void {\n    let adjusted = adjustCodeSet(codeSet, regexRefs);\n    match (adjusted) {\n      is CodeSet -> do {\n        out.add(\"[\");\n        if (adjusted.negated) {\n          out.add(\"^\");\n        }\n        for (var i = 0; i < adjusted.items.length; i += 1) {\n          pushCodeSetItem(adjusted.items[i]);\n        }\n        out.add(\"]\");\n      }\n      else -> pushRegex(adjusted);\n    }\n  }\n\n  @connected(\"RegexFormatter::adjustCodeSet\")\n  adjustCodeSet(codeSet: CodeSet, regexRefs: RegexRefs): Regex { codeSet }\n\n  pushCodeSetItem(codePart: CodePart): Void {\n    match (codePart) {\n      is CodePoints -> pushCodePoints(codePart, true);\n      is CodeRange -> pushCodeRangeUnwrapped(codePart);\n      is SpecialSet -> pushRegex(codePart);\n    }\n  }\n\n  pushOr(or: Or): Void {\n    if (!or.items.isEmpty) {\n      out.add(\"(?:\");\n      // TODO(tjp, regex): See #822. Until `this` works better, no this in funs.\n      // TODO(tjp, regex): So just manually loop here. Sometimes faster, anyway?\n      pushRegex(or.items[0]);\n      for (var i = 1; i < or.items.length; i += 1) {\n        out.add(\"|\");\n        pushRegex(or.items[i]);\n      }\n      out.add(\")\");\n    }\n  }\n\n  pushRepeat(repeat: Repeat): Void {\n    // Always wrap the main sub-pattern here to make life easy\n    out.add(\"(?:\");\n    pushRegex(repeat.item);\n    out.add(\")\");\n    // Then add the repetition part.\n    let min = repeat.min;\n    let max = repeat.max;\n    if (false) {\n    } else if (min == 0 && max == 1) {\n      out.add(\"?\");\n    } else if (min == 0 && max == null) {\n      out.add(\"*\");\n    } else if (min == 1 && max == null) {\n      out.add(\"+\");\n    } else {\n      out.add(\"{${min.toString()}\");\n      if (min != max) {\n        out.add(\",\");\n        if (max != null) {\n          out.add(max.as<Int>().toString());\n        }\n      }\n      out.add(\"}\");\n    }\n    if (repeat.reluctant) {\n      out.add(\"?\");\n    }\n  }\n\n  pushSequence(sequence: Sequence): Void {\n    // TODO(tjp, regex): Foreach loop/function would be nice.\n    for (var i = 0; i < sequence.items.length; i += 1) {\n      pushRegex(sequence.items[i]);\n    }\n  }\n\n  // Put this here instead of the data model for now because I'm not sure this\n  // makes sense to be part of the public api right now.\n  public maxCode(codePart: CodePart): Int | Null {\n    match (codePart) {\n      is CodePoints -> do {\n        // Iterating code points is the hardest of the current cases.\n        let value = codePart.value;\n        if (value.isEmpty) {\n          null\n        } else {\n          // My kingdom for a fold, or even just a max, in builtins.\n          var max = 0;\n          for (\n            var slice = value.codePoints;\n            !slice.isEmpty;\n            slice = slice.advance(1)\n          ) {\n            let next = slice.read();\n            if (next > max) {\n              max = next;\n            }\n          }\n          max\n        }\n      }\n      // Others below are easy for now.\n      is CodeRange -> codePart.max;\n      Digit -> \"9\".codePoints.read();\n      Space -> \" \".codePoints.read();\n      Word -> \"z\".codePoints.read();\n      // Actually unexpected, ever, but eh.\n      else -> null;\n    }\n  }\n}\n```\n\n</details>\n"
+        "# Regex Data Model and Functionality\n\nThe structural data model for regex patterns enables direct construction, and\nthe Temper regex dialect compiles static regex text patterns to these objects.\n\nA focus here is on providing tools people can actually reach for when they need\nto do text processing. The execution should be faster on backends like Python\nthan writing raw code, and the implementation in backends like C should\napproximate what you'd like to have written manually.\n\nDue to inadequate and distinct Unicode handling in backend regex engines, the\ninitial feature set avoids character classes and properties but is still aware\nof code points. Parsing focused on limited sets of delimiters works best for\nnow.\n\nThe core feature set here focuses on both the data model and utility functions,\nsuch as matching regexes against strings.\n\n## Regex Data Model\n\nTemper regex representation is composed hierarchically of `RegexNode` objects.\nAnd perhaps the most fundamental `RegexNode` is the [Sequence](#sequence),\nbecause it enables multiple regex components to be strung together. For example,\n`/hi./` is a sequence of [CodePoints](#codepoints) `/hi/` and dot `/./`, but all\ncomponent types extend the `RegexNode` interface.\n\n```\nexport /*sealed*/ interface RegexNode {\n```\n\nBefore a regex is used, it must be compiled. This transforms a `RegexNode` tree\ninto a backend-native [Regex](#regex). Some helper functions compile on the fly,\nalthough it is faster to reuse a pre-compiled regex.\n\n```\n  // TODO(tjp, regex): Make this into a macro behind the scenes.\n  // TODO(tjp, regex): `compiled<T>(): Regex<T>`\n  public compiled(): Regex { new Regex(this) }\n```\n\nThe simplest use of a regular expression is if it is found in a string.\nAgain, it is better to compile to a `Regex` in advance than to repeatedly call\nconvenience methods on a `RegexNode`.\n\n```\n  public found(text: String): Boolean { compiled().found(text) }\n```\n\nYou can also return match details or perform text replacement. The returned\ngroups map contains an entry for each key in the order defined in the regex\npattern. If no \"full\" group is defined, one is added automatically to capture\nthe full matched text.\n\nIn the future, we intend to support customized match types with fields to match\ncapture groups, statically checked where possible.\n\n```\n  // TODO(tjp, regex): Also macro because reification.\n\n  public find(text: String): Map<String, Group> | Bubble {\n    compiled().find(text)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiled().replace(text, format)\n  }\n```\n\nThat's it for what you can do with regex patterns in Temper today, but there's\nmuch more to say on what kinds of regexes can be built.\n\n```\n}\n```\n\n## Regex Item Types\n\nA `Regex` is composed of a potential variety of subtypes.\n\n### Groups\n\nMultiple types of groups exist:\n\n- [Capture](#capture) `/(?<name>...)/` to remember match groups for later use.\n- Non-capturing group syntax `/(?:...)/`, which is simply a [Regex](#regex)\n  instance in the data model.\n\n### Capture\n\nTODO(tjp, regex): Change to named captures only!\n\n`Capture` is a [group](#groups) that remembers the matched text for later\naccess. Temper supports only named matches, with current intended syntax\n`/(?name = ...)/`.\n\n```\nexport class Capture extends RegexNode {\n  public name: String;\n  public /*early*/ item: RegexNode;\n}\n```\n\n### CodePart\n\nA component of a [CodeSet][#codeset], aka character class, which applies to a\nsubset of regex data types.\n\nHere, \"code\" is short for \"code point\" although \"char\" might work better,\ndepending on expectations.\n\n```\nexport /*sealed*/ interface CodePart extends RegexNode {}\n```\n\n### CodePoints\n\nOne or more verbatim code points, where the sequence matters if within a\n[Regex](#regex) or not if within a [CodeSet](#codeset). Some escapes in\ntextual regex source, such as `/\\t/`, can be stored as raw code points.\n\nThe `String` here can enable more efficient storage than individual code\npoints, although the source text may require non-capture grouping. For example,\n`/(?:abc)?/` optionally matches the string `\"abc\"`, whereas `/abc?/` matches\n`\"ab\"` with an optional `\"c\"`.\n\n```\nexport class CodePoints extends CodePart {\n  public value: String;\n}\n```\n\n### Specials\n\nA number of special match forms exist. In the data model, these are empty\nclasses.\n\n- `.` - `Dot` In default mode, matches any Unicode code point except newline.\n- `^` - `Begin` in default mode matches zero-length at the beginning of a\n  string.\n- `$` - `End` in default mode matches zero-length at the end of a string.\n- `\\b` - `WordBoundary` matches zero-length at the boundary between word and\n  non-word code points. More sophisticated Unicode compliance is TBD.\n- `\\s` (negated as `\\S`) - `Space` matches any horizontal space code point.\n  Details are TBD.\n- `\\w` (negated as `\\W`) - `Word` matches any word code point. Details are TBD.\n  This is currently defined in terms of old ASCII definitions because those are\n  clear. Perhaps this will stay that way, and Unicode properties like `\\p{L}`\n  will be used for human language needs.\n- `\\X` - `GraphemeCluster` might not be supported, but [here is some discussion\n  of how to implement it](\n  https://github.com/rust-lang/regex/issues/54#issuecomment-661905060).\n\n<details>\n\n```\nexport /*sealed*/ interface Special extends RegexNode {}\nexport let Begin: Special = do { class Begin extends Special {}; new Begin() };\nexport let Dot: Special = do { class Dot extends Special {}; new Dot() };\nexport let End: Special = do { class End extends Special {}; new End() };\n// TODO(tjp, regex): We can't easily support this at present across backends.\n// export let GraphemeCluster = do {\n//   class GraphemeCluster extends Special {}; new GraphemeCluster()\n// };\nexport let WordBoundary: Special = do {\n  class WordBoundary extends Special {}; new WordBoundary()\n};\n\nexport /*sealed*/ interface SpecialSet extends CodePart & Special {}\nexport let Digit: SpecialSet = do {\n  class Digit extends SpecialSet {}; new Digit()\n};\nexport let Space: SpecialSet = do {\n  class Space extends SpecialSet {}; new Space()\n};\nexport let Word: SpecialSet = do {\n  class Word extends SpecialSet {}; new Word()\n};\n```\n\n</details>\n\n### CodeRange\n\nA code point range matches any code point in its inclusive bounds, such as\n`/[a-c]/`. In source, `-` is included in a code set either by escaping or by\nincluding it as the first or last character. A `CodeRange` is usually contained\ninside a [CodeSet](#codeset), and syntactically always is.\n\n```\nexport class CodeRange extends CodePart {\n  public min: Int;\n  public max: Int;\n}\n```\n\n### Itemized Regex Types\n\nMake an abstraction over Regex types that have lists of subitems. This can make\nprocessing more convenient.\n\n    export interface ItemizedRegex<ITEM extends RegexNode> extends RegexNode {\n      public get items(): List<ITEM>;\n    }\n\n### CodeSet\n\nA set of code points, any of which can match, such as `/[abc]/` matching any of\n`\"a\"`, `\"b\"`, or `\"c\"`. Alternatively, a negated set is the inverse of the code\npoints given, such as `/[^abc]/`, matching any code point that's not any of\nthese. This is also often called a character class.\n\nFurther, a subset of [specials](#specials) can also be used in code sets. A\nnegated code set of just a special set often has custom syntax. For example,\nnon-space can be said as either `/[^\\s]/` or `/\\S/`.\n\n```\nexport class CodeSet extends ItemizedRegex<CodePart> {\n  public items: List<CodePart>;\n  public negated: Boolean = false;\n}\n```\n\n### Or\n\n`Or` matches any one of multiple options, such as `/ab|cd|e*/`.\n\n```\nexport class Or extends ItemizedRegex<RegexNode> {\n  public /*early*/ items: List<RegexNode>;\n}\n```\n\n### Repeat\n\n`Repeat` matches from an minimum to a maximum number of repeats of a\nsubregex. This can be represented in regex source in a number of ways:\n\n- `?` matches 0 or 1.\n- `*` matches 0 or more.\n- `+` matches 1 or more.\n- `{m}` matches exactly `m` repetitions.\n- `{m,n}` matches between `m` and `n`. Missing `n` is a max of infinity. For\n  example, `{0,1}` is equivalent to `?`, and `{1,}` is equivalent to `+`.\n\nBy default, repetitions are greedy, matching as many repetitions as possible.\nIn regex source, any of the above can have `?` appended to indicated reluctant\n(aka non-greedy), matching as few repetitions as possible.\n\n```\nexport class Repeat extends RegexNode {\n  public /*early*/ item: RegexNode;\n  public min: Int;\n  public max: Int | Null; // where null means infinite\n  public reluctant: Boolean = false;\n}\n```\n\nWe also have convenience builders.\n\n```\nexport let entire(item: RegexNode): RegexNode {\n  new Sequence([Begin, item, End])\n}\n\nexport let oneOrMore(item: RegexNode, reluctant: Boolean = false): Repeat {\n  { item, min: 1, max: null, reluctant }\n}\n\nexport let optional(item: RegexNode, reluctant: Boolean = false): Repeat {\n  { item, min: 0, max: 1, reluctant }\n}\n```\n\n### Sequence\n\n`Sequence` strings along multiple other regexes in order.\n\n```\nexport class Sequence extends ItemizedRegex<RegexNode> {\n  public /*early*/ items: List<RegexNode>;\n}\n```\n\n## Match Objects\n\nFor detailed match results, call `find` on a regex to get a `Map` object from\n`String` keys to `Group` values.\n\n```\n// TODO Go back to a `Match` object with `groups` as a member so we can also\n// TODO easily return metadata alongside groups? Or is simpler better?\n// export class Match { // interface ... <T = Map<String, Group>> {\n//   public let groups: Map<String, Group>;\n// }\n\nexport class Group {\n  public let name: String;\n  public let value: String;\n  public let codePointsBegin: Int;\n}\n```\n\n## Compiled Regex Objects\n\nThe compiled form of a regex is mostly opaque, but it can be cached for more\nefficient reuse than working from a source [RegexNode](#regex-data-model).\n\n<details>\n\n```\n// Provides a workaround for access to std/regex from extension methods.\nclass RegexRefs {\n  public let codePoints: CodePoints = new CodePoints(\"\");\n  public let group: Group = { name: \"\", value: \"\", codePointsBegin: 0 }\n  public let orObject: Or = new Or([]);\n}\n\nlet regexRefs = new RegexRefs();\n```\n\n</details>\n\n```\n// TODO(tjp, regex): Generate subtypes of this interface later.\nexport class Regex { // interface ... <T> {\n```\n\nThe source `Regex` data is still available on compiled objects in case it's\nneeded for composition or other purposes.\n\n```\n  public let data: RegexNode;\n\n  public constructor(data: RegexNode) {\n    this.data = data;\n    compiled = compileFormatted(format());\n  }\n```\n\nA compiled regex exposes many of the same capabilities as `Regex`, but they are\nmore efficient to use repeatedly.\n\n```\n  public found(text: String): Boolean { compiledFound(compiled, text) }\n\n  public find(text: String): Map<String, Group> | Bubble {\n    compiledFind(compiled, text, regexRefs)\n  }\n\n  public replace(\n    text: String, format: fn (Map<String, Group>): String\n  ): String {\n    compiledReplace(compiled, text, format, regexRefs)\n  }\n```\n\nTODO(tjp, regex): Public method for replace with named references.\nTODO(tjp, regex): Any static checking?\n\n<details>\n\n```\n  let compiled: AnyValue;\n\n  // Extension functions on some backends need the private `compiled` value\n  // passed in directly.\n  @connected(\"Regex::compiledFound\")\n  compiledFound(compiled: AnyValue, text: String): Boolean;\n\n  @connected(\"Regex::compiledFind\")\n  compiledFind(\n    compiled: AnyValue, text: String, regexRefs: RegexRefs\n  ): Map<String, Group> | Bubble;\n\n  @connected(\"Regex::compileFormatted\")\n  compileFormatted(formatted: String): AnyValue;\n\n  @connected(\"Regex::compiledReplace\")\n  compiledReplace(\n    compiled: AnyValue,\n    text: String,\n    format: fn (Map<String, Group>): String,\n    regexRefs: RegexRefs,\n  ): String;\n\n  @connected(\"Regex::format\")\n  format(): String { new RegexFormatter().format(data) }\n```\n\n</details>\n\n```\n}\n```\n\n## Private implementation matters\n\nSome regex logic can be shared across backends. These features aren't directly\nexported to the user, however.\n\nThe intent is that these support features only get included in compiled Temper\ncode if usage depends on dynamically constructed regexes. If all regex building\nis done as stable values, we hope to generated backend compiled regexes purely\nat Temper compile time.\n\n### RegexFormatter\n\n<details>\n\n```\nclass RegexFormatter {\n  let out: ListBuilder<String> = new ListBuilder<String>();\n\n  public format(regex: RegexNode): String {\n    pushRegex(regex)\n    out.join(\"\") { (x);; x }\n  }\n\n  pushRegex(regex: RegexNode): Void {\n    match (regex) {\n      // Aggregate types.\n      is Capture -> pushCapture(regex);\n      is CodePoints -> pushCodePoints(regex, false);\n      is CodeRange -> pushCodeRange(regex);\n      is CodeSet -> pushCodeSet(regex);\n      is Or -> pushOr(regex);\n      is Repeat -> pushRepeat(regex);\n      is Sequence -> pushSequence(regex);\n      // Specials.\n      // Some of these will need to be customized on future backends.\n      Begin -> out.add(\"^\");\n      Dot -> out.add(\".\");\n      End -> out.add(\"$\");\n      WordBoundary -> out.add(\"\\\\b\");\n      // Special sets.\n      Digit -> out.add(\"\\\\d\");\n      Space -> out.add(\"\\\\s\");\n      Word -> out.add(\"\\\\w\");\n      // ...\n    }\n  }\n\n  pushCapture(capture: Capture): Void {\n    out.add(\"(\");\n    // TODO(tjp, regex): Consistent name validation rules for all backends???\n    // TODO(tjp, regex): Validate here or in `Capture` constructor???\n    // TODO(tjp, regex): Validate here or where against reused names???\n    pushCaptureName(out, capture.name);\n    pushRegex(capture.item);\n    out.add(\")\");\n  }\n\n  @connected(\"RegexFormatter::pushCaptureName\")\n  pushCaptureName(out: ListBuilder<String>, name: String): Void {\n    // All so far except Python use this form.\n    out.add(\"?<${name}>\");\n  }\n\n  pushCode(code: Int, insideCodeSet: Boolean): Void {\n    // Expose private property to extension.\n    pushCodeTo(out, code, insideCodeSet);\n    // TODO(tjp, regex): Implement more in Temper once we can.\n    // if (escapeCodes[code] && false) {\n    //   out.add(\"\\\\\");\n    //   // TODO(tjp, regex): How to convert back to strings?\n    // }\n  }\n\n  @connected(\"RegexFormatter::pushCodeTo\")\n  pushCodeTo(out: ListBuilder<String>, code: Int, insideCodeSet: Boolean): Void;\n\n  pushCodePoints(codePoints: CodePoints, insideCodeSet: Boolean): Void {\n    for (\n      var slice = codePoints.value.codePoints;\n      !slice.isEmpty;\n      slice = slice.advance(1)\n    ) {\n      pushCode(slice.read(), insideCodeSet);\n    }\n  }\n\n  pushCodeRange(codeRange: CodeRange): Void {\n    out.add(\"[\");\n    pushCodeRangeUnwrapped(codeRange);\n    out.add(\"]\");\n  }\n\n  pushCodeRangeUnwrapped(codeRange: CodeRange): Void {\n    pushCode(codeRange.min, true);\n    out.add(\"-\");\n    pushCode(codeRange.max, true);\n  }\n\n  pushCodeSet(codeSet: CodeSet): Void {\n    let adjusted = adjustCodeSet(codeSet, regexRefs);\n    match (adjusted) {\n      is CodeSet -> do {\n        out.add(\"[\");\n        if (adjusted.negated) {\n          out.add(\"^\");\n        }\n        for (var i = 0; i < adjusted.items.length; i += 1) {\n          pushCodeSetItem(adjusted.items[i]);\n        }\n        out.add(\"]\");\n      }\n      else -> pushRegex(adjusted);\n    }\n  }\n\n  @connected(\"RegexFormatter::adjustCodeSet\")\n  adjustCodeSet(codeSet: CodeSet, regexRefs: RegexRefs): RegexNode { codeSet }\n\n  pushCodeSetItem(codePart: CodePart): Void {\n    match (codePart) {\n      is CodePoints -> pushCodePoints(codePart, true);\n      is CodeRange -> pushCodeRangeUnwrapped(codePart);\n      is SpecialSet -> pushRegex(codePart);\n    }\n  }\n\n  pushOr(or: Or): Void {\n    if (!or.items.isEmpty) {\n      out.add(\"(?:\");\n      // TODO(tjp, regex): See #822. Until `this` works better, no this in funs.\n      // TODO(tjp, regex): So just manually loop here. Sometimes faster, anyway?\n      pushRegex(or.items[0]);\n      for (var i = 1; i < or.items.length; i += 1) {\n        out.add(\"|\");\n        pushRegex(or.items[i]);\n      }\n      out.add(\")\");\n    }\n  }\n\n  pushRepeat(repeat: Repeat): Void {\n    // Always wrap the main sub-pattern here to make life easy\n    out.add(\"(?:\");\n    pushRegex(repeat.item);\n    out.add(\")\");\n    // Then add the repetition part.\n    let min = repeat.min;\n    let max = repeat.max;\n    if (false) {\n    } else if (min == 0 && max == 1) {\n      out.add(\"?\");\n    } else if (min == 0 && max == null) {\n      out.add(\"*\");\n    } else if (min == 1 && max == null) {\n      out.add(\"+\");\n    } else {\n      out.add(\"{${min.toString()}\");\n      if (min != max) {\n        out.add(\",\");\n        if (max != null) {\n          out.add(max.as<Int>().toString());\n        }\n      }\n      out.add(\"}\");\n    }\n    if (repeat.reluctant) {\n      out.add(\"?\");\n    }\n  }\n\n  pushSequence(sequence: Sequence): Void {\n    // TODO(tjp, regex): Foreach loop/function would be nice.\n    for (var i = 0; i < sequence.items.length; i += 1) {\n      pushRegex(sequence.items[i]);\n    }\n  }\n\n  // Put this here instead of the data model for now because I'm not sure this\n  // makes sense to be part of the public api right now.\n  public maxCode(codePart: CodePart): Int | Null {\n    match (codePart) {\n      is CodePoints -> do {\n        // Iterating code points is the hardest of the current cases.\n        let value = codePart.value;\n        if (value.isEmpty) {\n          null\n        } else {\n          // My kingdom for a fold, or even just a max, in builtins.\n          var max = 0;\n          for (\n            var slice = value.codePoints;\n            !slice.isEmpty;\n            slice = slice.advance(1)\n          ) {\n            let next = slice.read();\n            if (next > max) {\n              max = next;\n            }\n          }\n          max\n        }\n      }\n      // Others below are easy for now.\n      is CodeRange -> codePart.max;\n      Digit -> \"9\".codePoints.read();\n      Space -> \" \".codePoints.read();\n      Word -> \"z\".codePoints.read();\n      // Actually unexpected, ever, but eh.\n      else -> null;\n    }\n  }\n}\n```\n\n</details>\n"
     ],
     "version": 3
 }
```

### Comparing `temper_std-0.2.1/temper_std/temporal.py` & `temper_std-0.3.0/temper_std/temporal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,42 @@
-from typing import Sequence as Sequence6, Any as Any9
+from typing import Sequence as Sequence9, Any as Any12
 from builtins import int as int5, bool as bool2, str as str1
-from temper_core import int_to_string as int_to_string_1266, string_code_points as string_code_points_1249, str_cat as str_cat_1265
+from temper_core import int_to_string as int_to_string_1274, string_code_points as string_code_points_1257, str_cat as str_cat_1273
 # Type nym`std//temporal.temper.md`.Date connected to datetime.date
-daysInMonth__21: 'Sequence6[int5]' = (0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31)
-def isLeapYear__19(year__22: 'int5') -> 'bool2':
-  return__13: 'bool2'
-  t_132: 'int5'
-  if year__22 % 4 == 0:
-    if year__22 % 100 != 0:
-      return__13 = True
+daysInMonth__26: 'Sequence9[int5]' = (0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31)
+def isLeapYear__24(year__29: 'int5') -> 'bool2':
+  return__16: 'bool2'
+  t_168: 'int5'
+  if year__29 % 4 == 0:
+    if year__29 % 100 != 0:
+      return__16 = True
     else:
-      t_132 = year__22 % 400
-      return__13 = t_132 == 0
+      t_168 = year__29 % 400
+      return__16 = t_168 == 0
   else:
-    return__13 = False
-  return return__13
-def pad__20(padding__24: 'str1', num__25: 'int5') -> 'str1':
+    return__16 = False
+  return return__16
+def pad__25(padding__31: 'str1', num__32: 'int5') -> 'str1':
   'If the decimal representation of \\|num\\| is longer than [padding],\nthen that representation.\nOtherwise any sign for [num] followed by the prefix of [padding]\nthat would bring the integer portion up to the length of [padding].\n\n```temper\npad("0000", 123) == "0123") &&\npad("000", 123) == "123") &&\npad("00", 123) == "123") &&\npad("0000", -123) == "-0123") &&\npad("000", -123) == "-123") &&\npad("00", -123) == "-123")\n```'
-  return__14: 'str1'
-  t_185: 'Any9'
-  decimal__27: 'str1' = int_to_string_1266(num__25, 10)
-  t_181: 'Any9' = string_code_points_1249(decimal__27)
-  decimalCodePoints__28: 'Any9' = t_181
-  sign__29: 'str1'
-  if decimalCodePoints__28.read() == 45:
-    sign__29 = '-'
-    t_185 = decimalCodePoints__28.advance(1)
-    decimalCodePoints__28 = t_185
+  return__17: 'str1'
+  t_228: 'Any12'
+  decimal__34: 'str1' = int_to_string_1274(num__32, 10)
+  t_224: 'Any12' = string_code_points_1257(decimal__34)
+  decimalCodePoints__35: 'Any12' = t_224
+  sign__36: 'str1'
+  if decimalCodePoints__35.read() == 45:
+    sign__36 = '-'
+    t_228 = decimalCodePoints__35.advance(1)
+    decimalCodePoints__35 = t_228
   else:
-    sign__29 = ''
-  paddingCp__30: 'Any9' = string_code_points_1249(padding__24)
-  nNeeded__31: 'int5' = paddingCp__30.length - decimalCodePoints__28.length
-  if nNeeded__31 <= 0:
-    return__14 = decimal__27
+    sign__36 = ''
+  paddingCp__37: 'Any12' = string_code_points_1257(padding__31)
+  nNeeded__38: 'int5' = paddingCp__37.length - decimalCodePoints__35.length
+  if nNeeded__38 <= 0:
+    return__17 = decimal__34
   else:
-    pad__32: 'str1' = paddingCp__30.limit(nNeeded__31).to_string()
-    decimalOnly__33: 'str1' = decimalCodePoints__28.to_string()
-    return__14 = str_cat_1265(sign__29, pad__32, decimalOnly__33)
-  return return__14
+    pad__39: 'str1' = paddingCp__37.limit(nNeeded__38).to_string()
+    decimalOnly__40: 'str1' = decimalCodePoints__35.to_string()
+    return__17 = str_cat_1273(sign__36, pad__39, decimalOnly__40)
+  return return__17
+dayOfWeekLookupTableLeapy__27: 'Sequence9[int5]' = (0, 0, 3, 4, 0, 2, 5, 0, 3, 6, 1, 4, 6)
+dayOfWeekLookupTableNotLeapy__28: 'Sequence9[int5]' = (0, 0, 3, 3, 6, 1, 4, 6, 2, 5, 0, 3, 5)
```

### Comparing `temper_std-0.2.1/temper_std/temporal.py.map` & `temper_std-0.3.0/temper_std/temporal.py.map`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7999999999999999%*

 * *Differences: {"'mappings'": "'A,mB,Q,I,S,E,G,I;A,qB,G,I,I,E,I,I,K,E,G,I;A,wB,a,I,kB,E,kB,I,uB,E,O,I;AAmFiB,mEA6GV;AAvLCW,eAAW,CAAA,AAAX,kBAAW,EAAG,EAChB,CAAC,CACe,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE;AAGpB,GAAI,CAAAC,cAAU,CAAA,AAACC,QAAI,CAAE,OAEpB,IAAA,AAF0B,QAAO,CAAA;AAAP,EAAAC,UAAA;AACa,EAAAC,KAAU,CAAA,AAAV,OAAU;AAA/C,KAAAF,QAAI,AAAJ,EAAO,EAAC,AAAR,GAAY,EAAC;AAAK,OAAAA,QAAI,AAAJ,EAAO,IAAG,AAAV,GAAc,EAAC;AAAA,MAAAC,UAAA;AAAA;AAAI,MAAAC,KAAA, […]*

```diff
@@ -1,40 +1,42 @@
 {
     "file": "py/std/temper_std/temporal.py",
-    "mappings": "A,mB,Q,I,S,E,G,I;A,qB,G,I,I,E,I,I,K,E,G,I;A,wB,a,I,kB,E,kB,I,uB,E,O,I;AAwEiB,mEAsEoB;AArI7BW,eAAW,CAAA,AAAX,kBAAW,EAAG,EAChB,CAAC,CACe,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE,CACF,GAAE;AAGpB,GAAI,CAAAC,cAAU,CAAA,AAACC,QAAI,CAAE,OAEpB,IAAA,AAF0B,QAAO,CAAA;AAAP,EAAAC,UAAA;AACa,EAAAC,KAAU,CAAA,AAAV,OAAU;AAA/C,KAAAF,QAAI,AAAJ,EAAO,EAAC,AAAR,GAAY,EAAC;AAAK,OAAAA,QAAI,AAAJ,EAAO,IAAG,AAAV,GAAc,EAAC;AAAA,MAAAC,UAAA;AAAA;AAAI,MAAAC,KAAA,GAAAF,QAAI,AAAJ,EAAO,IAAG;AAAV,MAAAC,UAAA,GAAAC,KAAU,AAAV,GAAc,EAAC;AAAA;AAAC,IAAAD,UAAA;AACvD,QAAA,AAF0B,CAAAA;AAmB3B,GAAI,CAAAE,OAAG,CAAA,AAACC,WAAO,CAAE,OAAM,CAAE,CAAAC,OAAG,CAAE,OAmB7B,IAAA,AAnBmC,OAAM,CAAA;AAA1C;AAAoC,EAAAJ,UAAA;AAMZ,EAAAK,KAA4B,CAAA,AAA5B,OAA4B;AAL9C,EAAAC,WAAO,CAAA,AAAP,OAAO,EAAO,CAAAd,kBAAQ,CAAA,AAAZY,OAAG,CAAU,GAAE;AACL,EAAAG,KAAkB,CAAA,AAAlB,OAAkB,EAAA,AAAV,CAAAb,uBAAU,CAAA,AAAlBY,WAAO,CAAW;AAAtC,EAAAE,qBAAiB,CAAA,AAAjB,OAAiB,EAAG,CAAAD;AACpB,EAAAE,QAAI,CAAE;AACN,IAAkB,AAAlB,CAAAD,qBAAiB,CAAA,AAAjB,IAAsB,EAAE,AAAxB,GAA4B,GAAE;AAChC,IAAAC,QAAI,EAAG,IAAG;AACU,IAAAJ,KAAA,EAAkB,AAAlB,CAAAG,qBAAiB,CAAA,AAAjB,OAAyB,CAAC,CAAC,CAAC;AAAhD,IAAAA,qBAAiB,EAAG,CAAAH,KAA4B;AAA/B;AAEjB,IAAAI,QAAI,EAAG,GAAE;AAEP,EAAAC,aAAS,CAAA,AAAT,OAAS,EAAW,CAAAhB,uBAAU,CAAA,AAAlBS,WAAO;AACnB,EAAAQ,WAAO,CAAA,AAAP,OAAO,EAAG,CAAAD,aAAS,CAAO,MAAA,AAAhB,EAAmB,CAAAF,qBAAiB,CAAO;AAAA,IACrD,CAAAG,WAAO,AAAP,GAAW,EAAC;AACd,IAAAX,UAAA,GAAAM,WAAO;AAAP;AAEI,IAAAJ,OAAG,CAAA,AAAH,OAAG,EAA4B,AAAzB,CAAAQ,aAAS,CAAA,AAAT,KAAe,CAACC,WAAO,CAAC,CAAA,AAAxB,SAAiC;AACvC,IAAAC,eAAW,CAAA,AAAX,OAAW,EAAqB,AAAlB,CAAAJ,qBAAiB,CAAA,AAAjB,SAA0B;AAC5C,IAAAR,UAAA,GAAAJ,YAAA,CAAGa,QAAI,CAAG,CAAAP,OAAG,CAAG,CAAAU,eAAW,CAAE;AAEhC,QAAA,AAnBmC,CAAAZ",
+    "mappings": "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",
     "names": [
         "Sequence",
         "Any",
         "int",
         "bool",
         "str",
         "int_to_string",
-        "int_to_string#1266",
+        "int_to_string#1274",
         "string_code_points",
-        "string_code_points#1249",
+        "string_code_points#1257",
         "str_cat",
-        "str_cat#1265",
+        "str_cat#1273",
         "daysInMonth",
         "isLeapYear",
         "year",
         "return",
-        "t#132",
+        "t#168",
         "pad",
         "padding",
         "num",
-        "t#185",
+        "t#228",
         "decimal",
-        "t#181",
+        "t#224",
         "decimalCodePoints",
         "sign",
         "paddingCp",
         "nNeeded",
-        "decimalOnly"
+        "decimalOnly",
+        "dayOfWeekLookupTableLeapy",
+        "dayOfWeekLookupTableNotLeapy"
     ],
     "sources": [
         "std/temporal.temper.md"
     ],
     "sourcesContent": [
-        "# Temporal\n\nWe're creating an initial Date type to help with developing\nTemper's machinery to connect to existing Date types in\ntarget languages.\n\nSome facts about the Gregorian calendar.\n\n    /** Indexed by the month number: 1 = January */\n    let daysInMonth = [\n      0,\n      /* January   */ 31,\n      /* February  */ 28, // Special case leap days\n      /* March     */ 31,\n      /* April     */ 30,\n      /* May       */ 31,\n      /* June      */ 30,\n      /* July      */ 31,\n      /* August    */ 31,\n      /* September */ 30,\n      /* October   */ 31,\n      /* November  */ 30,\n      /* December  */ 31,\n    ];\n\n    let isLeapYear(year: Int): Boolean {\n       year % 4 == 0 && (year % 100 != 0 || year % 400 == 0)\n    }\n\n    /**\n     * If the decimal representation of \\|num\\| is longer than [padding],\n     * then that representation.\n     * Otherwise any sign for [num] followed by the prefix of [padding]\n     * that would bring the integer portion up to the length of [padding].\n     *\n     * ```temper\n     * pad(\"0000\", 123) == \"0123\") &&\n     * pad(\"000\", 123) == \"123\") &&\n     * pad(\"00\", 123) == \"123\") &&\n     * pad(\"0000\", -123) == \"-0123\") &&\n     * pad(\"000\", -123) == \"-123\") &&\n     * pad(\"00\", -123) == \"-123\")\n     * ```\n     */\n    let pad(padding: String, num: Int): String {\n      let decimal = num.toString(10);\n      var decimalCodePoints = decimal.codePoints;\n      let sign: String;\n      if (decimalCodePoints.read() == 45 /* - */) {\n        sign = \"-\";\n        decimalCodePoints = decimalCodePoints.advance(1);\n      } else {\n        sign = \"\";\n      }\n      let paddingCp = padding.codePoints;\n      let nNeeded = paddingCp.length - decimalCodePoints.length;\n      if (nNeeded <= 0) {\n        decimal\n      } else {\n        let pad = paddingCp.limit(nNeeded).toString();\n        let decimalOnly = decimalCodePoints.toString();\n        \"${sign}${pad}${decimalOnly}\"\n      }\n    }\n\nHere's just enough of a Date type to get us started.\n\n    /**\n     * A Date identifies a day in the proleptic Gregorian calendar.\n     * It is unconnected to a time of day or a timezone.\n     */\n    @connected(\"Date\")\n    export class Date {\n      /** The year.  1900 means 1900. */\n      @connected(\"Date::getYear\")\n      public year: Int;\n      /** The month of the year in [1, 12]. */\n      @connected(\"Date::getMonth\")\n      public month: Int;\n      /**\n       * The day of the month in [1, 31]\n       * additionally constrained by the length of [month].\n       */\n      @connected(\"Date::getDay\")\n      public day: Int;\n\n      @connected(\"Date::constructor\")\n      public constructor(year: Int, month: Int, day: Int): Void | Bubble {\n        if (1 <= month && month <= 12 &&\n            1 <= day && (\n              (month != 2 || day != 29)\n              ? day <= daysInMonth[month]\n              : isLeapYear(year))) {\n          this.year = year;\n          this.month = month;\n          this.day = day;\n        } else {\n          bubble();\n        }\n      }\n\n      /** An ISO 8601 Date string with dashes like \"2000-12-31\". */\n      @connected(\"Date::toString\")\n      public toString(): String {\n         \"${pad(\"0000\", year)\n        }-${pad(\"00\",   month)\n        }-${pad(\"00\",   day)}\"\n      }\n\n      /**\n       * The count of whole years between the two dates.\n       *\n       * Think of this as floor of the magnitude of a range:\n       *\n       *     \u230a [start, end] \u230b\n       *\n       * If you think of it as subtraction, you have to reverse\n       * the order of arguments.\n       *\n       *     \u230a end - start \u230b, NOT \u230a start - end \u230b\n       *\n       * \"Whole year\" is based on month/day calculations, not\n       * day-of-year.  This means that there is one full year\n       * between 2020-03-01 and 2021-03-01 even though, because\n       * February of 2020 has 29 days, 2020-03-01 is the 61st\n       * day of 2020 but 2021-03-01 is only the 60th day of\n       * that year.\n       */\n      @connected(\"Date::yearsBetween\")\n      public static let yearsBetween(start: Date, end: Date): Int {\n        let yearDelta = end.year - start.year;\n        let monthDelta = end.month - start.month;\n        yearDelta - (\n            // If the end month/day is before the start's then we\n            // don't have a full year.\n            (monthDelta < 0 || monthDelta == 0 && end.day < start.day)\n            ? 1 : 0)\n      }\n\n      /** Today's date in UTC */\n      // TODO: take a zone\n      @connected(\"Date::today\")\n      public static let today(): Date;\n    };\n\nTODO: an auto-balancing Date builder.\nParse from ISO\nOther temporal values\nDay of week\n"
+        "# Temporal\n\nWe're creating an initial Date type to help with developing\nTemper's machinery to connect to existing Date types in\ntarget languages.\n\nSome facts about the Gregorian calendar.\n\n    /** Indexed by the month number: 1 = January */\n    let daysInMonth = [\n      0,\n      /* January   */ 31,\n      /* February  */ 28, // Special case leap days\n      /* March     */ 31,\n      /* April     */ 30,\n      /* May       */ 31,\n      /* June      */ 30,\n      /* July      */ 31,\n      /* August    */ 31,\n      /* September */ 30,\n      /* October   */ 31,\n      /* November  */ 30,\n      /* December  */ 31,\n    ];\n\n    let isLeapYear(year: Int): Boolean {\n       year % 4 == 0 && (year % 100 != 0 || year % 400 == 0)\n    }\n\n    /**\n     * If the decimal representation of \\|num\\| is longer than [padding],\n     * then that representation.\n     * Otherwise any sign for [num] followed by the prefix of [padding]\n     * that would bring the integer portion up to the length of [padding].\n     *\n     * ```temper\n     * pad(\"0000\", 123) == \"0123\") &&\n     * pad(\"000\", 123) == \"123\") &&\n     * pad(\"00\", 123) == \"123\") &&\n     * pad(\"0000\", -123) == \"-0123\") &&\n     * pad(\"000\", -123) == \"-123\") &&\n     * pad(\"00\", -123) == \"-123\")\n     * ```\n     */\n    let pad(padding: String, num: Int): String {\n      let decimal = num.toString(10);\n      var decimalCodePoints = decimal.codePoints;\n      let sign: String;\n      if (decimalCodePoints.read() == 45 /* - */) {\n        sign = \"-\";\n        decimalCodePoints = decimalCodePoints.advance(1);\n      } else {\n        sign = \"\";\n      }\n      let paddingCp = padding.codePoints;\n      let nNeeded = paddingCp.length - decimalCodePoints.length;\n      if (nNeeded <= 0) {\n        decimal\n      } else {\n        let pad = paddingCp.limit(nNeeded).toString();\n        let decimalOnly = decimalCodePoints.toString();\n        \"${sign}${pad}${decimalOnly}\"\n      }\n    }\n\n    // Relates months (one-indexed) to numbers used in day-of-week\n    // computations non-leapy.\n    let dayOfWeekLookupTableLeapy: List<Int> = [\n      0, // Not a month\n      0, 3, 4, 0, 2, 5, 0, 3, 6, 1, 4, 6,\n    ];\n    let dayOfWeekLookupTableNotLeapy: List<Int> = [\n      0, // Not a month\n      0, 3, 3, 6, 1, 4, 6, 2, 5, 0, 3, 5,\n    ];\n\nHere's just enough of a Date type to get us started.\n\n    /**\n     * A Date identifies a day in the proleptic Gregorian calendar.\n     * It is unconnected to a time of day or a timezone.\n     */\n    @connected(\"Date\")\n    export class Date {\n      /** The year.  1900 means 1900. */\n      @connected(\"Date::getYear\")\n      public year: Int;\n      /** The month of the year in [1, 12]. */\n      @connected(\"Date::getMonth\")\n      public month: Int;\n      /**\n       * The day of the month in [1, 31]\n       * additionally constrained by the length of [month].\n       */\n      @connected(\"Date::getDay\")\n      public day: Int;\n\n      @connected(\"Date::constructor\")\n      public constructor(year: Int, month: Int, day: Int): Void | Bubble {\n        if (1 <= month && month <= 12 &&\n            1 <= day && (\n              (month != 2 || day != 29)\n              ? day <= daysInMonth[month]\n              : isLeapYear(year))) {\n          this.year = year;\n          this.month = month;\n          this.day = day;\n        } else {\n          bubble();\n        }\n      }\n\n      /** An ISO 8601 Date string with dashes like \"2000-12-31\". */\n      @connected(\"Date::toString\")\n      public toString(): String {\n         \"${pad(\"0000\", year)\n        }-${pad(\"00\",   month)\n        }-${pad(\"00\",   day)}\"\n      }\n\n      /**\n       * The count of whole years between the two dates.\n       *\n       * Think of this as floor of the magnitude of a range:\n       *\n       *     \u230a [start, end] \u230b\n       *\n       * If you think of it as subtraction, you have to reverse\n       * the order of arguments.\n       *\n       *     \u230a end - start \u230b, NOT \u230a start - end \u230b\n       *\n       * \"Whole year\" is based on month/day calculations, not\n       * day-of-year.  This means that there is one full year\n       * between 2020-03-01 and 2021-03-01 even though, because\n       * February of 2020 has 29 days, 2020-03-01 is the 61st\n       * day of 2020 but 2021-03-01 is only the 60th day of\n       * that year.\n       */\n      @connected(\"Date::yearsBetween\")\n      public static let yearsBetween(start: Date, end: Date): Int {\n        let yearDelta = end.year - start.year;\n        let monthDelta = end.month - start.month;\n        yearDelta - (\n            // If the end month/day is before the start's then we\n            // don't have a full year.\n            (monthDelta < 0 || monthDelta == 0 && end.day < start.day)\n            ? 1 : 0)\n      }\n\n      /** Today's date in UTC */\n      // TODO: take a zone\n      @connected(\"Date::today\")\n      public static let today(): Date;\n\n      /**\n       * ISO 8601 weekday number.\n       *\n       * | Number | Weekday  |\n       * | ------ | -------- |\n       * |      1 | Monday   |\n       * |      2 | Tuesday  |\n       * |      3 | Monday   |\n       * |      4 | Thursday |\n       * |      5 | Friday   |\n       * |      6 | Saturday |\n       * |      7 | Sunday   |\n       */\n      @connected(\"Date::getDayOfWeek\")\n      public get dayOfWeek(): Int {\n        // Gauss's method.\n        let y = year;\n        let c = if (y >= 0) { y / 100 } else { -(-y / 100) };\n        let yy = y - (c * 100);\n        // See note below about avoiding negative modulus to see why\n        // some of the offsets differ from Wikipedia's rendering of\n        // Gauss's formula.\n        let janFirst = (8 + 5*((yy + 3) % 4) + 3*(yy - 1) + 5*(c % 4)) % 7;\n        let table = if (isLeapYear(y)) {\n          dayOfWeekLookupTableLeapy\n        } else {\n          dayOfWeekLookupTableNotLeapy\n        };\n        let monthOffset = table[month];\n        // Gauss's method produces a number in 0..6 but\n        // ISO assigns 1..7 where all values are the same\n        // except that Sunday is 7 instead of 0.\n        // Below we do (day + 6) since that is equivalent to\n        // (day - 1) where we end up % 7 but avoids any chance\n        // of a negative left operand to `%`.\n        let gaussWeekday = (janFirst + (day + 6) + monthOffset) % 7;\n        gaussWeekday == 0 ? 7 : gaussWeekday\n      }\n    };\n\nTODO: an auto-balancing Date builder.\nParse from ISO\nOther temporal values\nDay of week\n"
     ],
     "version": 3
 }
```

### Comparing `temper_std-0.2.1/temper_std/testing.py` & `temper_std-0.3.0/temper_std/testing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Any as Any9, MutableSequence as MutableSequence10, Callable as Callable4, Sequence as Sequence6, Union as Union8, Optional as Optional7
-from temper_core import LoggingConsole as LoggingConsole17, Pair as Pair_1275, Label as Label13, list_builder_add as list_builder_add_1246, list_join as list_join_1242, list_map as list_map_1276, list_get as list_get_1255, str_cat as str_cat_1265
-from builtins import bool as bool2, str as str1, Exception as Exception12, int as int5, RuntimeError as RuntimeError14, tuple as tuple_1274, list as list_1271, len as len_1254
-console_88: 'Any9' = LoggingConsole17(__name__)
+from typing import Any as Any12, MutableSequence as MutableSequence13, Callable as Callable4, Sequence as Sequence9, Union as Union11, Optional as Optional10
+from temper_core import LoggingConsole as LoggingConsole19, Pair as Pair_1283, Label as Label16, list_builder_add as list_builder_add_1254, list_join as list_join_1250, list_map as list_map_1284, list_get as list_get_1263, str_cat as str_cat_1273
+from builtins import bool as bool2, str as str1, Exception as Exception15, int as int5, RuntimeError as RuntimeError8, tuple as tuple_1282, list as list_1279, len as len_1262
+console_88: 'Any12' = LoggingConsole19(__name__)
 class Test:
   passing__16: 'bool2'
   failedOnAssert__17: 'bool2'
   hasUnhandledFail__18: 'bool2'
   _failedOnAssert__58: 'bool2'
   _passing__59: 'bool2'
-  _messages__60: 'MutableSequence10[str1]'
+  _messages__60: 'MutableSequence13[str1]'
   __slots__ = ('passing__16', 'failedOnAssert__17', 'hasUnhandledFail__18', '_failedOnAssert__58', '_passing__59', '_messages__60')
   def assert_(this__7, success__36: 'bool2', message__37: 'Callable4[[], str1]') -> 'None':
     if not success__36:
       this__7._passing__59 = False
-      list_builder_add_1246(this__7._messages__60, message__37())
+      list_builder_add_1254(this__7._messages__60, message__37())
     else:
       None
   def assert_hard(this__8, success__40: 'bool2', message__41: 'Callable4[[], str1]') -> 'None':
     this__8.assert_(success__40, message__41)
     if not success__40:
       this__8._failedOnAssert__58 = True
       assert False, str1(this__8.messages_combined())
@@ -28,130 +28,130 @@
       this__9._failedOnAssert__58 = True
       assert False, str1(this__9.messages_combined())
     else:
       None
   @property
   def passing(this__11) -> 'bool2':
     return this__11._passing__59
-  def messages(this__12) -> 'Sequence6[str1]':
-    return tuple_1274(this__12._messages__60)
+  def messages(this__12) -> 'Sequence9[str1]':
+    return tuple_1282(this__12._messages__60)
   @property
   def failed_on_assert(this__13) -> 'bool2':
     return this__13._failedOnAssert__58
   @property
   def has_unhandled_fail(this__14) -> 'bool2':
     t_186: 'bool2'
     if this__14._failedOnAssert__58:
       t_186 = True
     else:
       t_186 = this__14._passing__59
     return not t_186
-  def messages_combined(this__15) -> 'Union8[str1, None]':
-    return__30: 'Union8[str1, None]'
-    t_291: 'MutableSequence10[str1]'
-    t_292: 'Union8[str1, None]'
+  def messages_combined(this__15) -> 'Union11[str1, None]':
+    return__30: 'Union11[str1, None]'
+    t_291: 'MutableSequence13[str1]'
+    t_292: 'Union11[str1, None]'
     if not this__15._messages__60:
       return__30 = None
     else:
       t_291 = this__15._messages__60
       def fn__288(it__57: 'str1') -> 'str1':
         return it__57
-      t_292 = list_join_1242(t_291, ', ', fn__288)
+      t_292 = list_join_1250(t_291, ', ', fn__288)
       return__30 = t_292
     return return__30
-  def constructor__61(this__19, failed_on_assert: Optional7['bool2'] = None, passing: Optional7['bool2'] = None, messages: Optional7['MutableSequence10[str1]'] = None) -> 'None':
-    _failedOnAssert__62: Optional7['bool2'] = failed_on_assert
-    _passing__63: Optional7['bool2'] = passing
-    _messages__64: Optional7['MutableSequence10[str1]'] = messages
-    t_285: 'MutableSequence10[str1]'
+  def constructor__61(this__19, failed_on_assert: Optional10['bool2'] = None, passing: Optional10['bool2'] = None, messages: Optional10['MutableSequence13[str1]'] = None) -> 'None':
+    _failedOnAssert__62: Optional10['bool2'] = failed_on_assert
+    _passing__63: Optional10['bool2'] = passing
+    _messages__64: Optional10['MutableSequence13[str1]'] = messages
+    t_285: 'MutableSequence13[str1]'
     if _failedOnAssert__62 is None:
       _failedOnAssert__62 = False
     if _passing__63 is None:
       _passing__63 = True
     if _messages__64 is None:
-      t_285 = list_1271()
+      t_285 = list_1279()
       _messages__64 = t_285
     this__19._failedOnAssert__58 = _failedOnAssert__62
     this__19._passing__59 = _passing__63
     this__19._messages__60 = _messages__64
-  def __init__(this__19, failed_on_assert: Optional7['bool2'] = None, passing: Optional7['bool2'] = None, messages: Optional7['MutableSequence10[str1]'] = None) -> None:
-    _failedOnAssert__62: Optional7['bool2'] = failed_on_assert
-    _passing__63: Optional7['bool2'] = passing
-    _messages__64: Optional7['MutableSequence10[str1]'] = messages
+  def __init__(this__19, failed_on_assert: Optional10['bool2'] = None, passing: Optional10['bool2'] = None, messages: Optional10['MutableSequence13[str1]'] = None) -> None:
+    _failedOnAssert__62: Optional10['bool2'] = failed_on_assert
+    _passing__63: Optional10['bool2'] = passing
+    _messages__64: Optional10['MutableSequence13[str1]'] = messages
     this__19.constructor__61(_failedOnAssert__62, _passing__63, _messages__64)
-test_name: 'Any9' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: String: Type>>', NotImplemented)[1]
-test_fun: 'Any9' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: fn (Test): (Void | Bubble): Type>>', NotImplemented)[1]
-test_case: 'Any9' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: Pair<String, fn (Test): (Void | Bubble)>: Type>>', NotImplemented)[1]
-test_failure_message: 'Any9' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: String: Type>>', NotImplemented)[1]
-test_result: 'Any9' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: Pair<String, List<String>>: Type>>', NotImplemented)[1]
-def process_test_cases(testCases__65: 'Sequence6[(Pair_1275[str1, (Callable4[[Test], None])])]') -> 'Sequence6[(Pair_1275[str1, (Sequence6[str1])])]':
-  global list_map_1276
-  def fn__278(testCase__67: 'Pair_1275[str1, (Callable4[[Test], None])]') -> 'Pair_1275[str1, (Sequence6[str1])]':
-    global Pair_1275, tuple_1274
+test_name: 'Any12' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: String: Type>>', NotImplemented)[1]
+test_fun: 'Any12' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: fn (Test): (Void | Bubble): Type>>', NotImplemented)[1]
+test_case: 'Any12' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: Pair<String, fn (Test): (Void | Bubble)>: Type>>', NotImplemented)[1]
+test_failure_message: 'Any12' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: String: Type>>', NotImplemented)[1]
+test_result: 'Any12' = ('<<lang.temper.value.TType: Type, lang.temper.value.Value: Pair<String, List<String>>: Type>>', NotImplemented)[1]
+def process_test_cases(testCases__65: 'Sequence9[(Pair_1283[str1, (Callable4[[Test], None])])]') -> 'Sequence9[(Pair_1283[str1, (Sequence9[str1])])]':
+  global list_map_1284
+  def fn__278(testCase__67: 'Pair_1283[str1, (Callable4[[Test], None])]') -> 'Pair_1283[str1, (Sequence9[str1])]':
+    global Pair_1283, tuple_1282
     t_269: 'bool2'
-    t_271: 'Sequence6[str1]'
+    t_271: 'Sequence9[str1]'
     t_168: 'bool2'
     key__69: 'str1' = testCase__67.key
     fun__70: 'Callable4[[Test], None]' = testCase__67.value
     test__71: 'Test' = Test()
     hadBubble__72: 'bool2'
     try:
       fun__70(test__71)
       hadBubble__72 = False
-    except Exception12:
+    except Exception15:
       hadBubble__72 = True
-    messages__73: 'Sequence6[str1]' = test__71.messages()
-    failures__74: 'Sequence6[str1]'
+    messages__73: 'Sequence9[str1]' = test__71.messages()
+    failures__74: 'Sequence9[str1]'
     if test__71.passing:
       failures__74 = ()
     else:
       if hadBubble__72:
         t_269 = test__71.failed_on_assert
         t_168 = not t_269
       else:
         t_168 = False
       if t_168:
-        allMessages__75: 'MutableSequence10[str1]' = list_1271(messages__73)
-        list_builder_add_1246(allMessages__75, 'Bubble')
-        t_271 = tuple_1274(allMessages__75)
+        allMessages__75: 'MutableSequence13[str1]' = list_1279(messages__73)
+        list_builder_add_1254(allMessages__75, 'Bubble')
+        t_271 = tuple_1282(allMessages__75)
         failures__74 = t_271
       else:
         failures__74 = messages__73
-    return Pair_1275(key__69, failures__74)
-  return list_map_1276(testCases__65, fn__278)
-def report_test_results(testResults__76: 'Sequence6[(Pair_1275[str1, (Sequence6[str1])])]') -> 'None':
+    return Pair_1283(key__69, failures__74)
+  return list_map_1284(testCases__65, fn__278)
+def report_test_results(testResults__76: 'Sequence9[(Pair_1283[str1, (Sequence9[str1])])]') -> 'None':
   global console_88
   t_256: 'int5'
   t_257: 'str1'
   t_261: 'str1'
-  t_154: 'Pair_1275[str1, (Sequence6[str1])]'
+  t_154: 'Pair_1283[str1, (Sequence9[str1])]'
   i__78: 'int5' = 0
-  with Label13() as s__1277_1278:
+  with Label16() as s__1285_1286:
     while True:
-      t_256 = len_1254(testResults__76)
+      t_256 = len_1262(testResults__76)
       if i__78 < t_256:
         try:
-          t_154 = list_get_1255(testResults__76, i__78)
-        except Exception12:
+          t_154 = list_get_1263(testResults__76, i__78)
+        except Exception15:
           break
-        testResult__79: 'Pair_1275[str1, (Sequence6[str1])]' = t_154
-        failureMessages__80: 'Sequence6[str1]' = testResult__79.value
+        testResult__79: 'Pair_1283[str1, (Sequence9[str1])]' = t_154
+        failureMessages__80: 'Sequence9[str1]' = testResult__79.value
         if not failureMessages__80:
           t_261 = testResult__79.key
-          console_88.log(str_cat_1265(t_261, ': Passed'))
+          console_88.log(str_cat_1273(t_261, ': Passed'))
         else:
           def fn__254(it__82: 'str1') -> 'str1':
             return it__82
-          message__81: 'str1' = list_join_1242(failureMessages__80, ', ', fn__254)
+          message__81: 'str1' = list_join_1250(failureMessages__80, ', ', fn__254)
           t_257 = testResult__79.key
-          console_88.log(str_cat_1265(t_257, ': Failed ', message__81))
+          console_88.log(str_cat_1273(t_257, ': Failed ', message__81))
         i__78 = i__78 + 1
       else:
-        s__1277_1278.break_()
-    raise RuntimeError14()
-def run_test_cases(testCases__83: 'Sequence6[(Pair_1275[str1, (Callable4[[Test], None])])]') -> 'None':
+        s__1285_1286.break_()
+    raise RuntimeError8()
+def run_test_cases(testCases__83: 'Sequence9[(Pair_1283[str1, (Callable4[[Test], None])])]') -> 'None':
   global process_test_cases, report_test_results
   report_test_results(process_test_cases(testCases__83))
 def run_test(testFun__85: 'Callable4[[Test], None]') -> 'None':
   test__87: 'Test' = Test()
   testFun__85(test__87)
   test__87.soft_fail_to_hard()
```

### Comparing `temper_std-0.2.1/temper_std/testing.py.map` & `temper_std-0.3.0/temper_std/testing.py.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8983516483516484%*

 * *Differences: {"'mappings'": "'A,mB,G,I,K,E,e,I,iB,E,Q,I,S,E,Q,I,S,E,K,I,O,E,Q,I;A,wB,c,I,gB,E,I,I,S,E,K,I,O,E,gB,I,qB,E,S,I,c,E,Q,I,a,E,Q,I,a,E,O,I;A,qB,I,I,K,E,G,I,I,E,S,I,W,E,G,I,I,E,Y,I,a,E,K,I,U,E,I,I,S,E,G,I;AAOiB+B,UAAA,YAAAzB,gBAAA;AAAA,MAAA0B,IAAA;AAwDJ,EAAAC,WAAA,CAAA,AAxDI,QA4FuD;AApB3D,EAAAC,kBAAA,CAAA,AAxEI,QA4FuD;AAhB3D,EAAAC,oBAAA,CAAA,AA5EI,QA4FuD;AAFtD,EAAAC,mBAAe,CAAE;AACjB,EAAAC,YAAQ,CAAE;AACd,EAAAC,aAAS,CAAE,0BAA+C;AA5FvD,WA4FuD,EAAA,AA5FvD,EAwDJ,cAgBA,sBAIA,wBAcI,sBAAiC,CACjC,eAAyB,CAC5B,gBAA0D,CAAA; […]*

```diff
@@ -1,42 +1,42 @@
 {
     "file": "py/std/temper_std/testing.py",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "Any",
         "MutableSequence",
         "Callable",
         "Sequence",
         "Union",
         "Optional",
         "LoggingConsole",
         "Pair",
-        "Pair#1275",
+        "Pair#1283",
         "Label",
         "list_builder_add",
-        "list_builder_add#1246",
+        "list_builder_add#1254",
         "list_join",
-        "list_join#1242",
+        "list_join#1250",
         "list_map",
-        "list_map#1276",
+        "list_map#1284",
         "list_get",
-        "list_get#1255",
+        "list_get#1263",
         "str_cat",
-        "str_cat#1265",
+        "str_cat#1273",
         "bool",
         "str",
         "Exception",
         "int",
         "RuntimeError",
         "tuple",
-        "tuple#1274",
+        "tuple#1282",
         "list",
-        "list#1271",
+        "list#1279",
         "len",
-        "len#1254",
+        "len#1262",
         "console#88",
         "Test",
         "passing",
         "failedOnAssert",
         "hasUnhandledFail",
         "_failedOnAssert",
         "_passing",
@@ -73,15 +73,15 @@
         "reportTestResults",
         "testResults",
         "t#256",
         "t#257",
         "t#261",
         "t#154",
         "i",
-        "s__1277#1278",
+        "s__1285#1286",
         "testResult",
         "failureMessages",
         "runTestCases",
         "runTest",
         "testFun"
     ],
     "sources": [
```

