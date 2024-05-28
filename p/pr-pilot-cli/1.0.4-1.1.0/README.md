# Comparing `tmp/pr_pilot_cli-1.0.4.tar.gz` & `tmp/pr_pilot_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot_cli-1.0.4.tar", last modified: Mon May 27 23:37:16 2024, max compression
+gzip compressed data, was "pr_pilot_cli-1.1.0.tar", last modified: Tue May 28 00:36:21 2024, max compression
```

## Comparing `pr_pilot_cli-1.0.4.tar` & `pr_pilot_cli-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 23:37:16.000000 pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 23:37:16.637877 pr_pilot_cli-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-27 23:37:12.000000 pr_pilot_cli-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/cli/detect_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-28 00:36:21.000000 pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:36:21.774507 pr_pilot_cli-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-28 00:36:17.000000 pr_pilot_cli-1.1.0/setup.py
```

### Comparing `pr_pilot_cli-1.0.4/LICENSE` & `pr_pilot_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot_cli-1.0.4/PKG-INFO` & `pr_pilot_cli-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-pilot-cli
-Version: 1.0.4
+Version: 1.1.0
 Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -42,23 +42,40 @@
 
 To install the CLI, run the following command:
 
 ```bash
 pip install --upgrade pr-pilot-cli
 ```
 
+By default, the CLI will prompt you to input your API key if it is not already configured.
+
 ## Usage
 
-After installation, create tasks using the following command:
+After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
 
 ```bash
-pr-pilot --wait <repo> <prompt>
+pilot Translate the README file into German.
 ```
 
-Replace `<repo>` and `<prompt>` with the appropriate repository and task prompt.
+### Options and Parameters
+
+You can change the default settings with parameters and options:
+
+```bash
+Usage: pilot [OPTIONS] [PROMPT]...
+
+Options:
+  --wait / --no-wait  Wait for the result.
+  --repo TEXT         Github repository in the format owner/repo.
+  --chatty            Print more information.
+  --help              Show this message and exit.
+```
+
+
+
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.0.4 Summary: CLI for PR
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.1.0 Summary: CLI for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
 marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
 pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
 Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
@@ -15,15 +15,21 @@
 tasks by specifying a repository and a prompt. The CLI handles task creation
 and optionally waits for the result. - **Result Retrieval**: If the `--wait`
 option is used, the CLI waits for the task to complete and displays the result
 directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
 the CLI provides a link to the task's dashboard for further monitoring. ##
 Installation > Make sure you have PR Pilot [installed in your repository]
 (https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
-the following command: ```bash pip install --upgrade pr-pilot-cli ``` ## Usage
-After installation, create tasks using the following command: ```bash pr-pilot
---wait ``` Replace `` and `` with the appropriate repository and task prompt.
-## Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
+default, the CLI will prompt you to input your API key if it is not already
+configured. ## Usage After installation, open a terminal and `ls` into a
+repository you have installed PR Pilot in and talk to PR Pilot: ```bash pilot
+Translate the README file into German. ``` ### Options and Parameters You can
+change the default settings with parameters and options: ```bash Usage: pilot
+[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
+TEXT Github repository in the format owner/repo. --chatty Print more
+information. --help Show this message and exit. ``` ## Configuration The
+configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
+Contributors are welcome to improve the CLI by submitting pull requests or
+reporting issues. For more details, check the project's GitHub repository. ##
+License The PR Pilot CLI is open-source software licensed under the GPL-
+3 license.
```

### Comparing `pr_pilot_cli-1.0.4/README.md` & `pr_pilot_cli-1.1.0/pr_pilot_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: pr-pilot-cli
+Version: 1.1.0
+Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
+Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
+Author: Marco Lamina
+Author-email: marco@pr-pilot.ai
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click==8.1.7
+Requires-Dist: pr-pilot==1.4.0
+Requires-Dist: pyyaml==6.0.1
+Requires-Dist: yaspin==3.0.2
+Requires-Dist: rich==13.7.1
+
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
@@ -26,23 +42,40 @@
 
 To install the CLI, run the following command:
 
 ```bash
 pip install --upgrade pr-pilot-cli
 ```
 
+By default, the CLI will prompt you to input your API key if it is not already configured.
+
 ## Usage
 
-After installation, create tasks using the following command:
+After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
+
+```bash
+pilot Translate the README file into German.
+```
+
+### Options and Parameters
+
+You can change the default settings with parameters and options:
 
 ```bash
-pr-pilot --wait <repo> <prompt>
+Usage: pilot [OPTIONS] [PROMPT]...
+
+Options:
+  --wait / --no-wait  Wait for the result.
+  --repo TEXT         Github repository in the format owner/repo.
+  --chatty            Print more information.
+  --help              Show this message and exit.
 ```
 
-Replace `<repo>` and `<prompt>` with the appropriate repository and task prompt.
+
+
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,22 +1,35 @@
+Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.1.0 Summary: CLI for PR
+Pilot, a text-to-task automation platform for Github. Home-page: https://
+github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
+marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
+pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
+Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI The PR Pilot CLI is a command-line interface tool designed to
 interact with the PR Pilot API. It allows users to quickly hand over work to PR
 Pilot from the command line. ## Features - **Configuration Management**:
 Automatically manages API key configuration by prompting the user to input
 their API key if not already configured. - **Task Creation**: Users can create
 tasks by specifying a repository and a prompt. The CLI handles task creation
 and optionally waits for the result. - **Result Retrieval**: If the `--wait`
 option is used, the CLI waits for the task to complete and displays the result
 directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
 the CLI provides a link to the task's dashboard for further monitoring. ##
 Installation > Make sure you have PR Pilot [installed in your repository]
 (https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
-the following command: ```bash pip install --upgrade pr-pilot-cli ``` ## Usage
-After installation, create tasks using the following command: ```bash pr-pilot
---wait ``` Replace `` and `` with the appropriate repository and task prompt.
-## Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
+default, the CLI will prompt you to input your API key if it is not already
+configured. ## Usage After installation, open a terminal and `ls` into a
+repository you have installed PR Pilot in and talk to PR Pilot: ```bash pilot
+Translate the README file into German. ``` ### Options and Parameters You can
+change the default settings with parameters and options: ```bash Usage: pilot
+[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
+TEXT Github repository in the format owner/repo. --chatty Print more
+information. --help Show this message and exit. ``` ## Configuration The
+configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
+Contributors are welcome to improve the CLI by submitting pull requests or
+reporting issues. For more details, check the project's GitHub repository. ##
+License The PR Pilot CLI is open-source software licensed under the GPL-
+3 license.
```

### Comparing `pr_pilot_cli-1.0.4/cli/cli.py` & `pr_pilot_cli-1.1.0/cli/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import click
 import yaml
 from pr_pilot.util import create_task, wait_for_result
 from rich.console import Console
 from rich.markdown import Markdown
 from yaspin import yaspin
 
+from cli.detect_repository import detect_repository
+
 CONFIG_LOCATION = os.path.expanduser('~/.pr-pilot.yaml')
 CONFIG_API_KEY = "api_key"
 
 
 def load_config():
     """Load the configuration from the default location. If it doesn't exist,
     ask user to enter API key and save config."""
@@ -23,35 +25,50 @@
         click.echo(f"Configuration saved in {CONFIG_LOCATION}")
     with open(CONFIG_LOCATION) as f:
         config = yaml.safe_load(f)
     return config
 
 
 @click.command()
-@click.option('--wait', is_flag=True, help='Wait for the result.')
-@click.argument('repo')
+@click.option('--wait/--no-wait', is_flag=True, default=True, help='Wait for the result.')
+@click.option('--repo', help='Github repository in the format owner/repo.', required=False)
+@click.option('--chatty', is_flag=True, default=False, help='Print more information.')
 @click.argument('prompt', nargs=-1)
-def main(wait, repo, prompt):
+def main(wait, repo, chatty, prompt):
     prompt = ' '.join(prompt)
     config = load_config()
     if not os.getenv("PR_PILOT_API_KEY"):
         os.environ["PR_PILOT_API_KEY"] = config[CONFIG_API_KEY]
-    with yaspin(text="Creating new task", color="cyan") as sp:
+    if not repo:
+        # No repository provided, try to detect it
+        repo = detect_repository()
+    if not repo:
+        # Current directory is not a git repository, see if there is a default repo in the config
+        repo = config.get("default_repo")
+    if not repo:
+        click.echo(f"No Github repository provided. Use --repo or set 'default_repo' in {CONFIG_LOCATION}.")
+        return
+    if not prompt:
+        click.echo("Please provide a prompt.")
+        return
+    with yaspin(text=f"Creating new task for repository {repo}", color="cyan") as sp:
         task = create_task(repo, prompt)
         dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{task.id}/"
-        sp.write(f"✅ Task created: {dashboard_url}")
+        if chatty:
+            sp.write(f"✅ Task created: {dashboard_url}")
         if wait:
-            sp.text = "Waiting for the result"
+            sp.text = f"I'm working on it :) Track my progress in the dashboard: {dashboard_url}"
             try:
                 result = wait_for_result(task)
-                sp.ok("✅")
+                if chatty:
+                    sp.ok("✅")
+                else:
+                    sp.hide()
                 console = Console()
+                console.line()
                 console.print(Markdown(result))
             except Exception as e:
                 sp.fail("💥")
                 click.echo(f"Error: {e}")
-        else:
-            click.echo(f"Task created: {dashboard_url}")
-
 
 if __name__ == '__main__':
     main()
```

### Comparing `pr_pilot_cli-1.0.4/pr_pilot_cli.egg-info/PKG-INFO` & `pr_pilot_cli-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: pr-pilot-cli
-Version: 1.0.4
-Summary: CLI for PR Pilot, a text-to-task automation platform for Github.
-Home-page: https://github.com/PR-Pilot-AI/pr-pilot-cli
-Author: Marco Lamina
-Author-email: marco@pr-pilot.ai
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: click==8.1.7
-Requires-Dist: pr-pilot==1.4.0
-Requires-Dist: pyyaml==6.0.1
-Requires-Dist: yaspin==3.0.2
-Requires-Dist: rich==13.7.1
-
 <div align="center">
 <img src="https://avatars.githubusercontent.com/ml/17635?s=140&v=" width="100" alt="PR Pilot Logo">
 </div>
 
 <p align="center">
   <a href="https://github.com/apps/pr-pilot-ai/installations/new"><b>Install</b></a> |
   <a href="https://docs.pr-pilot.ai">Documentation</a> | 
@@ -42,23 +26,40 @@
 
 To install the CLI, run the following command:
 
 ```bash
 pip install --upgrade pr-pilot-cli
 ```
 
+By default, the CLI will prompt you to input your API key if it is not already configured.
+
 ## Usage
 
-After installation, create tasks using the following command:
+After installation, open a terminal and `ls` into a repository you have installed PR Pilot in and talk to PR Pilot:
+
+```bash
+pilot Translate the README file into German.
+```
+
+### Options and Parameters
+
+You can change the default settings with parameters and options:
 
 ```bash
-pr-pilot --wait <repo> <prompt>
+Usage: pilot [OPTIONS] [PROMPT]...
+
+Options:
+  --wait / --no-wait  Wait for the result.
+  --repo TEXT         Github repository in the format owner/repo.
+  --chatty            Print more information.
+  --help              Show this message and exit.
 ```
 
-Replace `<repo>` and `<prompt>` with the appropriate repository and task prompt.
+
+
 
 ## Configuration
 The configuration file is located at `~/.pr-pilot.yaml`.
 
 ## Contributing
 Contributors are welcome to improve the CLI by submitting pull requests or reporting issues. For more details, check the project's GitHub repository.
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
-Metadata-Version: 2.1 Name: pr-pilot-cli Version: 1.0.4 Summary: CLI for PR
-Pilot, a text-to-task automation platform for Github. Home-page: https://
-github.com/PR-Pilot-AI/pr-pilot-cli Author: Marco Lamina Author-email:
-marco@pr-pilot.ai Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE Requires-Dist: click==8.1.7 Requires-Dist: pr-
-pilot==1.4.0 Requires-Dist: pyyaml==6.0.1 Requires-Dist: yaspin==3.0.2
-Requires-Dist: rich==13.7.1
                                 [PR Pilot Logo]
                    _II_nn_ss_tt_aa_ll_ll | _D_o_c_u_m_e_n_t_a_t_i_o_n | _B_l_o_g | _W_e_b_s_i_t_e
 # PR Pilot CLI The PR Pilot CLI is a command-line interface tool designed to
 interact with the PR Pilot API. It allows users to quickly hand over work to PR
 Pilot from the command line. ## Features - **Configuration Management**:
 Automatically manages API key configuration by prompting the user to input
 their API key if not already configured. - **Task Creation**: Users can create
 tasks by specifying a repository and a prompt. The CLI handles task creation
 and optionally waits for the result. - **Result Retrieval**: If the `--wait`
 option is used, the CLI waits for the task to complete and displays the result
 directly in the terminal. - **Dashboard Link**: For tasks that are not awaited,
 the CLI provides a link to the task's dashboard for further monitoring. ##
 Installation > Make sure you have PR Pilot [installed in your repository]
 (https://github.com/apps/pr-pilot-ai/installations/new) To install the CLI, run
-the following command: ```bash pip install --upgrade pr-pilot-cli ``` ## Usage
-After installation, create tasks using the following command: ```bash pr-pilot
---wait ``` Replace `` and `` with the appropriate repository and task prompt.
-## Configuration The configuration file is located at `~/.pr-pilot.yaml`. ##
-Contributing Contributors are welcome to improve the CLI by submitting pull
-requests or reporting issues. For more details, check the project's GitHub
-repository. ## License The PR Pilot CLI is open-source software licensed under
-the GPL-3 license.
+the following command: ```bash pip install --upgrade pr-pilot-cli ``` By
+default, the CLI will prompt you to input your API key if it is not already
+configured. ## Usage After installation, open a terminal and `ls` into a
+repository you have installed PR Pilot in and talk to PR Pilot: ```bash pilot
+Translate the README file into German. ``` ### Options and Parameters You can
+change the default settings with parameters and options: ```bash Usage: pilot
+[OPTIONS] [PROMPT]... Options: --wait / --no-wait Wait for the result. --repo
+TEXT Github repository in the format owner/repo. --chatty Print more
+information. --help Show this message and exit. ``` ## Configuration The
+configuration file is located at `~/.pr-pilot.yaml`. ## Contributing
+Contributors are welcome to improve the CLI by submitting pull requests or
+reporting issues. For more details, check the project's GitHub repository. ##
+License The PR Pilot CLI is open-source software licensed under the GPL-
+3 license.
```

### Comparing `pr_pilot_cli-1.0.4/setup.py` & `pr_pilot_cli-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pr-pilot-cli',
-    version='1.0.4',
+    version='1.1.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         line.strip() for line in open('requirements.txt').readlines()
     ],
     python_requires='>=3.6',
     author='Marco Lamina',
```

