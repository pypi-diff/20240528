# Comparing `tmp/dc2host-0.0.1.tar.gz` & `tmp/dc2host-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dc2host-0.0.1.tar", last modified: Sun May 19 22:59:20 2024, max compression
+gzip compressed data, was "dc2host-1.0.0.tar", last modified: Tue May 28 00:09:47 2024, max compression
```

## Comparing `dc2host-0.0.1.tar` & `dc2host-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:59:20.143524 dc2host-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 22:59:15.000000 dc2host-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-19 22:59:20.143524 dc2host-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-19 22:59:15.000000 dc2host-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:59:20.143524 dc2host-0.0.1/dc2host/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 22:59:15.000000 dc2host-0.0.1/dc2host/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-19 22:59:15.000000 dc2host-0.0.1/dc2host/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 22:59:15.000000 dc2host-0.0.1/dc2host/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-19 22:59:15.000000 dc2host-0.0.1/dc2host/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:59:20.143524 dc2host-0.0.1/dc2host.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-19 22:59:20.000000 dc2host-0.0.1/dc2host.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 22:59:20.000000 dc2host-0.0.1/dc2host.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:59:20.000000 dc2host-0.0.1/dc2host.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 22:59:20.000000 dc2host-0.0.1/dc2host.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 22:59:20.000000 dc2host-0.0.1/dc2host.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-19 22:59:15.000000 dc2host-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:59:20.143524 dc2host-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:59:20.143524 dc2host-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-19 22:59:15.000000 dc2host-0.0.1/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:09:47.069232 dc2host-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-28 00:09:42.000000 dc2host-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-28 00:09:47.069232 dc2host-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-28 00:09:42.000000 dc2host-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:09:47.069232 dc2host-1.0.0/dc2host/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 00:09:42.000000 dc2host-1.0.0/dc2host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 00:09:42.000000 dc2host-1.0.0/dc2host/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-28 00:09:42.000000 dc2host-1.0.0/dc2host/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 00:09:42.000000 dc2host-1.0.0/dc2host/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-28 00:09:42.000000 dc2host-1.0.0/dc2host/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:09:47.069232 dc2host-1.0.0/dc2host.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-28 00:09:47.000000 dc2host-1.0.0/dc2host.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-28 00:09:47.000000 dc2host-1.0.0/dc2host.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:09:47.000000 dc2host-1.0.0/dc2host.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 00:09:47.000000 dc2host-1.0.0/dc2host.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 00:09:47.000000 dc2host-1.0.0/dc2host.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-28 00:09:42.000000 dc2host-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:09:47.069232 dc2host-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:09:47.069232 dc2host-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-28 00:09:42.000000 dc2host-1.0.0/tests/test_helpers.py
```

### Comparing `dc2host-0.0.1/LICENSE` & `dc2host-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dc2host-0.0.1/PKG-INFO` & `dc2host-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,101 +1,94 @@
 Metadata-Version: 2.1
 Name: dc2host
-Version: 0.0.1
+Version: 1.0.0
 Summary: VS Code Dev Containers integration with a host system
 Author-email: Vlad Folts <vladfolts@gmail.com>
+Project-URL: Homepage, https://github.com/vladfolts/dc2host
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docker
 Requires-Dist: flask
 Requires-Dist: GitPython
+Provides-Extra: test
+Requires-Dist: types-docker; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 # Introduction
 
 `dc2host` python package is intended to be used for interaction between VS Code running Dev Containers and other development tools that run on the host system (e.g. `git difftool` etc).
 It also contains a command line interface that can be used without VS Code just to open a source file from a local Git repository in GitLab/GitHub Web UI with the specified line number selected.
 
 ## `git difftool` example
 
 Suppose you have your favorite GUI `git difftool` configured to run from VS Code for the current file. This setup won't work when you start using Dev Containers because your host system is isolated from VS Code Server and file paths are different for what VS Code sees in a container and for what `git difftool` sees on the host.
 
 To resolve this problem `dc2host` runs a simple REST server on the host that handles requests from Dev Containers and knows how to translate file paths to use them on the host.
 
 # Supported REST endpoints
 
-## git command
+## run command
 
 ```
-POST /run_git
+POST /run
 {
-    "cwd": <container directory where from to execute the specified git command>,
-    "args": ["arguments", "for", "git"]
+    "cwd": <container directory where from to execute the specified command>,
+    "args": ["command", "argument1", "argument2"],
+    "check": false|true - check for zero exit code
 }
 ```
 
-The git repo directory is guessed from "cwd".
-
 Example:
 ```shell
-curl -d "{\"args\": [\"difftool\", \"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run_git
+curl -d "{\"args\": [\"git\", \"difftool\", \"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run
 ```                
 
 
-## gitk command
-
-```
-POST /run_gitk
-{
-    "cwd": <container directory where from to execute the specified gitk command>,
-    "args": ["arguments", "for", "gitk"]
-}
-```
-
-The git repo directory is guessed from "cwd".
-
-Example:
-```shell
-curl -d "{\"args\": [\"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run_gitk
-```                
-
 ## open_in_browser command
 
-Opens the specified file from a local repo in web browser on GitHub. 
+Opens the specified file from a local repo in Web browser on GitHub/GitLab. 
 
 ```
 POST /open_in_browser
 {
     "file": <file path in a container directory>,
     "lineNumber": <line number to highlight (optional)>
 }
 ```
 
 Example:
 ```shell
-curl -d "{\"file\": \"file1.txt\", \"lineNumber\": 42}" -H "Content-Type: application/json" host.docker.internal:5000/run_gitk
+curl -d "{\"file\": \"file1.txt\", \"lineNumber\": 42}" -H "Content-Type: application/json" host.docker.internal:5000/run
 ```                
 
 # Quick start
 
+
+Open file "README.md" from a local directory on GitHub:
+```shell
+python -m dc2host open README.md 
+```
+
 Run Flask on Windows host:
 ```shell
 python -m flask --app dc2host.app run --debug --host=0.0.0.0
 ```
 
 ## Configure VS Code "tasks.json"
 
 ```json
 {
     "tasks": [
         {
-            "label": "Open in GitHub",
+            "label": "Open in GitHub/GitLab",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
                 "{\"file\": \"${file}\", \"lineNumber\": ${lineNumber}}",
                 "-H",
                 "Content-Type: application/json",
@@ -104,30 +97,30 @@
         },
         {
             "label": "Diff current file",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
-                "{\"args\": [\"difftool\", \"${relativeFile}\"], \"cwd\": \"${workspaceFolder}\"}",
+                "{\"args\": [\"git\", \"difftool\", \"${fileBasename}\"], \"cwd\": \"${fileDirname}\"}",
                 "-H",
                 "Content-Type: application/json",
-                "host.docker.internal:5000/run_git"
+                "host.docker.internal:5000/run"
             ],
         },
         {
             "label": "History current file",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
-                "{\"args\": [\"--\", \"${relativeFile}\"], \"cwd\": \"${workspaceFolder}\"}",
+                "{\"args\": [\"gitk\", \"--\", \"${fileBasename}\"], \"cwd\": \"${fileDirname}\", \"check\": false}",
                 "-H",
                 "Content-Type: application/json",
-                "host.docker.internal:5000/run_gitk"
+                "host.docker.internal:5000/run"
             ],
         }
     ]
 }
 ```
 
 ## Configure VS Code "keybindings.json"
@@ -136,12 +129,7 @@
     {
         "key": "ctrl+k ctrl+d",
         "command": "workbench.action.tasks.runTask",
         "args": "Diff current file"
     }
 ]
 ```
-
-## Command line interface
-```shell
-python -m dc2host open <path to file in repo> 
-```
```

### Comparing `dc2host-0.0.1/README.md` & `dc2host-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,80 +7,68 @@
 
 Suppose you have your favorite GUI `git difftool` configured to run from VS Code for the current file. This setup won't work when you start using Dev Containers because your host system is isolated from VS Code Server and file paths are different for what VS Code sees in a container and for what `git difftool` sees on the host.
 
 To resolve this problem `dc2host` runs a simple REST server on the host that handles requests from Dev Containers and knows how to translate file paths to use them on the host.
 
 # Supported REST endpoints
 
-## git command
+## run command
 
 ```
-POST /run_git
+POST /run
 {
-    "cwd": <container directory where from to execute the specified git command>,
-    "args": ["arguments", "for", "git"]
+    "cwd": <container directory where from to execute the specified command>,
+    "args": ["command", "argument1", "argument2"],
+    "check": false|true - check for zero exit code
 }
 ```
 
-The git repo directory is guessed from "cwd".
-
 Example:
 ```shell
-curl -d "{\"args\": [\"difftool\", \"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run_git
+curl -d "{\"args\": [\"git\", \"difftool\", \"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run
 ```                
 
 
-## gitk command
-
-```
-POST /run_gitk
-{
-    "cwd": <container directory where from to execute the specified gitk command>,
-    "args": ["arguments", "for", "gitk"]
-}
-```
-
-The git repo directory is guessed from "cwd".
-
-Example:
-```shell
-curl -d "{\"args\": [\"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run_gitk
-```                
-
 ## open_in_browser command
 
-Opens the specified file from a local repo in web browser on GitHub. 
+Opens the specified file from a local repo in Web browser on GitHub/GitLab. 
 
 ```
 POST /open_in_browser
 {
     "file": <file path in a container directory>,
     "lineNumber": <line number to highlight (optional)>
 }
 ```
 
 Example:
 ```shell
-curl -d "{\"file\": \"file1.txt\", \"lineNumber\": 42}" -H "Content-Type: application/json" host.docker.internal:5000/run_gitk
+curl -d "{\"file\": \"file1.txt\", \"lineNumber\": 42}" -H "Content-Type: application/json" host.docker.internal:5000/run
 ```                
 
 # Quick start
 
+
+Open file "README.md" from a local directory on GitHub:
+```shell
+python -m dc2host open README.md 
+```
+
 Run Flask on Windows host:
 ```shell
 python -m flask --app dc2host.app run --debug --host=0.0.0.0
 ```
 
 ## Configure VS Code "tasks.json"
 
 ```json
 {
     "tasks": [
         {
-            "label": "Open in GitHub",
+            "label": "Open in GitHub/GitLab",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
                 "{\"file\": \"${file}\", \"lineNumber\": ${lineNumber}}",
                 "-H",
                 "Content-Type: application/json",
@@ -89,30 +77,30 @@
         },
         {
             "label": "Diff current file",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
-                "{\"args\": [\"difftool\", \"${relativeFile}\"], \"cwd\": \"${workspaceFolder}\"}",
+                "{\"args\": [\"git\", \"difftool\", \"${fileBasename}\"], \"cwd\": \"${fileDirname}\"}",
                 "-H",
                 "Content-Type: application/json",
-                "host.docker.internal:5000/run_git"
+                "host.docker.internal:5000/run"
             ],
         },
         {
             "label": "History current file",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
-                "{\"args\": [\"--\", \"${relativeFile}\"], \"cwd\": \"${workspaceFolder}\"}",
+                "{\"args\": [\"gitk\", \"--\", \"${fileBasename}\"], \"cwd\": \"${fileDirname}\", \"check\": false}",
                 "-H",
                 "Content-Type: application/json",
-                "host.docker.internal:5000/run_gitk"
+                "host.docker.internal:5000/run"
             ],
         }
     ]
 }
 ```
 
 ## Configure VS Code "keybindings.json"
@@ -121,12 +109,7 @@
     {
         "key": "ctrl+k ctrl+d",
         "command": "workbench.action.tasks.runTask",
         "args": "Diff current file"
     }
 ]
 ```
-
-## Command line interface
-```shell
-python -m dc2host open <path to file in repo> 
-```
```

### Comparing `dc2host-0.0.1/dc2host/cli.py` & `dc2host-1.0.0/dc2host/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from pathlib import Path
 
 from .helpers import open_in_browser
 
 
 def main():
     parser = argparse.ArgumentParser(description="VS Code Host")
-    subparsers = parser.add_subparsers(
-        dest="action", required=True
-    )
+    subparsers = parser.add_subparsers(dest="action", required=True)
     open_parser = subparsers.add_parser("open", help=f"open in a web browser")
-    open_parser.add_argument("path", type=Path)
-    open_parser.add_argument("--line", dest="line", type=int, help="highlight line number in the file")
+    open_parser.add_argument(
+        "path",
+        type=Path,
+        nargs="?",
+        help="path to the file or directory, default is current directory",
+    )
+    open_parser.add_argument(
+        "--line", dest="line", type=int, help="highlight line number in the file"
+    )
     open_parser.set_defaults(func=_handle_open)
 
     result = parser.parse_args()
     result.func(result)
 
 
-def _handle_open(args):
-    file_path: Path = args.path.absolute()
-    repo_path = file_path
-    if repo_path.is_file():
-        repo_path = repo_path.parent
-    git = Repo(repo_path)
-    open_in_browser(git, file_path.relative_to(git.working_dir), args.line)
+def _handle_open(args: argparse.Namespace):
+    file_path: Path = Path(args.path).absolute() if args.path else Path.cwd()
+    open_in_browser(file_path, args.line)
```

### Comparing `dc2host-0.0.1/dc2host/helpers.py` & `dc2host-1.0.0/dc2host/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from pathlib import Path
 import subprocess
+import webbrowser
+from pathlib import Path
 from shlex import quote
 from typing import Generator
 from urllib.parse import SplitResult, urlsplit, urlunsplit
-import webbrowser
 
 import docker
 from docker.models.containers import Container
 from git import Repo
+from werkzeug.exceptions import HTTPException
 
 
 def _gen_bind_mounts(container: Container) -> Generator[tuple[str, str], None, None]:
     if mounts := container.attrs["HostConfig"].get("Mounts"):
         for mount in mounts:
             if mount["Type"] == "bind":
                 src, dst = mount["Source"], mount["Target"]
                 yield src, dst
 
 
-def docker_bind_mounts() -> Generator[tuple[str, str], None, None]:
-    client = docker.from_env()
-    for c in client.containers.list():
-        yield from _gen_bind_mounts(c)
+class Host:
+    def __init__(self):
+        self.__docker = docker.from_env()
+
+    def docker_bind_mounts(self) -> Generator[tuple[str, str], None, None]:
+        for c in self.__docker.containers.list():
+            yield from _gen_bind_mounts(c)
 
 
 def git_remote(repo_path: str):
     repo = Repo(repo_path)
     return repo.remotes.origin.url
 
 
@@ -46,35 +50,43 @@
         result = "https://" + host + "/" + host_path
     return urlsplit(result)
 
 
 def repo_file_url(
     remote_url: str, path: Path, line: int | None = None, branch: str = "master"
 ):
+    known_hosts_mapping = {"github.com": "/blob/{0}/{1}"}
+    default_mapping = "/-/blob/{0}/{1}"
+
     url_parts = repo_root_url(remote_url)
-    branch_path = {"github.com": f"/blob/{branch}/{path}"}.get(url_parts.hostname, f"/-/blob/{branch}/{path}")
+    if not (host := url_parts.hostname):
+        raise HTTPException("Cannot parse remote URL's host: " + remote_url)
+    
+    fmt = known_hosts_mapping.get(host, default_mapping)
+    branch_path = fmt.format(branch, path)
     url_parts = url_parts._replace(path=url_parts.path + branch_path)
     if line is not None:
         url_parts = url_parts._replace(fragment=f"L{line}")
     return urlunsplit(url_parts)
 
 
-def map_container_path_to_git(path: Path) -> tuple[Repo, Path]:
-    for src, dst in docker_bind_mounts():
+def map_container_path(host: Host, path: Path) -> Path:
+    for src, dst in host.docker_bind_mounts():
         try:
             rel_path = path.relative_to(dst)
         except ValueError:
             pass
         else:
-            return Repo(src), rel_path
+            return (src / rel_path).resolve()
 
     raise ValueError(f"Path {path} is not in any bind mounts")
 
 
-def open_in_browser(git: Repo, rel_path: Path, line: int | None):
+def open_in_browser(path: Path, line: int | None):
+    git = Repo(path if path.is_dir() else path.parent, search_parent_directories=True)
     url = repo_file_url(
         git.remotes.origin.url,
-        rel_path,
+        path.relative_to(git.working_dir),
         line=line,
         branch=git.active_branch,
     )
     webbrowser.open(url)
```

### Comparing `dc2host-0.0.1/dc2host.egg-info/PKG-INFO` & `dc2host-1.0.0/dc2host.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,101 +1,94 @@
 Metadata-Version: 2.1
 Name: dc2host
-Version: 0.0.1
+Version: 1.0.0
 Summary: VS Code Dev Containers integration with a host system
 Author-email: Vlad Folts <vladfolts@gmail.com>
+Project-URL: Homepage, https://github.com/vladfolts/dc2host
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docker
 Requires-Dist: flask
 Requires-Dist: GitPython
+Provides-Extra: test
+Requires-Dist: types-docker; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: pytest; extra == "test"
 
 # Introduction
 
 `dc2host` python package is intended to be used for interaction between VS Code running Dev Containers and other development tools that run on the host system (e.g. `git difftool` etc).
 It also contains a command line interface that can be used without VS Code just to open a source file from a local Git repository in GitLab/GitHub Web UI with the specified line number selected.
 
 ## `git difftool` example
 
 Suppose you have your favorite GUI `git difftool` configured to run from VS Code for the current file. This setup won't work when you start using Dev Containers because your host system is isolated from VS Code Server and file paths are different for what VS Code sees in a container and for what `git difftool` sees on the host.
 
 To resolve this problem `dc2host` runs a simple REST server on the host that handles requests from Dev Containers and knows how to translate file paths to use them on the host.
 
 # Supported REST endpoints
 
-## git command
+## run command
 
 ```
-POST /run_git
+POST /run
 {
-    "cwd": <container directory where from to execute the specified git command>,
-    "args": ["arguments", "for", "git"]
+    "cwd": <container directory where from to execute the specified command>,
+    "args": ["command", "argument1", "argument2"],
+    "check": false|true - check for zero exit code
 }
 ```
 
-The git repo directory is guessed from "cwd".
-
 Example:
 ```shell
-curl -d "{\"args\": [\"difftool\", \"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run_git
+curl -d "{\"args\": [\"git\", \"difftool\", \"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run
 ```                
 
 
-## gitk command
-
-```
-POST /run_gitk
-{
-    "cwd": <container directory where from to execute the specified gitk command>,
-    "args": ["arguments", "for", "gitk"]
-}
-```
-
-The git repo directory is guessed from "cwd".
-
-Example:
-```shell
-curl -d "{\"args\": [\"file/relative/path\"], \"cwd\": \"/workspace/directory\"}" -H "Content-Type: application/json" host.docker.internal:5000/run_gitk
-```                
-
 ## open_in_browser command
 
-Opens the specified file from a local repo in web browser on GitHub. 
+Opens the specified file from a local repo in Web browser on GitHub/GitLab. 
 
 ```
 POST /open_in_browser
 {
     "file": <file path in a container directory>,
     "lineNumber": <line number to highlight (optional)>
 }
 ```
 
 Example:
 ```shell
-curl -d "{\"file\": \"file1.txt\", \"lineNumber\": 42}" -H "Content-Type: application/json" host.docker.internal:5000/run_gitk
+curl -d "{\"file\": \"file1.txt\", \"lineNumber\": 42}" -H "Content-Type: application/json" host.docker.internal:5000/run
 ```                
 
 # Quick start
 
+
+Open file "README.md" from a local directory on GitHub:
+```shell
+python -m dc2host open README.md 
+```
+
 Run Flask on Windows host:
 ```shell
 python -m flask --app dc2host.app run --debug --host=0.0.0.0
 ```
 
 ## Configure VS Code "tasks.json"
 
 ```json
 {
     "tasks": [
         {
-            "label": "Open in GitHub",
+            "label": "Open in GitHub/GitLab",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
                 "{\"file\": \"${file}\", \"lineNumber\": ${lineNumber}}",
                 "-H",
                 "Content-Type: application/json",
@@ -104,30 +97,30 @@
         },
         {
             "label": "Diff current file",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
-                "{\"args\": [\"difftool\", \"${relativeFile}\"], \"cwd\": \"${workspaceFolder}\"}",
+                "{\"args\": [\"git\", \"difftool\", \"${fileBasename}\"], \"cwd\": \"${fileDirname}\"}",
                 "-H",
                 "Content-Type: application/json",
-                "host.docker.internal:5000/run_git"
+                "host.docker.internal:5000/run"
             ],
         },
         {
             "label": "History current file",
             "type": "process",
             "command": "curl",
             "args": [
                 "-d",
-                "{\"args\": [\"--\", \"${relativeFile}\"], \"cwd\": \"${workspaceFolder}\"}",
+                "{\"args\": [\"gitk\", \"--\", \"${fileBasename}\"], \"cwd\": \"${fileDirname}\", \"check\": false}",
                 "-H",
                 "Content-Type: application/json",
-                "host.docker.internal:5000/run_gitk"
+                "host.docker.internal:5000/run"
             ],
         }
     ]
 }
 ```
 
 ## Configure VS Code "keybindings.json"
@@ -136,12 +129,7 @@
     {
         "key": "ctrl+k ctrl+d",
         "command": "workbench.action.tasks.runTask",
         "args": "Diff current file"
     }
 ]
 ```
-
-## Command line interface
-```shell
-python -m dc2host open <path to file in repo> 
-```
```

### Comparing `dc2host-0.0.1/tests/test_helpers.py` & `dc2host-1.0.0/tests/test_helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib.parse import SplitResult
-from d2host.helpers import repo_root_url
+from dc2host.helpers import repo_root_url
 
 
 def test_repo_root_url_with_git_prefix():
     assert repo_root_url("git@example.com:namespace/repo.git") == SplitResult(
         scheme="https",
         netloc="example.com",
         path="/namespace/repo",
```

