# Comparing `tmp/pytest_mh-1.0.8.tar.gz` & `tmp/pytest_mh-1.0.9.tar.gz`

## Comparing `pytest_mh-1.0.8.tar` & `pytest_mh-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/requirements.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/docs/requirements.txt
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/__init__.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/py.typed
--rw-r--r--   0        0        0    31966 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/ssh.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/data.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/fixtures.py
--rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/logging.py
--rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/marks.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/misc.py
--rw-r--r--   0        0        0    19789 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/multihost.py
--rw-r--r--   0        0        0    15999 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/plugin.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/topology.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/_private/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/utils/__init__.py
--rw-r--r--   0        0        0    26458 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/utils/firewall.py
--rw-r--r--   0        0        0    21034 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/utils/fs.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/utils/journald.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/utils/services.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pytest_mh/utils/tc.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/LICENSE
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/readme.md
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pytest_mh-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/requirements.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/docs/requirements.txt
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/__init__.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/py.typed
+-rw-r--r--   0        0        0    31966 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/ssh.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/data.py
+-rw-r--r--   0        0        0    12789 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/fixtures.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/logging.py
+-rw-r--r--   0        0        0     8334 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/marks.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/misc.py
+-rw-r--r--   0        0        0    19789 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/multihost.py
+-rw-r--r--   0        0        0    15999 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/plugin.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/topology.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/_private/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/utils/__init__.py
+-rw-r--r--   0        0        0    26458 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/utils/firewall.py
+-rw-r--r--   0        0        0    22470 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/utils/fs.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/utils/journald.py
+-rw-r--r--   0        0        0     9317 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/utils/services.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pytest_mh/utils/tc.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/readme.md
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pytest_mh-1.0.9/PKG-INFO
```

### Comparing `pytest_mh-1.0.8/pytest_mh/__init__.py` & `pytest_mh-1.0.9/pytest_mh/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/cli.py` & `pytest_mh-1.0.9/pytest_mh/cli.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/ssh.py` & `pytest_mh-1.0.9/pytest_mh/ssh.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/data.py` & `pytest_mh-1.0.9/pytest_mh/_private/data.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/fixtures.py` & `pytest_mh-1.0.9/pytest_mh/_private/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,16 +301,16 @@
         """
         Write log messages produced by current test case to a file, or clear
         them if no artifacts should be generated.
         """
         path = self._artifacts_dir()
         if path is None:
             self.logger.clear()
-
-        self.logger.write_to_file(f"{path}/test.log")
+        else:
+            self.logger.write_to_file(f"{path}/test.log")
 
     def log_phase(self, phase: str) -> None:
         """
         Log current test phase.
 
         :param phase: Phase name or description.
         :type phase: str
```

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/logging.py` & `pytest_mh-1.0.9/pytest_mh/_private/logging.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/marks.py` & `pytest_mh-1.0.9/pytest_mh/_private/marks.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/multihost.py` & `pytest_mh-1.0.9/pytest_mh/_private/multihost.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/plugin.py` & `pytest_mh-1.0.9/pytest_mh/_private/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/topology.py` & `pytest_mh-1.0.9/pytest_mh/_private/topology.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/_private/utils.py` & `pytest_mh-1.0.9/pytest_mh/_private/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/utils/firewall.py` & `pytest_mh-1.0.9/pytest_mh/utils/firewall.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/utils/fs.py` & `pytest_mh-1.0.9/pytest_mh/utils/fs.py`

 * *Files 3% similar despite different names*

```diff
@@ -604,14 +604,53 @@
             args.append("-b")
 
         if chars:
             args.append("-m")
 
         return self.host.ssh.exec(["wc", *args, file], log_level=SSHLog.Error)
 
+    def diff(
+        self,
+        path1: str,
+        path2: str,
+        *,
+        brief: bool = False,
+        recursive: bool = False,
+        ignore_case: bool = False,
+        args: list[str] | None = None,
+    ) -> SSHProcessResult:
+        """
+        Compare files line by line.
+        Exit status is 0 if inputs are the same, 1 if different, 2 if trouble.
+
+        :param path1: Path to file or directory to be compared
+        :type path1: str
+        :param path2: Path to file or directory to be compared
+        :type path2: str
+        :param brief: Report only when files differ, but do not print the diff itself, defaults to False
+        :type brief: bool, optional
+        :param recursive: Recursively compare any subdirectories found, defaults to False
+        :type recursive: bool, optional
+        :param ignore_case: Ignore case differences in file contents, defaults to False
+        :type ignore_case: bool, optional
+        :param args: Additional options, defaults to None
+        :type args: list[str] | None, optional
+        :return: Result of process
+        :rtype: SSHProcessResult
+        """
+        args = args if args else []
+        if brief:
+            args.append("--brief")
+        if recursive:
+            args.append("--recursive")
+        if ignore_case:
+            args.append("--ignore-case")
+
+        return self.host.ssh.exec(["diff", *args, path1, path2], raise_on_error=False)
+
     def chmod(self, mode: str, path: str, args: list[str] | None = None) -> SSHProcessResult:
         """
         Change file/folder mode bits.
         Mode can be specified in two ways: octal number e.g. "666", "444" or
         a symbolic representation of changes e.g. "u=rw,go=r", "go-rw"
 
         :param mode: New mode of file/folder
```

### Comparing `pytest_mh-1.0.8/pytest_mh/utils/journald.py` & `pytest_mh-1.0.9/pytest_mh/utils/journald.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pytest_mh/utils/services.py` & `pytest_mh-1.0.9/pytest_mh/utils/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         :type service: str
         :return: Running SSH process.
         :rtype: SSHProcess
         """
         self.__set_initial_state(service)
         self.logger.info(f'systemd: starting "{service}" asynchronously')
         return self.host.ssh.async_run(
-            f'systemctl start "{service}" || systemctl status "{service}"', log_level=SSHLog.Error
+            f'systemctl reset-failed "{service}"; systemctl start "{service}" || systemctl status "{service}"',
+            log_level=SSHLog.Error,
         )
 
     def start(self, service: str, raise_on_error: bool = True) -> SSHProcessResult:
         """
         Start a systemd unit. The call will wait until the operation is finished.
 
         ``systemctl status $unit`` is called automatically if the unit can not
@@ -62,15 +63,15 @@
         :type raise_on_error: bool, optional
         :return: SSH process result.
         :rtype: SSHProcessResult
         """
         self.__set_initial_state(service)
         self.logger.info(f'systemd: starting "{service}"')
         return self.host.ssh.run(
-            f'systemctl start "{service}" || systemctl status "{service}"',
+            f'systemctl reset-failed "{service}"; systemctl start "{service}" || systemctl status "{service}"',
             raise_on_error=raise_on_error,
             log_level=SSHLog.Error,
         )
 
     def async_stop(self, service: str) -> SSHProcess:
         """
         Stop a systemd unit. Non-blocking call.
@@ -122,15 +123,16 @@
         :type service: str
         :return: Running SSH process.
         :rtype: SSHProcess
         """
         self.__set_initial_state(service)
         self.logger.info(f'systemd: restarting "{service}" asynchronously')
         return self.host.ssh.async_run(
-            f'systemctl restart "{service}" || systemctl status "{service}"', log_level=SSHLog.Error
+            f'systemctl reset-failed "{service}"; systemctl restart "{service}" || systemctl status "{service}"',
+            log_level=SSHLog.Error,
         )
 
     def restart(self, service: str, raise_on_error: bool = True) -> SSHProcessResult:
         """
         Restart a systemd unit. The call will wait until the operation is finished.
 
         ``systemctl status $unit`` is called automatically if the unit can not
@@ -142,15 +144,15 @@
         :type raise_on_error: bool, optional
         :return: SSH process result.
         :rtype: SSHProcessResult
         """
         self.__set_initial_state(service)
         self.logger.info(f'systemd: restarting "{service}"')
         return self.host.ssh.run(
-            f'systemctl restart "{service}" || systemctl status "{service}"',
+            f'systemctl reset-failed "{service}"; systemctl restart "{service}" || systemctl status "{service}"',
             raise_on_error=raise_on_error,
             log_level=SSHLog.Error,
         )
 
     def async_reload(self, service: str) -> SSHProcess:
         """
         Reload a systemd unit. Non-blocking call.
```

### Comparing `pytest_mh-1.0.8/pytest_mh/utils/tc.py` & `pytest_mh-1.0.9/pytest_mh/utils/tc.py`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/LICENSE` & `pytest_mh-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/pyproject.toml` & `pytest_mh-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/readme.md` & `pytest_mh-1.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `pytest_mh-1.0.8/PKG-INFO` & `pytest_mh-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mh
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pytest multihost plugin
 Project-URL: Homepage, https://github.com/next-actions/pytest-mh
 Project-URL: Bug Tracker, https://github.com/next-actions/pytest-mh/issues
 Author-email: Pavel Březina <pbrezina@redhat.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

