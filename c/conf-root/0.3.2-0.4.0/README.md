# Comparing `tmp/conf_root-0.3.2.tar.gz` & `tmp/conf_root-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_root-0.3.2.tar", last modified: Wed May 22 08:56:27 2024, max compression
+gzip compressed data, was "conf_root-0.4.0.tar", last modified: Tue May 28 16:42:15 2024, max compression
```

## Comparing `conf_root-0.3.2.tar` & `conf_root-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 08:56:23.000000 conf_root-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-22 08:56:27.499952 conf_root-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-22 08:56:23.000000 conf_root-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.495952 conf_root-0.3.2/conf_root/
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/ConfRoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/conf_root/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/BasicAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/JsonAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/SingleFileYamlAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/YamlAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/conf_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:56:27.499952 conf_root-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-22 08:56:23.000000 conf_root-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_multi_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_nested_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_single_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 16:42:10.000000 conf_root-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-28 16:42:15.422658 conf_root-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-28 16:42:10.000000 conf_root-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.418658 conf_root-0.4.0/conf_root/
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/ConfRoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/conf_root/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/BasicAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/JsonAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/YamlAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/conf_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 16:42:10.000000 conf_root-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:42:15.422658 conf_root-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-28 16:42:10.000000 conf_root-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_ConfigurationField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_multi_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_nested_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_single_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_wrap.py
```

### Comparing `conf_root-0.3.2/LICENSE` & `conf_root-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.2/PKG-INFO` & `conf_root-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,77 @@
-Metadata-Version: 2.1
-Name: conf_root
-Version: 0.3.2
-Summary: 基于dataclass的符合逻辑的配置取用方式。
-Home-page: https://github.com/ciaranchen/conf_root
-Author: ciaranchen
-Author-email: ciaranchen@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ruamel.yaml
-
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
-基于dataclass的符合逻辑的配置文件取用方式。主要功能如下：
+基于dataclass的符合逻辑的配置文件取用方式。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
-1. 封装dataclass到配置文件。
-2. 将argparse的设置转换为配置文件。这允许在科研项目的代码中能快速地通过配置文件运行代码。
+1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
+2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
 
 > Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
 
-## 封装dataclass
+## 装饰类的定义生成配置文件
+
+项目使用dataclass对配置类进行封装，并产生配置文件。
+
+> note: 类定义的字段需要类型注解。如果不指定字段类型，将被视为类变量而不会被解析为dataclass中的字段，也无法被这个类进行解析。
+
+下面是一个对`AppConfig`进行封装
 
 ```python
 from conf_root import ConfRoot
-from dataclasses import dataclass
 
 
-# @ConfRoot().wrap(name='config')
-# @ConfRoot().wrap
+# @ConfRoot().config(name='config')
+# @ConfRoot().config
 # 这个装饰器也支持上面这两种调用方式
-@ConfRoot().wrap('config')
-@dataclass
+@ConfRoot().config('config')
 class AppConfig:
     database_host: str = 'localhost'
     database_port: int = 5432
 
 
-# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`)。
-# 如不存在则按照默认值新建文件（或在文件中添加字段）。
+# 在类实例化时，检测是否存在配置文件(文件名为name+后缀)。
+# 如不存在则新建文件。
 # 如存在配置文件，则加载文件中的配置。
 app_config = AppConfig()
 ```
 
-> note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
-
 ### 参数解释
 
-#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
 - agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
     - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
-- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
 
-#### `ConfRoot.wrap`
+#### `ConfRoot.config`
 
 可以使用不同方式调用。详见上方示例。
 
-- name。该配置在path中的位置。
+- name。该配置在path中的位置。默认为 `{cls.__qual_name__}`。
     - 对于多文件存储，name为文件名。指定时可以带上agent相应的后缀名。
     - 对于单文件存储，name为在文件中的section名。
+- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
+
+### 对field的拓展说明
+
+dataclass中的field可以通过metadata进行拓展。
+
+- comment: 注释。仅在Yaml的输出格式中有效。为导出文件中当前字段的行添加行内注释。
+- serialize: 自定义序列化函数。接受序列化字段的值，返回序列化的文本。
+- deserialize: 自定义反序列化函数。接受序列化后的文本，返回该字段应有的值。
+- validators: 函数的列表。在反序列化时，对获得的值依次校验；如不符合要求抛出 ValidateException.
 
 ## 解析 Argparse
 
-在科研项目中会出现一大堆parser.argument，我希望能将它们转换为配置文件，而不是每次都要记录运行时的命令行参数。
+在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`或者`run.bat`。
 
 ```python
 import argparse
 from conf_root import ConfRoot
 
 # 科研项目经常出现一大堆parser.argument
 parser = argparse.ArgumentParser()
@@ -111,30 +107,34 @@
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
-from dataclasses import dataclass, field
+from dataclasses import field
+from typing import List
 
 
-@ConfRoot(agent_class=None).wrap
-@dataclass
+@ConfRoot(agent_class=None).config
 class DataBaseUserConfig:
-  database_user: str = 'admin'
-  database_password: str = 'default_password'
+    database_user: str = 'admin'
+    database_password: str = 'default_password'
 
 
-@ConfRoot(agent_class=JsonAgent).wrap
+@ConfRoot(agent_class=JsonAgent).config
 # 可通过agent_class指定配置文件格式
 # 此时默认配置文件名为 `config.json`
-@dataclass
 class AppConfig:
-  database_host: str = 'localhost'
-  database_port: int = 5432
-  # 可嵌套dataclass定义
-  user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+    database_host: str = 'localhost'
+    database_port: int = 5432
+    # 可嵌套定义, 支持使用dataclasses的field。
+    user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+    # 使用 config_field，支持dataclasses.field 的所有参数；同时可以自定义serialize方式与deserialize方法
+    user_list: List = field(default_factory=list, metadata={
+        'serialize': lambda xs: ','.join([x.lower() for x in xs]),
+        'deserialize': lambda s: [x.upper() for x in s.split(',')]
+    })
 
 
 app_config = AppConfig()
 ```
```

### Comparing `conf_root-0.3.2/README.md` & `conf_root-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,90 @@
+Metadata-Version: 2.1
+Name: conf_root
+Version: 0.4.0
+Summary: Default template for PDM package
+Home-page: https://github.com/ciaranchen/conf_root
+Author: ciaranchen
+Author-email: ciaranchen <ciaranchen@qq.com>
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ruamel-yaml>=0.18.6
+
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
-基于dataclass的符合逻辑的配置文件取用方式。主要功能如下：
+基于dataclass的符合逻辑的配置文件取用方式。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
-1. 封装dataclass到配置文件。
-2. 将argparse的设置转换为配置文件。这允许在科研项目的代码中能快速地通过配置文件运行代码。
+1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
+2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
 
 > Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
 
-## 封装dataclass
+## 装饰类的定义生成配置文件
+
+项目使用dataclass对配置类进行封装，并产生配置文件。
+
+> note: 类定义的字段需要类型注解。如果不指定字段类型，将被视为类变量而不会被解析为dataclass中的字段，也无法被这个类进行解析。
+
+下面是一个对`AppConfig`进行封装
 
 ```python
 from conf_root import ConfRoot
-from dataclasses import dataclass
 
 
-# @ConfRoot().wrap(name='config')
-# @ConfRoot().wrap
+# @ConfRoot().config(name='config')
+# @ConfRoot().config
 # 这个装饰器也支持上面这两种调用方式
-@ConfRoot().wrap('config')
-@dataclass
+@ConfRoot().config('config')
 class AppConfig:
     database_host: str = 'localhost'
     database_port: int = 5432
 
 
-# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`)。
-# 如不存在则按照默认值新建文件（或在文件中添加字段）。
+# 在类实例化时，检测是否存在配置文件(文件名为name+后缀)。
+# 如不存在则新建文件。
 # 如存在配置文件，则加载文件中的配置。
 app_config = AppConfig()
 ```
 
-> note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
-
 ### 参数解释
 
-#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
 - agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
     - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
-- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
 
-#### `ConfRoot.wrap`
+#### `ConfRoot.config`
 
 可以使用不同方式调用。详见上方示例。
 
-- name。该配置在path中的位置。
+- name。该配置在path中的位置。默认为 `{cls.__qual_name__}`。
     - 对于多文件存储，name为文件名。指定时可以带上agent相应的后缀名。
     - 对于单文件存储，name为在文件中的section名。
+- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
+
+### 对field的拓展说明
+
+dataclass中的field可以通过metadata进行拓展。
+
+- comment: 注释。仅在Yaml的输出格式中有效。为导出文件中当前字段的行添加行内注释。
+- serialize: 自定义序列化函数。接受序列化字段的值，返回序列化的文本。
+- deserialize: 自定义反序列化函数。接受序列化后的文本，返回该字段应有的值。
+- validators: 函数的列表。在反序列化时，对获得的值依次校验；如不符合要求抛出 ValidateException.
 
 ## 解析 Argparse
 
-在科研项目中会出现一大堆parser.argument，我希望能将它们转换为配置文件，而不是每次都要记录运行时的命令行参数。
+在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`或者`run.bat`。
 
 ```python
 import argparse
 from conf_root import ConfRoot
 
 # 科研项目经常出现一大堆parser.argument
 parser = argparse.ArgumentParser()
@@ -96,30 +120,34 @@
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
-from dataclasses import dataclass, field
+from dataclasses import field
+from typing import List
 
 
-@ConfRoot(agent_class=None).wrap
-@dataclass
+@ConfRoot(agent_class=None).config
 class DataBaseUserConfig:
-  database_user: str = 'admin'
-  database_password: str = 'default_password'
+    database_user: str = 'admin'
+    database_password: str = 'default_password'
 
 
-@ConfRoot(agent_class=JsonAgent).wrap
+@ConfRoot(agent_class=JsonAgent).config
 # 可通过agent_class指定配置文件格式
 # 此时默认配置文件名为 `config.json`
-@dataclass
 class AppConfig:
-  database_host: str = 'localhost'
-  database_port: int = 5432
-  # 可嵌套dataclass定义
-  user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+    database_host: str = 'localhost'
+    database_port: int = 5432
+    # 可嵌套定义, 支持使用dataclasses的field。
+    user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+    # 使用 config_field，支持dataclasses.field 的所有参数；同时可以自定义serialize方式与deserialize方法
+    user_list: List = field(default_factory=list, metadata={
+        'serialize': lambda xs: ','.join([x.lower() for x in xs]),
+        'deserialize': lambda s: [x.upper() for x in s.split(',')]
+    })
 
 
 app_config = AppConfig()
 ```
```

### Comparing `conf_root-0.3.2/conf_root/ConfRoot.py` & `conf_root-0.4.0/conf_root/ConfRoot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,125 +1,134 @@
 import argparse
-from dataclasses import make_dataclass, is_dataclass, MISSING, dataclass
+from dataclasses import make_dataclass, is_dataclass, MISSING, dataclass, field as dataclass_field
 from pathlib import Path
-from typing import Optional, Type
+from typing import Optional, Type, List
 import logging
 
 from conf_root.Configuration import Configuration
 from conf_root.agents.BasicAgent import BasicAgent
 from conf_root.agents.YamlAgent import YamlAgent
 
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
                     datefmt='%m-%d %H:%M:%S')
 logger = logging.getLogger(__name__)
 
 
 class ConfRoot:
-    def __init__(self, path: str = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False):
+    def __init__(self, path: str = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent):
         self.path = Path(path) if path is not None else Path()
         self.agent_class = agent_class
         self.persist = (agent_class is not None)
         if self.persist:
             self.agent = self.agent_class(self.path)
-        self.dynamic = dynamic
 
-    def wrap(self, *args, **kwargs):
-        def decorator(cls, name: Optional[str] = None):
+    def config(self, *args, **kwargs):
+        def decorator(cls, name: Optional[str] = None, dynamic=False):
             if not is_dataclass(cls):
                 logger.debug(f'decorate class {cls.__qualname__} to dataclass...')
                 cls = dataclass(cls)
             if name is None:
                 name = cls.__qualname__.replace('<locals>.', '')
 
-            configuration = Configuration.from_wrapper(cls, name)
+            configuration = Configuration(name, cls)
             setattr(cls, '__CONF_ROOT__', configuration)
 
             # 覆盖其 __init__ 函数
             origin_init = cls.__init__
 
             def decorated_init(_self, *args, **kwargs):
                 origin_init(_self, *args, **kwargs)
                 self.post_init(_self, configuration)
 
             decorated_init.__name__ = '__init__'
             cls.__init__ = decorated_init
-            if self.persist and self.dynamic:
+            if self.persist and dynamic:
                 def save(_self):
                     return self.agent.save(configuration, _self)
 
                 def load(_self):
-                    data = self.agent.load(configuration)
-                    configuration.data2obj(_self, data)
+                    return self.agent.load(configuration, _self)
 
                 cls.save = save
                 cls.load = load
             return cls
 
         if len(args) == 1 and isinstance(args[0], type):
             # 无参数情况下，相当于直接用类的定义调用decorator.
             # @wrap
             return decorator(args[0], **kwargs)
         if len(args) >= 1:
             # 有args的情况下，取第一个args为 config 名称。
             # @wrap('config'）
-            return lambda cls: decorator(cls, args[0])
+            return lambda cls: decorator(cls, *args, **kwargs)
         # 无args, 只有kwargs的情况下，直接给出decorator
         # @wrap() or @wrap(name='config')
         return lambda cls: decorator(cls, **kwargs)
 
     def post_init(self, instance, configuration):
         if self.persist:
             if self.agent.exist(configuration):
                 # 如果已存在，读取和实例化
-                data = self.agent.load(configuration)
-                configuration.data2obj(instance, data)
+                self.agent.load(configuration, instance)
             else:
                 # 若文件不存在，根据默认值创建
-                self.agent.create(configuration)
+                self.agent.save(configuration, instance)
 
-    def from_argparse(self, parser: argparse.ArgumentParser, cls_name: str = 'argparse'):
+    def from_argparse(self, parser: argparse.ArgumentParser, cls_name: str = 'ArgparseConfig'):
         def get_default(action):
-            if isinstance(action, argparse._StoreConstAction):
-                return action.const
-            if action.default:
+            if action.default and action.default != argparse.SUPPRESS:
                 return action.default
-            if action.const:
+            if action.const and isinstance(action, argparse._StoreConstAction):
                 return action.const
-            return MISSING
+            # 如果是Required的话，那么传入的参数中必定有它，所以不必有default。
+            return MISSING if action.required else None  # 实在没有default的话，就先给None了
 
         def get_type(action):
             if action.type:
                 return action.type
+            if action.nargs and action.nargs != '?':
+                return List
+            if (isinstance(action, argparse._AppendAction) or
+                    isinstance(action, argparse._AppendConstAction) or isinstance(action, argparse._ExtendAction)):
+                return List
             default = get_default(action)
             if default:
                 return type(default)
 
+        def default_field(action):
+            metadata = {'validators': []}
+            if action.help:
+                metadata['comment'] = action.help
+            # validators
+            if action.choices:
+                metadata['validators'].append(lambda x: x in action.choices)
+            if action.nargs:
+                if isinstance(action.nargs, int):
+                    metadata['validators'].append(lambda x: len(x) == action.nargs)
+                if action.nargs == '+':
+                    metadata['validators'].append(lambda x: len(x) > 0)
+            return dataclass_field(default=get_default(action), metadata=metadata)
+
         fields = []
         for action in parser._actions:
             name = action.dest
-            if name == 'help':
+            if isinstance(action, argparse._HelpAction) or isinstance(action, argparse._VersionAction):
                 continue
-            if not (isinstance(action, argparse._StoreAction)
-                    or isinstance(action, argparse._StoreFalseAction)
-                    or isinstance(action, argparse._StoreTrueAction)
-                    or isinstance(action, argparse._StoreConstAction)):
+            _SUPPORT_ACTIONS = [
+                argparse._AppendAction, argparse._AppendConstAction, argparse._CountAction, argparse._ExtendAction,
+                argparse._StoreAction, argparse._StoreConstAction, argparse._StoreFalseAction, argparse._StoreTrueAction
+            ]
+            if not any([isinstance(action, sa) for sa in _SUPPORT_ACTIONS]):
+                logger.warning(f'Skiped Argparse: {action.dest} action {action.__class__.__name__}')
                 # 暂不考虑不支持的action
                 continue
-            if action.nargs not in [None, 0, 1]:
-                # 暂不考虑多参数的情况
-                continue
             # TODO: handle other Action.
 
-            if isinstance(action, argparse._StoreFalseAction):
-                field = (name, bool, False)
-            elif isinstance(action, argparse._StoreTrueAction):
-                field = (name, bool, True)
-            else:
-                default = get_default(action)
-                _type = get_type(action)
-                field = (name, _type, default)
+            _type = get_type(action)
+            field = (name, _type, default_field(action))
             fields.append(field)
+            print(field)
 
-        fields = sorted(fields, key=lambda x: x[2] == MISSING, reverse=True)
+        fields = sorted(fields, key=lambda x: x[2].default == MISSING, reverse=True)
 
         cls = make_dataclass(cls_name.replace(f'.{self.agent.default_extension}', ''), fields)
-        return self.wrap(cls_name)(cls)
+        return self.config(cls)
```

### Comparing `conf_root-0.3.2/conf_root/agents/JsonAgent.py` & `conf_root-0.4.0/conf_root/agents/JsonAgent.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-import os
-
-from conf_root.Configuration import Configuration
-from conf_root.agents.BasicAgent import BasicAgent
+from typing import Dict, Any
+from dataclasses import fields
+from conf_root.Configuration import is_config_class
+from conf_root.agents.BasicAgent import BasicAgent, MultiFileAgent
 import json
 
+from conf_root.agents.utils import data2obj
 
-class JsonAgent(BasicAgent):
-    default_extension = 'json'
-
-    def exist(self, configuration: Configuration) -> bool:
-        return self.get_configuration_location(configuration).exists()
-
-    def create(self, configuration: Configuration):
-        super().create(configuration)
-        location = self.get_configuration_location(configuration)
-        # 将默认值转换为dict，便于序列化
-        default_dict = configuration.defaults
 
-        # 将dict转换为YAML并写入文件
-        if len(default_dict.keys()) > 0:
-            with open(location, "w") as file:
-                json.dump(default_dict, file)
+class JsonAgent(BasicAgent, MultiFileAgent):
+    default_extension = '.json'
 
-    def load(self, configuration):
-        super().load(configuration)
+    def load(self, configuration, instance):
+        super().load(configuration, instance)
         location = self.get_configuration_location(configuration)
         with open(location, encoding='utf-8') as file:
             data = json.load(file)
         # 将dict展开为对象。
-        return data
+        data2obj(instance, data, custom=True)
+        return instance
 
-    def save(self, configuration, obj):
-        super().save(configuration, obj)
+    @staticmethod
+    def obj2data(obj: Any) -> Dict[str, Any]:
+        """
+        递归地将dataclass实例及其嵌套的dataclass字段转换为字典。
+        """
+        if is_config_class(obj):
+            # 对于dataclass实例，递归地处理其字段
+            res = {}
+            for field in fields(obj):
+                value = getattr(obj, field.name)
+                # 尝试获取serialize函数并调用之。
+                if 'serialize' in field.metadata and (serialize_func := field.metadata['serialize']) is not None:
+                    value = serialize_func(value)
+                    res[field.name] = value
+                    # 在进行用户自定义 serialize之后，不再进入递归。
+                    continue
+                res[field.name] = JsonAgent.obj2data(value)
+            return res
+        return obj
+
+    def save(self, configuration, instance):
+        super().save(configuration, instance)
+        data = self.obj2data(instance)
         location = self.get_configuration_location(configuration)
-        data_dict = configuration.obj2data(obj)
-        # 将dict转换为YAML并写入文件
         with open(location, "w") as file:
-            json.dump(data_dict, file)
+            json.dump(data, file)
```

### Comparing `conf_root-0.3.2/conf_root.egg-info/PKG-INFO` & `conf_root-0.4.0/conf_root.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,90 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.3.2
-Summary: 基于dataclass的符合逻辑的配置取用方式。
+Version: 0.4.0
+Summary: Default template for PDM package
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
-Author-email: ciaranchen@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Author-email: ciaranchen <ciaranchen@qq.com>
+License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: ruamel.yaml
+Requires-Dist: ruamel-yaml>=0.18.6
 
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
-基于dataclass的符合逻辑的配置文件取用方式。主要功能如下：
+基于dataclass的符合逻辑的配置文件取用方式。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
-1. 封装dataclass到配置文件。
-2. 将argparse的设置转换为配置文件。这允许在科研项目的代码中能快速地通过配置文件运行代码。
+1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
+2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
 
 > Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
 
-## 封装dataclass
+## 装饰类的定义生成配置文件
+
+项目使用dataclass对配置类进行封装，并产生配置文件。
+
+> note: 类定义的字段需要类型注解。如果不指定字段类型，将被视为类变量而不会被解析为dataclass中的字段，也无法被这个类进行解析。
+
+下面是一个对`AppConfig`进行封装
 
 ```python
 from conf_root import ConfRoot
-from dataclasses import dataclass
 
 
-# @ConfRoot().wrap(name='config')
-# @ConfRoot().wrap
+# @ConfRoot().config(name='config')
+# @ConfRoot().config
 # 这个装饰器也支持上面这两种调用方式
-@ConfRoot().wrap('config')
-@dataclass
+@ConfRoot().config('config')
 class AppConfig:
     database_host: str = 'localhost'
     database_port: int = 5432
 
 
-# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`)。
-# 如不存在则按照默认值新建文件（或在文件中添加字段）。
+# 在类实例化时，检测是否存在配置文件(文件名为name+后缀)。
+# 如不存在则新建文件。
 # 如存在配置文件，则加载文件中的配置。
 app_config = AppConfig()
 ```
 
-> note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
-
 ### 参数解释
 
-#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
 - agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
     - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
-- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
 
-#### `ConfRoot.wrap`
+#### `ConfRoot.config`
 
 可以使用不同方式调用。详见上方示例。
 
-- name。该配置在path中的位置。
+- name。该配置在path中的位置。默认为 `{cls.__qual_name__}`。
     - 对于多文件存储，name为文件名。指定时可以带上agent相应的后缀名。
     - 对于单文件存储，name为在文件中的section名。
+- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
+
+### 对field的拓展说明
+
+dataclass中的field可以通过metadata进行拓展。
+
+- comment: 注释。仅在Yaml的输出格式中有效。为导出文件中当前字段的行添加行内注释。
+- serialize: 自定义序列化函数。接受序列化字段的值，返回序列化的文本。
+- deserialize: 自定义反序列化函数。接受序列化后的文本，返回该字段应有的值。
+- validators: 函数的列表。在反序列化时，对获得的值依次校验；如不符合要求抛出 ValidateException.
 
 ## 解析 Argparse
 
-在科研项目中会出现一大堆parser.argument，我希望能将它们转换为配置文件，而不是每次都要记录运行时的命令行参数。
+在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`或者`run.bat`。
 
 ```python
 import argparse
 from conf_root import ConfRoot
 
 # 科研项目经常出现一大堆parser.argument
 parser = argparse.ArgumentParser()
@@ -111,30 +120,34 @@
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
 from conf_root import ConfRoot, JsonAgent
-from dataclasses import dataclass, field
+from dataclasses import field
+from typing import List
 
 
-@ConfRoot(agent_class=None).wrap
-@dataclass
+@ConfRoot(agent_class=None).config
 class DataBaseUserConfig:
-  database_user: str = 'admin'
-  database_password: str = 'default_password'
+    database_user: str = 'admin'
+    database_password: str = 'default_password'
 
 
-@ConfRoot(agent_class=JsonAgent).wrap
+@ConfRoot(agent_class=JsonAgent).config
 # 可通过agent_class指定配置文件格式
 # 此时默认配置文件名为 `config.json`
-@dataclass
 class AppConfig:
-  database_host: str = 'localhost'
-  database_port: int = 5432
-  # 可嵌套dataclass定义
-  user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+    database_host: str = 'localhost'
+    database_port: int = 5432
+    # 可嵌套定义, 支持使用dataclasses的field。
+    user_config: DataBaseUserConfig = field(default_factory=DataBaseUserConfig)
+    # 使用 config_field，支持dataclasses.field 的所有参数；同时可以自定义serialize方式与deserialize方法
+    user_list: List = field(default_factory=list, metadata={
+        'serialize': lambda xs: ','.join([x.lower() for x in xs]),
+        'deserialize': lambda s: [x.upper() for x in s.split(',')]
+    })
 
 
 app_config = AppConfig()
 ```
```

### Comparing `conf_root-0.3.2/setup.py` & `conf_root-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="conf_root",  # 包名
-    version="0.3.2",  # 版本号
+    version="0.4.0",  # 版本号
     install_requires=[
         "ruamel.yaml"
     ],
     author="ciaranchen",
     author_email="ciaranchen@qq.com",
     description="基于dataclass的符合逻辑的配置取用方式。",
     long_description=long_description,
```

### Comparing `conf_root-0.3.2/tests/test_argparse.py` & `conf_root-0.4.0/tests/test_argparse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import argparse
 import os
 import unittest
-import yaml
+
 from conf_root import ConfRoot
 
 
 class TestArgparse(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.location = 'argparse.yml'
+        self.location = 'ArgparseConfig.yml'
+
+        self.parser = argparse.ArgumentParser(description="Test without default value")
+        self.parser.add_argument("--default_value", default=40, type=int)
+        self.parser.add_argument("--arg1", type=int)
+        self.parser.add_argument("--arg2", type=int)
 
     def tearDown(self):
         # 这个方法将在每个测试方法结束后运行
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
@@ -28,54 +33,48 @@
         args_dataclass = ArgsClass(**vars(args_namespace))
 
         self.assertEqual(args_dataclass.arg1, 10)
         self.assertEqual(args_dataclass.arg2, 30)
 
         self.assertTrue(os.path.exists(self.location))
         with open(self.location, encoding='utf-8') as yaml_file:
-            data = yaml.safe_load(yaml_file)
-        self.assertEqual(data['arg1'], 10)
-        # 配置文件保存的是默认值 而非传入值。
-        self.assertEqual(data['arg2'], 20)
+            content = yaml_file.read()
+        self.assertTrue('arg1: 10' in content)
+        self.assertTrue('arg2: 30' in content)
 
     def test_without_default_value(self):
-        parser = argparse.ArgumentParser(description="Test without default value")
-        parser.add_argument("--default_value", default=40, type=int)
-        parser.add_argument("--arg1", type=int)
-        parser.add_argument("--arg2", type=int)
-        ArgsClass = ConfRoot().from_argparse(parser)
+        ArgsClass = ConfRoot().from_argparse(self.parser)
 
-        args_namespace = parser.parse_args(['--arg2', '30'])
+        args_namespace = self.parser.parse_args(['--arg2', '30'])
         args_dataclass = ArgsClass(**vars(args_namespace))
 
         self.assertIsNone(args_dataclass.arg1)
         self.assertEqual(args_dataclass.arg2, 30)
         self.assertEqual(args_dataclass.default_value, 40)
 
-        # 注意，因为dataclass中non-default的定义需在default的变量前，所以在ArgsClass的定义中会对他们进行排序。
-        args_dataclass2 = ArgsClass(12, 13)
-        self.assertEqual(args_dataclass2.default_value, 40)
-        self.assertEqual(args_dataclass2.arg1, 12)
-        self.assertEqual(args_dataclass2.arg2, 13)
+    def test_without_default_value2(self):
+        parser = argparse.ArgumentParser(description="Test without default value")
+        parser.add_argument("--default_value", default=40, type=int)
+        parser.add_argument("--arg1", type=int, required=True)
+        parser.add_argument("--arg2", type=int, required=True)
 
-        self.assertTrue(os.path.exists(self.location))
-        with open(self.location, encoding='utf-8') as yaml_file:
-            data = yaml.safe_load(yaml_file)
-        # 配置文件中不会保存没有默认参数的值。
-        self.assertFalse(hasattr(data, 'arg1'))
-        self.assertFalse(hasattr(data, 'arg2'))
+        ArgsClass = ConfRoot().from_argparse(parser)
+
+        # 注意，因为dataclass中non-default的定义需在default的变量前，所以在ArgsClass的定义中会将required的函数提到最前。
+        args_dataclass = ArgsClass(12, 13)
+        # print(args_dataclass)
         self.assertEqual(args_dataclass.default_value, 40)
+        self.assertEqual(args_dataclass.arg1, 12)
+        self.assertEqual(args_dataclass.arg2, 13)
 
     def test_action(self):
         parser = argparse.ArgumentParser(description="Test action")
         parser.add_argument("--verbose", action="store_true", help="Enable verbose mode")
         parser.add_argument('--foo', action='store_const', const=42)
         parser.add_argument("--items", nargs='+', type=str, help="List of items")
         parser.add_argument('--count', '-c', action='count', default=0)
         ArgsClass = ConfRoot().from_argparse(parser)
         args_dataclass = ArgsClass()
 
-        self.assertFalse(hasattr(args_dataclass, 'items'))
         self.assertFalse(hasattr(args_dataclass, 'help'))
-        self.assertFalse(hasattr(args_dataclass, 'count'))
         self.assertTrue(args_dataclass.verbose)
         self.assertEqual(args_dataclass.foo, 42)
```

### Comparing `conf_root-0.3.2/tests/test_multi_file_agent.py` & `conf_root-0.4.0/tests/test_multi_file_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 from conf_root import ConfRoot, YamlAgent, JsonAgent
 
 
 class TestYamlAgent(unittest.TestCase):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
         self.agent = YamlAgent
-        self.location = 'settings.' + self.agent.default_extension
-        self.test_load_content = "database_host: 127.0.0.1\ndatabase_port: 5432"
+        self.location = 'settings' + self.agent.default_extension
+        self.test_load_content = """!AppConfig
+database_host: 127.0.0.1
+database_port: 5432
+"""
 
     def tearDown(self):
         # 这个方法将在每个测试方法结束后运行
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
     def test_create(self):
-        @ConfRoot(agent_class=self.agent).wrap(self.location)
+        @ConfRoot(agent_class=self.agent).config(self.location)
         @dataclass
         class AppConfig:
             not_default: str
             database_host: str = 'localhost'
             database_port: int = 5432
 
         app_config = AppConfig('admin')
@@ -36,36 +39,35 @@
         # 外部修改配置文件后读取，结果应为配置文件内的设置。
         # 打开文件，读取内容
         self.assertTrue(os.path.exists(self.location))
         with open(self.location, 'r') as file:
             content = file.read()
         self.assertTrue('localhost' in content)
         self.assertTrue('5432' in content)
-        # admin 因为非默认配置，不在配置文件中。
-        self.assertFalse('admin' in content)
+        self.assertTrue('admin' in content)
 
     def test_load(self):
         content = self.test_load_content
         # 将处理后的内容写回文件（可以先备份原文件）
         with open(self.location, 'w') as file:
             file.write(content)
 
-        @ConfRoot(agent_class=self.agent).wrap(self.location)
+        @ConfRoot(agent_class=self.agent).config(self.location, dynamic=True)
         @dataclass
         class AppConfig:
             not_default: str
             database_host: str = 'localhost'
             database_port: int = 5432
 
         app_config = AppConfig('admin')
         self.assertEqual(app_config.database_host, '127.0.0.1')
         self.assertEqual(app_config.database_port, 5432)
 
     def test_save(self):
-        @ConfRoot(agent_class=self.agent).wrap(self.location)
+        @ConfRoot(agent_class=self.agent).config(self.location, dynamic=True)
         @dataclass
         class AppConfig:
             not_default: str
             database_host: str = 'localhost'
             database_port: int = 5432
 
         app_config = AppConfig('admin')
@@ -83,9 +85,9 @@
         self.assertTrue('admin' in content)
 
 
 class TestJsonConfig(TestYamlAgent):
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
         self.agent = JsonAgent
-        self.location = 'settings.' + self.agent.default_extension
+        self.location = 'settings' + self.agent.default_extension
         self.test_load_content = """{"database_host": "127.0.0.1", "database_port": 5432}"""
```

### Comparing `conf_root-0.3.2/tests/test_nested_dataclass.py` & `conf_root-0.4.0/tests/test_nested_dataclass.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import unittest
 from dataclasses import dataclass, field as dataclass_field
 
 from conf_root import ConfRoot
 
 
-@ConfRoot(agent_class=None).wrap()
+@ConfRoot(agent_class=None).config()
 @dataclass
 class NestedConfig:
     config1: str = 'nest_config1'
     config2: str = 'nest_config2'
 
 
 @dataclass
@@ -28,54 +28,54 @@
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
     def test_create(self):
-        DecoratedConfig = ConfRoot().wrap(self.location)(AppConfig)
+        DecoratedConfig = ConfRoot().config(self.location)(AppConfig)
         app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
         self.assertEqual(app_config.nc_default.config1, 'nest_config1')
         self.assertEqual(app_config.nc_default.config2, 'nest_config2')
 
         self.assertEqual(app_config.nc_defined.config1, 'defined1')
         self.assertEqual(app_config.nc_defined.config2, 'defined2')
         # print(app_config.__CONF_ROOT__.defaults)
         # 外部修改配置文件后读取，结果应为配置文件内的设置。
         # 打开文件，读取内容
         self.assertTrue(os.path.exists(self.location))
         with open(self.location, 'r') as file:
             content = file.read()
         self.assertTrue('nest_config1' in content)
         self.assertTrue('nest_config2' in content)
-        # defined 因为非默认配置，不在配置文件中。
-        self.assertFalse('defined1' in content)
-        self.assertFalse('defined2' in content)
+        self.assertTrue('defined1' in content)
+        self.assertTrue('defined2' in content)
 
     def test_load(self):
-        content = """nc_default:
-    config1: default_load1
-nc_defined:
-    config1: load1
-    config2: load2"""
+        content = """!AppConfig
+nc_default: !NestedConfig
+  config1: default_load1
+nc_defined: !NestedConfig
+  config1: load1
+  config2: load2"""
 
         # 将处理后的内容写回文件（可以先备份原文件）
         with open(self.location, 'w') as file:
             file.write(content)
 
-        DecoratedConfig = ConfRoot().wrap(self.location)(AppConfig)
+        DecoratedConfig = ConfRoot().config(self.location, dynamic=True)(AppConfig)
         app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
         self.assertEqual(app_config.nc_default.config1, 'default_load1')
         self.assertEqual(app_config.nc_default.config2, 'nest_config2')
 
         self.assertEqual(app_config.nc_defined.config1, 'load1')
         self.assertEqual(app_config.nc_defined.config2, 'load2')
 
     def test_save(self):
-        DecoratedConfig = ConfRoot().wrap(self.location)(AppConfig)
+        DecoratedConfig = ConfRoot().config(self.location, dynamic=True)(AppConfig)
         app_config = DecoratedConfig(NestedConfig(config1='defined1', config2='defined2'))
         app_config.nc_default.config1 = 'save_default'
         app_config.nc_defined.config1 = 'save_defined'
         app_config.save()
 
         # 外部修改配置文件后读取，结果应为配置文件内的设置。
         # 打开文件，读取内容
```

### Comparing `conf_root-0.3.2/tests/test_single_file_agent.py` & `conf_root-0.4.0/tests/test_single_file_agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-import unittest
-
 import os
 import unittest
 from dataclasses import dataclass
 
-from conf_root import ConfRoot
-from conf_root.agents.SingleFileYamlAgent import SingleFileYamlAgent
+from conf_root import ConfRoot, SingleFileYamlAgent
 from tests.utils import replace_text
 
 
 class TestSingleFileYamlAgent(unittest.TestCase):
     location = 'settings.yml'
 
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
         self.conf_root = ConfRoot(self.location, agent_class=SingleFileYamlAgent)
 
-        @self.conf_root.wrap
+        @self.conf_root.config(dynamic=True)
         @dataclass
         class AppConfig:
             not_default: str
             database_host: str = 'localhost'
             database_port: int = 5432
 
-        @self.conf_root.wrap
+        @self.conf_root.config
         @dataclass
         class AppConfig2:
             one_thing: int = 42
             another_thing: int = 1024
 
         self.conf1 = AppConfig
         self.conf2 = AppConfig2
@@ -72,9 +69,7 @@
         self.assertTrue('9527' in content)
         self.assertTrue(self.section_name2 in content)
 
         replace_text(self.location, '42', '43')
         conf2 = self.conf2()
         self.assertEqual(conf2.one_thing, 43)
         self.assertEqual(conf2.another_thing, 1024)
-
-
```

### Comparing `conf_root-0.3.2/tests/test_wrap.py` & `conf_root-0.4.0/tests/test_wrap.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,56 +12,60 @@
         self.location = 'config.yml'
 
         @dataclass
         class AppConfig:
             num1: int = 42
 
         self.conf_class = AppConfig
-        self.qualname_location = 'TestWrap.__init__.AppConfig.yml'
+        self.q_location = AppConfig.__qualname__.replace('<locals>.', '') + '.yml'
 
     def tearDown(self):
         # 使用os.remove删除在测试中创建的文件
         try:
             os.remove(self.location)
         except FileNotFoundError:
             pass
 
         try:
-            os.remove(self.qualname_location)
+            os.remove(self.q_location)
         except FileNotFoundError:
             pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
 
     def test_wrap_direct(self):
-        # @ConfRoot().wrap
-        conf_class = ConfRoot().wrap(self.conf_class)
-        conf = conf_class()
-        self.assertTrue(os.path.exists(self.qualname_location))
+        # @ConfRoot().config
+        ConfRoot().config(self.conf_class)()
+        self.assertTrue(os.path.exists(self.q_location))
 
     def test_wrap_no_args(self):
-        # @ConfRoot().wrap()
-        conf_class = ConfRoot().wrap()(self.conf_class)
-        conf = conf_class()
-        self.assertTrue(os.path.exists(self.qualname_location))
+        # @ConfRoot().config()
+        ConfRoot().config()(self.conf_class)()
+        self.assertTrue(os.path.exists(self.q_location))
 
     def test_wrap_with_args(self):
-        # @ConfRoot().wrap(self.location)
-        conf_class = ConfRoot().wrap(self.location)(self.conf_class)
-        conf = conf_class()
+        # @ConfRoot().config(self.location)
+        ConfRoot().config(self.location)(self.conf_class)()
         self.assertTrue(os.path.exists(self.location))
 
     def test_wrap_with_named_args(self):
-        # @ConfRoot().wrap(self.location)
-        conf_class = ConfRoot().wrap(name=self.location)(self.conf_class)
-        conf = conf_class()
+        # @ConfRoot().config(name=self.location)
+        ConfRoot().config(name=self.location)(self.conf_class)()
         self.assertTrue(os.path.exists(self.location))
 
+    def test_wrap_dynamic(self):
+        conf = ConfRoot().config(self.location, True)(self.conf_class)()
+        self.assertTrue(os.path.exists(self.location))
+        self.assertTrue(hasattr(conf, 'save'))
+        self.assertTrue(hasattr(conf, 'load'))
+
+    def test_wrap_named_dynamic(self):
+        conf = ConfRoot().config(dynamic=True)(self.conf_class)()
+        self.assertTrue(os.path.exists(self.q_location))
+        self.assertTrue(hasattr(conf, 'save'))
+        self.assertTrue(hasattr(conf, 'load'))
+
     def test_without_dataclass(self):
-        @ConfRoot().wrap(self.location)
+        @ConfRoot().config(self.location)
         class AppConfig:
             num1: int = 42
 
         conf = AppConfig()
         self.assertTrue(os.path.exists(self.location))
-
-
-if __name__ == '__main__':
-    unittest.main()
```

