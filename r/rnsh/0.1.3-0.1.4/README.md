# Comparing `tmp/rnsh-0.1.3.tar.gz` & `tmp/rnsh-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnsh-0.1.3.tar", max compression
+gzip compressed data, was "rnsh-0.1.4.tar", max compression
```

## Comparing `rnsh-0.1.3.tar` & `rnsh-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.1.3/LICENSE
--rw-r--r--   0        0        0    12702 2023-12-17 19:17:26.972211 rnsh-0.1.3/README.md
--rw-r--r--   0        0        0      800 2023-12-17 19:10:26.006971 rnsh-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1708 2023-05-11 18:54:53.778369 rnsh-0.1.3/rnsh/__init__.py
--rw-r--r--   0        0        0     6200 2023-10-27 22:07:37.666520 rnsh-0.1.3/rnsh/args.py
--rw-r--r--   0        0        0      798 2023-02-17 16:48:38.181439 rnsh-0.1.3/rnsh/exception.py
--rw-r--r--   0        0        0      817 2023-02-19 00:35:54.411700 rnsh-0.1.3/rnsh/helpers.py
--rw-r--r--   0        0        0    19702 2023-12-17 19:10:26.006971 rnsh-0.1.3/rnsh/initiator.py
--rw-r--r--   0        0        0     8813 2023-09-24 18:37:07.705158 rnsh-0.1.3/rnsh/listener.py
--rw-r--r--   0        0        0      644 2023-02-23 12:37:08.623322 rnsh-0.1.3/rnsh/loop.py
--rw-r--r--   0        0        0    25969 2023-12-17 19:10:26.006971 rnsh-0.1.3/rnsh/process.py
--rw-r--r--   0        0        0     4206 2023-03-08 22:54:16.949580 rnsh-0.1.3/rnsh/protocol.py
--rw-r--r--   0        0        0     7661 2023-02-18 06:09:41.069929 rnsh-0.1.3/rnsh/retry.py
--rw-r--r--   0        0        0     6172 2023-09-24 18:37:07.709158 rnsh-0.1.3/rnsh/rnsh.py
--rw-r--r--   0        0        0     5225 2023-02-18 14:10:38.940197 rnsh-0.1.3/rnsh/rnslogging.py
--rw-r--r--   0        0        0    16792 2023-12-17 19:10:26.010971 rnsh-0.1.3/rnsh/session.py
--rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.1.3/rnsh/testlogging.py
--rw-r--r--   0        0        0    13421 1970-01-01 00:00:00.000000 rnsh-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-02-11 05:21:53.643929 rnsh-0.1.4/LICENSE
+-rw-r--r--   0        0        0    12824 2024-05-21 19:14:57.488472 rnsh-0.1.4/README.md
+-rw-r--r--   0        0        0      642 2024-05-11 11:45:15.150759 rnsh-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1940 2024-05-11 11:45:15.150759 rnsh-0.1.4/rnsh/__init__.py
+-rw-r--r--   0        0        0     6210 2024-05-11 11:45:15.150759 rnsh-0.1.4/rnsh/args.py
+-rw-r--r--   0        0        0    16594 2024-05-11 11:45:15.150759 rnsh-0.1.4/rnsh/docopt.py
+-rw-r--r--   0        0        0      798 2023-02-17 16:48:38.181439 rnsh-0.1.4/rnsh/exception.py
+-rw-r--r--   0        0        0      817 2023-02-19 00:35:54.411700 rnsh-0.1.4/rnsh/helpers.py
+-rw-r--r--   0        0        0    19954 2024-05-11 11:45:15.150759 rnsh-0.1.4/rnsh/initiator.py
+-rw-r--r--   0        0        0     8813 2023-09-24 18:37:07.705158 rnsh-0.1.4/rnsh/listener.py
+-rw-r--r--   0        0        0      644 2023-02-23 12:37:08.623322 rnsh-0.1.4/rnsh/loop.py
+-rw-r--r--   0        0        0    25970 2024-05-11 11:45:15.150759 rnsh-0.1.4/rnsh/process.py
+-rw-r--r--   0        0        0     4206 2023-03-08 22:54:16.949580 rnsh-0.1.4/rnsh/protocol.py
+-rw-r--r--   0        0        0     7661 2023-02-18 06:09:41.069929 rnsh-0.1.4/rnsh/retry.py
+-rw-r--r--   0        0        0     6172 2023-09-24 18:37:07.709158 rnsh-0.1.4/rnsh/rnsh.py
+-rw-r--r--   0        0        0     5225 2023-02-18 14:10:38.940197 rnsh-0.1.4/rnsh/rnslogging.py
+-rw-r--r--   0        0        0    16792 2023-12-17 19:10:26.010971 rnsh-0.1.4/rnsh/session.py
+-rw-r--r--   0        0        0     1609 2023-02-11 14:06:05.513301 rnsh-0.1.4/rnsh/testlogging.py
+-rw-r--r--   0        0        0    13466 1970-01-01 00:00:00.000000 rnsh-0.1.4/PKG-INFO
```

### Comparing `rnsh-0.1.3/LICENSE` & `rnsh-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/README.md` & `rnsh-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
 ### Reminder: Beta Software
 The interface is starting to firm up, but some bug fixes at this
 point still may introduce breaking changes, especially in the
 protocol layers of the software.
 
 ## Recent Changes
+### v0.1.4
+- Fix invalid escape sequence handling for terminal escape sequences
+
 ### v0.1.3
 - Fix an issue where disconnecting a session using ~. would result in further connections to
   the same initiator would appear to hang.
 - Setting `-q` will suppress the pre-connect spinners
 
 ### v0.1.2
 - Adaptive compression (RNS update) provides significant performance improvements ([PR](https://github.com/acehoss/rnsh/pull/24))
@@ -283,21 +286,23 @@
   piping the output of `tar` over `rsh`.~~
 - [X] ~~Test on several platforms~~
 - [X] ~~Fix issues that come up with testing~~
 - [X] ~~v0.1.0 beta~~
 - [X] ~~Test and fix more issues~~
 - [ ] More betas
 - [ ] Enhancement Ideas
-  - [ ] `authorized_keys` mode similar to SSH to allow one listener
+  - [x] `authorized_keys` mode similar to SSH to allow one listener
         process to serve multiple users
   - [ ] Git over `rnsh` (git remote helper)
   - [ ] Sliding window acknowledgements for improved throughput
 - [ ] v1.0 someday probably maybe
 
 ## Miscellaneous
 
 By piping into/out of `rnsh`, it is possible to transfer
 files using the same method discussed in 
 [this article](https://cromwell-intl.com/open-source/tar-and-ssh.html).
 It's not terribly fast currently, due to the round-trip rule 
 enforced by the protocol. Sliding window acknowledgements will
 speed this up significantly.
+
+Running tests: `poetry run pytest tests`
```

### Comparing `rnsh-0.1.3/pyproject.toml` & `rnsh-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 [tool.poetry]
 name = "rnsh"
-version = "0.1.3"
+version = "0.1.4"
 description = "Shell over Reticulum"
 authors = ["acehoss <acehoss@acehoss.net>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-docopt = "^0.6.2"
-rns = ">=0.5.9"
-# rns = { git = "https://github.com/acehoss/Reticulum.git", branch = "feature/channel" }
-# rns = { path = "../Reticulum/", develop = true }
-tomli = "^2.0.1"
+rns = ">=0.7.4"
 
 [tool.poetry.scripts]
 rnsh = 'rnsh.rnsh:rnsh_cli'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 setuptools = "^67.2.0"
 pytest-asyncio = "^0.20.3"
 safety = "^2.3.5"
+tomli = "^2.0.1"
 
 [tool.pytest.ini_options]
 markers = [
     "skip_ci: marks tests that should not be run in CI builds (deselect with '-m \"not skip_ci\"')"
 ]
 
 [build-system]
```

### Comparing `rnsh-0.1.3/rnsh/__init__.py` & `rnsh-0.1.4/rnsh/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,25 +19,33 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 module_abs_filename = os.path.abspath(__file__)
 module_dir = os.path.dirname(module_abs_filename)
-# print(os.path.dirname(module_dir))
 
 def _get_version():
+    def pkg_res_version():
+        import pkg_resources
+        return pkg_resources.get_distribution("rnsh").version
+
+    def tomli_version():
+        import tomli
+        return tomli.load(open(os.path.join(os.path.dirname(module_dir), "pyproject.toml"), "rb"))["tool"]["poetry"]["version"]
+
     try:
-        try:
-            import tomli
-            return tomli.load(open(os.path.join(os.path.dirname(module_dir), "pyproject.toml"), "rb"))["tool"]["poetry"]["version"]
-        except:
+        if (os.path.isfile(os.path.join(os.path.dirname(module_dir), "pyproject.toml"))):
             try:
-                import pkg_resources
-                return pkg_resources.get_distribution("rnsh").version
+                return tomli_version()
             except:
                 return "0.0.0"
-
+        else:
+            try:
+                return pkg_res_version()
+            except:
+                return "0.0.0"
+                
     except:
         return "0.0.0"
 
 __version__ = _get_version()
```

### Comparing `rnsh-0.1.3/rnsh/args.py` & `rnsh-0.1.4/rnsh/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TypeVar
 import RNS
 import rnsh
-import docopt
 import sys
+from rnsh import docopt
 
 _T = TypeVar("_T")
 
 
 def _split_array_at(arr: [_T], at: _T) -> ([_T], [_T]):
     try:
         idx = arr.index(at)
```

### Comparing `rnsh-0.1.3/rnsh/exception.py` & `rnsh-0.1.4/rnsh/exception.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/helpers.py` & `rnsh-0.1.4/rnsh/helpers.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/initiator.py` & `rnsh-0.1.4/rnsh/initiator.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,33 +279,34 @@
         pre_esc = True
         line_mode = False
         line_flush = False
         blind_write_count = 0
         flush_chars = ["\x01", "\x03", "\x04", "\x05", "\x0c", "\x11", "\x13", "\x15", "\x19", "\t", "\x1A", "\x1B"]
         def handle_escape(b):
             nonlocal line_mode
-            if b == "~":
-                return "~"
-            elif b == "?":
+            if b == "?":
                 os.write(1, "\n\r\n\rSupported rnsh escape sequences:".encode("utf-8"))
                 os.write(1, "\n\r  ~~  Send the escape character by typing it twice".encode("utf-8"))
                 os.write(1, "\n\r  ~.  Terminate session and exit immediately".encode("utf-8"))
                 os.write(1, "\n\r  ~L  Toggle line-interactive mode".encode("utf-8"))
                 os.write(1, "\n\r  ~?  Display this quick reference\n\r".encode("utf-8"))
                 os.write(1, "\n\r(Escape sequences are only recognized immediately after newline)\n\r".encode("utf-8"))
+                return None
             elif b == ".":
                 _link.teardown()
+                return None
             elif b == "L":
                 line_mode = not line_mode
                 if line_mode:
                     os.write(1, "\n\rLine-interactive mode enabled\n\r".encode("utf-8"))
                 else:
                     os.write(1, "\n\rLine-interactive mode disabled\n\r".encode("utf-8"))
-            
-            return None
+                return None
+
+            return b
 
         stdin_eof = False
         def stdin():
             nonlocal stdin_eof, pre_esc, esc, line_mode
             nonlocal line_flush, blind_write_count
             try:
                 in_data = process.tty_read(sys.stdin.fileno())
@@ -314,30 +315,35 @@
                     for b in bytes(in_data):
                         c = chr(b)
                         if c == "\r":
                             pre_esc = True
                             line_flush = True
                             data.append(b)
                         elif line_mode and c in flush_chars:
+                            pre_esc = False
                             line_flush = True
                             data.append(b)
                         elif line_mode and (c == "\b" or c == "\x7f"):
+                            pre_esc = False
                             if len(line_buffer)>0:
                                 line_buffer.pop(-1)
                                 blind_write_count -= 1
                                 os.write(1, "\b \b".encode("utf-8"))
                         elif pre_esc == True and c == "~":
                             pre_esc = False
                             esc = True
                         elif esc == True:
                             ret = handle_escape(c)
                             if ret != None:
+                                if ret != "~":
+                                    data.append(ord("~"))
                                 data.append(ord(ret))
                             esc = False
                         else:
+                            pre_esc = False
                             data.append(b)
 
                     if not line_mode:
                         data_buffer.extend(data)
                     else:
                         line_buffer.extend(data)
                         if line_flush:
```

### Comparing `rnsh-0.1.3/rnsh/listener.py` & `rnsh-0.1.4/rnsh/listener.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/loop.py` & `rnsh-0.1.4/rnsh/loop.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/process.py` & `rnsh-0.1.4/rnsh/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             if e.errno != errno.EIO and e.errno != errno.EWOULDBLOCK:
                 raise
             elif e.errno == errno.EIO:
                 raise EOFError
     except EOFError:
         raise
     except Exception as ex:
-        module_logger.error("tty_read error: {ex}")
+        module_logger.error(f"tty_read error: {ex}")
     return result
 
 
 def fd_is_closed(fd: int) -> bool:
     """
     Check if file descriptor is closed
     :param fd: file descriptor
```

### Comparing `rnsh-0.1.3/rnsh/protocol.py` & `rnsh-0.1.4/rnsh/protocol.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/retry.py` & `rnsh-0.1.4/rnsh/retry.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/rnsh.py` & `rnsh-0.1.4/rnsh/rnsh.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/rnslogging.py` & `rnsh-0.1.4/rnsh/rnslogging.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/session.py` & `rnsh-0.1.4/rnsh/session.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/rnsh/testlogging.py` & `rnsh-0.1.4/rnsh/testlogging.py`

 * *Files identical despite different names*

### Comparing `rnsh-0.1.3/PKG-INFO` & `rnsh-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: rnsh
-Version: 0.1.3
+Version: 0.1.4
 Summary: Shell over Reticulum
 License: MIT
 Author: acehoss
 Author-email: acehoss@acehoss.net
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: rns (>=0.5.9)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: rns (>=0.7.4)
 Description-Content-Type: text/markdown
 
 # `r n s h`  Shell over Reticulum 
 [![CI](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-package.yml) 
 [![Release](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml/badge.svg)](https://github.com/acehoss/rnsh/actions/workflows/python-publish.yml) 
 [![PyPI version](https://badge.fury.io/py/rnsh.svg)](https://badge.fury.io/py/rnsh)  
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/rnsh?color=informational&label=Installs&logo=pypi)
@@ -42,14 +40,17 @@
 
 ### Reminder: Beta Software
 The interface is starting to firm up, but some bug fixes at this
 point still may introduce breaking changes, especially in the
 protocol layers of the software.
 
 ## Recent Changes
+### v0.1.4
+- Fix invalid escape sequence handling for terminal escape sequences
+
 ### v0.1.3
 - Fix an issue where disconnecting a session using ~. would result in further connections to
   the same initiator would appear to hang.
 - Setting `-q` will suppress the pre-connect spinners
 
 ### v0.1.2
 - Adaptive compression (RNS update) provides significant performance improvements ([PR](https://github.com/acehoss/rnsh/pull/24))
@@ -304,22 +305,23 @@
   piping the output of `tar` over `rsh`.~~
 - [X] ~~Test on several platforms~~
 - [X] ~~Fix issues that come up with testing~~
 - [X] ~~v0.1.0 beta~~
 - [X] ~~Test and fix more issues~~
 - [ ] More betas
 - [ ] Enhancement Ideas
-  - [ ] `authorized_keys` mode similar to SSH to allow one listener
+  - [x] `authorized_keys` mode similar to SSH to allow one listener
         process to serve multiple users
   - [ ] Git over `rnsh` (git remote helper)
   - [ ] Sliding window acknowledgements for improved throughput
 - [ ] v1.0 someday probably maybe
 
 ## Miscellaneous
 
 By piping into/out of `rnsh`, it is possible to transfer
 files using the same method discussed in 
 [this article](https://cromwell-intl.com/open-source/tar-and-ssh.html).
 It's not terribly fast currently, due to the round-trip rule 
 enforced by the protocol. Sliding window acknowledgements will
 speed this up significantly.
 
+Running tests: `poetry run pytest tests`
```

