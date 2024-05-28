# Comparing `tmp/l3c-0.1.0.5.tar.gz` & `tmp/l3c-0.1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/l3c-0.1.0.5.tar", last modified: Thu Apr 25 08:00:52 2024, max compression
+gzip compressed data, was "dist/l3c-0.1.1.0.tar", last modified: Tue May 28 03:00:20 2024, max compression
```

## Comparing `l3c-0.1.0.5.tar` & `l3c-0.1.1.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1108 2024-04-25 08:00:52.000000 l3c-0.1.0.5/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.0.5/LICENSE
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/bandits/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.0.5/l3c/bandits/demo_thompson_sampling.py
--rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/bandits/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/bandits/bandits_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/mazeworld/
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/mazeworld/demo/
--rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-02-22 14:53:11.000000 l3c-0.1.0.5/l3c/mazeworld/demo/keyboard_play_demo.py
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.0.5/l3c/mazeworld/demo/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3877 2024-04-25 07:54:35.000000 l3c-0.1.0.5/l3c/mazeworld/demo/agent_play_demo.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/l3c/mazeworld/tests/
--rw-r--r--   0 wangfan04   (502) staff       (20)     2414 2024-04-25 07:55:18.000000 l3c-0.1.0.5/l3c/mazeworld/tests/test_agent.py
--rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.0.5/l3c/mazeworld/tests/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.0.5/l3c/mazeworld/tests/test.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.0.5/l3c/mazeworld/__init__.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c/mazeworld/agents/
--rw-r--r--   0 wangfan04   (502) staff       (20)     3931 2024-04-25 07:54:08.000000 l3c-0.1.0.5/l3c/mazeworld/agents/agent_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.0.5/l3c/mazeworld/agents/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    11869 2024-04-25 07:30:00.000000 l3c-0.1.0.5/l3c/mazeworld/agents/smart_slam_agent.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/l3c/mazeworld/envs/
--rw-r--r--   0 wangfan04   (502) staff       (20)     7295 2024-04-16 02:07:18.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_env.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3428 2024-04-25 07:44:06.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_2d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6781 2024-04-25 06:47:52.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    14954 2024-04-23 08:19:34.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_base.py
--rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.0.5/l3c/mazeworld/envs/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_task.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     6256 2024-04-25 06:48:19.000000 l3c-0.1.0.5/l3c/mazeworld/envs/maze_continuous_3d.py
--rw-r--r--   0 wangfan04   (502) staff       (20)    12366 2024-04-16 02:19:02.000000 l3c-0.1.0.5/l3c/mazeworld/envs/ray_caster_utils.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.0.5/l3c/mazeworld/envs/dynamics.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:52.000000 l3c-0.1.0.5/l3c/metalang/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1112 2024-04-23 10:49:18.000000 l3c-0.1.0.5/l3c/metalang/__init__.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     5496 2024-04-23 10:52:10.000000 l3c-0.1.0.5/l3c/metalang/metalangv2.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     4420 2024-04-23 10:51:20.000000 l3c-0.1.0.5/l3c/metalang/metalangv1.py
--rw-r--r--   0 wangfan04   (502) staff       (20)     2666 2024-04-23 10:53:14.000000 l3c-0.1.0.5/l3c/metalang/generator.py
--rw-r--r--   0 wangfan04   (502) staff       (20)      682 2024-04-23 08:58:47.000000 l3c-0.1.0.5/README.md
--rwxr-xr-x   0 wangfan04   (502) staff       (20)     1814 2024-04-25 08:00:49.000000 l3c-0.1.0.5/setup.py
-drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/
--rw-r--r--   0 wangfan04   (502) staff       (20)     1108 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/PKG-INFO
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.0.5/l3c.egg-info/not-zip-safe
--rw-r--r--   0 wangfan04   (502) staff       (20)     1050 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/SOURCES.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/requires.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/top_level.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-04-25 08:00:51.000000 l3c-0.1.0.5/l3c.egg-info/dependency_links.txt
--rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-04-25 08:00:52.000000 l3c-0.1.0.5/setup.cfg
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:20.000000 l3c-0.1.1.0/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1151 2024-05-28 03:00:20.000000 l3c-0.1.1.0/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11357 2023-02-23 10:00:57.000000 l3c-0.1.1.0/LICENSE
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c/
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c/bandits/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1022 2023-02-23 10:32:50.000000 l3c-0.1.1.0/l3c/bandits/demo_thompson_sampling.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      838 2023-02-23 10:11:06.000000 l3c-0.1.1.0/l3c/bandits/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2717 2023-02-23 10:11:06.000000 l3c-0.1.1.0/l3c/bandits/bandits_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      762 2023-02-23 10:11:06.000000 l3c-0.1.1.0/l3c/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c/mazeworld/
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:20.000000 l3c-0.1.1.0/l3c/mazeworld/demo/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3366 2024-05-28 02:58:39.000000 l3c-0.1.1.0/l3c/mazeworld/demo/keyboard_play_demo.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:15.000000 l3c-0.1.1.0/l3c/mazeworld/demo/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3902 2024-04-30 10:04:43.000000 l3c-0.1.1.0/l3c/mazeworld/demo/agent_play_demo.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:20.000000 l3c-0.1.1.0/l3c/mazeworld/tests/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2414 2024-04-25 07:55:18.000000 l3c-0.1.1.0/l3c/mazeworld/tests/test_agent.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)        0 2024-02-22 12:15:23.000000 l3c-0.1.1.0/l3c/mazeworld/tests/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2068 2024-02-04 15:06:43.000000 l3c-0.1.1.0/l3c/mazeworld/tests/test.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1714 2024-02-20 08:03:46.000000 l3c-0.1.1.0/l3c/mazeworld/__init__.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:20.000000 l3c-0.1.1.0/l3c/mazeworld/agents/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3931 2024-04-25 07:54:08.000000 l3c-0.1.1.0/l3c/mazeworld/agents/agent_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)       45 2024-02-22 03:03:45.000000 l3c-0.1.1.0/l3c/mazeworld/agents/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    11869 2024-04-25 07:30:00.000000 l3c-0.1.1.0/l3c/mazeworld/agents/smart_slam_agent.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:20.000000 l3c-0.1.1.0/l3c/mazeworld/envs/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     8095 2024-05-28 02:56:24.000000 l3c-0.1.1.0/l3c/mazeworld/envs/maze_env.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3428 2024-04-25 07:44:06.000000 l3c-0.1.1.0/l3c/mazeworld/envs/maze_discrete_2d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6781 2024-04-25 06:47:52.000000 l3c-0.1.1.0/l3c/mazeworld/envs/maze_discrete_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    14954 2024-04-23 08:19:34.000000 l3c-0.1.1.0/l3c/mazeworld/envs/maze_base.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      258 2024-02-04 12:16:02.000000 l3c-0.1.1.0/l3c/mazeworld/envs/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     9184 2024-02-20 01:19:41.000000 l3c-0.1.1.0/l3c/mazeworld/envs/maze_task.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     6256 2024-04-25 06:48:19.000000 l3c-0.1.1.0/l3c/mazeworld/envs/maze_continuous_3d.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)    12366 2024-04-16 02:19:02.000000 l3c-0.1.1.0/l3c/mazeworld/envs/ray_caster_utils.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     3644 2023-02-23 10:11:06.000000 l3c-0.1.1.0/l3c/mazeworld/envs/dynamics.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:20.000000 l3c-0.1.1.0/l3c/metalang/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1112 2024-04-23 10:49:18.000000 l3c-0.1.1.0/l3c/metalang/__init__.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     5496 2024-04-28 10:00:10.000000 l3c-0.1.1.0/l3c/metalang/metalangv2.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      621 2024-04-28 10:30:46.000000 l3c-0.1.1.0/l3c/metalang/test.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     4420 2024-04-23 10:51:20.000000 l3c-0.1.1.0/l3c/metalang/metalangv1.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)     2666 2024-04-23 10:53:14.000000 l3c-0.1.1.0/l3c/metalang/generator.py
+-rw-r--r--   0 wangfan04   (502) staff       (20)      653 2024-05-28 02:37:31.000000 l3c-0.1.1.0/README.md
+-rwxr-xr-x   0 wangfan04   (502) staff       (20)     1814 2024-05-28 02:59:21.000000 l3c-0.1.1.0/setup.py
+drwxr-xr-x   0 wangfan04   (502) staff       (20)        0 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c.egg-info/
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1151 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c.egg-info/PKG-INFO
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2023-04-19 12:54:38.000000 l3c-0.1.1.0/l3c.egg-info/not-zip-safe
+-rw-r--r--   0 wangfan04   (502) staff       (20)     1071 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)       84 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c.egg-info/requires.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        4 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c.egg-info/top_level.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)        1 2024-05-28 03:00:19.000000 l3c-0.1.1.0/l3c.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfan04   (502) staff       (20)       38 2024-05-28 03:00:20.000000 l3c-0.1.1.0/setup.cfg
```

### Comparing `l3c-0.1.0.5/LICENSE` & `l3c-0.1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/bandits/demo_thompson_sampling.py` & `l3c-0.1.1.0/l3c/bandits/demo_thompson_sampling.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/bandits/__init__.py` & `l3c-0.1.1.0/l3c/bandits/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/bandits/bandits_env.py` & `l3c-0.1.1.0/l3c/bandits/bandits_env.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/__init__.py` & `l3c-0.1.1.0/l3c/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/demo/keyboard_play_demo.py` & `l3c-0.1.1.0/l3c/mazeworld/demo/keyboard_play_demo.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/demo/agent_play_demo.py` & `l3c-0.1.1.0/l3c/mazeworld/demo/agent_play_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,11 +59,12 @@
         action = agent.step(observation, reward)
         observation, reward, done, _ = maze_env.step(action)
         sum_reward += reward
         if(args.verbose):
             print("Instant r = %.2f, Accumulate r = %.2f" % (reward, sum_reward))
         if(maze_env.key_done):
             break
+        time.sleep(0.20)
     print("Episode is over! You got %.2f score."%sum_reward)
 
     if(args.save_replay is not None):
         maze_env.save_trajectory(args.save_replay)
```

### Comparing `l3c-0.1.0.5/l3c/mazeworld/tests/test_agent.py` & `l3c-0.1.1.0/l3c/mazeworld/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/tests/test.py` & `l3c-0.1.1.0/l3c/mazeworld/tests/test.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/__init__.py` & `l3c-0.1.1.0/l3c/mazeworld/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/agents/agent_base.py` & `l3c-0.1.1.0/l3c/mazeworld/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/agents/smart_slam_agent.py` & `l3c-0.1.1.0/l3c/mazeworld/agents/smart_slam_agent.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/maze_env.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/maze_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             render_scale=480,
             max_steps=5000,
             task_type="NAVIGATION",
             ):
         self.maze_type = maze_type
         self.enable_render = enable_render
         self.render_viewsize = render_scale
+        self.task_type = task_type
 
         self.need_reset = True
         self.need_set_task = True
 
     def set_task(self, task_config):
         self.maze_core.set_task(task_config)
         self.need_set_task = False
@@ -69,14 +70,29 @@
             raise NotImplementedError("Only human mode is supported")
         if(self.enable_render):
             self.key_done, self.keyboard_press = self.maze_core.render_update()
 
     def get_loc_map(self, map_range=2):
         return self.maze_core.get_loc_map(map_rang=map_range)
 
+    def get_target_gt_direction(self):
+        if(self.task_type != "NAVIGATION"):
+            raise Exception("Only \"NAVIGATION\" task type is supported")
+        target_id = self.maze_core._commands_sequence[self.maze_core._commands_sequence_idx]
+        target_grid = self.maze_core._landmarks_coordinates[target_id]
+        deta_grid = numpy.zeros(shape=(2,), dtype=numpy.float32)
+        deta_grid[0] = target_grid[0] - self.maze_core._agent_grid[0]
+        deta_grid[1] = target_grid[1] - self.maze_core._agent_grid[1]
+        angle = numpy.arctan2(deta_grid[1], deta_grid[0]) - self.maze_core._agent_ori
+        if(angle < -numpy.pi):
+            angle += 2 * numpy.pi
+        elif(angle > numpy.pi):
+            angle -= 2 * numpy.pi
+        return angle
+
     def save_trajectory(self, file_name, view_size=480):
         if(not self.enable_render):
             self.maze_core.render_init(view_size)
         self.maze_core.render_trajectory(file_name)
 
 
 class MazeWorldDiscrete3D(MazeWorldEnvBase):
```

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_2d.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/maze_discrete_2d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/maze_discrete_3d.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/maze_discrete_3d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/maze_base.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/maze_base.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/maze_task.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/maze_task.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/maze_continuous_3d.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/maze_continuous_3d.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/ray_caster_utils.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/ray_caster_utils.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/mazeworld/envs/dynamics.py` & `l3c-0.1.1.0/l3c/mazeworld/envs/dynamics.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/metalang/__init__.py` & `l3c-0.1.1.0/l3c/metalang/__init__.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/metalang/metalangv2.py` & `l3c-0.1.1.0/l3c/metalang/metalangv2.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/metalang/metalangv1.py` & `l3c-0.1.1.0/l3c/metalang/metalangv1.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/l3c/metalang/generator.py` & `l3c-0.1.1.0/l3c/metalang/generator.py`

 * *Files identical despite different names*

### Comparing `l3c-0.1.0.5/setup.py` & `l3c-0.1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
 from setuptools import setup, find_packages
 
-__version__ = '0.1.0.5'
+__version__ = '0.1.1.0'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='l3c',
     version=__version__,
```

### Comparing `l3c-0.1.0.5/l3c.egg-info/SOURCES.txt` & `l3c-0.1.1.0/l3c.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 l3c/mazeworld/envs/ray_caster_utils.py
 l3c/mazeworld/tests/__init__.py
 l3c/mazeworld/tests/test.py
 l3c/mazeworld/tests/test_agent.py
 l3c/metalang/__init__.py
 l3c/metalang/generator.py
 l3c/metalang/metalangv1.py
-l3c/metalang/metalangv2.py
+l3c/metalang/metalangv2.py
+l3c/metalang/test.py
```

