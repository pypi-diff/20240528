# Comparing `tmp/rina_pp_pyb-1.0.0.tar.gz` & `tmp/rina_pp_pyb-1.0.1.tar.gz`

## Comparing `rina_pp_pyb-1.0.0.tar` & `rina_pp_pyb-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 rina_pp_pyb-1.0.0/Cargo.toml
--rw-r--r--   0     1001      127     3748 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      686 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/.gitignore
--rw-r--r--   0     1001      127     1060 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/LICENSE
--rw-r--r--   0     1001      127     5801 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/README.md
--rw-r--r--   0     1001      127    29489 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/rina_pp_pyb.pyi
--rw-r--r--   0     1001      127     7873 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/attributes/beatmap.rs
--rw-r--r--   0     1001      127     8228 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/attributes/difficulty.rs
--rw-r--r--   0     1001      127       58 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/attributes/mod.rs
--rw-r--r--   0     1001      127     3152 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/attributes/performance.rs
--rw-r--r--   0     1001      127     5272 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/beatmap.rs
--rw-r--r--   0     1001      127     8261 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/difficulty.rs
--rw-r--r--   0     1001      127      228 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/error.rs
--rw-r--r--   0     1001      127     1006 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/gradual/difficulty.rs
--rw-r--r--   0     1001      127       41 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/gradual/mod.rs
--rw-r--r--   0     1001      127      940 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/gradual/performance.rs
--rw-r--r--   0     1001      127     1575 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/lib.rs
--rw-r--r--   0     1001      127     2407 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/macros.rs
--rw-r--r--   0     1001      127      975 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/mode.rs
--rw-r--r--   0     1001      127    13895 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/performance.rs
--rw-r--r--   0     1001      127     4291 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/score_state.rs
--rw-r--r--   0     1001      127     2646 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/src/strains.rs
--rw-r--r--   0     1001      127    48913 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/Cargo.lock
--rw-r--r--   0     1001      127      778 2024-04-29 17:28:09.000000 rina_pp_pyb-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6566 1970-01-01 00:00:00.000000 rina_pp_pyb-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 rina_pp_pyb-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      127     3748 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      686 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/.gitignore
+-rw-r--r--   0     1001      127     1060 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/LICENSE
+-rw-r--r--   0     1001      127     5801 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/README.md
+-rw-r--r--   0     1001      127    29489 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/rina_pp_pyb.pyi
+-rw-r--r--   0     1001      127     7873 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/attributes/beatmap.rs
+-rw-r--r--   0     1001      127     8228 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/attributes/difficulty.rs
+-rw-r--r--   0     1001      127       58 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/attributes/mod.rs
+-rw-r--r--   0     1001      127     3152 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/attributes/performance.rs
+-rw-r--r--   0     1001      127     5272 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/beatmap.rs
+-rw-r--r--   0     1001      127     8261 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/difficulty.rs
+-rw-r--r--   0     1001      127      228 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/error.rs
+-rw-r--r--   0     1001      127     1006 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/gradual/difficulty.rs
+-rw-r--r--   0     1001      127       41 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/gradual/mod.rs
+-rw-r--r--   0     1001      127      940 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/gradual/performance.rs
+-rw-r--r--   0     1001      127     1575 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      127     2407 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/macros.rs
+-rw-r--r--   0     1001      127      975 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/mode.rs
+-rw-r--r--   0     1001      127    13895 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/performance.rs
+-rw-r--r--   0     1001      127     4291 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/score_state.rs
+-rw-r--r--   0     1001      127     2646 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/src/strains.rs
+-rw-r--r--   0     1001      127    10571 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/Cargo.lock
+-rw-r--r--   0     1001      127      778 2024-05-28 13:45:06.000000 rina_pp_pyb-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6566 1970-01-01 00:00:00.000000 rina_pp_pyb-1.0.1/PKG-INFO
```

### Comparing `rina_pp_pyb-1.0.0/Cargo.toml` & `rina_pp_pyb-1.0.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "rina-pp-pyb"
-version = "1.0.0"
+version = "1.0.1"
 edition = "2021"
 authors = ["Max Ohn <ohn.m@hotmail.de>", "Simon G."]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/osuthailand/rina-pp-pyb"
 description = "Difficulty and performance calculation for osu!"
 
 [lib]
 name = "rina_pp_pyb"
 crate-type = ["cdylib"]
 
 [dependencies]
 pyo3 = { version = "0.21", features = ["extension-module", "macros"] }
-rina-pp = { version = "0.9.24", git = "https://github.com/osuthailand/rina-pp-sys", features = ["sync"] }
+rina-pp = { version = "0.9.25", git = "https://github.com/osuthailand/rina-pp-sys", features = ["sync"] }
 openssl = { version = "0.10.40", features = ["vendored"] }
 
 [profile.release]
 lto = true
 panic = "abort"
 codegen-units = 1
 strip = true
```

### Comparing `rina_pp_pyb-1.0.0/.github/workflows/ci.yml` & `rina_pp_pyb-1.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/.gitignore` & `rina_pp_pyb-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/LICENSE` & `rina_pp_pyb-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/README.md` & `rina_pp_pyb-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/rina_pp_pyb.pyi` & `rina_pp_pyb-1.0.1/rina_pp_pyb.pyi`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/attributes/beatmap.rs` & `rina_pp_pyb-1.0.1/src/attributes/beatmap.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/attributes/difficulty.rs` & `rina_pp_pyb-1.0.1/src/attributes/difficulty.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/attributes/performance.rs` & `rina_pp_pyb-1.0.1/src/attributes/performance.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/beatmap.rs` & `rina_pp_pyb-1.0.1/src/beatmap.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/difficulty.rs` & `rina_pp_pyb-1.0.1/src/difficulty.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/gradual/difficulty.rs` & `rina_pp_pyb-1.0.1/src/gradual/difficulty.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/gradual/performance.rs` & `rina_pp_pyb-1.0.1/src/gradual/performance.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/lib.rs` & `rina_pp_pyb-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/macros.rs` & `rina_pp_pyb-1.0.1/src/macros.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/mode.rs` & `rina_pp_pyb-1.0.1/src/mode.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/performance.rs` & `rina_pp_pyb-1.0.1/src/performance.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/score_state.rs` & `rina_pp_pyb-1.0.1/src/score_state.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/src/strains.rs` & `rina_pp_pyb-1.0.1/src/strains.rs`

 * *Files identical despite different names*

### Comparing `rina_pp_pyb-1.0.0/pyproject.toml` & `rina_pp_pyb-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [project]
 name = "rina-pp-pyb"
-version = "1.0.0"
+version = "1.0.1"
 requires-python = ">=3.7"
 description = "Difficulty and performance calculation for osu!"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Rust",
```

### Comparing `rina_pp_pyb-1.0.0/PKG-INFO` & `rina_pp_pyb-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rina-pp-pyb
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
```

