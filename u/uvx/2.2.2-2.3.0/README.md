# Comparing `tmp/uvx-2.2.2.tar.gz` & `tmp/uvx-2.3.0.tar.gz`

## Comparing `uvx-2.2.2.tar` & `uvx-2.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 uvx-2.2.2/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.2.2/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.2.2/.gitignore
--rw-rw-r--   0     1000     1000     2115 2024-05-28 11:30:53.000000 uvx-2.2.2/CHANGELOG.md
--rw-rw-r--   0     1000     1000    91955 2024-05-28 11:30:27.000000 uvx-2.2.2/Cargo.lock
--rw-rw-r--   0     1000     1000     2456 2024-05-15 08:49:40.000000 uvx-2.2.2/README.md
--rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.2.2/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.2.2/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-05-10 16:04:44.000000 uvx-2.2.2/src/animate.rs
--rw-rw-r--   0     1000     1000    12070 2024-05-28 09:54:13.000000 uvx-2.2.2/src/cli.rs
--rw-rw-r--   0     1000     1000     3194 2024-05-14 19:37:08.000000 uvx-2.2.2/src/cmd.rs
--rw-rw-r--   0     1000     1000     1346 2024-05-15 07:59:15.000000 uvx-2.2.2/src/commands/activate.rs
--rw-rw-r--   0     1000     1000     3751 2024-05-28 11:03:35.000000 uvx-2.2.2/src/commands/changelog.rs
--rw-rw-r--   0     1000     1000      899 2024-05-14 19:03:10.000000 uvx-2.2.2/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     1156 2024-05-15 09:17:21.000000 uvx-2.2.2/src/commands/create.rs
--rw-rw-r--   0     1000     1000     2462 2024-05-14 19:10:06.000000 uvx-2.2.2/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1680 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5112 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/install.rs
--rw-rw-r--   0     1000     1000     3026 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/list.rs
--rw-rw-r--   0     1000     1000      377 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2560 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1414 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.2.2/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.2.2/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.2.2/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.2.2/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.2.2/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     3763 2024-05-15 08:51:29.000000 uvx-2.2.2/src/commands/setup.rs
--rw-rw-r--   0     1000     1000     1675 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2061 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000     1016 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4188 2024-05-28 11:28:44.000000 uvx-2.2.2/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1089 2024-05-28 09:54:13.000000 uvx-2.2.2/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.2.2/src/helpers.rs
--rw-rw-r--   0     1000     1000     1999 2024-05-28 09:54:13.000000 uvx-2.2.2/src/main.rs
--rw-rw-r--   0     1000     1000    12905 2024-05-28 10:25:06.000000 uvx-2.2.2/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.2.2/src/pip.rs
--rw-rw-r--   0     1000     1000     3154 2024-05-28 10:43:55.000000 uvx-2.2.2/src/pypi.rs
--rw-rw-r--   0     1000     1000      487 2024-05-13 18:28:56.000000 uvx-2.2.2/src/shell/activate.sh
--rw-rw-r--   0     1000     1000     3722 2024-04-29 13:40:53.000000 uvx-2.2.2/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.2.2/src/uv.rs
--rw-rw-r--   0     1000     1000     2819 2024-05-15 08:51:43.000000 uvx-2.2.2/src/venv.rs
--rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 uvx-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 uvx-2.3.0/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.3.0/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.3.0/.gitignore
+-rw-rw-r--   0     1000     1000     2312 2024-05-28 15:59:54.000000 uvx-2.3.0/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    91955 2024-05-28 15:59:01.000000 uvx-2.3.0/Cargo.lock
+-rw-rw-r--   0     1000     1000     2456 2024-05-15 08:49:40.000000 uvx-2.3.0/README.md
+-rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.3.0/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.3.0/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1805 2024-05-28 15:27:09.000000 uvx-2.3.0/src/animate.rs
+-rw-rw-r--   0     1000     1000    12927 2024-05-28 15:26:22.000000 uvx-2.3.0/src/cli.rs
+-rw-rw-r--   0     1000     1000     3177 2024-05-28 15:22:30.000000 uvx-2.3.0/src/cmd.rs
+-rw-rw-r--   0     1000     1000     1346 2024-05-15 07:59:15.000000 uvx-2.3.0/src/commands/activate.rs
+-rw-rw-r--   0     1000     1000     3765 2024-05-28 15:21:04.000000 uvx-2.3.0/src/commands/changelog.rs
+-rw-rw-r--   0     1000     1000     3634 2024-05-28 15:37:31.000000 uvx-2.3.0/src/commands/check.rs
+-rw-rw-r--   0     1000     1000      897 2024-05-28 15:21:21.000000 uvx-2.3.0/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     1154 2024-05-28 15:21:12.000000 uvx-2.3.0/src/commands/create.rs
+-rw-rw-r--   0     1000     1000     2519 2024-05-28 15:13:17.000000 uvx-2.3.0/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1681 2024-05-28 15:10:13.000000 uvx-2.3.0/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5108 2024-05-28 15:09:27.000000 uvx-2.3.0/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2673 2024-05-28 15:08:04.000000 uvx-2.3.0/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      388 2024-05-28 13:58:35.000000 uvx-2.3.0/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2558 2024-05-28 15:05:56.000000 uvx-2.3.0/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1414 2024-05-28 15:05:34.000000 uvx-2.3.0/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4031 2024-05-28 15:05:14.000000 uvx-2.3.0/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.3.0/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1227 2024-05-28 15:19:42.000000 uvx-2.3.0/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.3.0/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     3238 2024-05-28 14:57:28.000000 uvx-2.3.0/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     3793 2024-05-28 14:47:03.000000 uvx-2.3.0/src/commands/setup.rs
+-rw-rw-r--   0     1000     1000     1674 2024-05-28 14:44:42.000000 uvx-2.3.0/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2069 2024-05-28 14:44:00.000000 uvx-2.3.0/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000     1016 2024-05-28 14:42:57.000000 uvx-2.3.0/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4167 2024-05-28 14:42:29.000000 uvx-2.3.0/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1089 2024-05-28 14:41:07.000000 uvx-2.3.0/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.3.0/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1934 2024-05-28 14:08:13.000000 uvx-2.3.0/src/main.rs
+-rw-rw-r--   0     1000     1000    13211 2024-05-28 14:56:01.000000 uvx-2.3.0/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4372 2024-05-28 14:27:42.000000 uvx-2.3.0/src/pip.rs
+-rw-rw-r--   0     1000     1000     3128 2024-05-28 14:26:39.000000 uvx-2.3.0/src/pypi.rs
+-rw-rw-r--   0     1000     1000      487 2024-05-13 18:28:56.000000 uvx-2.3.0/src/shell/activate.sh
+-rw-rw-r--   0     1000     1000     3691 2024-05-28 14:26:22.000000 uvx-2.3.0/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3735 2024-05-28 14:24:57.000000 uvx-2.3.0/src/uv.rs
+-rw-rw-r--   0     1000     1000     2806 2024-05-28 14:10:08.000000 uvx-2.3.0/src/venv.rs
+-rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 uvx-2.3.0/PKG-INFO
```

### Comparing `uvx-2.2.2/.gitignore` & `uvx-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.2.2/CHANGELOG.md` & `uvx-2.3.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.3.0 (2024-05-28)
+
+### Feature
+
+* `uvx check` to perform checks (like uvx list does) and report any problems.
+
+### Refactoring
+
+* improved Rust-esque codestyle (according to Clippy)
+
 ## v2.2.2 (2024-05-28)
 
 ### Fix
 
 * `uvx upgrade` stored version metadata wrong
 
-
 ## v2.2.1 (2024-05-28)
 
 ### Fix
 
 * `uvx list` was slow due to incorrect SSL behavior.
 
 ## v2.2.0 (2024-05-28)
 
 ### Features
+
 * Added the `self` subcommand namespace
-  * `uvx self update` to self-update
-  * `uvx self changelog` to see the changelog of uvx
+    * `uvx self update` to self-update
+    * `uvx self changelog` to see the changelog of uvx
 * Look for available updates on `uvx list`
-  * Includes `--skip-updates`, `--show-prereleases`, `--ignore-constraints` as options
+    * Includes `--skip-updates`, `--show-prereleases`, `--ignore-constraints` as options
 
 ### BREAKING CHANGE
+
 * `uvx self-update` is now `uvx self update`
 
 ## v2.1.0 (2024-05-15)
 
 ### Features
 
 * Introduced the `uvx activate` command, enabling venv activation via bash function.
-* Added `uvx setup`, allowing which handles installation of bash integration features (like `uvx activate` and tab completion).
+* Added `uvx setup`, allowing which handles installation of bash integration features (like `uvx activate` and tab
+  completion).
 * Added `uvx create` to create new (empty) virtualenvs without installing from a package.
 
 ### Fixes
 
 * Enhanced shell compatibility by displaying a warning for unsupported shells during activation and hinting at the
   necessity of running `uvx setup` (and others).
```

### Comparing `uvx-2.2.2/Cargo.lock` & `uvx-2.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3309,15 +3309,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.2.2"
+version = "2.3.0"
 dependencies = [
  "anstyle",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
  "directories",
```

### Comparing `uvx-2.2.2/README.md` & `uvx-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.2.2/src/animate.rs` & `uvx-2.3.0/src/animate.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 pub struct AnimationSettings {
     pub style: AnimationStyle,
     pub order: AnimationOrder,
 }
 
 impl AnimationSettings {
-    pub fn default() -> AnimationSettings {
-        AnimationSettings {
+    pub const fn default() -> Self {
+        Self {
             style: AnimationStyle::Modern,
             order: AnimationOrder::Before,
         }
     }
 }
 
 fn get_spinner_chars(style: &AnimationStyle) -> Vec<char> {
@@ -39,18 +39,18 @@
 }
 
 pub async fn animation(
     message: String,
     style: AnimationSettings,
 ) {
     let spinner_chars = get_spinner_chars(&style.style);
-    let _order = &style.order;
+    let ordering = &style.order;
     let mut idx = 0;
     loop {
-        match &_order {
+        match &ordering {
             AnimationOrder::Before => {
                 eprint!("\r{} {} ", &spinner_chars[idx], &message);
             },
             AnimationOrder::After => {
                 eprint!("\r{} {} ", &message, &spinner_chars[idx]);
             },
         };
```

### Comparing `uvx-2.2.2/src/cli.rs` & `uvx-2.3.0/src/cli.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use clap::{Parser, Subcommand};
 use clap_complete::Shell;
 
-pub fn get_styles() -> clap::builder::Styles {
+pub const fn get_styles() -> clap::builder::Styles {
     clap::builder::Styles::styled()
         .usage(
             anstyle::Style::new()
                 .bold()
                 .underline()
                 .fg_color(Some(anstyle::Color::Ansi(anstyle::AnsiColor::Yellow))),
         )
@@ -259,14 +259,31 @@
 #[derive(Debug, Parser)]
 pub struct UnInjectOptions {
     pub outof: String,
     pub package_specs: Vec<String>,
 }
 
 #[derive(Debug, Parser)]
+pub struct CheckOptions {
+    #[clap(long, help = "Don't check if scripts are installed correctly.")]
+    pub skip_scripts: bool,
+    #[clap(long, help = "Don't check for updates", conflicts_with_all = ["show_prereleases", "ignore_constraints"])]
+    pub skip_updates: bool,
+    #[clap(long, help = "Show prerelease updates", conflicts_with_all = ["skip_updates"])]
+    pub show_prereleases: bool,
+    #[clap(long, help="Ignore version constraints when checking updates", conflicts_with_all = ["skip_updates"])]
+    pub ignore_constraints: bool,
+
+    #[clap(long, short, help = "Output as JSON")]
+    pub json: bool,
+
+    pub venv_names: Vec<String>,
+}
+
+#[derive(Debug, Parser)]
 pub struct CompletionsOptions {
     #[clap(long, short, help = "Add to ~/.bashrc")]
     pub install: bool,
     // todo: support others than bash
 }
 
 #[derive(Subcommand, Debug)]
@@ -295,14 +312,17 @@
     Reinstall(ReinstallOptions),
     #[clap(about = "Reinstall all uvx-installed packages.")]
     ReinstallAll(ReinstallAllOptions),
     #[clap(about = "Install additional packages to a virtual environment managed by uvx.")]
     Inject(InjectOptions),
     #[clap(aliases = &["eject"], about="Uninstall additional packages from a virtual environment managed by uvx. (alias: `eject`)")]
     Uninject(UnInjectOptions),
+    #[clap(about = "Check for possible issues and updates.")]
+    Check(CheckOptions),
+
     #[clap(about = "Run a package in a temporary virtual environment.")]
     Run(RunOptions),
     #[clap(about = "Run 'uv' in the right venv.")]
     Runuv(RunuvOptions),
     #[clap(about = "Run 'pip' in the right venv.")]
     Runpip(RunpipOptions),
     #[clap(about = "Run 'python' in the right venv.")]
@@ -314,37 +334,43 @@
     #[clap(about = "Use --install to install the autocomplete script (bash).")]
     Completions(CompletionsOptions),
 
     #[clap(subcommand, about = "Manage uvx itself.")]
     Self_(SelfCommands),
 }
 
+// todo `uvx check`:
+//   - show missing metadata
+//   - show packages with updates
+//   - show packages with script issues
+
 impl Process for Commands {
     async fn process(self) -> Result<i32, String> {
         match self {
-            Commands::List(opts) => opts.process().await,
-            Commands::Install(opts) => opts.process().await,
-            Commands::Upgrade(opts) => opts.process().await,
-            Commands::Uninstall(opts) => opts.process().await,
-            Commands::Reinstall(opts) => opts.process().await,
-            Commands::Inject(opts) => opts.process().await,
-            Commands::Activate(opts) => opts.process().await,
-            Commands::UpgradeAll(opts) => opts.process().await,
-            Commands::Runuv(opts) => opts.process().await,
-            Commands::Runpip(opts) => opts.process().await,
-            Commands::Runpython(opts) => opts.process().await,
-            Commands::Ensurepath(opts) => opts.process().await,
-            Commands::UninstallAll(opts) => opts.process().await,
-            Commands::ReinstallAll(opts) => opts.process().await,
-            Commands::Uninject(opts) => opts.process().await,
-            Commands::Completions(opts) => opts.process().await,
-            Commands::Run(opts) => opts.process().await,
-            Commands::Setup(opts) => opts.process().await,
-            Commands::Create(opts) => opts.process().await,
-            Commands::Self_(opts) => opts.process().await,
+            Self::List(opts) => opts.process().await,
+            Self::Install(opts) => opts.process().await,
+            Self::Upgrade(opts) => opts.process().await,
+            Self::Uninstall(opts) => opts.process().await,
+            Self::Reinstall(opts) => opts.process().await,
+            Self::Inject(opts) => opts.process().await,
+            Self::Activate(opts) => opts.process().await,
+            Self::UpgradeAll(opts) => opts.process().await,
+            Self::Runuv(opts) => opts.process().await,
+            Self::Runpip(opts) => opts.process().await,
+            Self::Runpython(opts) => opts.process().await,
+            Self::Ensurepath(opts) => opts.process().await,
+            Self::UninstallAll(opts) => opts.process().await,
+            Self::ReinstallAll(opts) => opts.process().await,
+            Self::Uninject(opts) => opts.process().await,
+            Self::Completions(opts) => opts.process().await,
+            Self::Run(opts) => opts.process().await,
+            Self::Setup(opts) => opts.process().await,
+            Self::Create(opts) => opts.process().await,
+            Self::Self_(opts) => opts.process().await,
+            Self::Check(opts) => opts.process().await,
         }
     }
 }
 
 #[derive(Debug, Parser)]
 pub struct SelfUpdateOptions {
     #[clap(long, help = "Update without also updating uv")]
@@ -362,12 +388,12 @@
     #[clap(about = "Show the uvx changelog")]
     Changelog(ChangelogOptions),
 }
 
 impl Process for SelfCommands {
     async fn process(self) -> Result<i32, String> {
         match self {
-            SelfCommands::Update(opts) => opts.process().await,
-            SelfCommands::Changelog(opts) => opts.process().await,
+            Self::Update(opts) => opts.process().await,
+            Self::Changelog(opts) => opts.process().await,
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/cmd.rs` & `uvx-2.3.0/src/cmd.rs`

 * *Files 6% similar despite different names*

```diff
@@ -67,40 +67,41 @@
 
     match result {
         Ok(result) => match result.status.code() {
             Some(0) => Ok(true),
             Some(_) | None => {
                 let err = String::from_utf8(result.stderr).unwrap_or_default();
                 match err_prefix {
-                    Some(prefix) => Err(format!("{} | {}", prefix, err)),
+                    Some(prefix) => Err(format!("{prefix} | {err}")),
                     None => Err(err),
                 }
             },
         },
         Err(result) => {
             let err = result.to_string();
             match err_prefix {
-                Some(prefix) => Err(format!("{} | {}", prefix, err)),
+                Some(prefix) => Err(format!("{prefix} | {err}")),
                 None => Err(err),
             }
         },
     }
 }
 
 /// Given a target shell (e.g. 'bash'), run a positive or negative callback function.
 pub fn run_if_shell<T, Y: Fn(String) -> Option<T>, N: Fn(String) -> Option<T>>(
     target: &str,
     if_bash: Y,
     if_not_bash: N,
 ) -> Option<T> {
     let shell = env::var("SHELL").ok().unwrap_or_default();
 
-    match shell.ends_with(target) {
-        true => if_bash(shell),
-        false => if_not_bash(shell),
+    if shell.ends_with(target) {
+        if_bash(shell)
+    } else {
+        if_not_bash(shell)
     }
 }
 
 /// Run a callback function if bash, or show a message saying the user's shell is unsupported.
 pub fn run_if_bash_else_warn<T, Y: Fn(String) -> Option<T>>(if_bash: Y) -> Option<T> {
     run_if_shell("bash", if_bash, |shell| {
         eprintln!(
```

### Comparing `uvx-2.2.2/src/commands/activate.rs` & `uvx-2.3.0/src/commands/activate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.2/src/commands/changelog.rs` & `uvx-2.3.0/src/commands/changelog.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
             continue;
         }
 
         if let Some(category_caps) = category_re.captures(line) {
             let category = category_caps[1].to_string();
             if let Some(map) = changelog.get_mut(&current_version) {
                 map.insert(category.clone(), Vec::new());
-                current_category = category
+                current_category = category;
             }
             continue;
         }
 
         if let Some(feature_caps) = feature_re.captures(line) {
             let features = feature_caps[1].to_string();
 
             if let Some(map) = changelog.get_mut(&current_version) {
                 if let Some(vec) = map.get_mut(&current_category) {
-                    vec.push(features)
+                    vec.push(features);
                 }
             }
             continue;
         }
     }
 
     changelog
@@ -94,15 +94,15 @@
 
 pub fn display_changelog(changelog: &Changelogs) {
     for (version, changes) in changelog {
         println!("- {}", version.bold());
         for (category, descriptions) in changes {
             println!("-- {}", color(category));
             for change in descriptions {
-                println!("---- {}", colored_markdown(change))
+                println!("---- {}", colored_markdown(change));
             }
         }
     }
 }
 
 pub async fn changelog() -> Option<i32> {
     let md = get_changelog().await?;
@@ -112,12 +112,12 @@
     display_changelog(&parsed);
 
     Some(0)
 }
 
 impl Process for ChangelogOptions {
     async fn process(self) -> Result<i32, String> {
-        changelog().await.ok_or(String::from(
-            "Something went wrong while loading the changelog.",
-        ))
+        changelog()
+            .await
+            .ok_or_else(|| String::from("Something went wrong while loading the changelog."))
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/completions.rs` & `uvx-2.3.0/src/commands/completions.rs`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         Ok(0)
     } else {
         Ok(run_if_bash_else_warn(|_shell| {
             eprintln!(
                 "Tip: place this line in your ~/.bashrc or run '{}' to do this automatically!",
                 "uvx setup".green()
             );
-            println!("{}", for_bash);
+            println!("{for_bash}");
             Some(0)
         })
         .unwrap_or(1))
     }
 }
 
 impl Process for CompletionsOptions {
```

### Comparing `uvx-2.2.2/src/commands/create.rs` & `uvx-2.3.0/src/commands/create.rs`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,14 @@
             self.python.as_ref(),
             !self.no_seed,
             self.force,
         )
         .await
         {
             Ok(msg) => {
-                println!("{}", msg);
+                println!("{msg}");
                 Ok(0)
             },
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/ensurepath.rs` & `uvx-2.3.0/src/commands/ensurepath.rs`

 * *Files 10% similar despite different names*

```diff
@@ -46,48 +46,48 @@
            f.write(final_text)
     */
     let path = get_home_dir().join(".bashrc");
 
     let now = now();
     let mut final_text = String::from("\n");
     if with_comment {
-        final_text.push_str(&format!("# Added by `uvx` at {now}\n"))
+        final_text.push_str(&format!("# Added by `uvx` at {now}\n"));
     }
 
     final_text.push_str(text);
     final_text.push('\n');
 
     append(&path, final_text).await
 }
 
 pub async fn ensure_path(force: bool) -> Result<(), String> {
     let bin_path = ensure_bin_dir().await;
     let bin_dir = bin_path.to_str().unwrap_or_default();
 
     let path = std::env::var("PATH").unwrap_or_default();
 
-    let parts: Vec<&str> = path.split(':').collect();
-
-    if parts.contains(&bin_dir) && !force {
+    // let parts: Vec<&str> = path.split(':').collect();
+    // if parts.contains(&bin_dir) && !force {
+    if !force && path.split(':').any(|x| x == bin_dir) {
         return Err(format!("{}: {} is already added to your path. Use '--force' to add it to your .bashrc file anyway.",
             "Warning".yellow(),
             bin_dir.green()
-    ))  ;
+    ));
     }
 
-    add_to_bashrc(&format!("export PATH=\"$PATH:{}\"", bin_dir), true).await?;
+    add_to_bashrc(&format!("export PATH=\"$PATH:{bin_dir}\""), true).await?;
 
     println!("Added '{}' to ~/.bashrc", bin_dir.green());
     Ok(())
 }
 
 pub async fn ensure_path_generate() -> String {
     let bin_path = ensure_bin_dir().await;
     let bin_dir = bin_path.to_str().unwrap_or_default();
-    format!("export PATH=\"$PATH:{}\"", bin_dir)
+    format!("export PATH=\"$PATH:{bin_dir}\"")
 }
 
 impl Process for EnsurepathOptions {
     async fn process(self) -> Result<i32, String> {
         ensure_path(self.force).await?;
         Ok(0)
     }
```

### Comparing `uvx-2.2.2/src/commands/inject.rs` & `uvx-2.3.0/src/commands/uninject.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,58 @@
-use crate::metadata::LoadMetadataConfig;
-use crate::{
-    animate::{show_loading_indicator, AnimationSettings},
-    cli::{InjectOptions, Process},
-    metadata::Metadata,
-    uv::{uv, Helpers},
-    venv::setup_environ_from_requirement,
-};
+use crate::animate::{show_loading_indicator, AnimationSettings};
+use crate::cli::{Process, UnInjectOptions};
+use crate::metadata::{LoadMetadataConfig, Metadata};
+use crate::venv::setup_environ_from_requirement;
+use itertools::Itertools;
 use owo_colors::OwoColorize;
 
-pub async fn inject_package(
-    venv_spec: &str,
-    to_inject_specs: &[String],
-    no_cache: bool,
+use crate::uv::{uv, Helpers};
+
+pub async fn eject_package(
+    from: &str,
+    to_eject_specs: &[String],
 ) -> Result<String, String> {
-    let (requirement, environ) = setup_environ_from_requirement(venv_spec).await?;
+    let (requirement, environ) = setup_environ_from_requirement(from).await?;
     let mut metadata = Metadata::for_requirement(&requirement, &LoadMetadataConfig::none()).await;
 
-    let mut args = vec!["pip", "install"];
-
-    if no_cache {
-        args.push("--no-cache")
-    }
+    let mut args = vec!["pip", "uninstall"];
 
-    // vec<string> -> vec<str>
-    let inject_args: Vec<&str> = to_inject_specs.iter().map(|k| k.as_ref()).collect();
-    args.extend(inject_args);
+    let eject_args: Vec<&str> = to_eject_specs.iter().map(AsRef::as_ref).collect();
+    args.extend(eject_args);
 
     let promise = uv(args);
 
-    let to_inject_str = &to_inject_specs.join(", ");
+    let to_eject_str = &to_eject_specs.iter().map(|it| it.green()).join(", ");
     show_loading_indicator(
         promise,
-        format!("injecting {} into {}", &to_inject_str, &metadata.name),
+        format!("injecting {} into {}", &to_eject_str, &metadata.name),
         AnimationSettings::default(),
     )
     .await?;
 
-    metadata
+    metadata.injected = metadata
         .injected
-        .extend(to_inject_specs.iter().map(|k| k.to_string()));
+        .iter()
+        .filter(|i| !to_eject_specs.contains(i))
+        .map(ToString::to_string)
+        .collect();
+
     metadata.save(&environ.to_path_buf()).await?;
 
     Ok(format!(
-        "💉 Injected [{}] into {}.",
-        &to_inject_str,
+        "⏏️  Ejected [{}] from {}.",
+        &to_eject_str,
         &metadata.name.green(),
     ))
 }
 
-impl Process for InjectOptions {
+impl Process for UnInjectOptions {
     async fn process(self) -> Result<i32, String> {
-        match inject_package(&self.into, &self.package_specs, self.no_cache).await {
+        match eject_package(&self.outof, &self.package_specs).await {
             Ok(msg) => {
-                println!("{}", msg);
+                println!("{msg}");
                 Ok(0)
             },
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/install.rs` & `uvx-2.3.0/src/commands/install.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,52 +21,52 @@
     no_cache: bool,
     force: bool,
     editable: bool,
 ) -> Result<bool, String> {
     let mut args: Vec<&str> = vec!["pip", "install"];
 
     if !inject.is_empty() {
-        args.append(&mut inject.to_owned())
+        args.append(&mut inject.to_owned());
     }
 
     if no_cache || force {
-        args.push("--no-cache")
+        args.push("--no-cache");
     }
 
     if editable {
         // -e should go right before package name!
-        args.push("--editable")
+        args.push("--editable");
     }
     args.push(package_name);
 
     let promise = uv(args);
 
     show_loading_indicator(
         promise,
-        format!("installing {}", package_name),
+        format!("installing {package_name}"),
         AnimationSettings::default(),
     )
     .await
 }
 
 async fn ensure_venv(
     maybe_venv: Option<&Path>,
     requirement: &Requirement,
     python: Option<&String>,
     force: bool,
 ) -> Result<PathBuf, String> {
     match maybe_venv {
         Some(venv) => {
             let buf = venv.to_path_buf();
-            if !buf.exists() {
+            if buf.exists() {
+                Ok(buf)
+            } else {
                 Err(String::from(
                     "Package could not be installed because supplied venv was misssing.",
                 ))
-            } else {
-                Ok(buf)
             }
         },
         None => create_venv(&requirement.name, python, force, true, None).await,
     }
 }
 
 async fn store_metadata(
@@ -90,15 +90,15 @@
         "{} {}",
         python_info.platform_python_implementation(),
         python_info.python_full_version()
     );
     metadata.python_raw = venv.stdlib_as_string();
 
     metadata.extras = requirement.extras();
-    metadata.injected = inject.iter().map(|inj| inj.to_string()).collect();
+    metadata.injected = inject.iter().map(ToString::to_string).collect();
 
     if let Ok(version) = uv_get_installed_version(&requirement.name, Some(venv)) {
         metadata.installed_version = version;
     }
 
     metadata.save(&venv.to_path_buf()).await?;
     Ok(metadata)
@@ -183,14 +183,14 @@
             vec![],
             self.no_cache,
             self.editable,
         )
         .await
         {
             Ok(msg) => {
-                println!("{}", msg);
+                println!("{msg}");
                 Ok(0)
             },
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/list.rs` & `uvx-2.3.0/src/commands/list.rs`

 * *Files 5% similar despite different names*

```diff
@@ -9,88 +9,80 @@
     metadata_dir: ReadDir,
     config: &LoadMetadataConfig,
 ) -> Vec<Metadata> {
     let mut result: Vec<Metadata> = vec![];
 
     for dir in metadata_dir.flatten() {
         if let Some(metadata) = Metadata::for_dir(&dir.path(), config).await {
-            result.push(metadata)
+            result.push(metadata);
         } else {
             let venv_name = dir.file_name().into_string().unwrap_or_default();
 
             eprintln!("! metadata for '{}' could not be read!", venv_name.red());
         }
     }
 
     result
 }
 
 impl ListOptions {
-    pub async fn process_json(
+    pub fn process_json(
         self,
-        items: &Vec<&Metadata>,
+        items: &Vec<Metadata>,
     ) -> Result<i32, String> {
         let json = if self.short {
             serde_json::to_string(items).map_err_to_string()?
         } else {
             serde_json::to_string_pretty(items).map_err_to_string()?
         };
 
-        println!("{}", json);
+        println!("{json}");
 
         Ok(0)
     }
 
-    pub fn to_metadataconfig(&self) -> LoadMetadataConfig {
+    pub const fn to_metadataconfig(&self) -> LoadMetadataConfig {
         LoadMetadataConfig {
             recheck_scripts: true, // always done
             updates_check: !self.skip_updates,
             updates_prereleases: self.show_prereleases,
             updates_ignore_constraints: self.ignore_constraints,
         }
     }
 }
 
 pub async fn list_packages(config: &LoadMetadataConfig) -> Result<Vec<Metadata>, String> {
     let venv_dir_path = get_venv_dir();
-    let possibly_missing = std::fs::read_dir(&venv_dir_path);
 
     // no tokio::fs because ReadDir.flatten doesn't exist then.
-    let must_exist = match possibly_missing {
-        Ok(dir) => dir,
-        Err(_) => {
-            std::fs::create_dir_all(&venv_dir_path).map_err_to_string()?;
-            std::fs::read_dir(&venv_dir_path).map_err_to_string()?
-        },
+    let must_exist = if let Ok(dir) = std::fs::read_dir(&venv_dir_path) {
+        dir
+    } else {
+        std::fs::create_dir_all(&venv_dir_path).map_err_to_string()?;
+        std::fs::read_dir(&venv_dir_path).map_err_to_string()?
     };
 
     Ok(read_from_folder(must_exist, config).await)
 }
 
 impl Process for ListOptions {
     async fn process(self) -> Result<i32, String> {
         let config = self.to_metadataconfig();
 
-        let all_items = list_packages(&config).await?;
+        let mut items = list_packages(&config).await?;
 
-        let filtered_items: Vec<&Metadata> = if !self.venv_names.is_empty() {
-            // add filter
-            all_items
-                .iter()
-                .filter(|k| self.venv_names.contains(&k.name))
-                .collect()
-        } else {
-            all_items.iter().collect() // iter collect to make it the same type as the other branch...
-        };
+        if !self.venv_names.is_empty() {
+            items.retain(|k| self.venv_names.contains(&k.name));
+        }
 
         if self.json {
-            return self.process_json(&filtered_items).await;
+            return self.process_json(&items);
         }
 
-        for metadata in filtered_items {
+        for metadata in items {
             if self.verbose {
                 // println!("{}", dbg_pls::color(&metadata));
                 println!("{:#?}", &metadata);
             } else if self.short {
                 println!("{}", &metadata.format_short());
             } else {
                 println!("{}", &metadata.format_human());
```

### Comparing `uvx-2.2.2/src/commands/reinstall.rs` & `uvx-2.3.0/src/commands/reinstall.rs`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,14 @@
             !self.without_injected,
             self.no_cache,
             self.editable,
         )
         .await
         {
             Ok(msg) => {
-                println!("{}", msg);
+                println!("{msg}");
                 Ok(0)
             },
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/reinstall_all.rs` & `uvx-2.3.0/src/commands/reinstall_all.rs`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             !without_injected,
             no_cache,
             editable,
         )
         .await
         {
             Ok(msg) => {
-                println!("{}", msg)
+                println!("{msg}");
             },
             Err(msg) => {
                 eprintln!("{}", msg.red());
                 all_ok = false;
             },
         }
     }
@@ -50,12 +50,12 @@
             self.force,
             self.without_injected,
             self.no_cache,
             self.editable,
         )
         .await
         {
-            Ok(_) => Ok(0),
+            Ok(()) => Ok(0),
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/run.rs` & `uvx-2.3.0/src/commands/run.rs`

 * *Files 3% similar despite different names*

```diff
@@ -8,52 +8,58 @@
 use crate::commands::install::_install_package;
 use crate::commands::runpython::process_subprocess;
 use crate::pip::parse_requirement;
 use crate::symlinks::find_symlinks;
 use crate::uv::uv_get_installed_version;
 use crate::venv::{activate_venv, create_venv, remove_venv};
 
+async fn _find_executable(
+    requirement: &Requirement,
+    package_spec: &str,
+    venv: &PythonEnvironment,
+) -> Result<String, String> {
+    let installed_version = uv_get_installed_version(&requirement.name, Some(venv))?;
+    let symlinks = find_symlinks(requirement, &installed_version, venv).await;
+
+    match symlinks.len() {
+        0 => {
+            // just return the original name just as a last hope:
+            Ok(requirement.name.to_string())
+        },
+        1 => Ok(symlinks[0].clone()),
+        _ => {
+            // too many choices, user should provide --binary <something>
+            let mut related = String::new();
+
+            for option in symlinks {
+                let code = format!("uvx run {package_spec} --binary {option} ...");
+                related.push_str(&format!("\t- {} | `{}` \n", option.green(), code.blue()));
+            }
+
+            Err(
+                format!("'{}' executable not found for install spec '{}'.\nMultiple related scripts were found:\n{}",
+                        requirement.name.to_string().green(),
+                        package_spec.green(),
+                        related,
+                )
+            )
+        },
+    }
+}
+
 pub async fn find_executable(
     requirement: &Requirement,
     binary: Option<&String>,
     package_spec: &str,
     venv: &PythonEnvironment,
     venv_path: &Path,
 ) -> Result<PathBuf, String> {
     let executable = match binary {
         Some(executable) => executable.to_owned(),
-        None => {
-            let installed_version = uv_get_installed_version(&requirement.name, Some(venv))?;
-            let symlinks = find_symlinks(requirement, &installed_version, venv).await;
-
-            match symlinks.len() {
-                0 => {
-                    // just return the original name just as a last hope:
-                    requirement.name.to_string()
-                },
-                1 => symlinks[0].to_owned(),
-                _ => {
-                    // too many choices, user should provide --binary <something>
-                    let mut related = String::new();
-
-                    for option in symlinks {
-                        let code = format!("uvx run {} --binary {} ...", package_spec, option);
-                        related.push_str(&format!("\t- {} | `{}` \n", option.green(), code.blue()));
-                    }
-
-                    return Err(
-                        format!("'{}' executable not found for install spec '{}'.\nMultiple related scripts were found:\n{}",
-                                requirement.name.to_string().green(),
-                                package_spec.green(),
-                                related,
-                        )
-                    );
-                },
-            }
-        },
+        None => _find_executable(requirement, package_spec, venv).await?,
     };
 
     let full_exec_path = venv_path.join("bin").join(executable);
     Ok(full_exec_path)
 }
 
 pub async fn run_executable(
@@ -94,15 +100,15 @@
         Some(String::from("/tmp/uvx-")),
     )
     .await?;
 
     let venv_name = &venv_path.to_str().unwrap_or_default();
 
     if keep {
-        eprintln!("ℹ️ Using virtualenv {}", venv_name.blue())
+        eprintln!("ℹ️ Using virtualenv {}", venv_name.blue());
     }
 
     // ### 2 ###
     let venv = &activate_venv(venv_path).await?;
 
     // already expects activated venv:
     _install_package(package_spec, &Vec::new(), no_cache, false, false).await?;
```

### Comparing `uvx-2.2.2/src/commands/runpip.rs` & `uvx-2.3.0/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.2/src/commands/runpython.rs` & `uvx-2.3.0/src/commands/runpython.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 use crate::{
     cli::{Process, RunpythonOptions},
     helpers::ResultToString,
     venv::setup_environ_from_requirement,
 };
 
+#[allow(clippy::cast_lossless)]
 pub fn process_subprocess<S: AsRef<OsStr>>(
     exec_path: &Path,
     args: &[S],
 ) -> Result<i32, String> {
     Ok(
         match Exec::cmd(exec_path).args(args).join().map_err_to_string()? {
             subprocess::ExitStatus::Exited(int) => int as i32,
```

### Comparing `uvx-2.2.2/src/commands/runuv.rs` & `uvx-2.3.0/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.2/src/commands/self_update.rs` & `uvx-2.3.0/src/commands/self_update.rs`

 * *Files 4% similar despite different names*

```diff
@@ -46,70 +46,75 @@
 
     packages
         .iter()
         .map(|k| extract_version(&output, k.as_ref()).unwrap_or_default())
         .collect()
 }
 
+pub fn find_global_python() -> Result<PathBuf, String> {
+    let fallback = PathBuf::from("/usr/bin/python3");
+    if fallback.exists() {
+        Ok(fallback)
+    } else {
+        Err(format!(
+            "Python could not be found! Is `{}` installed globally (without a venv)?",
+            "uvx".green()
+        ))
+    }
+}
+
+pub async fn find_python() -> Result<PathBuf, String> {
+    find_sibling("python")
+        .await
+        .map_or_else(find_global_python, Ok)
+}
+
 pub async fn self_update(with_uv: bool) -> Result<i32, String> {
-    let exe = match find_sibling("python").await {
-        Some(sibling) => sibling,
-        None => {
-            let fallback = PathBuf::from("/usr/bin/python3");
-            if fallback.exists() {
-                fallback
-            } else {
-                return Err(format!(
-                    "Python could not be found! Is `{}` installed globally (without a venv)?",
-                    "uvx".green()
-                ));
-            }
-        },
-    };
+    let exe = find_python().await?;
 
     // todo: with 'uv' instead of pip later?
     let mut args = vec!["-m", "pip", "install", "--no-cache-dir", "--upgrade", "uvx"];
 
     let mut to_track = vec!["uvx"];
     let mut msg = String::from("uvx");
     if with_uv {
         args.push("uv");
         to_track.push("uv");
-        msg.push_str(" and uv")
+        msg.push_str(" and uv");
     }
 
     let old = get_package_versions(&exe, &to_track).await;
 
     let exe_str = exe.to_str().unwrap_or_default();
     let promise = run(&exe_str, args, None);
 
     show_loading_indicator(
         promise,
-        format!("updating {}", msg),
+        format!("updating {msg}"),
         AnimationSettings::default(),
     )
     .await?;
 
     let new = get_package_versions(&exe, &to_track).await;
 
     for (versions, package) in new.iter().zip(old.iter()).zip(to_track.iter()) {
         let (after, before) = versions;
         if before == after {
             println!(
                 "🌟 '{}' not updated (version: {})",
                 package.blue(),
                 before.green()
-            )
+            );
         } else {
             println!(
                 "🚀 '{}' updated from {} to {}",
                 package.blue(),
                 before.red(),
                 after.green(),
-            )
+            );
         }
     }
 
     Ok(0)
 }
 
 impl Process for SelfUpdateOptions {
```

### Comparing `uvx-2.2.2/src/commands/setup.rs` & `uvx-2.3.0/src/commands/setup.rs`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 use crate::cli::{Process, SetupOptions};
 use crate::cmd::run_if_bash_else_warn;
 use crate::commands::activate::install_activate;
 use crate::commands::completions::completions;
 use crate::commands::ensurepath::ensure_path;
 use crate::metadata::{get_work_dir, load_generic_msgpack, store_generic_msgpack};
 
-#[derive(Debug, PartialEq, Deserialize, Serialize)] // dbg_pls::DebugPls
+#[derive(Debug, PartialEq, Eq, Deserialize, Serialize)] // dbg_pls::DebugPls
 pub struct SetupMetadata {
     // order is important, new features should go last!!
     #[serde(default)]
     pub feature_ensurepath: bool,
     #[serde(default)]
     pub feature_completions: bool,
     #[serde(default)]
     pub feature_activate: bool,
 }
 
 impl SetupMetadata {
-    pub fn new() -> Self {
-        SetupMetadata {
+    pub const fn new() -> Self {
+        Self {
             feature_ensurepath: false,
             feature_completions: false,
             feature_activate: false,
         }
     }
 }
 
@@ -44,15 +44,17 @@
     // Open the msgpack file
     let metadata: SetupMetadata = load_generic_msgpack(&filename, &mut buf).await?;
 
     Ok(metadata)
 }
 
 pub async fn load_setup_metadata() -> SetupMetadata {
-    _load_setup_metadata().await.unwrap_or(SetupMetadata::new())
+    _load_setup_metadata()
+        .await
+        .unwrap_or_else(|_| SetupMetadata::new())
 }
 
 pub async fn store_setup_metadata(metadata: &SetupMetadata) -> Result<(), String> {
     let filename = setup_metadata_filename();
 
     store_generic_msgpack(&filename, metadata).await
 }
@@ -66,42 +68,43 @@
     let mut any_warnings: bool = false;
 
     let mut metadata = load_setup_metadata().await;
 
     if do_ensurepath && (!metadata.feature_ensurepath || force) {
         if let Err(msg) = ensure_path(force).await {
             any_warnings = true;
-            eprintln!("{}", msg);
+            eprintln!("{msg}");
         }
         metadata.feature_ensurepath = true;
     }
 
     if do_completions && (!metadata.feature_completions || force) {
         if let Err(msg) = completions(true).await {
             any_warnings = true;
-            eprintln!("{}", msg);
+            eprintln!("{msg}");
         }
         metadata.feature_completions = true;
     }
 
     if do_activate && (!metadata.feature_activate || force) {
         if let Err(msg) = install_activate().await {
             any_warnings = true;
-            eprintln!("{}", msg);
+            eprintln!("{msg}");
         }
         metadata.feature_activate = true;
     }
 
     if let Err(msg) = store_setup_metadata(&metadata).await {
         any_warnings = true;
-        eprintln!("{}", msg);
+        eprintln!("{msg}");
     }
 
     println!("Setup finished, you may want to run `{}` now in order to apply these changes to your shell.", "exec bash".green());
-    Ok(if any_warnings { 1 } else { 0 })
+    // bool to int
+    Ok(i32::from(any_warnings))
 }
 
 impl Process for SetupOptions {
     async fn process(self) -> Result<i32, String> {
         let result = run_if_bash_else_warn(move |_| {
             // some logic here
             let result = setup_for_bash(
```

### Comparing `uvx-2.2.2/src/commands/uninstall.rs` & `uvx-2.3.0/src/commands/uninstall.rs`

 * *Files 12% similar despite different names*

```diff
@@ -13,53 +13,53 @@
 ) -> Result<String, String> {
     let (requirement, _) = parse_requirement(package_name).await?;
     let requirement_name = requirement.name.to_string();
 
     let venv_dir = venv_path(&requirement_name);
 
     if !venv_dir.exists() {
-        return if !force {
-            Err(format!("No virtualenv for '{}', stopping.\nUse '{}' to remove an executable with that name anyway.",
-                        &requirement_name.green(), "--force".green()))
-        } else {
+        return if force {
             remove_symlink(&requirement_name).await?;
             Err(format!(
                 "{}: No virtualenv for '{}'.",
                 "Warning".yellow(),
                 &requirement_name.green()
             ))
+        } else {
+            Err(format!("No virtualenv for '{}', stopping.\nUse '{}' to remove an executable with that name anyway.",
+                                        &requirement_name.green(), "--force".green()))
         };
     }
 
     let venv = activate_venv(&venv_dir).await?;
 
     let metadata = Metadata::for_requirement(&requirement, &LoadMetadataConfig::none()).await;
 
     // symlinks = find_symlinks(package_name, venv_path) or [package_name]
     let symlinks = find_symlinks(&requirement, &metadata.installed_version, &venv).await;
 
     remove_symlinks(symlinks).await?;
 
     remove_venv(&venv.to_path_buf()).await?;
 
-    let version_msg = if !metadata.installed_version.is_empty() {
-        format!(" ({})", metadata.installed_version.cyan())
-    } else {
+    let version_msg = if metadata.installed_version.is_empty() {
         String::new()
+    } else {
+        format!(" ({})", metadata.installed_version.cyan())
     };
 
-    let msg = format!("🗑️  {}{} removed!", package_name, version_msg);
+    let msg = format!("🗑️  {package_name}{version_msg} removed!");
 
     Ok(msg)
 }
 
 impl Process for UninstallOptions {
     async fn process(self) -> Result<i32, String> {
         match uninstall_package(&self.package_name, self.force).await {
             Ok(msg) => {
-                println!("{}", msg);
+                println!("{msg}");
                 Ok(0)
             },
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/uninstall_all.rs` & `uvx-2.3.0/src/commands/uninstall_all.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 pub async fn uninstall_all(force: bool) -> Result<(), String> {
     let mut all_ok = true;
 
     for meta in list_packages(&LoadMetadataConfig::none()).await? {
         match uninstall_package(&meta.name, force).await {
             Ok(msg) => {
-                println!("{}", msg)
+                println!("{msg}");
             },
             Err(msg) => {
                 eprintln!("{}", msg.red());
                 all_ok = false;
             },
         }
     }
@@ -27,12 +27,12 @@
         ))
     }
 }
 
 impl Process for UninstallAllOptions {
     async fn process(self) -> Result<i32, String> {
         match uninstall_all(self.force).await {
-            Ok(_) => Ok(0),
+            Ok(()) => Ok(0),
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/upgrade.rs` & `uvx-2.3.0/src/commands/upgrade.rs`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     metadata.installed_version.clone_from(&new_version);
     metadata.save(&environ.to_path_buf()).await?;
 
     Ok(new_version)
 }
 
 fn build_msg(
-    old_version: String,
-    new_version: String,
-    metadata: &mut Metadata,
-) -> Result<String, String> {
+    old_version: &str,
+    new_version: &str,
+    metadata: &Metadata,
+) -> String {
     let mut msg = String::new();
     if old_version == new_version {
         msg.push_str(&format!(
             "🌟 '{}' is already up to date at version {}!",
             &metadata.name.green(),
             &new_version.cyan()
         ));
@@ -52,15 +52,15 @@
             "🚀 Successfully updated '{}' from version {} to version {}!",
             metadata.name.green(),
             old_version.cyan(),
             new_version.cyan()
         ));
     }
 
-    Ok(msg)
+    msg
 }
 
 pub async fn _upgrade_package(
     requirement: &Requirement,
     metadata: &mut Metadata,
     environ: &PythonEnvironment,
     force: bool,
@@ -68,34 +68,34 @@
     skip_injected: bool,
 ) -> Result<String, String> {
     let old_version = metadata.installed_version.clone();
 
     let mut args = vec!["pip", "install", "--upgrade"];
 
     if force || no_cache {
-        args.push("--no-cache")
+        args.push("--no-cache");
     }
 
     let version = requirement.version().or(if force {
         ""
     } else {
         &metadata.requested_version
     });
 
     let mut upgrade_spec = metadata.name.clone();
 
     let mut extras = metadata.extras.clone();
     extras.extend(requirement.extras());
 
     if !extras.is_empty() {
-        upgrade_spec.push_str(&format!("[{}]", extras.iter().join(",")))
+        upgrade_spec.push_str(&format!("[{}]", extras.iter().join(",")));
     }
 
     if !version.is_empty() {
-        upgrade_spec.push_str(&version)
+        upgrade_spec.push_str(&version);
     }
 
     args.push(&upgrade_spec);
 
     if !skip_injected {
         args.extend(metadata.vec_injected());
     }
@@ -107,15 +107,15 @@
         format!("upgrading {}", &metadata.name),
         AnimationSettings::default(),
     )
     .await?;
 
     let new_version = update_metadata(metadata, requirement, environ, version).await?;
 
-    build_msg(old_version, new_version, metadata)
+    Ok(build_msg(&old_version, &new_version, metadata))
 }
 
 pub async fn upgrade_package(
     install_spec: &str,
     force: bool,
     no_cache: bool,
     skip_injected: bool,
@@ -146,14 +146,14 @@
             self.force,
             self.no_cache,
             self.skip_injected,
         )
         .await
         {
             Ok(msg) => {
-                println!("{}", msg);
+                println!("{msg}");
                 Ok(0)
             },
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/commands/upgrade_all.rs` & `uvx-2.3.0/src/commands/upgrade_all.rs`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     skip_injected: bool,
 ) -> Result<(), String> {
     let mut all_ok = true;
 
     for meta in list_packages(&LoadMetadataConfig::none()).await? {
         match upgrade_package(&meta.name, force, no_cache, skip_injected).await {
             Ok(msg) => {
-                println!("{}", msg)
+                println!("{msg}");
             },
             Err(msg) => {
                 eprintln!("{}", msg.red());
                 all_ok = false;
             },
         }
     }
@@ -30,12 +30,12 @@
         Err(String::from("⚠️ Not all packages were properly upgraded!"))
     }
 }
 
 impl Process for UpgradeAllOptions {
     async fn process(self) -> Result<i32, String> {
         match upgrade_all(self.force, self.no_cache, self.skip_injected).await {
-            Ok(_) => Ok(0),
+            Ok(()) => Ok(0),
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.2.2/src/helpers.rs` & `uvx-2.3.0/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.2.2/src/main.rs` & `uvx-2.3.0/src/main.rs`

 * *Files 6% similar despite different names*

```diff
@@ -15,65 +15,62 @@
 use clap::{Command, CommandFactory, Parser};
 use clap_complete::{generate, Generator, Shell};
 
 use crate::cli::{Args, Process};
 use crate::commands::activate::generate_activate;
 use crate::commands::ensurepath::ensure_path_generate;
 
-pub async fn print_completions<G: Generator>(
+pub fn print_completions<G: Generator>(
     gen: G,
     cmd: &mut Command,
 ) {
     generate(gen, cmd, cmd.get_name().to_string(), &mut io::stdout());
 }
 
 pub async fn generate_bash(generator: Shell) {
     let mut cmd = Args::command();
 
     let args = &cmd.clone().get_matches();
     match args.subcommand_name() {
         Some("activate") => {
             // generate code for uvx activate
-            println!("{}", generate_activate().await)
+            println!("{}", generate_activate().await);
         },
         Some("ensurepath") => {
             // geneate code for uvx ensurepath
-            println!("{}", ensure_path_generate().await)
+            println!("{}", ensure_path_generate().await);
         },
         _ => {
             // other cases: show regular completions
-            print_completions(generator, &mut cmd).await;
+            print_completions(generator, &mut cmd);
             // todo: dynamic completions for e.g. `uvx upgrade <venv>`
         },
     }
 }
 
 pub async fn generate_code(target: Shell) -> i32 {
-    match target {
-        Shell::Bash => {
-            generate_bash(target).await;
-            0
-        },
-        _ => {
-            eprintln!("Error: only 'bash' is supported at this moment.");
-            126
-        },
+    if target == Shell::Bash {
+        generate_bash(target).await;
+        0
+    } else {
+        eprintln!("Error: only 'bash' is supported at this moment.");
+        126
     }
 }
 
 #[tokio::main]
 async fn main() {
     let args = Args::parse();
 
     let exit_code = if let Some(generator) = args.generator {
         generate_code(generator).await
     } else {
         let result = args.cmd.process().await;
         result.unwrap_or_else(|msg| {
-            eprintln!("Something went wrong | {}", msg);
+            eprintln!("Something went wrong | {msg}");
             1
         })
     };
 
     // If bundled via an entrypoint, the first argument is 'python' so skip it:
     // let args = Args::parse_from_python();
```

### Comparing `uvx-2.2.2/src/metadata.rs` & `uvx-2.3.0/src/metadata.rs`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     get_venv_dir().join(venv_name)
 }
 
 pub fn version_0() -> Version {
     Version::from_str("0.0.0").unwrap()
 }
 
-#[derive(Debug, PartialEq, Deserialize, Serialize)] // dbg_pls::DebugPls
+#[derive(Debug, PartialEq, Eq, Deserialize, Serialize)] // dbg_pls::DebugPls
 pub struct Metadata {
     // order is important!!
     pub name: String,
     #[serde(default)]
     pub scripts: HashMap<String, bool>,
     pub install_spec: String,
     #[serde(default)]
@@ -81,16 +81,16 @@
     #[serde(default)]
     pub available_version: String,
     #[serde(default)]
     pub outdated: bool,
 }
 
 impl Metadata {
-    pub fn new(name: &str) -> Metadata {
-        Metadata {
+    pub fn new(name: &str) -> Self {
+        Self {
             name: name.to_string(),
             scripts: HashMap::new(),
             install_spec: name.to_string(),
             extras: HashSet::new(),
             requested_version: String::new(),
             installed_version: String::new(),
             python: String::new(),
@@ -100,22 +100,22 @@
             available_version: String::new(),
             outdated: false,
         }
     }
 
     #[allow(dead_code)]
     pub fn requested_version_parsed(&self) -> Version {
-        Version::from_str(&self.requested_version).unwrap_or(version_0())
+        Version::from_str(&self.requested_version).unwrap_or_else(|_| version_0())
     }
     pub fn installed_version_parsed(&self) -> Version {
-        Version::from_str(&self.installed_version).unwrap_or(version_0())
+        Version::from_str(&self.installed_version).unwrap_or_else(|_| version_0())
     }
 
-    pub fn find(req: &Requirement) -> Metadata {
-        let mut empty = Metadata::new(req.name.as_ref());
+    pub fn find(req: &Requirement) -> Self {
+        let mut empty = Self::new(req.name.as_ref());
 
         empty.installed_version = uv_get_installed_version(&req.name, None).unwrap_or_default();
 
         empty.fill(None);
         empty
     }
 
@@ -126,77 +126,75 @@
         let python_info = venv.interpreter().markers();
 
         if self.python.is_empty() {
             self.python = format!(
                 "{} {}",
                 python_info.platform_python_implementation(),
                 python_info.python_full_version()
-            )
+            );
         }
 
         if self.python_raw.is_empty() {
             self.python_raw = venv.stdlib_as_string();
         }
     }
 
     /// try to guess/deduce some values
     pub fn fill(
         &mut self,
         maybe_venv: Option<&PythonEnvironment>,
     ) -> Option<()> {
-        let _v: PythonEnvironment;
+        let environment: PythonEnvironment;
 
         if self.install_spec.is_empty() {
             self.install_spec = String::from(&self.name);
         }
 
         let venv = match maybe_venv {
             Some(v) => v,
             None => match uv_venv(None) {
-                Some(v) => {
+                Some(venv) => {
                     // black magic fuckery to
                     // get a reference to the currently active venv
-                    _v = v;
-                    &_v
+                    environment = venv;
+                    &environment
                 },
                 None => return None,
             },
         };
 
         self.fill_python(venv);
 
         Some(())
     }
 
     pub async fn for_dir(
         dirname: &Path,
         config: &LoadMetadataConfig,
-    ) -> Option<Metadata> {
+    ) -> Option<Self> {
         let meta_path = dirname.join(".metadata");
 
-        Metadata::for_file(&meta_path, config).await
+        Self::for_file(&meta_path, config).await
     }
 
     pub async fn for_requirement(
         requirement: &Requirement,
         config: &LoadMetadataConfig,
-    ) -> Metadata {
+    ) -> Self {
         let requirement_name = requirement.name.to_string();
         let venv_dir = venv_path(&requirement_name);
 
-        match Metadata::for_dir(&venv_dir, config).await {
-            Some(m) => m,
-            None => Metadata::find(requirement),
-        }
+        (Self::for_dir(&venv_dir, config).await)
+            .map_or_else(|| Self::find(requirement), |meta| meta)
     }
 
     pub async fn for_file(
         filename: &Path,
         config: &LoadMetadataConfig,
-    ) -> Option<Metadata> {
+    ) -> Option<Self> {
         let result = load_metadata(filename, config).await;
         result.ok()
     }
 
     pub async fn save(
         &self,
         dirname: &Path,
@@ -224,38 +222,49 @@
         }
     }
 
     pub async fn check_scripts(
         &mut self,
         venv_path: &Path,
     ) {
-        for (key, value) in self.scripts.iter_mut() {
+        for (key, value) in &mut self.scripts {
             *value = check_symlink(key, venv_path).await;
         }
     }
 
+    pub fn invalid_scripts(&self) -> Vec<String> {
+        let list: Vec<String> = self
+            .scripts
+            .iter()
+            //                                if True, the script is valid -> skip from filter_map
+            .filter_map(|(k, v)| if *v { None } else { Some(k.to_owned()) })
+            .collect();
+
+        list
+    }
+
     pub fn format_installed_version(&self) -> String {
         if self.outdated {
             self.installed_version.red().to_string()
         } else {
             self.installed_version.cyan().to_string()
         }
     }
 
     pub fn format_short(&self) -> String {
         format!("- {} {}", self.name, self.format_installed_version())
     }
 
     #[allow(dead_code)]
     pub fn vec_extras(&self) -> Vec<&str> {
-        self.extras.iter().map(|k| k.as_ref()).collect()
+        self.extras.iter().map(AsRef::as_ref).collect()
     }
 
     pub fn vec_injected(&self) -> Vec<&str> {
-        self.injected.iter().map(|k| k.as_ref()).collect()
+        self.injected.iter().map(AsRef::as_ref).collect()
     }
 
     pub fn format_extras(&self) -> String {
         self.extras
             .iter()
             .map(|k| format!("'{}'", k.green()))
             .join(",")
@@ -276,15 +285,15 @@
         }
 
         if !self.requested_version.is_empty() {
             result.push_str(&format!(" {}", self.requested_version.cyan()));
         }
 
         if self.editable {
-            result.push_str(&format!(" {}", "--editable".yellow()))
+            result.push_str(&format!(" {}", "--editable".yellow()));
         }
 
         result.push('\n');
 
         result.push_str(&format!(
             "{}Installed Version: {} on {}.\n",
             INDENT,
@@ -298,48 +307,45 @@
                 INDENT,
                 self.available_version.green(),
             ));
         }
 
         if !self.injected.is_empty() {
             let formatted_injects = self.format_injected();
-            result.push_str(&format!(
-                "{}Injected Packages: {}\n",
-                INDENT, formatted_injects
-            ));
+            result.push_str(&format!("{INDENT}Injected Packages: {formatted_injects}\n"));
         }
 
         let formatted_scripts = self
             .scripts
             .iter()
             .map(|(key, value)| {
                 if *value {
                     key.green().to_string()
                 } else {
                     key.red().to_string()
                 }
             })
             .join(" | ");
-        result.push_str(&format!("{}Scripts: {}", INDENT, formatted_scripts));
+        result.push_str(&format!("{INDENT}Scripts: {formatted_scripts}"));
 
         result
     }
 }
 
-/// Drop the MAGIC_HEADER from a buffer (if present)
+/// Drop the `MAGIC_HEADER` from a buffer (if present)
 pub fn strip_header(buf: &mut Vec<u8>) {
     // postponed: the current header is 7 chars long.
     //            the version should be ignored for starts_with,
     //            and if the length should change, this must be 'match'ed based on the version
     if buf.starts_with(MAGIC_HEADER) {
         let _ = buf.drain(0..MAGIC_HEADER.len());
     }
 }
 
-/// Prepend the MAGIC_HEADER to a buffer
+/// Prepend the `MAGIC_HEADER` to a buffer
 fn add_header(buf: &mut Vec<u8>) {
     let mut new_buf = Vec::with_capacity(MAGIC_HEADER.len() + buf.len());
     new_buf.extend_from_slice(MAGIC_HEADER);
     new_buf.append(buf);
     *buf = new_buf;
 }
 
@@ -368,43 +374,44 @@
 
     // Read the contents of the file into a Metadata struct
     let metadata: T = rmp_serde::decode::from_slice(&buf[..]).map_err_to_string()?;
 
     Ok(metadata)
 }
 
+#[allow(clippy::struct_excessive_bools)]
 pub struct LoadMetadataConfig {
     pub recheck_scripts: bool,
     pub updates_check: bool,
     pub updates_prereleases: bool,
     pub updates_ignore_constraints: bool,
 }
 
 impl LoadMetadataConfig {
     #[allow(dead_code)]
-    pub fn all() -> Self {
-        LoadMetadataConfig {
+    pub const fn all() -> Self {
+        Self {
             recheck_scripts: true,
             updates_check: true,
             updates_prereleases: true,
             updates_ignore_constraints: true,
         }
     }
 
-    pub fn none() -> Self {
-        LoadMetadataConfig {
+    pub const fn none() -> Self {
+        Self {
             recheck_scripts: false,
             updates_check: false,
             updates_prereleases: false,
             updates_ignore_constraints: false,
         }
     }
 
-    pub fn default() -> Self {
-        LoadMetadataConfig {
+    pub const fn default() -> Self {
+        Self {
             recheck_scripts: true,
             updates_check: true,
             updates_prereleases: false,
             updates_ignore_constraints: false,
         }
     }
 }
@@ -417,15 +424,15 @@
 
     let mut metadata: Metadata = load_generic_msgpack(filename, &mut buf).await?;
 
     if let Some(folder) = filename.parent() {
         // filename.parent should always be Some
 
         if config.recheck_scripts {
-            metadata.check_scripts(folder).await
+            metadata.check_scripts(folder).await;
         }
 
         if config.updates_check {
             metadata
                 .check_for_update(
                     config.updates_prereleases,
                     config.updates_ignore_constraints,
```

### Comparing `uvx-2.2.2/src/pip.rs` & `uvx-2.3.0/src/pip.rs`

 * *Files 14% similar despite different names*

```diff
@@ -105,26 +105,19 @@
 
     let Some(install) = pip_data.install.first() else {
         return Err(String::from(
             "Failed to find package name for local install.",
         ));
     };
 
-    // let empty_vec = Vec::new();
-    // let extras = match &install.requested_extras {
-    //     Some(extras) => extras,
-    //     None => &empty_vec,
-    // };
-
-    let full_name = match &install.requested_extras {
-        Some(extras) => {
-            format!("{}[{}]", &install.metadata.name, extras.join(","))
-        },
-        None => String::from(&install.metadata.name),
-    };
+    // if extras exist, the full name is name[extras]. Otherwise, it's just the name.
+    let full_name = install.requested_extras.as_ref().map_or_else(
+        || String::from(&install.metadata.name),
+        |extras| format!("{}[{}]", &install.metadata.name, extras.join(",")),
+    );
 
     let file_url = &install.download_info.url;
 
     Ok(FakeInstallResult {
         name: full_name,
         file_url: String::from(file_url),
     })
@@ -134,15 +127,15 @@
     install_spec: &str
 ) -> Result<(Requirement, String), String> {
     // fake install and extract the relevant info
     let promise = fake_install(install_spec);
 
     let result = show_loading_indicator(
         promise,
-        format!("Trying to install local package {}", install_spec),
+        format!("Trying to install local package {install_spec}"),
         AnimationSettings::default(),
     )
     .await?;
 
     let new_install_spec = result.to_spec();
     let requirement = Requirement::from_str(&new_install_spec).map_err_to_string()?;
```

### Comparing `uvx-2.2.2/src/pypi.rs` & `uvx-2.3.0/src/pypi.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 use pep440_rs::{Version, VersionSpecifier};
 use pep508_rs::{PackageName, Requirement};
 use rkyv::{de::deserializers::SharedDeserializeMap, Deserialize};
-use uv_client::{
-    RegistryClient, RegistryClientBuilder, SimpleMetadatum,
-};
+use uv_client::{RegistryClient, RegistryClientBuilder, SimpleMetadatum};
 
 use crate::pip::parse_requirement;
 use crate::uv::uv_cache;
 
-pub async fn get_client() -> Option<RegistryClient> {
+pub fn get_client() -> Option<RegistryClient> {
     let cache = uv_cache()?;
 
     Some(RegistryClientBuilder::new(cache).build())
 }
 
 pub fn deserialize_version(datum: &rkyv::Archived<Version>) -> Option<Version> {
     // for some reason, pycharm doesn't understand this type (but it compiles)
@@ -30,21 +28,21 @@
 pub async fn get_versions_for_packagename(
     package_name: &PackageName,
     stable: bool,
     constraint: Option<VersionSpecifier>,
 ) -> Vec<Version> {
     let mut versions: Vec<Version> = vec![];
 
-    let Some(client) = get_client().await else {
+    let Some(client) = get_client() else {
         return versions;
     };
 
     let data = match client.simple(package_name).await {
         Err(err) => {
-            eprintln!("Something went wrong: {}", err);
+            eprintln!("Something went wrong: {err}");
             return versions;
         },
         Ok(data) => data,
     };
 
     if let Some((_, metadata)) = data.iter().next_back() {
         versions = metadata
@@ -54,15 +52,15 @@
     }
 
     if stable {
         versions.retain(|version| !version.any_prerelease());
     }
 
     if let Some(specifier) = constraint {
-        versions.retain(|version| specifier.contains(version))
+        versions.retain(|version| specifier.contains(version));
     }
 
     versions
 }
 
 pub async fn get_latest_version_for_packagename(
     package_name: &PackageName,
@@ -71,15 +69,15 @@
 ) -> Option<Version> {
     let versions = get_versions_for_packagename(package_name, stable, constraint).await;
 
     versions.last().cloned()
 }
 #[allow(dead_code)]
 pub async fn get_pypi_data_for_packagename(package_name: &PackageName) -> Option<SimpleMetadatum> {
-    let client = get_client().await?;
+    let client = get_client()?;
 
     let data = client.simple(package_name).await.ok()?;
 
     if let Some((_, metadata)) = data.iter().next_back() {
         if let Some(latest) = metadata.iter().next_back() {
             return deserialize_metadata(latest);
         }
```

### Comparing `uvx-2.2.2/src/symlinks.rs` & `uvx-2.3.0/src/symlinks.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         .map_err(|err| format!("entry_points.txt is invalid: {err}"))?;
 
     let Some(console_scripts) = entry_points_mapping.get("console_scripts") else {
         return Ok(Vec::new());
     };
 
     // extract script keys
-    return Ok(console_scripts.keys().map(|k| k.to_string()).collect());
+    return Ok(console_scripts.keys().map(ToString::to_string).collect());
 }
 
 pub async fn find_symlinks(
     requirement: &Requirement,
     installed_version: &str,
     venv: &PythonEnvironment,
 ) -> Vec<String> {
@@ -38,19 +38,19 @@
         .interpreter()
         .purelib()
         .join(dist_info_fname)
         .join("entry_points.txt");
     let entrypoints_path = entrypoints_ini.to_str().unwrap_or_default();
     let scripts = console_scripts(entrypoints_path).await.unwrap_or_default();
 
-    if !scripts.is_empty() {
-        scripts
-    } else {
+    if scripts.is_empty() {
         // no scripts found, use requirement name as fallback (e.g. for `uv`)
         vec![requirement.name.to_string()]
+    } else {
+        scripts
     }
 }
 
 pub async fn create_symlink(
     symlink: &str,
     venv: &Path,
     force: bool,
@@ -63,28 +63,26 @@
     }
 
     let target_path = bin_dir.join(symlink);
 
     if target_path.exists() {
         if !force {
             return Err(format!(
-                "Script {} already exists in {:?}. Use --force to ignore this warning.",
-                symlink, bin_dir
+                "Script {symlink} already exists in {bin_dir:?}. Use --force to ignore this warning.",
             ));
         }
         tokio::fs::remove_file(&target_path)
             .await
             .map_err(|_| format!("Failed to create symlink {:?}", &target_path))?;
     }
 
     let symlink_path = venv.join("bin").join(symlink);
     if !symlink_path.exists() {
         return Err(format!(
-            "Could not symlink {:?} because the script didn't exist.",
-            symlink_path
+            "Could not symlink {symlink_path:?} because the script didn't exist.",
         ));
     }
 
     tokio::fs::symlink(&symlink_path, &target_path)
         .await
         .map_err(|_| format!("Failed to create symlink {:?}", &target_path))?;
```

### Comparing `uvx-2.2.2/src/uv.rs` & `uvx-2.3.0/src/uv.rs`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     // let Some(binary) = env::args().nth(0) else {
     //     return None;
     // };
     // let Ok(binary_path) = PathBuf::from_str(&binary) else {
     //     return None;
     // };
 
-    find_sibling("uv").await.map(|buf| buf.to_string())
+    find_sibling("uv").await.map(PathToString::to_string)
 }
 
 pub async fn get_uv_binary() -> String {
     _get_uv_binary().await.unwrap_or_else(
         // fallback, hope 'uv' is available in global scope:
         || String::from("uv"),
     )
@@ -38,53 +38,50 @@
 where
     S: AsRef<OsStr>,
 {
     // venv could be unavailable, use 'uv' from this library's requirement
     let script = get_uv_binary().await;
 
     let subcommand = &args[0].as_ref().to_str().unwrap_or_default(); // cursed but makes it work with both &str and String
-    let err_prefix = format!("uv {}", subcommand);
+    let err_prefix = format!("uv {subcommand}");
 
     run(&script, args, Some(err_prefix)).await
 }
 
 pub async fn uv_with_output<S: AsRef<OsStr>>(args: Vec<S>) -> Result<i32, String> {
     let script = get_uv_binary().await;
     run_print_output(script, args).await
 }
 
 pub fn uv_cache() -> Option<Cache> {
-    if let Some(project_dirs) = ProjectDirs::from("", "", "uv") {
-        Cache::from_path(project_dirs.cache_dir())
-    } else {
-        Cache::from_path(".uv_cache")
-    }
-    .ok()
+    ProjectDirs::from("", "", "uv")
+        .map_or_else(
+            || Cache::from_path(".uv_cache"),
+            |project_dirs| Cache::from_path(project_dirs.cache_dir()),
+        )
+        .ok()
 }
 
 pub fn uv_venv(maybe_cache: Option<Cache>) -> Option<PythonEnvironment> {
-    if let Some(cache) = maybe_cache.or_else(uv_cache) {
-        PythonEnvironment::from_virtualenv(&cache).ok()
-    } else {
-        None
-    }
+    maybe_cache
+        .or_else(uv_cache)
+        .and_then(|cache| PythonEnvironment::from_virtualenv(&cache).ok())
 }
 
 pub fn uv_get_installed_version(
     package_name: &PackageName,
     maybe_venv: Option<&PythonEnvironment>,
 ) -> Result<String, String> {
-    let _venv: PythonEnvironment; // lifetime for if maybe_venv is None
+    let environment: PythonEnvironment; // lifetime for if maybe_venv is None
 
-    let site_packages = match maybe_venv {
-        Some(venv) => SitePackages::from_executable(venv),
-        None => {
-            _venv = uv_venv(None).ok_or_else(|| format!("{}", "Failed to set up venv!".red()))?;
-            SitePackages::from_executable(&_venv)
-        },
+    let site_packages = if let Some(venv) = maybe_venv {
+        SitePackages::from_executable(venv)
+    } else {
+        environment = uv_venv(None).ok_or_else(|| format!("{}", "Failed to set up venv!".red()))?;
+        SitePackages::from_executable(&environment)
     }
     .ok();
 
     if let Some(pkgs) = site_packages {
         // for result in pkgs.get_packages(package_name) {
         if let Some(result) = pkgs.get_packages(package_name).into_iter().next() {
             return Ok(result.version().to_string());
@@ -100,15 +97,15 @@
 pub trait Helpers {
     fn to_path_buf(&self) -> PathBuf;
     fn stdlib_as_string(&self) -> String;
 }
 
 impl Helpers for PythonEnvironment {
     fn to_path_buf(&self) -> PathBuf {
-        return self.root().to_path_buf();
+        self.root().to_path_buf()
     }
 
     fn stdlib_as_string(&self) -> String {
         let stdlib = self.interpreter().stdlib().to_str();
         stdlib.unwrap_or_default().to_string()
     }
 }
@@ -123,10 +120,10 @@
         match self.version_or_url.clone() {
             Some(pep508_rs::VersionOrUrl::VersionSpecifier(v)) => v.to_string(),
             _ => String::new(),
         }
     }
 
     fn extras(&self) -> HashSet<String> {
-        self.extras.iter().map(|extra| extra.to_string()).collect()
+        self.extras.iter().map(ToString::to_string).collect()
     }
 }
```

### Comparing `uvx-2.2.2/src/venv.rs` & `uvx-2.3.0/src/venv.rs`

 * *Files 3% similar despite different names*

```diff
@@ -39,29 +39,29 @@
 pub async fn create_venv(
     package_name: &PackageName,
     python: Option<&String>,
     force: bool,
     with_pip: bool,
     custom_prefix: Option<String>,
 ) -> Result<PathBuf, String> {
-    let venv_path = match custom_prefix {
-        None => venv_path(package_name.as_ref()),
-        Some(prefix) => PathBuf::from(format!("{}{}", prefix, package_name)),
-    };
+    let venv_path = custom_prefix.map_or_else(
+        || venv_path(package_name.as_ref()),
+        |prefix| PathBuf::from(format!("{prefix}{package_name}")),
+    );
 
     create_venv_raw(&venv_path, python, force, with_pip).await?;
 
     Ok(venv_path)
 }
 
 pub async fn activate_venv(venv: &Path) -> Result<PythonEnvironment, String> {
     let venv_str = venv.to_str().unwrap_or_default();
     std::env::set_var("VIRTUAL_ENV", venv_str);
 
-    uv_venv(None).ok_or_else(|| format!("Could not properly activate venv '{}'!", venv_str))
+    uv_venv(None).ok_or_else(|| format!("Could not properly activate venv '{venv_str}'!"))
 }
 
 #[allow(dead_code)]
 pub async fn find_venv(install_spec: &str) -> Option<PathBuf> {
     let (requirement, _) = parse_requirement(install_spec).await.ok()?;
     let requirement_name = requirement.name.to_string();
```

### Comparing `uvx-2.2.2/pyproject.toml` & `uvx-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.2.2/PKG-INFO` & `uvx-2.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.2.2
+Version: 2.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
 Requires-Dist: patchelf
 Summary: uvx: pipx for uv (🦀)
 Keywords: 
 Author-email: Robin van der Noord <robinvandernoord@gmail.com>
 License: MIT
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/robinvandernoord/uvx2
 
 # uvx: pipx for uv
 
 Inspired by:
 
 - [pipx](https://github.com/pypa/pipx)
 - [uv](https://github.com/astral-sh/uv)
```

