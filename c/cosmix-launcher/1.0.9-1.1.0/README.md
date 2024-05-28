# Comparing `tmp/cosmix_launcher-1.0.9.tar.gz` & `tmp/cosmix_launcher-1.1.0.tar.gz`

## Comparing `cosmix_launcher-1.0.9.tar` & `cosmix_launcher-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/license.txt
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/requirements.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/scripts/test.sh
--rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/config.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/net.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/.gitignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/readme.md
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/license.txt
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/scripts/test.sh
+-rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     7793 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/.gitignore
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/readme.md
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 cosmix_launcher-1.1.0/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.9/license.txt` & `cosmix_launcher-1.1.0/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.9/src/cosmix/__init__.py` & `cosmix_launcher-1.1.0/src/cosmix/api/instance.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,203 +1,230 @@
-from . import api
-from .api.instance import Instance
-from .api import paths
-from .api import logger
-from .api import net
-from .api import versions
-from .api import config
+from . import paths
+from . import net
+from . import maven
+from . import logger
+from . import mod
+from . import versions
 from typing import Optional
-import sys
-import click
+import hjson
 import os
-import send2trash
+import re
+import java_manifest
 import shutil
 
 
-@click.group()
-@click.option("--work-dir", "-w", type=str, default=paths.WORK_DIR, help="Set a working directory for Cosmix.")
-def cosmix(work_dir: str):
-    if work_dir != paths.WORK_DIR:
-        paths.update_work_dir(os.path.abspath(work_dir))
-        # We clear config caches here just in case the config was cached before the
-        # working directory was updated
-        config._CACHED_CONFIG = None
-        logger._sanatization_mode = None
-        logger._sanatized_username = None
-        logger._colored_logs = None
-        logger.info("Set working directory to " + work_dir)
-
-
-@cosmix.command()
-def version():
-    logger.info("Cosmix " + api.VERSION)
-
-
-@cosmix.command()
-@click.option("--no-versions", "-V", is_flag=True, default=False, help="Disables latest version checks.")
-def debug(no_versions: bool):
-    logger.info("Cosmix " + api.VERSION)
-    logger.info("Paths:")
-    logger.info("  Local Path: " + paths.LOCAL_PATH)
-    logger.info("  Work Dir:   " + paths.WORK_DIR)
-    logger.info("  Instances:  " + paths.INSTANCES)
-    logger.info("  Deps:       " + paths.DEPS)
-    if not no_versions:
-        logger.info("Latest Available Versions: (these may take a second)")
-        logger.info("  Cosmic Reach: " + versions.get_latest_of("reach"))
-        logger.info("  Cosmic Quilt: " + versions.get_latest_of("quilt"))
-
-
-@cosmix.command()
-@click.option("--version", "-v", default="latest", type=str, help="The version of Cosmic Reach to use. Defaults to 'latest'")
-@click.option("--quilt-version", "-q", default=None, type=str, help="The Cosmic Quilt version to use.")
-@click.option("--display-name", "-n", default=None, type=str, help="An optional display name to use for the instance.")
-@click.argument("name")
-def add(version: str, quilt_version: str, display_name: Optional[str], name: str):
-    if Instance.exists(name):
-        logger.error("Instance already exists.")
-        exit(1)
-    instance = Instance.make_instance(name, version, quilt_version, display_name)
-    instance.download()
-    logger.info("Made instance " + name)
-
-
-@cosmix.command()
-@click.option("--version", "-v", default="none", type=str, help="The version of Cosmic Reach to update to. Defaults to 'none'")
-@click.option("--quilt-version", "-q", default="none", type=str, help="The Cosmic Quilt version to update to. Defaults to 'none'")
-@click.argument("name")
-def update(version: str, quilt_version: str, name: str):
-    instance = Instance.get_or_throw(name)
-
-    if version != "none":
-        instance.version = versions.get_version_or_latest_of("reach", version)
-    if quilt_version != "none":
-        instance.quilt_version = versions.get_version_or_latest_of("quilt", quilt_version)
-
-    instance.save()
-    instance.download(is_updating = True)
-
-    logger.info("Updated instance " + name)
-
-
-@cosmix.command()
-@click.option("--args", "-a", default="none", type=str, help="A list of JVM args to pass to Cosmic Reach when launched.")
-@click.argument("name")
-def launch(args: str, name: str):
-    Instance.from_config_file(name).launch(args.split())
-
-
-@cosmix.command()
-def instances():
-    if not os.path.exists(paths.INSTANCES) or len(os.listdir(paths.INSTANCES)) <= 0:
-        logger.error("No instances found.")
-        exit(1)
-
-    for instance_name in os.listdir(paths.INSTANCES):
-        instance = Instance.get_or_throw(instance_name)
-        s = f" - \u001b[1m{instance.display_name}\u001b[0m"
-        if instance.display_name != instance.name:
-            s += f" ({instance.name})"
-        s += f" \u001b[33m(Version: {instance.version})\u001b[0m"
-        if instance.quilt_version is not None:
-            s += f" \u001b[34m(Quilt: {instance.quilt_version})\u001b[0m"
-        print(s)
-
-
-@cosmix.command()
-@click.argument("name")
-def trash(name: str):
-    instance = Instance.get_or_throw(name)
-    send2trash.send2trash(instance.path)
-    logger.info("Moved " + name + " to trash.")
-
-
-@cosmix.command()
-@click.argument("name")
-def info(name: str):
-    i = Instance.get_or_throw(name)
-    print(i.display_name + ":")
-    print("Instance: " + i.name + (" (modded)" if i.is_modded() else ""))
-    print("Path:     " + i.path.replace(os.path.expanduser("~"), "~", 1))
-    print("Version:  " + i.version)
-    if i.is_modded():
-        print("Quilt:    " + i.quilt_version)
-        mods = i.get_mods()
-        if (l := len(mods)) > 0:
-            print(f"{l} Mods:")
-            for mod in mods:
-                print(f"  - {mod}")
-
-
-@cosmix.command("add-mod")
-@click.argument("name")
-@click.argument("mod", type=click.Path(exists = True))
-def add_mod(name: str, mod):
-    i = Instance.get_or_throw(name)
-    if not i.is_modded():
-        logger.error("Instance is not modded")
-        exit(1)
-
-    path = os.path.join(i.path, "mods")
-    os.makedirs(path, exist_ok = True)
-    shutil.copyfile(mod, os.path.join(path, os.path.split(mod)[-1]))
-
-    logger.info("Done.")
-
-
-@cosmix.command("add-crm1-mod")
-@click.option("--repo", "-r", default=None, type=str, help="Provide a CRM-1 repo to use to resolve the mod. Dependencies may still be found using default_repos.")
-@click.argument("name")
-@click.argument("mod")
-def add_crm1_mod(repo: Optional[str], name: str, mod: str):
-    i = Instance.get_or_throw(name)
-
-    if not i.is_modded():
-        logger.error("Instance is not modded")
-        exit(1)
-
-    path = os.path.join(i.path, "mods")
-    os.makedirs(path, exist_ok = True)
-
-    repos = config.get_config()["crm1"]["default_repos"]
-    if repo is not None:
-        repos.append(repo)
-
-    net.download_crm1_mod(mod, path, repos)
-    logger.info("Done.")
-
-
-@cosmix.command("add-data-mod")
-@click.option("--ignore-global-warning", "-I", is_flag = True, default = False, help = "Ignores the global path warning.")
-@click.argument("name")
-@click.argument("mod", type=click.Path(exists = True))
-def add_crm_mod(ignore_global_warning: bool, name: str, mod):
-    i = Instance.get_or_throw(name)
-
-    if not i.is_modded() and not ignore_global_warning:
-        logger.warn("Instance is not modded, this means the data mod will be installed to the GLOBAL Cosmic Reach directory (~/.local/share/cosmic-reach/)")
-        logger.warn("Use --ignore-global-warning or -I to ignore this warning.")
-        exit(1)
+__all__ = (
+    "VALID_INSTANCE_NAME",
+    "COSMIC_ARCHIVE_RAW_URL",
+    "Instance",
+)
+
+
+VALID_INSTANCE_NAME = re.compile(r"[a-zA-Z0-9_-]*")
+COSMIC_ARCHIVE_RAW_URL = "https://raw.githubusercontent.com/CRModders/CosmicArchive/main"
+
+
+class Instance:
+    def __init__(
+        self,
+        instance_name: str,
+        cosmic_reach_version: str,
+        args: list[str],
+        quilt_version: Optional[str] = None,
+        display_name: Optional[str] = None,
+        auto_update_reach: Optional[bool] = False,
+        auto_update_quilt: Optional[bool] = False,
+    ):
+        self.name = instance_name
+        self.version = cosmic_reach_version
+        self.args = args
+        self.quilt_version = quilt_version
+        self.display_name = instance_name if display_name is None else display_name
+        self.auto_update_reach = auto_update_reach
+        self.auto_update_quilt = auto_update_quilt
+        self.path = os.path.join(paths.INSTANCES, self.name)
+
+    def is_modded(self) -> bool:
+        return self.quilt_version is not None
+
+    def path_to(self, path: str) -> str:
+        return os.path.join(self.path, path)
+
+    def get_classpath(self) -> str:
+        classpath = []
+        cq_path = paths.path_to_cq_deps(self.quilt_version)
+        path = self.path_to("deps")
+
+        # Get Cosmic Quilt deps from the global folder
+        if self.is_modded() and os.path.exists(cq_path):
+            classpath.extend([os.path.join(cq_path, dep) for dep in os.listdir(cq_path)])
+
+        # Get per-instance dependencies
+        if os.path.exists(path):
+            classpath.extend([os.path.join(path, dep) for dep in os.listdir(path)])
+
+        return ":".join(classpath)
+
+    def launch(self, launch_args: Optional[list[str]] = None):
+        os.chdir(self.path)
+
+        # Check for updates
+        has_updates = False
+        if self.auto_update_reach:
+            latest_reach = versions.get_latest_of("reach")
+            if self.version != latest_reach:
+                self.version = latest_reach
+                has_updates = True
+
+        if self.auto_update_quilt:
+            if self.is_modded():
+                latest_quilt = versions.get_latest_of("quilt")
+                if self.quilt_version != latest_quilt:
+                    self.quilt_version = latest_quilt
+                has_updates = True
+
+        if has_updates:
+            logger.info("Instance has updates!")
+            self.download(True)
+            self.save()
+
+        args = ["java"]
+        if not self.is_modded():
+            args.extend(["-jar", paths.path_to_cr(self.version)])
+        else:
+            args.extend([
+                f"-Dloader.gameJarPath={paths.path_to_cr(self.version)}",
+                "-classpath", self.get_classpath(),
+                "org.quiltmc.loader.impl.launch.knot.KnotClient"
+            ])
+        args.extend(self.args)
+        if launch_args is not None:
+            args.extend(launch_args)
+
+        logger.info(f"Launching \"{self.display_name}\" ({self.name}) with args {args} in folder {self.path}")
+        os.execvp("java", args)
+
+    def download(self, is_updating: bool = False):
+        cr_path = paths.path_to_cr(self.version)
+        if not os.path.isfile(cr_path):
+            net.download(f"{COSMIC_ARCHIVE_RAW_URL}/Cosmic Reach-{self.version}.jar", cr_path)
+
+        if self.is_modded() and not os.path.exists(paths.path_to_cq_deps(self.quilt_version)):
+            logger.info("Downloading Cosmic Quilt dependencies...")
+
+            pom = os.path.join(paths.path_to_cq_deps(self.quilt_version), "pom.xml")
+            deps = paths.path_to_cq_deps(self.quilt_version)
+            os.makedirs(deps, exist_ok = True)
+            maven.make_pom(pom, self.quilt_version)
+            maven.copy_deps(deps, deps)
+            os.remove(pom)
+
+            self.save()
+
+    def save(self):
+        os.makedirs(self.path, exist_ok = True)
+        with open(self.path_to("config.hjson"), "w") as f:
+            hjson.dump(Instance.get_hjson(self), f)
+
+    def get_mods(self) -> list[str]:
+        mods = []
+        mods_dir = self.path_to("mods")
+        if os.path.exists(mods_dir):
+            for mod_file in os.listdir(mods_dir):
+                if os.path.isdir(mod_file):
+                    continue
+                manifest = java_manifest.from_jar(os.path.join(mods_dir, mod_file))
+                mods.append(mod.Mod.from_data(manifest, mod_file))
+        return mods
+
+    # Static Methods
+    @staticmethod
+    def from_config_file(instance_name: str) -> "Instance":
+        if not Instance.exists(instance_name):
+            logger.error("Instance does not exist.")
+            exit(1)
 
-    if i.is_modded():
-        path = os.path.join(i.path_to("mods"), "assets")
-        os.makedirs(path, exist_ok = True)
-        shutil.copytree(mod, path, dirs_exist_ok = True)
-    elif ignore_global_warning:
-        if not os.path.exists(paths.CR_DIR):
-            logger.error("Global Cosmic Reach path does not exist. This should not happen.")
+        data = None
+        path = os.path.join(paths.INSTANCES, instance_name, "config.hjson")
+        with open(path, "r") as f:
+            data = hjson.load(f)
+        if data is None:
+            logger.error(f"Failed to load config at {path}")
             exit(1)
-        path = os.path.join(paths.CR_DIR, "mods", "assets")
-        shutil.copytree(mod, path, dirs_exist_ok = True)
 
-    logger.info("Done.")
+        ins = Instance(data["name"], data["version"], data["args"])
+        if "quilt-version" in data:
+            ins.quilt_version = data["quilt-version"]
+        if "display-name" in data:
+            ins.display_name = data["display-name"]
+        if "auto-update-reach" in data:
+            ins.auto_update_reach = data["auto-update-reach"]
+        if "auto-update-quilt" in data:
+            ins.auto_update_quilt = data["auto-update-quilt"]
+
+        return ins
+
+    @staticmethod
+    def make_instance(
+        instance_name: str,
+        cosmic_reach_version: str,
+        quilt_version: Optional[str] = None,
+        display_name: Optional[str] = None,
+    ) -> "Instance":
+        if not VALID_INSTANCE_NAME.match(instance_name):
+            logger.error("Instance name must match `[a-zA-Z0-9_-]*`")
+            exit(1)
 
+        reach_is_auto = cosmic_reach_version == "auto"
+        quilt_is_auto = quilt_version == "auto"
 
-@cosmix.command("whereis")
-@click.argument("name")
-def whereis(name: str):
-    i = Instance.get_or_throw(name)
-    logger.info(i.path)
+        cosmic_reach_version = versions.get_version_or_latest_of(
+            "reach",
+            "latest" if cosmic_reach_version == "auto" else cosmic_reach_version
+        )
+        quilt_version = versions.get_version_or_latest_of(
+            "quilt",
+            "latest" if quilt_version == "auto" else quilt_version
+        )
 
+        path = os.path.join(paths.INSTANCES, instance_name)
+        os.makedirs(path, exist_ok = True)
 
-if __name__ == "__main__":
-    cosmix()
+        instance = Instance(
+            instance_name,
+            cosmic_reach_version,
+            [],
+            quilt_version,
+            display_name,
+            reach_is_auto,
+            quilt_is_auto,
+        )
+        instance.save()
+        return instance
+
+    @staticmethod
+    def get_hjson(instance: "Instance") -> dict:
+        d = {
+            "name": instance.name,
+            "version": instance.version,
+            "args": instance.args,
+        }
+        if instance.is_modded():
+            d["quilt-version"] = instance.quilt_version
+        if instance.display_name != instance.name:
+            d["display-name"] = instance.display_name
+        if instance.auto_update_reach:
+            d["auto-update-reach"] = instance.auto_update_reach
+        if instance.auto_update_quilt:
+            d["auto-update-quilt"] = instance.auto_update_quilt
+        return d
+
+    @staticmethod
+    def exists(instance_name: str) -> bool:
+        return os.path.exists(os.path.join(paths.INSTANCES, instance_name))
+
+    @staticmethod
+    def get_or_throw(instance_name: str) -> Optional["Instance"]:
+        if not Instance.exists(instance_name):
+            logger.error("Instance does not exist.")
+            exit(1)
+        return Instance.from_config_file(instance_name)
```

### Comparing `cosmix_launcher-1.0.9/src/cosmix/api/config.py` & `cosmix_launcher-1.1.0/src/cosmix/api/config.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.9/src/cosmix/api/logger.py` & `cosmix_launcher-1.1.0/src/cosmix/api/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from . import config
-# import getpass
 import os
 
 
 __all__ = (
     "LEVELS",
     "sanatize_username",
     "log",
```

### Comparing `cosmix_launcher-1.0.9/src/cosmix/api/maven.py` & `cosmix_launcher-1.1.0/src/cosmix/api/maven.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.9/src/cosmix/api/mod.py` & `cosmix_launcher-1.1.0/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.9/src/cosmix/api/net.py` & `cosmix_launcher-1.1.0/src/cosmix/api/net.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.9/src/cosmix/api/paths.py` & `cosmix_launcher-1.1.0/src/cosmix/api/paths.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.9/src/cosmix/api/versions.py` & `cosmix_launcher-1.1.0/src/cosmix/api/versions.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,19 @@
     "LATEST_QUILT_URL",
     "SOURCES",
     "get_latest_of",
     "get_version_or_latest_of",
 )
 
 
-LATEST_REACH_URL = "https://raw.githubusercontent.com/CRModders/CosmicArchive/main/CurrentInstallableVersion.txt"
+LATEST_REACH_URL = "https://raw.githubusercontent.com/CRModders/CosmicArchive/main/versions.json"
 LATEST_QUILT_URL = "https://codeberg.org/api/v1/repos/CRModders/cosmic-quilt/releases/latest"
 SOURCES = {
-    "reach": lambda: net.get_data(LATEST_REACH_URL).strip().removeprefix("Cosmic Reach-").removesuffix(".jar"),
+    # TODO: Use `alpha`, `beta`, `release`, or whatever once CR changes latest versions
+    "reach": lambda: net.get_json(LATEST_REACH_URL)["latest"]["pre_alpha"],
     "quilt": lambda: net.get_json(LATEST_QUILT_URL)["tag_name"],
 }
 
 
 def get_latest_of(source: str) -> str:
     return SOURCES[source]()
```

### Comparing `cosmix_launcher-1.0.9/pyproject.toml` & `cosmix_launcher-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmix-launcher"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
     { name = "EmmaTheMartian", email="emmathemartian@gmail.com" },
 ]
 description = "A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -14,14 +14,15 @@
 dependencies = [
     "hjson",
     "tqdm",
     "requests",
     "crm1",
     "Send2Trash",
     "click",
+    "click-aliases",
     "java-manifest"
 ]
 
 [project.urls]
 Homepage = "https://codeberg.org/EmmaTheMartian/cosmix"
 Issues = "https://codeberg.org/EmmaTheMartian/cosmix/issues"
```

### Comparing `cosmix_launcher-1.0.9/readme.md` & `cosmix_launcher-1.1.0/readme.md`

 * *Files 21% similar despite different names*

```diff
@@ -15,117 +15,96 @@
 python3 -m pip install ./dist/*.whl
 ```
 
 To makes sure it's installed, run `cosmix version`. You should see `[info]: Cosmix <some version>` in the console.
 
 > If the command is not found, make sure your `~/.local/bin/` is on your `$PATH`.
 
+If you have any issues, see [Troubleshooting](#troubleshooting).
+
 <!--TODO: List the Windows script $PATH here as well.-->
 
 ### Updating
 
 ```sh
 python3 -m pip install --upgrade cosmix-launcher
 ```
 
 ### Uninstallation
 
 ```sh
 python3 -m pip uninstall cosmix-launcher
+# If you also want to delete your instances, delete ~/.local/share/cosmix (or %APPDATA%\cosmix on Windows)
 ```
 
 ### Troubleshooting
 
 **Arch Linux:**
 
 Arch Linux and its derivatives may complain with `error: externally-managed-environment`. To get around this, use the `--user --break-system-packages` options with `pip install`.
 
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
 **Maven:**
 
 You may also need to install Maven. On Arch Linux this is just `pacman -S maven`.
 
-> Maven is used to download and resolve all of Cosmic Quilt's dependencies automatically, hence why it is required.
+> Maven is used to download and resolve all of Cosmic Quilt's dependencies automatically. If you are a developer, you will probably have this downloaded already. You can check by running `mvn -v` in your terminal.
 
 ### Dependencies
 
-> `hjson tqdm requests crm1 Send2Trash click java-manifest`
+> `hjson tqdm requests crm1 Send2Trash click click-aliases java-manifest`
 
 To install and/or upgrade all of them at once, just run:
 
-`python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click java-manifest`
+`python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click click-aliases java-manifest`
 
 ## Usage
 
 ```
-global options:
-    --work-dir -w               specify a working directory for Cosmix to use.
-
-cosmix version
-    prints the current installed cosmix version
-
-cosmix debug
-    prints a lot of debug information related to cosmix
-
-cosmix add [instance]
-    adds and downloads a new instance
-    options:
-    --version -v VERSION        specify a Cosmic Reach version to use. defaults to "latest"
-    --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
-    --display-name -n NAME      optionally specify a display name for the instance
-
-cosmix update [instance]
-    updates an existing version
-    options:
-    --version -v VERSION        specify a Cosimc Reach version to use. defaults to "latest"
-    --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
-
-cosmix instances
-    lists all instances
-
-cosmix launch [instance]
-    launches an instance
+Usage: python -m src.cosmix [OPTIONS] COMMAND [ARGS]...
 
-cosmix info [instance]
-    prints info about an instance
-
-cosmix add-mod [instance] [path to mod jar]
-    adds a mod jar to an instance
-
-cosmix add-crm1-mod [instance] [mod id]
-    adds a mod to an instance via CRM-1. To add repos, see ~/.local/share/cosmix/config.hjson
-
-cosmix add-data-mod [instance] [mod path]
-    adds a data mod to an instance
-
-cosmic whereis [instance]
-    prints the path to a given instance
-
-cosmix trash [instance]
-    moves an instance to the system's trash folder
+Options:
+  -w, --work-dir TEXT  Set a working directory for Cosmix.
+  --help               Show this message and exit.
+
+Commands:
+  add (new)     Adds a new instance.
+  add-crm1-mod  Adds a jar mod via CRM-1.
+  add-data-mod  Adds a data mod.
+  add-mod       Adds a jar mod.
+  debug         Shows debug information.
+  info          Gets info about an instance.
+  instances     Shows all instances.
+  launch        Launches an instance.
+  trash         Trashes an instance.
+  update        Updates an existing instance.
+  version       Shows the current cosmix version.
+  whereis       Shows the path to an instance.
 ```
 
+> You can use `cosmix [command] --help` to get help about a specific command.
+
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
-cosmix add vanilla
+cosmix new vanilla
 # Create a Cosmic Quilt instance named `my-quilt` on the latest CR version with Cosmic Quilt 1.2.7
-cosmix add my-quilt --quilt-version 1.2.7
+cosmix new my-quilt --quilt-version 1.2.7
 # Create a vanilla instance named `old-version` on CR 0.0.1
-cosmix add old-version -v 0.0.1
+cosmix new old-version -v 0.0.1
 # Install the latest version of Flux API available on JoJoJux's autorepo to the instance `test`
 cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
 cosmix update latest -v latest -q latest
 ```
 
 ## File Structure
 
-Cosmix stores all of its data in your `$XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
+Cosmix stores all of its data in your `$XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%APPDATA%` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
     config.hjson - Configs for Cosmix
 
     deps/
```

### Comparing `cosmix_launcher-1.0.9/PKG-INFO` & `cosmix_launcher-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.9
+Version: 1.1.0
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: click
+Requires-Dist: click-aliases
 Requires-Dist: crm1
 Requires-Dist: hjson
 Requires-Dist: java-manifest
 Requires-Dist: requests
 Requires-Dist: send2trash
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
@@ -34,117 +35,96 @@
 python3 -m pip install ./dist/*.whl
 ```
 
 To makes sure it's installed, run `cosmix version`. You should see `[info]: Cosmix <some version>` in the console.
 
 > If the command is not found, make sure your `~/.local/bin/` is on your `$PATH`.
 
+If you have any issues, see [Troubleshooting](#troubleshooting).
+
 <!--TODO: List the Windows script $PATH here as well.-->
 
 ### Updating
 
 ```sh
 python3 -m pip install --upgrade cosmix-launcher
 ```
 
 ### Uninstallation
 
 ```sh
 python3 -m pip uninstall cosmix-launcher
+# If you also want to delete your instances, delete ~/.local/share/cosmix (or %APPDATA%\cosmix on Windows)
 ```
 
 ### Troubleshooting
 
 **Arch Linux:**
 
 Arch Linux and its derivatives may complain with `error: externally-managed-environment`. To get around this, use the `--user --break-system-packages` options with `pip install`.
 
 > Obviously this has a chance of breaking something, but in my testing I have yet to have that happen. Though be aware and know that I am not responsible if you break your system.
 
 **Maven:**
 
 You may also need to install Maven. On Arch Linux this is just `pacman -S maven`.
 
-> Maven is used to download and resolve all of Cosmic Quilt's dependencies automatically, hence why it is required.
+> Maven is used to download and resolve all of Cosmic Quilt's dependencies automatically. If you are a developer, you will probably have this downloaded already. You can check by running `mvn -v` in your terminal.
 
 ### Dependencies
 
-> `hjson tqdm requests crm1 Send2Trash click java-manifest`
+> `hjson tqdm requests crm1 Send2Trash click click-aliases java-manifest`
 
 To install and/or upgrade all of them at once, just run:
 
-`python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click java-manifest`
+`python3 -m pip install --upgrade hjson tqdm requests crm1 Send2Trash click click-aliases java-manifest`
 
 ## Usage
 
 ```
-global options:
-    --work-dir -w               specify a working directory for Cosmix to use.
-
-cosmix version
-    prints the current installed cosmix version
-
-cosmix debug
-    prints a lot of debug information related to cosmix
-
-cosmix add [instance]
-    adds and downloads a new instance
-    options:
-    --version -v VERSION        specify a Cosmic Reach version to use. defaults to "latest"
-    --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
-    --display-name -n NAME      optionally specify a display name for the instance
-
-cosmix update [instance]
-    updates an existing version
-    options:
-    --version -v VERSION        specify a Cosimc Reach version to use. defaults to "latest"
-    --quilt-version -q VERSION  specify a Cosmic Quilt version to use. defaults to "none"
-
-cosmix instances
-    lists all instances
-
-cosmix launch [instance]
-    launches an instance
+Usage: python -m src.cosmix [OPTIONS] COMMAND [ARGS]...
 
-cosmix info [instance]
-    prints info about an instance
-
-cosmix add-mod [instance] [path to mod jar]
-    adds a mod jar to an instance
-
-cosmix add-crm1-mod [instance] [mod id]
-    adds a mod to an instance via CRM-1. To add repos, see ~/.local/share/cosmix/config.hjson
-
-cosmix add-data-mod [instance] [mod path]
-    adds a data mod to an instance
-
-cosmic whereis [instance]
-    prints the path to a given instance
-
-cosmix trash [instance]
-    moves an instance to the system's trash folder
+Options:
+  -w, --work-dir TEXT  Set a working directory for Cosmix.
+  --help               Show this message and exit.
+
+Commands:
+  add (new)     Adds a new instance.
+  add-crm1-mod  Adds a jar mod via CRM-1.
+  add-data-mod  Adds a data mod.
+  add-mod       Adds a jar mod.
+  debug         Shows debug information.
+  info          Gets info about an instance.
+  instances     Shows all instances.
+  launch        Launches an instance.
+  trash         Trashes an instance.
+  update        Updates an existing instance.
+  version       Shows the current cosmix version.
+  whereis       Shows the path to an instance.
 ```
 
+> You can use `cosmix [command] --help` to get help about a specific command.
+
 **Examples**
 ```sh
 # Create an unmodded instance named `vanilla` on the latest CR version
-cosmix add vanilla
+cosmix new vanilla
 # Create a Cosmic Quilt instance named `my-quilt` on the latest CR version with Cosmic Quilt 1.2.7
-cosmix add my-quilt --quilt-version 1.2.7
+cosmix new my-quilt --quilt-version 1.2.7
 # Create a vanilla instance named `old-version` on CR 0.0.1
-cosmix add old-version -v 0.0.1
+cosmix new old-version -v 0.0.1
 # Install the latest version of Flux API available on JoJoJux's autorepo to the instance `test`
 cosmix add-crm1-mod test dev.crmodders.flux
 # Update the `latest` instance to the latest available versions of Cosmic Reach and Cosmic Quilt
 cosmix update latest -v latest -q latest
 ```
 
 ## File Structure
 
-Cosmix stores all of its data in your `$XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%appdata%` on Windows and in the `cosmix` folder.
+Cosmix stores all of its data in your `$XDG_DATA_HOME` (typically `~/.local/share/`) on Linux and `%APPDATA%` on Windows and in the `cosmix` folder.
 
 This folder will contain the following extra folders:
 ```
 cosmix/
     config.hjson - Configs for Cosmix
 
     deps/
```

