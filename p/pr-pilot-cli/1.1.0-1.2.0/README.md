# Comparing `tmp/pr_pilot_cli-1.1.0.tar.gz` & `tmp/pr_pilot_cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.1.0.tar", last modified: Tue May 28 00:36:21 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.2.0.tar", last modified: Tue May 28 01:10:01 2024, max compression
```

## Comparing `pr_pilot_cli-1.1.0.tar` & `pr_pilot_cli-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/cli/detect_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:10:01.607020 pr_pilot_cli-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-28 01:10:01.607020 pr_pilot_cli-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:10:01.603020 pr_pilot_cli-1.2.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/cli/detect_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:10:01.607020 pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-28 01:10:01.000000 pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 01:10:01.000000 pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:10:01.000000 pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 01:10:01.000000 pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 01:10:01.000000 pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 01:10:01.000000 pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:10:01.607020 pr_pilot_cli-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 01:09:53.000000 pr_pilot_cli-1.2.0/setup.py
```

### Comparing `pr_pilot_cli-1.1.0/LICENSE` & `pr_pilot_cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.1.0/PKG-INFO` & `pr_pilot_cli-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,22 +23,17 @@
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
   <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
 # PR Pilot CLI
 
-The PR Pilot CLI is a command-line interface tool designed to interact with the PR Pilot API. 
-It allows users to quickly hand over work to PR Pilot from the command line.
-
-## Features
-- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
-- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
-- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
-- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
+PR Pilot gives you a natural language interface for your Github projects.
+Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
+and Github issues, enabling a wide variety of ground-breaking AI-assisted automation use cases.
 
 ## Installation
 
  > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
 
 To install the CLI, run the following command:
 
@@ -48,33 +43,57 @@
 
 By default, the CLI will prompt you to input your API key if it is not already configured.
 
 ## Usage
 
 After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
 
+### Examples
+
+Translate a file:
+
+```bash
+pilot --raw "translate the README into German" > README_German.md
+```
+
+Let it write some unit tests:
+
+```bash
+pilot "Write some unit tests for the utils.py file."
+```
+
+Find some information in your Github issues:
+
 ```bash
-pilot Translate the README file into German.
+pilot "Do we have any open Github issues regarding the AuthenticationView class?"
 ```
 
+For more information, check out our [User Guide](https://docs.pr-pilot.ai/user_guide.html).
+
 ### Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
 Usage: pilot [OPTIONS] [PROMPT]...
 
 Options:
   --wait / --no-wait  Wait for the result.
   --repo TEXT         Github repository in the format owner/repo.
   --chatty            Print more information.
+  --raw               For piping. No pretty-print, no status indicator.
   --help              Show this message and exit.
 ```
 
 
+## Features
+- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
+- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
+- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
+- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
 
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,35 +1,42 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.1.0 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.2.0 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
-# PR Pilot CLI The PR Pilot CLI is a command-line interface tool designed to
-interact with the PR Pilot API. It allows users to quickly hand over work to PR
-Pilot from the command line. ## Features - **Configuration Management**:
-Automatically manages API key configuration by prompting the user to input
-their API key if not already configured. - **Task Creation**: Users can create
-tasks by specifying a repository and a prompt. The CLI handles task creation
-and optionally waits for the result. - **Result Retrieval**: If the `--wait`
-option is used, the CLI waits for the task to complete and displays the result
-directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
-the CLI provides a link to the task's dashboard for further monitoring. ##
+# PR Pilot CLI PR Pilot gives you a natural language interface for your Github
+projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
+fulfill tasks by interacting with your code base and Github issues, enabling a
+wide variety of ground-breaking AI-assisted automation use cases. ##
 Installation > Make sure you have PR Pilot [installed in your repository]
 (https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
 the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
 default, the CLI will prompt you to input your API key if it is not already
 configured. ## Usage After installation, open a terminal and `ls` into a
-repository you have installed PR Pilot in and talk to PR Pilot: ```bash pilot
-Translate the README file into German. ``` ### Options and Parameters You can
+repository you have installed PR Pilot in and talk to PR Pilot: ### Examples
+Translate a file: ```bash pilot --raw "translate the README into German" >
+README_German.md ``` Let it write some unit tests: ```bash pilot "Write some
+unit tests for the utils.py file." ``` Find some information in your Github
+issues: ```bash pilot "Do we have any open Github issues regarding the
+AuthenticationView class?" ``` For more information, check out our [User Guide]
+(https://docs.pr-pilot.ai/user_guide.html). ### Options and Parameters You can
 change the default settings with parameters and options: ```bash Usage: pilot
 [OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
 TEXT Github repository in the format owner/repo. --chatty Print more
-information. --help Show this message and exit. ``` ## Configuration The
-configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
-Contributors are welcome to improve the CLI by submitting pull requests or
-reporting issues. For more details, check the project's GitHub repository. ##
-License The PR Pilot CLI is open-source software licensed under the GPL-
-3 license.
+information. --raw For piping. No pretty-print, no status indicator. --help
+Show this message and exit. ``` ## Features - **Configuration Management**:
+Automatically manages API key configuration by prompting the user to input
+their API key if not already configured. - **Task Creation**: Users can create
+tasks by specifying a repository and a prompt. The CLI handles task creation
+and optionally waits for the result. - **Result Retrieval**: If the `--wait`
+option is used, the CLI waits for the task to complete and displays the result
+directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
+the CLI provides a link to the task's dashboard for further monitoring. ##
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.1.0/README.md` & `pr_pilot_cli-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,17 @@
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
   <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
 # PR Pilot CLI
 
-The PR Pilot CLI is a command-line interface tool designed to interact with the PR Pilot API. 
-It allows users to quickly hand over work to PR Pilot from the command line.
-
-## Features
-- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
-- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
-- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
-- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
+PR Pilot gives you a natural language interface for your Github projects.
+Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
+and Github issues, enabling a wide variety of ground-breaking AI-assisted automation use cases.
 
 ## Installation
 
  > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
 
 To install the CLI, run the following command:
 
@@ -32,33 +27,57 @@
 
 By default, the CLI will prompt you to input your API key if it is not already configured.
 
 ## Usage
 
 After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
 
+### Examples
+
+Translate a file:
+
+```bash
+pilot --raw "translate the README into German" > README_German.md
+```
+
+Let it write some unit tests:
+
+```bash
+pilot "Write some unit tests for the utils.py file."
+```
+
+Find some information in your Github issues:
+
 ```bash
-pilot Translate the README file into German.
+pilot "Do we have any open Github issues regarding the AuthenticationView class?"
 ```
 
+For more information, check out our [User Guide](https://docs.pr-pilot.ai/user_guide.html).
+
 ### Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
 Usage: pilot [OPTIONS] [PROMPT]...
 
 Options:
   --wait / --no-wait  Wait for the result.
   --repo TEXT         Github repository in the format owner/repo.
   --chatty            Print more information.
+  --raw               For piping. No pretty-print, no status indicator.
   --help              Show this message and exit.
 ```
 
 
+## Features
+- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
+- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
+- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
+- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
 
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,28 +1,35 @@
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
-# PR Pilot CLI The PR Pilot CLI is a command-line interface tool designed to
-interact with the PR Pilot API. It allows users to quickly hand over work to PR
-Pilot from the command line. ## Features - **Configuration Management**:
-Automatically manages API key configuration by prompting the user to input
-their API key if not already configured. - **Task Creation**: Users can create
-tasks by specifying a repository and a prompt. The CLI handles task creation
-and optionally waits for the result. - **Result Retrieval**: If the `--wait`
-option is used, the CLI waits for the task to complete and displays the result
-directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
-the CLI provides a link to the task's dashboard for further monitoring. ##
+# PR Pilot CLI PR Pilot gives you a natural language interface for your Github
+projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
+fulfill tasks by interacting with your code base and Github issues, enabling a
+wide variety of ground-breaking AI-assisted automation use cases. ##
 Installation > Make sure you have PR Pilot [installed in your repository]
 (https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
 the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
 default, the CLI will prompt you to input your API key if it is not already
 configured. ## Usage After installation, open a terminal and `ls` into a
-repository you have installed PR Pilot in and talk to PR Pilot: ```bash pilot
-Translate the README file into German. ``` ### Options and Parameters You can
+repository you have installed PR Pilot in and talk to PR Pilot: ### Examples
+Translate a file: ```bash pilot --raw "translate the README into German" >
+README_German.md ``` Let it write some unit tests: ```bash pilot "Write some
+unit tests for the utils.py file." ``` Find some information in your Github
+issues: ```bash pilot "Do we have any open Github issues regarding the
+AuthenticationView class?" ``` For more information, check out our [User Guide]
+(https://docs.pr-pilot.ai/user_guide.html). ### Options and Parameters You can
 change the default settings with parameters and options: ```bash Usage: pilot
 [OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
 TEXT Github repository in the format owner/repo. --chatty Print more
-information. --help Show this message and exit. ``` ## Configuration The
-configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
-Contributors are welcome to improve the CLI by submitting pull requests or
-reporting issues. For more details, check the project's GitHub repository. ##
-License The PR Pilot CLI is open-source software licensed under the GPL-
-3 license.
+information. --raw For piping. No pretty-print, no status indicator. --help
+Show this message and exit. ``` ## Features - **Configuration Management**:
+Automatically manages API key configuration by prompting the user to input
+their API key if not already configured. - **Task Creation**: Users can create
+tasks by specifying a repository and a prompt. The CLI handles task creation
+and optionally waits for the result. - **Result Retrieval**: If the `--wait`
+option is used, the CLI waits for the task to complete and displays the result
+directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
+the CLI provides a link to the task's dashboard for further monitoring. ##
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.1.0/cli/cli.py` & `pr_pilot_cli-1.2.0/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,17 @@
     return config
 
 
 @click.command()
 @click.option('--wait/--no-wait', is_flag=True, default=True, help='Wait for the result.')
 @click.option('--repo', help='Github repository in the format owner/repo.', required=False)
 @click.option('--chatty', is_flag=True, default=False, help='Print more information.')
+@click.option('--raw', is_flag=True, default=False, help='For piping. No pretty-print, no status indicator.')
 @click.argument('prompt', nargs=-1)
-def main(wait, repo, chatty, prompt):
+def main(wait, repo, chatty, raw, prompt):
     prompt = ' '.join(prompt)
     config = load_config()
     if not os.getenv("PR_PILOT_API_KEY"):
         os.environ["PR_PILOT_API_KEY"] = config[CONFIG_API_KEY]
     if not repo:
         # No repository provided, try to detect it
         repo = detect_repository()
@@ -46,14 +47,20 @@
         repo = config.get("default_repo")
     if not repo:
         click.echo(f"No Github repository provided. Use --repo or set 'default_repo' in {CONFIG_LOCATION}.")
         return
     if not prompt:
         click.echo("Please provide a prompt.")
         return
+
+    if raw:
+        task = create_task(repo, prompt, log=False)
+        result = wait_for_result(task, log=False)
+        print(result)
+        return
     with yaspin(text=f"Creating new task for repository {repo}", color="cyan") as sp:
         task = create_task(repo, prompt)
         dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{task.id}/"
         if chatty:
             sp.write(f"✅ Task created: {dashboard_url}")
         if wait:
             sp.text = f"I'm working on it :) Track my progress in the dashboard: {dashboard_url}"
@@ -61,14 +68,17 @@
                 result = wait_for_result(task)
                 if chatty:
                     sp.ok("✅")
                 else:
                     sp.hide()
                 console = Console()
                 console.line()
-                console.print(Markdown(result))
+                if raw:
+                    console.print(result)
+                else:
+                    console.print(Markdown(result))
             except Exception as e:
                 sp.fail("💥")
                 click.echo(f"Error: {e}")
 
 if __name__ == '__main__':
     main()
```

### Comparing `pr_pilot_cli-1.1.0/cli/detect_repository.py` & `pr_pilot_cli-1.2.0/cli/detect_repository.py`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.2.0/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.1.0
+Version: 1.2.0
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,22 +23,17 @@
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
   <a href="https://www.pr-pilot.ai/blog">Blog</a> | 
   <a href="https://www.pr-pilot.ai">Website</a>
 </p>
 
 # PR Pilot CLI
 
-The PR Pilot CLI is a command-line interface tool designed to interact with the PR Pilot API. 
-It allows users to quickly hand over work to PR Pilot from the command line.
-
-## Features
-- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
-- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
-- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
-- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
+PR Pilot gives you a natural language interface for your Github projects.
+Given a prompt, it uses LLMs (Large Language Models) to autonomously fulfill tasks by interacting with your code base
+and Github issues, enabling a wide variety of ground-breaking AI-assisted automation use cases.
 
 ## Installation
 
  > Make sure you have PR Pilot [installed in your repository](https://github.com/apps/pr-pilot-ai/installations/new)
 
 To install the CLI, run the following command:
 
@@ -48,33 +43,57 @@
 
 By default, the CLI will prompt you to input your API key if it is not already configured.
 
 ## Usage
 
 After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
 
+### Examples
+
+Translate a file:
+
+```bash
+pilot --raw "translate the README into German" > README_German.md
+```
+
+Let it write some unit tests:
+
+```bash
+pilot "Write some unit tests for the utils.py file."
+```
+
+Find some information in your Github issues:
+
 ```bash
-pilot Translate the README file into German.
+pilot "Do we have any open Github issues regarding the AuthenticationView class?"
 ```
 
+For more information, check out our [User Guide](https://docs.pr-pilot.ai/user_guide.html).
+
 ### Options and Parameters
 
 You can change the default settings with parameters and options:
 
 ```bash
 Usage: pilot [OPTIONS] [PROMPT]...
 
 Options:
   --wait / --no-wait  Wait for the result.
   --repo TEXT         Github repository in the format owner/repo.
   --chatty            Print more information.
+  --raw               For piping. No pretty-print, no status indicator.
   --help              Show this message and exit.
 ```
 
 
+## Features
+- **Configuration Management**: Automatically manages API key configuration by prompting the user to input their API key if not already configured.
+- **Task Creation**: Users can create tasks by specifying a repository and a prompt. The CLI handles task creation and optionally waits for the result.
+- **Result Retrieval**: If the `--wait` option is used, the CLI waits for the task to complete and displays the result directly in the terminal.
+- **Dashboard Link**: For tasks that are not awaited, the CLI provides a link to the task's dashboard for further monitoring.
 
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,35 +1,42 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.1.0 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.2.0 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
-# PR Pilot CLI The PR Pilot CLI is a command-line interface tool designed to
-interact with the PR Pilot API. It allows users to quickly hand over work to PR
-Pilot from the command line. ## Features - **Configuration Management**:
-Automatically manages API key configuration by prompting the user to input
-their API key if not already configured. - **Task Creation**: Users can create
-tasks by specifying a repository and a prompt. The CLI handles task creation
-and optionally waits for the result. - **Result Retrieval**: If the `--wait`
-option is used, the CLI waits for the task to complete and displays the result
-directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
-the CLI provides a link to the task's dashboard for further monitoring. ##
+# PR Pilot CLI PR Pilot gives you a natural language interface for your Github
+projects. Given a prompt, it uses LLMs (Large Language Models) to autonomously
+fulfill tasks by interacting with your code base and Github issues, enabling a
+wide variety of ground-breaking AI-assisted automation use cases. ##
 Installation > Make sure you have PR Pilot [installed in your repository]
 (https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
 the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
 default, the CLI will prompt you to input your API key if it is not already
 configured. ## Usage After installation, open a terminal and `ls` into a
-repository you have installed PR Pilot in and talk to PR Pilot: ```bash pilot
-Translate the README file into German. ``` ### Options and Parameters You can
+repository you have installed PR Pilot in and talk to PR Pilot: ### Examples
+Translate a file: ```bash pilot --raw "translate the README into German" >
+README_German.md ``` Let it write some unit tests: ```bash pilot "Write some
+unit tests for the utils.py file." ``` Find some information in your Github
+issues: ```bash pilot "Do we have any open Github issues regarding the
+AuthenticationView class?" ``` For more information, check out our [User Guide]
+(https://docs.pr-pilot.ai/user_guide.html). ### Options and Parameters You can
 change the default settings with parameters and options: ```bash Usage: pilot
 [OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
 TEXT Github repository in the format owner/repo. --chatty Print more
-information. --help Show this message and exit. ``` ## Configuration The
-configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
-Contributors are welcome to improve the CLI by submitting pull requests or
-reporting issues. For more details, check the project's GitHub repository. ##
-License The PR Pilot CLI is open-source software licensed under the GPL-
-3 license.
+information. --raw For piping. No pretty-print, no status indicator. --help
+Show this message and exit. ``` ## Features - **Configuration Management**:
+Automatically manages API key configuration by prompting the user to input
+their API key if not already configured. - **Task Creation**: Users can create
+tasks by specifying a repository and a prompt. The CLI handles task creation
+and optionally waits for the result. - **Result Retrieval**: If the `--wait`
+option is used, the CLI waits for the task to complete and displays the result
+directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
+the CLI provides a link to the task's dashboard for further monitoring. ##
+Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
+Contributing Contributors are welcome to improve the CLI by submitting pull
+requests or reporting issues. For more details, check the project's GitHub
+repository. ## License The PR Pilot CLI is open-source software licensed under
+the GPL-3 license.
```

### Comparing `pr_pilot_cli-1.1.0/setup.py` & `pr_pilot_cli-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.1.0',
+    version='1.2.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

