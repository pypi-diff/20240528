# Comparing `tmp/rstms_testmail-0.2.3.tar.gz` & `tmp/rstms_testmail-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstms_testmail-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rstms_testmail-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rstms_testmail-0.2.3.tar` & `rstms_testmail-0.2.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      381 2024-05-17 20:13:32.498412 rstms_testmail-0.2.3/.bumpversion.cfg
--rw-r--r--   0        0        0     1375 2024-04-28 12:24:23.591184 rstms_testmail-0.2.3/.gitignore
--rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.2.3/LICENSE
--rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.2.3/Makefile
--rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.2.3/README.md
--rw-r--r--   0        0        0        6 2024-05-17 20:13:32.498412 rstms_testmail-0.2.3/VERSION
--rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.2.3/docs/Makefile
--rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.2.3/docs/cli.rst
--rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.2.3/docs/conf.py
--rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.2.3/docs/contributing.rst
--rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.2.3/docs/index.rst
--rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.2.3/docs/installation.rst
--rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.2.3/docs/make.bat
--rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.2.3/docs/readme.rst
--rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.2.3/make/browser.mk
--rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.2.3/make/clean.mk
--rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.2.3/make/common.mk
--rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.2.3/make/depends.mk
--rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.2.3/make/dist.mk
--rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.2.3/make/docs.mk
--rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.2.3/make/lint.mk
--rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.2.3/make/publish.mk
--rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.2.3/make/release.mk
--rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.2.3/make/requirements.mk
--rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.2.3/make/test.mk
--rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.2.3/make/version.mk
--rw-r--r--   0        0        0     1232 2024-05-17 20:13:32.498412 rstms_testmail-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.2.3/pytest.ini
--rw-r--r--   0        0        0       97 2024-05-17 20:13:32.346414 rstms_testmail-0.2.3/requirements-dev.txt
--rw-r--r--   0        0        0       47 2024-05-17 20:13:32.402413 rstms_testmail-0.2.3/requirements-docs.txt
--rw-r--r--   0        0        0       89 2024-05-17 20:13:32.286414 rstms_testmail-0.2.3/requirements.txt
--rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.2.3/rstms_testmail/__init__.py
--rw-r--r--   0        0        0     4699 2024-05-17 19:52:43.571922 rstms_testmail-0.2.3/rstms_testmail/cli.py
--rw-r--r--   0        0        0      957 2024-04-28 02:18:58.990987 rstms_testmail-0.2.3/rstms_testmail/counter.py
--rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.2.3/rstms_testmail/exception_handler.py
--rw-r--r--   0        0        0     3676 2024-05-17 19:53:13.035598 rstms_testmail-0.2.3/rstms_testmail/gmail.py
--rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.2.3/rstms_testmail/netstat.py
--rw-r--r--   0        0        0      584 2024-05-17 19:53:22.655493 rstms_testmail-0.2.3/rstms_testmail/sendgrid_server.py
--rw-r--r--   0        0        0     1575 2024-05-17 19:52:23.144146 rstms_testmail-0.2.3/rstms_testmail/settings.py
--rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.2.3/rstms_testmail/shell.py
--rw-r--r--   0        0        0     1342 2024-05-17 20:05:28.167622 rstms_testmail-0.2.3/rstms_testmail/smtp_server.py
--rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.2.3/rstms_testmail/timer.py
--rw-r--r--   0        0        0      127 2024-05-17 20:13:32.498412 rstms_testmail-0.2.3/rstms_testmail/version.py
--rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.2.3/rstms_testmail/watcher.py
--rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-17 19:56:14.241618 rstms_testmail-0.2.3/tests/test_cli.py
--rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.2.3/tests/test_counter.py
--rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.2.3/tests/test_gmail.py
--rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.2.3/tests/test_netstat.py
--rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.2.3/tests/test_sendgrid.py
--rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.2.3/tests/test_watcher.py
--rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.2.3/tox.ini
--rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      381 2024-05-28 05:14:49.396163 rstms_testmail-0.2.4/.bumpversion.cfg
+-rw-r--r--   0        0        0     1375 2024-04-28 12:24:23.591184 rstms_testmail-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1071 2024-04-28 01:24:57.918261 rstms_testmail-0.2.4/LICENSE
+-rw-r--r--   0        0        0      539 2024-04-28 01:24:57.918261 rstms_testmail-0.2.4/Makefile
+-rw-r--r--   0        0        0      679 2024-04-28 01:24:57.930261 rstms_testmail-0.2.4/README.md
+-rw-r--r--   0        0        0        6 2024-05-28 05:14:49.392163 rstms_testmail-0.2.4/VERSION
+-rw-r--r--   0        0        0      615 2024-04-28 01:24:58.006260 rstms_testmail-0.2.4/docs/Makefile
+-rw-r--r--   0        0        0       93 2024-04-28 01:24:58.018260 rstms_testmail-0.2.4/docs/cli.rst
+-rwxr-xr-x   0        0        0     4934 2024-04-28 01:24:58.014260 rstms_testmail-0.2.4/docs/conf.py
+-rw-r--r--   0        0        0       33 2024-04-28 01:24:58.018260 rstms_testmail-0.2.4/docs/contributing.rst
+-rw-r--r--   0        0        0      298 2024-04-28 01:24:58.002260 rstms_testmail-0.2.4/docs/index.rst
+-rw-r--r--   0        0        0     1158 2024-04-28 01:24:58.010260 rstms_testmail-0.2.4/docs/installation.rst
+-rw-r--r--   0        0        0      776 2024-04-28 01:24:58.002260 rstms_testmail-0.2.4/docs/make.bat
+-rw-r--r--   0        0        0       27 2024-04-28 01:24:57.998260 rstms_testmail-0.2.4/docs/readme.rst
+-rw-r--r--   0        0        0      431 2024-04-28 01:24:57.946261 rstms_testmail-0.2.4/make/browser.mk
+-rw-r--r--   0        0        0      694 2024-04-28 01:24:57.954260 rstms_testmail-0.2.4/make/clean.mk
+-rw-r--r--   0        0        0     3808 2024-04-28 01:24:57.950260 rstms_testmail-0.2.4/make/common.mk
+-rw-r--r--   0        0        0      477 2024-04-28 01:24:57.946261 rstms_testmail-0.2.4/make/depends.mk
+-rw-r--r--   0        0        0      441 2024-04-28 01:24:57.942261 rstms_testmail-0.2.4/make/dist.mk
+-rw-r--r--   0        0        0      719 2024-04-28 01:24:57.938261 rstms_testmail-0.2.4/make/docs.mk
+-rw-r--r--   0        0        0      610 2024-04-28 01:24:57.934261 rstms_testmail-0.2.4/make/lint.mk
+-rw-r--r--   0        0        0     1214 2024-04-28 01:24:57.938261 rstms_testmail-0.2.4/make/publish.mk
+-rw-r--r--   0        0        0      517 2024-04-28 01:24:57.942261 rstms_testmail-0.2.4/make/release.mk
+-rw-r--r--   0        0        0      502 2024-04-28 01:24:57.942261 rstms_testmail-0.2.4/make/requirements.mk
+-rw-r--r--   0        0        0      947 2024-04-28 01:24:57.938261 rstms_testmail-0.2.4/make/test.mk
+-rw-r--r--   0        0        0     1610 2024-04-28 01:24:57.946261 rstms_testmail-0.2.4/make/version.mk
+-rw-r--r--   0        0        0     1232 2024-05-28 05:14:49.396163 rstms_testmail-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-04-28 01:24:57.890261 rstms_testmail-0.2.4/pytest.ini
+-rw-r--r--   0        0        0       97 2024-05-28 05:14:49.248164 rstms_testmail-0.2.4/requirements-dev.txt
+-rw-r--r--   0        0        0       47 2024-05-28 05:14:49.304164 rstms_testmail-0.2.4/requirements-docs.txt
+-rw-r--r--   0        0        0       89 2024-05-28 05:14:49.192165 rstms_testmail-0.2.4/requirements.txt
+-rw-r--r--   0        0        0      215 2024-04-28 01:57:04.207457 rstms_testmail-0.2.4/rstms_testmail/__init__.py
+-rw-r--r--   0        0        0     5131 2024-05-28 04:45:46.874257 rstms_testmail-0.2.4/rstms_testmail/cli.py
+-rw-r--r--   0        0        0     1083 2024-05-28 03:51:36.702296 rstms_testmail-0.2.4/rstms_testmail/counter.py
+-rw-r--r--   0        0        0     1067 2024-04-28 01:24:57.990260 rstms_testmail-0.2.4/rstms_testmail/exception_handler.py
+-rw-r--r--   0        0        0     3690 2024-05-28 05:11:13.522586 rstms_testmail-0.2.4/rstms_testmail/gmail.py
+-rw-r--r--   0        0        0      353 2024-04-28 06:41:02.468012 rstms_testmail-0.2.4/rstms_testmail/netstat.py
+-rw-r--r--   0        0        0      584 2024-05-17 19:53:22.655493 rstms_testmail-0.2.4/rstms_testmail/sendgrid_server.py
+-rw-r--r--   0        0        0     1730 2024-05-28 04:19:47.052744 rstms_testmail-0.2.4/rstms_testmail/settings.py
+-rw-r--r--   0        0        0     1092 2024-04-28 01:57:04.247457 rstms_testmail-0.2.4/rstms_testmail/shell.py
+-rw-r--r--   0        0        0     1454 2024-05-28 04:52:46.146775 rstms_testmail-0.2.4/rstms_testmail/smtp_server.py
+-rw-r--r--   0        0        0      698 2024-04-28 07:28:06.715644 rstms_testmail-0.2.4/rstms_testmail/timer.py
+-rw-r--r--   0        0        0      127 2024-05-28 05:14:49.392163 rstms_testmail-0.2.4/rstms_testmail/version.py
+-rw-r--r--   0        0        0     2669 2024-04-28 08:38:07.194667 rstms_testmail-0.2.4/rstms_testmail/watcher.py
+-rw-r--r--   0        0        0       44 2024-04-28 01:24:57.970260 rstms_testmail-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-17 19:56:14.241618 rstms_testmail-0.2.4/tests/test_cli.py
+-rw-r--r--   0        0        0      330 2024-04-28 06:40:10.408723 rstms_testmail-0.2.4/tests/test_counter.py
+-rw-r--r--   0        0        0      353 2024-04-28 13:04:29.510760 rstms_testmail-0.2.4/tests/test_gmail.py
+-rw-r--r--   0        0        0      201 2024-04-28 06:40:42.264287 rstms_testmail-0.2.4/tests/test_netstat.py
+-rw-r--r--   0        0        0      553 2024-04-28 13:09:49.371217 rstms_testmail-0.2.4/tests/test_sendgrid.py
+-rw-r--r--   0        0        0     1156 2024-04-28 08:39:55.537304 rstms_testmail-0.2.4/tests/test_watcher.py
+-rw-r--r--   0        0        0      430 2024-04-28 01:24:57.894261 rstms_testmail-0.2.4/tox.ini
+-rw-r--r--   0        0        0     2006 1970-01-01 00:00:00.000000 rstms_testmail-0.2.4/PKG-INFO
```

### Comparing `rstms_testmail-0.2.3/.gitignore` & `rstms_testmail-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/LICENSE` & `rstms_testmail-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/Makefile` & `rstms_testmail-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/README.md` & `rstms_testmail-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/docs/Makefile` & `rstms_testmail-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/docs/conf.py` & `rstms_testmail-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/docs/installation.rst` & `rstms_testmail-0.2.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/docs/make.bat` & `rstms_testmail-0.2.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/clean.mk` & `rstms_testmail-0.2.4/make/clean.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/common.mk` & `rstms_testmail-0.2.4/make/common.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/docs.mk` & `rstms_testmail-0.2.4/make/docs.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/lint.mk` & `rstms_testmail-0.2.4/make/lint.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/publish.mk` & `rstms_testmail-0.2.4/make/publish.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/release.mk` & `rstms_testmail-0.2.4/make/release.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/test.mk` & `rstms_testmail-0.2.4/make/test.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/make/version.mk` & `rstms_testmail-0.2.4/make/version.mk`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/pyproject.toml` & `rstms_testmail-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 requires_python = ">=3.10"
 
 
 
 [project]
 name = "rstms-testmail"
-version = "0.2.3"
+version = "0.2.4"
 authors = [{name = "Matt Krueger", email = "mkrueger@rstms.net"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ["rstms_testmail"]
 classifiers = [
   "Intended Audience :: Developers",
```

### Comparing `rstms_testmail-0.2.3/rstms_testmail/cli.py` & `rstms_testmail-0.2.4/rstms_testmail/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Console script for rstms_testmail."""
 
 import json
 import subprocess
 import sys
 from pprint import pformat
+from pathlib import Path
 
 import click
 import click.core
 
 from .counter import Counter
 from .exception_handler import ExceptionHandler
 from .gmail import Gmail
@@ -53,17 +54,18 @@
 @click.option("-u", "--username", envvar="TESTMAIL_USERNAME")
 @click.option("-p", "--password", envvar="TESTMAIL_PASSWORD")
 @click.option("-P", "--port", default=465, envvar="TESTMAIL_PORT")
 @click.option("-m", "--message", help="message to send or - to read from stdin")
 @click.option("--profile", "profile_option", default="default", show_envvar=True, envvar="TESTMAIL_PROFILE")
 @click.option("--dryrun", is_flag=True)
 @click.option("--reset-token", is_flag=True)
-@click.option("-W", "--write-profile", help="profile name to write")
+@click.option("--show-password", is_flag=True, help='unmask password in dryrun output')
+@click.option("-W", "--write-profile", help="write current profile")
 @click.option("-D", "--delete", "delete_profile", is_flag=True, help="profile name to delete")
-@click.option("-L", "--list", "list_profiles", is_flag=True, help="profile name to write")
+@click.option("-L", "--list", "list_profiles", is_flag=True, help="list available profiles")
 @click.argument("profile", required=False)
 @click.pass_context
 def cli(  # noqa:
     ctx,
     debug,
     shell_completion,
     quiet,
@@ -82,36 +84,43 @@
     api_key,
     profile,
     write_profile,
     reset_token,
     delete_profile,
     list_profiles,
     profile_option,
+    show_password
 ):
     """send a test email"""
 
+    config_dir = Path.home()/'.testmail'
+
     if profile is None:
         profile = profile_option
 
     if "{}" in subject:
-        counter = Counter(label="testmail")
+        counter = Counter(label="testmail", dir=config_dir)
         count = counter.bump(set_counter)
         subject = subject.replace("{}", str(count))
+    else:
+        counter = None
 
     settings = Settings(
-        profile=f"testmail_{profile}",
+        label='testmail',
+        dir=config_dir,
+        profile=profile,
         from_addr=from_addr,
         to_addr=to_addr,
         system=system,
         exec_command=exec_command,
         username=username,
         password=password,
         port=port,
         api_key=api_key,
-        write_profile=f"testmail_{write_profile}",
+        write_profile=write_profile,
     )
 
     if delete_profile:
         settings.delete()
         sys.exit(0)
 
     profiles = settings.profiles()
@@ -137,20 +146,25 @@
     system = settings.system or ""
 
     if system == "gmail":
         server = Gmail(settings.password, reset_token)
     elif system == "sendgrid":
         server = SendGrid(settings.api_key)
     elif system.startswith("smtp:") or system.startswith("smtps:"):
-        server = SMTPServer(settings.system, settings.port, settings.username, settings.password)
+        server = SMTPServer(settings.system, settings.port, settings.username, settings.password, verbose)
     else:
         fail(f"unknown system: {repr(system)}")
 
     if dryrun:
-        click.echo(pformat(settings.dict()))
+        output = settings.dict()
+        if not show_password:
+            output['password'] = '***************'
+        click.echo(pformat({profile: output}))
+        if counter is not None:
+            counter.rewind()
         sys.exit(0)
     else:
         error = server.send(settings.from_addr, settings.to_addr, subject, message)
 
     if error:
         fail(pformat(error))
```

### Comparing `rstms_testmail-0.2.3/rstms_testmail/counter.py` & `rstms_testmail-0.2.4/rstms_testmail/counter.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,24 +10,27 @@
             dir = Path.home()
         else:
             dir = Path(dir)
 
         if label is None:
             filename = ".counter"
         else:
-            filename = f".{label}_counter"
+            filename = f".{label}.counter"
 
         self.file = dir / filename
 
         if count is None:
             self.read()
         else:
             self.value = int(count)
             self.write()
 
+        self.initial_value = self.value
+
+
     def read(self):
         if not self.file.is_file():
             self.value = 0
             return self.write()
         self.value = int(self.file.read_text() or "0")
         return self.value
 
@@ -38,7 +41,11 @@
     def bump(self, value=None):
         if value:
             self.value = value
         else:
             self.value += 1
 
         return self.write()
+
+    def rewind(self):
+        self.value = self.initial_value
+        self.write()
```

### Comparing `rstms_testmail-0.2.3/rstms_testmail/exception_handler.py` & `rstms_testmail-0.2.4/rstms_testmail/exception_handler.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/rstms_testmail/gmail.py` & `rstms_testmail-0.2.4/rstms_testmail/gmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class Gmail:
 
     def __init__(self, credentials, reset_token=False):
         """credentials is a base64 encoded credentials.json file. (see https://console.cloud.google.com)"""
 
         self.credentials = credentials
-        self.token_file = Path.home() / ".testmail-gmail-token.json"
+        self.token_file = Path.home() / ".testmail" / ".testmail-gmail-token.json"
         if reset_token:
             self.token_file.unlink()
 
         with PortWatcher("ssh -q -N -R {}:localhost:{} beaker"):
             self.creds = self.authenticate_gmail_api()
 
             # create gmail api client
```

### Comparing `rstms_testmail-0.2.3/rstms_testmail/sendgrid_server.py` & `rstms_testmail-0.2.4/rstms_testmail/sendgrid_server.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/rstms_testmail/settings.py` & `rstms_testmail-0.2.4/rstms_testmail/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 import json
 from pathlib import Path
 
 
 class Settings:
     def __init__(self, **kwargs):
-        profile = kwargs.pop("profile", "")
+        self.label = kwargs.pop("label", "")
+        self.profile = kwargs.pop("profile", "")
         write_profile = kwargs.pop("write_profile", "")
+        self.dir = kwargs.pop("dir", "~")
 
-        dir = kwargs.pop("dir", "~")
-        if dir in ["~", None]:
-            dir = Path.home()
+        if self.dir in ["~", None]:
+            self.dir = Path.home()
         else:
-            dir = Path(dir)
-        self.dir = dir
+            self.dir = Path(self.dir)
 
-        self.file = dir / f".{profile}_settings"
+        self.file = self.dir / f".{self.label}_{self.profile}_settings"
 
         old_settings = self.read()
 
         self._settings = {}
 
         for k, v in kwargs.items():
             if v is None:
                 v = old_settings.get(k, None)
             self._settings[k] = v
             setattr(self, k, v)
 
         if write_profile:
-            self.write(self._settings, dir / f".{write_profile}_settings")
+            self.write(self._settings, self.dir / f".{self.label}_{write_profile}_settings")
 
     def delete(self):
         self.file.unlink()
         return
 
     def profiles(self):
         profiles = []
         label, _, _ = self.file.name.partition("_")
         for item in self.file.parent.iterdir():
             if not item.is_file():
                 continue
             prefix, _, tail = item.name.partition("_")
             if prefix != label:
                 continue
-            name, _, _ = tail.partition("_")
+            name, _, tail = tail.partition("_")
+            if tail != 'settings':
+                continue
             if name:
                 profiles.append(name)
         return profiles
 
     def read(self):
         if self.file.is_file():
             content = self.file.read_text()
+            return json.loads(content)
         else:
-            content = "{}"
-        return json.loads(content)
+            return {}
 
     def write(self, settings, file):
         file.write_text(json.dumps(settings, indent=2))
 
     def dict(self):
         return self._settings
```

### Comparing `rstms_testmail-0.2.3/rstms_testmail/shell.py` & `rstms_testmail-0.2.4/rstms_testmail/shell.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/rstms_testmail/smtp_server.py` & `rstms_testmail-0.2.4/rstms_testmail/smtp_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import make_msgid
 
 
 class SMTPServer:
 
-    def __init__(self, system, port, username, password):
+    def __init__(self, system, port, username, password, debug=None):
         self.protocol, _, self.server = system.partition(":")
         self.port = int(port)
         self.username = username
         self.password = password
+        self.debug = debug
 
     def send(self, from_addr, to_addr, subject, message):
         """
         Send an email using an SMTP server that requires SSL and authentication.
 
         Parameters:
         - from_addr: str - the sender's email address
@@ -28,11 +29,13 @@
         mime_message["From"] = from_addr
         mime_message["To"] = to_addr
         mime_message['Message-ID'] = make_msgid()
         mime_message.attach(MIMEText(message, "plain"))
 
         # Connect to the SMTP server using SSL
         server = smtplib.SMTP_SSL(self.server, self.port)
+        server.set_debuglevel(self.debug)
         server.login(self.username, self.password)
-        server.sendmail(from_addr, to_addr, mime_message.as_string())
+        ret = server.sendmail(from_addr, to_addr, mime_message.as_string())
         server.quit()
-        return None
+        self.result = ret
+        return ret
```

### Comparing `rstms_testmail-0.2.3/rstms_testmail/timer.py` & `rstms_testmail-0.2.4/rstms_testmail/timer.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/rstms_testmail/watcher.py` & `rstms_testmail-0.2.4/rstms_testmail/watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/tests/test_cli.py` & `rstms_testmail-0.2.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/tests/test_sendgrid.py` & `rstms_testmail-0.2.4/tests/test_sendgrid.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/tests/test_watcher.py` & `rstms_testmail-0.2.4/tests/test_watcher.py`

 * *Files identical despite different names*

### Comparing `rstms_testmail-0.2.3/PKG-INFO` & `rstms_testmail-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstms-testmail
-Version: 0.2.3
+Version: 0.2.4
 Summary: Top-level package for rstms-testmail.
 Keywords: rstms_testmail
 Author-email: Matt Krueger <mkrueger@rstms.net>
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

