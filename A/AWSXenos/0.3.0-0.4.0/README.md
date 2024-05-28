# Comparing `tmp/awsxenos-0.3.0.tar.gz` & `tmp/awsxenos-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsxenos-0.3.0.tar", last modified: Tue May 14 08:56:55 2024, max compression
+gzip compressed data, was "awsxenos-0.4.0.tar", last modified: Tue May 28 08:45:26 2024, max compression
```

## Comparing `awsxenos-0.3.0.tar` & `awsxenos-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:55.022516 awsxenos-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:55.022516 awsxenos-0.3.0/AWSXenos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-14 08:56:55.000000 awsxenos-0.3.0/AWSXenos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 08:56:55.000000 awsxenos-0.3.0/AWSXenos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:56:55.000000 awsxenos-0.3.0/AWSXenos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-14 08:56:55.000000 awsxenos-0.3.0/AWSXenos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 08:56:55.000000 awsxenos-0.3.0/AWSXenos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 08:56:55.000000 awsxenos-0.3.0/AWSXenos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 08:56:46.000000 awsxenos-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-14 08:56:46.000000 awsxenos-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-14 08:56:55.022516 awsxenos-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-05-14 08:56:46.000000 awsxenos-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:55.018516 awsxenos-0.3.0/awsxenos/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92879 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/accounts.json
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5604 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:55.018516 awsxenos-0.3.0/awsxenos/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/efs.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/eventbridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/kms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/services/sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-14 08:56:46.000000 awsxenos-0.3.0/awsxenos/template.html
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-14 08:56:46.000000 awsxenos-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:56:55.022516 awsxenos-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-14 08:56:46.000000 awsxenos-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:55.022516 awsxenos-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:56:46.000000 awsxenos-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-14 08:56:46.000000 awsxenos-0.3.0/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-14 08:56:46.000000 awsxenos-0.3.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-14 08:56:46.000000 awsxenos-0.3.0/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:26.153775 awsxenos-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:26.153775 awsxenos-0.4.0/AWSXenos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-05-28 08:45:26.000000 awsxenos-0.4.0/AWSXenos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-28 08:45:26.000000 awsxenos-0.4.0/AWSXenos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:45:26.000000 awsxenos-0.4.0/AWSXenos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 08:45:26.000000 awsxenos-0.4.0/AWSXenos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 08:45:26.000000 awsxenos-0.4.0/AWSXenos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 08:45:26.000000 awsxenos-0.4.0/AWSXenos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-28 08:45:22.000000 awsxenos-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 08:45:22.000000 awsxenos-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-05-28 08:45:26.153775 awsxenos-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-28 08:45:22.000000 awsxenos-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:26.149775 awsxenos-0.4.0/awsxenos/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92879 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/accounts.json
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6049 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:26.153775 awsxenos-0.4.0/awsxenos/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/efs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/eventbridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/kms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/sns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/services/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-28 08:45:22.000000 awsxenos-0.4.0/awsxenos/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-28 08:45:22.000000 awsxenos-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:45:26.153775 awsxenos-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-28 08:45:22.000000 awsxenos-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:26.153775 awsxenos-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 08:45:22.000000 awsxenos-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-28 08:45:22.000000 awsxenos-0.4.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-28 08:45:22.000000 awsxenos-0.4.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-28 08:45:22.000000 awsxenos-0.4.0/tests/test_scan.py
```

### Comparing `awsxenos-0.3.0/AWSXenos.egg-info/PKG-INFO` & `awsxenos-0.4.0/AWSXenos.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: AWSXenos
-Version: 0.3.0
+Version: 0.4.0
 Summary: Scan and classify cross-account roles and resources in your AWS Account
 Home-page: https://github.com/AirWalk-Digital/AWSXenos
 Author: Costas Kourmpoglou
 Author-email: costas.kourmpoglou@airwalkconsulting.com
 License: MIT
 Keywords: aws iam cross-account roles security
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: policyuniverse==1.5.1.20231109
 Requires-Dist: boto3==1.34.101
-Requires-Dist: jinja2==3.1.3
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: pyyaml==6.0.1
 
 # AWS External Account Scanner
 
 > Xenos, is Greek for stranger.
 
 AWSXenos will assess the trust relationships in all the IAM roles, and resource policies for [several AWS services](#aws-iam-access-analyzer-comparison) in an AWS account and give you a breakdown of all the accounts that have trust relationships to your account. It will also highlight whether the trusts have an [external ID](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html) or not.
@@ -46,14 +46,15 @@
 
 2. Identified external entities might be known entities. E.g. a trusted third party vendor or a vendor you no longer trust. An Account number is seldom useful. 
 
 3. Zone of trust is a fixed set of the AWS organisation. You won’t know if a trust between sandbox->prod has been established. 
 
 4. Does not identify AWS Service principals. This is mainly important because of [Wiz's AWSConfig, et al vulnverabilities](http://i.blackhat.com/USA21/Wednesday-Handouts/us-21-Breaking-The-Isolation-Cross-Account-AWS-Vulnerabilities.pdf)
 
+
 ## AWS IAM Access Analyzer comparison 
 
 Comparison based on AWS Documentation [1](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_aws-services-that-work-with-iam.html) and [2](https://docs.aws.amazon.com/IAM/latest/UserGuide/what-is-access-analyzer.html#what-is-access-analyzer-resource-identification), including services or resources outside of docs, e.g. VPC endpoints.
 
 
 | Service | AWSXenos | Access Analyzer |
 | :--: | :--: | :--: |
@@ -62,38 +63,38 @@
 | S3 Access Points | :x: |  :white_check_mark: |
 | S3 Bucket ACLs | :white_check_mark: | :white_check_mark: |
 | S3 Glacier | :white_check_mark: | :x: |
 | IAM |  :white_check_mark: |  :white_check_mark: |
 | KMS |  :white_check_mark: |  :white_check_mark: |
 | Secrets Manager |  :white_check_mark: |  :white_check_mark: |
 | Lambda | :white_check_mark: |  :white_check_mark: |
-| SNS | :x: |  :white_check_mark: |
+| SNS | :white_check_mark: |  :white_check_mark: |
 | SQS | :white_check_mark: |  :white_check_mark: |
 | RDS Snapshots | :x: |  :white_check_mark: |
 | RDS Cluster Snapshots | :x: |  :white_check_mark: |
 | ECR | :x: |  :white_check_mark: |
 | EFS | :white_check_mark: |  :white_check_mark: |
-| DynamoDB streams | :x: |  :white_check_mark: |
-| DynamoDB tables | :x: |  :white_check_mark: |
+| DynamoDB streams |  :white_check_mark: |  :white_check_mark: |
+| DynamoDB tables |  :white_check_mark: |  :white_check_mark: |
 | EBS Snapshots | :x: |  :white_check_mark: |
 | EventBridge | :white_check_mark: | :x: |
 | EventBridge Schema | :x: | :x: |
 | Mediastore | :x: | :x: |
 | Glue | :x: | :x: |
-| Kinesis Data Streams | :x: | :x: |
+| Kinesis Data Streams | :white_check_mark: | :x: |
 | Lex v2 | :x: | :x: |
 | Migration Hub Orchestrator | :x: | :x: |
-| OpenSearch | :x: | :x: |
+| OpenSearch | :white_check_mark: | :x: |
 | AWS PCA | :x: | :x: |
 | Redshift Serverless | :x: | :x: |
 | Serverless Application Repository | :x: | :x: |
 | SES v2 | :x: | :x: |
 | Incident Manager | :x: | :x: |
 | Incident Manager Contacts | :x: | :x: |
-| VPC endpoints | :x: | :x: |
+| VPC endpoints | :white_check_mark: | :x: |
 
 ## How to run
 
 ### Cli
 ```sh
 pip install AWSXenos
 awsxenos --reporttype HTML -w report.html
@@ -126,38 +127,49 @@
 r = Report(s.findings, s.known_accounts)
 json_summary = r.JSON_report()
 html_summary = r.HTML_report()
 ```
 
 ### IAM Permissions
 
-Permissions required.
+Permissions required to scan all services.
 
 ```json
 {
   "Version": "2012-10-17",
   "Statement": [
     {
       "Action": [
+        "dynamodb:GetResourcePolicy",
+        "dynamodb:ListStreams",
+        "dynamodb:ListTables",
+        "ec2:DescribeVpcEndpoints",
         "elasticfilesystem:DescribeFileSystemPolicy",
         "elasticfilesystem:DescribeFileSystems",
+        "es:DescribeDomains",
+        "es:ListDomainNames",
         "events:ListEventBuses",
         "glacier:GetVaultAccessPolicy",
         "glacier:ListVaults",
         "iam:ListRoles",
-        "organizations:ListAccounts",
+        "kinesis:GetResourcePolicy",
+        "kinesis:ListStreams", 
         "kms:GetKeyPolicy",
         "kms:ListKeys",
         "lambda:GetPolicy",
         "lambda:ListFunctions",
+        "organizations:DescribeOrganization",
+        "organizations:ListAccounts",
         "s3:GetBucketAcl",
         "s3:GetBucketPolicy",
         "s3:ListAllMyBuckets",
         "secretsmanager:GetResourcePolicy",
         "secretsmanager:ListSecrets",
+        "sns:GetTopicAttributes",
+        "sns:ListTopics",
         "sqs:GetQueueAttributes",
         "sqs:ListQueues"
       ],
       "Effect": "Allow",
       "Resource": "*"
     }
   ]
@@ -177,29 +189,34 @@
 3. Your class must inherit from `Service` and return `Findings`
 
 Example: 
 
 ```python
 class S3(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set] ) -> Findings:
+    def fetch(self, accounts: Accounts ) -> Findings:
         self._buckets = self.list_account_buckets()
         self.policies = self.get_bucket_policies()
         return super().collate(accounts, self.policies)
 ```
 4. Add your filename and class to the config
 
 ---
 
-:warning: AWSXenos currently assesses access based on [https://github.com/Netflix-Skunkworks/policyuniverse](https://github.com/Netflix-Skunkworks/policyuniverse).
-There are cases where IAM `conditions`, will _not_ be taken into account, therefore resulting in false positives. 
-This could be fairly common in KMS Customer Managed Keys created by AWS Services.
-AWSXenos findings are per IAM statement on an IAM policy.
+## FAQ
+
+### Are there false positives?
+Yes. AWSXenos doesn't take into consideration Identity or SCP. It assumes that everything else other than the resource or trust policy _has_ access. 
 
-## I want to add more known accounts
-Create a PR or raise an issue. Contributions are welcome.
+### Is this using an SMT Solver or automated reasoning ?
+No. AWSXenos only takes into account resource and IAM trust policies. Maybe in the next project or iteration.
 
+### Why not use [CheckAccessNotGranted](https://docs.aws.amazon.com/access-analyzer/latest/APIReference/API_CheckAccessNotGranted.html) ?
+We don't know the set of accounts that shouldn't access the resource or role.
 
+### How does it work ?
+AWSXenos currently assesses access based on [https://github.com/Netflix-Skunkworks/policyuniverse](https://github.com/Netflix-Skunkworks/policyuniverse).
 
 ## Features
 - [x] Use as library
 - [x] HTML and JSON output 
+- [x] Multi-threaded querying of each service
```

### Comparing `awsxenos-0.3.0/LICENSE` & `awsxenos-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `awsxenos-0.3.0/PKG-INFO` & `awsxenos-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: AWSXenos
-Version: 0.3.0
+Version: 0.4.0
 Summary: Scan and classify cross-account roles and resources in your AWS Account
 Home-page: https://github.com/AirWalk-Digital/AWSXenos
 Author: Costas Kourmpoglou
 Author-email: costas.kourmpoglou@airwalkconsulting.com
 License: MIT
 Keywords: aws iam cross-account roles security
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: policyuniverse==1.5.1.20231109
 Requires-Dist: boto3==1.34.101
-Requires-Dist: jinja2==3.1.3
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: pyyaml==6.0.1
 
 # AWS External Account Scanner
 
 > Xenos, is Greek for stranger.
 
 AWSXenos will assess the trust relationships in all the IAM roles, and resource policies for [several AWS services](#aws-iam-access-analyzer-comparison) in an AWS account and give you a breakdown of all the accounts that have trust relationships to your account. It will also highlight whether the trusts have an [external ID](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_create_for-user_externalid.html) or not.
@@ -46,14 +46,15 @@
 
 2. Identified external entities might be known entities. E.g. a trusted third party vendor or a vendor you no longer trust. An Account number is seldom useful. 
 
 3. Zone of trust is a fixed set of the AWS organisation. You won’t know if a trust between sandbox->prod has been established. 
 
 4. Does not identify AWS Service principals. This is mainly important because of [Wiz's AWSConfig, et al vulnverabilities](http://i.blackhat.com/USA21/Wednesday-Handouts/us-21-Breaking-The-Isolation-Cross-Account-AWS-Vulnerabilities.pdf)
 
+
 ## AWS IAM Access Analyzer comparison 
 
 Comparison based on AWS Documentation [1](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_aws-services-that-work-with-iam.html) and [2](https://docs.aws.amazon.com/IAM/latest/UserGuide/what-is-access-analyzer.html#what-is-access-analyzer-resource-identification), including services or resources outside of docs, e.g. VPC endpoints.
 
 
 | Service | AWSXenos | Access Analyzer |
 | :--: | :--: | :--: |
@@ -62,38 +63,38 @@
 | S3 Access Points | :x: |  :white_check_mark: |
 | S3 Bucket ACLs | :white_check_mark: | :white_check_mark: |
 | S3 Glacier | :white_check_mark: | :x: |
 | IAM |  :white_check_mark: |  :white_check_mark: |
 | KMS |  :white_check_mark: |  :white_check_mark: |
 | Secrets Manager |  :white_check_mark: |  :white_check_mark: |
 | Lambda | :white_check_mark: |  :white_check_mark: |
-| SNS | :x: |  :white_check_mark: |
+| SNS | :white_check_mark: |  :white_check_mark: |
 | SQS | :white_check_mark: |  :white_check_mark: |
 | RDS Snapshots | :x: |  :white_check_mark: |
 | RDS Cluster Snapshots | :x: |  :white_check_mark: |
 | ECR | :x: |  :white_check_mark: |
 | EFS | :white_check_mark: |  :white_check_mark: |
-| DynamoDB streams | :x: |  :white_check_mark: |
-| DynamoDB tables | :x: |  :white_check_mark: |
+| DynamoDB streams |  :white_check_mark: |  :white_check_mark: |
+| DynamoDB tables |  :white_check_mark: |  :white_check_mark: |
 | EBS Snapshots | :x: |  :white_check_mark: |
 | EventBridge | :white_check_mark: | :x: |
 | EventBridge Schema | :x: | :x: |
 | Mediastore | :x: | :x: |
 | Glue | :x: | :x: |
-| Kinesis Data Streams | :x: | :x: |
+| Kinesis Data Streams | :white_check_mark: | :x: |
 | Lex v2 | :x: | :x: |
 | Migration Hub Orchestrator | :x: | :x: |
-| OpenSearch | :x: | :x: |
+| OpenSearch | :white_check_mark: | :x: |
 | AWS PCA | :x: | :x: |
 | Redshift Serverless | :x: | :x: |
 | Serverless Application Repository | :x: | :x: |
 | SES v2 | :x: | :x: |
 | Incident Manager | :x: | :x: |
 | Incident Manager Contacts | :x: | :x: |
-| VPC endpoints | :x: | :x: |
+| VPC endpoints | :white_check_mark: | :x: |
 
 ## How to run
 
 ### Cli
 ```sh
 pip install AWSXenos
 awsxenos --reporttype HTML -w report.html
@@ -126,38 +127,49 @@
 r = Report(s.findings, s.known_accounts)
 json_summary = r.JSON_report()
 html_summary = r.HTML_report()
 ```
 
 ### IAM Permissions
 
-Permissions required.
+Permissions required to scan all services.
 
 ```json
 {
   "Version": "2012-10-17",
   "Statement": [
     {
       "Action": [
+        "dynamodb:GetResourcePolicy",
+        "dynamodb:ListStreams",
+        "dynamodb:ListTables",
+        "ec2:DescribeVpcEndpoints",
         "elasticfilesystem:DescribeFileSystemPolicy",
         "elasticfilesystem:DescribeFileSystems",
+        "es:DescribeDomains",
+        "es:ListDomainNames",
         "events:ListEventBuses",
         "glacier:GetVaultAccessPolicy",
         "glacier:ListVaults",
         "iam:ListRoles",
-        "organizations:ListAccounts",
+        "kinesis:GetResourcePolicy",
+        "kinesis:ListStreams", 
         "kms:GetKeyPolicy",
         "kms:ListKeys",
         "lambda:GetPolicy",
         "lambda:ListFunctions",
+        "organizations:DescribeOrganization",
+        "organizations:ListAccounts",
         "s3:GetBucketAcl",
         "s3:GetBucketPolicy",
         "s3:ListAllMyBuckets",
         "secretsmanager:GetResourcePolicy",
         "secretsmanager:ListSecrets",
+        "sns:GetTopicAttributes",
+        "sns:ListTopics",
         "sqs:GetQueueAttributes",
         "sqs:ListQueues"
       ],
       "Effect": "Allow",
       "Resource": "*"
     }
   ]
@@ -177,29 +189,34 @@
 3. Your class must inherit from `Service` and return `Findings`
 
 Example: 
 
 ```python
 class S3(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set] ) -> Findings:
+    def fetch(self, accounts: Accounts ) -> Findings:
         self._buckets = self.list_account_buckets()
         self.policies = self.get_bucket_policies()
         return super().collate(accounts, self.policies)
 ```
 4. Add your filename and class to the config
 
 ---
 
-:warning: AWSXenos currently assesses access based on [https://github.com/Netflix-Skunkworks/policyuniverse](https://github.com/Netflix-Skunkworks/policyuniverse).
-There are cases where IAM `conditions`, will _not_ be taken into account, therefore resulting in false positives. 
-This could be fairly common in KMS Customer Managed Keys created by AWS Services.
-AWSXenos findings are per IAM statement on an IAM policy.
+## FAQ
+
+### Are there false positives?
+Yes. AWSXenos doesn't take into consideration Identity or SCP. It assumes that everything else other than the resource or trust policy _has_ access. 
 
-## I want to add more known accounts
-Create a PR or raise an issue. Contributions are welcome.
+### Is this using an SMT Solver or automated reasoning ?
+No. AWSXenos only takes into account resource and IAM trust policies. Maybe in the next project or iteration.
 
+### Why not use [CheckAccessNotGranted](https://docs.aws.amazon.com/access-analyzer/latest/APIReference/API_CheckAccessNotGranted.html) ?
+We don't know the set of accounts that shouldn't access the resource or role.
 
+### How does it work ?
+AWSXenos currently assesses access based on [https://github.com/Netflix-Skunkworks/policyuniverse](https://github.com/Netflix-Skunkworks/policyuniverse).
 
 ## Features
 - [x] Use as library
 - [x] HTML and JSON output 
+- [x] Multi-threaded querying of each service
```

### Comparing `awsxenos-0.3.0/README.md` & `awsxenos-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 2. Identified external entities might be known entities. E.g. a trusted third party vendor or a vendor you no longer trust. An Account number is seldom useful. 
 
 3. Zone of trust is a fixed set of the AWS organisation. You won’t know if a trust between sandbox->prod has been established. 
 
 4. Does not identify AWS Service principals. This is mainly important because of [Wiz's AWSConfig, et al vulnverabilities](http://i.blackhat.com/USA21/Wednesday-Handouts/us-21-Breaking-The-Isolation-Cross-Account-AWS-Vulnerabilities.pdf)
 
+
 ## AWS IAM Access Analyzer comparison 
 
 Comparison based on AWS Documentation [1](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_aws-services-that-work-with-iam.html) and [2](https://docs.aws.amazon.com/IAM/latest/UserGuide/what-is-access-analyzer.html#what-is-access-analyzer-resource-identification), including services or resources outside of docs, e.g. VPC endpoints.
 
 
 | Service | AWSXenos | Access Analyzer |
 | :--: | :--: | :--: |
@@ -42,38 +43,38 @@
 | S3 Access Points | :x: |  :white_check_mark: |
 | S3 Bucket ACLs | :white_check_mark: | :white_check_mark: |
 | S3 Glacier | :white_check_mark: | :x: |
 | IAM |  :white_check_mark: |  :white_check_mark: |
 | KMS |  :white_check_mark: |  :white_check_mark: |
 | Secrets Manager |  :white_check_mark: |  :white_check_mark: |
 | Lambda | :white_check_mark: |  :white_check_mark: |
-| SNS | :x: |  :white_check_mark: |
+| SNS | :white_check_mark: |  :white_check_mark: |
 | SQS | :white_check_mark: |  :white_check_mark: |
 | RDS Snapshots | :x: |  :white_check_mark: |
 | RDS Cluster Snapshots | :x: |  :white_check_mark: |
 | ECR | :x: |  :white_check_mark: |
 | EFS | :white_check_mark: |  :white_check_mark: |
-| DynamoDB streams | :x: |  :white_check_mark: |
-| DynamoDB tables | :x: |  :white_check_mark: |
+| DynamoDB streams |  :white_check_mark: |  :white_check_mark: |
+| DynamoDB tables |  :white_check_mark: |  :white_check_mark: |
 | EBS Snapshots | :x: |  :white_check_mark: |
 | EventBridge | :white_check_mark: | :x: |
 | EventBridge Schema | :x: | :x: |
 | Mediastore | :x: | :x: |
 | Glue | :x: | :x: |
-| Kinesis Data Streams | :x: | :x: |
+| Kinesis Data Streams | :white_check_mark: | :x: |
 | Lex v2 | :x: | :x: |
 | Migration Hub Orchestrator | :x: | :x: |
-| OpenSearch | :x: | :x: |
+| OpenSearch | :white_check_mark: | :x: |
 | AWS PCA | :x: | :x: |
 | Redshift Serverless | :x: | :x: |
 | Serverless Application Repository | :x: | :x: |
 | SES v2 | :x: | :x: |
 | Incident Manager | :x: | :x: |
 | Incident Manager Contacts | :x: | :x: |
-| VPC endpoints | :x: | :x: |
+| VPC endpoints | :white_check_mark: | :x: |
 
 ## How to run
 
 ### Cli
 ```sh
 pip install AWSXenos
 awsxenos --reporttype HTML -w report.html
@@ -106,38 +107,49 @@
 r = Report(s.findings, s.known_accounts)
 json_summary = r.JSON_report()
 html_summary = r.HTML_report()
 ```
 
 ### IAM Permissions
 
-Permissions required.
+Permissions required to scan all services.
 
 ```json
 {
   "Version": "2012-10-17",
   "Statement": [
     {
       "Action": [
+        "dynamodb:GetResourcePolicy",
+        "dynamodb:ListStreams",
+        "dynamodb:ListTables",
+        "ec2:DescribeVpcEndpoints",
         "elasticfilesystem:DescribeFileSystemPolicy",
         "elasticfilesystem:DescribeFileSystems",
+        "es:DescribeDomains",
+        "es:ListDomainNames",
         "events:ListEventBuses",
         "glacier:GetVaultAccessPolicy",
         "glacier:ListVaults",
         "iam:ListRoles",
-        "organizations:ListAccounts",
+        "kinesis:GetResourcePolicy",
+        "kinesis:ListStreams", 
         "kms:GetKeyPolicy",
         "kms:ListKeys",
         "lambda:GetPolicy",
         "lambda:ListFunctions",
+        "organizations:DescribeOrganization",
+        "organizations:ListAccounts",
         "s3:GetBucketAcl",
         "s3:GetBucketPolicy",
         "s3:ListAllMyBuckets",
         "secretsmanager:GetResourcePolicy",
         "secretsmanager:ListSecrets",
+        "sns:GetTopicAttributes",
+        "sns:ListTopics",
         "sqs:GetQueueAttributes",
         "sqs:ListQueues"
       ],
       "Effect": "Allow",
       "Resource": "*"
     }
   ]
@@ -157,29 +169,34 @@
 3. Your class must inherit from `Service` and return `Findings`
 
 Example: 
 
 ```python
 class S3(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set] ) -> Findings:
+    def fetch(self, accounts: Accounts ) -> Findings:
         self._buckets = self.list_account_buckets()
         self.policies = self.get_bucket_policies()
         return super().collate(accounts, self.policies)
 ```
 4. Add your filename and class to the config
 
 ---
 
-:warning: AWSXenos currently assesses access based on [https://github.com/Netflix-Skunkworks/policyuniverse](https://github.com/Netflix-Skunkworks/policyuniverse).
-There are cases where IAM `conditions`, will _not_ be taken into account, therefore resulting in false positives. 
-This could be fairly common in KMS Customer Managed Keys created by AWS Services.
-AWSXenos findings are per IAM statement on an IAM policy.
+## FAQ
+
+### Are there false positives?
+Yes. AWSXenos doesn't take into consideration Identity or SCP. It assumes that everything else other than the resource or trust policy _has_ access. 
 
-## I want to add more known accounts
-Create a PR or raise an issue. Contributions are welcome.
+### Is this using an SMT Solver or automated reasoning ?
+No. AWSXenos only takes into account resource and IAM trust policies. Maybe in the next project or iteration.
 
+### Why not use [CheckAccessNotGranted](https://docs.aws.amazon.com/access-analyzer/latest/APIReference/API_CheckAccessNotGranted.html) ?
+We don't know the set of accounts that shouldn't access the resource or role.
 
+### How does it work ?
+AWSXenos currently assesses access based on [https://github.com/Netflix-Skunkworks/policyuniverse](https://github.com/Netflix-Skunkworks/policyuniverse).
 
 ## Features
 - [x] Use as library
-- [x] HTML and JSON output 
+- [x] HTML and JSON output 
+- [x] Multi-threaded querying of each service
```

### Comparing `awsxenos-0.3.0/awsxenos/accounts.json` & `awsxenos-0.4.0/awsxenos/accounts.json`

 * *Files identical despite different names*

### Comparing `awsxenos-0.3.0/awsxenos/finding.py` & `awsxenos-0.4.0/awsxenos/finding.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 from collections import defaultdict, UserDict
 from dataclasses import dataclass, field
-from typing import Any, DefaultDict, List, Set
+from typing import Any, DefaultDict, List
 
 from policyuniverse.arn import ARN  # type: ignore
 from policyuniverse.policy import Policy  # type: ignore
-from policyuniverse.statement import ConditionTuple  # type: ignore
+from policyuniverse.statement import ConditionTuple, Statement  # type: ignore
 
 
 @dataclass
 class Finding:
     principal: str
     external_id: bool
 
@@ -22,108 +22,127 @@
 
 @dataclass
 class Accounts:
     org_accounts: List[Finding] = field(default_factory=list)
     known_accounts: List[Finding] = field(default_factory=list)
     unknown_accounts: List[Finding] = field(default_factory=list)
     aws_services: List[Finding] = field(default_factory=list)
+    org_id: str = ""
 
     def __getitem__(self, key):
         return super().__getattribute__(key)
 
+    def __contains__(self, key):
+        return getattr(self, key)
+
+
+"""Container for Finding"""
+
 
 class Findings(UserDict):
     def __missing__(self, key):
         self[key] = Accounts()
         return self[key]
 
 
+""" Container for any resource, e.g. IAM roles returned by a service
+    Expects a key of arn and a value of the policy
+"""
+
+
 class Resources(UserDict):
     def __missing__(self, key):
         self[key] = defaultdict()
         return self[key]
 
 
+"""Main class to derive from when implementing other services"""
+
+
 class Service(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def fetch(self, accounts: DefaultDict[str, Set], **kwargs) -> Findings:
+    def fetch(self, accounts: Accounts, **kwargs) -> Findings:
         raise NotImplementedError
 
-    def collate(self, accounts: DefaultDict[str, Set], resources: Resources) -> Findings:
-        """Combine all accounts with all the resources to classify findings. Try custom_collate first and fallback to this.
+    def _get_account_type(self, account: str, accounts: Accounts) -> str:
+        account_types = ["org_accounts", "known_accounts"]
+        for account_type in account_types:
+            if account in accounts[account_type]:
+                return account_type
+        return "unknown_accounts"
+
+    def collate(self, accounts: Accounts, resources: Resources) -> Findings:
+        """Combine all accounts with all the resources to classify findings.
+            This is the default collation function called by Service
 
         Args:
-            accounts (DefaultDict[str, Set]): Key of account type. Value account ids
-            resources (DefaultDict[str, Dict[Any, Any]]): Key ResourceIdentifier. Value Dict PolicyDocument
+            accounts (Accounts): Key of account type. Value account ids
+            resources (Resources): Key ResourceIdentifier. Value Dict PolicyDocument
 
         Returns:
             DefaultDict[str, AccountType]: Key of ARN, Value of AccountType
         """
 
         findings = Findings()
-        for resource, policy_document in resources.items():
+
+        for resource, policy_document in resources.items():  # TODO: extract the IAM trust policy logic
             try:
                 policy = Policy(policy_document)
             except:
-                continue
-            for unparsed_principal in policy.whos_allowed():
-                try:
-                    principal = ARN(unparsed_principal.value)  # type: Any
-                except Exception as e:
-                    print(e)
-                    findings[resource].known_accounts.append(Finding(principal=unparsed_principal, external_id=True))
+                continue  # TODO: Don't fail silently
+            for st in policy.statements:
+                if st.effect != "Allow":
                     continue
-                # Check if Principal is an AWS Service
-                if principal.service:
-                    findings[resource].aws_services.append(Finding(principal=principal.arn, external_id=True))
-                # Check against org_accounts
-                elif principal.account_number in accounts["org_accounts"]:
-                    findings[resource].org_accounts.append(Finding(principal=principal.arn, external_id=True))
-                # Check against known external accounts
-                elif (
-                    principal.account_number in accounts["known_accounts"]
-                    or ConditionTuple(category="saml-endpoint", value="https://signin.aws.amazon.com/saml")
-                    in policy.whos_allowed()
-                ):
-                    sts_set = False
-                    for pstate in policy.statements:
-                        if "sts" in pstate.action_summary():
-                            try:
-                                conditions = [
-                                    k.lower() for k in list(pstate.statement["Condition"]["StringEquals"].keys())
-                                ]
-                                if "sts:externalid" in conditions:
-                                    findings[resource].known_accounts.append(
-                                        Finding(principal=principal.arn, external_id=True)
-                                    )
-                            except:
-                                findings[resource].known_accounts.append(
-                                    Finding(principal=principal.arn, external_id=False)
+                for unparsed_principal in st.principals:  # There is always a principal - including "*"
+                    principal = ARN(unparsed_principal)
+                    if st.condition_accounts:  # If condition exists on account, it's an account
+                        for account in st.condition_accounts:
+                            findings[resource][self._get_account_type(account, accounts)].append(
+                                Finding(principal=account, external_id=True)
+                            )
+                    elif st.condition_orgids:  # If condition exists on orgid, it's the orgid
+                        for org_id in st.condition_orgids:
+                            if accounts.org_id == org_id:
+                                findings[resource]["org_accounts"].append(
+                                    Finding(principal=principal.arn, external_id=True)  # type: ignore
+                                )
+                            else:
+                                findings[resource]["unknown_accounts"].append(
+                                    Finding(principal=principal.arn, external_id=True)  # type: ignore
                                 )
-                            finally:
-                                sts_set = True
-                                break
-                    if not sts_set:
-                        findings[resource].known_accounts.append(Finding(principal=principal.arn, external_id=False))
-
-                # Unknown Account
-                else:
-                    sts_set = False
-                    for pstate in policy.statements:
-                        if "sts" in pstate.action_summary():
+                    elif principal.account_number:  # if there are no conditions
+                        if "sts" in st.action_summary():  # IAM Assume Role
                             try:
-                                conditions = [
-                                    k.lower() for k in list(pstate.statement["Condition"]["StringEquals"].keys())
-                                ]
+                                conditions = [k.lower() for k in list(st.statement["Condition"]["StringEquals"].keys())]
                                 if "sts:externalid" in conditions:
-                                    findings[resource].unknown_accounts.append(
-                                        Finding(principal=principal.arn, external_id=True)
+                                    findings[resource][
+                                        self._get_account_type(principal.account_number, accounts)
+                                    ].append(
+                                        Finding(principal=principal.arn, external_id=True)  # type: ignore
+                                    )
+                                else:
+                                    findings[resource][
+                                        self._get_account_type(principal.account_number, accounts)
+                                    ].append(
+                                        Finding(principal=principal.arn, external_id=False)  # type: ignore
                                     )
                             except:
-                                findings[resource].unknown_accounts.append(
-                                    Finding(principal=principal.arn, external_id=False)
+                                findings[resource][self._get_account_type(principal.account_number, accounts)].append(
+                                    Finding(principal=principal.arn, external_id=False)  # type: ignore
                                 )
-                            finally:
-                                break
-                    if not sts_set:
-                        findings[resource].unknown_accounts.append(Finding(principal=principal.arn, external_id=False))
+                        else:
+                            findings[resource][self._get_account_type(principal.account_number, accounts)].append(
+                                Finding(principal=principal.arn, external_id=True)  # type: ignore
+                            )
+                    elif not principal.account_number and principal.service:  # It's an aws service
+                        findings[resource].aws_services.append(
+                            Finding(principal=principal.arn, external_id=True)  # type: ignore
+                        )
+                    elif not principal.account_number and not principal.service:  # It's anonymous
+                        findings[resource].unknown_accounts.append(
+                            Finding(principal=principal.arn, external_id=True)  # type: ignore
+                        )
+                    else:  # Catch-all
+                        findings[resource].unknown_accounts.append(
+                            Finding(principal=principal, external_id=True)  # type: ignore
+                        )
         return findings
```

### Comparing `awsxenos-0.3.0/awsxenos/report.py` & `awsxenos-0.4.0/awsxenos/report.py`

 * *Files identical despite different names*

### Comparing `awsxenos-0.3.0/awsxenos/scan.py` & `awsxenos-0.4.0/awsxenos/scan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import argparse
 import concurrent.futures
 import importlib
 import json
+import logging
 import sys
 
 from typing import Any, Callable, Dict
 
 import boto3  # type: ignore
 import yaml  # type: ignore
 
@@ -19,22 +20,37 @@
 High level architecture
 
 1. Run prescan to collect org_accounts and buckets. 
 2. Load config, instantiate classes, submit to ThreadPoolExecutor to run "fetch"
 3. Each fetch will return `Findings` by running `collate` or `custom_collate`
 4. Pass the findings to `Report`
 """
+logging.basicConfig(
+    format="%(asctime)s, %(msecs)d %(name)s %(levelname)s - %(filename)s:%(lineno)d - %(message)s",
+    level=logging.INFO,
+    filename="awsxenos.log",
+)
+logger = logging.getLogger("awsxenos")
 
 
 class PreScan:
     def __init__(self):
         self.known_accounts = Resources()
         self._buckets = self.list_account_buckets()
         self.accounts = self.get_all_accounts()
 
+    def get_org_id(self):
+        orgs = boto3.client("organizations")
+        try:
+            return orgs.describe_organization()["Organization"]["Id"]
+        except:
+            logger.error("[!] - Failed to get organization ID")
+            logger.error(e)
+        return "o-xxxxxxxxxx"
+
     def get_org_accounts(self) -> Resources:
         """Get Account Ids from the AWS Organization
 
         Returns:
             DefaultDict: Key of Account Ids. Value of other Information
         """
         accounts = Resources()
@@ -43,29 +59,30 @@
         try:
             account_iterator = paginator.paginate()
             for account_resp in account_iterator:
                 for account in account_resp["Accounts"]:
                     accounts[account["Id"]] = account
             return accounts
         except Exception as e:
-            print("[!] - Failed to get organization accounts")
-            print(e)
+            logger.error("[!] - Failed to get organization accounts")
+            logger.error(e)
         return accounts
 
     def list_account_buckets(self) -> Dict[str, Dict[Any, Any]]:
         s3 = boto3.client("s3")
         return s3.list_buckets()
 
     def get_all_accounts(self) -> Accounts:
         """Get all known accounts and from the AWS Organization
 
         Returns:
             DefaultDict[str, Set]: Key of account type. Value account ids
         """
         accounts = Accounts()
+        accounts.org_id = self.get_org_id()
 
         with open(f"{package_path.resolve().parent}/accounts.json", "r") as f:
             accounts_file = json.load(f)
             for account in accounts_file:
                 self.known_accounts[account["id"]] = account
 
         accounts.known_accounts = set(self.known_accounts.keys())  # type: ignore
@@ -114,17 +131,15 @@
             future_to_name[future] = plugin["module"] + "." + plugin["class"]
 
         for future in concurrent.futures.as_completed(future_to_name):
             name = future_to_name[future]
             try:
                 results.update(future.result())
             except Exception as e:
-                # TODO: Better handling, add logger
-                print(f"Failed at {name} with: {e}")
-                # results[name] = str(e)  # Store the exception if the function call fails
+                logger.error(f"Failed at {name} with: {e}")
     return results
 
 
 def cli():
     parser = argparse.ArgumentParser(description="Scan an AWS Account for external trusts")
 
     parser.add_argument(
```

### Comparing `awsxenos-0.3.0/awsxenos/services/efs.py` & `awsxenos-0.4.0/awsxenos/services/efs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,45 @@
 import json
-from typing import DefaultDict, Set
 
 import boto3  # type: ignore
+from botocore.client import ClientError  # type: ignore
 
-from awsxenos.finding import Findings, Resources, Service
+from awsxenos.finding import Accounts, Findings, Resources, Service
 
 """EFS Resource Policies"""
 
 
 class EFSResource(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set]) -> Findings:  # type: ignore
+    def fetch(self, accounts: Accounts) -> Findings:  # type: ignore
         return super().collate(accounts, self.get_efs_policies())
 
     def get_efs_policies(self) -> Resources:
         filesystems = Resources()
         efs = boto3.client("efs")
         paginator = efs.get_paginator("describe_file_systems")
         for page in paginator.paginate():
             if "FileSystems" not in page:
                 continue
             for fs in page["FileSystems"]:
-                filesystems[fs["FileSystemArn"]] = json.loads(
-                    efs.describe_file_system_policy(FileSystemId=fs["FileSystemId"])["Policy"]
-                )
+                try:
+                    filesystems[fs["FileSystemArn"]] = json.loads(
+                        efs.describe_file_system_policy(FileSystemId=fs["FileSystemId"])["Policy"]
+                    )
+                except ClientError as e:
+                    if e.response["Error"]["Code"] == "PolicyNotFound":
+                        continue
+                    else:
+                        filesystems[fs["FileSystemArn"]] = {
+                            "Version": "2012-10-17",
+                            "Statement": [
+                                {
+                                    "Sid": "Exception",
+                                    "Effect": "Allow",
+                                    "Principal": {"AWS": "*"},
+                                    "Action": ["efs:*"],
+                                    "Resource": "*",
+                                }
+                            ],
+                        }
+
         return filesystems
```

### Comparing `awsxenos-0.3.0/awsxenos/services/iam.py` & `awsxenos-0.4.0/awsxenos/services/iam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import DefaultDict, Optional, Set
+from typing import Optional
 
 import boto3  # type: ignore
 
-from awsxenos.finding import Findings, Resources, Service
+from awsxenos.finding import Accounts, Findings, Resources, Service
 
 """IAM Roles trust policies"""
 
 
 class IAM(Service):
 
     def fetch(  # type: ignore
         self,
-        accounts: DefaultDict[str, Set],
+        accounts: Accounts,
         exclude_service: Optional[bool] = True,
         exclude_aws: Optional[bool] = True,
     ) -> Findings:
         return super().collate(accounts, self.get_role_policies(exclude_service, exclude_aws))
 
     def get_role_policies(
         self, exclude_service: Optional[bool] = True, exclude_aws: Optional[bool] = True
```

### Comparing `awsxenos-0.3.0/awsxenos/services/lambda.py` & `awsxenos-0.4.0/awsxenos/services/lambda.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import json
-from typing import DefaultDict, Set
 
 import boto3  # type: ignore
 from botocore.exceptions import ClientError  # type: ignore
 
-from awsxenos.finding import Findings, Resources, Service
+from awsxenos.finding import Accounts, Findings, Resources, Service
 
 """Lambda Resource Policies"""
 
 
 class LambdaResource(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set]) -> Findings:  # type: ignore
+    def fetch(self, accounts: Accounts) -> Findings:  # type: ignore
         return super().collate(accounts, self.get_lambda_policies())
 
     def get_lambda_policies(self) -> Resources:
         lambdas = Resources()
         lam = boto3.client("lambda")
         paginator = lam.get_paginator("list_functions")
         for lam_resp in paginator.paginate():
             if "Functions" not in lam_resp:
                 continue
             for func in lam_resp["Functions"]:
                 try:
                     lambdas[func["FunctionArn"]] = json.loads(
                         lam.get_policy(FunctionName=func["FunctionName"])["Policy"]
                     )
+
                 except ClientError as err:
-                    lambdas[func["FunctionArn"]] = {
-                        "Version": "2012-10-17",
-                        "Statement": [
-                            {
-                                "Sid": f"{err}",
-                                "Effect": "Allow",
-                                "Principal": {"AWS": ["arn:aws:iam::111122223333:root"]},
-                                "Action": ["lambda:*"],
-                                "Resource": f'{func["FunctionArn"]}',
-                            }
-                        ],
-                    }
+                    if err.response["Error"]["Code"] == "ResourceNotFoundException":
+                        continue  # empty policy
+                    else:
+                        lambdas[func["FunctionArn"]] = {
+                            "Version": "2012-10-17",
+                            "Statement": [
+                                {
+                                    "Sid": f"{err}",
+                                    "Effect": "Allow",
+                                    "Principal": {"AWS": ["arn:aws:iam::111122223333:root"]},
+                                    "Action": ["lambda:*"],
+                                    "Resource": f'{func["FunctionArn"]}',
+                                }
+                            ],
+                        }
+
         return lambdas
```

### Comparing `awsxenos-0.3.0/awsxenos/services/s3.py` & `awsxenos-0.4.0/awsxenos/services/s3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
-from typing import Any, DefaultDict, Dict, Set
+from typing import Any, Dict
 
 import boto3  # type: ignore
 from botocore.client import ClientError  # type: ignore
 
-from awsxenos.finding import Finding, Findings, Resources, Service
+from awsxenos.finding import Accounts, Finding, Findings, Resources, Service
 
 """S3 Buckets Resource Policy """
 
 
 class S3(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set]) -> Findings:  # type: ignore
+    def fetch(self, accounts: Accounts) -> Findings:  # type: ignore
         self._buckets = self.list_account_buckets()
         self.policies = self.get_bucket_policies()
         return super().collate(accounts, self.policies)
 
     def list_account_buckets(self) -> Dict[str, Dict[Any, Any]]:
         s3 = boto3.client("s3")
         return s3.list_buckets()
@@ -37,69 +37,68 @@
                 if e.response["Error"]["Code"] == "AccessDenied":
                     bucket_policies[bucket_arn] = {
                         "Version": "2012-10-17",
                         "Statement": [
                             {
                                 "Sid": "AccessDeniedOnResource",
                                 "Effect": "Allow",
-                                "Principal": {"AWS": ["arn:aws:iam::111122223333:root"]},
+                                "Principal": {"AWS": "*"},
                                 "Action": ["s3:*"],
                                 "Resource": f"{bucket_arn}",
                             }
                         ],
                     }
                     continue
                 elif e.response["Error"]["Code"] == "NoSuchBucketPolicy":
+                    continue
+                else:
                     bucket_policies[bucket_arn] = {
                         "Version": "2012-10-17",
                         "Statement": [
                             {
-                                "Sid": "NoSuchBucketPolicy",
+                                "Sid": "Exception",
                                 "Effect": "Allow",
-                                "Principal": {},
+                                "Principal": {"AWS": "*"},
                                 "Action": ["s3:*"],
                                 "Resource": f"{bucket_arn}",
                             }
                         ],
                     }
-                else:
-                    print(e)
-                    continue
         return bucket_policies
 
 
 """S3 Buckets ACLs"""
 
 
 class S3ACL(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set]) -> Findings:  # type: ignore
+    def fetch(self, accounts: Accounts) -> Findings:  # type: ignore
         self._buckets = self.list_account_buckets()
         self.policies = self.get_acls()
         return self.custom_collate(accounts, self.policies)
 
     def list_account_buckets(self) -> Dict[str, Dict[Any, Any]]:
         s3 = boto3.client("s3")
         return s3.list_buckets()
 
-    def custom_collate(self, accounts: DefaultDict[str, Set], resources: Resources) -> Findings:
+    def custom_collate(self, accounts: Accounts, resources: Resources) -> Findings:
         """Combine all accounts with all the acls to classify findings
 
         Args:
             accounts (DefaultDict[str, Set]): [description]
             resources (DefaultDict[str, List[Dict[Any, Any]]]): [description]
 
         Returns:
             DefaultDict[str, Accounts]: [description]
         """
         findings = Findings()
         for resource, grants in resources.items():
             for grant in grants:
                 if grant["Grantee"]["ID"] == self._buckets["Owner"]["ID"]:
-                    continue  # Don't add if the ACL is of the same account
+                    continue
                 elif grant["Grantee"]["ID"] in accounts["known_accounts"]:
                     findings[resource].known_accounts.append(
                         Finding(principal=grant["Grantee"]["ID"], external_id=True)
                     )
                 elif grant["Grantee"]["ID"] in accounts["org_accounts"]:
                     findings[resource].org_accounts.append(Finding(principal=grant["Grantee"]["ID"], external_id=True))
                 else:
@@ -121,33 +120,68 @@
                     bucket_acls[bucket_arn] = [
                         {
                             "Grantee": {"DisplayName": "AccessDenied", "ID": "AccessDenied", "Type": "CanonicalUser"},
                             "Permission": "FULL_CONTROL",
                         }
                     ]
                 else:
-                    print(e)
-                    continue
+                    bucket_acls[bucket_arn] = [
+                        {
+                            "Grantee": {"DisplayName": "Exception", "ID": "Exception", "Type": "CanonicalUser"},
+                            "Permission": "FULL_CONTROL",
+                        }
+                    ]
         return bucket_acls
 
 
 """S3 Glacier Vault Policies"""
 
 
 class S3Glacier(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set]) -> Findings:  # type: ignore
+    def fetch(self, accounts: Accounts) -> Findings:  # type: ignore
         return super().collate(accounts, self.get_vault_policies())
 
     def get_vault_policies(self) -> Resources:
         vaults = Resources()
         glacier = boto3.client("glacier")
         paginator = glacier.get_paginator("list_vaults")
         glacier_iterator = paginator.paginate()
         for glacier_resp in glacier_iterator:
             if "VaultList" not in glacier_resp:
                 continue
             for vault in glacier_resp["VaultList"]:
-                vaults[vault["VaultARN"]] = json.loads(
-                    glacier.get_vault_access_policy(vaultName=vault["VaultName"])["policy"]["Policy"]
-                )
+                try:
+                    vaults[vault["VaultARN"]] = json.loads(
+                        glacier.get_vault_access_policy(vaultName=vault["VaultName"])["policy"]["Policy"]
+                    )
+                except ClientError as e:
+                    if e.response["Error"]["Code"] == "AccessDenied":
+                        vaults[vault["VaultARN"]] = {
+                            "Version": "2012-10-17",
+                            "Statement": [
+                                {
+                                    "Sid": "AccessDeniedOnResource",
+                                    "Effect": "Allow",
+                                    "Principal": {"AWS": "*"},
+                                    "Action": ["glacier:*"],
+                                    "Resource": f'{vault["VaultARN"]}',
+                                }
+                            ],
+                        }
+                        continue
+                    elif e.response["Error"]["Code"] == "NoSuchBucketPolicy":
+                        continue
+                    else:
+                        vaults[vault["VaultARN"]] = {
+                            "Version": "2012-10-17",
+                            "Statement": [
+                                {
+                                    "Sid": "Exception",
+                                    "Effect": "Allow",
+                                    "Principal": {"AWS": "*"},
+                                    "Action": ["glacier:*"],
+                                    "Resource": f'{vault["VaultARN"]}',
+                                }
+                            ],
+                        }
         return vaults
```

### Comparing `awsxenos-0.3.0/awsxenos/services/secretsmanager.py` & `awsxenos-0.4.0/awsxenos/services/secretsmanager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
-from typing import DefaultDict, Set
 
 import boto3  # type: ignore
 
-from awsxenos.finding import Findings, Resources, Service
+from awsxenos.finding import Accounts, Findings, Resources, Service
 
 """Secrets Manager Secrets Resource Policies"""
 
 
 class SecretsManager(Service):
 
-    def fetch(self, accounts: DefaultDict[str, Set]) -> Findings:  # type: ignore
+    def fetch(self, accounts: Accounts) -> Findings:  # type: ignore
         return super().collate(accounts, self.get_secret_policies())
 
     def get_secret_policies(self) -> Resources:
         """Get a dictionary of secrets and their policies from the AWS Account
 
         Args:
 
@@ -25,10 +24,25 @@
         sm = boto3.client("secretsmanager")
         paginator = sm.get_paginator("list_secrets")
         sm_iterator = paginator.paginate()
         for sm_resp in sm_iterator:
             if "SecretList" not in sm_resp:
                 continue
             for secret in sm_resp["SecretList"]:
-                secrets[secret["ARN"]] = json.loads(sm.get_resource_policy(SecretId=secret["ARN"])["ResourcePolicy"])
-
+                try:
+                    secrets[secret["ARN"]] = json.loads(
+                        sm.get_resource_policy(SecretId=secret["ARN"])["ResourcePolicy"]
+                    )
+                except Exception as err:
+                    secrets[secret["ARN"]] = {
+                        "Version": "2012-10-17",
+                        "Statement": [
+                            {
+                                "Sid": "Exception",
+                                "Effect": "Allow",
+                                "Principal": {"AWS": "*"},
+                                "Action": ["secretsmanager:*"],
+                                "Resource": "*",
+                            }
+                        ],
+                    }
         return secrets
```

### Comparing `awsxenos-0.3.0/awsxenos/services/sqs.py` & `awsxenos-0.4.0/awsxenos/services/sqs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import json
-from typing import DefaultDict, Optional, Set
 
 import boto3  # type: ignore
 
-from awsxenos.finding import Findings, Resources, Service
+from awsxenos.finding import Accounts, Findings, Resources, Service
 
 """SQS Access/Resource Policy"""
 
 
 class SQS(Service):
 
     def fetch(  # type: ignore
         self,
-        accounts: DefaultDict[str, Set],
-        exclude_service: Optional[bool] = True,
-        exclude_aws: Optional[bool] = True,
+        accounts: Accounts,
     ) -> Findings:
         return super().collate(accounts, self.get_sqs_policies())
 
     def get_sqs_policies(self) -> Resources:
         queues = Resources()
         sqs = boto3.client("sqs")
         paginator = sqs.get_paginator("list_queues")
         for sqs_resp in paginator.paginate():
             if "QueueUrls" not in sqs_resp:
                 continue
             for queue in sqs_resp["QueueUrls"]:
-                queues[queue] = json.loads(
-                    sqs.get_queue_attributes(QueueUrl=queue, AttributeNames=["Policy"])["Attributes"]["Policy"]
-                )
+                try:
+                    queues[queue] = json.loads(
+                        sqs.get_queue_attributes(QueueUrl=queue, AttributeNames=["Policy"])["Attributes"]["Policy"]
+                    )
+                except Exception as err:
+                    queues[queue] = {
+                        "Version": "2012-10-17",
+                        "Statement": [
+                            {
+                                "Sid": f"{err}",
+                                "Effect": "Allow",
+                                "Principal": {"AWS": ["arn:aws:iam::111122223333:root"]},
+                                "Action": ["sqs:*"],
+                                "Resource": "*",
+                            }
+                        ],
+                    }
 
         return queues
```

### Comparing `awsxenos-0.3.0/awsxenos/template.html` & `awsxenos-0.4.0/awsxenos/template.html`

 * *Files identical despite different names*

### Comparing `awsxenos-0.3.0/setup.py` & `awsxenos-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 setup(
     name="AWSXenos",
-    version="0.3.0",
+    version="0.4.0",
     author="Costas Kourmpoglou",
     author_email="costas.kourmpoglou@airwalkconsulting.com",
     license="MIT",
     description="Scan and classify cross-account roles and resources in your AWS Account",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AirWalk-Digital/AWSXenos",
```

### Comparing `awsxenos-0.3.0/tests/fixtures.py` & `awsxenos-0.4.0/tests/fixtures.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,29 +91,47 @@
                     },
                     "MaxSessionDuration": 3600,
                 },
                 {
                     "Path": "/",
                     "RoleName": "ExternalUserWithinOrg",
                     "RoleId": "AROA02I634LQK4QC3IIWF",
-                    "Arn": "arn:aws:iam::000000000000:user/ExternalUserWithinOrg",
+                    "Arn": "arn:aws:iam::000000000000:user/ExternalUserWithinOrgButOrgIdCondition",
                     "CreateDate": datetime.datetime(2021, 4, 8, 14, 1, 34),
                     "AssumeRolePolicyDocument": {
                         "Version": "2012-10-17",
                         "Statement": [
                             {
                                 "Effect": "Allow",
                                 "Principal": {"AWS" : "arn:aws:iam::000000000002:root"},
                                 "Action": "sts:AssumeRoleWithSAML",
                                 "Condition": {"StringEquals": {"aws:PrincipalOrgID": "o-290nd8mdls"}},
                             }
                         ],
                     },
                     "MaxSessionDuration": 3600,
                 },
+                                {
+                    "Path": "/",
+                    "RoleName": "ExternalUserWithinOrg",
+                    "RoleId": "AROA02I634LQK4QC3IIWF",
+                    "Arn": "arn:aws:iam::000000000000:user/ExternalUserWithinOrg",
+                    "CreateDate": datetime.datetime(2021, 4, 8, 14, 1, 34),
+                    "AssumeRolePolicyDocument": {
+                        "Version": "2012-10-17",
+                        "Statement": [
+                            {
+                                "Effect": "Allow",
+                                "Principal": {"AWS" : "arn:aws:iam::000000000002:root"},
+                                "Action": "sts:AssumeRoleWithSAML"
+                            }
+                        ],
+                    },
+                    "MaxSessionDuration": 3600,
+                },
                 {
                     "Path": "/",
                     "RoleName": "test-sdlc-notifier-dev-eu-west-1-lambdaRole",
                     "RoleId": "AROA49I634LQK4QC3ISLR",
                     "Arn": "arn:aws:iam::000000000000:role/test-sdlc-notifier-dev-eu-west-1-lambdaRole",
                     "CreateDate": datetime.datetime(2021, 5, 11, 8, 59, 9),
                     "AssumeRolePolicyDocument": {
@@ -132,15 +150,16 @@
             ]
         }
         roles = {role["Arn"]: role["AssumeRolePolicyDocument"] for role in boto_list_roles["Roles"]}
         return roles
 
     @staticmethod
     def mock_get_accounts():
-        accounts = defaultdict(set)
+        #accounts = defaultdict(set)
+        accounts = Accounts()
         boto_list_orgs = {
             "Accounts": [
                 {
                     "Id": "000000000000",
                     "Arn": "arn:aws:organizations::000000000000:account/o-7s9fjxxxxn/000000000000",
                     "Email": "info@airwalkconsulting.com",
                     "Name": "AirWalk Sandbox",
@@ -155,27 +174,28 @@
                     "Name": "AirWalk Sandbox1",
                     "Status": "ACTIVE",
                     "JoinedMethod": "CREATED",
                     "JoinedTimestamp": datetime.datetime(2019, 4, 29, 16, 7, 32, 155000),
                 },
             ]
         }
-        accounts["org_accounts"] = set([account["Id"] for account in boto_list_orgs["Accounts"]])
-        accounts["org_accounts"].add("xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
-        accounts["known_accounts"] = set(["000000000001"])
+        accounts.org_accounts = set([account["Id"] for account in boto_list_orgs["Accounts"]]) # type: ignore
+        accounts.org_accounts.add("xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
+        accounts.known_accounts = set(["000000000001"]) # type: ignore
+        accounts.org_id = "o-xxxxxxxx" # type: ignore
         return accounts
 
     @staticmethod
     def mock_list_s3_buckets():
         return {
             "Buckets": [
-                {"Name": "examplebucket", "CreationDate": datetime.datetime(2021, 3, 29, 20, 17, 11)},
-                {"Name": "anotherexample", "CreationDate": datetime.datetime(2021, 5, 11, 8, 58, 53)},
+                {"Name": "examplebucketwithpolicy", "CreationDate": datetime.datetime(2021, 3, 29, 20, 17, 11)},
+                {"Name": "examplebucketexternalaccount", "CreationDate": datetime.datetime(2021, 5, 11, 8, 58, 53)},
                 {
-                    "Name": "aws-athena-query-results-examplebucket",
+                    "Name": "examplebucketsameaccount",
                     "CreationDate": datetime.datetime(2021, 8, 10, 10, 12, 28),
                 },
             ],
             "Owner": {"DisplayName": "exampleaccount", "ID": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"},
         }
 
     @staticmethod
@@ -193,23 +213,33 @@
                 ],
             }
         }
 
     @staticmethod
     def mock_get_bucket_acl():
         return {
-            "arn:aws:s3:::examplebucket": [
+            "arn:aws:s3:::examplebucketexternalaccount": [
                 {
                     "Grantee": {
                         "DisplayName": "exampleexternalaccount",
                         "ID": "yyyyyyyyyyyyyyyyyyyyyyyyyyyyyyy",
                         "Type": "CanonicalUser",
                     },
                     "Permission": "FULL_CONTROL",
                 }
+            ],
+                "arn:aws:s3:::examplebucketsameaccount": [
+                {
+                    "Grantee": {
+                        "DisplayName": "examplesameaccount",
+                        "ID": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
+                        "Type": "CanonicalUser",
+                    },
+                    "Permission": "FULL_CONTROL",
+                }
             ]
         }
 
     @staticmethod
     def mock_known_accounts():
         known_accounts = defaultdict(dict)
         accounts = Fixtures.mock_get_accounts()
```

### Comparing `awsxenos-0.3.0/tests/test_report.py` & `awsxenos-0.4.0/tests/test_report.py`

 * *Files identical despite different names*

