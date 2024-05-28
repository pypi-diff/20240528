# Comparing `tmp/sp_variant-3.5.0.tar.gz` & `tmp/sp_variant-3.5.1.tar.gz`

## Comparing `sp_variant-3.5.0.tar` & `sp_variant-3.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sp_variant-3.5.0/.editorconfig
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sp_variant-3.5.0/mkdocs.yml
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 sp_variant-3.5.0/tox.ini
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sp_variant-3.5.0/.reuse/dep5
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.5.0/LICENSES/BSD-2-Clause.txt
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/common/scripts/add-storpool-repo.sh
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/common/scripts/storpool_variant.sh
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/debian/repo/storpool-keyring.gpg
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/debian/repo/storpool.sources
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/redhat/repo/RPM-GPG-KEY-StorPool
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sp_variant-3.5.0/data/redhat/repo/storpool-centos.repo
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sp_variant-3.5.0/docs/api.md
--rw-r--r--   0        0        0    23414 2020-02-02 00:00:00.000000 sp_variant-3.5.0/docs/changes.md
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sp_variant-3.5.0/docs/index.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sp_variant-3.5.0/examples/build-repo-overrides.toml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/docs.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/ruff.txt
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/test-mypy.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/test-tox-stages.txt
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/test-unit.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/requirements/tools.txt
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/__init__.py
--rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/__main__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/diag.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/py.typed
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_build_repo/subst.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/__init__.py
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/__main__.py
--rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/defs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/py.typed
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/variant.py
--rw-r--r--   0        0        0    27505 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/vbuild.py
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/sp_variant/yaiparser.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/test_docker/__init__.py
--rw-r--r--   0        0        0    17971 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/test_docker/__main__.py
--rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/tests/vetox.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/__init__.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/test_subst.py
--rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/test_variant.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sp_variant-3.5.0/python/unit_tests/test_yaiparser.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sp_variant-3.5.0/.gitignore
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.5.0/README.md
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 sp_variant-3.5.0/pyproject.toml
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 sp_variant-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 sp_variant-3.5.1/.editorconfig
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sp_variant-3.5.1/mkdocs.yml
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 sp_variant-3.5.1/tox.ini
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 sp_variant-3.5.1/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 sp_variant-3.5.1/LICENSES/BSD-2-Clause.txt
+-rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 sp_variant-3.5.1/data/common/scripts/add-storpool-repo.sh
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 sp_variant-3.5.1/data/common/scripts/storpool_variant.sh
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sp_variant-3.5.1/data/debian/repo/storpool-keyring.gpg
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sp_variant-3.5.1/data/debian/repo/storpool.sources
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 sp_variant-3.5.1/data/redhat/repo/RPM-GPG-KEY-StorPool
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 sp_variant-3.5.1/data/redhat/repo/storpool-centos.repo
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 sp_variant-3.5.1/docs/api.md
+-rw-r--r--   0        0        0    23579 2020-02-02 00:00:00.000000 sp_variant-3.5.1/docs/changes.md
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sp_variant-3.5.1/docs/index.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sp_variant-3.5.1/examples/build-repo-overrides.toml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/requirements/docs.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/requirements/ruff.txt
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/requirements/test-mypy.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/requirements/test-tox-stages.txt
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/requirements/test-unit.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/requirements/tools.txt
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_build_repo/__init__.py
+-rw-r--r--   0        0        0    13209 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_build_repo/__main__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_build_repo/diag.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_build_repo/py.typed
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_build_repo/subst.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_variant/__init__.py
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_variant/__main__.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_variant/defs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_variant/py.typed
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_variant/variant.py
+-rw-r--r--   0        0        0    29470 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_variant/vbuild.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/sp_variant/yaiparser.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/test_docker/__init__.py
+-rw-r--r--   0        0        0    17971 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/test_docker/__main__.py
+-rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/tests/vetox.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/unit_tests/__init__.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/unit_tests/test_subst.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/unit_tests/test_variant.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 sp_variant-3.5.1/python/unit_tests/test_yaiparser.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sp_variant-3.5.1/.gitignore
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 sp_variant-3.5.1/README.md
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 sp_variant-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 sp_variant-3.5.1/PKG-INFO
```

### Comparing `sp_variant-3.5.0/.editorconfig` & `sp_variant-3.5.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/mkdocs.yml` & `sp_variant-3.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/tox.ini` & `sp_variant-3.5.1/tox.ini`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/LICENSES/BSD-2-Clause.txt` & `sp_variant-3.5.1/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/data/debian/repo/storpool-keyring.gpg` & `sp_variant-3.5.1/data/debian/repo/storpool-keyring.gpg`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/data/redhat/repo/RPM-GPG-KEY-StorPool` & `sp_variant-3.5.1/data/redhat/repo/RPM-GPG-KEY-StorPool`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/data/redhat/repo/storpool-centos.repo` & `sp_variant-3.5.1/data/redhat/repo/storpool-centos.repo`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/docs/changes.md` & `sp_variant-3.5.1/docs/changes.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 All notable changes to the sp-variant project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [3.5.1] - 2024-05-28
+
+### Additions
+
+- all:
+    - add support for Oracle 8
+
 ## [3.5.0] - 2024-04-03
 
 ### Semi-incompatible changes
 
 - use Python 3.x as `min_sys_python` everywhere
 - drop the definitions for CentOS 6, Debian 9, Ubuntu 16.04, and Ubuntu 23.04;
   they will no longer even be recognized
@@ -608,15 +615,16 @@
 
 ## [1.3.0] - 2021-09-15
 
 ### Started
 
 - First public release.
 
-[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.5.0...main
+[Unreleased]: https://github.com/storpool/sp-variant/compare/release/3.5.1...main
+[3.5.1]: https://github.com/storpool/sp-variant/compare/release/3.5.0...release/3.5.1
 [3.5.0]: https://github.com/storpool/sp-variant/compare/release/3.4.2...release/3.5.0
 [3.4.2]: https://github.com/storpool/sp-variant/compare/release/3.4.1...release/3.4.2
 [3.4.1]: https://github.com/storpool/sp-variant/compare/release/3.4.0...release/3.4.1
 [3.4.0]: https://github.com/storpool/sp-variant/compare/release/3.3.0...release/3.4.0
 [3.3.0]: https://github.com/storpool/sp-variant/compare/release/3.2.3...release/3.3.0
 [3.2.3]: https://github.com/storpool/sp-variant/compare/release/3.2.2...release/3.2.3
 [3.2.2]: https://github.com/storpool/sp-variant/compare/release/3.2.1...release/3.2.2
```

### Comparing `sp_variant-3.5.0/docs/index.md` & `sp_variant-3.5.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/sp_build_repo/__main__.py` & `sp_variant-3.5.1/python/sp_build_repo/__main__.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/sp_build_repo/diag.py` & `sp_variant-3.5.1/python/sp_build_repo/diag.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/sp_build_repo/subst.py` & `sp_variant-3.5.1/python/sp_build_repo/subst.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/sp_variant/__main__.py` & `sp_variant-3.5.1/python/sp_variant/__main__.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/sp_variant/defs.py` & `sp_variant-3.5.1/python/sp_variant/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     extension: str
     """The extension to be used in filenames for configurating the package manager."""
 
     url: str
     """The base URL of the StorPool package repository."""
 
 
-VERSION: Final = "3.5.0"
+VERSION: Final = "3.5.1"
 FORMAT_VERSION: Final = (1, 4)
 
 REPO_TYPES: Final = [
     RepoType(name="contrib", extension="", url="https://repo.storpool.com/public/"),
     RepoType(
         name="staging",
         extension="-staging",
```

### Comparing `sp_variant-3.5.0/python/sp_variant/variant.py` & `sp_variant-3.5.1/python/sp_variant/variant.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/sp_variant/vbuild.py` & `sp_variant-3.5.1/python/sp_variant/vbuild.py`

 * *Files 3% similar despite different names*

```diff
@@ -622,14 +622,75 @@
                 "alias": "oracle7",
                 "base_image": "IGNORE",
                 "branch": "",
             },
         },
     ),
     defs.VariantUpdate(
+        name="ORACLE8",
+        descr="Oracle Linux 8.x",
+        parent="ALMA8",
+        detect=defs.Detect(
+            filename="/etc/oracle-release",
+            regex=re.compile(
+                r"^ Oracle \s+ Linux \s+ Server \s+ release \s .* "
+                r"\s 8 \. (?: [4-9] | [1-9][0-9] )",
+                re.X,
+            ),
+            os_id="ol",
+            os_version_regex=re.compile(r"^8(?:$|\.[4-9]|\.[1-9][0-9])"),
+        ),
+        updates={
+            "commands": {
+                "package": {
+                    "install": [
+                        "dnf",
+                        "--disablerepo=*",
+                        "--enablerepo=ol8_appstream",
+                        "--enablerepo=ol8_baseos_latest",
+                        "--enablerepo=storpool-contrib",
+                        "install",
+                        "-q",
+                        "-y",
+                        "--",
+                    ],
+                },
+                "pkgfile": {
+                    "install": [
+                        "sh",
+                        "-c",
+                        """
+unset to_install to_reinstall
+for f in $packages; do
+    package="$(rpm -qp "$f")"
+    if rpm -q -- "$package"; then
+        to_reinstall="$to_reinstall ./$f"
+    else
+        to_install="$to_install ./$f"
+    fi
+done
+
+if [ -n "$to_install" ]; then
+    dnf install -y --disablerepo='*' --enablerepo=ol8_appstream,ol8_baseos_latest,storpool-contrib --setopt=localpkg_gpgcheck=0 -- $to_install
+fi
+if [ -n "$to_reinstall" ]; then
+    dnf reinstall -y --disablerepo='*' --enablerepo=ol8_appstream,ol8_baseos_latest,storpool-contrib --setopt=localpkg_gpgcheck=0 -- $to_reinstall
+fi
+""",  # noqa: E501
+                    ],
+                },
+            },
+            "builder": {
+                "alias": "oracle8",
+                "base_image": "oraclelinux:8",
+                "branch": "",
+            },
+        },
+    ),
+    defs.VariantUpdate(
         name="RHEL8",
         descr="RedHat Enterprise Linux 8.x",
         parent="CENTOS8",
         detect=defs.Detect(
             filename="/etc/redhat-release",
             regex=re.compile(
                 r"^ Red \s+ Hat \s+ Enterprise \s+ Linux \s .* "
```

### Comparing `sp_variant-3.5.0/python/sp_variant/yaiparser.py` & `sp_variant-3.5.1/python/sp_variant/yaiparser.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/test_docker/__main__.py` & `sp_variant-3.5.1/python/test_docker/__main__.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/tests/vetox.py` & `sp_variant-3.5.1/python/tests/vetox.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/unit_tests/test_subst.py` & `sp_variant-3.5.1/python/unit_tests/test_subst.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/unit_tests/test_variant.py` & `sp_variant-3.5.1/python/unit_tests/test_variant.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/python/unit_tests/test_yaiparser.py` & `sp_variant-3.5.1/python/unit_tests/test_yaiparser.py`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/README.md` & `sp_variant-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/pyproject.toml` & `sp_variant-3.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sp_variant-3.5.0/PKG-INFO` & `sp_variant-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sp-variant
-Version: 3.5.0
+Version: 3.5.1
 Summary: Detect the Linux distribution for the StorPool build system
 Project-URL: Homepage, https://repo.storpool.com/public/doc/sp-variant/
 Project-URL: Changelog, https://github.com/storpool/sp-variant/blob/main/docs/changes.md
 Project-URL: Source Code, https://github.com/storpool/sp-variant
 Author-email: StorPool <support@storpool.com>
 License: BSD-2-Clause
 Classifier: Development Status :: 5 - Production/Stable
```

