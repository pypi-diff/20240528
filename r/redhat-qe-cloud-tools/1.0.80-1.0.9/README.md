# Comparing `tmp/redhat_qe_cloud_tools-1.0.80.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.80.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.9.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.80.tar` & `redhat_qe_cloud_tools-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-05-28 06:57:35.971658 redhat_qe_cloud_tools-1.0.80/LICENSE
--rw-r--r--   0        0        0      956 2024-05-28 06:57:35.971658 redhat_qe_cloud_tools-1.0.80/README.md
--rw-r--r--   0        0        0        0 2024-05-28 06:57:35.971658 redhat_qe_cloud_tools-1.0.80/clouds/__init__.py
--rw-r--r--   0        0        0      787 2024-05-28 06:57:35.971658 redhat_qe_cloud_tools-1.0.80/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2024-05-28 06:57:35.971658 redhat_qe_cloud_tools-1.0.80/clouds/aws/__init__.py
--rw-r--r--   0        0        0     5602 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     4480 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0      455 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/aws/roles/README.md
--rw-r--r--   0        0        0        0 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/aws/roles/__init__.py
--rw-r--r--   0        0        0     1999 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/aws/roles/roles.py
--rw-r--r--   0        0        0      779 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/aws/session_clients.py
--rw-r--r--   0        0        0     1418 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/cli/README.md
--rw-r--r--   0        0        0        0 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 06:57:35.972658 redhat_qe_cloud_tools-1.0.80/clouds/cli/aws/__init__.py
--rw-r--r--   0        0        0     6937 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/cli/aws/aws_cli.py
--rwxr-xr-x   0        0        0     2867 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/cli/microsoft_azure/__init__.py
--rw-r--r--   0        0        0     1965 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/cli/microsoft_azure/microsoft_azure_cli.py
--rw-r--r--   0        0        0        0 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/gcp/__init__.py
--rw-r--r--   0        0        0      431 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/gcp/utils.py
--rw-r--r--   0        0        0     1259 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/microsoft_azure/session_clients.py
--rw-r--r--   0        0        0      942 2024-05-28 06:57:35.973658 redhat_qe_cloud_tools-1.0.80/clouds/microsoft_azure/utils.py
--rw-r--r--   0        0        0     1983 2024-05-28 06:57:40.638645 redhat_qe_cloud_tools-1.0.80/pyproject.toml
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.80/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-09 18:06:16.328454 redhat_qe_cloud_tools-1.0.9/LICENSE
+-rw-r--r--   0        0        0      852 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/__init__.py
+-rw-r--r--   0        0        0     4565 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     4317 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      455 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/roles/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/roles/__init__.py
+-rw-r--r--   0        0        0     1193 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/roles/roles.py
+-rw-r--r--   0        0        0      554 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/session_clients.py
+-rw-r--r--   0        0        0     8197 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/utilities/delete_aws_resources.py
+-rw-r--r--   0        0        0      850 2023-07-09 18:06:16.330454 redhat_qe_cloud_tools-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.9/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.80/LICENSE` & `redhat_qe_cloud_tools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.80/README.md` & `redhat_qe_cloud_tools-1.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 
 ```
 poetry install
 ```
 
 ## Docs
 - [AWS Readme](clouds/aws/README.md)
-- [Cloud nuke CLI tools Readme](clouds/cli/README.md)
 
 ## Release new version
 ### requirements:
 * Export GitHub token
 ```bash
 export GITHUB_TOKEN=<your_github_token>
 ```
 * [release-it](https://github.com/release-it/release-it)
-Run the following once (execute outside repository dir for example `~/`):
+Run the following once:
 ```bash
 sudo npm install --global release-it
 npm install --save-dev @j-ulrich/release-it-regex-bumper
 rm -f package.json package-lock.json
 ```
 ### usage:
 * Create a release, run from the relevant branch.
```

### Comparing `redhat_qe_cloud_tools-1.0.80/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.80/clouds/aws/aws_utils.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/aws_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from __future__ import annotations
 import json
 import os
 from configparser import ConfigParser, NoOptionError, NoSectionError
 from http import HTTPStatus
-from typing import List, Optional
 
-import botocore
 from simple_logger.logger import get_logger
 
 from clouds.aws.session_clients import ec2_client
 
 LOGGER = get_logger(name=__name__)
-AWS_CONFIG_FILE: str = os.environ.get("AWS_CONFIG_FILE", os.path.expanduser("~/.aws/config"))
-AWS_CREDENTIALS_FILE: str = os.environ.get("AWS_SHARED_CREDENTIALS_FILE", os.path.expanduser("~/.aws/credentials"))
+AWS_CONFIG_FILE = os.environ.get("AWS_CONFIG_FILE", os.path.expanduser("~/.aws/config"))
+AWS_CREDENTIALS_FILE = os.environ.get(
+    "AWS_CONFIG_FILE", os.path.expanduser("~/.aws/credentials")
+)
 
 
 class AWSConfigurationError(Exception):
     pass
 
 
 def set_and_verify_existing_config_in_env_vars_or_file(
-    vars_list: List[str], file_path: str, section: str = "default"
-) -> None:
+    vars_list, file_path, section="default"
+):
     """
     Verify vars are either set as environment variables or in a config file.
 
     When var exists as OS environment then continue.
     When vars exists in config file, set them as OS environment.
     If none of the above raise.
 
@@ -41,15 +40,17 @@
     parser = ConfigParser()
     parser.read(file_path)
     aws_region_str = "region"
     for var in vars_list:
         if os.getenv(var.upper()):
             continue
 
-        LOGGER.info(f"Variable {var} is not set as environment variables, checking in config" " file.")
+        LOGGER.info(
+            f"Variable {var} is not set as environment variables, checking in config file."
+        )
         try:
             var_in_file = var.lower()
             # `AWS_REGION` environment variable is set as `region` in the config file
             if aws_region_str in var_in_file:
                 var_in_file = aws_region_str
 
             os.environ[var.upper()] = parser.get(section, var_in_file)
@@ -60,31 +61,30 @@
         LOGGER.error(
             f"Missing configuration: {','.join(missing_vars)}. "
             f"Values should be set in environment variables or in {file_path}"
         )
         raise AWSConfigurationError()
 
 
-def set_and_verify_aws_credentials(region_name: Optional[str | None]) -> None:
+def set_and_verify_aws_credentials():
     set_and_verify_existing_config_in_env_vars_or_file(
         vars_list=["AWS_ACCESS_KEY_ID", "AWS_SECRET_ACCESS_KEY"],
         file_path=AWS_CREDENTIALS_FILE,
     )
-
-    ec2_client(region_name=region_name).describe_regions()
+    ec2_client().describe_regions()
 
 
-def set_and_verify_aws_config() -> None:
+def set_and_verify_aws_config():
     set_and_verify_existing_config_in_env_vars_or_file(
         vars_list=["AWS_REGION"],
         file_path=AWS_CONFIG_FILE,
     )
 
 
-def delete_all_objects_from_s3_folder(bucket_name: str, boto_client: "botocore.client.S3") -> None:
+def delete_all_objects_from_s3_folder(bucket_name: str, boto_client) -> None:
     """
     Deletes all files in a folder of an S3 bucket
 
     Args:
         bucket_name: The bucket name
         boto_client: AWS S3 client
     """
@@ -102,25 +102,28 @@
 
     files_to_delete = [{"Key": file["Key"]} for file in files_in_folder]
     delete_response = boto_client.delete_objects(
         Bucket=bucket_name,
         Delete={"Objects": files_to_delete, "Quiet": True},
     )
 
-    delete_response_http_status_code = delete_response["ResponseMetadata"]["HTTPStatusCode"]
+    delete_response_http_status_code = delete_response["ResponseMetadata"][
+        "HTTPStatusCode"
+    ]
     if delete_response_http_status_code == HTTPStatus.OK:
         LOGGER.info("Objects deleted successfully")
         return
     else:
         LOGGER.error(
-            "Objects not deleted:\n:" f"{json.dumps(delete_response, default=str, indent=4)}",
+            "Objects not deleted:\n:"
+            f"{json.dumps(delete_response, default=str, indent=4)}",
         )
 
 
-def delete_bucket(bucket_name: str, boto_client: "botocore.client.S3") -> None:
+def delete_bucket(bucket_name: str, boto_client) -> None:
     """
     Delete velero bucket
 
     Args:
         bucket_name: the bucket name
         boto_client: AWS client
     """
@@ -140,41 +143,7 @@
         LOGGER.info(f"Bucket '{bucket_name}' not found")
         return
 
     LOGGER.error(
         f"Bucket {bucket_name} not deleted",
         json.dumps(response, defualt=str, indent=4),
     )
-
-
-def aws_region_names() -> List[str]:
-    """
-    Lists AWS regions
-
-    Returns:
-        list: list of AWS regions name
-
-    """
-    regions = ec2_client().describe_regions()["Regions"]
-    return [region["RegionName"] for region in regions]
-
-
-def get_least_crowded_aws_vpc_region(region_list: List[str]) -> str:
-    """
-    Selects region with the least number of VPCs.
-
-    Args:
-        region_list: list of region names
-
-    Returns:
-        str: region name with have the least number of VPCs
-
-    """
-    if not region_list:
-        raise ValueError("`region_list` must not be empty")
-
-    region, vpcs = region_list[0], 0
-    for _region in region_list:
-        if (num_vpcs := len(ec2_client(region_name=_region).describe_vpcs()["Vpcs"])) <= vpcs:
-            region = _region
-            vpcs = num_vpcs
-    return region
```

### Comparing `redhat_qe_cloud_tools-1.0.80/clouds/aws/delete_s3_velero_bucket.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/delete_s3_velero_bucket.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from __future__ import annotations
 import os
 import re
-from typing import Any, List
+from typing import Union
 
 import boto3
-import botocore
 import click
 from simple_logger.logger import get_logger
 
 from clouds.aws.aws_utils import delete_all_objects_from_s3_folder, delete_bucket
 
 LOGGER = get_logger(name=__name__)
 
 
-def delete_velero_cluster_buckets(cluster: str, boto_client: "botocore.client.S3") -> None:
+def delete_velero_cluster_buckets(cluster, boto_client) -> None:
     """
     Delete the velero bucket associated with a cluster
 
     Args:
-        cluster (str): The cluster name
-        boto_client (botocore.client.S3): aws boto client
+        cluster: The cluster name
+        boto_client: aws boto client
+
 
     """
 
     LOGGER.info(f"Delete velero buckets for '{cluster}' cluster")
 
     velero_bucket_list = get_velero_buckets(boto_client=boto_client)
     if not velero_bucket_list:
@@ -33,39 +32,45 @@
     for bucket in velero_bucket_list:
         bucket_name = bucket["Name"]
         if verify_cluster_matches_velero_infrastructure_name(
             boto_client=boto_client,
             cluster_name=cluster,
             bucket_name=bucket_name,
         ):
-            delete_all_objects_from_s3_folder(bucket_name=bucket_name, boto_client=boto_client)
+            delete_all_objects_from_s3_folder(
+                bucket_name=bucket_name, boto_client=boto_client
+            )
             delete_bucket(bucket_name=bucket_name, boto_client=boto_client)
             # A cluster is mapped to only one bucket, so don't check any remaining buckets
             return
 
     LOGGER.info("No buckets deleted")
 
 
-def get_velero_buckets(boto_client: "botocore.client.S3") -> List[dict[str, Any]]:
+def get_velero_buckets(boto_client) -> list:
     """
     Get a list of velero buckets
 
     Args:
         boto_client: AWS client
 
     Returns:
         list of velero buckets
     """
     LOGGER.info("Get a list of velero buckets")
 
     buckets = boto_client.list_buckets()["Buckets"]
-    return [bucket for bucket in buckets if re.search("managed-velero-backups-", bucket["Name"])]
+    return [
+        bucket
+        for bucket in buckets
+        if re.search("managed-velero-backups-", bucket["Name"])
+    ]
 
 
-def get_velero_infrastructure_name(bucket_name: str, boto_client: "botocore.client.S3") -> str | None:
+def get_velero_infrastructure_name(bucket_name: str, boto_client) -> Union[str, None]:
     """
     Get the velero bucket infrastructure name
 
     Args:
         bucket_name: The name of the cluster bucket to delete
         boto_client: AWS client
 
@@ -76,19 +81,17 @@
     LOGGER.info(f"Get tags for bucket: {bucket_name}")
     bucket_tags = boto_client.get_bucket_tagging(Bucket=bucket_name)["TagSet"]
 
     for tag in bucket_tags:
         if tag["Key"] == "velero.io/infrastructureName":
             return tag["Value"]
 
-    return None
-
 
 def verify_cluster_matches_velero_infrastructure_name(
-    boto_client: "botocore.client.S3",
+    boto_client,
     cluster_name: str,
     bucket_name: str,
 ) -> bool:
     """
     Get the velero bucket infrastructure name and compare it with the cluster
 
     Args:
@@ -97,54 +100,56 @@
         bucket_name: The bucket name
 
     Returns:
          bool: True if the cluster matches a velero infrastructure name, False otherwise
     """
 
     LOGGER.info(
-        "Verify cluster matches a velero infrastructure name via its bucket tag:" f" {bucket_name}",
+        f"Verify cluster matches a velero infrastructure name via its bucket tag: {bucket_name}",
     )
 
-    velero_infrastructure_name = get_velero_infrastructure_name(bucket_name=bucket_name, boto_client=boto_client)
+    velero_infrastructure_name = get_velero_infrastructure_name(
+        bucket_name=bucket_name, boto_client=boto_client
+    )
 
     # Verify if the bucket is associated with the cluster
     if velero_infrastructure_name and re.search(
         rf"{cluster_name}(-\w+)?$",
         velero_infrastructure_name,
     ):
         LOGGER.info(
-            f"Verified cluster '{cluster_name}' is associated with velero"
-            f" infrastructure name {velero_infrastructure_name}",
+            f"Verified cluster '{cluster_name}' "
+            f"is associated with velero infrastructure name {velero_infrastructure_name}",
         )
         return True
 
     return False
 
 
 @click.command()
 @click.option(
     "--aws-access-key-id",
-    help=("Set AWS access key id, default if taken from environment variable:" " AWS_ACCESS_KEY_ID"),
+    help="Set AWS access key id, default if taken from environment variable: AWS_ACCESS_KEY_ID",
     required=True,
     default=os.getenv("AWS_ACCESS_KEY_ID"),
 )
 @click.option(
     "--aws-secret-access-key",
-    help=("Set AWS secret access key id,default if taken from environment variable:" " AWS_SECRET_ACCESS_KEY"),
+    help="Set AWS secret access key id,default if taken from environment variable: AWS_SECRET_ACCESS_KEY",
     required=True,
     default=os.getenv("AWS_SECRET_ACCESS_KEY"),
 )
 @click.option(
     "-c",
     "--cluster-name",
     help="",
     required=True,
     default=os.getenv("AWS_SECRET_ACCESS_KEY"),
 )
-def main(aws_access_key_id: str, aws_secret_access_key: str, cluster_name: str) -> None:
+def main(aws_access_key_id, aws_secret_access_key, cluster_name):
     boto_client = boto3.client(
         service_name="s3",
         aws_access_key_id=aws_access_key_id,
         aws_secret_access_key=aws_secret_access_key,
     )
 
     delete_velero_cluster_buckets(cluster=cluster_name, boto_client=boto_client)
```

### Comparing `redhat_qe_cloud_tools-1.0.80/clouds/cli/aws/aws_cli.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/utilities/delete_aws_resources.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,187 @@
-from __future__ import annotations
 import multiprocessing
 import re
 import shlex
-from multiprocessing import Queue
-from typing import List
+import shutil
 
+import click
 from ocp_utilities.utils import run_command
 from simple_logger.logger import get_logger
 
 from clouds.aws.aws_utils import (
     delete_all_objects_from_s3_folder,
     delete_bucket,
+    set_and_verify_aws_credentials,
 )
 from clouds.aws.session_clients import ec2_client, iam_client, rds_client, s3_client
 
-LOGGER = get_logger(name="aws-nuke-cli")
-MAX_ITEMS: int = 1000
+LOGGER = get_logger(name="delete-aws-resources", filename="delete_aws_resources.log")
+MAX_ITEMS = 1000
 
 
-def delete_rds_instances(region_name: str) -> bool:
-    db_instances = rds_client(region_name=region_name).describe_db_instances()["DBInstances"]
+def aws_region_names():
+    regions = ec2_client().describe_regions()["Regions"]
+    return [region["RegionName"] for region in regions]
+
+
+def delete_rds_instances(region_name):
+    db_instances = rds_client(region_name=region_name).describe_db_instances()[
+        "DBInstances"
+    ]
     for db_instance_identifier in db_instances:
         LOGGER.warning(f"DB instance identifier: {db_instance_identifier}")
-        # TODO: once we have the contents of db_instance_identifier, update code to delete it update return value
+        # TODO: once we have the contents of db_instance_identifier, update code to delete it
         # aws rds modify-db-instance --no-deletion-protection --db-instance-identifier "${rds}"
 
-    return False
-
 
-def delete_vpc_peering_connections(region_name: str) -> bool:
-    for conn in ec2_client(region_name=region_name).describe_vpc_peering_connections()["VpcPeeringConnections"]:
+def delete_vpc_peering_connections(region_name):
+    for conn in ec2_client(region_name=region_name).describe_vpc_peering_connections()[
+        "VpcPeeringConnections"
+    ]:
         LOGGER.warning(f"VPC peering connection: {conn}")
-        # TODO: once we have the contents of conn, update code to delete it update return value
+        # TODO: once we have the contents of conn, update code to delete it
         # aws ec2 delete-vpc-peering-connection --vpc-peering-connection-id "${pc}"
 
-    return False
 
-
-def delete_open_id_connect_providers(region_name: str) -> bool:
+def delete_open_id_connect_providers(region_name):
     LOGGER.info("Executing delete_open_id_connect_provider")
     _iam_client = iam_client(region_name=region_name)
-    for conn in _iam_client.list_open_id_connect_providers()["OpenIDConnectProviderList"]:
+    for conn in _iam_client.list_open_id_connect_providers()[
+        "OpenIDConnectProviderList"
+    ]:
         conn_name = conn["Arn"]
         LOGGER.info(f"Delete open id connection provider {conn_name}")
         _iam_client.delete_open_id_connect_provider(OpenIDConnectProviderArn=conn_name)
 
-    return True
-
 
-def delete_instance_profiles(region_name: str) -> bool:
+def delete_instance_profiles(region_name):
     LOGGER.info("Executing delete_instance_profiles")
     _iam_client = iam_client(region_name=region_name)
     instance_profiles_dict = _iam_client.list_instance_profiles(MaxItems=MAX_ITEMS)
     for profile in instance_profiles_dict["InstanceProfiles"]:
         profile_name = profile["InstanceProfileName"]
-        for role in _iam_client.get_instance_profile(InstanceProfileName=profile_name)["InstanceProfile"]["Roles"]:
+        for role in _iam_client.get_instance_profile(InstanceProfileName=profile_name)[
+            "InstanceProfile"
+        ]["Roles"]:
             role_name = role["RoleName"]
             LOGGER.info(f"Remove role {role_name} from instance profile {profile_name}")
-            _iam_client.remove_role_from_instance_profile(InstanceProfileName=profile_name, RoleName=role_name)
+            _iam_client.remove_role_from_instance_profile(
+                InstanceProfileName=profile_name, RoleName=role_name
+            )
         LOGGER.info(f"Delete Profile {profile_name}")
         _iam_client.delete_instance_profile(InstanceProfileName=profile_name)
 
     return instance_profiles_dict["IsTruncated"]
 
 
-def delete_roles(region_name: str) -> bool:
+def delete_roles(region_name):
     LOGGER.info("Executing delete_roles")
     _iam_client = iam_client(region_name=region_name)
     roles_dict = _iam_client.list_roles(MaxItems=MAX_ITEMS)
     attached_role_policies_dict = {}
     detached_policy_names_dict = {}
     for role in roles_dict["Roles"]:
         role_name = role["RoleName"]
         if not re.search(
             r"ManagedOpenShift|AWS|OrganizationAccountAccessRole|pco-|RedHatIT|RH-",
             role_name,
         ):
             # Need to iterate over both list_attached_role_policies and list_role_policies
             # For attached policies, we need to detach them using ARN
-            attached_role_policies_dict = _iam_client.list_attached_role_policies(RoleName=role_name, MaxItems=1000)
+            attached_role_policies_dict = _iam_client.list_attached_role_policies(
+                RoleName=role_name, MaxItems=1000
+            )
             for attached_policy in attached_role_policies_dict["AttachedPolicies"]:
                 attached_policy_name = attached_policy["PolicyName"]
-                LOGGER.info(f"Detach policy {attached_policy_name} for role {role_name}")
-                _iam_client.detach_role_policy(RoleName=role_name, PolicyArn=attached_policy["PolicyArn"])
+                LOGGER.info(
+                    f"Detach policy {attached_policy_name} for role {role_name}"
+                )
+                _iam_client.detach_role_policy(
+                    RoleName=role_name, PolicyArn=attached_policy["PolicyArn"]
+                )
 
             # For detached policies, we need to delete them by name
-            detached_policy_names_dict = _iam_client.list_role_policies(RoleName=role_name, MaxItems=1000)
+            detached_policy_names_dict = _iam_client.list_role_policies(
+                RoleName=role_name, MaxItems=1000
+            )
             for detached_policy_name in detached_policy_names_dict["PolicyNames"]:
-                LOGGER.info(f"Delete policy {detached_policy_name} for role {role_name}")
-                _iam_client.delete_role_policy(RoleName=role_name, PolicyName=detached_policy_name)
+                LOGGER.info(
+                    f"Delete policy {detached_policy_name} for role {role_name}"
+                )
+                _iam_client.delete_role_policy(
+                    RoleName=role_name, PolicyName=detached_policy_name
+                )
 
             LOGGER.info(f"Delete role {role_name}")
             _iam_client.delete_role(RoleName=role_name)
 
-    return any([
-        roles_dict["IsTruncated"],
-        attached_role_policies_dict.get("IsTruncated"),
-        detached_policy_names_dict.get("IsTruncated"),
-    ])
+    return any(
+        [
+            roles_dict["IsTruncated"],
+            attached_role_policies_dict.get("IsTruncated"),
+            detached_policy_names_dict.get("IsTruncated"),
+        ]
+    )
 
 
-def delete_buckets(region_name: str) -> bool:
+def delete_buckets(region_name):
     LOGGER.info("Executing delete_buckets")
     _s3_client = s3_client(region_name=region_name)
     buckets_dict = _s3_client.list_buckets(MaxItems=MAX_ITEMS)
     for bucket in buckets_dict["Buckets"]:
-        delete_all_objects_from_s3_folder(bucket_name=bucket["Name"], boto_client=_s3_client)
+        delete_all_objects_from_s3_folder(
+            bucket_name=bucket["Name"], boto_client=_s3_client
+        )
         delete_bucket(bucket_name=bucket["Name"], boto_client=_s3_client)
 
     return buckets_dict.get("IsTruncated")
 
 
-def clean_aws_resources(aws_regions: List[str]) -> None:
+@click.command()
+@click.option(
+    "--aws-regions",
+    help="""
+        \b
+        Comma-separated string of AWS regions to delete resources from.
+        If not provided will iterate over all regions.
+        """,
+    required=False,
+)
+@click.option(
+    "--all-aws-regions",
+    help="""
+        \b
+        Run on all AWS regions.
+        """,
+    is_flag=True,
+)
+def main(aws_regions, all_aws_regions):
+    if all_aws_regions:
+        _aws_regions = aws_region_names()
+    elif aws_regions:
+        _aws_regions = aws_regions.split(",")
+    else:
+        click.echo("Either pass --all-aws-regions or --aws-regions to run cleanup")
+        raise click.Abort()
+
+    if not shutil.which("cloud-nuke"):
+        click.echo(
+            "cloud-nuke is not installed; install from https://github.com/gruntwork-io/cloud-nuke"
+        )
+        raise click.Abort()
+
+    set_and_verify_aws_credentials()
+
+    clean_aws_resources(aws_regions=_aws_regions)
+
+
+def clean_aws_resources(aws_regions):
     rerun_cleanup_regions_list = []
     jobs = []
-    cleanup_queue: Queue[str] = multiprocessing.Queue()
+    cleanup_queue = multiprocessing.Queue()
 
     for region in aws_regions:
         job = multiprocessing.Process(
             name=f"--- Clean up {region} ---",
             target=clean_aws_region,
             kwargs={"aws_region": region, "queue": cleanup_queue},
         )
@@ -131,34 +194,38 @@
     for _job in jobs:
         _job.join()
 
     if rerun_cleanup_regions_list:
         clean_aws_resources(aws_regions=rerun_cleanup_regions_list)
 
 
-def clean_aws_region(aws_region: str, queue: Queue[str]) -> None:
+def clean_aws_region(aws_region, queue):
     """Deletes AWS resources.
 
     Deletes open id connector providers, instance profiles and roles.
     (calls rds instances and vpc peerings connections - currently to only log data).
     Runs `cloud-nuke` utility - https://github.com/gruntwork-io/cloud-nuke
     Deletes S2 buckets.
     Adds aws_region to queue in case additional cleanup is needed.
 
     Args:
         aws_region (str): AWS region name
         queue (Queue): multiprocessing queue to pass result
 
     """
     LOGGER.info(f"Deleting resources in region {aws_region}")
-    rerun_results: List[bool] = [
+    rerun_results = [
         delete_rds_instances(region_name=aws_region),
         delete_vpc_peering_connections(region_name=aws_region),
         delete_open_id_connect_providers(region_name=aws_region),
         delete_instance_profiles(region_name=aws_region),
         delete_roles(region_name=aws_region),
     ]
     run_command(command=shlex.split(f"cloud-nuke aws --region {aws_region} --force"))
     rerun_results.append(delete_buckets(region_name=aws_region))
 
     if any(rerun_results):
         queue.put(aws_region)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `redhat_qe_cloud_tools-1.0.80/PKG-INFO` & `redhat_qe_cloud_tools-1.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,25 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.80
+Version: 1.0.9
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
-License: Apache-2.0
 Author: Meni Yakove
-Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: azure-core (>=1.30.1,<2.0.0)
-Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
-Requires-Dist: azure-mgmt-network (>=25.2.0,<26.0.0)
-Requires-Dist: azure-mgmt-redhatopenshift (>=1.4.0,<2.0.0)
-Requires-Dist: azure-mgmt-resource (>=23.0.1,<24.0.0)
-Requires-Dist: azure-mgmt-subscription (>=3.1.1,<4.0.0)
-Requires-Dist: boto3 (>=1.34.110,<2.0.0)
+Requires-Dist: boto3 (>=1.28.1,<2.0.0)
 Requires-Dist: click (>=8.1.4,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
-Requires-Dist: configparser (>=7.0.0,<8.0.0)
-Requires-Dist: google-cloud-compute (>=1.14.1,<2.0.0)
-Requires-Dist: openshift-python-utilities (>=5.0.46,<6.0.0)
-Requires-Dist: pyhelper-utils (>=0.0.21,<0.0.22)
-Requires-Dist: python-simple-logger (>=1.0.5)
-Project-URL: Bug Tracker, https://github.com/RedHatQE/cloud-tools/issues
-Project-URL: Documentation, https://github.com/RedHatQE/cloud-tools/blob/main/README.md
-Project-URL: Download, https://pypi.org/project/redhat-qe-cloud-tools/
+Requires-Dist: configparser (>=6.0.0,<7.0.0)
+Requires-Dist: openshift-python-utilities (>=4.14.2,<5.0.0)
+Requires-Dist: python-simple-logger (>=1.0.5,<2.0.0)
 Project-URL: Repository, https://github.com/RedHatQE/cloud-tools
 Description-Content-Type: text/markdown
 
 # cloud-tools
 Python utilities to manage cloud services, such as AWS.
 
 ## Local run
@@ -50,24 +34,23 @@
 
 ```
 poetry install
 ```
 
 ## Docs
 - [AWS Readme](clouds/aws/README.md)
-- [Cloud nuke CLI tools Readme](clouds/cli/README.md)
 
 ## Release new version
 ### requirements:
 * Export GitHub token
 ```bash
 export GITHUB_TOKEN=<your_github_token>
 ```
 * [release-it](https://github.com/release-it/release-it)
-Run the following once (execute outside repository dir for example `~/`):
+Run the following once:
 ```bash
 sudo npm install --global release-it
 npm install --save-dev @j-ulrich/release-it-regex-bumper
 rm -f package.json package-lock.json
 ```
 ### usage:
 * Create a release, run from the relevant branch.
```

