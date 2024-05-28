# Comparing `tmp/pytvpaint-1.0.0b8.tar.gz` & `tmp/pytvpaint-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytvpaint-1.0.0b8.tar", max compression
+gzip compressed data, was "pytvpaint-1.0.0b9.tar", max compression
```

## Comparing `pytvpaint-1.0.0b8.tar` & `pytvpaint-1.0.0b9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2024-05-22 18:39:25.575981 pytvpaint-1.0.0b8/LICENSE.md
--rw-r--r--   0        0        0     3515 2024-05-22 18:39:25.575981 pytvpaint-1.0.0b8/README.md
--rw-r--r--   0        0        0     2229 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     1233 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/__init__.py
--rw-r--r--   0        0        0     8570 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/camera.py
--rw-r--r--   0        0        0    33490 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/clip.py
--rw-r--r--   0        0        0      573 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/__init__.py
--rw-r--r--   0        0        0     4936 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/client/__init__.py
--rw-r--r--   0        0        0     9747 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/client/parse.py
--rw-r--r--   0        0        0     5389 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/client/rpc.py
--rw-r--r--   0        0        0      687 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/exceptions.py
--rw-r--r--   0        0        0    28228 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_base.py
--rw-r--r--   0        0        0     2719 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_camera.py
--rw-r--r--   0        0        0    19130 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_clip.py
--rw-r--r--   0        0        0    31138 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_layer.py
--rw-r--r--   0        0        0    14926 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_project.py
--rw-r--r--   0        0        0     1189 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_scene.py
--rw-r--r--   0        0        0    41942 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/layer.py
--rw-r--r--   0        0        0    23105 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/project.py
--rw-r--r--   0        0        0        0 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/py.typed
--rw-r--r--   0        0        0     4384 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/scene.py
--rw-r--r--   0        0        0     8745 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/sound.py
--rw-r--r--   0        0        0    17136 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/utils.py
--rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-28 20:46:39.013467 pytvpaint-1.0.0b9/LICENSE.md
+-rw-r--r--   0        0        0     3509 2024-05-28 20:46:39.013467 pytvpaint-1.0.0b9/README.md
+-rw-r--r--   0        0        0     2229 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     1233 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/__init__.py
+-rw-r--r--   0        0        0     8570 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/camera.py
+-rw-r--r--   0        0        0    33490 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/clip.py
+-rw-r--r--   0        0        0      573 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/george/__init__.py
+-rw-r--r--   0        0        0     4936 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/george/client/__init__.py
+-rw-r--r--   0        0        0     9747 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/george/client/parse.py
+-rw-r--r--   0        0        0     5389 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/george/client/rpc.py
+-rw-r--r--   0        0        0      687 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/george/exceptions.py
+-rw-r--r--   0        0        0    28228 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/george/grg_base.py
+-rw-r--r--   0        0        0     2719 2024-05-28 20:46:39.021467 pytvpaint-1.0.0b9/pytvpaint/george/grg_camera.py
+-rw-r--r--   0        0        0    19431 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/george/grg_clip.py
+-rw-r--r--   0        0        0    31132 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/george/grg_layer.py
+-rw-r--r--   0        0        0    15223 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/george/grg_project.py
+-rw-r--r--   0        0        0     1189 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/george/grg_scene.py
+-rw-r--r--   0        0        0    41983 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/layer.py
+-rw-r--r--   0        0        0    23105 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/project.py
+-rw-r--r--   0        0        0        0 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/py.typed
+-rw-r--r--   0        0        0     4384 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/scene.py
+-rw-r--r--   0        0        0     8745 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/sound.py
+-rw-r--r--   0        0        0    17136 2024-05-28 20:46:39.025467 pytvpaint-1.0.0b9/pytvpaint/utils.py
+-rw-r--r--   0        0        0     4414 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b9/PKG-INFO
```

### Comparing `pytvpaint-1.0.0b8/LICENSE.md` & `pytvpaint-1.0.0b9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/README.md` & `pytvpaint-1.0.0b9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/brunchstudio/pytvpaint/main/docs/assets/pytvpaint_code_banner.png" width=700 />
 </p>
 
 **PyTVPaint** is a type-safe Python library that wraps the George programming language commands in order to interact with the 2D animation software TVPaint.
 
-It communicates through WebSocket to a [custom C++ plugin](https://github.com/brunchstudio/tvpaint-rpc) running in an opened TVPaint instance.
+It communicates through WebSocket to a [custom C++ plugin](https://github.com/brunchstudio/tvpaint-rpc) running in an open TVPaint instance.
 
 You can check the [documentation](https://brunchstudio.github.io/pytvpaint/) for more details.
 
 ## Installation
 
 ### Requirements
 
@@ -25,15 +25,15 @@
 - Python v3.9+
 - TVPaint v11.5+
 - TVPaint RPC plugin (install instructions [here](https://brunchstudio.github.io/pytvpaint/installation/#tvpaint-plugin-installation))
 
 Install the package with Pip:
 
 ```console
-❯ pip install pytvpaint
+pip install pytvpaint
 ```
 
 ## Simple example
 
 ```python
 from pytvpaint import george
 from pytvpaint.project import Project
```

### Comparing `pytvpaint-1.0.0b8/pyproject.toml` & `pytvpaint-1.0.0b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytvpaint"
-version = "1.0.0b8"
+version = "1.0.0b9"
 description = "Python scripting for TVPaint"
 authors = [
     "Brunch Studio Developers <dev@brunchstudio.tv>",
     "Radouane Lahmidi <rlahmidi@brunchstudio.tv>",
     "Joseph Henry <jhenry@brunchstudio.tv>",
 ]
 license = "MIT"
```

### Comparing `pytvpaint-1.0.0b8/pytvpaint/__init__.py` & `pytvpaint-1.0.0b9/pytvpaint/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/camera.py` & `pytvpaint-1.0.0b9/pytvpaint/camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/clip.py` & `pytvpaint-1.0.0b9/pytvpaint/clip.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/__init__.py` & `pytvpaint-1.0.0b9/pytvpaint/george/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/client/__init__.py` & `pytvpaint-1.0.0b9/pytvpaint/george/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/client/parse.py` & `pytvpaint-1.0.0b9/pytvpaint/george/client/parse.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/client/rpc.py` & `pytvpaint-1.0.0b9/pytvpaint/george/client/rpc.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/exceptions.py` & `pytvpaint-1.0.0b9/pytvpaint/george/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/grg_base.py` & `pytvpaint-1.0.0b9/pytvpaint/george/grg_base.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/grg_camera.py` & `pytvpaint-1.0.0b9/pytvpaint/george/grg_camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/grg_clip.py` & `pytvpaint-1.0.0b9/pytvpaint/george/grg_clip.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from typing import Any
 
 from pytvpaint.george.client import send_cmd, try_cmd
 from pytvpaint.george.client.parse import (
     args_dict_to_list,
     tv_parse_dict,
     tv_parse_list,
-    validate_args_list,
 )
 from pytvpaint.george.exceptions import NoObjectWithIdError
 from pytvpaint.george.grg_base import (
     FieldOrder,
     GrgErrorValue,
     SaveFormat,
     SpriteLayout,
@@ -215,61 +214,58 @@
 
 
 @try_cmd(exception_msg="Invalid format for sequence")
 def tv_load_sequence(
     seq_path: Path | str,
     offset_count: tuple[int, int] | None = None,
     field_order: FieldOrder | None = None,
-    stretch: bool | None = None,
-    time_stretch: bool | None = None,
-    preload: bool | None = None,
+    stretch: bool = False,
+    time_stretch: bool = False,
+    preload: bool = False,
 ) -> int:
     """Load a sequence of images or movie in a new layer.
 
     Args:
         seq_path: the first file of the sequence to load
-        offset_count: the start and number of image of sequence to load. Defaults to None.
+        offset_count: the start and number of images in the sequence to load. Defaults to None.
         field_order: the field order. Defaults to None.
         stretch: Stretch each image to the size of the layer. Defaults to None.
-        time_stretch: Once loaded, the layer will have a new number of image corresponding to the project framerate. Defaults to None.
+        time_stretch: Once loaded, the layer will have a new number of images corresponding to the project framerate. Defaults to None.
         preload: Load all the images in memory, no more reference on the files. Defaults to None.
 
     Raises:
         FileNotFoundError: if the sequence file doesn't exist
         GeorgeError: if the input file is in an invalid format
 
     Returns:
         the number of images of the new layer
     """
     seq_path = Path(seq_path)
 
     if not seq_path.exists():
         raise FileNotFoundError(f"File not found at: {seq_path.as_posix()}")
 
-    args: list[int | str | None] = [field_order.value if field_order else None]
-
-    if offset_count is not None:
-        offset, count = offset_count
-        args.insert(0, count)
-        args.insert(0, offset)
-
-    # Filter None inline arguments
-    args = [a for a in args if a is not None]
-
-    args += args_dict_to_list(
-        {
-            "stretch": stretch,
-            "timestretch": time_stretch,
-            "preload": preload,
-        }
-    )
+    args: list[int | str] = [seq_path.as_posix()]
+    if offset_count and len(offset_count) == 2:
+        args.extend(offset_count)
+    if field_order:
+        args.append(field_order.value)
+
+    extra_args = [
+        (stretch, "stretch"),
+        (time_stretch, "timestretch"),
+        (preload, "preload"),
+    ]
+    for param, param_name in extra_args:
+        if not param:
+            continue
+        args.append(param_name)
 
     result = send_cmd(
         "tv_LoadSequence",
-        seq_path.as_posix(),
         *args,
         error_values=[-1],
     )
 
     return int(result)
 
 
@@ -642,23 +638,30 @@
     fade_in_start: float | None = None,
     fade_in_stop: float | None = None,
     fade_out_start: float | None = None,
     fade_out_stop: float | None = None,
     color_index: int | None = None,
 ) -> None:
     """Change a soundtracks settings."""
+    cur_options = tv_sound_clip_info(tv_clip_current_id(), track_index)
+    args: list[int | float | None] = []
+
     optional_args = [
-        int(mute) if mute is not None else None,
-        volume,
-        offset,
-        (fade_in_start, fade_in_stop, fade_out_start, fade_out_stop),
-        color_index,
+        (int(mute) if mute is not None else None, int(cur_options.mute)),
+        (volume, cur_options.volume),
+        (offset, cur_options.offset),
+        (fade_in_start, cur_options.fade_in_start),
+        (fade_in_stop, cur_options.fade_in_stop),
+        (fade_out_start, cur_options.fade_out_start),
+        (fade_out_stop, cur_options.fade_out_stop),
     ]
+    for arg, default_value in optional_args:
+        args.append(arg if arg is not None else default_value)
 
-    args = validate_args_list(optional_args)
+    args.append(color_index)
     send_cmd("tv_SoundClipAdjust", track_index, *args, error_values=[-2, -3])
 
 
 def tv_layer_image_get() -> int:
     """Get the current frame of the current clip."""
     return int(send_cmd("tv_LayerGetImage"))
```

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/grg_layer.py` & `pytvpaint-1.0.0b9/pytvpaint/george/grg_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1209,15 +1209,15 @@
         GeorgeError: if the file couldn't be saved or an invalid format was provided
     """
     export_path = Path(export_path)
     send_cmd("tv_SaveImage", export_path.as_posix())
 
 
 @try_cmd(exception_msg="Invalid image format")
-def tv_load_image(img_path: Path | str, stretch: bool | None = None) -> None:
+def tv_load_image(img_path: Path | str, stretch: bool = False) -> None:
     """Load an image in the current image layer.
 
     Raises:
         FileNotFoundError: if the input file doesn't exist
         GeorgeError: if the provided file is in an invalid format
     """
     img_path = Path(img_path)
```

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/grg_project.py` & `pytvpaint-1.0.0b9/pytvpaint/george/grg_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from pathlib import Path
 from typing import Any
 
 from pytvpaint.george.client import send_cmd, try_cmd
 from pytvpaint.george.client.parse import (
     tv_cast_to_type,
     tv_parse_list,
-    validate_args_list,
 )
 from pytvpaint.george.exceptions import NoObjectWithIdError
 from pytvpaint.george.grg_base import (
     FieldOrder,
     GrgErrorValue,
     ResizeOption,
     RGBColor,
@@ -123,29 +122,29 @@
         field_order.value,
         start_frame,
         error_values=[GrgErrorValue.EMPTY],
     )
 
 
 @try_cmd(exception_msg="Invalid format")
-def tv_load_project(project_path: Path | str, silent: bool | None = None) -> str:
+def tv_load_project(project_path: Path | str, silent: bool = False) -> str:
     """Load a file as a project if possible or open Import panel.
 
     Raises:
         FileNotFoundError: if the project file doesn't exist
         GeorgeError: if the provided file is in an invalid format
     """
     project_path = Path(project_path)
 
     if not project_path.exists():
         raise FileNotFoundError(f"Project not found at: {project_path.as_posix()}")
 
     args: list[Any] = [project_path.as_posix()]
 
-    if silent is not None:
+    if silent:
         args.extend(["silent", int(silent)])
 
     return send_cmd("tv_LoadProject", *args, error_values=[-1])
 
 
 def tv_save_project(project_path: Path | str) -> None:
     """Save the current project as tvpp."""
@@ -251,15 +250,15 @@
 def tv_get_field() -> FieldOrder:
     """Get the current project field mode."""
     return tv_cast_to_type(send_cmd("tv_GetField"), cast_type=FieldOrder)
 
 
 def tv_project_save_sequence(
     export_path: Path | str,
-    use_camera: bool | None = None,
+    use_camera: bool = False,
     start: int | None = None,
     end: int | None = None,
 ) -> None:
     """Save the current project."""
     export_path = Path(export_path).resolve()
     args: list[Any] = [export_path.as_posix()]
 
@@ -310,17 +309,15 @@
         args = ["timestretch"]
     if preview:
         args = ["preview"]
     args.insert(0, frame_rate)
     send_cmd("tv_FrameRate", *args)
 
 
-def tv_frame_rate_project_set(
-    frame_rate: float, time_stretch: bool | None = None
-) -> None:
+def tv_frame_rate_project_set(frame_rate: float, time_stretch: bool = False) -> None:
     """Set the framerate of the current project."""
     args: list[Any] = [frame_rate]
     if time_stretch:
         args.append("timestretch")
     send_cmd("tv_FrameRate", *args)
 
 
@@ -423,30 +420,31 @@
     fade_in_start: float | None = None,
     fade_in_stop: float | None = None,
     fade_out_start: float | None = None,
     fade_out_stop: float | None = None,
     color_index: int | None = None,
 ) -> None:
     """Change the current project's soundtrack settings."""
+    cur_options = tv_sound_project_info(tv_project_current_id(), track_index)
+    args: list[int | float | None] = []
+
     optional_args = [
-        int(mute) if mute is not None else None,
-        volume,
-        offset,
-        (fade_in_start, fade_in_stop, fade_out_start, fade_out_stop),
-        color_index,
+        (int(mute) if mute is not None else None, int(cur_options.mute)),
+        (volume, cur_options.volume),
+        (offset, cur_options.offset),
+        (fade_in_start, cur_options.fade_in_start),
+        (fade_in_stop, cur_options.fade_in_stop),
+        (fade_out_start, cur_options.fade_out_start),
+        (fade_out_stop, cur_options.fade_out_stop),
     ]
+    for arg, default_value in optional_args:
+        args.append(arg if arg is not None else default_value)
 
-    args = validate_args_list(optional_args)
-
-    send_cmd(
-        "tv_SoundProjectAdjust",
-        track_index,
-        *args,
-        error_values=[-2, -3],
-    )
+    args.append(color_index)
+    send_cmd("tv_SoundProjectAdjust", track_index, *args, error_values=[-2, -3])
 
 
 @try_cmd(
     raise_exc=NoObjectWithIdError,
     exception_msg="Invalid project id",
 )
 def tv_project_header_info_get(project_id: str) -> str:
```

### Comparing `pytvpaint-1.0.0b8/pytvpaint/george/grg_scene.py` & `pytvpaint-1.0.0b9/pytvpaint/george/grg_scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/layer.py` & `pytvpaint-1.0.0b9/pytvpaint/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -781,14 +781,16 @@
             color: the layer color
             image: the background image to load
             stretch: whether to stretch the image to fit the view
 
         Returns:
             Layer: the new animation layer
         """
+        from pytvpaint.clip import Clip
+
         clip = clip or Clip.current_clip()
         layer = cls.new(name, clip, color)
         layer.pre_behavior = george.LayerBehavior.HOLD
         layer.post_behavior = george.LayerBehavior.HOLD
         layer.thumbnails_visible = True
 
         image = Path(image or "")
```

### Comparing `pytvpaint-1.0.0b8/pytvpaint/project.py` & `pytvpaint-1.0.0b9/pytvpaint/project.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/scene.py` & `pytvpaint-1.0.0b9/pytvpaint/scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/sound.py` & `pytvpaint-1.0.0b9/pytvpaint/sound.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/pytvpaint/utils.py` & `pytvpaint-1.0.0b9/pytvpaint/utils.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b8/PKG-INFO` & `pytvpaint-1.0.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytvpaint
-Version: 1.0.0b8
+Version: 1.0.0b9
 Summary: Python scripting for TVPaint
 Home-page: https://github.com/brunchstudio/pytvpaint
 License: MIT
 Keywords: tvpaint,brunch,tvp,george
 Author: Brunch Studio Developers
 Author-email: dev@brunchstudio.tv
 Requires-Python: >=3.9
@@ -32,15 +32,15 @@
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/brunchstudio/pytvpaint/main/docs/assets/pytvpaint_code_banner.png" width=700 />
 </p>
 
 **PyTVPaint** is a type-safe Python library that wraps the George programming language commands in order to interact with the 2D animation software TVPaint.
 
-It communicates through WebSocket to a [custom C++ plugin](https://github.com/brunchstudio/tvpaint-rpc) running in an opened TVPaint instance.
+It communicates through WebSocket to a [custom C++ plugin](https://github.com/brunchstudio/tvpaint-rpc) running in an open TVPaint instance.
 
 You can check the [documentation](https://brunchstudio.github.io/pytvpaint/) for more details.
 
 ## Installation
 
 ### Requirements
 
@@ -48,15 +48,15 @@
 - Python v3.9+
 - TVPaint v11.5+
 - TVPaint RPC plugin (install instructions [here](https://brunchstudio.github.io/pytvpaint/installation/#tvpaint-plugin-installation))
 
 Install the package with Pip:
 
 ```console
-❯ pip install pytvpaint
+pip install pytvpaint
 ```
 
 ## Simple example
 
 ```python
 from pytvpaint import george
 from pytvpaint.project import Project
```

