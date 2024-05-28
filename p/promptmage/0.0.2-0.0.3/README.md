# Comparing `tmp/promptmage-0.0.2.tar.gz` & `tmp/promptmage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptmage-0.0.2.tar", max compression
+gzip compressed data, was "promptmage-0.0.3.tar", max compression
```

## Comparing `promptmage-0.0.2.tar` & `promptmage-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,36 @@
--rw-r--r--   0        0        0     1071 2024-05-01 10:16:57.039782 promptmage-0.0.2/LICENSE
--rw-r--r--   0        0        0     2593 2024-05-16 05:43:40.375705 promptmage-0.0.2/README.md
--rw-r--r--   0        0        0       56 2024-05-16 05:39:40.593438 promptmage-0.0.2/promptmage/__init__.py
--rw-r--r--   0        0        0     1437 2024-05-16 05:38:09.148454 promptmage-0.0.2/promptmage/cli.py
--rw-r--r--   0        0        0     4648 2024-05-16 05:39:07.242600 promptmage-0.0.2/promptmage/mage.py
--rw-r--r--   0        0        0      156 2024-05-01 14:22:05.697936 promptmage-0.0.2/promptmage/prompt.py
--rw-r--r--   0        0        0        0 2024-05-01 14:14:30.462689 promptmage-0.0.2/promptmage/prompt_store.py
--rw-r--r--   0        0        0    49892 2024-05-08 10:56:54.337714 promptmage-0.0.2/promptmage/static/apple-touch-icon.png
--rw-r--r--   0        0        0      517 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/asset-manifest.json
--rw-r--r--   0        0        0      981 2024-05-08 10:56:54.337714 promptmage-0.0.2/promptmage/static/favicon-16x16.png
--rw-r--r--   0        0        0     3042 2024-05-08 10:56:54.337714 promptmage-0.0.2/promptmage/static/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2024-05-08 10:56:54.337714 promptmage-0.0.2/promptmage/static/favicon.ico
--rw-r--r--   0        0        0      675 2024-05-08 10:57:02.381641 promptmage-0.0.2/promptmage/static/index.html
--rw-r--r--   0        0        0    55404 2024-05-08 10:56:54.341714 promptmage-0.0.2/promptmage/static/logo192.png
--rw-r--r--   0        0        0   263823 2024-05-08 10:56:54.341714 promptmage-0.0.2/promptmage/static/logo512.png
--rw-r--r--   0        0        0      501 2024-05-08 10:56:54.341714 promptmage-0.0.2/promptmage/static/manifest.json
--rw-r--r--   0        0        0       67 2024-05-08 10:56:54.341714 promptmage-0.0.2/promptmage/static/robots.txt
--rw-r--r--   0        0        0     1198 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/static/css/main.97eee1a4.css
--rw-r--r--   0        0        0     2271 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/static/css/main.97eee1a4.css.map
--rw-r--r--   0        0        0     4536 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/static/js/453.3f617a88.chunk.js
--rw-r--r--   0        0        0    10597 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/static/js/453.3f617a88.chunk.js.map
--rw-r--r--   0        0        0   174673 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/static/js/main.b5cd8004.js
--rw-r--r--   0        0        0      971 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/static/js/main.b5cd8004.js.LICENSE.txt
--rw-r--r--   0        0        0   513090 2024-05-08 10:57:02.385640 promptmage-0.0.2/promptmage/static/static/js/main.b5cd8004.js.map
--rw-r--r--   0        0        0      608 2024-05-16 05:39:28.365872 promptmage-0.0.2/promptmage/utils.py
--rw-r--r--   0        0        0      816 2024-05-16 05:46:50.806998 promptmage-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 promptmage-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-01 10:16:57.039782 promptmage-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2783 2024-05-16 07:40:35.563388 promptmage-0.0.3/README.md
+-rw-r--r--   0        0        0      134 2024-05-20 10:17:26.582761 promptmage-0.0.3/promptmage/__init__.py
+-rw-r--r--   0        0        0     5131 2024-05-28 08:47:13.647744 promptmage-0.0.3/promptmage/api.py
+-rw-r--r--   0        0        0     1093 2024-05-20 18:51:34.244504 promptmage-0.0.3/promptmage/cli.py
+-rw-r--r--   0        0        0      245 2024-05-22 15:54:46.025235 promptmage-0.0.3/promptmage/exceptions.py
+-rw-r--r--   0        0        0       76 2024-05-20 18:32:01.442590 promptmage-0.0.3/promptmage/frontend/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 10:18:02.735560 promptmage-0.0.3/promptmage/frontend/components/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-28 13:15:16.820722 promptmage-0.0.3/promptmage/frontend/components/main_runner.py
+-rw-r--r--   0        0        0      224 2024-05-28 11:29:41.779569 promptmage-0.0.3/promptmage/frontend/components/menu.py
+-rw-r--r--   0        0        0     1948 2024-05-28 15:41:20.413814 promptmage-0.0.3/promptmage/frontend/components/prompts_page.py
+-rw-r--r--   0        0        0      821 2024-05-28 12:27:52.923085 promptmage-0.0.3/promptmage/frontend/components/runs_page.py
+-rw-r--r--   0        0        0     4812 2024-05-28 13:55:48.614188 promptmage-0.0.3/promptmage/frontend/components/step_runner.py
+-rw-r--r--   0        0        0      608 2024-05-28 14:08:46.822693 promptmage-0.0.3/promptmage/frontend/components/theme.py
+-rw-r--r--   0        0        0     2163 2024-05-28 15:39:14.780957 promptmage-0.0.3/promptmage/frontend/frontend.py
+-rw-r--r--   0        0        0     8628 2024-05-28 15:32:02.893219 promptmage-0.0.3/promptmage/mage.py
+-rw-r--r--   0        0        0     1713 2024-05-28 15:24:22.850110 promptmage-0.0.3/promptmage/prompt.py
+-rw-r--r--   0        0        0     1670 2024-05-28 15:18:45.093533 promptmage-0.0.3/promptmage/run_data.py
+-rw-r--r--   0        0        0    41939 2024-05-21 04:38:10.000000 promptmage-0.0.3/promptmage/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0   145613 2024-05-21 04:38:10.000000 promptmage-0.0.3/promptmage/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0    37714 2024-05-21 04:38:10.000000 promptmage-0.0.3/promptmage/static/apple-touch-icon.png
+-rw-r--r--   0        0        0      988 2024-05-21 04:38:10.000000 promptmage-0.0.3/promptmage/static/favicon-16x16.png
+-rw-r--r--   0        0        0     2753 2024-05-21 04:38:10.000000 promptmage-0.0.3/promptmage/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2024-05-21 04:38:10.000000 promptmage-0.0.3/promptmage/static/favicon.ico
+-rw-r--r--   0        0        0   142843 2024-05-16 06:17:33.031012 promptmage-0.0.3/promptmage/static/promptmage-logo.png
+-rw-r--r--   0        0        0      263 2024-05-21 04:38:10.000000 promptmage-0.0.3/promptmage/static/site.webmanifest
+-rw-r--r--   0        0        0      492 2024-05-28 15:16:36.918766 promptmage-0.0.3/promptmage/storage/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-28 12:05:55.802014 promptmage-0.0.3/promptmage/storage/data_store.py
+-rw-r--r--   0        0        0      413 2024-05-18 10:08:47.883389 promptmage-0.0.3/promptmage/storage/file_backend.py
+-rw-r--r--   0        0        0     1583 2024-05-28 15:09:01.558603 promptmage-0.0.3/promptmage/storage/memory_backend.py
+-rw-r--r--   0        0        0     1474 2024-05-22 16:04:52.475434 promptmage-0.0.3/promptmage/storage/prompt_store.py
+-rw-r--r--   0        0        0     5971 2024-05-28 15:27:37.772060 promptmage-0.0.3/promptmage/storage/sqlite_backend.py
+-rw-r--r--   0        0        0      297 2024-05-18 10:08:15.226438 promptmage-0.0.3/promptmage/storage/storage_backend.py
+-rw-r--r--   0        0        0      608 2024-05-16 05:39:28.365872 promptmage-0.0.3/promptmage/utils.py
+-rw-r--r--   0        0        0     1248 2024-05-28 15:49:16.573900 promptmage-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 promptmage-0.0.3/PKG-INFO
```

### Comparing `promptmage-0.0.2/LICENSE` & `promptmage-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptmage-0.0.2/README.md` & `promptmage-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 <br />
 <div align="center">
   <a href="https://github.com/tsterbak/promptmage">
-    <img src="images/flowforge-logo.png" alt="PromptMage-Logo" width="120" height="120">
+    <img src="images/promptmage-logo.png" alt="PromptMage-Logo" width="120" height="120">
   </a>
 
   <h1 align="center">PromptMage</h1>
 
   <p align="center">
     simplifies the process of creating and managing LLM workflows as a self-hosted solution.
   </p>
 </div>
 
 ## About the Project
 
-"PromptMage" is designed to offer an intuitive interface that simplifies the process of creating and managing LLM workflows as a self-hosted solution. It facilitates prompt testing and comparison, and it incorporates version control features to help users track the development of their prompts. Suitable for both small teams and large enterprises, "FlowForge" seeks to improve productivity and foster the practical use of LLM technology.
+"PromptMage" is designed to offer an intuitive interface that simplifies the process of creating and managing LLM workflows as a self-hosted solution. It facilitates prompt testing and comparison, and it incorporates version control features to help users track the development of their prompts. Suitable for both small teams and large enterprises, "PromptMage" seeks to improve productivity and foster the practical use of LLM technology.
 
 The approach with "PromptMage" is to provide a pragmatic solution that bridges the current gap in LLM workflow management. We aim to empower developers, researchers, and organizations by making LLM technology more accessible and manageable, thereby supporting the next wave of AI innovations.
 
+## Philosophy
+- Prompts as first-class citizens
+- Type-hint everything for automatic inference and validation magic
+- build-in, automatically created API with fastAPI for easy integration
 
 ## Getting Started
 
 ### Installation
 
 To install promptmage, run the following command:
```

#### html2text {}

```diff
@@ -3,31 +3,33 @@
                            ************ PPrroommppttMMaaggee ************
 simplifies the process of creating and managing LLM workflows as a self-hosted
                                    solution.
 ## About the Project "PromptMage" is designed to offer an intuitive interface
 that simplifies the process of creating and managing LLM workflows as a self-
 hosted solution. It facilitates prompt testing and comparison, and it
 incorporates version control features to help users track the development of
-their prompts. Suitable for both small teams and large enterprises, "FlowForge"
-seeks to improve productivity and foster the practical use of LLM technology.
-The approach with "PromptMage" is to provide a pragmatic solution that bridges
-the current gap in LLM workflow management. We aim to empower developers,
-researchers, and organizations by making LLM technology more accessible and
-manageable, thereby supporting the next wave of AI innovations. ## Getting
-Started ### Installation To install promptmage, run the following command:
-```bash pip install promptmage ``` ## Usage To use promptmage, run the
-following command: ```bash promptmage cast ``` ## Roadmap Coming soon. ##
-Development To develop PromptMage, check out the [DEVELOPMENT.md]
-(DEVELOPMENT.md) file. ## Contributing Contributing We welcome contributions
-from the community! If you're interested in improving PromptMage, you can
-contribute in the following ways: * **Reporting Bugs**: Submit an issue in our
-repository, providing a detailed description of the problem and steps to
-reproduce it. * **Feature Requests**: Have ideas on how to make FlowForge
-better? We'd love to hear from you! Please submit an issue, detailing your
-suggestions. * **Pull Requests**: Contributions via pull requests are highly
-appreciated. Please ensure your code adheres to the coding standards of the
-project, and submit a pull request with a clear description of your changes. ##
-License This project is licensed under the MIT License - see the [LICENSE.md]
-(LICENSE.md) file for details. ## Contact For any inquiries or further
-information, feel free to reach out at [promptmage@tobiassterbak.com](mailto:
-promptmage@tobiassterbak.com). ## â¤ï¸ Acknowledgements This project was
-supported by_[_i_m_a_g_e_s_/_m_t_l_-_p_o_w_e_r_e_d_-_b_y_._p_n_g_]
+their prompts. Suitable for both small teams and large enterprises,
+"PromptMage" seeks to improve productivity and foster the practical use of LLM
+technology. The approach with "PromptMage" is to provide a pragmatic solution
+that bridges the current gap in LLM workflow management. We aim to empower
+developers, researchers, and organizations by making LLM technology more
+accessible and manageable, thereby supporting the next wave of AI innovations.
+## Philosophy - Prompts as first-class citizens - Type-hint everything for
+automatic inference and validation magic - build-in, automatically created API
+with fastAPI for easy integration ## Getting Started ### Installation To
+install promptmage, run the following command: ```bash pip install promptmage
+``` ## Usage To use promptmage, run the following command: ```bash promptmage
+cast ``` ## Roadmap Coming soon. ## Development To develop PromptMage, check
+out the [DEVELOPMENT.md](DEVELOPMENT.md) file. ## Contributing Contributing We
+welcome contributions from the community! If you're interested in improving
+PromptMage, you can contribute in the following ways: * **Reporting Bugs**:
+Submit an issue in our repository, providing a detailed description of the
+problem and steps to reproduce it. * **Feature Requests**: Have ideas on how to
+make FlowForge better? We'd love to hear from you! Please submit an issue,
+detailing your suggestions. * **Pull Requests**: Contributions via pull
+requests are highly appreciated. Please ensure your code adheres to the coding
+standards of the project, and submit a pull request with a clear description of
+your changes. ## License This project is licensed under the MIT License - see
+the [LICENSE.md](LICENSE.md) file for details. ## Contact For any inquiries or
+further information, feel free to reach out at [promptmage@tobiassterbak.com]
+(mailto:promptmage@tobiassterbak.com). ## â¤ï¸ Acknowledgements This project
+was supported by_[_i_m_a_g_e_s_/_m_t_l_-_p_o_w_e_r_e_d_-_b_y_._p_n_g_]
```

### Comparing `promptmage-0.0.2/promptmage/utils.py` & `promptmage-0.0.3/promptmage/utils.py`

 * *Files identical despite different names*

### Comparing `promptmage-0.0.2/pyproject.toml` & `promptmage-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,40 @@
 [tool.poetry]
 name = "promptmage"
-version = "0.0.2"
+version = "0.0.3"
 description = "\"PromptMage\" is designed to offer an intuitive interface that simplifies the process of creating and managing LLM workflows as a self-hosted solution."
 authors = ["Tobias Sterbak <github@tobiassterbak.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://www.promptmage.io"
+repository = "https://github.comm/tsterbak/promptmage"
+keywords = ["promptmage", "llm", "workflow", "management", "self-hosted", "solution", "ai", "nlp", "prompt"]
+classifiers = [
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Software Development :: Libraries :: Python Modules"
+]
 include = ["promptmage/static"]
-homepage = "https://promptmage.io"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 loguru = "^0.7.2"
 click = "^8.1.7"
-fastapi = "^0.110.3"
 uvicorn = {extras = ["standard"], version = "^0.29.0"}
 setuptools = "^69.5.1"
+nicegui = "^1.4.25"
+fastapi = ">=0.109.1,<0.110.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 ruff = "^0.4.2"
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
+mkdocs = "^1.6.0"
+mkdocs-material = "^9.5.23"
+material-plausible-plugin = "^0.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 promptmage = "promptmage.cli:serve"
```

### Comparing `promptmage-0.0.2/PKG-INFO` & `promptmage-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: promptmage
-Version: 0.0.2
+Version: 0.0.3
 Summary: "PromptMage" is designed to offer an intuitive interface that simplifies the process of creating and managing LLM workflows as a self-hosted solution.
-Home-page: https://promptmage.io
+Home-page: https://www.promptmage.io
 License: MIT
+Keywords: promptmage,llm,workflow,management,self-hosted,solution,ai,nlp,prompt
 Author: Tobias Sterbak
 Author-email: github@tobiassterbak.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: fastapi (>=0.110.3,<0.111.0)
+Requires-Dist: fastapi (>=0.109.1,<0.110.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: nicegui (>=1.4.25,<2.0.0)
 Requires-Dist: setuptools (>=69.5.1,<70.0.0)
 Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
+Project-URL: Repository, https://github.comm/tsterbak/promptmage
 Description-Content-Type: text/markdown
 
 <br />
 <div align="center">
   <a href="https://github.com/tsterbak/promptmage">
-    <img src="images/flowforge-logo.png" alt="PromptMage-Logo" width="120" height="120">
+    <img src="images/promptmage-logo.png" alt="PromptMage-Logo" width="120" height="120">
   </a>
 
   <h1 align="center">PromptMage</h1>
 
   <p align="center">
     simplifies the process of creating and managing LLM workflows as a self-hosted solution.
   </p>
 </div>
 
 ## About the Project
 
-"PromptMage" is designed to offer an intuitive interface that simplifies the process of creating and managing LLM workflows as a self-hosted solution. It facilitates prompt testing and comparison, and it incorporates version control features to help users track the development of their prompts. Suitable for both small teams and large enterprises, "FlowForge" seeks to improve productivity and foster the practical use of LLM technology.
+"PromptMage" is designed to offer an intuitive interface that simplifies the process of creating and managing LLM workflows as a self-hosted solution. It facilitates prompt testing and comparison, and it incorporates version control features to help users track the development of their prompts. Suitable for both small teams and large enterprises, "PromptMage" seeks to improve productivity and foster the practical use of LLM technology.
 
 The approach with "PromptMage" is to provide a pragmatic solution that bridges the current gap in LLM workflow management. We aim to empower developers, researchers, and organizations by making LLM technology more accessible and manageable, thereby supporting the next wave of AI innovations.
 
+## Philosophy
+- Prompts as first-class citizens
+- Type-hint everything for automatic inference and validation magic
+- build-in, automatically created API with fastAPI for easy integration
 
 ## Getting Started
 
 ### Installation
 
 To install promptmage, run the following command:
```

#### html2text {}

```diff
@@ -1,43 +1,49 @@
-Metadata-Version: 2.1 Name: promptmage Version: 0.0.2 Summary: "PromptMage" is
+Metadata-Version: 2.1 Name: promptmage Version: 0.0.3 Summary: "PromptMage" is
 designed to offer an intuitive interface that simplifies the process of
 creating and managing LLM workflows as a self-hosted solution. Home-page:
-https://promptmage.io License: MIT Author: Tobias Sterbak Author-email:
-github@tobiassterbak.com Requires-Python: >=3.11,<4.0 Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
-(>=8.1.7,<9.0.0) Requires-Dist: fastapi (>=0.110.3,<0.111.0) Requires-Dist:
-loguru (>=0.7.2,<0.8.0) Requires-Dist: setuptools (>=69.5.1,<70.0.0) Requires-
-Dist: uvicorn[standard] (>=0.29.0,<0.30.0) Description-Content-Type: text/
-markdown
+https://www.promptmage.io License: MIT Keywords:
+promptmage,llm,workflow,management,self-hosted,solution,ai,nlp,prompt Author:
+Tobias Sterbak Author-email: github@tobiassterbak.com Requires-Python:
+>=3.11,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.11 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: click (>=8.1.7,<9.0.0) Requires-Dist: fastapi
+(>=0.109.1,<0.110.0) Requires-Dist: loguru (>=0.7.2,<0.8.0) Requires-Dist:
+nicegui (>=1.4.25,<2.0.0) Requires-Dist: setuptools (>=69.5.1,<70.0.0)
+Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0) Project-URL: Repository,
+https://github.comm/tsterbak/promptmage Description-Content-Type: text/markdown
                                _[_P_r_o_m_p_t_M_a_g_e_-_L_o_g_o_]
                            ************ PPrroommppttMMaaggee ************
 simplifies the process of creating and managing LLM workflows as a self-hosted
                                    solution.
 ## About the Project "PromptMage" is designed to offer an intuitive interface
 that simplifies the process of creating and managing LLM workflows as a self-
 hosted solution. It facilitates prompt testing and comparison, and it
 incorporates version control features to help users track the development of
-their prompts. Suitable for both small teams and large enterprises, "FlowForge"
-seeks to improve productivity and foster the practical use of LLM technology.
-The approach with "PromptMage" is to provide a pragmatic solution that bridges
-the current gap in LLM workflow management. We aim to empower developers,
-researchers, and organizations by making LLM technology more accessible and
-manageable, thereby supporting the next wave of AI innovations. ## Getting
-Started ### Installation To install promptmage, run the following command:
-```bash pip install promptmage ``` ## Usage To use promptmage, run the
-following command: ```bash promptmage cast ``` ## Roadmap Coming soon. ##
-Development To develop PromptMage, check out the [DEVELOPMENT.md]
-(DEVELOPMENT.md) file. ## Contributing Contributing We welcome contributions
-from the community! If you're interested in improving PromptMage, you can
-contribute in the following ways: * **Reporting Bugs**: Submit an issue in our
-repository, providing a detailed description of the problem and steps to
-reproduce it. * **Feature Requests**: Have ideas on how to make FlowForge
-better? We'd love to hear from you! Please submit an issue, detailing your
-suggestions. * **Pull Requests**: Contributions via pull requests are highly
-appreciated. Please ensure your code adheres to the coding standards of the
-project, and submit a pull request with a clear description of your changes. ##
-License This project is licensed under the MIT License - see the [LICENSE.md]
-(LICENSE.md) file for details. ## Contact For any inquiries or further
-information, feel free to reach out at [promptmage@tobiassterbak.com](mailto:
-promptmage@tobiassterbak.com). ## â¤ï¸ Acknowledgements This project was
-supported by_[_i_m_a_g_e_s_/_m_t_l_-_p_o_w_e_r_e_d_-_b_y_._p_n_g_]
+their prompts. Suitable for both small teams and large enterprises,
+"PromptMage" seeks to improve productivity and foster the practical use of LLM
+technology. The approach with "PromptMage" is to provide a pragmatic solution
+that bridges the current gap in LLM workflow management. We aim to empower
+developers, researchers, and organizations by making LLM technology more
+accessible and manageable, thereby supporting the next wave of AI innovations.
+## Philosophy - Prompts as first-class citizens - Type-hint everything for
+automatic inference and validation magic - build-in, automatically created API
+with fastAPI for easy integration ## Getting Started ### Installation To
+install promptmage, run the following command: ```bash pip install promptmage
+``` ## Usage To use promptmage, run the following command: ```bash promptmage
+cast ``` ## Roadmap Coming soon. ## Development To develop PromptMage, check
+out the [DEVELOPMENT.md](DEVELOPMENT.md) file. ## Contributing Contributing We
+welcome contributions from the community! If you're interested in improving
+PromptMage, you can contribute in the following ways: * **Reporting Bugs**:
+Submit an issue in our repository, providing a detailed description of the
+problem and steps to reproduce it. * **Feature Requests**: Have ideas on how to
+make FlowForge better? We'd love to hear from you! Please submit an issue,
+detailing your suggestions. * **Pull Requests**: Contributions via pull
+requests are highly appreciated. Please ensure your code adheres to the coding
+standards of the project, and submit a pull request with a clear description of
+your changes. ## License This project is licensed under the MIT License - see
+the [LICENSE.md](LICENSE.md) file for details. ## Contact For any inquiries or
+further information, feel free to reach out at [promptmage@tobiassterbak.com]
+(mailto:promptmage@tobiassterbak.com). ## â¤ï¸ Acknowledgements This project
+was supported by_[_i_m_a_g_e_s_/_m_t_l_-_p_o_w_e_r_e_d_-_b_y_._p_n_g_]
```

