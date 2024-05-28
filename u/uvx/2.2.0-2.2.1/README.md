# Comparing `tmp/uvx-2.2.0.tar.gz` & `tmp/uvx-2.2.1.tar.gz`

## Comparing `uvx-2.2.0.tar` & `uvx-2.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 uvx-2.2.0/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.2.0/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.2.0/.gitignore
--rw-rw-r--   0     1000     1000     1947 2024-05-28 09:55:59.000000 uvx-2.2.0/CHANGELOG.md
--rw-rw-r--   0     1000     1000    94917 2024-05-28 09:56:50.000000 uvx-2.2.0/Cargo.lock
--rw-rw-r--   0     1000     1000     2456 2024-05-15 08:49:40.000000 uvx-2.2.0/README.md
--rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.2.0/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.2.0/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-05-10 16:04:44.000000 uvx-2.2.0/src/animate.rs
--rw-rw-r--   0     1000     1000    12070 2024-05-28 09:54:13.000000 uvx-2.2.0/src/cli.rs
--rw-rw-r--   0     1000     1000     3194 2024-05-14 19:37:08.000000 uvx-2.2.0/src/cmd.rs
--rw-rw-r--   0     1000     1000     1346 2024-05-15 07:59:15.000000 uvx-2.2.0/src/commands/activate.rs
--rw-rw-r--   0     1000     1000     3751 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/changelog.rs
--rw-rw-r--   0     1000     1000      899 2024-05-14 19:03:10.000000 uvx-2.2.0/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     1156 2024-05-15 09:17:21.000000 uvx-2.2.0/src/commands/create.rs
--rw-rw-r--   0     1000     1000     2462 2024-05-14 19:10:06.000000 uvx-2.2.0/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1680 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5112 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/install.rs
--rw-rw-r--   0     1000     1000     3026 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/list.rs
--rw-rw-r--   0     1000     1000      377 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2560 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1414 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.2.0/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.2.0/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.2.0/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.2.0/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.2.0/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     3763 2024-05-15 08:51:29.000000 uvx-2.2.0/src/commands/setup.rs
--rw-rw-r--   0     1000     1000     1675 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2061 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000     1016 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4245 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1089 2024-05-28 09:54:13.000000 uvx-2.2.0/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.2.0/src/helpers.rs
--rw-rw-r--   0     1000     1000     1999 2024-05-28 09:54:13.000000 uvx-2.2.0/src/main.rs
--rw-rw-r--   0     1000     1000    12905 2024-05-28 09:54:13.000000 uvx-2.2.0/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.2.0/src/pip.rs
--rw-rw-r--   0     1000     1000     3031 2024-05-28 09:54:13.000000 uvx-2.2.0/src/pypi.rs
--rw-rw-r--   0     1000     1000      487 2024-05-13 18:28:56.000000 uvx-2.2.0/src/shell/activate.sh
--rw-rw-r--   0     1000     1000     3722 2024-04-29 13:40:53.000000 uvx-2.2.0/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.2.0/src/uv.rs
--rw-rw-r--   0     1000     1000     2819 2024-05-15 08:51:43.000000 uvx-2.2.0/src/venv.rs
--rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 uvx-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 uvx-2.2.1/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.2.1/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.2.1/.gitignore
+-rw-rw-r--   0     1000     1000     2034 2024-05-28 10:49:08.000000 uvx-2.2.1/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    91955 2024-05-28 10:48:34.000000 uvx-2.2.1/Cargo.lock
+-rw-rw-r--   0     1000     1000     2456 2024-05-15 08:49:40.000000 uvx-2.2.1/README.md
+-rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.2.1/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.2.1/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-05-10 16:04:44.000000 uvx-2.2.1/src/animate.rs
+-rw-rw-r--   0     1000     1000    12070 2024-05-28 09:54:13.000000 uvx-2.2.1/src/cli.rs
+-rw-rw-r--   0     1000     1000     3194 2024-05-14 19:37:08.000000 uvx-2.2.1/src/cmd.rs
+-rw-rw-r--   0     1000     1000     1346 2024-05-15 07:59:15.000000 uvx-2.2.1/src/commands/activate.rs
+-rw-rw-r--   0     1000     1000     3751 2024-05-28 10:40:03.000000 uvx-2.2.1/src/commands/changelog.rs
+-rw-rw-r--   0     1000     1000      899 2024-05-14 19:03:10.000000 uvx-2.2.1/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     1156 2024-05-15 09:17:21.000000 uvx-2.2.1/src/commands/create.rs
+-rw-rw-r--   0     1000     1000     2462 2024-05-14 19:10:06.000000 uvx-2.2.1/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1680 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5112 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     3026 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      377 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2560 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1414 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.2.1/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.2.1/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.2.1/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.2.1/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.2.1/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     3763 2024-05-15 08:51:29.000000 uvx-2.2.1/src/commands/setup.rs
+-rw-rw-r--   0     1000     1000     1675 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2061 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000     1016 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4245 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1089 2024-05-28 09:54:13.000000 uvx-2.2.1/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.2.1/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1999 2024-05-28 09:54:13.000000 uvx-2.2.1/src/main.rs
+-rw-rw-r--   0     1000     1000    12905 2024-05-28 10:25:06.000000 uvx-2.2.1/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.2.1/src/pip.rs
+-rw-rw-r--   0     1000     1000     3154 2024-05-28 10:43:55.000000 uvx-2.2.1/src/pypi.rs
+-rw-rw-r--   0     1000     1000      487 2024-05-13 18:28:56.000000 uvx-2.2.1/src/shell/activate.sh
+-rw-rw-r--   0     1000     1000     3722 2024-04-29 13:40:53.000000 uvx-2.2.1/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.2.1/src/uv.rs
+-rw-rw-r--   0     1000     1000     2819 2024-05-15 08:51:43.000000 uvx-2.2.1/src/venv.rs
+-rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 uvx-2.2.1/PKG-INFO
```

### Comparing `uvx-2.2.0/Cargo.toml` & `uvx-2.2.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uvx"
-version = "2.2.0"
+version = "2.2.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
 
@@ -26,15 +26,15 @@
 home = "0.5.9" # ~ resolving
 directories = "5.0.1"
 itertools = "0.13.0" # more .iter magic
 configparser = "3.0.4"
 tempfile = "3.10.1"
 chrono = "0.4.38"
 subprocess = "0.2.9"
-reqwest = "0.12.4"
+reqwest = { version = "0.12.4", default-features = false, features = ["json", "gzip", "brotli", "stream", "rustls-tls", "rustls-tls-native-roots"] }
 regex = "1.10.4"
 
 # fancy
 anstyle = "1.0.7" # color styling for clap
 owo-colors = "4.0.0" # color styling for strings
 
 # uv
```

### Comparing `uvx-2.2.0/.gitignore` & `uvx-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/CHANGELOG.md` & `uvx-2.2.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.2.1 (2024-05-28)
+
+### Fix
+
+* `uvx list` was slow due to incorrect SSL behavior.
+
 ## v2.2.0 (2024-05-28)
 
 ### Features
 * Added the `self` subcommand namespace
   * `uvx self update` to self-update
   * `uvx self changelog` to see the changelog of uvx
 * Look for available updates on `uvx list`
```

### Comparing `uvx-2.2.0/Cargo.lock` & `uvx-2.2.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -899,29 +899,14 @@
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
-name = "foreign-types"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
-dependencies = [
- "foreign-types-shared",
-]
-
-[[package]]
-name = "foreign-types-shared"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
-
-[[package]]
 name = "form_urlencoded"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
@@ -1120,33 +1105,14 @@
  "bstr",
  "log",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
-name = "h2"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "816ec7294445779408f36fe57bc5b7fc1cf59664059096c65f905c1c61f58069"
-dependencies = [
- "bytes",
- "fnv",
- "futures-core",
- "futures-sink",
- "futures-util",
- "http",
- "indexmap",
- "slab",
- "tokio",
- "tokio-util",
- "tracing",
-]
-
-[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
  "ahash",
 ]
@@ -1253,15 +1219,14 @@
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
- "h2",
  "http",
  "http-body",
  "httparse",
  "itoa",
  "pin-project-lite",
  "smallvec",
  "tokio",
@@ -1282,30 +1247,14 @@
  "rustls-pki-types",
  "tokio",
  "tokio-rustls",
  "tower-service",
 ]
 
 [[package]]
-name = "hyper-tls"
-version = "0.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70206fc6890eaca9fde8a0bf71caa2ddfc9fe045ac9e5c70df101a7dbde866e0"
-dependencies = [
- "bytes",
- "http-body-util",
- "hyper",
- "hyper-util",
- "native-tls",
- "tokio",
- "tokio-native-tls",
- "tower-service",
-]
-
-[[package]]
 name = "hyper-util"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
 dependencies = [
  "bytes",
  "futures-channel",
@@ -1672,32 +1621,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3ffa00dec017b5b1a8b7cf5e2c008bfda1aa7e0697ac1508b491fdf2622fb4d8"
 dependencies = [
  "rand",
 ]
 
 [[package]]
-name = "native-tls"
-version = "0.2.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
-dependencies = [
- "lazy_static",
- "libc",
- "log",
- "openssl",
- "openssl-probe",
- "openssl-sys",
- "schannel",
- "security-framework",
- "security-framework-sys",
- "tempfile",
-]
-
-[[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
@@ -1744,40 +1675,14 @@
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
-name = "openssl"
-version = "0.10.64"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
-dependencies = [
- "bitflags 2.5.0",
- "cfg-if",
- "foreign-types",
- "libc",
- "once_cell",
- "openssl-macros",
- "openssl-sys",
-]
-
-[[package]]
-name = "openssl-macros"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.58",
-]
-
-[[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
@@ -2237,45 +2142,39 @@
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "async-compression",
  "base64 0.22.0",
  "bytes",
- "encoding_rs",
  "futures-channel",
  "futures-core",
  "futures-util",
- "h2",
  "http",
  "http-body",
  "http-body-util",
  "hyper",
  "hyper-rustls",
- "hyper-tls",
  "hyper-util",
  "ipnet",
  "js-sys",
  "log",
  "mime",
- "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
  "rustls 0.22.4",
  "rustls-native-certs",
  "rustls-pemfile",
  "rustls-pki-types",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
- "system-configuration",
  "tokio",
- "tokio-native-tls",
  "tokio-rustls",
  "tokio-util",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wasm-streams",
@@ -2750,35 +2649,14 @@
 checksum = "0b3a0d0aba8bf96a0e1ddfdc352fc53b3df7f39318c71854910c3c4b024ae52c"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
-name = "system-configuration"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
-dependencies = [
- "bitflags 1.3.2",
- "core-foundation",
- "system-configuration-sys",
-]
-
-[[package]]
-name = "system-configuration-sys"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "tempfile"
@@ -2859,24 +2737,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
-name = "tokio-native-tls"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
-dependencies = [
- "native-tls",
- "tokio",
-]
-
-[[package]]
 name = "tokio-rustls"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
 dependencies = [
  "rustls 0.22.4",
  "rustls-pki-types",
@@ -3441,15 +3309,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.2.0"
+version = "2.2.1"
 dependencies = [
  "anstyle",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
  "directories",
```

### Comparing `uvx-2.2.0/README.md` & `uvx-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/animate.rs` & `uvx-2.2.1/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/cli.rs` & `uvx-2.2.1/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/cmd.rs` & `uvx-2.2.1/src/cmd.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/activate.rs` & `uvx-2.2.1/src/commands/activate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/changelog.rs` & `uvx-2.2.1/src/commands/changelog.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/completions.rs` & `uvx-2.2.1/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/create.rs` & `uvx-2.2.1/src/commands/create.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/ensurepath.rs` & `uvx-2.2.1/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/inject.rs` & `uvx-2.2.1/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/install.rs` & `uvx-2.2.1/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/list.rs` & `uvx-2.2.1/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/reinstall.rs` & `uvx-2.2.1/src/commands/reinstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/reinstall_all.rs` & `uvx-2.2.1/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/run.rs` & `uvx-2.2.1/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/runpip.rs` & `uvx-2.2.1/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/runpython.rs` & `uvx-2.2.1/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/runuv.rs` & `uvx-2.2.1/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/self_update.rs` & `uvx-2.2.1/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/setup.rs` & `uvx-2.2.1/src/commands/setup.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/uninject.rs` & `uvx-2.2.1/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/uninstall.rs` & `uvx-2.2.1/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/uninstall_all.rs` & `uvx-2.2.1/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/upgrade.rs` & `uvx-2.2.1/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/commands/upgrade_all.rs` & `uvx-2.2.1/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/helpers.rs` & `uvx-2.2.1/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/main.rs` & `uvx-2.2.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/metadata.rs` & `uvx-2.2.1/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/pip.rs` & `uvx-2.2.1/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/pypi.rs` & `uvx-2.2.1/src/pypi.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use pep440_rs::{Version, VersionSpecifier};
 use pep508_rs::{PackageName, Requirement};
 use rkyv::{de::deserializers::SharedDeserializeMap, Deserialize};
-use uv_client::{RegistryClient, RegistryClientBuilder, SimpleMetadatum};
+use uv_client::{
+    RegistryClient, RegistryClientBuilder, SimpleMetadatum,
+};
 
 use crate::pip::parse_requirement;
 use crate::uv::uv_cache;
 
 pub async fn get_client() -> Option<RegistryClient> {
     let cache = uv_cache()?;
 
@@ -32,16 +34,20 @@
 ) -> Vec<Version> {
     let mut versions: Vec<Version> = vec![];
 
     let Some(client) = get_client().await else {
         return versions;
     };
 
-    let Ok(data) = client.simple(package_name).await else {
-        return versions;
+    let data = match client.simple(package_name).await {
+        Err(err) => {
+            eprintln!("Something went wrong: {}", err);
+            return versions;
+        },
+        Ok(data) => data,
     };
 
     if let Some((_, metadata)) = data.iter().next_back() {
         versions = metadata
             .iter()
             .filter_map(|metadatum| deserialize_version(&metadatum.version))
             .collect();
```

### Comparing `uvx-2.2.0/src/symlinks.rs` & `uvx-2.2.1/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/uv.rs` & `uvx-2.2.1/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/src/venv.rs` & `uvx-2.2.1/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/pyproject.toml` & `uvx-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.2.0/PKG-INFO` & `uvx-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.2.0
+Version: 2.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
```

