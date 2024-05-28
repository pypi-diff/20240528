# Comparing `tmp/md_ulb_pwrap-0.1.0.tar.gz` & `tmp/md_ulb_pwrap-0.1.1.tar.gz`

## Comparing `md_ulb_pwrap-0.1.0.tar` & `md_ulb_pwrap-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 md_ulb_pwrap-0.1.0/local_dependencies/md-ulb-pwrap/Cargo.toml
--rw-r--r--   0     1001      123     7020 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/local_dependencies/md-ulb-pwrap/src/lib.rs
--rw-r--r--   0     1001      123     3594 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/local_dependencies/md-ulb-pwrap/src/parser.rs
--rw-r--r--   0     1001      123     7293 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/local_dependencies/md-ulb-pwrap/src/pwrap.rs
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 md_ulb_pwrap-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123       26 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/dev-requirements.txt
--rw-r--r--   0     1001      123      320 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      486 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     1819 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/test.py
--rw-r--r--   0     1001      123    10008 2023-08-10 06:50:54.000000 md_ulb_pwrap-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1948 1970-01-01 00:00:00.000000 md_ulb_pwrap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      286 1970-01-01 00:00:00.000000 md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/Cargo.toml
+-rw-r--r--   0     1001      127     1393 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/README.md
+-rw-r--r--   0     1001      127      753 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/README.tpl
+-rw-r--r--   0     1001      127     7624 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/src/lib.rs
+-rw-r--r--   0     1001      127     3569 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/src/parser.rs
+-rw-r--r--   0     1001      127     7185 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/src/pwrap.rs
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 md_ulb_pwrap-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      127     1394 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/README.md
+-rw-r--r--   0     1001      127      754 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/README.tpl
+-rw-r--r--   0     1001      127       26 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/dev-requirements.txt
+-rw-r--r--   0     1001      127      320 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      127      493 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      127     1819 2024-05-28 20:33:53.000000 md_ulb_pwrap-0.1.1/test.py
+-rw-r--r--   0        0        0    14062 2024-05-28 20:34:38.000000 md_ulb_pwrap-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 md_ulb_pwrap-0.1.1/PKG-INFO
```

### Comparing `md_ulb_pwrap-0.1.0/local_dependencies/md-ulb-pwrap/src/lib.rs` & `md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+//! [![Crate](https://img.shields.io/crates/v/md-ulb-pwrap?logo=rust)](https://crates.io/crates/md-ulb-pwrap) [![PyPI](https://img.shields.io/pypi/v/md-ulb-pwrap?logo=python&logoColor=white)](https://pypi.org/project/md-ulb-pwrap/)
+//!
+//! Markdown paragraph wrapper using [Unicode Line Breaking
+//! Algorithm].
+//!
+//! Wrap a Markdown paragraph using a maximum desired width.
+//! Only works for paragraphs that don't contain other
+//! [container blocks]. Respects the prohibition against wrapping
+//! text inside inline code blocks and links.
+//!
+//! [unicode line breaking algorithm]: https://unicode.org/reports/tr14/
+//! [container blocks]: https://spec.commonmark.org/0.30/#container-blocks
+
 mod parser;
 pub mod pwrap;
 
 use crate::pwrap::MarkdownParagraphWrapper;
 
-pub fn ulb_wrap_paragraph(
-        text: &str,
-        width: usize,
-        first_line_width: usize,
-) -> String {
-    MarkdownParagraphWrapper::new(
-        text,
-        first_line_width,
-    ).wrap(width)
+pub fn ulb_wrap_paragraph(text: &str, width: usize, first_line_width: usize) -> String {
+    MarkdownParagraphWrapper::new(text, first_line_width).wrap(width)
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use rstest::rstest;
 
@@ -317,15 +323,11 @@
         concat!(
             "支持常见的温度传感器（例\n如，常见的热敏电阻、\n",
             "AD595、\nAD597、\nAD849x、\nPT100、\nPT1000、\n",
             "MAX6675、\nMAX31855、\nMAX31856、\nMAX31865、\n",
             "BME280、\nHTU21D和\nLM75）。还可以配\n置",
         ).to_string(),
     )]
-    fn ulb_wrap_paragraph_test(
-            #[case] text: &str,
-            #[case] width: usize,
-            #[case] expected: String,
-    ) {
+    fn ulb_wrap_paragraph_test(#[case] text: &str, #[case] width: usize, #[case] expected: String) {
         assert_eq!(ulb_wrap_paragraph(text, width, width), expected);
     }
 }
```

### Comparing `md_ulb_pwrap-0.1.0/local_dependencies/md-ulb-pwrap/src/parser.rs` & `md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/src/parser.rs`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,16 @@
             if character == '`' {
                 self.context <<= 1;
                 self.current_codespan_number_of_backticks_inside += 1;
             }
         } else if self.context & EXITING_CODESPAN != 0 {
             if character == '`' {
                 self.current_codespan_number_of_backticks_inside += 1;
-            } else if 
-                    self.current_codespan_number_of_backticks_inside
-                    == self.current_codespan_number_of_backticks_at_start
+            } else if self.current_codespan_number_of_backticks_inside
+                == self.current_codespan_number_of_backticks_at_start
             {
                 self.context = INSIDE_TEXT;
                 self.current_codespan_number_of_backticks_at_start = 0;
                 self.current_codespan_number_of_backticks_inside = 0;
             } else {
                 self.context = INSIDE_CODESPAN;
                 self.current_codespan_number_of_backticks_inside = 0;
```

### Comparing `md_ulb_pwrap-0.1.0/local_dependencies/md-ulb-pwrap/src/pwrap.rs` & `md_ulb_pwrap-0.1.1/local_dependencies/md-ulb-pwrap/src/pwrap.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     next_linebreak: (usize, BreakOpportunity),
     last_linebreak_i: usize,
     current_line: String,
 }
 
 impl MarkdownParagraphWrapper {
     pub fn new(text: &str, first_line_width: usize) -> Self {
-        let linebreaks = linebreaks(text)
-            .collect::<Vec<(usize, BreakOpportunity)>>();
+        let linebreaks = linebreaks(text).collect::<Vec<(usize, BreakOpportunity)>>();
         let linebreaks_length = linebreaks.len();
         let mut wrapper = MarkdownParagraphWrapper {
             width: first_line_width,
 
             characters: text.char_indices().enumerate().collect(),
             characters_i: 0,
             linebreaks,
@@ -43,18 +42,15 @@
             last_linebreak_i: 0,
             current_line: String::new(),
         };
         wrapper.update_next_linebreak();
         wrapper
     }
 
-    fn is_linebreak_possible(
-            &mut self,
-            linebreak: (usize, BreakOpportunity),
-    ) -> bool {
+    fn is_linebreak_possible(&mut self, linebreak: (usize, BreakOpportunity)) -> bool {
         let mut bindex = linebreak.0 - 1;
         let mut character: char;
         loop {
             if self.codespan_parser.characters_i >= self.last_character_i {
                 // reached end of text
                 //
                 // In cases where the last character has more than
@@ -62,37 +58,35 @@
                 // last linebreak (mandatory) is not
                 // detected because at this point we are before
                 // the break, so keep updating the bindex until
                 // the one of the break is reached
                 bindex += 1;
                 character = '\0';
             } else {
-                let (_, (bindex_, character_)) = self.characters[
-                    self.codespan_parser.characters_i
-                ];
+                let (_, (bindex_, character_)) = self.characters[self.codespan_parser.characters_i];
                 bindex = bindex_;
                 character = character_;
             }
 
             if bindex != linebreak.0 {
                 self.codespan_parser.parse_character(character);
                 continue;
             }
 
             // reached next linebreak index
             if linebreak.1 == Mandatory {
                 // is inside text?
                 return self.codespan_parser.is_inside_text();
             } else if self.codespan_parser.is_inside_text() {
-                let (_, (_, prev_character)) = self.characters[
-                    self.codespan_parser.characters_i - 1
-                ];
+                let (_, (_, prev_character)) =
+                    self.characters[self.codespan_parser.characters_i - 1];
 
-                if is_link_breaking_character(character) ||
-                        is_link_breaking_character(prev_character) {
+                if is_link_breaking_character(character)
+                    || is_link_breaking_character(prev_character)
+                {
                     break;
                 }
                 self.codespan_parser.backup_state();
                 self.codespan_parser.parse_character(character);
                 let result = self.codespan_parser.is_inside_link();
                 self.codespan_parser.restore_state();
                 return result;
@@ -117,22 +111,19 @@
                 break;
             }
 
             // Get next linebreak index to see if we
             // can fit more text in the line
             while self.linebreaks_i < self.linebreaks_length {
                 let current_line_width =
-                    self.get_next_linebreak_index()
-                    - self.last_linebreak_i - 1;
+                    self.get_next_linebreak_index() - self.last_linebreak_i - 1;
                 if current_line_width > self.width {
                     break;
                 }
-                self.next_linebreak = self.linebreaks[
-                    self.linebreaks_i
-                ];
+                self.next_linebreak = self.linebreaks[self.linebreaks_i];
                 self.linebreaks_i += 1;
             }
             break;
         }
     }
 
     fn get_next_linebreak_index(&mut self) -> usize {
@@ -154,28 +145,29 @@
         self.codespan_parser.restore_state();
 
         result
     }
 
     pub fn wrap(&mut self, width: usize) -> String {
         let mut result = String::new();
-        let first_line = self.next().unwrap_or(String::new());
+        let first_line = self.next().unwrap_or_default();
         result.push_str(&first_line);
         self.width = width;
         for line in self {
             result.push_str(&line);
         }
         result
     }
 }
 
 impl Iterator for MarkdownParagraphWrapper {
     type Item = String;
 
     fn next(&mut self) -> Option<Self::Item> {
+        #[allow(clippy::comparison_chain)]
         if self.characters_i == self.last_character_i {
             self.characters_i += 1;
             //
             // The last character have been processed
             //
             // unicode-linebreak always include a mandatory
             // linebreak at the end of the string, so we
```

### Comparing `md_ulb_pwrap-0.1.0/test.py` & `md_ulb_pwrap-0.1.1/test.py`

 * *Files identical despite different names*

### Comparing `md_ulb_pwrap-0.1.0/Cargo.lock` & `md_ulb_pwrap-0.1.1/Cargo.lock`

 * *Files 18% similar despite different names*

```diff
@@ -1,375 +1,526 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "ahash"
-version = "0.7.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
-dependencies = [
- "getrandom",
- "once_cell",
- "version_check",
-]
-
-[[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "getrandom"
-version = "0.2.8"
+name = "futures"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
- "cfg-if",
- "libc",
- "wasi",
+ "futures-channel",
+ "futures-core",
+ "futures-executor",
+ "futures-io",
+ "futures-sink",
+ "futures-task",
+ "futures-util",
 ]
 
 [[package]]
-name = "hashbrown"
-version = "0.12.3"
+name = "futures-channel"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+]
+
+[[package]]
+name = "futures-core"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
+
+[[package]]
+name = "futures-executor"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
- "ahash",
+ "futures-core",
+ "futures-task",
+ "futures-util",
 ]
 
 [[package]]
+name = "futures-io"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
+
+[[package]]
+name = "futures-macro"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
+name = "futures-sink"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
+
+[[package]]
+name = "futures-task"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
+
+[[package]]
+name = "futures-timer"
+version = "3.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f288b0a4f20f9a56b5d1da57e2227c661b7b16168e2f72365f57b63326e29b24"
+
+[[package]]
+name = "futures-util"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
+dependencies = [
+ "futures-channel",
+ "futures-core",
+ "futures-io",
+ "futures-macro",
+ "futures-sink",
+ "futures-task",
+ "memchr",
+ "pin-project-lite",
+ "pin-utils",
+ "slab",
+]
+
+[[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "md-ulb-pwrap"
-version = "0.0.3"
+version = "0.1.1"
 dependencies = [
+ "rstest",
  "unicode-linebreak",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
+name = "pin-project-lite"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
+
+[[package]]
+name = "pin-utils"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-md-ulb-pwrap"
-version = "0.0.3"
+version = "0.1.1"
 dependencies = [
  "md-ulb-pwrap",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.1"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "48aaa5748ba571fb95cd2c85c09f629215d3a6ece942baa100950af03a34f733"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
-name = "scopeguard"
-version = "1.1.0"
+name = "relative-path"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "ba39f3699c378cd8970968dcbff9c43159ea4cfbd88d43c00b22f2ef10a435d2"
 
 [[package]]
-name = "smallvec"
-version = "1.10.0"
+name = "rstest"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "9d5316d2a1479eeef1ea21e7f9ddc67c191d497abc8fc3ba2467857abbb68330"
+dependencies = [
+ "futures",
+ "futures-timer",
+ "rstest_macros",
+ "rustc_version",
+]
 
 [[package]]
-name = "syn"
-version = "1.0.107"
+name = "rstest_macros"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "04a9df72cc1f67020b0d63ad9bfe4a323e459ea7eb68e03bd9824db49f9a4c25"
 dependencies = [
+ "cfg-if",
+ "glob",
  "proc-macro2",
  "quote",
+ "regex",
+ "relative-path",
+ "rustc_version",
+ "syn",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.6"
+name = "rustc_version"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver",
+]
 
 [[package]]
-name = "unicode-ident"
-version = "1.0.6"
+name = "scopeguard"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "unicode-linebreak"
-version = "0.1.4"
+name = "semver"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5faade31a542b8b35855fff6e8def199853b2da8da256da52f52f1316ee3137"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
+
+[[package]]
+name = "slab"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
- "hashbrown",
- "regex",
+ "autocfg",
 ]
 
 [[package]]
-name = "unindent"
-version = "0.1.11"
+name = "smallvec"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
-name = "version_check"
-version = "0.9.4"
+name = "syn"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
-name = "wasi"
-version = "0.11.0+wasi-snapshot-preview1"
+name = "target-lexicon"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
-name = "windows-sys"
-version = "0.45.0"
+name = "unicode-ident"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
+
+[[package]]
+name = "unicode-linebreak"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b09c83c3c29d37506a3e260c08c03743a6bb66a9cd432c6934ab501a190571f"
+
+[[package]]
+name = "unindent"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e2522491fbfcd58cc84d47aeb2958948c4b8982e9a2d8a2a35bbaed431390e7"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `md_ulb_pwrap-0.1.0/PKG-INFO` & `md_ulb_pwrap-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,38 @@
 Metadata-Version: 2.1
 Name: md-ulb-pwrap
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python bindings for Rust crate md-ulb-pwrap.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # md-ulb-pwrap
 
+<!-- This file has been autogenerated.
+To update it, change the content of `rust/src/lib.rs`
+and run `pre-commit run -a cargo-readme`
+-->
+
 [![Crate](https://img.shields.io/crates/v/md-ulb-pwrap?logo=rust)](https://crates.io/crates/md-ulb-pwrap) [![PyPI](https://img.shields.io/pypi/v/md-ulb-pwrap?logo=python&logoColor=white)](https://pypi.org/project/md-ulb-pwrap/)
 
 Markdown paragraph wrapper using [Unicode Line Breaking
-Algorithm]. Includes a Rust library with Python bindings.
+Algorithm].
 
 Wrap a Markdown paragraph using a maximum desired width.
 Only works for paragraphs that don't contain other
 [container blocks]. Respects the prohibition against wrapping
 text inside inline code blocks and links.
 
-## Rust library
-
-```bash
-cargo add md-ulb-pwrap
-```
-
-````rust
-use md_ulb_pwrap::ulb_wrap_paragraph;
-
-assert_eq!(
-    ulb_wrap_paragraph(
-        &"aaa ``` ``  ` a b c ``` ccc",
-        3,
-        3,
-    ),
-    "aaa\n``` ``  ` a b c ```\nccc",
-);
-````
+[unicode line breaking algorithm]: https://unicode.org/reports/tr14/
+[container blocks]: https://spec.commonmark.org/0.30/#container-blocks
 
-## Python bindings
+## Usage
 
 ```bash
 pip install md-ulb-pwrap
 ```
 
 ````python
 from md_ulb_pwrap import ulb_wrap_paragraph
@@ -59,10 +48,7 @@
 
 - **text** (_str_): The text to wrap.
 - **width** (_int_): The maximum width of the lines after the first.
 - **first_line_width** (_int_): The maximum width of the first line.
 
 **Returns** (_str_): The wrapped text.
 
-[unicode line breaking algorithm]: https://unicode.org/reports/tr14/
-[container blocks]: https://spec.commonmark.org/0.30/#container-blocks
-
```

