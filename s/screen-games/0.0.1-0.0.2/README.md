# Comparing `tmp/screen_games-0.0.1.tar.gz` & `tmp/screen_games-0.0.2.tar.gz`

## Comparing `screen_games-0.0.1.tar` & `screen_games-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 screen_games-0.0.1/screen_games/__init__.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 screen_games-0.0.1/screen_games/config.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 screen_games-0.0.1/screen_games/envs/__init__.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 screen_games-0.0.1/screen_games/envs/dino.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 screen_games-0.0.1/screen_games/envs/dino_slow.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 screen_games-0.0.1/screen_games/envs/screen.py
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 screen_games-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 screen_games-0.0.1/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 screen_games-0.0.1/README.md
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 screen_games-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 screen_games-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 screen_games-0.0.2/screen_games/__init__.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 screen_games-0.0.2/screen_games/config.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 screen_games-0.0.2/screen_games/envs/__init__.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 screen_games-0.0.2/screen_games/envs/dino.py
+-rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 screen_games-0.0.2/screen_games/envs/dino_slow.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 screen_games-0.0.2/screen_games/envs/screen.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 screen_games-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 screen_games-0.0.2/LICENSE
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 screen_games-0.0.2/README.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 screen_games-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 screen_games-0.0.2/PKG-INFO
```

### Comparing `screen_games-0.0.1/screen_games/config.py` & `screen_games-0.0.2/screen_games/config.py`

 * *Files identical despite different names*

### Comparing `screen_games-0.0.1/screen_games/envs/dino.py` & `screen_games-0.0.2/screen_games/envs/dino.py`

 * *Files identical despite different names*

### Comparing `screen_games-0.0.1/screen_games/envs/dino_slow.py` & `screen_games-0.0.2/screen_games/envs/dino_slow.py`

 * *Files identical despite different names*

### Comparing `screen_games-0.0.1/screen_games/envs/screen.py` & `screen_games-0.0.2/screen_games/envs/screen.py`

 * *Files identical despite different names*

### Comparing `screen_games-0.0.1/.gitignore` & `screen_games-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `screen_games-0.0.1/LICENSE` & `screen_games-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `screen_games-0.0.1/pyproject.toml` & `screen_games-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "screen_games"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="timcsy", email="timocsy@yahoo.com.tw" },
 ]
 description = "Connect your PC screen and keyboard, mouse event to OpenAI Gym!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "gymnasium>=0.28",
-		"eventstreaming>=0.0.1",
+	"eventstreaming>=0.0.2",
     "python-dotenv>=0.19",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/timcsy/screen_games"
 "Bug Tracker" = "https://github.com/timcsy/screen_games/issues"
```

### Comparing `screen_games-0.0.1/PKG-INFO` & `screen_games-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.3
 Name: screen_games
-Version: 0.0.1
+Version: 0.0.2
 Summary: Connect your PC screen and keyboard, mouse event to OpenAI Gym!
 Project-URL: Homepage, https://github.com/timcsy/screen_games
 Project-URL: Bug Tracker, https://github.com/timcsy/screen_games/issues
 Author-email: timcsy <timocsy@yahoo.com.tw>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: eventstreaming>=0.0.1
+Requires-Dist: eventstreaming>=0.0.2
 Requires-Dist: gymnasium>=0.28
 Requires-Dist: python-dotenv>=0.19
 Description-Content-Type: text/markdown
 
 # ScreenGames
 
 Connect your PC screen and keyboard, mouse event to OpenAI Gym!
```

