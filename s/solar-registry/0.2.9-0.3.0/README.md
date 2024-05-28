# Comparing `tmp/solar_registry-0.2.9.tar.gz` & `tmp/solar_registry-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.9.tar", last modified: Thu May 16 02:30:58 2024, max compression
+gzip compressed data, was "solar_registry-0.3.0.tar", last modified: Mon May 27 11:57:02 2024, max compression
```

## Comparing `solar_registry-0.2.9.tar` & `solar_registry-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,35 @@
--rw-r--r--   0        0        0    11357 2024-05-16 02:30:35.744616 solar_registry-0.2.9/LICENSE
--rw-r--r--   0        0        0      682 2024-05-16 02:30:35.744616 solar_registry-0.2.9/README.md
--rw-r--r--   0        0        0     1240 2024-05-16 02:30:58.312821 solar_registry-0.2.9/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     2228 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4959 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     4161 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/cos_sync.py
--rw-r--r--   0        0        0     2517 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     2068 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/__init__.py
--rw-r--r--   0        0        0      364 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_cos_sync.py
--rw-r--r--   0        0        0      680 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_testtool.py
--rw-r--r--   0        0        0      291 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_validator.py
--rw-r--r--   0        0        0      731 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2778 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     2942 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-27 11:56:39.327552 solar_registry-0.3.0/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-27 11:56:39.327552 solar_registry-0.3.0/README.md
+-rw-r--r--   0        0        0     1240 2024-05-27 11:57:02.587620 solar_registry-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     5891 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/asset.py
+-rw-r--r--   0        0        0     1009 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/legacy.py
+-rw-r--r--   0        0        0     4538 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/py.typed
+-rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     5496 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     3003 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2699 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      956 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2069 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-27 11:56:39.327552 solar_registry-0.3.0/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-27 11:56:39.327552 solar_registry-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_cos_sync.py
+-rw-r--r--   0        0        0     1512 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_merger.py
+-rw-r--r--   0        0        0      503 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_pr_generator.py
+-rw-r--r--   0        0        0     3842 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_testtool.py
+-rw-r--r--   0        0        0      299 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/test_validator.py
+-rw-r--r--   0        0        0      730 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_loose.yaml
+-rw-r--r--   0        0        0     1249 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict.yaml
+-rw-r--r--   0        0        0      774 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml
+-rw-r--r--   0        0        0      763 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml
+-rw-r--r--   0        0        0     1405 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/legacy/testtool.yaml
+-rw-r--r--   0        0        0     3074 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     3090 2024-05-27 11:56:39.331552 solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.3.0/PKG-INFO
```

### Comparing `solar_registry-0.2.9/LICENSE` & `solar_registry-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.9/README.md` & `solar_registry-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.9/pyproject.toml` & `solar_registry-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.2.9"
+version = "0.3.0"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.2.9/src/solar_registry/cli.py` & `solar_registry-0.3.0/src/solar_registry/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typer
 from loguru import logger
 from typing_extensions import Annotated
 
 from .commands.meta_merger import MetaMerger
 from .service.cos_sync import CosSyncService
 from .service.pr_generator import PullRequestGenerator
-from .service.testtool import get_testtool
+from .service.testtool import get_testtool, github_asset_gen
 from .service.validator import ToolValidator
 
 app = typer.Typer()
 
 
 @app.command()
 def merge(tool_name: str, output: str, working_dir: Optional[str] = None) -> None:
@@ -20,15 +20,15 @@
     合并工具版本元数据
 
     :param tool_name: 工具名称
     :param output: registry仓库本地目录
     :param working_dir: 可选工作目录
     """
     testtool = get_testtool(tool_name, working_dir)
-    merger = MetaMerger(testtool)
+    merger = MetaMerger(testtool, asset_url_gen=github_asset_gen)
     merger.merge_index_and_history(Path(output))
 
 
 @app.command()
 def pull_request(
     tool_name: Annotated[str, typer.Argument(help="工具名称")],
     working_dir: Annotated[Optional[str], typer.Argument(help="可选工作目录")] = None,
@@ -46,15 +46,15 @@
     """
     校验测试工具的testtools.yaml是否符合要求
 
     :param tool_name: 工具名称
     :param working_dir: 可选工作目录
     """
     testtool = get_testtool(tool_name, working_dir)
-    logger.info(f"测试工具 {testtool.name} 有效性校验通过")
+    logger.info(f"✅ 测试工具 {testtool.name} 有效性校验通过")
 
 
 @app.command()
 def validate_json(working_dir: Optional[str] = None) -> None:
     """
     校验当前目录下的json文件是否符合要求
```

### Comparing `solar_registry-0.2.9/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.3.0/src/solar_registry/commands/meta_merger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import tempfile
 from pathlib import Path
 
+from typing import Callable
 from loguru import logger
 from requests import HTTPError
 
 from ..model.test_tool import (
     StableIndexMetaData,
     MetaDataHistory,
     TestTool,
+    TestToolMetadata,
 )
 from ..service.generator import Generator
 from ..util.file import download_file_to
 
 
 class MetaMerger:
-    def __init__(self, testtool: TestTool):
+    def __init__(self, testtool: TestTool, asset_url_gen: Callable[[TestTool], str]):
         self.testtool = testtool
 
-        gen = Generator(self.testtool)
+        gen = Generator(self.testtool, asset_url_gen)
         self.metadata = gen.generate_meta_data()
 
     def merge_index_and_history(self, output_dir: Path) -> None:
         """
         合并新的索引文件和版本文件
         :param output_dir:  registry目录
         :return:
@@ -111,33 +113,54 @@
             for index, tool in enumerate(stable_result.tools):
                 if tool.name == self.testtool.name:
                     stable_result.tools[index] = self.testtool
                     break
             else:
                 stable_result.tools.append(self.testtool)
 
-            logger.info(f"Merge stable index: {stable_result}")
+            logger.info(
+                f"Merge stable index: {stable_result.model_dump_json(by_alias=True, indent=2, exclude_none=True)}"
+            )
             return stable_result
 
     def _merge_meta_history(self, history: MetaDataHistory) -> MetaDataHistory:
         logger.info("Merging meta history...")
         if not history.versions:
             history.versions = []
 
-        for index, version in enumerate(history.versions):
-            if version.meta.version == self.metadata.meta.version:
-                history.versions[index] = self.metadata
-                break
-        else:
-            history.versions.append(self.metadata)
+        self._upsert_meta_history(tool_meta=self.metadata, history=history)
+
+        # 在历史记录中增加一个固定的stable版本，方便用户使用
+        stable_version = self.metadata.model_copy(deep=True)
+        stable_version.meta.version = "stable"
+        self._upsert_meta_history(tool_meta=stable_version, history=history)
 
         logger.info(
             f"Merge meta history result: {history.model_dump_json(by_alias=True, indent=2, exclude_none=True)}"
         )
 
         return history
 
+    @staticmethod
+    def _upsert_meta_history(
+        tool_meta: TestToolMetadata, history: MetaDataHistory
+    ) -> MetaDataHistory:
+        for index, version in enumerate(history.versions):
+            if version.meta.version == tool_meta.meta.version:
+                history.versions[index] = tool_meta
+                break
+        else:
+            history.versions.append(tool_meta)
+
+        return history
+
     def _create_new_metadata_history(self) -> MetaDataHistory:
         # 读取本地生成好的metadata文件
         logger.info("Creating meta history...")
         history = MetaDataHistory(versions=[self.metadata])
+
+        # 在历史记录中增加一个固定的stable版本，方便用户使用
+        stable_version = self.metadata.model_copy(deep=True)
+        stable_version.meta.version = "stable"
+        history.versions.append(stable_version)
+
         return history
```

### Comparing `solar_registry-0.2.9/src/solar_registry/service/cos_sync.py` & `solar_registry-0.3.0/src/solar_registry/service/cos_sync.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,56 @@
 import hashlib
 import os
+import tarfile
 import tempfile
-
-from loguru import logger
-
 from pathlib import Path
+from typing import Callable
 
+from loguru import logger
 from qcloud_cos import CosS3Client, CosConfig  # type: ignore[import-untyped]
 
+from ..model.asset import gen_asset_relative_path
+from ..model.test_tool import TestTool
+
 
 class CosSyncService:
-    def __init__(self, workdir: str | None = None) -> None:
+    def __init__(
+        self,
+        workdir: str | None = None,
+        endpoint_gen: Callable[[str], str] | None = None,
+    ) -> None:
         self.workdir = workdir or os.getcwd()
         if "COS_SECRET_ID" not in os.environ:
             raise ValueError("Environment COS_SECRET_ID variables not set")
+        self.cos_secret_id = os.environ["COS_SECRET_ID"]
         if "COS_SECRET_KEY" not in os.environ:
             raise ValueError("Environment COS_SECRET_KEY variables not set")
+        self.cos_secret_key = os.environ["COS_SECRET_KEY"]
         if "COS_REGION" not in os.environ:
             raise ValueError("Environment COS_REGION variables not set")
         self.cos_region = os.environ["COS_REGION"]
         if "COS_BUCKET" not in os.environ:
             raise ValueError("Environment COS_BUCKET variables not set")
         self.cos_bucket = os.environ["COS_BUCKET"]
 
-        self.cos_client = CosS3Client(
-            CosConfig(
-                Region=os.environ["COS_REGION"],
-                SecretId=os.environ["COS_SECRET_ID"],
-                SecretKey=os.environ["COS_SECRET_KEY"],
+        if endpoint_gen:
+            config = CosConfig(
+                Region=self.cos_region,
+                SecretId=self.cos_secret_id,
+                SecretKey=self.cos_secret_key,
+                Endpoint=endpoint_gen(self.cos_region),
             )
-        )
+        else:
+            config = CosConfig(
+                Region=self.cos_region,
+                SecretId=self.cos_secret_id,
+                SecretKey=self.cos_secret_key,
+            )
+
+        self.cos_client = CosS3Client(config)
 
     def sync_meta_data(self, force: bool) -> None:
         for dir_path, _, filenames in os.walk(Path(self.workdir) / "testtools"):
             for filename in filenames:
                 full_path = Path(dir_path, filename)
                 logger.info(f"Syncing {full_path}")
                 relative_path = os.path.relpath(full_path, self.workdir)
@@ -76,21 +93,34 @@
                 logger.info(
                     f"File {relative_file} does not exist on cos, start upload..."
                 )
                 self.upload_file_to_cos(
                     relative_file=relative_file, full_path=str(full_path)
                 )
 
+    def upload_archive_file(self, test_tool: TestTool) -> None:
+        # 生成对应测试工具的压缩包，并上传到COS的指定位置
+        with tempfile.TemporaryDirectory() as tmpdir:
+            output_file = Path(tmpdir) / f"{test_tool.name}.tar.gz"
+            with tarfile.open(output_file, "w:gz") as tar:
+                tar.add(Path(self.workdir) / test_tool.name, arcname=test_tool.name)
+
+            cos_file_path = gen_asset_relative_path(testtool=test_tool)
+            logger.info(f"Uploading {cos_file_path} to COS bucket {self.cos_bucket}...")
+            self.upload_file_to_cos(
+                relative_file=cos_file_path, full_path=str(output_file)
+            )
+            logger.info(f"✅ Uploaded {cos_file_path} to COS bucket {self.cos_bucket}")
+
     def upload_file_to_cos(self, relative_file: str, full_path: str) -> None:
         response = self.cos_client.upload_file(
             Bucket=self.cos_bucket,
             Key=relative_file,
             LocalFilePath=full_path,
             EnableMD5=True,
-            ACL="public-read",
             progress_callback=None,
         )
         logger.info(
             f"✅ relative_file {relative_file} uploaded, ETag: {response['ETag']}"
         )
```

### Comparing `solar_registry-0.2.9/src/solar_registry/service/generator.py` & `solar_registry-0.3.0/src/solar_registry/service/generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,76 @@
 import hashlib
 from pathlib import Path
+from typing import Callable
 
 from loguru import logger
 
 from ..model.test_tool import (
     TestTool,
     TestToolTarget,
-    OsType,
-    ArchType,
     TestToolMetadata,
 )
 from ..util.file import download_file_to
 
 
 class Generator:
-    def __init__(self, testtool: TestTool):
+    def __init__(self, testtool: TestTool, asset_url_gen: Callable[[TestTool], str]):
         self.testtool = testtool
+        self.asset_url_gen = asset_url_gen
 
     def generate_meta_data(self) -> TestToolMetadata:
         """
         生成测试工具元数据，包含工具信息和最新的版本信息
         """
         logger.info(
-            f"Generating meta data for {self.testtool.model_dump_json(by_alias=True, indent=2)}"
+            f"Generating meta data for {self.testtool.model_dump_json(by_alias=True, indent=2, exclude_none=True)}"
         )
-        sha256 = self.compute_asset_sha256(self.testtool)
 
-        metadata = TestToolMetadata(
-            meta=self.testtool, target=self.generate_targets(self.testtool, sha256)
-        )
-
-        logger.info(
-            f"Generated metadata: {metadata.model_dump_json(indent=2, by_alias=True)}"
-        )
+        if not self.testtool.legacy_spec:
+            sha256 = self.compute_asset_sha256(self.testtool)
+            metadata = TestToolMetadata(
+                meta=self.testtool, target=self.generate_targets(self.testtool, sha256)
+            )
+            logger.info(
+                f"Generated metadata: {metadata.model_dump_json(indent=2, by_alias=True, exclude_none=True)}"
+            )
+        else:
+            logger.info(
+                f"Testtool {self.testtool.name} is legacy tool, skip target generation."
+            )
+            metadata = TestToolMetadata(meta=self.testtool, target=[])
 
         return metadata
 
     def generate_targets(self, testtool: TestTool, sha256: str) -> list[TestToolTarget]:
         re: list[TestToolTarget] = []
-        for _os in [OsType.Linux, OsType.Windows, OsType.Darwin]:
-            for arch in [ArchType.Amd64, ArchType.Arm64]:
+
+        assert testtool.support_os
+        assert testtool.support_arch
+
+        for _os in testtool.support_os:
+            for arch in testtool.support_arch:
                 re.append(
                     TestToolTarget(
                         os=_os,
                         arch=arch,
                         downloadUrl=self.generate_asset_url(testtool),
                         sha256=sha256,
                     )
                 )
         return re
 
-    @staticmethod
-    def generate_asset_url(testtool: TestTool) -> str:
-        return f"https://github.com/OpenTestSolar/testtool-{testtool.lang}-{testtool.name}/archive/refs/tags/{testtool.version}.tar.gz"
+    def generate_asset_url(self, testtool: TestTool) -> str:
+        """
+        指定产物的URL
+
+        不同场景下，可能产物的URL需要定制，因此这个需要能动态配置
+        """
+
+        return self.asset_url_gen(testtool)
 
     def compute_asset_sha256(self, testtool: TestTool) -> str:
         # 读取本次发布的产物信息，并计算sha256值
         output_file = (
             Path("/tmp/testsolar/generate")
             / testtool.lang
             / testtool.name
```

### Comparing `solar_registry-0.2.9/src/solar_registry/service/pr_generator.py` & `solar_registry-0.3.0/src/solar_registry/service/pr_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import tempfile
 from pathlib import Path
 
 from loguru import logger
 
 from ..commands.meta_merger import MetaMerger
 from ..model.test_tool import TestTool
+from .testtool import github_asset_gen
 
 
 class PullRequestGenerator:
     def __init__(self, testtool: TestTool):
         self.testtool = testtool
 
     def merge_and_create_pull_request(self) -> None:
@@ -33,15 +34,15 @@
                     "-b",
                     branch_name,
                 ],
                 cwd=git_dir,
                 check=True,
             )
 
-            merger = MetaMerger(self.testtool)
+            merger = MetaMerger(self.testtool, asset_url_gen=github_asset_gen)
             merger.merge_index_and_history(git_dir)
 
             subprocess.run(["git", "add", "."], cwd=git_dir, check=True)
             subprocess.run(
                 [
                     "git",
                     "commit",
```

### Comparing `solar_registry-0.2.9/src/solar_registry/service/validator.py` & `solar_registry-0.3.0/src/solar_registry/service/validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     def validate_stable_index(self) -> None:
         stable_index_file = Path(self.workdir) / "testtools" / "stable.index.json"
         logger.info(f"Validating stable index file [{stable_index_file}]")
 
         with open(stable_index_file) as f:
             sim = StableIndexMetaData.model_validate_json(f.read())
+
             logger.info(f"✅ Validated stable index file [{stable_index_file}] OK.")
             logger.info(f"✅ It has {len(sim.tools)} tools.")
 
     def validate_tool_meta_json(self) -> None:
         for dir_path, _, filenames in os.walk(self.workdir / "testtools"):
             for filename in filenames:
                 if filename != "stable.index.json":
```

### Comparing `solar_registry-0.2.9/src/solar_registry/util/file.py` & `solar_registry-0.3.0/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.9/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_loose.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 defaultBaseImage: python:3.10 # 用户在 TestContainer 配置中未指定 baseImage 时的默认镜像
 scaffoldRepo: https://github.com/OpenTestSolar/testtool-scaffold-python-pytest/archive/refs/tags/0.1.0.tar.gz
 indexFile: https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/stable.index.json
 versionFile: https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/python/pytest/metadata.json
 homePage: https://github.com/OpenTestSolar/testtool-python-pytest
 entry:
   load: "python3 /testtools/qta/src/load.py $1"
-  run: "python3 /testtools/qta/src/run.py $1"
+  run: "python3 /testtools/qta/src/run.py $1"
```

### Comparing `solar_registry-0.2.9/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.3.0/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 schemaVersion: 1.0
-name: pytest
+name: PyTest
 lang: python
 langType: "INTERPRETED"
 description: Pytest测试工具
-version: '0.1.3.beta'
+version: '0.1.3'
 defaultBaseImage: python:3.10 # 用户在 TestContainer 配置中未指定 baseImage 时的默认镜像
 scaffoldRepo: https://github.com/OpenTestSolar/testtool-scaffold-python-pytest/archive/refs/tags/0.1.0.tar.gz
 indexFile: https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/stable.index.json
 versionFile: https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/python/pytest/metadata.json
 homePage: https://github.com/OpenTestSolar/testtool-python-pytest
 entry:
   load: "python3 /testtools/qta/src/load.py $1"
   run: "python3 /testtools/qta/src/run.py $1"
+supportArch:
+  - amd64
+  - arm64
```

### Comparing `solar_registry-0.2.9/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.3.0/tests/testdata/pytest/testtool.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 schemaVersion: 1.0
 name: pytest
+nameZh: pytest自动化测试
 lang: python
 langType: "INTERPRETED"
 description: Pytest测试工具
 version: '0.1.6'
 defaultBaseImage: python:3.10 # 用户在 TestContainer 配置中未指定 baseImage 时的默认镜像
 scaffoldRepo: https://github.com/OpenTestSolar/testtool-scaffold-python-pytest/archive/refs/tags/0.1.0.tar.gz
 indexFile: https://opentestsolar.github.io/testtool-registry/testtools/stable.index.json
 versionFile: https://opentestsolar.github.io/testtool-registry/testtools/python/pytest/metadata.json
 homePage: https://github.com/OpenTestSolar/testtool-python-pytest
 parameterDefs: # 用户 use 这个测试工具时可以配置的 with 参数
   - name: parseMode
     value: 加载用例的模式
+    desc: 加载用例的模式
     default: auto
     choices:
       - value: auto
         desc: 根据测试文件的内容自动识别加载模式。数据驱动用例使用 `qtaf` 模式，其余用例使用 `ast` 模式。
       - value: ast
         desc: |
           使用python内置的ast模块，运行静态语法分析模式来解析测试用例。
@@ -36,14 +38,15 @@
             - 支持数据驱动用例解析
           
           缺点：
             - 用户测试用例有运行时依赖，在加载阶段可能无法成功
             - 依赖测试运行的pip包，解析速度较慢
   - name: runMode
     value: 运行用例的模式
+    desc: 加载用例的模式
     default: singleprocess # choice: singleprocess/multiprocess
     choices:
       - value: singleprocess
         desc: |
           使用单进程执行测试用例，一般用于串行模式。
           
           优点：
@@ -60,14 +63,24 @@
             - 整体执行效率高
           
           缺点：
             - 不保证用例执行顺序
             - 单机并发量设置太高可能导致执行机异常
   - name: qtafSettings
     value: QTAF测试项目配置
+    desc: QTAF测试项目配置
     default: ""
   - name: extraFieldsConfig
     value: 用例额外属性
+    desc: 用例额外属性
     default: ""
 entry:
   load: "python3 /testtools/qta/src/load.py $1"
   run: "python3 /testtools/qta/src/run.py $1"
+supportOS:
+  - windows
+  - linux
+  - darwin
+supportArch:
+  - amd64
+  - arm64
+gitPkgUrl: github.com/OpenTestSolar/testtool-python@main:pytest
```

### Comparing `solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.3.0/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'tools'": "{0: {'supportOS': ['windows', 'linux', 'darwin'], 'supportArch': ['amd64', 'arm64']}}"}*

```diff
@@ -53,12 +53,21 @@
                     "default": "",
                     "name": "extraFieldsConfig",
                     "value": "\u7528\u4f8b\u989d\u5916\u5c5e\u6027"
                 }
             ],
             "scaffoldRepo": "https://github.com/OpenTestSolar/testtool-scaffold-python-pytest/archive/refs/tags/0.1.0.tar.gz",
             "schemaVersion": 1.0,
+            "supportArch": [
+                "amd64",
+                "arm64"
+            ],
+            "supportOS": [
+                "windows",
+                "linux",
+                "darwin"
+            ],
             "version": "0.1.4",
             "versionFile": "https://raw.githubusercontent.com/OpenTestSolar/testtool-registry/main/testtools/python/pytest/metadata.json"
         }
     ]
 }
```

### Comparing `solar_registry-0.2.9/PKG-INFO` & `solar_registry-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.9
+Version: 0.3.0
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

