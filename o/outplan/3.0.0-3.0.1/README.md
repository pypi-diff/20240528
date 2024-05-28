# Comparing `tmp/outplan-3.0.0.tar.gz` & `tmp/outplan-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/outplan/outplan/dist/.tmp-yfgcoqid/outplan-3.0.0.tar", last modified: Tue Apr 23 12:06:04 2024, max compression
+gzip compressed data, was "/home/runner/work/outplan/outplan/dist/.tmp-wz0ddb17/outplan-3.0.1.tar", last modified: Tue May 28 08:53:01 2024, max compression
```

## Comparing `outplan-3.0.0.tar` & `outplan-3.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 12:05:59.000000 outplan-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-23 12:06:04.000000 outplan-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-23 12:05:59.000000 outplan-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14202 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-23 12:05:59.000000 outplan-3.0.0/outplan/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 12:06:04.000000 outplan-3.0.0/outplan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 12:05:59.000000 outplan-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:06:04.000000 outplan-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:06:04.000000 outplan-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    30837 2024-04-23 12:05:59.000000 outplan-3.0.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-23 12:05:59.000000 outplan-3.0.0/tests/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:53:01.000000 outplan-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 08:52:57.000000 outplan-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-28 08:53:01.000000 outplan-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-28 08:52:57.000000 outplan-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:53:01.000000 outplan-3.0.1/outplan/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-28 08:52:57.000000 outplan-3.0.1/outplan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-05-28 08:52:57.000000 outplan-3.0.1/outplan/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 08:52:57.000000 outplan-3.0.1/outplan/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 08:52:57.000000 outplan-3.0.1/outplan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-05-28 08:52:57.000000 outplan-3.0.1/outplan/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-28 08:52:57.000000 outplan-3.0.1/outplan/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:53:01.000000 outplan-3.0.1/outplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-28 08:53:01.000000 outplan-3.0.1/outplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-28 08:53:01.000000 outplan-3.0.1/outplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 08:53:01.000000 outplan-3.0.1/outplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-28 08:53:01.000000 outplan-3.0.1/outplan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 08:53:01.000000 outplan-3.0.1/outplan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-28 08:52:57.000000 outplan-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 08:53:01.000000 outplan-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 08:53:01.000000 outplan-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37818 2024-05-28 08:52:57.000000 outplan-3.0.1/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-28 08:52:57.000000 outplan-3.0.1/tests/test_local.py
```

### Comparing `outplan-3.0.0/LICENSE` & `outplan-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `outplan-3.0.0/PKG-INFO` & `outplan-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outplan
-Version: 3.0.0
+Version: 3.0.1
 Summary: Support nested experiment/namespace base on Facebook Planout
 Author-email: x1ah <gaoxiaoqiang@xiachufang.com>
 License: MIT License
         
         Copyright (c) 2019 xiachufang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `outplan-3.0.0/README.md` & `outplan-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `outplan-3.0.0/outplan/client.py` & `outplan-3.0.1/outplan/client.py`

 * *Files identical despite different names*

### Comparing `outplan-3.0.0/outplan/experiment.py` & `outplan-3.0.1/outplan/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,17 @@
                 experiment_name=res.get('experiment_name'),
                 group_extra_params=group_item.extra_params,
             )
         elif group_item.result_type == GroupResultType.layer:
             # 直到取到最底层分组
             while True:
                 _res = group_item.get_group(unit, **params)
+                # 没有通过 bucket 匹配到实验
+                if _res is None:
+                    return None
                 if isinstance(_res, TrackingGroup):
                     for group_name, exp_name in zip(group_names, exp_names):
                         _res.add_group_name(group_name)
                         _res.add_experiment_name(exp_name)
                     return _res
                 else:
                     group_names.append(_res.get('group').name)
```

### Comparing `outplan-3.0.0/outplan/local.py` & `outplan-3.0.1/outplan/local.py`

 * *Files identical despite different names*

### Comparing `outplan-3.0.0/outplan.egg-info/PKG-INFO` & `outplan-3.0.1/outplan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outplan
-Version: 3.0.0
+Version: 3.0.1
 Summary: Support nested experiment/namespace base on Facebook Planout
 Author-email: x1ah <gaoxiaoqiang@xiachufang.com>
 License: MIT License
         
         Copyright (c) 2019 xiachufang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `outplan-3.0.0/pyproject.toml` & `outplan-3.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `outplan-3.0.0/tests/test_experiment.py` & `outplan-3.0.1/tests/test_experiment.py`

 * *Files 13% similar despite different names*

```diff
@@ -692,14 +692,175 @@
 
     cnt = 0
     while cnt <= 10 and namespace.get_group(unit=f"foo-{cnt}") is None:
         cnt += 1
     assert cnt <= 10
 
 
+def test_nested_not_full_experiment_group_client():
+    """
+    测试实验组嵌套子namespace，并且子 namespace 中实验 bucket 不满的情况
+    """
+    namespace_spec = {
+        "name": "test_namespace_exp2",
+        "bucket": 100,
+        "unit_type": "pdid",
+        "auto_upper_unit": True,
+        "experiment_items": [
+            {
+                "name": "ttt111",
+                "bucket": 50,
+                "pre_condition": "",
+                "group_items": [
+                    {
+                        "name": "ns1",
+                        "weight": 0.33,
+                        "extra_params": "",
+                        "layer_namespaces": [
+                            {
+                                "name": "nested_ns1",
+                                "bucket": 100,
+                                "unit_type": "pdid",
+                                "auto_upper_unit": True,
+                                "experiment_items": [
+                                    {
+                                        "name": "nested_test_1",
+                                        "bucket": 10,
+                                        "pre_condition": "",
+                                        "group_items": [
+                                            {
+                                                "name": "exp1",
+                                                "weight": 0.5,
+                                                "extra_params": "",
+                                                "layer_namespaces": [],
+                                            },
+                                            {
+                                                "name": "control1",
+                                                "weight": 0.5,
+                                                "extra_params": "",
+                                                "layer_namespaces": [],
+                                            },
+                                        ],
+                                        "user_tags": [],
+                                    }
+                                ],
+                            }
+                        ],
+                    },
+                    {
+                        "name": "ns2",
+                        "weight": 0.34,
+                        "extra_params": "",
+                        "layer_namespaces": [
+                            {
+                                "name": "nested_test_ns2",
+                                "bucket": 100,
+                                "unit_type": "pdid",
+                                "auto_upper_unit": True,
+                                "experiment_items": [
+                                    {
+                                        "name": "nested_test_0528_2",
+                                        "bucket": 20,
+                                        "pre_condition": "",
+                                        "group_items": [
+                                            {
+                                                "name": "exp2",
+                                                "weight": 0.5,
+                                                "extra_params": "",
+                                                "layer_namespaces": [],
+                                            },
+                                            {
+                                                "name": "control2",
+                                                "weight": 0.5,
+                                                "extra_params": "",
+                                                "layer_namespaces": [],
+                                            },
+                                        ],
+                                        "user_tags": [],
+                                    }
+                                ],
+                            }
+                        ],
+                    },
+                    {
+                        "name": "ns3",
+                        "weight": 0.33,
+                        "extra_params": "",
+                        "layer_namespaces": [
+                            {
+                                "name": "test_nested_0528_3",
+                                "bucket": 100,
+                                "unit_type": "pdid",
+                                "auto_upper_unit": True,
+                                "experiment_items": [
+                                    {
+                                        "name": "test_nested_0528_3",
+                                        "bucket": 30,
+                                        "pre_condition": "",
+                                        "group_items": [
+                                            {
+                                                "name": "exp3",
+                                                "weight": 0.5,
+                                                "extra_params": "",
+                                                "layer_namespaces": [],
+                                            },
+                                            {
+                                                "name": "control3",
+                                                "weight": 0.5,
+                                                "extra_params": "",
+                                                "layer_namespaces": [],
+                                            },
+                                        ],
+                                        "user_tags": [],
+                                    }
+                                ],
+                            }
+                        ],
+                    },
+                ],
+                "user_tags": [],
+            },
+            {
+                "name": "test_nest_0528_4",
+                "bucket": 50,
+                "pre_condition": "",
+                "group_items": [
+                    {
+                        "name": "a",
+                        "weight": 0.5,
+                        "extra_params": "",
+                        "layer_namespaces": [],
+                    },
+                    {
+                        "name": "control",
+                        "weight": 0.5,
+                        "extra_params": "",
+                        "layer_namespaces": [],
+                    },
+                ],
+                "user_tags": [],
+            },
+        ],
+    }
+    namespace = NamespaceItem.from_dict(namespace_spec)
+    namespace.validate()
+
+    for i in range(1000):
+        namespace.get_group(unit=f"foo-{i}")
+
+    expected = ['a', None, 'control', 'a', None, 'control', 'a', None, 'a', 'control', 'exp1', 'control3', 'control', None, 'control3', None, 'exp3', 'a', None, None]
+
+    for i in range(20):
+        res = namespace.get_group(unit=f"foo-{i}")
+        if res:
+            assert res.last_group == expected[i]
+        else:
+            assert expected[i] is None
+
+
 def test_auto_upper_unit_namespace():
     def same_group(group_a, group_b):
         if group_a is None and group_b is None:
             return True
         if group_a is None or group_b is None:
             return False
         return (
```

### Comparing `outplan-3.0.0/tests/test_local.py` & `outplan-3.0.1/tests/test_local.py`

 * *Files identical despite different names*

