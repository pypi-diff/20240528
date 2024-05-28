# Comparing `tmp/solar_registry-0.3.0.tar.gz` & `tmp/solar_registry-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.3.0.tar", last modified: Mon May 27 11:57:02 2024, max compression
+gzip compressed data, was "solar_registry-0.3.1.tar", last modified: Tue May 28 02:48:40 2024, max compression
```

## Comparing `solar_registry-0.3.0.tar` & `solar_registry-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11357 2024-05-27 11:56:39.327552 solar_registry-0.3.0/LICENSE
--rw-r--r--   0        0        0      682 2024-05-27 11:56:39.327552 solar_registry-0.3.0/README.md
--rw-r--r--   0        0        0     1240 2024-05-27 11:57:02.587620 solar_registry-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     2282 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     5891 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0      298 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/asset.py
--rw-r--r--   0        0        0     1009 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/legacy.py
--rw-r--r--   0        0        0     4538 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/py.typed
--rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     5496 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/cos_sync.py
--rw-r--r--   0        0        0     3003 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2699 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      956 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     2069 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      383 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_cos_sync.py
--rw-r--r--   0        0        0     1512 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_merger.py
--rw-r--r--   0        0        0      503 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_pr_generator.py
--rw-r--r--   0        0        0     3842 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_testtool.py
--rw-r--r--   0        0        0      299 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_validator.py
--rw-r--r--   0        0        0      730 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_loose.yaml
--rw-r--r--   0        0        0     1249 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict.yaml
--rw-r--r--   0        0        0      774 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml
--rw-r--r--   0        0        0      763 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml
--rw-r--r--   0        0        0     1405 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/legacy/testtool.yaml
--rw-r--r--   0        0        0     3074 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     3090 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 02:48:16.595188 solar_registry-0.3.1/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-28 02:48:16.595188 solar_registry-0.3.1/README.md
+-rw-r--r--   0        0        0     1240 2024-05-28 02:48:40.639181 solar_registry-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     5891 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/model/asset.py
+-rw-r--r--   0        0        0     1009 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/model/legacy.py
+-rw-r--r--   0        0        0     4536 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/py.typed
+-rw-r--r--   0        0        0        0 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     5496 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     3003 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2699 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      956 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2069 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-28 02:48:16.599187 solar_registry-0.3.1/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-28 02:48:16.599187 solar_registry-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-28 02:48:16.599187 solar_registry-0.3.1/tests/test_cos_sync.py
+-rw-r--r--   0        0        0     1512 2024-05-28 02:48:16.599187 solar_registry-0.3.1/tests/test_merger.py
+-rw-r--r--   0        0        0      503 2024-05-28 02:48:16.599187 solar_registry-0.3.1/tests/test_pr_generator.py
+-rw-r--r--   0        0        0     3842 2024-05-28 02:48:16.599187 solar_registry-0.3.1/tests/test_testtool.py
+-rw-r--r--   0        0        0      299 2024-05-28 02:48:16.599187 solar_registry-0.3.1/tests/test_validator.py
+-rw-r--r--   0        0        0      730 2024-05-28 02:48:16.599187 solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_loose.yaml
+-rw-r--r--   0        0        0     1249 2024-05-28 02:48:16.603187 solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_strict.yaml
+-rw-r--r--   0        0        0      774 2024-05-28 02:48:16.603187 solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml
+-rw-r--r--   0        0        0      763 2024-05-28 02:48:16.603187 solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml
+-rw-r--r--   0        0        0     1405 2024-05-28 02:48:16.603187 solar_registry-0.3.1/tests/testdata/legacy/testtool.yaml
+-rw-r--r--   0        0        0     3074 2024-05-28 02:48:16.603187 solar_registry-0.3.1/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-28 02:48:16.603187 solar_registry-0.3.1/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     3090 2024-05-28 02:48:16.603187 solar_registry-0.3.1/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.3.1/PKG-INFO
```

### Comparing `solar_registry-0.3.0/LICENSE` & `solar_registry-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/README.md` & `solar_registry-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/pyproject.toml` & `solar_registry-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.3.0"
+version = "0.3.1"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.3.0/src/solar_registry/cli.py` & `solar_registry-0.3.1/src/solar_registry/cli.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.3.1/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/model/legacy.py` & `solar_registry-0.3.1/src/solar_registry/model/legacy.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/model/test_tool.py` & `solar_registry-0.3.1/src/solar_registry/model/test_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 测试工具模型定义
 
 这里面的模型都是对外体现的
 """
 
 from enum import Enum
-from typing import Literal
+from typing import Literal, Self
 
 from pydantic import BaseModel, Field, ValidationInfo, model_validator
-from typing_extensions import Self
 
 from .legacy import LegacySpec
 
 
 class ParamChoice(BaseModel):
     value: str
     desc: str
@@ -116,15 +115,16 @@
                 if not self.version_file:
                     raise ValueError("versionFile must be set")
                 if not self.index_file:
                     raise ValueError("indexFile must be set")
                 if not self.scaffold_repo:
                     raise ValueError("scaffoldRepo must be set")
 
-            assert self.name_zh, "should have nameZh in yaml"
+            if not self.name_zh:
+                raise ValueError("name_zh must be set")
 
         return self
 
 
 class TestToolTarget(BaseModel):
     __test__ = False
```

### Comparing `solar_registry-0.3.0/src/solar_registry/service/cos_sync.py` & `solar_registry-0.3.1/src/solar_registry/service/cos_sync.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/service/generator.py` & `solar_registry-0.3.1/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/service/pr_generator.py` & `solar_registry-0.3.1/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/service/testtool.py` & `solar_registry-0.3.1/src/solar_registry/service/testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/service/validator.py` & `solar_registry-0.3.1/src/solar_registry/service/validator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/src/solar_registry/util/file.py` & `solar_registry-0.3.1/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/test_merger.py` & `solar_registry-0.3.1/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/test_testtool.py` & `solar_registry-0.3.1/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_loose.yaml` & `solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_loose.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict.yaml` & `solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_strict.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml` & `solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml` & `solar_registry-0.3.1/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/legacy/testtool.yaml` & `solar_registry-0.3.1/tests/testdata/legacy/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.3.1/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.3.1/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.3.1/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.0/PKG-INFO` & `solar_registry-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

