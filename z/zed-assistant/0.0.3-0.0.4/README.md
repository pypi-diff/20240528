# Comparing `tmp/zed_assistant-0.0.3.tar.gz` & `tmp/zed_assistant-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zed_assistant-0.0.3.tar", max compression
+gzip compressed data, was "zed_assistant-0.0.4.tar", max compression
```

## Comparing `zed_assistant-0.0.3.tar` & `zed_assistant-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1079 2024-05-05 21:32:34.195806 zed_assistant-0.0.3/LICENSE
--rw-r--r--   0        0        0     1601 2024-05-05 21:18:16.110046 zed_assistant-0.0.3/README.md
--rw-r--r--   0        0        0      594 2024-05-12 03:41:02.085393 zed_assistant-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      236 2024-05-12 03:37:47.407923 zed_assistant-0.0.3/zed_assistant/__init__.py
--rw-r--r--   0        0        0     2752 2024-05-12 03:38:46.770788 zed_assistant-0.0.3/zed_assistant/cli.py
--rw-r--r--   0        0        0      247 2024-05-12 02:26:14.914931 zed_assistant-0.0.3/zed_assistant/constants.py
--rw-r--r--   0        0        0       94 2024-05-05 19:30:23.980421 zed_assistant-0.0.3/zed_assistant/model/__init__.py
--rw-r--r--   0        0        0      191 2024-05-11 23:53:42.882886 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/__init__.py
--rw-r--r--   0        0        0      798 2024-05-12 02:30:09.298230 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/defs.py
--rw-r--r--   0        0        0     3478 2024-05-12 02:44:52.194827 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/runner.py
--rw-r--r--   0        0        0     3855 2024-05-12 02:36:33.556106 zed_assistant-0.0.3/zed_assistant/model/cli_prompt/template_system.j2
--rw-r--r--   0        0        0      466 2024-05-11 23:51:04.059745 zed_assistant-0.0.3/zed_assistant/model/defs.py
--rw-r--r--   0        0        0       78 2024-05-05 21:00:13.235985 zed_assistant-0.0.3/zed_assistant/utils/__init__.py
--rw-r--r--   0        0        0     2850 2024-05-11 23:29:31.307038 zed_assistant-0.0.3/zed_assistant/utils/console.py
--rw-r--r--   0        0        0      400 2024-05-05 19:30:23.981509 zed_assistant-0.0.3/zed_assistant/utils/render_utils.py
--rw-r--r--   0        0        0     1538 2024-05-12 02:44:52.938205 zed_assistant-0.0.3/zed_assistant/zed.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 zed_assistant-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-05 21:32:34.195806 zed_assistant-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1675 2024-05-27 23:33:06.034449 zed_assistant-0.0.4/README.md
+-rw-r--r--   0        0        0      594 2024-05-27 23:31:07.771997 zed_assistant-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      236 2024-05-12 03:37:47.407923 zed_assistant-0.0.4/zed_assistant/__init__.py
+-rw-r--r--   0        0        0     2469 2024-05-27 23:33:10.927137 zed_assistant-0.0.4/zed_assistant/cli.py
+-rw-r--r--   0        0        0      104 2024-05-27 23:00:01.870569 zed_assistant-0.0.4/zed_assistant/model/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-26 22:46:15.001340 zed_assistant-0.0.4/zed_assistant/model/command_prompt/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-27 22:48:27.156571 zed_assistant-0.0.4/zed_assistant/model/command_prompt/defs.py
+-rw-r--r--   0        0        0     3720 2024-05-27 23:09:14.045016 zed_assistant-0.0.4/zed_assistant/model/command_prompt/prompt_runner.py
+-rw-r--r--   0        0        0     3855 2024-05-12 02:36:33.556106 zed_assistant-0.0.4/zed_assistant/model/command_prompt/template_system.j2
+-rw-r--r--   0        0        0      755 2024-05-27 23:30:17.457102 zed_assistant-0.0.4/zed_assistant/model/defs.py
+-rw-r--r--   0        0        0        0 2024-05-26 22:28:31.784064 zed_assistant-0.0.4/zed_assistant/settings/__init__.py
+-rw-r--r--   0        0        0      723 2024-05-27 22:59:58.519004 zed_assistant-0.0.4/zed_assistant/settings/defs.py
+-rw-r--r--   0        0        0     1672 2024-05-27 23:17:33.426332 zed_assistant-0.0.4/zed_assistant/settings/loader.py
+-rw-r--r--   0        0        0       78 2024-05-05 21:00:13.235985 zed_assistant-0.0.4/zed_assistant/utils/__init__.py
+-rw-r--r--   0        0        0     2850 2024-05-11 23:29:31.307038 zed_assistant-0.0.4/zed_assistant/utils/console.py
+-rw-r--r--   0        0        0      223 2024-05-27 22:58:44.026876 zed_assistant-0.0.4/zed_assistant/utils/file_utils.py
+-rw-r--r--   0        0        0     1867 2024-05-27 23:09:14.843868 zed_assistant-0.0.4/zed_assistant/zed.py
+-rw-r--r--   0        0        0     2523 1970-01-01 00:00:00.000000 zed_assistant-0.0.4/PKG-INFO
```

### Comparing `zed_assistant-0.0.3/LICENSE` & `zed_assistant-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zed_assistant-0.0.3/pyproject.toml` & `zed_assistant-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zed-assistant"
-version = "0.0.3"
+version = "0.0.4"
 description = "Zed is an LLM-based CLI assistant built with python and Chat GPT"
 authors = ["Matheus Hoffmann Silva <me@mhsilva.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hoffmannmatheus/zed"
 
 [tool.poetry.dependencies]
```

### Comparing `zed_assistant-0.0.3/zed_assistant/cli.py` & `zed_assistant-0.0.4/zed_assistant/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,61 @@
 import asyncio
 import logging
-import os
 import sys
 from argparse import ArgumentParser
-from typing import get_args
+from typing import Tuple, get_args
 
-from zed_assistant import __version__, zed
-from zed_assistant.constants import (DEFAULT_MODEL, ENV_VARIABLE_OAI_KEY,
-                                     ENV_VARIABLE_YODA_MODE, OpenAiModel)
+from zed_assistant import __version__
+from zed_assistant.model.defs import DEFAULT_MODEL, OpenAiModel
+from zed_assistant.settings.defs import ZedSettings, SETTINGS_CONFIG_FILE
+from zed_assistant.settings.loader import merge_with_local_settings
+from zed_assistant.zed import Zed
 
 logging.basicConfig(stream=sys.stdout)
 log = logging.getLogger(__name__)
 
 zed_ascii = rf"""
      ______ ___________
     |___  /|  ___|  _  \
        / / | |__ | | | |
       / /  |  __|| | | |
     ./ /___| |___| |/ /
     \_____/\____/|___/  v{__version__}
 """
 
 
-def main():
+def main() -> None:
     parser = ArgumentParser(
-        description="zed is a LLM-based CLI assistant built with python and Chat GPT",
+        description=(
+            "zed is a LLM-based CLI assistant."
+        ),
     )
+    user_query, settings = parse_arguments(parser)
+
+    log.setLevel(logging.DEBUG if settings.debug else logging.WARNING)
+    log.debug(f" {settings=} {user_query=}")
+
+    if not user_query:
+        log.debug(" No question or command provided to zed.")
+        print(zed_ascii)
+        parser.print_help()
+        sys.exit(0)
+    if not settings.openai_key:
+        log.error(
+            " Open AI key is not configured. Please set the 'openai_key' "
+            "in ~/.zed/config"
+        )
+        sys.exit(-1)
+
+    zed = Zed(settings=settings, log=log)
+    success = asyncio.run(zed.run(user_query=user_query))
+    sys.exit(0 if success else -1)
+
+
+def parse_arguments(parser: ArgumentParser) -> Tuple[str, ZedSettings]:
     parser.add_argument(
         "--version",
         action="version",
         version=f"zed-assistant {__version__}",
     )
     parser.add_argument(
         "--debug",
@@ -38,58 +64,27 @@
         help="Enables print debug logs.",
     )
     parser.add_argument(
         "--model",
         type=str,
         choices=get_args(OpenAiModel),
         default=DEFAULT_MODEL,
-        help=f"The specific Open AI model to be used. Default is '{DEFAULT_MODEL}'.",
-    )
-    parser.add_argument(
-        "--open-ai-key",
-        type=str,
-        required=False,
-        help=f"The Open AI API key. You can also set the environment variable {ENV_VARIABLE_OAI_KEY}=key.",
+        help=f"The specific Open AI model to be used. Default is '{DEFAULT_MODEL}'",
     )
     parser.add_argument(
         "--yoda-mode",
-        default=False,
         action="store_true",
-        help=f"Enables Master Yoda mode. You can set the environment variable {ENV_VARIABLE_YODA_MODE}=true.",
+        default=False,
+        help=f"Enables Master Yoda mode.",
     )
     parsed, user_query = parser.parse_known_args()
-
-    is_debug: bool = parsed.debug
-    model: OpenAiModel = parsed.model
-    oai_key = parsed.open_ai_key or os.environ.get(ENV_VARIABLE_OAI_KEY)
-    yoda_mode = parsed.yoda_mode or os.environ.get(ENV_VARIABLE_YODA_MODE) == "true"
-
-    log.setLevel(logging.DEBUG if is_debug else logging.WARNING)
-    log.debug(f"arguments: {is_debug = }, {model = }, {yoda_mode = }. {user_query}")
-
-    if not oai_key:
-        log.error(
-            f" Open AI key is missing. Please set the '{ENV_VARIABLE_OAI_KEY}' "
-            "environment variable, or as a command parameter."
-        )
-        sys.exit(-1)
-    if not user_query:
-        log.debug(" No question or comment provided to zed.")
-        print(zed_ascii)
-        parser.print_help()
-        sys.exit(0)
-
-    formatted_input = " ".join(user_query)
-    success = asyncio.run(
-        zed.run(
-            log=log,
-            oai_key=oai_key,
-            model=model,
-            user_query=formatted_input,
-            yoda_mode=yoda_mode,
-        )
+    formatted_query = " ".join(user_query)
+    settings = merge_with_local_settings(
+        model=parsed.model,
+        is_debug=parsed.debug,
+        yoda_mode=parsed.yoda_mode,
     )
-    sys.exit(0 if success else -1)
+    return formatted_query, settings
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `zed_assistant-0.0.3/zed_assistant/model/cli_prompt/defs.py` & `zed_assistant-0.0.4/zed_assistant/model/command_prompt/defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,28 @@
-from dataclasses import asdict, dataclass
+from dataclasses import dataclass
 from enum import Enum
-from typing import Optional
 
 from zed_assistant.model.defs import PromptTemplateValues
 
 
 class CliCommandType(str, Enum):
     COMMAND = "COMMAND"
     CONFIRM = "CONFIRM"
     ANSWER = "ANSWER"
 
 
 class OperatingSystem(str, Enum):
     MAC_OS = "Mac OS"
     UBUNTU = "Ubuntu"
-    ARCH = "Arch Linux"
-
-
-##
-# Cli prompt runner input and output
-##
 
 
 @dataclass
-class CliPromptInput:
+class CommandPromptInput:
     input: str
-    operating_system: OperatingSystem
     yoda_mode: bool
-
-
-@dataclass
-class CliPromptOutput:
-    answer: Optional[str] = None
-    command: Optional[str] = None
-    needs_confirmation: bool = True
-
-
-##
-# Cli prompt template values
-##
+    operating_system: OperatingSystem
 
 
 @dataclass
 class SystemTemplateValues(PromptTemplateValues):
     operating_system: str
     yoda_mode: bool
```

### Comparing `zed_assistant-0.0.3/zed_assistant/model/cli_prompt/runner.py` & `zed_assistant-0.0.4/zed_assistant/model/command_prompt/prompt_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,82 @@
 from logging import Logger
 from typing import List, Optional
 
+from jinja2 import Template
 from openai import AsyncOpenAI
 
-from zed_assistant.constants import OpenAiModel
-from zed_assistant.model.defs import OpenAIMessage, Settings
-from zed_assistant.utils.render_utils import render_template
-
-from .defs import (CliCommandType, CliPromptInput, CliPromptOutput,
-                   SystemTemplateValues)
-
-
-class Runner:
-    def __init__(self, log: Logger, client: AsyncOpenAI, model: OpenAiModel):
+from zed_assistant.model.defs import (
+    ModelSettings,
+    OpenAIMessage,
+    OpenAiModel,
+    ZedAnswer,
+)
+from zed_assistant.utils.file_utils import read_file_contents
+
+from .defs import CliCommandType, CommandPromptInput, SystemTemplateValues
+
+
+class CommandPromptRunner:
+    def __init__(
+        self,
+        log: Logger,
+        client: AsyncOpenAI,
+        model: OpenAiModel,
+    ):
         self.log = log
         self.client = client
-        self.settings = Settings(
+        self.template_system = read_file_contents(
+            folder_path=__file__,
+            file_name="template_system.j2",
+        )
+        self.model_settings = ModelSettings(
             model=model,
             max_tokens=64,
             temperature=0.0,
             stream=False,
         )
 
-    async def run_prompt(
-        self, prompt_input: CliPromptInput
-    ) -> Optional[CliPromptOutput]:
-        self.log.debug(f"Calling OpenAI with args {self.settings.to_dict()}")
+    async def run_prompt(self, prompt_input: CommandPromptInput) -> Optional[ZedAnswer]:
+        self.log.debug(f"Calling OpenAI with args {self.model_settings.to_dict()}")
         result = await self.client.chat.completions.create(
-            **self.settings.to_dict(),
-            messages=self._build_messages(prompt_input=prompt_input),
+            **self.model_settings.to_dict(),
+            messages=self._build_prompt_messages(prompt_input=prompt_input),
         )
 
         self.log.debug(f"Full OAI {result = }")
         if result.usage:
             # TODO log usage.prompt_tokens and usage.completition_tokens
             ...
         choices = result.choices
         if not choices or not choices[0].message or not choices[0].message.content:
             self.log.warning(f"Warning: bad OpenAI result: {result}")
             return None
 
         return self._parse_result(result=result.choices[0].message.content)
 
-    def _build_messages(self, prompt_input: CliPromptInput) -> List[OpenAIMessage]:
+    def _build_prompt_messages(
+        self, prompt_input: CommandPromptInput
+    ) -> List[OpenAIMessage]:
         system_template_values = SystemTemplateValues(
-            operating_system=prompt_input.operating_system,
+            operating_system=prompt_input.operating_system.value,
             yoda_mode=prompt_input.yoda_mode,
+        ).to_dict()
+        rendered_system_prompt = Template(self.template_system).render(
+            system_template_values
         )
-        rendered_system_prompt = render_template(
-            origin_path=__file__,
-            template_name="template_system",
-            data=system_template_values.to_dict(),
-        )
-        self.log.debug(f" {rendered_system_prompt = }")
+        self.log.debug(f"{system_template_values = } {rendered_system_prompt = }")
         return [
             # TODO add previous assistant and user exchanges for?
             OpenAIMessage(role="system", content=rendered_system_prompt),
             OpenAIMessage(role="user", content=prompt_input.input),
         ]
 
-    def _parse_result(self, result: str) -> Optional[CliPromptOutput]:
+    def _parse_result(self, result: Optional[str]) -> Optional[ZedAnswer]:
+        if not result:
+            return None
         result_by_line = result.split("\n")
         self.log.debug(f"_parse_result(): {result_by_line = }")
         answer: Optional[str] = None
         command: Optional[str] = None
         included_confirm = False
         needs_confirmation = False
 
@@ -80,12 +93,12 @@
         if not answer and not command:
             return None
         if command and not included_confirm:
             self.log.warning(
                 "Error! Answer included a COMMAND, but no CONFIRM instruction"
             )
             return None
-        return CliPromptOutput(
+        return ZedAnswer(
             answer=answer,
             command=command,
             needs_confirmation=needs_confirmation,
         )
```

### Comparing `zed_assistant-0.0.3/zed_assistant/model/cli_prompt/template_system.j2` & `zed_assistant-0.0.4/zed_assistant/model/command_prompt/template_system.j2`

 * *Files identical despite different names*

### Comparing `zed_assistant-0.0.3/zed_assistant/utils/console.py` & `zed_assistant-0.0.4/zed_assistant/utils/console.py`

 * *Files identical despite different names*

### Comparing `zed_assistant-0.0.3/zed_assistant/zed.py` & `zed_assistant-0.0.4/zed_assistant/zed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 import os
 from logging import Logger
 
 from openai import AsyncOpenAI
 
-from zed_assistant.constants import OpenAiModel
-from zed_assistant.model.cli_prompt import (CliPromptInput, OperatingSystem,
-                                            Runner)
+from zed_assistant.model.command_prompt import (
+    CommandPromptInput,
+    CommandPromptRunner,
+    OperatingSystem,
+)
+from zed_assistant.settings.defs import ZedSettings
 from zed_assistant.utils import Console
 
 
-async def run(
-    log: Logger,
-    oai_key: str,
-    model: OpenAiModel,
-    user_query: str,
-    yoda_mode: bool = False,
-) -> bool:
-    """
-    Main Zed executor.
-    """
-    console = Console()
-    console.show_spinner()
-
-    runner = Runner(
-        log=log,
-        client=AsyncOpenAI(api_key=oai_key),
-        model=model,
-    )
-    cli_prompt_output = await runner.run_prompt(
-        CliPromptInput(
-            input=user_query,
-            yoda_mode=yoda_mode,
-            operating_system=OperatingSystem.MAC_OS,
-        ),
-    )
-    console.hide_spinner()
-    log.debug(f"Runner result: {cli_prompt_output = }")
-
-    if not cli_prompt_output:
-        console.print_retry()
-        return False
-
-    if cli_prompt_output.answer:
-        console.print_answer(cli_prompt_output.answer)
-    if not cli_prompt_output.command:
-        return True
-
-    console.print_command(cli_prompt_output.command)
-    confirmed = console.await_confirmation()
-    if confirmed:
-        log.info(f"RUNNING {cli_prompt_output.command}")
-        console.print_run_command(cli_prompt_output.command)
-        command_result = os.system(cli_prompt_output.command)
-        return command_result == 0
-    else:
-        console.print_farewell()
-        return True
+class Zed:
+    def __init__(self, settings: ZedSettings, log: Logger):
+        self.log = log
+        self.console = Console()
+        self.settings = settings
+        self.command_prompt_runner = CommandPromptRunner(
+            log=log,
+            client=AsyncOpenAI(api_key=settings.openai_key),
+            model=settings.model,
+        )
+
+    async def run(self, user_query: str) -> bool:
+        """
+        Main Zed executor.
+        """
+        self.console.show_spinner()
+        cli_prompt_output = await self.command_prompt_runner.run_prompt(
+            CommandPromptInput(
+                input=user_query,
+                operating_system=OperatingSystem.MAC_OS,
+                yoda_mode=self.settings.yoda_mode,
+            ),
+        )
+        self.console.hide_spinner()
+        self.log.debug(f"Runner result: {cli_prompt_output = }")
+
+        if not cli_prompt_output:
+            self.console.print_retry()
+            return False
+
+        if cli_prompt_output.answer:
+            self.console.print_answer(cli_prompt_output.answer)
+        if not cli_prompt_output.command:
+            return True
+
+        self.console.print_command(cli_prompt_output.command)
+        confirmed = self.console.await_confirmation()
+        if confirmed:
+            self.log.info(f"RUNNING {cli_prompt_output.command}")
+            self.console.print_run_command(cli_prompt_output.command)
+            command_result = os.system(cli_prompt_output.command)
+            return command_result == 0
+        else:
+            self.console.print_farewell()
+            return True
```

### Comparing `zed_assistant-0.0.3/PKG-INFO` & `zed_assistant-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zed-assistant
-Version: 0.0.3
+Version: 0.0.4
 Summary: Zed is an LLM-based CLI assistant built with python and Chat GPT
 Home-page: https://github.com/hoffmannmatheus/zed
 License: MIT
 Author: Matheus Hoffmann Silva
 Author-email: me@mhsilva.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,69 +20,74 @@
 Project-URL: Repository, https://github.com/hoffmannmatheus/zed
 Description-Content-Type: text/markdown
 
 
 # Overview 
 A helpful command line assistant, based on ChatGPT.
 
-# Getting started
+## Getting started
 Install Zed by running: 
 ```bash
 pip install zed-assistant
 ```
 Note that Zed requires Python 3.8+.
 
-You'll need your own OpenAI key to be able to use Zed. The key can be configured as an environment variable or  passed as a command parameter:
-```
-echo "export ZED_OAI_KEY=my-key" >> ~/.zshrc  # or .bash_profile, etc
-```
+You'll need your own OpenAI key to be able to use Zed. See "Configure" below to know how.
 
-# Usage
+## Usage
 Run `zed` with no arguments to get the help menu:
 ```
 ~ zed
-
      ______ ___________
     |___  /|  ___|  _  \
        / / | |__ | | | |
       / /  |  __|| | | |
     ./ /___| |___| |/ /
-    \_____/\____/|___/
+    \_____/\____/|___/  v0.0.4
 
-usage: zed [-h] [--debug] [--model {gpt-4,gpt-4-turbo,gpt-3.5-turbo}] [--open-ai-key OPEN_AI_KEY]
+usage: zed [-h] [--version] [--debug] [--model {gpt-4o,gpt-4-turbo,gpt-3.5-turbo}] [--yoda-mode]
 
-zed is a LLM-based CLI assistant built with python and Chat GPT
+zed is a LLM-based CLI assistant.
 
 optional arguments:
   -h, --help            show this help message and exit
+  --version             show program's version number and exit
   --debug               Enables print debug logs.
-  --model {gpt-4,gpt-4-turbo,gpt-3.5-turbo}
-                        The specific Open AI model to be used. Default is 'gpt-4-turbo'.
-  --open-ai-key OPEN_AI_KEY
-                        The Open AI API key. You can also set the environment variable ZED_OAI_KEY.
+  --model {gpt-4o,gpt-4-turbo,gpt-3.5-turbo}
+                        The specific Open AI model to be used. Default is 'gpt-4o'
+  --yoda-mode           Enables Master Yoda mode.
+```
+
+## Configure
+After you run `zed` for the first time, a default configuration file is created. To include your Open AI key, or 
+change other settings, edit the `~/.zed/config` file:
+```bash
+openai_key=<YOUR_OPEN_AI_KEY>
+model=gpt-4-turbo
+debug=False
+yoda_mode=False
 ```
 
+
+
 # Contributing 
 ## Install dependencies
 Setup the project locally:
 ```bash
 git clone https://github.com/hoffmannmatheus/zed/ && cd zed
 poetry install
 ```
 
 ## Run tests
 ```bash
 poetry run pytest
 ```
 
 ## Run zed locally
-First, setup your local OpenAI API key: 
-```bash
-export ZED_OAI_KEY="your-openai-key"
-```
+First, setup your local OpenAI API in the `~/.zed/config` file. 
 Then, run locally with:
 ```bash
 poetry run zed
 ```
 
 ## Publishing a new version
 ```bash
```

