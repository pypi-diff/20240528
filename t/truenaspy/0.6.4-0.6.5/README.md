# Comparing `tmp/truenaspy-0.6.4.tar.gz` & `tmp/truenaspy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truenaspy-0.6.4.tar", last modified: Mon May 27 16:47:26 2024, max compression
+gzip compressed data, was "truenaspy-0.6.5.tar", last modified: Tue May 28 08:39:09 2024, max compression
```

## Comparing `truenaspy-0.6.4.tar` & `truenaspy-0.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.742401 truenaspy-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.738401 truenaspy-0.6.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.738401 truenaspy-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-27 16:47:11.000000 truenaspy-0.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 16:47:11.000000 truenaspy-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-27 16:47:11.000000 truenaspy-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 16:47:26.742401 truenaspy-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-27 16:47:11.000000 truenaspy-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-27 16:47:11.000000 truenaspy-0.6.4/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-27 16:47:11.000000 truenaspy-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 16:47:11.000000 truenaspy-0.6.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-27 16:47:11.000000 truenaspy-0.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 16:47:26.742401 truenaspy-0.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.738401 truenaspy-0.6.4/truenaspy/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/collects.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-27 16:47:11.000000 truenaspy-0.6.4/truenaspy/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:47:26.742401 truenaspy-0.6.4/truenaspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-27 16:47:26.000000 truenaspy-0.6.4/truenaspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:39:09.892608 truenaspy-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:39:09.888608 truenaspy-0.6.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-28 08:39:01.000000 truenaspy-0.6.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:39:09.888608 truenaspy-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-28 08:39:01.000000 truenaspy-0.6.5/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 08:39:01.000000 truenaspy-0.6.5/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-28 08:39:01.000000 truenaspy-0.6.5/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-28 08:39:01.000000 truenaspy-0.6.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-28 08:39:01.000000 truenaspy-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-28 08:39:01.000000 truenaspy-0.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 08:39:01.000000 truenaspy-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 08:39:01.000000 truenaspy-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-28 08:39:09.892608 truenaspy-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-28 08:39:01.000000 truenaspy-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-28 08:39:01.000000 truenaspy-0.6.5/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-28 08:39:01.000000 truenaspy-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 08:39:01.000000 truenaspy-0.6.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 08:39:01.000000 truenaspy-0.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:39:09.892608 truenaspy-0.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:39:09.888608 truenaspy-0.6.5/truenaspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-28 08:39:01.000000 truenaspy-0.6.5/truenaspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23468 2024-05-28 08:39:01.000000 truenaspy-0.6.5/truenaspy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-28 08:39:01.000000 truenaspy-0.6.5/truenaspy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-28 08:39:01.000000 truenaspy-0.6.5/truenaspy/collects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 08:39:01.000000 truenaspy-0.6.5/truenaspy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-28 08:39:01.000000 truenaspy-0.6.5/truenaspy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-28 08:39:01.000000 truenaspy-0.6.5/truenaspy/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:39:09.888608 truenaspy-0.6.5/truenaspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-28 08:39:09.000000 truenaspy-0.6.5/truenaspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-28 08:39:09.000000 truenaspy-0.6.5/truenaspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:39:09.000000 truenaspy-0.6.5/truenaspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:39:09.000000 truenaspy-0.6.5/truenaspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 08:39:09.000000 truenaspy-0.6.5/truenaspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 08:39:09.000000 truenaspy-0.6.5/truenaspy.egg-info/top_level.txt
```

### Comparing `truenaspy-0.6.4/.github/dependabot.yml` & `truenaspy-0.6.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/.github/workflows/auto-approve.yml` & `truenaspy-0.6.5/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/.github/workflows/lint.yml` & `truenaspy-0.6.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/.github/workflows/pythonpublish.yml` & `truenaspy-0.6.5/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/.github/workflows/release.yml` & `truenaspy-0.6.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/.gitignore` & `truenaspy-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/.pre-commit-config.yaml` & `truenaspy-0.6.5/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ---
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.4
+    rev: v0.4.5
     hooks:
       - id: ruff
         args:
           - --fix
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.6
+    rev: v2.3.0
     hooks:
       - id: codespell
         args:
           - --ignore-words-list=fro,hass
           - --skip="./.*,*.csv,*.json,*.ambr"
           - --quiet-level=2
         exclude_types: [csv, json]
```

### Comparing `truenaspy-0.6.4/LICENSE` & `truenaspy-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/PKG-INFO` & `truenaspy-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truenaspy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Provides asynchronous authentication and access to Truenas devices
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: async,truenas,scale,core
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `truenaspy-0.6.4/README.md` & `truenaspy-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/example.py` & `truenaspy-0.6.5/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     await api.async_get_interfaces()
     await api.async_get_services()
     await api.async_get_datasets()
     await api.async_get_pools()
     await api.async_get_disks()
     await api.async_get_jails()
     await api.async_get_virtualmachines()
-    await api.async_get_cloudsync()
+    await api.async_get_cloudsyncs()
     await api.async_get_replications()
     await api.async_get_snapshottasks()
     await api.async_get_charts()
     await api.async_close()
 
     # ==================
     # Subscribe at Event
```

### Comparing `truenaspy-0.6.4/pyproject.toml` & `truenaspy-0.6.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,7 +42,11 @@
 force-sort-within-sections = true
 combine-as-imports = true
 split-on-trailing-comma = false
 
 [[tool.mypy.overrides]]
 module = "yaml"
 ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "pytz"
+ignore_missing_imports = true
```

### Comparing `truenaspy-0.6.4/truenaspy/api.py` & `truenaspy-0.6.5/truenaspy/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -196,14 +196,28 @@
             # if item.get("name") == "arcresult":
             #     tmp_arr = []
             #     systemstats_process(self.system_infos, tmp_arr, item, "arc")
 
         self._sub.notify(Events.SYSTEM.value)
         return self.system_infos
 
+    async def async_restart_system(self) -> None:
+        """Restart system."""
+        await self.async_request("system/reboot", method="post")
+
+    async def async_shutdown_system(self) -> None:
+        """Restart system."""
+        await self.async_request("system/shutdown", method="post")
+
+    async def async_update_system(self, reboot: bool = False) -> None:
+        """Update system."""
+        await self.async_request(
+            "update/update", method="post", json={"reboot": reboot}
+        )
+
     async def async_get_interfaces(self) -> list[dict[str, Any]]:
         """Get interface info from TrueNAS."""
         response = await self.async_request("interface")
         self.interfaces = search_attrs(Interfaces, response)
 
         # Get stats
         query = [
@@ -283,14 +297,42 @@
     async def async_get_services(self) -> list[dict[str, Any]]:
         """Get service info from TrueNAS."""
         response = await self.async_request("service")
         self.services = search_attrs(Service, response)
         self._sub.notify(Events.SERVICES.value)
         return self.services
 
+    async def async_get_service(self, id: int) -> Any:
+        """Get Service from TrueNAS."""
+        return await self.async_request(f"service/id/{id}")
+
+    async def async_reload_service(self, service: str) -> None:
+        """Reload service."""
+        await self.async_request(
+            "service/reload", method="post", json={"service": service}
+        )
+
+    async def async_restart_service(self, service: str) -> None:
+        """Restart service."""
+        await self.async_request(
+            "service/restart", method="post", json={"service": service}
+        )
+
+    async def async_stop_service(self, service: str) -> None:
+        """Stop service."""
+        await self.async_request(
+            "service/stop", method="post", json={"service": service}
+        )
+
+    async def async_start_service(self, service: str) -> None:
+        """Start service."""
+        await self.async_request(
+            "service/start", method="post", json={"service": service}
+        )
+
     async def async_get_pools(self) -> list[dict[str, Any]]:
         """Get pools from TrueNAS."""
         response = await self.async_request("pool")
         self.pools = search_attrs(Pool, response)
 
         try:
             response = await self.async_request("boot/get_state")
@@ -360,28 +402,68 @@
                 self.jails = search_attrs(Jail, response)
             except NotFoundError as error:
                 _LOGGER.warning(error)
                 self.jails = []
         self._sub.notify(Events.JAILS.value)
         return self.jails
 
+    async def async_get_jail(self, id: int) -> Any:
+        """Get jail."""
+        return await self.async_request(f"jail/id/{id}")
+
+    async def async_restart_jail(self, id: int) -> None:
+        """Restart jail."""
+        await self.async_request("jail/restart", method="post", json={"jail": id})
+
+    async def async_stop_jail(self, id: int) -> None:
+        """Stop jail."""
+        await self.async_request("jail/stop", method="post", json={"jail": id})
+
+    async def async_start_jail(self, id: int) -> None:
+        """Start jail."""
+        await self.async_request("jail/start", method="post", json={"jail": id})
+
     async def async_get_virtualmachines(self) -> list[dict[str, Any]]:
         """Get VMs from TrueNAS."""
         response = await self.async_request("vm")
         self.virtualmachines = search_attrs(VirtualMachine, response)
         self._sub.notify(Events.VMS.value)
         return self.virtualmachines
 
-    async def async_get_cloudsync(self) -> list[dict[str, Any]]:
+    async def async_get_virtualmachine(self, id: int) -> Any:
+        """Get virtualmachine."""
+        return await self.async_request(f"vm/id/{id}")
+
+    async def async_stop_virtualmachine(self, id: int) -> None:
+        """Stop virtualmachine."""
+        await self.async_request(f"vm/id/{id}/stop", method="post")
+
+    async def async_start_virtualmachine(
+        self, id: int, overcommit: bool = False
+    ) -> None:
+        """Start virtualmachine."""
+        await self.async_request(
+            f"vm/id/{id}/start", method="post", json={"overcommit": overcommit}
+        )
+
+    async def async_get_cloudsyncs(self) -> list[dict[str, Any]]:
         """Get cloudsync from TrueNAS."""
         response = await self.async_request("cloudsync")
         self.cloudsync = search_attrs(CloudSync, response)
         self._sub.notify(Events.CLOUD.value)
         return self.cloudsync
 
+    async def async_get_cloudsync(self, id: int) -> Any:
+        """Get cloudsync job."""
+        return await self.async_request(f"cloudsync/id/{id}")
+
+    async def async_sync_cloudsync(self, id: int) -> None:
+        """Sync cloudsync job."""
+        await self.async_request(f"cloudsync/id/{id}/sync", method="post")
+
     async def async_get_replications(self) -> list[dict[str, Any]]:
         """Get replication from TrueNAS."""
         response = await self.async_request("replication")
         self.replications = search_attrs(Replication, response)
         self._sub.notify(Events.REPLS.value)
         return self.replications
 
@@ -395,14 +477,46 @@
     async def async_get_charts(self) -> list[dict[str, Any]]:
         """Get Charts from TrueNAS."""
         response = await self.async_request("chart/release")
         self.charts = search_attrs(Charts, response)
         self._sub.notify(Events.CHARTS.value)
         return self.charts
 
+    async def async_get_chart(self, id: int) -> Any:
+        """Get Charts from TrueNAS."""
+        return await self.async_request(f"chart/release/id/{id}")
+
+    async def async_update_chart(self, id: int) -> None:
+        """Update chart."""
+        await self.async_request(
+            "chart/release/upgrade", method="post", json={"release_name": id}
+        )
+
+    async def async_update_chart_image(self, repo: str, tag: str) -> None:
+        """Update chart image."""
+        await self.async_request(
+            "container/image/pull", method="post", json={"from_image": repo, "tag": tag}
+        )
+
+    async def async_stop_chart(self, id: int, replicas: int = 0) -> None:
+        """Stop chart."""
+        await self.async_request(
+            "chart/release/scale",
+            method="post",
+            json={"release_name": id, "scale_options": {"replica_count": replicas}},
+        )
+
+    async def async_start_chart(self, id: int, replicas: int = 1) -> None:
+        """Start chart."""
+        await self.async_request(
+            "chart/release/scale",
+            method="post",
+            json={"release_name": id, "scale_options": {"replica_count": replicas}},
+        )
+
     async def async_get_smartdisks(self) -> list[dict[str, Any]]:
         """Get smartdisk from TrueNAS."""
         response = await self.async_request("smart/test/results", params={"offset": 1})
         self.smartdisks = search_attrs(Smart, response)
         self._sub.notify(Events.SMARTS.value)
         return self.smartdisks
 
@@ -416,48 +530,73 @@
     async def async_get_rsynctasks(self) -> list[dict[str, Any]]:
         """Get smartdisk from TrueNAS."""
         response = await self.async_request("rsynctask")
         self.rsynctasks = search_attrs(Rsync, response)
         self._sub.notify(Events.RSYNC.value)
         return self.rsynctasks
 
+    async def async_get_update_system(self) -> Any:
+        """Check update available."""
+        return await self.async_request("update/check_available", method="post")
+
+    async def async_get_trains(self) -> Any:
+        """Get trains update."""
+        return await self.async_request("update/get_trains")
+
+    async def async_get_jobs(self) -> Any:
+        """Get core jobs."""
+        return await self.async_request("core/get_jobs")
+
+    async def async_get_job(self, id: int) -> Any:
+        """Get core job."""
+        return await self.async_request("core/get_jobs", params={"id": id})
+
     async def async_get_update(self) -> dict[str, Any]:
         """Get update info from TrueNAS."""
         try:
-            response = await self.async_request("update/check_available", "post")
+            response = await self.async_get_update_system()
         except TruenasException as error:
             _LOGGER.debug(error)
             response = ExtendedDict()
         self.update_infos = search_attrs(Update, response)
 
         try:
-            response = await self.async_request("update/get_trains")
+            response = await self.async_get_trains()
         except TruenasException as error:
             _LOGGER.debug(error)
             response = ExtendedDict()
         self.update_infos.update({"current_train": response.get("current")})
 
-        if jobid := self.system_infos.get("job_id", 0):
-            response = await self.async_request("core/get_jobs", params={"id": jobid})
+        if job_id := self.system_infos.get("job_id", 0):
+            response = await self.async_get_job(job_id)
             jobs = search_attrs(Job, response)
             for job in jobs:
                 if (
                     job.get("state") != "RUNNING"
                     or not self.update_infos["update_available"]
                 ):
                     self.update_infos.update(
                         {"progress": 0, "status": None, "job_id": 0}
                     )
         return self.update_infos
 
     async def async_is_alive(self) -> bool:
         """Check connection."""
-        result = await self.auth.async_request("core/ping")
+        result = await self.async_request("core/ping")
         return "pong" in result
 
+    async def async_take_snapshot(self, name: str) -> None:
+        """Create dataset snapshot."""
+        ts = datetime.now().isoformat(sep="_", timespec="microseconds")
+        await self.async_request(
+            "zfs/snapshot",
+            method="post",
+            json={"dataset": name, "name": f"custom-{ts}"},
+        )
+
     def subscribe(self, _callback: str, *args: Any) -> None:
         """Subscribe event."""
         self._sub.subscribe(_callback, *args)
 
     def unsubscribe(self, _callback: str, *args: Any) -> None:
         """Unsubscribe event."""
         self._sub.subscribe(_callback, *args)
```

### Comparing `truenaspy-0.6.4/truenaspy/auth.py` & `truenaspy-0.6.5/truenaspy/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,15 @@
             {
                 "Accept": "application/json",
                 "Authorization": f"Bearer {self._access_token}",
             }
         )
         try:
             async with asyncio.timeout(self._timeout):
-                _LOGGER.debug(
-                    "Url: %s (%s) - Content: %s", path, method, kwargs.get("json")
-                )
+                _LOGGER.debug("Request: %s (%s) - %s", path, method, kwargs.get("json"))
                 response = await self._session.request(
                     method, f"{self._url}/{path}", **kwargs
                 )
                 response.raise_for_status()
         except (asyncio.CancelledError, asyncio.TimeoutError) as error:
             msg = "Timeout occurred while connecting to the Truenas API"
             raise TimeoutExceededError(msg) from error
```

### Comparing `truenaspy-0.6.4/truenaspy/collects.py` & `truenaspy-0.6.5/truenaspy/collects.py`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/truenaspy/helper.py` & `truenaspy-0.6.5/truenaspy/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from datetime import datetime
 from functools import reduce
 import json
 from logging import getLogger
 from typing import Any, Callable, Type
 
-from pytz import utc  # type: ignore[import-untyped]
+from pytz import utc
 
 _LOGGER = getLogger(__name__)
 
 
 class ExtendedDict(dict[Any, Any]):
     """Extend dictionary class."""
```

### Comparing `truenaspy-0.6.4/truenaspy/subscription.py` & `truenaspy-0.6.5/truenaspy/subscription.py`

 * *Files identical despite different names*

### Comparing `truenaspy-0.6.4/truenaspy.egg-info/PKG-INFO` & `truenaspy-0.6.5/truenaspy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truenaspy
-Version: 0.6.4
+Version: 0.6.5
 Summary: Provides asynchronous authentication and access to Truenas devices
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: async,truenas,scale,core
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `truenaspy-0.6.4/truenaspy.egg-info/SOURCES.txt` & `truenaspy-0.6.5/truenaspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

