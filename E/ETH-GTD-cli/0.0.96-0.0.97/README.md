# Comparing `tmp/eth_gtd_cli-0.0.96.tar.gz` & `tmp/eth_gtd_cli-0.0.97.tar.gz`

## Comparing `eth_gtd_cli-0.0.96.tar` & `eth_gtd_cli-0.0.97.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/deploy.sh
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/src/ETH_GTD_cli/__init__.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/src/ETH_GTD_cli/auth.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/src/ETH_GTD_cli/consts.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/src/ETH_GTD_cli/helper.py
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/src/ETH_GTD_cli/main.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/LICENSE
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/pyproject.toml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.96/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/deploy.sh
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/src/ETH_GTD_cli/__init__.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/src/ETH_GTD_cli/auth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/src/ETH_GTD_cli/consts.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/src/ETH_GTD_cli/helper.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/src/ETH_GTD_cli/main.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/LICENSE
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/pyproject.toml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 eth_gtd_cli-0.0.97/PKG-INFO
```

### Comparing `eth_gtd_cli-0.0.96/src/ETH_GTD_cli/auth.py` & `eth_gtd_cli-0.0.97/src/ETH_GTD_cli/auth.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.96/src/ETH_GTD_cli/helper.py` & `eth_gtd_cli-0.0.97/src/ETH_GTD_cli/helper.py`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.96/src/ETH_GTD_cli/main.py` & `eth_gtd_cli-0.0.97/src/ETH_GTD_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,18 +345,18 @@
     response = client.post(f"{API_URL}/user/demote", json={"email": email})
     response.raise_for_status()
     print("User demoted.")
 
 
 @files.command("download")
 def download(
-        runUUID: Annotated[str, typer.Argument()],
+        runuuid: Annotated[str, typer.Argument()],
 ):
     try:
-        response = client.get(f"{API_URL}/file/downloadWithToken", params={"uuid": runUUID})
+        response = client.get(f"{API_URL}/file/downloadWithToken", params={"uuid": runuuid})
         response.raise_for_status()
         print(response.json())
     except:
         print("Failed to download file")
 
 if __name__ == "__main__":
     app()
```

### Comparing `eth_gtd_cli-0.0.96/LICENSE` & `eth_gtd_cli-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `eth_gtd_cli-0.0.96/pyproject.toml` & `eth_gtd_cli-0.0.97/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ETH_GTD_cli"
-version = "0.0.96"
+version = "0.0.97"
 authors = [
   { name="Johann Schwabe", email="jschwab@ethz.ch" },
 ]
 description = "A CLI for the ETH project Grand Tour"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `eth_gtd_cli-0.0.96/PKG-INFO` & `eth_gtd_cli-0.0.97/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ETH_GTD_cli
-Version: 0.0.96
+Version: 0.0.97
 Summary: A CLI for the ETH project Grand Tour
 Project-URL: Homepage, https://github.com/leggedrobotics/GrandTourDatasets
 Project-URL: Issues, https://github.com/leggedrobotics/GrandTourDatasets/issues
 Author-email: Johann Schwabe <jschwab@ethz.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

