# Comparing `tmp/nexus_pcv-0.1.6.tar.gz` & `tmp/nexus_pcv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus_pcv-0.1.6.tar", max compression
+gzip compressed data, was "nexus_pcv-0.2.0.tar", max compression
```

## Comparing `nexus_pcv-0.1.6.tar` & `nexus_pcv-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    16295 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/LICENSE
--rw-r--r--   0        0        0     4292 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/README.md
--rw-r--r--   0        0        0      394 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/__init__.py
--rw-r--r--   0        0        0      169 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/__main__.py
--rw-r--r--   0        0        0     5456 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/apic.py
--rw-r--r--   0        0        0        0 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/cli/__init__.py
--rw-r--r--   0        0        0     2488 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/cli/main.py
--rw-r--r--   0        0        0     4210 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/cli/options.py
--rw-r--r--   0        0        0     5879 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/const.py
--rw-r--r--   0        0        0    11189 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/nae.py
--rw-r--r--   0        0        0     8224 2024-05-08 19:37:40.519698 nexus_pcv-0.1.6/nexus_pcv/ndi.py
--rw-r--r--   0        0        0    10017 2024-05-08 19:37:40.523698 nexus_pcv-0.1.6/nexus_pcv/pcv.py
--rw-r--r--   0        0        0     1914 2024-05-08 19:37:40.523698 nexus_pcv-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 nexus_pcv-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4150 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/README.md
+-rw-r--r--   0        0        0      281 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/__main__.py
+-rw-r--r--   0        0        0     5456 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/apic.py
+-rw-r--r--   0        0        0        0 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/cli/__init__.py
+-rw-r--r--   0        0        0     2259 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/cli/main.py
+-rw-r--r--   0        0        0     4307 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/cli/options.py
+-rw-r--r--   0        0        0     5879 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/const.py
+-rw-r--r--   0        0        0     8142 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/ndi.py
+-rw-r--r--   0        0        0     8433 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/nexus_pcv/pcv.py
+-rw-r--r--   0        0        0     1854 2024-05-28 10:32:29.473260 nexus_pcv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5213 1970-01-01 00:00:00.000000 nexus_pcv-0.2.0/PKG-INFO
```

### Comparing `nexus_pcv-0.1.6/LICENSE` & `nexus_pcv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.6/README.md` & `nexus_pcv-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 [![Tests](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml/badge.svg)](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml)
-![Python Support](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational "Python Support: 3.7, 3.8, 3.9, 3.10")
+![Python Support](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-informational "Python Support: 3.8, 3.9, 3.10, 3.11, 3.12")
 
 # nexus-pcv
 
-A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine. It can either work with provided JSON file(s) or a `terraform plan` output from a [Nexus as Code](https://cisco.com/go/nexusascode) project. It waits for the analysis to complete and evaluates the results.
+A CLI tool to perform a pre-change validation on Nexus Dashboard Insights. It can either work with provided JSON file(s) or a `terraform plan` output from a [Nexus as Code](https://cisco.com/go/nexusascode) project. It waits for the analysis to complete and evaluates the results.
 
 ```
 $ nexus-pcv -h
 Usage: nexus-pcv [OPTIONS]
 
-  A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or
-  Network Assurance Engine.
+  A CLI tool to perform a pre-change validation on Nexus Dashboard Insights.
 
 Options:
-  --version                   Show the version and exit.
-  -v, --verbosity LVL         Either CRITICAL, ERROR, WARNING, INFO or DEBUG.
-  -i, --hostname-ip TEXT      NAE/ND hostname or IP (required, env:
-                              PCV_HOSTNAME_IP).
-  -u, --username TEXT         NAE/ND username (required, env: PCV_USERNAME).
-  -p, --password TEXT         NAE/ND password (required, env: PCV_PASSWORD).
-  -d, --domain TEXT           NAE/ND login domain (optional, default: 'Local',
-                              env: PCV_DOMAIN).
-  -g, --group TEXT            NAE assurance group name or NDI insights group
-                              name (required, env: PCV_GROUP).
-  -s, --site TEXT             NDI site or fabric name (optional, only required
-                              for NDI, env: PCV_SITE).
-  -n, --name TEXT             NAE/NDI pre-change validation name (optional,
-                              env: PCV_NAME).
-  -s, --suppress-events TEXT  NAE/NDI comma-separated list of events to
-                              suppress (optional, default: 'APP_EPG_NOT_DEPLOY
-                              ED,APP_EPG_HAS_NO_CONTRACT_IN_ENFORCED_VRF',
-                              env: PCV_SUPPRESS_EVENTS).
-  -t, --timeout INTEGER       NAE/NDI pre-change validation timeout in minutes
-                              (optional, default: 15, env: PCV_TIMEOUT).
-  -f, --file FILE             NAE/NDI proposed change JSON file (optional,
-                              env: PCV_FILE).
-  -t, --nac-tf-plan FILE      NAE/NDI proposed change Terraform plan output
-                              (optional, env: PCV_NAC_TF_PLAN).
-  -o, --output-summary FILE   NAE/NDI summary of new events/anomalies written
-                              to a file (optional, env: PCV_OUTPUT_SUMMARY).
-  -r, --output-url FILE       NAE/NDI link (URL) to pre-change validation
-                              results written to a file (optional, env:
-                              PCV_OUTPUT_URL).
-  -h, --help                  Show this message and exit.
+  --version                  Show the version and exit.
+  -v, --verbosity LVL        Either CRITICAL, ERROR, WARNING, INFO or DEBUG.
+  -i, --hostname-ip TEXT     ND hostname or IP (required, env:
+                             PCV_HOSTNAME_IP).
+  -u, --username TEXT        ND username (required, env: PCV_USERNAME).
+  -p, --password TEXT        ND password (required, env: PCV_PASSWORD).
+  -d, --domain TEXT          ND login domain (optional, default: 'local', env:
+                             PCV_DOMAIN).
+  -g, --group TEXT           NDI insights group name (optional, default:
+                             'default', env: PCV_GROUP).
+  -s, --site TEXT            NDI site or fabric name (required, env:
+                             PCV_SITE).
+  -n, --name TEXT            NDI pre-change validation name (optional, env:
+                             PCV_NAME).
+  --suppress-events TEXT     NDI comma-separated list of events to suppress
+                             (optional, default: 'APP_EPG_NOT_DEPLOYED,APP_EPG
+                             _HAS_NO_CONTRACT_IN_ENFORCED_VRF', env:
+                             PCV_SUPPRESS_EVENTS).
+  --timeout INTEGER          NDI pre-change validation timeout in minutes
+                             (optional, default: 15, env: PCV_TIMEOUT).
+  -f, --file FILE            NDI proposed change JSON file (optional, env:
+                             PCV_FILE).
+  -t, --nac-tf-plan FILE     NDI proposed change Terraform plan output
+                             (optional, env: PCV_NAC_TF_PLAN).
+  -o, --output-summary FILE  NDI summary of new events/anomalies written to a
+                             file (optional, env: PCV_OUTPUT_SUMMARY).
+  -r, --output-url FILE      NDI link (URL) to pre-change validation results
+                             written to a file (optional, env:
+                             PCV_OUTPUT_URL).
+  -h, --help                 Show this message and exit.
 ```
 
 ## Installation
 
 Python 3.7+ is required to install `nexus-pcv`. Don't have Python 3.7 or later? See [Python 3 Installation & Setup Guide](https://realpython.com/installing-python/).
 
 `nexus-pcv` can be installed in a virtual environment using `pip`:
```

### Comparing `nexus_pcv-0.1.6/nexus_pcv/apic.py` & `nexus_pcv-0.2.0/nexus_pcv/apic.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.6/nexus_pcv/cli/main.py` & `nexus_pcv-0.2.0/nexus_pcv/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,29 +73,25 @@
     suppress_events: str,
     timeout: int,
     file: List[str],
     nac_tf_plan: str,
     output_summary: str,
     output_url: str,
 ) -> None:
-    """A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine."""
+    """A CLI tool to perform a pre-change validation on Nexus Dashboard Insights."""
     configure_logging(verbosity)
 
-    platform = PCV.Platform.NDI if site else PCV.Platform.NAE
-    pcv = PCV(hostname_ip, username, password, domain, timeout, platform)
+    pcv = PCV(hostname_ip, username, password, domain, timeout)
     if file:
         pcv.load_json_files(file)
     if nac_tf_plan:
         pcv.load_tf_plan(nac_tf_plan)
     if error_handler.fired:
         exit()
-    if platform is PCV.Platform.NDI:
-        pcv.ndi_pcv(name, group, site, suppress_events, output_summary, output_url)
-    else:
-        pcv.nae_pcv(name, group, suppress_events, output_summary, output_url)
+    pcv.ndi_pcv(name, group, site, suppress_events, output_summary, output_url)
     exit()
 
 
 def exit() -> None:
     if error_handler.fired:
         sys.exit(1)
     else:
```

### Comparing `nexus_pcv-0.1.6/nexus_pcv/cli/options.py` & `nexus_pcv-0.2.0/nexus_pcv/cli/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,118 +32,127 @@
 
 
 hostname_ip = click.option(
     "-i",
     "--hostname-ip",
     type=str,
     envvar="PCV_HOSTNAME_IP",
-    help="NAE/ND hostname or IP (required, env: PCV_HOSTNAME_IP).",
+    help="ND hostname or IP (required, env: PCV_HOSTNAME_IP).",
+    required=True,
 )
 
 username = click.option(
     "-u",
     "--username",
     type=str,
     envvar="PCV_USERNAME",
-    help="NAE/ND username (required, env: PCV_USERNAME).",
+    help="ND username (required, env: PCV_USERNAME).",
+    required=True,
 )
 
 password = click.option(
     "-p",
     "--password",
     type=str,
     envvar="PCV_PASSWORD",
-    help="NAE/ND password (required, env: PCV_PASSWORD).",
+    help="ND password (required, env: PCV_PASSWORD).",
     prompt=True,
     hide_input=True,
     confirmation_prompt=True,
+    required=True,
 )
 
 domain = click.option(
     "-d",
     "--domain",
     type=str,
-    default="Local",
+    default="local",
     envvar="PCV_DOMAIN",
-    help="NAE/ND login domain (optional, default: 'Local/local', env: PCV_DOMAIN).",
+    help="ND login domain (optional, default: 'local', env: PCV_DOMAIN).",
     required=False,
 )
 
 group = click.option(
     "-g",
     "--group",
     type=str,
+    default="default",
     envvar="PCV_GROUP",
-    help="NAE assurance group name or NDI insights group name (required, env: PCV_GROUP).",
+    help="NDI insights group name (optional, default: 'default', env: PCV_GROUP).",
+    required=False,
 )
 
 site = click.option(
     "-s",
     "--site",
     type=str,
     envvar="PCV_SITE",
-    help="NDI site or fabric name (optional, only required for NDI, env: PCV_SITE).",
-    required=False,
+    help="NDI site or fabric name (required, env: PCV_SITE).",
+    required=True,
 )
 
 name = click.option(
     "-n",
     "--name",
     type=str,
     envvar="PCV_NAME",
-    help="NAE/NDI pre-change validation name (optional, env: PCV_NAME).",
+    help="NDI pre-change validation name (required, env: PCV_NAME).",
+    required=True,
 )
 
 timeout = click.option(
     "--timeout",
     type=int,
     default=15,
     envvar="PCV_TIMEOUT",
-    help="NAE/NDI pre-change validation timeout in minutes (optional, default: 15, env: PCV_TIMEOUT).",
+    help="NDI pre-change validation timeout in minutes (optional, default: 15, env: PCV_TIMEOUT).",
     required=False,
 )
 
 suppress_events = click.option(
     "--suppress-events",
     type=str,
     envvar="PCV_SUPPRESS_EVENTS",
     default="APP_EPG_NOT_DEPLOYED,APP_EPG_HAS_NO_CONTRACT_IN_ENFORCED_VRF",
-    help="NAE/NDI comma-separated list of events to suppress (optional, default: 'APP_EPG_NOT_DEPLOYED,APP_EPG_HAS_NO_CONTRACT_IN_ENFORCED_VRF', env: PCV_SUPPRESS_EVENTS).",
+    help="NDI comma-separated list of events to suppress (optional, default: 'APP_EPG_NOT_DEPLOYED,APP_EPG_HAS_NO_CONTRACT_IN_ENFORCED_VRF', env: PCV_SUPPRESS_EVENTS).",
+    required=False,
 )
 
 
 file = click.option(
     "-f",
     "--file",
     cls=MutuallyExclusiveOption,
     type=click.Path(exists=True, dir_okay=False, file_okay=True),
     multiple=True,
     envvar="PCV_FILE",
-    help="NAE/NDI proposed change JSON file (optional, env: PCV_FILE).",
+    help="NDI proposed change JSON file (optional, env: PCV_FILE).",
+    required=False,
 )
 
 nac_tf_plan = click.option(
     "-t",
     "--nac-tf-plan",
     cls=MutuallyExclusiveOption,
     type=click.Path(exists=True, dir_okay=False, file_okay=True),
     envvar="PCV_NAC_TF_PLAN",
-    help="NAE/NDI proposed change Terraform plan output (optional, env: PCV_NAC_TF_PLAN).",
+    help="NDI proposed change Terraform plan output (optional, env: PCV_NAC_TF_PLAN).",
+    required=False,
 )
 
 output_summary = click.option(
     "-o",
     "--output-summary",
     type=click.Path(exists=False, dir_okay=False, file_okay=True),
     envvar="PCV_OUTPUT_SUMMARY",
-    help="NAE/NDI summary of new events/anomalies written to a file (optional, env: PCV_OUTPUT_SUMMARY).",
+    help="NDI summary of new events/anomalies written to a file (optional, env: PCV_OUTPUT_SUMMARY).",
     required=False,
 )
 
 output_url = click.option(
     "-r",
     "--output-url",
     type=click.Path(exists=False, dir_okay=False, file_okay=True),
     envvar="PCV_OUTPUT_URL",
-    help="NAE/NDI link (URL) to pre-change validation results written to a file (optional, env: PCV_OUTPUT_URL).",
+    help="NDI link (URL) to pre-change validation results written to a file (optional, env: PCV_OUTPUT_URL).",
     required=False,
 )
```

### Comparing `nexus_pcv-0.1.6/nexus_pcv/const.py` & `nexus_pcv-0.2.0/nexus_pcv/const.py`

 * *Files identical despite different names*

### Comparing `nexus_pcv-0.1.6/nexus_pcv/nae.py` & `nexus_pcv-0.2.0/nexus_pcv/ndi.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,291 +10,219 @@
 
 import requests
 import yaml
 
 logger = logging.getLogger(__name__)
 
 
-class NAE:
+class NDI:
     def __init__(
         self,
         hostname_ip: str,
         username: str,
         password: str,
         domain: str,
         timeout: int,
     ):
         self.hostname_ip = hostname_ip
-        self.api_url = "https://{}/nae/api/v1".format(hostname_ip)
+        self.api_url = "https://{}/sedgeapi/v1/cisco-nir/api/api/telemetry/v2".format(
+            hostname_ip
+        )
         self.username = username
         self.password = password
         self.domain = domain
         self.timeout = timeout
         self.session = requests.Session()
         self.session.verify = False
         self.authenticated = False
-        self.assurance_group_uuid = ""
+        self.site_uuid = ""
 
     def _login(self) -> Optional[requests.Response]:
         """Helper function to authenticate and populate headers"""
-        url = "{}/whoami".format(self.api_url)
-        resp = self.session.get(url)
-        if resp.status_code != 200:
-            logger.error("Whoami failed: {}".format(resp.json()))
-            return resp
-        if "X-NAE-LOGIN-OTP" not in resp.headers:
-            logger.error(
-                "X-NAE-LOGIN-OTP header missing in whoami response: {}".format(
-                    resp.json()
-                )
-            )
-            return resp
-
-        headers = {}
-        headers["X-NAE-LOGIN-OTP"] = resp.headers.get("X-NAE-LOGIN-OTP")
-        headers["Cookie"] = resp.headers.get("Set-Cookie")
         auth_payload = {
-            "username": self.username,
-            "password": self.password,
+            "userName": self.username,
+            "userPasswd": self.password,
             "domain": self.domain,
         }
-        url = "{}/login".format(self.api_url)
-        resp = self.session.post(url, headers=headers, json=auth_payload)
+        url = "https://{}/login".format(self.hostname_ip)
+        resp = self.session.post(url, json=auth_payload)
         if resp.status_code != 200:
             logger.error("Login failed: {}".format(resp.json()))
             return resp
-        if "X-NAE-CSRF-TOKEN" not in resp.headers:
-            logger.error(
-                "X-NAE-CSRF-TOKEN header missing in login response: {}".format(
-                    resp.json()
-                )
-            )
-            return resp
-
-        self.session.headers["X-NAE-CSRF-TOKEN"] = str(
-            resp.headers.get("X-NAE-CSRF-TOKEN")
-        )
-        self.session.headers["Cookie"] = str(resp.headers.get("Set-Cookie"))
         self.authenticated = True
         return None
 
-    def get_assurance_group_uuid(
-        self, name: str
-    ) -> Tuple[Optional[requests.Response], Optional[str]]:
-        """Get assurance group ID by its name"""
-        if not self.authenticated:
-            err = self._login()
-            if err is not None:
-                return err, None
-
-        url = "{}/config-services/assured-networks/aci-fabric/".format(self.api_url)
-        resp = self.session.get(url)
-        if resp.status_code != 200:
-            logger.error("Get assurance group failed: {}".format(resp.json()))
-            return resp, None
-
-        try:
-            ags = json.loads(resp.content)["value"]["data"]
-            for ag in ags:
-                if ag["unique_name"] == name:
-                    self.assurance_group_uuid = ag.get("uuid")
-                    return None, ag.get("uuid")
-        except KeyError:
-            pass
-        logger.error("UUID could not be found: {}".format(resp.json()))
-        return resp, None
-
     def get_last_epoch_id(
-        self, name: str
+        self, name: str, site: str
     ) -> Tuple[Optional[requests.Response], Optional[str]]:
         """Get last epoch ID of assurance group"""
         if not self.authenticated:
             err = self._login()
             if err is not None:
                 return err, None
 
-        err, uuid = self.get_assurance_group_uuid(name)
-        if err is not None:
-            return err, None
-
-        url = "{}/event-services/assured-networks/{}/epochs?$sort=-collectionTimestamp".format(
-            self.api_url, uuid
+        url = "{}/events/insightsGroup/{}/fabric/{}/epochs?$size=1&$status=FINISHED&$epochType=ONLINE".format(
+            self.api_url, name, site
         )
         resp = self.session.get(url)
         if resp.status_code != 200:
             logger.error("Get epoch id failed: {}".format(resp.json()))
             return resp, None
 
         try:
             epochs = json.loads(resp.content)["value"]["data"]
-            epoch_id = epochs[0]["epoch_id"]
+            epoch_id = epochs[0]["epochId"]
+            self.site_uuid = epochs[0]["fabricId"]
             return None, epoch_id
         except KeyError:
             pass
         logger.error("Epoch ID could not be found: {}".format(resp.json()))
         return resp, None
 
     def start_pcv(
-        self, name: str, ag_name: str, json_data: str
+        self, name: str, group: str, site: str, json_data: str
     ) -> Tuple[Optional[requests.Response], Optional[str]]:
         """Start pre-change validation and return job ID"""
         if not self.authenticated:
             err = self._login()
             if err is not None:
                 return err, None
 
-        err, epoch_id = self.get_last_epoch_id(ag_name)
+        err, epoch_id = self.get_last_epoch_id(group, site)
         if err is not None:
             return err, None
 
         payload = {}
         payload["name"] = name
-        payload["fabric_uuid"] = self.assurance_group_uuid
-        payload["base_epoch_id"] = str(epoch_id)
-        payload["stop_analysis"] = str(True)
-        payload["allow_unsupported_object_modification"] = "true"
-        payload["uploaded_file_name"] = "tmp.json"
+        payload["fabricUuid"] = self.site_uuid
+        payload["baseEpochId"] = str(epoch_id)
+        payload["allowUnsupportedObjectModification"] = "true"
+        payload["uploadedFileName"] = "tmp.json"
+        payload["assuranceEntityName"] = site
 
         files = [
             ("data", ("blob", json.dumps(payload), "application/json")),
             ("file", ("tmp.json", json_data, "application/json")),
         ]
 
-        url = "{}/config-services/prechange-analysis/file-changes".format(self.api_url)
+        url = (
+            "{}/config/insightsGroup/{}/fabric/{}/prechangeAnalysis/fileChanges".format(
+                self.api_url, group, site
+            )
+        )
         resp = self.session.post(url, files=files)
         if resp.status_code != 200:
             logger.error("Start pre-change analysis failed: {}".format(resp.json()))
             return resp, None
 
         try:
-            job_id = json.loads(resp.content)["value"]["data"]["job_id"]
+            job_id = json.loads(resp.content)["value"]["data"]["jobId"]
             logger.info("Pre-change analysis started. Job ID: {}".format(job_id))
             return None, job_id
         except KeyError:
             pass
         logger.error("Job ID could not be found: {}".format(resp.json()))
         return resp, None
 
     def wait_pcv(
-        self, job_id: str
+        self, group: str, site: str, job_id: str
     ) -> Tuple[Optional[requests.Response], Optional[str]]:
         """Wair for pre-change validation to complete and return epoch job ID"""
         if not self.authenticated:
             err = self._login()
             if err is not None:
                 return err, None
 
         status = None
         start_time = datetime.now()
         while True:
-            url = "{}/config-services/prechange-analysis/{}".format(
-                self.api_url, job_id
+            url = "{}/config/insightsGroup/{}/fabric/{}/prechangeAnalysis/{}".format(
+                self.api_url, group, site, job_id
             )
             resp = self.session.get(url)
             if resp.status_code != 200:
                 logger.error(
                     "Get pre-change analysis status failed: {}".format(resp.json())
                 )
                 return resp, None
             try:
-                status = json.loads(resp.content)["value"]["data"]["analysis_status"]
+                status = json.loads(resp.content)["value"]["data"]["analysisStatus"]
                 if status == "COMPLETED":
                     break
             except KeyError:
                 logger.error("Status could not be found: {}".format(resp.json()))
             delta_minutes = (datetime.now() - start_time).total_seconds() / 60
             if delta_minutes > self.timeout:
                 break
             logger.info("Waiting for pre-change analysis to complete ...")
             time.sleep(10)
 
         try:
-            epoch_job_id = json.loads(resp.content)["value"]["data"][
-                "epoch_delta_job_id"
-            ]
+            epoch_job_id = json.loads(resp.content)["value"]["data"]["epochDeltaJobId"]
             logger.info(
                 "Pre-change analysis completed. Epoch job ID: {}".format(epoch_job_id)
             )
             return None, epoch_job_id
         except KeyError:
             pass
         logger.error("Epoch job ID could not be found: {}".format(resp.json()))
         return resp, None
 
     def get_pcv_results(
-        self, epoch_job_id: str, suppress_events: str
+        self, group: str, site: str, epoch_job_id: str, suppress_events: str
     ) -> Tuple[Optional[requests.Response], Optional[List[Any]]]:
         """Retrieve pre-change validation results"""
         if not self.authenticated:
             err = self._login()
             if err is not None:
                 return err, None
 
         suppress_events_list = suppress_events.split(",")
 
-        url = "{}/epoch-delta-services/assured-networks/{}/job/{}/health/view/aggregate-table?category=ADC,CHANGE_ANALYSIS,TENANT_ENDPOINT,TENANT_FORWARDING,TENANT_SECURITY,RESOURCE_UTILIZATION,SYSTEM,COMPLIANCE&epoch_status=EPOCH2_ONLY&severity=EVENT_SEVERITY_CRITICAL,EVENT_SEVERITY_MAJOR,EVENT_SEVERITY_MINOR,EVENT_SEVERITY_WARNING,EVENT_SEVERITY_INFO".format(
-            self.api_url, self.assurance_group_uuid, epoch_job_id
+        url = "{}/epochDelta/insightsGroup/{}/fabric/{}/job/{}/health/view/aggregateTable?epochStatus=EPOCH2_ONLY".format(
+            self.api_url, group, site, epoch_job_id
         )
         resp = self.session.get(url)
         if resp.status_code != 200:
             logger.error("Get PCV results failed: {}".format(resp.json()))
             return resp, None
 
         event_list = []
         try:
-            for event in json.loads(resp.content)["value"]["data"]:
+            for event in json.loads(resp.content)["entries"]:
                 if int(event["count"]) > 0:
                     if (
-                        str(event["epoch2_details"]["severity"])
-                        == "EVENT_SEVERITY_INFO"
-                        or str(event["epoch2_details"]["mnemonic"])
-                        in suppress_events_list
+                        str(event.get("severity")) == "info"
+                        or str(event.get("mnemonicTitle")) in suppress_events_list
                     ):
                         continue
                     event_list.append(
                         {
-                            "Category": event["category"].title(),
-                            "Count": event["count"],
-                            "Description": event["epoch2_details"]["description"],
-                            "Severity": event["epoch2_details"]["severity"][
-                                15:
-                            ].title(),
+                            "Category": event.get("category").title(),
+                            "Count": event.get("count"),
+                            "Description": event.get("anomalyStr"),
+                            "Severity": event.get("severity"),
                         }
                     )
         except KeyError:
             logger.error("Could not find events: {}".format(resp.json()))
             return resp, None
         if event_list:
             logger.error(
-                "The following events have been raised:\n{}".format(
+                "The following anomalies have been raised:\n{}".format(
                     yaml.dump(event_list)
                 )
             )
         return None, event_list
 
-    def get_pcv_url(
-        self, job_id: str
-    ) -> Tuple[Optional[requests.Response], Optional[str]]:
+    def get_pcv_url(self) -> Tuple[Optional[requests.Response], Optional[str]]:
         """Get URL pointing to pre-change validation results"""
         if not self.authenticated:
             err = self._login()
             if err is not None:
                 return err, None
 
-        url = "{}/config-services/prechange-analysis/{}".format(self.api_url, job_id)
-        resp = self.session.get(url)
-        if resp.status_code != 200:
-            logger.error("Get PCV url failed: {}".format(resp.json()))
-            return resp, None
-        try:
-            response = json.loads(resp.content)["value"]["data"]
-            pcv_url = "https://{}/nae/epoch-delta-analysis/result/health?analysis_id={}&type=PCV_EPOCH_DELTA_ANALYSIS&fabric_id={}&epoch={}#top".format(
-                self.hostname_ip,
-                response["epoch_delta_job_id"],
-                response["fabric_uuid"],
-                response["pre_change_epoch_uuid"],
-            )
-            return None, pcv_url
-        except KeyError:
-            pass
-        logger.error("PCV url parameters could not be found: {}".format(resp.json()))
-        return resp, None
+        url = "https://{}/appcenter/cisco/nexus-insights/ui/#/changeManagement/preChangeAnalysis".format(
+            self.hostname_ip
+        )
+
+        return None, url
```

### Comparing `nexus_pcv-0.1.6/nexus_pcv/pcv.py` & `nexus_pcv-0.2.0/nexus_pcv/pcv.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,37 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2022, Daniel Schmidt <danischm@cisco.com>
 
-from enum import Enum
 import json
 import logging
 import re
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 import urllib3
 import yaml
 
 from .apic import ApicObject
 from .const import RN_PREFIX_CLASSNAME_MAPPINGS
-from .nae import NAE
 from .ndi import NDI
 
 logger = logging.getLogger(__name__)
 
 
 class PCV:
-    class Platform(Enum):
-        NDI = 1
-        NAE = 2
-
     def __init__(
         self,
         hostname_ip: str,
         username: str,
         password: str,
         domain: str,
         timeout: int,
-        platform: Platform,
     ):
-        self.platform = platform
-        if platform is self.Platform.NDI:
-            self.ndi = NDI(hostname_ip, username, password, domain, timeout)
-        elif platform is self.Platform.NAE:
-            self.nae = NAE(hostname_ip, username, password, domain, timeout)
+        self.ndi = NDI(hostname_ip, username, password, domain, timeout)
         self.root = ApicObject("root", {}, [], None)
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
     def _resolve_tf_classnames(self, root: ApicObject, tf_plan: Any) -> None:
         """Helper function to resolve missing class names and key attributes using the Terraform plan"""
         if root.cl is None:
             dn = root["dn"]
@@ -206,38 +195,7 @@
         if err is not None:
             return err, None, None
         if file_summary and events:
             self._write_pcv_events(events, file_summary)
         if file_url and url is not None:
             self._write_pcv_url(url, file_url)
         return None, events, url
-
-    def nae_pcv(
-        self,
-        name: str,
-        group: str,
-        suppress_events: str,
-        file_summary: str,
-        file_url: str,
-    ) -> Tuple[Optional[requests.Response], Optional[List[Any]], Optional[str]]:
-        """Trigger an NAE pre-change validation"""
-        if not len(self.root.children):
-            logger.info("No updates planned. No need to trigger a pre-change analysis.")
-            return None, None, None
-        logger.debug("Proposed change (JSON): {}".format(self.root[0]))
-        err, job_id = self.nae.start_pcv(name, group, str(self.root[0]))
-        if err is not None:
-            return err, None, None
-        err, epoch_job_id = self.nae.wait_pcv(str(job_id))
-        if err is not None:
-            return err, None, None
-        err, events = self.nae.get_pcv_results(str(epoch_job_id), suppress_events)
-        if err is not None:
-            return err, None, None
-        err, url = self.nae.get_pcv_url(str(job_id))
-        if err is not None:
-            return err, None, None
-        if file_summary and events:
-            self._write_pcv_events(events, file_summary)
-        if file_url and url is not None:
-            self._write_pcv_url(url, file_url)
-        return None, events, url
```

### Comparing `nexus_pcv-0.1.6/pyproject.toml` & `nexus_pcv-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 documentation = "https://github.com/netascode/nexus-pcv"
 homepage = "https://github.com/netascode/nexus-pcv"
 license = "LICENSE"
 maintainers = ["Daniel Schmidt <danischm@cisco.com>"]
 name = "nexus-pcv"
 readme = "README.md"
 repository = "https://github.com/netascode/nexus-pcv"
-version = "0.1.6"
+version = "0.2.0"
 
 [tool.poetry.scripts]
 nexus-pcv = "nexus_pcv.cli.main:main"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 errorhandler = "^2.0.1"
-importlib-metadata = {version = "^2.0.0", python = "<3.8"}
-python = "^3.7"
+python = "^3.8"
 pyyaml = "^6.0"
 requests = "^2.28.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.10.0"
+black = "^24.4.0"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 mypy = "^0.982"
 pre-commit = "^2.20.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
```

### Comparing `nexus_pcv-0.1.6/PKG-INFO` & `nexus_pcv-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,77 @@
 Metadata-Version: 2.1
 Name: nexus-pcv
-Version: 0.1.6
+Version: 0.2.0
 Summary: A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine.
 Home-page: https://github.com/netascode/nexus-pcv
 License: LICENSE
 Author: Daniel Schmidt
 Author-email: danischm@cisco.com
 Maintainer: Daniel Schmidt
 Maintainer-email: danischm@cisco.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: errorhandler (>=2.0.1,<3.0.0)
-Requires-Dist: importlib-metadata (>=2.0.0,<3.0.0) ; python_version < "3.8"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://github.com/netascode/nexus-pcv
 Project-URL: Repository, https://github.com/netascode/nexus-pcv
 Description-Content-Type: text/markdown
 
 [![Tests](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml/badge.svg)](https://github.com/netascode/nexus-pcv/actions/workflows/test.yml)
-![Python Support](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational "Python Support: 3.7, 3.8, 3.9, 3.10")
+![Python Support](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-informational "Python Support: 3.8, 3.9, 3.10, 3.11, 3.12")
 
 # nexus-pcv
 
-A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or Network Assurance Engine. It can either work with provided JSON file(s) or a `terraform plan` output from a [Nexus as Code](https://cisco.com/go/nexusascode) project. It waits for the analysis to complete and evaluates the results.
+A CLI tool to perform a pre-change validation on Nexus Dashboard Insights. It can either work with provided JSON file(s) or a `terraform plan` output from a [Nexus as Code](https://cisco.com/go/nexusascode) project. It waits for the analysis to complete and evaluates the results.
 
 ```
 $ nexus-pcv -h
 Usage: nexus-pcv [OPTIONS]
 
-  A CLI tool to perform a pre-change validation on Nexus Dashboard Insights or
-  Network Assurance Engine.
+  A CLI tool to perform a pre-change validation on Nexus Dashboard Insights.
 
 Options:
-  --version                   Show the version and exit.
-  -v, --verbosity LVL         Either CRITICAL, ERROR, WARNING, INFO or DEBUG.
-  -i, --hostname-ip TEXT      NAE/ND hostname or IP (required, env:
-                              PCV_HOSTNAME_IP).
-  -u, --username TEXT         NAE/ND username (required, env: PCV_USERNAME).
-  -p, --password TEXT         NAE/ND password (required, env: PCV_PASSWORD).
-  -d, --domain TEXT           NAE/ND login domain (optional, default: 'Local',
-                              env: PCV_DOMAIN).
-  -g, --group TEXT            NAE assurance group name or NDI insights group
-                              name (required, env: PCV_GROUP).
-  -s, --site TEXT             NDI site or fabric name (optional, only required
-                              for NDI, env: PCV_SITE).
-  -n, --name TEXT             NAE/NDI pre-change validation name (optional,
-                              env: PCV_NAME).
-  -s, --suppress-events TEXT  NAE/NDI comma-separated list of events to
-                              suppress (optional, default: 'APP_EPG_NOT_DEPLOY
-                              ED,APP_EPG_HAS_NO_CONTRACT_IN_ENFORCED_VRF',
-                              env: PCV_SUPPRESS_EVENTS).
-  -t, --timeout INTEGER       NAE/NDI pre-change validation timeout in minutes
-                              (optional, default: 15, env: PCV_TIMEOUT).
-  -f, --file FILE             NAE/NDI proposed change JSON file (optional,
-                              env: PCV_FILE).
-  -t, --nac-tf-plan FILE      NAE/NDI proposed change Terraform plan output
-                              (optional, env: PCV_NAC_TF_PLAN).
-  -o, --output-summary FILE   NAE/NDI summary of new events/anomalies written
-                              to a file (optional, env: PCV_OUTPUT_SUMMARY).
-  -r, --output-url FILE       NAE/NDI link (URL) to pre-change validation
-                              results written to a file (optional, env:
-                              PCV_OUTPUT_URL).
-  -h, --help                  Show this message and exit.
+  --version                  Show the version and exit.
+  -v, --verbosity LVL        Either CRITICAL, ERROR, WARNING, INFO or DEBUG.
+  -i, --hostname-ip TEXT     ND hostname or IP (required, env:
+                             PCV_HOSTNAME_IP).
+  -u, --username TEXT        ND username (required, env: PCV_USERNAME).
+  -p, --password TEXT        ND password (required, env: PCV_PASSWORD).
+  -d, --domain TEXT          ND login domain (optional, default: 'local', env:
+                             PCV_DOMAIN).
+  -g, --group TEXT           NDI insights group name (optional, default:
+                             'default', env: PCV_GROUP).
+  -s, --site TEXT            NDI site or fabric name (required, env:
+                             PCV_SITE).
+  -n, --name TEXT            NDI pre-change validation name (optional, env:
+                             PCV_NAME).
+  --suppress-events TEXT     NDI comma-separated list of events to suppress
+                             (optional, default: 'APP_EPG_NOT_DEPLOYED,APP_EPG
+                             _HAS_NO_CONTRACT_IN_ENFORCED_VRF', env:
+                             PCV_SUPPRESS_EVENTS).
+  --timeout INTEGER          NDI pre-change validation timeout in minutes
+                             (optional, default: 15, env: PCV_TIMEOUT).
+  -f, --file FILE            NDI proposed change JSON file (optional, env:
+                             PCV_FILE).
+  -t, --nac-tf-plan FILE     NDI proposed change Terraform plan output
+                             (optional, env: PCV_NAC_TF_PLAN).
+  -o, --output-summary FILE  NDI summary of new events/anomalies written to a
+                             file (optional, env: PCV_OUTPUT_SUMMARY).
+  -r, --output-url FILE      NDI link (URL) to pre-change validation results
+                             written to a file (optional, env:
+                             PCV_OUTPUT_URL).
+  -h, --help                 Show this message and exit.
 ```
 
 ## Installation
 
 Python 3.7+ is required to install `nexus-pcv`. Don't have Python 3.7 or later? See [Python 3 Installation & Setup Guide](https://realpython.com/installing-python/).
 
 `nexus-pcv` can be installed in a virtual environment using `pip`:
```

