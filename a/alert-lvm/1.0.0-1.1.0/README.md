# Comparing `tmp/alert_lvm-1.0.0.tar.gz` & `tmp/alert_lvm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alert_lvm-1.0.0.tar", last modified: Fri May 24 07:37:41 2024, max compression
+gzip compressed data, was "alert_lvm-1.1.0.tar", last modified: Tue May 28 09:29:37 2024, max compression
```

## Comparing `alert_lvm-1.0.0.tar` & `alert_lvm-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:37:41.831550 alert_lvm-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-23 08:04:06.000000 alert_lvm-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4494 2024-05-24 07:37:41.831550 alert_lvm-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2578 2024-05-24 07:27:47.000000 alert_lvm-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      708 2024-05-24 07:31:33.000000 alert_lvm-1.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 07:37:41.831550 alert_lvm-1.0.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:37:41.821550 alert_lvm-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:37:41.831550 alert_lvm-1.0.0/src/alert_lvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4494 2024-05-24 07:37:41.000000 alert_lvm-1.0.0/src/alert_lvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2024-05-24 07:37:41.000000 alert_lvm-1.0.0/src/alert_lvm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 07:37:41.000000 alert_lvm-1.0.0/src/alert_lvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-24 07:37:41.000000 alert_lvm-1.0.0/src/alert_lvm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-24 07:37:41.000000 alert_lvm-1.0.0/src/alert_lvm.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 07:37:41.821550 alert_lvm-1.0.0/src/alertlvm/
--rw-r--r--   0 root         (0) root         (0)       26 2024-05-24 02:00:06.000000 alert_lvm-1.0.0/src/alertlvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2356 2024-05-24 06:30:27.000000 alert_lvm-1.0.0/src/alertlvm/lvm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:29:37.196889 alert_lvm-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-23 08:04:06.000000 alert_lvm-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-05-28 09:29:37.196889 alert_lvm-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3176 2024-05-28 09:23:58.000000 alert_lvm-1.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      708 2024-05-28 09:29:03.000000 alert_lvm-1.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 09:29:37.196889 alert_lvm-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:29:37.196889 alert_lvm-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:29:37.196889 alert_lvm-1.1.0/src/alert_lvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-05-28 09:29:37.000000 alert_lvm-1.1.0/src/alert_lvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-28 09:29:37.000000 alert_lvm-1.1.0/src/alert_lvm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 09:29:37.000000 alert_lvm-1.1.0/src/alert_lvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-28 09:29:37.000000 alert_lvm-1.1.0/src/alert_lvm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-28 09:29:37.000000 alert_lvm-1.1.0/src/alert_lvm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 09:29:37.196889 alert_lvm-1.1.0/src/alertlvm/
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-24 02:00:06.000000 alert_lvm-1.1.0/src/alertlvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3636 2024-05-28 09:08:45.000000 alert_lvm-1.1.0/src/alertlvm/lvm.py
```

### Comparing `alert_lvm-1.0.0/LICENSE` & `alert_lvm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alert_lvm-1.0.0/PKG-INFO` & `alert_lvm-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert-lvm
-Version: 1.0.0
+Version: 1.1.0
 Summary: A client library to call the LVM API with some helpful functions
 Author-email: "intellicloud.ai" <xbrain_lvm@intellicloud.ai>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -56,23 +56,23 @@
 
 scenario_key = "<the key>"
 
 image_path = "<image_path>"
 
 result = client.analyze(scenario_key, image_path)
 if result.get("error"):
-        print(result.get("code"))
-        print(result.get("error_message"))
-    else:
-        print(result.get("conclusion")) # conclusion of the analysis
-        print(result.get("text")) # detail content of the analysis
+    print(result.get("code"))
+    print(result.get("error_message"))
+else:
+    print(result.get("conclusion")) # conclusion of the analysis
+    print(result.get("text")) # detail content of the analysis
 
-        # ... your code here ...
+    # ... your code here ...
 
-        os.remove(result.get("frame"))
+    os.remove(result.get("frame"))
 ```
 
 ### Analyze video:
 
 The default setting is to extract and analyze one frame every 750 frames (250 frames/second * 30 seconds):
 
 ```python
@@ -139,7 +139,30 @@
         print(result.get("conclusion")) # conclusion of the analysis
         print(result.get("text")) # detail content of the analysis
 
         # ... your code here ...
 
         os.remove(result.get("frame"))
 ```
+
+### Show result:
+
+Please note that the ```show``` method will block the current thread. You can press the 'q' key or use the close button to close the current window. Only after this will the program continue to execute.
+
+```python
+import os
+from alertlvm import AlertLVM
+
+client = AlertLVM(
+    token="<your token here>"
+)
+
+scenario_key = "<the key>"
+
+video_path = "<video_path>"
+
+for result in client.analyzeVideo(scenario_key, video_path):
+    if 'error' not in result:
+        print(result.get("text")) # detail content of the analysis
+        client.show(result) # show result
+        os.remove(result.get("frame"))
+```
```

### Comparing `alert_lvm-1.0.0/README.md` & `alert_lvm-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 scenario_key = "<the key>"
 
 image_path = "<image_path>"
 
 result = client.analyze(scenario_key, image_path)
 if result.get("error"):
-        print(result.get("code"))
-        print(result.get("error_message"))
-    else:
-        print(result.get("conclusion")) # conclusion of the analysis
-        print(result.get("text")) # detail content of the analysis
+    print(result.get("code"))
+    print(result.get("error_message"))
+else:
+    print(result.get("conclusion")) # conclusion of the analysis
+    print(result.get("text")) # detail content of the analysis
 
-        # ... your code here ...
+    # ... your code here ...
 
-        os.remove(result.get("frame"))
+    os.remove(result.get("frame"))
 ```
 
 ### Analyze video:
 
 The default setting is to extract and analyze one frame every 750 frames (250 frames/second * 30 seconds):
 
 ```python
@@ -99,8 +99,31 @@
         print(result.get("frame")) # the file path of a frame extracted from the video that has been sent to the server
         print(result.get("conclusion")) # conclusion of the analysis
         print(result.get("text")) # detail content of the analysis
 
         # ... your code here ...
 
         os.remove(result.get("frame"))
+```
+
+### Show result:
+
+Please note that the ```show``` method will block the current thread. You can press the 'q' key or use the close button to close the current window. Only after this will the program continue to execute.
+
+```python
+import os
+from alertlvm import AlertLVM
+
+client = AlertLVM(
+    token="<your token here>"
+)
+
+scenario_key = "<the key>"
+
+video_path = "<video_path>"
+
+for result in client.analyzeVideo(scenario_key, video_path):
+    if 'error' not in result:
+        print(result.get("text")) # detail content of the analysis
+        client.show(result) # show result
+        os.remove(result.get("frame"))
 ```
```

### Comparing `alert_lvm-1.0.0/pyproject.toml` & `alert_lvm-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alert-lvm"
-version = "1.0.0"
+version = "1.1.0"
 description = "A client library to call the LVM API with some helpful functions"
 readme = "README.md"
 authors = [{ name = "intellicloud.ai", email = "xbrain_lvm@intellicloud.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `alert_lvm-1.0.0/src/alert_lvm.egg-info/PKG-INFO` & `alert_lvm-1.1.0/src/alert_lvm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert-lvm
-Version: 1.0.0
+Version: 1.1.0
 Summary: A client library to call the LVM API with some helpful functions
 Author-email: "intellicloud.ai" <xbrain_lvm@intellicloud.ai>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -56,23 +56,23 @@
 
 scenario_key = "<the key>"
 
 image_path = "<image_path>"
 
 result = client.analyze(scenario_key, image_path)
 if result.get("error"):
-        print(result.get("code"))
-        print(result.get("error_message"))
-    else:
-        print(result.get("conclusion")) # conclusion of the analysis
-        print(result.get("text")) # detail content of the analysis
+    print(result.get("code"))
+    print(result.get("error_message"))
+else:
+    print(result.get("conclusion")) # conclusion of the analysis
+    print(result.get("text")) # detail content of the analysis
 
-        # ... your code here ...
+    # ... your code here ...
 
-        os.remove(result.get("frame"))
+    os.remove(result.get("frame"))
 ```
 
 ### Analyze video:
 
 The default setting is to extract and analyze one frame every 750 frames (250 frames/second * 30 seconds):
 
 ```python
@@ -139,7 +139,30 @@
         print(result.get("conclusion")) # conclusion of the analysis
         print(result.get("text")) # detail content of the analysis
 
         # ... your code here ...
 
         os.remove(result.get("frame"))
 ```
+
+### Show result:
+
+Please note that the ```show``` method will block the current thread. You can press the 'q' key or use the close button to close the current window. Only after this will the program continue to execute.
+
+```python
+import os
+from alertlvm import AlertLVM
+
+client = AlertLVM(
+    token="<your token here>"
+)
+
+scenario_key = "<the key>"
+
+video_path = "<video_path>"
+
+for result in client.analyzeVideo(scenario_key, video_path):
+    if 'error' not in result:
+        print(result.get("text")) # detail content of the analysis
+        client.show(result) # show result
+        os.remove(result.get("frame"))
+```
```

### Comparing `alert_lvm-1.0.0/src/alertlvm/lvm.py` & `alert_lvm-1.1.0/src/alertlvm/lvm.py`

 * *Files 24% similar despite different names*

```diff
@@ -60,7 +60,46 @@
                     "code": resp.status_code,
                 }
             )
             with tempfile.NamedTemporaryFile(suffix=".jpg", delete=False) as temp:
                 cv2.imwrite(temp.name, frame)
                 result["frame"] = temp.name
             yield result
+
+    def show(self, result):
+        img = cv2.imread(result.get("frame"))
+        conclusion = {0: "Alarm", 1: "Unclear", 2: "Passed"}.get(
+            result.get("conclusion"), "Unknown"
+        )
+        color = {0: (0, 0, 255), 1: (0, 255, 255), 2: (0, 255, 0)}.get(
+            result.get("conclusion"), (220, 220, 220)
+        )
+        (text_width, text_height), _ = cv2.getTextSize(
+            conclusion, cv2.FONT_HERSHEY_SIMPLEX, 3, 2
+        )
+        org = (img.shape[1] - text_width - 15, img.shape[0] - 30)
+        thickness = 2
+        for i in range(5):
+            cv2.putText(
+                img,
+                conclusion,
+                org,
+                cv2.FONT_HERSHEY_SIMPLEX,
+                3,
+                color,
+                thickness + i,
+            )
+        cv2.rectangle(
+            img,
+            (org[0] - 5, org[1] + 10),
+            (org[0] + text_width + 3, org[1] - text_height - 10),
+            color,
+            5,
+        )
+        cv2.imshow("image", img)
+        cv2.moveWindow("image", 100, 100)
+        while True:
+            if cv2.getWindowProperty("image", cv2.WND_PROP_VISIBLE) < 1:
+                break
+            if cv2.waitKey(100) & 0xFF == ord("q"):
+                break
+        cv2.destroyAllWindows()
```

