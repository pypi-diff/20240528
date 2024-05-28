# Comparing `tmp/pr_pilot_cli-1.0.3.tar.gz` & `tmp/pr_pilot_cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.0.3.tar", last modified: Mon May 27 23:32:44 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.0.4.tar", last modified: Mon May 27 23:37:16 2024, max compression
```

## Comparing `pr_pilot_cli-1.0.3.tar` & `pr_pilot_cli-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:32:44.581102 pr_pilot_cli-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 23:32:40.000000 pr_pilot_cli-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 23:32:40.000000 pr_pilot_cli-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-27 23:32:44.581102 pr_pilot_cli-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-27 23:32:40.000000 pr_pilot_cli-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:32:44.577102 pr_pilot_cli-1.0.3/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:32:40.000000 pr_pilot_cli-1.0.3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-27 23:32:40.000000 pr_pilot_cli-1.0.3/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:32:44.581102 pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-27 23:32:44.000000 pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 23:32:44.000000 pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:32:44.000000 pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 23:32:44.000000 pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 23:32:44.000000 pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 23:32:44.000000 pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 23:32:40.000000 pr_pilot_cli-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 23:32:44.581102 pr_pilot_cli-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 23:32:40.000000 pr_pilot_cli-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/setup.py
```

### Comparing `pr_pilot_cli-1.0.3/LICENSE` & `pr_pilot_cli-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.0.3/PKG-INFO` & `pr_pilot_cli-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,18 +33,21 @@
 ## Features
 - **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
 - **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
 - **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
 - **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
 
 ## Installation
+
+ > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
+
 To install the CLI, run the following command:
 
 ```bash
-pip install pr-pilot-cli
+pip install --upgrade pr-pilot-cli
 ```
 
 ## Usage
 
 After installation, create tasks using the following command:
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.0.3 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.0.4 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
@@ -13,15 +13,17 @@
 Automatically manages API key configuration by prompting the user to input
 their API key if not already configured. - **Task Creation**: Users can create
 tasks by specifying a repository and a prompt. The CLI handles task creation
 and optionally waits for the result. - **Result Retrieval**: If the `--wait`
 option is used, the CLI waits for the task to complete and displays the result
 directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
 the CLI provides a link to the task's dashboard for further monitoring. ##
-Installation To install the CLI, run the following command: ```bash pip install
-pr-pilot-cli ``` ## Usage After installation, create tasks using the following
-command: ```bash pr-pilot --wait ``` Replace `` and `` with the appropriate
-repository and task prompt. ## Configuration The configuration file is located
-at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to improve the
-CLI by submitting pull requests or reporting issues. For more details, check
-the project's GitHub repository. ## License The PR Pilot CLI is open-source
-software licensed under the GPL-3 license.
+Installation > Make sure you have PR Pilot [installed in your repository]
+(https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
+the following command: ```bash pip install --upgrade pr-pilot-cli ``` ## Usage
+After installation, create tasks using the following command: ```bash pr-pilot
+--wait ``` Replace `` and `` with the appropriate repository and task prompt.
+## Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.0.3/README.md` & `pr_pilot_cli-1.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,21 @@
 ## Features
 - **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
 - **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
 - **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
 - **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
 
 ## Installation
+
+ > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
+
 To install the CLI, run the following command:
 
 ```bash
-pip install pr-pilot-cli
+pip install --upgrade pr-pilot-cli
 ```
 
 ## Usage
 
 After installation, create tasks using the following command:
 
 ```bash
```

#### html2text {}

```diff
@@ -6,15 +6,17 @@
 Automatically manages API key configuration by prompting the user to input
 their API key if not already configured. - **Task Creation**: Users can create
 tasks by specifying a repository and a prompt. The CLI handles task creation
 and optionally waits for the result. - **Result Retrieval**: If the `--wait`
 option is used, the CLI waits for the task to complete and displays the result
 directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
 the CLI provides a link to the task's dashboard for further monitoring. ##
-Installation To install the CLI, run the following command: ```bash pip install
-pr-pilot-cli ``` ## Usage After installation, create tasks using the following
-command: ```bash pr-pilot --wait ``` Replace `` and `` with the appropriate
-repository and task prompt. ## Configuration The configuration file is located
-at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to improve the
-CLI by submitting pull requests or reporting issues. For more details, check
-the project's GitHub repository. ## License The PR Pilot CLI is open-source
-software licensed under the GPL-3 license.
+Installation > Make sure you have PR Pilot [installed in your repository]
+(https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
+the following command: ```bash pip install --upgrade pr-pilot-cli ``` ## Usage
+After installation, create tasks using the following command: ```bash pr-pilot
+--wait ``` Replace `` and `` with the appropriate repository and task prompt.
+## Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.0.3/cli/cli.py` & `pr_pilot_cli-1.0.4/cli/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     return config
 
 
 @click.command()
 @click.option('--wait', is_flag=True, help='Wait for the result.')
 @click.argument('repo')
 @click.argument('prompt', nargs=-1)
-def pilot_command(wait, repo, prompt):
+def main(wait, repo, prompt):
     prompt = ' '.join(prompt)
     config = load_config()
     if not os.getenv("PR_PILOT_API_KEY"):
         os.environ["PR_PILOT_API_KEY"] = config[CONFIG_API_KEY]
     with yaspin(text="Creating new task", color="cyan") as sp:
         task = create_task(repo, prompt)
         dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{task.id}/"
@@ -50,8 +50,8 @@
                 sp.fail("💥")
                 click.echo(f"Error: {e}")
         else:
             click.echo(f"Task created: {dashboard_url}")
 
 
 if __name__ == '__main__':
-    pilot_command()
+    main()
```

### Comparing `pr_pilot_cli-1.0.3/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -33,18 +33,21 @@
 ## Features
 - **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
 - **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
 - **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
 - **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
 
 ## Installation
+
+ > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
+
 To install the CLI, run the following command:
 
 ```bash
-pip install pr-pilot-cli
+pip install --upgrade pr-pilot-cli
 ```
 
 ## Usage
 
 After installation, create tasks using the following command:
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.0.3 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.0.4 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
@@ -13,15 +13,17 @@
 Automatically manages API key configuration by prompting the user to input
 their API key if not already configured. - **Task Creation**: Users can create
 tasks by specifying a repository and a prompt. The CLI handles task creation
 and optionally waits for the result. - **Result Retrieval**: If the `--wait`
 option is used, the CLI waits for the task to complete and displays the result
 directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
 the CLI provides a link to the task's dashboard for further monitoring. ##
-Installation To install the CLI, run the following command: ```bash pip install
-pr-pilot-cli ``` ## Usage After installation, create tasks using the following
-command: ```bash pr-pilot --wait ``` Replace `` and `` with the appropriate
-repository and task prompt. ## Configuration The configuration file is located
-at `~/.pr-pilot.yaml`. ## Contributing Contributors are welcome to improve the
-CLI by submitting pull requests or reporting issues. For more details, check
-the project's GitHub repository. ## License The PR Pilot CLI is open-source
-software licensed under the GPL-3 license.
+Installation > Make sure you have PR Pilot [installed in your repository]
+(https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
+the following command: ```bash pip install --upgrade pr-pilot-cli ``` ## Usage
+After installation, create tasks using the following command: ```bash pr-pilot
+--wait ``` Replace `` and `` with the appropriate repository and task prompt.
+## Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.0.3/setup.py` & `pr_pilot_cli-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

