# Comparing `tmp/signate-0.9.9.tar.gz` & `tmp/signate-9.9.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signate-0.9.9.tar", last modified: Tue Dec 14 00:36:25 2021, max compression
+gzip compressed data, was "signate-9.9.10.tar", last modified: Mon Mar  6 02:06:26 2023, max compression
```

## Comparing `signate-0.9.9.tar` & `signate-9.9.10.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 00:36:25.565352 signate-0.9.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-14 00:36:12.000000 signate-0.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7599 2021-12-14 00:36:25.565352 signate-0.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7297 2021-12-14 00:36:12.000000 signate-0.9.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      377 2021-12-14 00:36:25.565352 signate-0.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2021-12-14 00:36:12.000000 signate-0.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 00:36:25.565352 signate-0.9.9/signate/
--rw-r--r--   0 runner    (1001) docker     (121)      635 2021-12-14 00:36:12.000000 signate-0.9.9/signate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7390 2021-12-14 00:36:12.000000 signate-0.9.9/signate/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2021-12-14 00:36:12.000000 signate-0.9.9/signate/info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 00:36:25.565352 signate-0.9.9/signate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7599 2021-12-14 00:36:25.000000 signate-0.9.9/signate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      785 2021-12-14 00:36:25.000000 signate-0.9.9/signate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 00:36:25.000000 signate-0.9.9/signate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-12-14 00:36:25.000000 signate-0.9.9/signate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-12-14 00:36:25.000000 signate-0.9.9/signate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-14 00:36:25.000000 signate-0.9.9/signate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 00:36:25.565352 signate-0.9.9/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (121)      937 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 00:36:25.565352 signate-0.9.9/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28562 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    24939 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     7978 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 00:36:25.565352 signate-0.9.9/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5829 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/competition.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/competitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5320 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     2417 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/downloads.py
--rw-r--r--   0 runner    (1001) docker     (121)     5022 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/success.py
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/models/token.py
--rw-r--r--   0 runner    (1001) docker     (121)    13112 2021-12-14 00:36:12.000000 signate-0.9.9/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:06:26.740214 signate-9.9.10/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-06 02:06:16.000000 signate-9.9.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-03-06 02:06:26.740214 signate-9.9.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-03-06 02:06:16.000000 signate-9.9.10/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-06 02:06:26.740214 signate-9.9.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-03-06 02:06:16.000000 signate-9.9.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:06:26.740214 signate-9.9.10/signate/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-06 02:06:16.000000 signate-9.9.10/signate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-03-06 02:06:16.000000 signate-9.9.10/signate/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-06 02:06:16.000000 signate-9.9.10/signate/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:06:26.740214 signate-9.9.10/signate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-03-06 02:06:26.000000 signate-9.9.10/signate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-06 02:06:26.000000 signate-9.9.10/signate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 02:06:26.000000 signate-9.9.10/signate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 02:06:26.000000 signate-9.9.10/signate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-06 02:06:26.000000 signate-9.9.10/signate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-06 02:06:26.000000 signate-9.9.10/signate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:06:26.740214 signate-9.9.10/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:06:26.740214 signate-9.9.10/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28562 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24939 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 02:06:26.740214 signate-9.9.10/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/competition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/competitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/success.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2023-03-06 02:06:16.000000 signate-9.9.10/swagger_client/rest.py
```

### Comparing `signate-0.9.9/LICENSE` & `signate-9.9.10/LICENSE`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/PKG-INFO` & `signate-9.9.10/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: signate
-Version: 0.9.9
-Summary: SIGNATE CLI
-Home-page: https://github.com/signatelab/signate-cli
-Author: SIGNATE Inc.
-License: Apache 2.0
-Keywords: signate,signate-cli
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![pytest](https://github.com/signatelab/signate-cli/workflows/pytest/badge.svg) [![PyPI version](https://badge.fury.io/py/signate.svg)](https://badge.fury.io/py/signate)
 
 # **SIGNATE CLI**
 [SIGNATE](https://signate.jp) の公式APIコマンドラインインターフェイス(以下：SIGNATE CLI)です。  
 SIGNATEはData Science Competitionのご提供を始めとした、データサイエンティストの皆様のための統合プラットフォームです。
 
 **※SIGNATE CLIの動作にはPython3.6 以降の環境が必要です。**  
@@ -30,15 +17,18 @@
 ```
 
 インストール後、以下の手順を実施ください。
 
  1. [SIGNATE](https://signate.jp) でアカウント登録  
  2. アカウント登録後、[アカウント設定](https://signate.jp/account_settings) 画面の "API Token" の "作成" をクリック  
  3. "新規作成" をクリックしてAPI Token(``signate.json``)を取得  
- 4. 取得したAPI Tokenを ``~/.signate``直下に配置   
+ 4. ~/.signateを作成  
+ ＊ ~/ はホームディレクトリを指します。ホームディレクトリ直下に .signate を作成してください。  
+ ＊ . から始まるフォルダは隠しフォルダです。隠しフォルダを表示した状態でご確認ください。  
+ 5. 取得したAPI Tokenを ``~/.signate``直下に配置   
  ＊ SIGNATE CLI 上でも API Token は取得できます。詳しくは「利用方法」⑤をご参照ください。  
  ＊ SNS で会員登録した場合は[アカウント設定](https://signate.jp/account_settings) 画面でのみ API Token を取得可能です。
 
 以下のコマンドでヘルプが表示されましたら利用準備完了です。
 
 ```
 $ signate --help
@@ -178,9 +168,7 @@
 ```
 You have not filled in user infomation to join the competition. Go to https://signate.jp/profile.
 ```
 のメッセージが表示された場合は[SIGNATE](https://signate.jp)にアクセスいただき、プロフィールのご入力をお願いいたします。
 
 # **ライセンス**
 SIGNATE CLIは[Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0). を適用しております。
-
-
```

### Comparing `signate-0.9.9/README.md` & `signate-9.9.10/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: signate
+Version: 9.9.10
+Summary: SIGNATE CLI
+Home-page: https://github.com/signatelab/signate-cli
+Author: SIGNATE Inc.
+License: Apache 2.0
+Keywords: signate,signate-cli
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![pytest](https://github.com/signatelab/signate-cli/workflows/pytest/badge.svg) [![PyPI version](https://badge.fury.io/py/signate.svg)](https://badge.fury.io/py/signate)
 
 # **SIGNATE CLI**
 [SIGNATE](https://signate.jp) の公式APIコマンドラインインターフェイス(以下：SIGNATE CLI)です。  
 SIGNATEはData Science Competitionのご提供を始めとした、データサイエンティストの皆様のための統合プラットフォームです。
 
 **※SIGNATE CLIの動作にはPython3.6 以降の環境が必要です。**  
@@ -17,15 +29,18 @@
 ```
 
 インストール後、以下の手順を実施ください。
 
  1. [SIGNATE](https://signate.jp) でアカウント登録  
  2. アカウント登録後、[アカウント設定](https://signate.jp/account_settings) 画面の "API Token" の "作成" をクリック  
  3. "新規作成" をクリックしてAPI Token(``signate.json``)を取得  
- 4. 取得したAPI Tokenを ``~/.signate``直下に配置   
+ 4. ~/.signateを作成  
+ ＊ ~/ はホームディレクトリを指します。ホームディレクトリ直下に .signate を作成してください。  
+ ＊ . から始まるフォルダは隠しフォルダです。隠しフォルダを表示した状態でご確認ください。  
+ 5. 取得したAPI Tokenを ``~/.signate``直下に配置   
  ＊ SIGNATE CLI 上でも API Token は取得できます。詳しくは「利用方法」⑤をご参照ください。  
  ＊ SNS で会員登録した場合は[アカウント設定](https://signate.jp/account_settings) 画面でのみ API Token を取得可能です。
 
 以下のコマンドでヘルプが表示されましたら利用準備完了です。
 
 ```
 $ signate --help
```

### Comparing `signate-0.9.9/setup.py` & `signate-9.9.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2018 - 2020 SIGNATE Inc.
+# Copyright 2018 - 2023 SIGNATE Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `signate-0.9.9/signate/__init__.py` & `signate-9.9.10/signate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2018 - 2020 SIGNATE Inc.
+# Copyright 2018 - 2023 SIGNATE Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `signate-0.9.9/signate/cli.py` & `signate-9.9.10/signate/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/python
 #
-# Copyright 2018 - 2020 SIGNATE Inc.
+# Copyright 2018 - 2023 SIGNATE Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `signate-0.9.9/signate/info.py` & `signate-9.9.10/signate/info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/python
 #
-# Copyright 2018 - 2020 SIGNATE Inc.
+# Copyright 2018 - 2023 SIGNATE Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 NAME = 'SIGNATE CLI'
-VERSION = '0.9.9'
+VERSION = '9.9.10'
```

### Comparing `signate-0.9.9/signate.egg-info/PKG-INFO` & `signate-9.9.10/signate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: signate
-Version: 0.9.9
+Version: 9.9.10
 Summary: SIGNATE CLI
 Home-page: https://github.com/signatelab/signate-cli
 Author: SIGNATE Inc.
 License: Apache 2.0
 Keywords: signate,signate-cli
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![pytest](https://github.com/signatelab/signate-cli/workflows/pytest/badge.svg) [![PyPI version](https://badge.fury.io/py/signate.svg)](https://badge.fury.io/py/signate)
 
 # **SIGNATE CLI**
@@ -30,15 +29,18 @@
 ```
 
 インストール後、以下の手順を実施ください。
 
  1. [SIGNATE](https://signate.jp) でアカウント登録  
  2. アカウント登録後、[アカウント設定](https://signate.jp/account_settings) 画面の "API Token" の "作成" をクリック  
  3. "新規作成" をクリックしてAPI Token(``signate.json``)を取得  
- 4. 取得したAPI Tokenを ``~/.signate``直下に配置   
+ 4. ~/.signateを作成  
+ ＊ ~/ はホームディレクトリを指します。ホームディレクトリ直下に .signate を作成してください。  
+ ＊ . から始まるフォルダは隠しフォルダです。隠しフォルダを表示した状態でご確認ください。  
+ 5. 取得したAPI Tokenを ``~/.signate``直下に配置   
  ＊ SIGNATE CLI 上でも API Token は取得できます。詳しくは「利用方法」⑤をご参照ください。  
  ＊ SNS で会員登録した場合は[アカウント設定](https://signate.jp/account_settings) 画面でのみ API Token を取得可能です。
 
 以下のコマンドでヘルプが表示されましたら利用準備完了です。
 
 ```
 $ signate --help
@@ -178,9 +180,7 @@
 ```
 You have not filled in user infomation to join the competition. Go to https://signate.jp/profile.
 ```
 のメッセージが表示された場合は[SIGNATE](https://signate.jp)にアクセスいただき、プロフィールのご入力をお願いいたします。
 
 # **ライセンス**
 SIGNATE CLIは[Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0). を適用しております。
-
-
```

### Comparing `signate-0.9.9/signate.egg-info/SOURCES.txt` & `signate-9.9.10/signate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/__init__.py` & `signate-9.9.10/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/api/default_api.py` & `signate-9.9.10/swagger_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/api_client.py` & `signate-9.9.10/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/configuration.py` & `signate-9.9.10/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/__init__.py` & `signate-9.9.10/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/competition.py` & `signate-9.9.10/swagger_client/models/competition.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/competitions.py` & `signate-9.9.10/swagger_client/models/competitions.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/download.py` & `signate-9.9.10/swagger_client/models/download.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/downloads.py` & `signate-9.9.10/swagger_client/models/downloads.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/error.py` & `signate-9.9.10/swagger_client/models/error.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/file.py` & `signate-9.9.10/swagger_client/models/file.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/files.py` & `signate-9.9.10/swagger_client/models/files.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/success.py` & `signate-9.9.10/swagger_client/models/success.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/models/token.py` & `signate-9.9.10/swagger_client/models/token.py`

 * *Files identical despite different names*

### Comparing `signate-0.9.9/swagger_client/rest.py` & `signate-9.9.10/swagger_client/rest.py`

 * *Files identical despite different names*

