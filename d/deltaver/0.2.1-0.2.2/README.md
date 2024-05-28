# Comparing `tmp/deltaver-0.2.1.tar.gz` & `tmp/deltaver-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltaver-0.2.1.tar", max compression
+gzip compressed data, was "deltaver-0.2.2.tar", max compression
```

## Comparing `deltaver-0.2.1.tar` & `deltaver-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1114 2024-02-12 23:08:22.920350 deltaver-0.2.1/LICENSE
--rw-r--r--   0        0        0     1122 2024-02-12 23:08:22.920350 deltaver-0.2.1/README.md
--rw-r--r--   0        0        0       55 2024-02-12 23:08:22.920350 deltaver-0.2.1/deltaver/__init__.py
--rw-r--r--   0        0        0     5121 2024-02-12 23:08:22.920350 deltaver-0.2.1/deltaver/__main__.py
--rw-r--r--   0        0        0      368 2024-02-12 23:08:22.920350 deltaver-0.2.1/deltaver/config.py
--rw-r--r--   0        0        0     1886 2024-02-12 23:08:22.920350 deltaver-0.2.1/deltaver/parsed_requirements.py
--rw-r--r--   0        0        0     6589 2024-02-12 23:08:22.920350 deltaver-0.2.1/deltaver/version_delta.py
--rw-r--r--   0        0        0     2482 2024-02-12 23:08:23.352352 deltaver-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 deltaver-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-05-28 14:02:20.989069 deltaver-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1117 2024-05-28 14:02:20.989069 deltaver-0.2.2/README.md
+-rw-r--r--   0        0        0       55 2024-05-28 14:02:20.989069 deltaver-0.2.2/deltaver/__init__.py
+-rw-r--r--   0        0        0     5687 2024-05-28 14:02:20.989069 deltaver-0.2.2/deltaver/__main__.py
+-rw-r--r--   0        0        0      477 2024-05-28 14:02:20.989069 deltaver-0.2.2/deltaver/config.py
+-rw-r--r--   0        0        0     2220 2024-05-28 14:02:20.989069 deltaver-0.2.2/deltaver/parsed_requirements.py
+-rw-r--r--   0        0        0     7763 2024-05-28 14:02:20.989069 deltaver-0.2.2/deltaver/version_delta.py
+-rw-r--r--   0        0        0     2489 2024-05-28 14:02:21.849065 deltaver-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 deltaver-0.2.2/PKG-INFO
```

### Comparing `deltaver-0.2.1/LICENSE` & `deltaver-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deltaver-0.2.1/README.md` & `deltaver-0.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 ## Overview
 
 The "Deltaver" is a Python project designed to calculate the lag or delay in dependencies in terms of days. It provides insights into how outdated your project dependencies are, helping you stay up-to-date with the latest developments and security patches.
 
 ## Features:
 
- - **Dependency Lag Calculation**: The tool analyzes the timestamp of the current dependency version and compares it with the latest available version, providing the time lag in days.
- - **Security Insights**: Identify outdated dependencies to prioritize updates based on security considerations.
- - **Customization**: Configure the tool to focus on specific dependencies or categories, allowing for flexibility in analysis.
+- **Dependency Lag Calculation**: The tool analyzes the timestamp of the current dependency version and compares it with the latest available version, providing the time lag in days.
+- **Security Insights**: Identify outdated dependencies to prioritize updates based on security considerations.
+- **Customization**: Configure the tool to focus on specific dependencies or categories, allowing for flexibility in analysis.
 
 ## Getting Started
 ### Prerequisites
 
 Make sure you have the following installed:
 
- - Python 3.x
- - Pip (Python package installer)
+- Python 3.x
+- Pip (Python package installer)
 
 ### Installation
 
 ```bash
 pip install deltaver
 ```
```

### Comparing `deltaver-0.2.1/deltaver/__main__.py` & `deltaver-0.2.2/deltaver/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,29 @@
 import typer
 from rich import print
 from rich.console import Console
 from rich.progress import track
 from rich.table import Table
 from typing_extensions import TypeAlias
 
-from deltaver.config import ConfigDict, Formats
-from deltaver.parsed_requirements import ExcludedReqs, FileNotFoundSafeReqs, FreezedReqs, PoetryLockReqs
+from deltaver.config import ConfigDict, Formats, Langs
+from deltaver.parsed_requirements import (
+    ExcludedReqs,
+    FileNotFoundSafeReqs,
+    FreezedReqs,
+    PackageLockReqs,
+    PoetryLockReqs,
+)
 from deltaver.version_delta import (
     CachedSortedVersions,
     DecrDelta,
+    NpmjsVersionsSortedBySemver,
     OvertakingSafeVersionDelta,
     PypiVersionDelta,
-    VersionsSortedBySemver,
+    PypiVersionsSortedBySemver,
 )
 
 app = typer.Typer()
 PackageName: TypeAlias = str
 PackageVersion: TypeAlias = str
 PackageDelta: TypeAlias = float
 FIRST_DATE: Final = datetime.datetime(
@@ -66,30 +73,36 @@
     int,
     int,
     ConfigDict,
 ]:
     sum_delta = 0
     max_delta = 0
     packages = []
-    reqs_obj_ctor = {
-        'freezed': FreezedReqs,
-        'lock': PoetryLockReqs,
-    }[config['file_format'].value]
+    lang_format = {
+        'js': {
+            'lock': (PackageLockReqs, NpmjsVersionsSortedBySemver),
+        },
+        'py': {
+            'freezed': (FreezedReqs, PypiVersionsSortedBySemver),
+            'lock': (PoetryLockReqs, PypiVersionsSortedBySemver),
+        },
+    }[config['lang'].value]
+    reqs_obj_ctor, sorted_versions_ctor = lang_format[config['file_format'].value]  # type: ignore [index]
     dependencies = FileNotFoundSafeReqs(
         ExcludedReqs(
             reqs_obj_ctor(config['path_to_requirements_file']),
             config,
         ),
     ).reqs()
     for package, version in track(dependencies, description='Scanning...'):
         delta = OvertakingSafeVersionDelta(
             DecrDelta(
                 PypiVersionDelta(
                     CachedSortedVersions(
-                        VersionsSortedBySemver(
+                        sorted_versions_ctor(
                             config['artifactory_domain'],
                             package,
                         ),
                         package,
                     ),
                     version,
                 ),
@@ -116,34 +129,38 @@
     file_format: Annotated[str, typer.Option('--format')] = 'freezed',
     fail_on_average: Annotated[int, typer.Option('--fail-on-avg')] = -1,
     fail_on_max: Annotated[int, typer.Option('--fail-on-max')] = -1,
     artifactory_domain: Annotated[str, typer.Option('--artifactory-domain')] = 'https://pypi.org',
     exclude_deps: Annotated[list[str], typer.Option('--exclude')] = [],  # noqa: B006
     # Use unreal date because time_machine.move_to fixture not work for datetime.datetime.now() here
     for_date_param: Annotated[datetime.datetime, typer.Option('--for-date')] = FIRST_DATE_STR,  # type: ignore[assignment]
+    lang: Annotated[str, typer.Option('--lang')] = 'py',
 ) -> None:
-
     if for_date_param.date() == FIRST_DATE:
         for_date = datetime.datetime.now(tz=datetime.timezone.utc)
     else:
         for_date = for_date_param
     pyproject_config_path = Path('pyproject.toml')
     if not pyproject_config_path.exists():
         pyproject_config = {}
     else:
         pyproject_config = toml.loads(pyproject_config_path.read_text()).get('tool', {}).get('deltaver', {})
     config = ConfigDict({
         'path_to_requirements_file': (
             pyproject_config.get('path_to_requirements_file')
             or Path(path_to_requirements_file)
         ),
+        'lang': Langs(lang),
         'file_format': Formats(file_format),
         'fail_on_avg': pyproject_config.get('fail_on_avg') or fail_on_average,
         'fail_on_max': pyproject_config.get('fail_on_max') or fail_on_max,
-        'artifactory_domain': pyproject_config.get('artifactory_domain') or artifactory_domain,
+        'artifactory_domain': pyproject_config.get(
+            'artifactory_domain',
+            {'js': 'https://registry.npmjs.org', 'py': 'https://pypi.org'}.get(lang),
+        ) or artifactory_domain,
         'excluded': pyproject_config.get('excluded') or exclude_deps,
         'for_date': pyproject_config.get('for_date') or for_date.date(),
     })
     results(*controller(config))
 
 
 if __name__ == '__main__':
```

### Comparing `deltaver-0.2.1/deltaver/parsed_requirements.py` & `deltaver-0.2.2/deltaver/parsed_requirements.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import re
 from pathlib import Path
 from typing import Protocol, final
 
 import attrs
 import toml
 import typer
@@ -73,7 +74,21 @@
 
     def reqs(self) -> list[tuple[str, str]]:
         try:
             return self._origin.reqs()
         except FileNotFoundError as err:
             print('Requirements file not found')
             raise typer.Exit(1) from err
+
+
+@final
+@attrs.define(frozen=True)
+class PackageLockReqs(ParsedReqs):
+
+    _path: Path
+
+    def reqs(self) -> list[tuple[str, str]]:
+        data = json.loads(self._path.read_text())
+        return [
+            (name, version_info['version'])
+            for name, version_info in data['dependencies'].items()
+        ]
```

### Comparing `deltaver-0.2.1/deltaver/version_delta.py` & `deltaver-0.2.2/deltaver/version_delta.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             for dict_ in origin_val
         ]))
         return origin_val
 
 
 @final
 @attrs.define(frozen=True)
-class VersionsSortedBySemver(SortedVersions):
+class PypiVersionsSortedBySemver(SortedVersions):
 
     _artifactory_domain: str
     _package_name: str
 
     def fetch(self) -> SortedVersionsList:
         response = httpx.get(
             httpx.URL(self._artifactory_domain).join('pypi/{0}/json'.format(self._package_name)),
@@ -144,14 +144,44 @@
                     })
         return sorted(
             correct_versions,
             key=lambda release_dict: version.parse(next(iter(release_dict.keys()))),
         )
 
 
+@final
+@attrs.define(frozen=True)
+class NpmjsVersionsSortedBySemver(SortedVersions):
+
+    _artifactory_domain: str
+    _package_name: str
+
+    def fetch(self) -> SortedVersionsList:
+        response = httpx.get(
+            httpx.URL(self._artifactory_domain).join(self._package_name),
+        )
+        response.raise_for_status()
+        versions = response.json()['time'].items()
+        correct_versions = []
+        for version_number, release_time in versions:
+            with suppress(version.InvalidVersion, IndexError, KeyError):
+                parsed_version = version.parse(version_number)
+                if not parsed_version.is_prerelease and not parsed_version.is_devrelease:
+                    parsed_release_time = datetime.datetime.strptime(
+                        release_time, '%Y-%m-%dT%H:%M:%S.%f%z',
+                    ).astimezone(datetime.timezone.utc).date()
+                    correct_versions.append({
+                        version_number: parsed_release_time,
+                    })
+        return sorted(
+            correct_versions,
+            key=lambda release_dict: version.parse(next(iter(release_dict.keys()))),
+        )
+
+
 @final
 @attrs.define(frozen=True)
 class OvertakingSafeVersionDelta(VersionDelta):
 
     _origin: VersionDelta
     _enable: bool
```

### Comparing `deltaver-0.2.1/pyproject.toml` & `deltaver-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "deltaver"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 packages = [
   {include = "deltaver"}
 ]
 authors = ["Almaz Ilaletdinov <a.ilaletdinov@yandex.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 attrs = "^23.0"
 httpx = "^0"
-packaging = "^23.2"
-typer = "^0.9"
+packaging = ">=23,<25"
+typer = "^0"
 rich = "^13.0"
-typing-extensions = "^4.9.0"
+typing-extensions = "^4.9"
 toml = "^0.10.2"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "8.0.0"
-respx = "0.20.2"
-time-machine = "2.13.0"
+pytest = "8.2.1"
+respx = "0.21.1"
+time-machine = "2.14.1"
 isort = "5.13.2"
-pytest-cov = "4.1.0"
-ruff = "0.2.1"
-mypy = "1.8.0"
-types-toml = "0.10.8.7"
+pytest-cov = "5.0.0"
+ruff = "0.4.5"
+mypy = "1.10.0"
+types-toml = "0.10.8.20240310"
 pytest-randomly = "3.15.0"
 
 [tool.poetry.scripts]
 deltaver = "deltaver.__main__:app"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `deltaver-0.2.1/PKG-INFO` & `deltaver-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: deltaver
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Almaz Ilaletdinov
 Author-email: a.ilaletdinov@yandex.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=23.0,<24.0)
 Requires-Dist: httpx (>=0,<1)
-Requires-Dist: packaging (>=23.2,<24.0)
+Requires-Dist: packaging (>=23,<25)
 Requires-Dist: rich (>=13.0,<14.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typer (>=0.9,<0.10)
-Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
+Requires-Dist: typer (>=0,<1)
+Requires-Dist: typing-extensions (>=4.9,<5.0)
 Description-Content-Type: text/markdown
 
 # Deltaver (Dependency Lag Calculator)
 
 ## Overview
 
 The "Deltaver" is a Python project designed to calculate the lag or delay in dependencies in terms of days. It provides insights into how outdated your project dependencies are, helping you stay up-to-date with the latest developments and security patches.
 
 ## Features:
 
- - **Dependency Lag Calculation**: The tool analyzes the timestamp of the current dependency version and compares it with the latest available version, providing the time lag in days.
- - **Security Insights**: Identify outdated dependencies to prioritize updates based on security considerations.
- - **Customization**: Configure the tool to focus on specific dependencies or categories, allowing for flexibility in analysis.
+- **Dependency Lag Calculation**: The tool analyzes the timestamp of the current dependency version and compares it with the latest available version, providing the time lag in days.
+- **Security Insights**: Identify outdated dependencies to prioritize updates based on security considerations.
+- **Customization**: Configure the tool to focus on specific dependencies or categories, allowing for flexibility in analysis.
 
 ## Getting Started
 ### Prerequisites
 
 Make sure you have the following installed:
 
- - Python 3.x
- - Pip (Python package installer)
+- Python 3.x
+- Pip (Python package installer)
 
 ### Installation
 
 ```bash
 pip install deltaver
 ```
```

