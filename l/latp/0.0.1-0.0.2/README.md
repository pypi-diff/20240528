# Comparing `tmp/latp-0.0.1.tar.gz` & `tmp/latp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latp-0.0.1.tar", last modified: Fri May 24 08:33:31 2024, max compression
+gzip compressed data, was "latp-0.0.2.tar", last modified: Tue May 28 08:03:31 2024, max compression
```

## Comparing `latp-0.0.1.tar` & `latp-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 08:33:31.241200 latp-0.0.1/
--rw-rw-rw-   0        0        0       45 2024-05-24 07:53:12.000000 latp-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      423 2024-05-24 08:33:31.241200 latp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-05-24 07:39:59.000000 latp-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-24 08:33:31.233405 latp-0.0.1/latp/
--rw-rw-rw-   0        0        0      309 2024-05-24 07:53:12.000000 latp-0.0.1/latp/__init__.py
--rw-rw-rw-   0        0        0     2012 2024-05-24 07:53:12.000000 latp-0.0.1/latp/cli.py
--rw-rw-rw-   0        0        0      654 2024-05-24 07:17:39.000000 latp-0.0.1/latp/config.yaml
--rw-rw-rw-   0        0        0     1998 2024-05-24 07:56:24.000000 latp-0.0.1/latp/decorators.py
--rw-rw-rw-   0        0        0     6158 2024-05-24 07:56:24.000000 latp-0.0.1/latp/runner.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:33:31.241200 latp-0.0.1/latp.egg-info/
--rw-rw-rw-   0        0        0      423 2024-05-24 08:33:31.000000 latp-0.0.1/latp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-05-24 08:33:31.000000 latp-0.0.1/latp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 08:33:31.000000 latp-0.0.1/latp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-24 08:33:31.000000 latp-0.0.1/latp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-24 07:53:22.000000 latp-0.0.1/latp.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-05-24 08:33:31.000000 latp-0.0.1/latp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-24 08:33:31.000000 latp-0.0.1/latp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-24 08:33:31.241200 latp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1071 2024-05-24 07:53:12.000000 latp-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-24 08:33:31.240196 latp-0.0.1/test_case/
--rw-rw-rw-   0        0        0      128 2024-05-24 08:02:17.000000 latp-0.0.1/test_case/__init__.py
--rw-rw-rw-   0        0        0      874 2024-05-24 08:05:10.000000 latp-0.0.1/test_case/test_latp1.py
--rw-rw-rw-   0        0        0     1037 2024-05-24 08:05:10.000000 latp-0.0.1/test_case/test_latp2.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:31.060366 latp-0.0.2/
+-rw-rw-rw-   0        0        0       45 2024-05-24 07:53:12.000000 latp-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      502 2024-05-28 08:03:31.060366 latp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-05-24 08:58:32.000000 latp-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:31.048798 latp-0.0.2/latp/
+-rw-rw-rw-   0        0        0      309 2024-05-28 07:49:26.000000 latp-0.0.2/latp/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-05-28 07:22:32.000000 latp-0.0.2/latp/base_request.py
+-rw-rw-rw-   0        0        0     2744 2024-05-28 07:58:35.000000 latp-0.0.2/latp/cli.py
+-rw-rw-rw-   0        0        0      654 2024-05-24 07:17:39.000000 latp-0.0.2/latp/config.yaml
+-rw-rw-rw-   0        0        0     2444 2024-05-28 06:48:58.000000 latp-0.0.2/latp/decorators.py
+-rw-rw-rw-   0        0        0     1616 2024-05-28 07:27:26.000000 latp-0.0.2/latp/exceptions.py
+-rw-rw-rw-   0        0        0     6315 2024-05-28 07:23:34.000000 latp-0.0.2/latp/http_request.py
+-rw-rw-rw-   0        0        0     2320 2024-05-28 07:26:13.000000 latp-0.0.2/latp/models.py
+-rw-rw-rw-   0        0        0     1019 2024-05-28 07:24:54.000000 latp-0.0.2/latp/request_manager.py
+-rw-rw-rw-   0        0        0     8181 2024-05-28 07:59:17.000000 latp-0.0.2/latp/runner.py
+-rw-rw-rw-   0        0        0     5786 2024-05-28 07:26:51.000000 latp-0.0.2/latp/utils.py
+-rw-rw-rw-   0        0        0      652 2024-05-28 07:24:23.000000 latp-0.0.2/latp/websocket_request.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:31.060366 latp-0.0.2/latp.egg-info/
+-rw-rw-rw-   0        0        0      502 2024-05-28 08:03:30.000000 latp-0.0.2/latp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-05-28 08:03:31.000000 latp-0.0.2/latp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:03:30.000000 latp-0.0.2/latp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-28 08:03:30.000000 latp-0.0.2/latp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-24 07:53:22.000000 latp-0.0.2/latp.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2024-05-28 08:03:30.000000 latp-0.0.2/latp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-28 08:03:30.000000 latp-0.0.2/latp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:03:31.060366 latp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-05-28 07:48:49.000000 latp-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:03:31.060366 latp-0.0.2/test_case/
+-rw-rw-rw-   0        0        0      128 2024-05-24 08:02:17.000000 latp-0.0.2/test_case/__init__.py
+-rw-rw-rw-   0        0        0      874 2024-05-24 08:05:10.000000 latp-0.0.2/test_case/test_latp1.py
+-rw-rw-rw-   0        0        0     1037 2024-05-24 08:05:10.000000 latp-0.0.2/test_case/test_latp2.py
```

### Comparing `latp-0.0.1/latp/cli.py` & `latp-0.0.2/latp/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,89 @@
+# cli.py
 # !/usr/bin/python3
 # -*- coding: utf-8 -*-
-# @author  : Tanyu
-# @file    : cli.py
-# @time    : 2024/5/24 下午15:46
-
 from __future__ import absolute_import
 import argparse
 import os
 import sys
 import yaml
+import logging
 from latp import __description__, __version__, __pro_name__
 from latp import runner
 
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+
 
 def load_config(config_file):
+    """
+    加载配置文件。
+
+    Args:
+        config_file: 配置文件路径。
+
+    Returns:
+        配置字典。
+    """
     if not os.path.exists(config_file):
-        # 如果指定的配置文件不存在，则使用默认配置文件
+        logger.warning(f"Config file {config_file} does not exist, using default config.yaml")
         config_file = os.path.join(os.path.dirname(__file__), 'config.yaml')
     with open(config_file, 'r', encoding='utf-8') as f:
         return yaml.safe_load(f)
 
 
 def main():
+    """
+    主函数，解析命令行参数并运行测试。
+    """
     parser = argparse.ArgumentParser(prog=__pro_name__, description=__description__)
     parser.add_argument(
         "-V", "--version", dest="version", action="store_true", help="show version")
-    parser.add_argument("-k", default=None, action="store", help="run tests which match the given substring expression")
-    parser.add_argument("-m", default=None, action="store", help="run tests with same marks")
-    parser.add_argument("-c", "--config", default=None, action="store", help="path to config file")
-    parser.add_argument("path", nargs='?', help="please input test folder", action="store")
+    parser.add_argument(
+        "-k", default=None, action="store", help="run tests which match the given substring expression")
+    parser.add_argument(
+        "-m", default=None, action="store", help="run tests with same marks")
+    parser.add_argument(
+        "-c", "--config", default=None, action="store", help="path to config file")
+    parser.add_argument(
+        "--collect-only", action="store_true", help="collect only testcase counts")
+    parser.add_argument(
+        "path", nargs='?', help="please input test folder", action="store")
 
     args = parser.parse_args()
 
-    config = load_config(args.config if args.config else 'config.yaml')
+    # 加载配置文件
+    config_path = args.config if args.config else os.path.join(os.path.dirname(__file__), 'config.yaml')
+    config = load_config(config_path)
 
     if args.version:
         print(f"{__version__}")
         sys.exit(0)
 
     test_path = args.path if args.path else config['tests']['test_path']
 
     if not test_path:
-        print("请提供测试文件夹路径，或者在配置文件中指定测试路径。")
+        logger.error("请提供测试文件夹路径，或者在配置文件中指定测试路径。")
         sys.exit(0)
 
     if not os.path.exists(test_path):
-        print(f'输入的路径不存在: {test_path}')
+        logger.error(f'输入的路径不存在: {test_path}')
+        sys.exit(0)
+
+    if args.collect_only:
+        # 统计测试用例数量
+        test_case_count = runner.count_test_cases(test_path)
+        print(f"总测试用例数量: {test_case_count}")
         sys.exit(0)
 
     if args.k:
-        print(f"测试路径: {test_path}")
-        print(f"用例过滤表达式: {args.k}")
+        logger.info(f"测试路径: {test_path}")
+        logger.info(f"用例过滤表达式: {args.k}")
     if args.m:
-        print(f"测试路径: {test_path}")
-        print(f"用例标签: {args.m}")
+        logger.info(f"测试路径: {test_path}")
+        logger.info(f"用例标签: {args.m}")
 
     runner.run(args, test_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `latp-0.0.1/latp/config.yaml` & `latp-0.0.2/latp/config.yaml`

 * *Files identical despite different names*

### Comparing `latp-0.0.1/latp/runner.py` & `latp-0.0.2/latp/runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,105 @@
+# runner.py
 # !/usr/bin/python3
 # -*- coding: utf-8 -*-
-# @author  : Tanyu
-# @file    : runner.py
-# @time    : 2024/5/24 下午15:46
-
 import inspect
 import os
 import sys
 import glob
 import pytest
 import importlib.util
 import logging
 import yaml
 import re
 
 
-# 配置日志记录
 def configure_logging(level, log_file, log_format):
-    logging.basicConfig(level=level, format=log_format, filename=log_file, filemode='w')
+    """
+    配置日志记录。
+
+    Args:
+        level: 日志级别。
+        log_file: 日志文件路径。
+        log_format: 日志格式。
+    """
+    logging.basicConfig(level=level, format=log_format, filename=log_file, encoding='utf-8', filemode='w')
     console = logging.StreamHandler()
     console.setLevel(level)
     formatter = logging.Formatter(log_format)
     console.setFormatter(formatter)
     logging.getLogger('').addHandler(console)
 
 
-# 加载配置文件
 def load_config(config_file):
+    """
+    加载配置文件。
+
+    Args:
+        config_file: 配置文件路径。
+
+    Returns:
+        配置字典。
+    """
     if not os.path.exists(config_file):
-        # 如果指定的配置文件不存在，则使用默认配置文件
         config_file = os.path.join(os.path.dirname(__file__), 'config.yaml')
     with open(config_file, 'r', encoding='utf-8') as f:
         return yaml.safe_load(f)
 
 
-# 从指定文件夹下获取模块及其所在的路径
 def find_modules_from_folder(folder, module_pattern):
+    """
+    从指定文件夹中查找符合模式的模块。
+
+    Args:
+        folder: 文件夹路径。
+        module_pattern: 模块名称匹配模式（正则表达式）。
+
+    Returns:
+        模块名称和路径的列表。
+    """
     absolute_f = os.path.abspath(folder)
     modules = glob.glob(os.path.join(absolute_f, "**", "*.py"), recursive=True)
     pattern = re.compile(module_pattern)
     return [(os.path.relpath(f, start=absolute_f)[:-3].replace(os.sep, '.'), f) for f in modules if
             os.path.isfile(f) and not f.endswith('__init__.py') and pattern.match(os.path.basename(f)[:-3])]
 
 
-# 动态导入模块
 def import_modules_dynamically(module, file_path):
+    """
+    动态导入模块。
+
+    Args:
+        module: 模块名称。
+        file_path: 文件路径。
+
+    Returns:
+        导入的模块对象。
+    """
     spec = importlib.util.spec_from_file_location(module, file_path)
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     return module
 
 
-# 测试框架的执行函数
 def run(args, test_path):
-    config = load_config(args.config if args.config else 'config.yaml')
+    """
+    运行测试。
+
+    Args:
+        args: 命令行参数。
+        test_path: 测试路径。
+    """
+    config_path = args.config if args.config else os.path.join(os.path.dirname(__file__), 'config.yaml')
+    config = load_config(config_path)
     configure_logging(config['logging']['level'], config['logging']['file'], config['logging']['format'])
     logger = logging.getLogger(__name__)
 
-    logger.info(f"加载的配置文件: {args.config if args.config else 'config.yaml'}")
+    logger.info(f"加载的配置文件: {config_path}")
     logger.info(f"测试路径: {test_path}")
 
-    # 使用配置文件中的默认值，如果没有提供命令行参数
     keyword = args.k if args.k is not None else config['tests']['keyword_expression']
     mark = args.m if args.m is not None else config['tests']['mark_expression']
 
     module_pattern = config['tests']['module_pattern']
     class_pattern = config['tests']['class_pattern']
     function_pattern = config['tests']['function_pattern']
 
@@ -82,45 +117,63 @@
         module_name, module_file = module
         logger.info(f"正在导入模块: {module_name}，路径: {module_file}")
         _module = import_modules_dynamically(module_name, module_file)
         collect_test_cases(_module, test_case_list, module_file, class_pattern, function_pattern)
 
     logger.info(f"所有找到的测试用例: {test_case_list}")
 
-    # 统一过滤
     filtered_test_cases = filter_test_cases(test_case_list, keyword, mark)
 
     if filtered_test_cases:
         logger.info(f"过滤后的测试用例: {filtered_test_cases}")
         sys.exit(run_test_case(filtered_test_cases))
     else:
         logger.info("未找到任何匹配的测试用例。")
 
 
 def collect_test_cases(_module, test_case_list, module_file, class_pattern, function_pattern):
+    """
+    收集测试用例。
+
+    Args:
+        _module: 导入的模块对象。
+        test_case_list: 测试用例列表。
+        module_file: 模块文件路径。
+        class_pattern: 类匹配模式（正则表达式）。
+        function_pattern: 函数/方法匹配模式（正则表达式）。
+    """
     module_file_path = os.path.relpath(module_file)
     class_re = re.compile(class_pattern)
     function_re = re.compile(function_pattern)
 
-    # 查找模块级别的测试函数
     for func_name, func in inspect.getmembers(_module, inspect.isfunction):
         if function_re.match(func_name):
             test_case = f"{module_file_path}::{func_name}"
             test_case_list.append((test_case, func))
 
-    # 查找类中的测试方法
     for cls_name, cls in inspect.getmembers(_module, inspect.isclass):
         if class_re.match(cls_name):
             for func_name, func in inspect.getmembers(cls, inspect.isfunction):
                 if function_re.match(func_name):
                     test_case = f"{module_file_path}::{cls_name}::{func_name}"
                     test_case_list.append((test_case, func))
 
 
 def filter_test_cases(test_case_list, keyword, mark):
+    """
+    过滤测试用例。
+
+    Args:
+        test_case_list: 测试用例列表。
+        keyword: 关键字过滤表达式。
+        mark: 标记过滤表达式。
+
+    Returns:
+        过滤后的测试用例列表。
+    """
     logger = logging.getLogger(__name__)
     filtered_cases = []
 
     for test_case, func in test_case_list:
         if keyword and keyword not in test_case:
             continue
         if mark:
@@ -131,21 +184,54 @@
                 continue
         filtered_cases.append(test_case)
 
     return filtered_cases
 
 
 def run_test_case(test_case_list):
+    """
+    运行测试用例。
+
+    Args:
+        test_case_list: 测试用例列表。
+
+    Returns:
+        pytest 的运行结果。
+    """
     logger = logging.getLogger(__name__)
     logger.info(f"本次执行用例的数量为: {len(test_case_list)}")
     extra_args_list = ["-vs", "--tb=short"] + test_case_list
     logger.info(f"运行的参数列表：{extra_args_list}")
     return pytest.main(extra_args_list)
 
 
+def count_test_cases(test_path):
+    """
+    统计测试用例数量。
+
+    Args:
+        test_path: 测试用例路径。
+
+    Returns:
+        测试用例数量。
+    """
+    config_path = os.path.join(os.path.dirname(__file__), 'config.yaml')
+    config = load_config(config_path)
+    module_list = find_modules_from_folder(test_path, config['tests']['module_pattern'])
+    test_case_count = 0
+    for module in module_list:
+        module_name, module_file = module
+        _module = import_modules_dynamically(module_name, module_file)
+        test_case_list = []
+        collect_test_cases(_module, test_case_list, module_file, config['tests']['class_pattern'],
+                           config['tests']['function_pattern'])
+        test_case_count += len(test_case_list)
+    return test_case_count
+
+
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser(description="Test Runner")
     parser.add_argument('test_path', type=str, help="Path to the test files")
     parser.add_argument('-k', type=str, help="Only run tests that match the given substring expression")
     parser.add_argument('-m', type=str, help="Only run tests that have the given mark expression")
```

### Comparing `latp-0.0.1/setup.py` & `latp-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,10 @@
+# setup.py
 # !/usr/bin/python3
 # -*- coding: utf-8 -*-
-# @author  : Tanyu
-# @file    : setup.py
-# @time    : 2024/5/24 下午15:46
-
 from setuptools import setup, find_packages
 from latp import __description__, __version__, __pro_name__
 
 # 读取 README 文件作为长描述
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
@@ -19,24 +16,26 @@
     long_description_content_type="text/markdown",
     author='Tanyu',
     author_email='cypenite@gmail.com',
     zip_safe=False,
     include_package_data=True,
     packages=find_packages(),
     license='MIT',
-    # url='http',
     entry_points={
         'console_scripts': [
             'latp = latp.cli:main'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         'pytest',
         'pyyaml',
+        'requests',
+        'loguru',
+        'pydantic'
     ],
 )
```

### Comparing `latp-0.0.1/test_case/test_latp1.py` & `latp-0.0.2/test_case/test_latp1.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.1/test_case/test_latp2.py` & `latp-0.0.2/test_case/test_latp2.py`

 * *Files identical despite different names*

