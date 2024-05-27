# Comparing `tmp/pdftext-0.3.8.tar.gz` & `tmp/pdftext-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdftext-0.3.8.tar", max compression
+gzip compressed data, was "pdftext-0.3.9.tar", max compression
```

## Comparing `pdftext-0.3.8.tar` & `pdftext-0.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11269 2024-05-23 19:30:54.933288 pdftext-0.3.8/LICENSE
--rw-r--r--   0        0        0     7180 2024-05-23 19:30:54.933288 pdftext-0.3.8/README.md
--rw-r--r--   0        0        0     1904 2024-05-23 19:30:54.933288 pdftext-0.3.8/extract_text.py
--rw-r--r--   0        0        0    14097 2024-05-23 19:30:54.933288 pdftext-0.3.8/models/dt.joblib
--rw-r--r--   0        0        0     3700 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/extraction.py
--rw-r--r--   0        0        0     7382 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/inference.py
--rw-r--r--   0        0        0      153 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/model.py
--rw-r--r--   0        0        0     3811 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/pdf/chars.py
--rw-r--r--   0        0        0     4613 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/pdf/utils.py
--rw-r--r--   0        0        0     3222 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/postprocessing.py
--rw-r--r--   0        0        0      569 2024-05-23 19:30:54.933288 pdftext-0.3.8/pdftext/settings.py
--rw-r--r--   0        0        0      856 2024-05-23 19:30:54.933288 pdftext-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     8156 1970-01-01 00:00:00.000000 pdftext-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11269 2024-05-24 18:00:24.775289 pdftext-0.3.9/LICENSE
+-rw-r--r--   0        0        0     7180 2024-05-24 18:00:24.775289 pdftext-0.3.9/README.md
+-rw-r--r--   0        0        0     1904 2024-05-24 18:00:24.775289 pdftext-0.3.9/extract_text.py
+-rw-r--r--   0        0        0    14097 2024-05-24 18:00:24.775289 pdftext-0.3.9/models/dt.joblib
+-rw-r--r--   0        0        0     3573 2024-05-24 18:00:24.775289 pdftext-0.3.9/pdftext/extraction.py
+-rw-r--r--   0        0        0     7584 2024-05-24 18:00:24.775289 pdftext-0.3.9/pdftext/inference.py
+-rw-r--r--   0        0        0      153 2024-05-24 18:00:24.775289 pdftext-0.3.9/pdftext/model.py
+-rw-r--r--   0        0        0     3753 2024-05-24 18:00:24.775289 pdftext-0.3.9/pdftext/pdf/chars.py
+-rw-r--r--   0        0        0     4180 2024-05-24 18:00:24.775289 pdftext-0.3.9/pdftext/pdf/utils.py
+-rw-r--r--   0        0        0     3222 2024-05-24 18:00:24.779289 pdftext-0.3.9/pdftext/postprocessing.py
+-rw-r--r--   0        0        0      569 2024-05-24 18:00:24.779289 pdftext-0.3.9/pdftext/settings.py
+-rw-r--r--   0        0        0      856 2024-05-24 18:00:24.779289 pdftext-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     8156 1970-01-01 00:00:00.000000 pdftext-0.3.9/PKG-INFO
```

### Comparing `pdftext-0.3.8/LICENSE` & `pdftext-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.8/README.md` & `pdftext-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.8/extract_text.py` & `pdftext-0.3.9/extract_text.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.8/models/dt.joblib` & `pdftext-0.3.9/models/dt.joblib`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.8/pdftext/extraction.py` & `pdftext-0.3.9/pdftext/extraction.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,34 +57,34 @@
     pages = _get_pages(pdf_path, model, page_range, workers=workers)
     text = []
     for page in pages:
         text.append(merge_text(page, sort=sort, hyphens=hyphens).strip())
     return text
 
 
+def _process_span(span, page_width, page_height, keep_chars):
+    span["bbox"] = unnormalize_bbox(span["bbox"], page_width, page_height)
+    span["text"] = handle_hyphens(postprocess_text(span["text"]), keep_hyphens=True)
+    if not keep_chars:
+        del span["chars"]
+    else:
+        for char in span["chars"]:
+            char["bbox"] = unnormalize_bbox(char["bbox"], page_width, page_height)
+
+
 def dictionary_output(pdf_path, sort=False, model=None, page_range=None, keep_chars=False, workers=None):
     pages = _get_pages(pdf_path, model, page_range, workers=workers)
     for page in pages:
+        page_width, page_height = page["width"], page["height"]
         for block in page["blocks"]:
-            bad_keys = [key for key in block.keys() if key not in ["lines", "bbox"]]
-            for key in bad_keys:
-                del block[key]
+            block = {k: v for k, v in block.items() if k in ["lines", "bbox"]}
+            block["bbox"] = unnormalize_bbox(block["bbox"], page_width, page_height)
             for line in block["lines"]:
-                bad_keys = [key for key in line.keys() if key not in ["bbox", "spans"]]
-                for key in bad_keys:
-                    del line[key]
+                line = {k: v for k, v in line.items() if k in ["bbox", "spans"]}
+                line["bbox"] = unnormalize_bbox(line["bbox"], page_width, page_height)
                 for span in line["spans"]:
-                    span["bbox"] = unnormalize_bbox(span["bbox"], page["width"], page["height"])
-                    span["text"] = postprocess_text(span["text"])
-                    span["text"] = handle_hyphens(span["text"], keep_hyphens=True)
-
-                    if not keep_chars:
-                        del span["chars"]
-                    else:
-                        for char in span["chars"]:
-                            char["bbox"] = unnormalize_bbox(char["bbox"], page["width"], page["height"])
+                    _process_span(span, page_width, page_height, keep_chars)
 
-                line["bbox"] = unnormalize_bbox(line["bbox"], page["width"], page["height"])
-            block["bbox"] = unnormalize_bbox(block["bbox"], page["width"], page["height"])
         if sort:
             page["blocks"] = sort_blocks(page["blocks"])
+
     return pages
```

### Comparing `pdftext-0.3.8/pdftext/inference.py` & `pdftext-0.3.9/pdftext/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,94 +5,105 @@
 from pdftext.pdf.utils import LINE_BREAKS, TABS, SPACES
 from pdftext.settings import settings
 
 
 def update_current(current, new_char):
     bbox = new_char["bbox"]
     if "bbox" not in current:
-        current_bbox = bbox.copy()
-        current["bbox"] = current_bbox
+        current["bbox"] = bbox.copy()
     else:
         current_bbox = current["bbox"]
         current_bbox[0] = min(bbox[0], current_bbox[0])
         current_bbox[1] = min(bbox[1], current_bbox[1])
         current_bbox[2] = max(bbox[2], current_bbox[2])
         current_bbox[3] = max(bbox[3], current_bbox[3])
+    current_bbox = current["bbox"]
     current["center_x"] = (current_bbox[0] + current_bbox[2]) / 2
     current["center_y"] = (current_bbox[1] + current_bbox[3]) / 2
 
 
 def create_training_row(char_info, prev_char, currblock, currline):
     char = char_info["char"]
 
     # Store variables used multiple times
-    char_x1, char_y1, char_x2, char_y2 = char_info["bbox"]
-    prev_x1, prev_y1, prev_x2, prev_y2 = prev_char["bbox"]
+    char_bbox = char_info["bbox"]
+    prev_bbox = prev_char["bbox"]
+    currblock_bbox = currblock["bbox"]
+    currline_bbox = currline["bbox"]
+
+    char_x1, char_y1, char_x2, char_y2 = char_bbox
+    prev_x1, prev_y1, prev_x2, prev_y2 = prev_bbox
     char_center_x = (char_x2 + char_x1) / 2
     char_center_y = (char_y2 + char_y1) / 2
     x_gap = char_x1 - prev_x2
     y_gap = char_y1 - prev_y2
 
     char_font = char_info["font"]
     prev_font = prev_char["font"]
-    font_match = all(
-        [char_font[key] == prev_font[key] for key in ["name", "size", "weight", "flags"]] +
-        [char_info["rotation"] == prev_char["rotation"]]
-    )
-    is_space = any([
-        char in SPACES,
-        char in TABS,
-    ])
+    font_match = (char_font["name"] == prev_font["name"] and
+                  char_font["size"] == prev_font["size"] and
+                  char_font["weight"] == prev_font["weight"] and
+                  char_font["flags"] == prev_font["flags"] and
+                  char_info["rotation"] == prev_char["rotation"])
+
+    is_space = char in SPACES or char in TABS
 
     training_row = {
         "is_newline": char in LINE_BREAKS,
         "is_space": is_space,
         "x_gap": x_gap,
         "y_gap": y_gap,
         "font_match": font_match,
         "x_outer_gap": char_x2 - prev_x1,
         "y_outer_gap": char_y2 - prev_y1,
         "line_x_center_gap": char_center_x - currline["center_x"],
         "line_y_center_gap": char_center_y - currline["center_y"],
-        "line_x_gap": char_x1 - currline["bbox"][2],
-        "line_y_gap": char_y1 - currline["bbox"][3],
-        "line_x_start_gap": char_x1 - currline["bbox"][0],
-        "line_y_start_gap": char_y1 - currline["bbox"][1],
+        "line_x_gap": char_x1 - currline_bbox[2],
+        "line_y_gap": char_y1 - currline_bbox[3],
+        "line_x_start_gap": char_x1 - currline_bbox[0],
+        "line_y_start_gap": char_y1 - currline_bbox[1],
         "block_x_center_gap": char_center_x - currblock["center_x"],
         "block_y_center_gap": char_center_y - currblock["center_y"],
-        "block_x_gap": char_x1 - currblock["bbox"][2],
-        "block_y_gap": char_y1 - currblock["bbox"][3],
-        "block_x_start_gap": char_x1 - currblock["bbox"][0],
-        "block_y_start_gap": char_y1 - currblock["bbox"][1]
+        "block_x_gap": char_x1 - currblock_bbox[2],
+        "block_y_gap": char_y1 - currblock_bbox[3],
+        "block_x_start_gap": char_x1 - currblock_bbox[0],
+        "block_y_start_gap": char_y1 - currblock_bbox[1]
     }
 
     return training_row
 
 
 def update_span(line, span):
-    if len(span["chars"]) > 0:
-        span["font"] = span["chars"][0]["font"]
-        span["rotation"] = span["chars"][0]["rotation"]
+    if span["chars"]:
+        first_char = span["chars"][0]
+        span["font"] = first_char["font"]
+        span["rotation"] = first_char["rotation"]
+
         char_bboxes = [char["bbox"] for char in span["chars"]]
-        span["bbox"] = [min([bbox[0] for bbox in char_bboxes]),
-                        min([bbox[1] for bbox in char_bboxes]),
-                        max([bbox[2] for bbox in char_bboxes]),
-                        max([bbox[3] for bbox in char_bboxes])]
-        span["text"] = "".join([char["char"] for char in span["chars"]])
-        span["char_start_idx"] = span["chars"][0]["char_idx"]
+        min_x, min_y, max_x, max_y = char_bboxes[0]
+
+        for bbox in char_bboxes[1:]:
+            min_x = min(min_x, bbox[0])
+            min_y = min(min_y, bbox[1])
+            max_x = max(max_x, bbox[2])
+            max_y = max(max_y, bbox[3])
+
+        span["bbox"] = [min_x, min_y, max_x, max_y]
+        span["text"] = "".join(char["char"] for char in span["chars"])
+        span["char_start_idx"] = first_char["char_idx"]
         span["char_end_idx"] = span["chars"][-1]["char_idx"]
 
-    # Remove unneeded keys from the characters
-    for char in span["chars"]:
-        del_keys = [k for k in list(char.keys()) if k not in ["char", "bbox"]]
-        for key in del_keys:
-            del char[key]
-    line["spans"].append(span)
-    span = {"chars": []}
-    return span
+        # Remove unneeded keys from the characters
+        for char in span["chars"]:
+            for key in list(char.keys()):
+                if key not in ["char", "bbox"]:
+                    del char[key]
+
+        line["spans"].append(span)
+    return {"chars": []}
 
 
 def update_line(block, line):
     block["lines"].append(line)
     line = {"spans": []}
     return line
 
@@ -114,16 +125,18 @@
         "bbox": text_chars["bbox"],
         "width": text_chars["width"],
         "height": text_chars["height"],
     }
     block = {"lines": []}
     line = {"spans": []}
     span = {"chars": []}
-    for i, char_info in enumerate(text_chars["chars"]):
-        font_info = f"{char_info['font']['name']}_{char_info['font']['size']}_{char_info['font']['weight']}_{char_info['font']['flags']}_{char_info['rotation']}"
+
+    for char_info in text_chars["chars"]:
+        font = char_info['font']
+        font_info = f"{font['name']}_{font['size']}_{font['weight']}_{font['flags']}_{char_info['rotation']}"
         if prev_char:
             training_row = create_training_row(char_info, prev_char, block, line)
             sorted_keys = sorted(training_row.keys())
             training_row = [training_row[key] for key in sorted_keys]
 
             prediction_probs = yield training_row
             # First item is probability of same line/block, second is probability of new line, third is probability of new block
@@ -143,19 +156,20 @@
 
         span["chars"].append(char_info)
         update_current(line, char_info)
         update_current(block, char_info)
 
         prev_char = char_info
         prev_font_info = font_info
-    if len(span["chars"]) > 0:
+
+    if span["chars"]:
         update_span(line, span)
-    if len(line["spans"]) > 0:
+    if line["spans"]:
         update_line(block, line)
-    if len(block["lines"]) > 0:
+    if block["lines"]:
         update_block(blocks, block)
 
     return blocks
 
 
 def inference(text_chars, model):
     # Create generators and get first training row from each
```

### Comparing `pdftext-0.3.8/pdftext/pdf/chars.py` & `pdftext-0.3.9/pdftext/pdf/chars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import decimal
 import math
-from typing import Dict
+from typing import Dict, List
 
-import pypdfium2 as pdfium
 import pypdfium2.raw as pdfium_c
 
 from pdftext.pdf.utils import get_fontname, pdfium_page_bbox_to_device_bbox, page_bbox_to_device_bbox
 from pdftext.settings import settings
 
 
-def update_previous_fonts(text_chars: Dict, i: int, prev_fontname: str, prev_fontflags: int, text_page, fontname_sample_freq: int):
+def update_previous_fonts(char_infos: List, i: int, prev_fontname: str, prev_fontflags: int, text_page, fontname_sample_freq: int):
     min_update = max(0, i - fontname_sample_freq) # Minimum index to update
     for j in range(i-1, min_update, -1): # Goes from i to min_update
         fontname, fontflags = get_fontname(text_page, j)
 
         # If we hit the region with the previous fontname, we can bail out
         if fontname == prev_fontname and fontflags == prev_fontflags:
             break
-        text_chars["chars"][j]["font"]["name"] = fontname
-        text_chars["chars"][j]["font"]["flags"] = fontflags
+        char_infos[j]["font"]["name"] = fontname
+        char_infos[j]["font"]["flags"] = fontflags
 
 
 def get_pdfium_chars(pdf, page_range, fontname_sample_freq=settings.FONTNAME_SAMPLE_FREQ):
     blocks = []
 
     for page_idx in page_range:
         page = pdf.get_page(page_idx)
@@ -38,42 +36,40 @@
         page_width = math.ceil(abs(bbox[2] - bbox[0]))
         page_height = math.ceil(abs(bbox[1] - bbox[3]))
 
         # Flip width and height if rotated
         if page_rotation == 90 or page_rotation == 270:
             page_width, page_height = page_height, page_width
 
-        bl_origin = all([
-            mediabox[0] == 0,
-            mediabox[1] == 0
-        ])
+        bl_origin = (mediabox[0] == 0 and mediabox[1] == 0)
 
         text_chars = {
-            "chars": [],
             "page": page_idx,
             "rotation": page_rotation,
             "bbox": bbox,
             "width": page_width,
             "height": page_height,
         }
 
         fontname = None
         fontflags = None
         total_chars = text_page.count_chars()
+        char_infos = []
+
         for i in range(total_chars):
             char = pdfium_c.FPDFText_GetUnicode(text_page, i)
             char = chr(char)
             fontsize = round(pdfium_c.FPDFText_GetFontSize(text_page, i), 1)
             fontweight = round(pdfium_c.FPDFText_GetFontWeight(text_page, i), 1)
             if fontname is None or i % fontname_sample_freq == 0:
                 prev_fontname = fontname
                 prev_fontflags = fontflags
                 fontname, fontflags = get_fontname(text_page, i)
                 if (fontname != prev_fontname or fontflags != prev_fontflags) and i > 0:
-                    update_previous_fonts(text_chars, i, prev_fontname, prev_fontflags, text_page, fontname_sample_freq)
+                    update_previous_fonts(char_infos, i, prev_fontname, prev_fontflags, text_page, fontname_sample_freq)
 
             rotation = pdfium_c.FPDFText_GetCharAngle(text_page, i)
             rotation = rotation * 180 / math.pi # convert from radians to degrees
             coords = text_page.get_charbox(i, loose=rotation == 0) # Loose doesn't work properly when charbox is rotated
             device_coords = page_bbox_to_device_bbox(page, coords, page_width, page_height, bl_origin, page_rotation, normalize=True)
 
             char_info = {
@@ -84,12 +80,13 @@
                     "flags": fontflags
                 },
                 "rotation": rotation,
                 "char": char,
                 "bbox": device_coords,
                 "char_idx": i
             }
-            text_chars["chars"].append(char_info)
+            char_infos.append(char_info)
 
+        text_chars["chars"] = char_infos
         text_chars["total_chars"] = total_chars
         blocks.append(text_chars)
     return blocks
```

### Comparing `pdftext-0.3.8/pdftext/pdf/utils.py` & `pdftext-0.3.9/pdftext/pdf/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,22 @@
 import pypdfium2.raw as pdfium_c
 import ctypes
 import math
 
-from pdftext.settings import settings
-
 LINE_BREAKS = ["\n", "\u000D", "\u000A"]
 TABS = ["\t", "\u0009", "\x09"]
 SPACES = [" ", "\ufffe", "\uFEFF", "\xa0"]
 WHITESPACE_CHARS = ["\n", "\r", "\f", "\t", " "]
 
 
-def char_count(textpage, *rect):
-    args = (textpage, *rect)
-    n_chars = pdfium_c.FPDFText_GetBoundedText(*args, None, 0)
-    if n_chars <= 0:
-        return 0
-    return n_chars
-
-
-def normalize_bbox(bbox, page_bound):
-    x1, y1, x2, y2 = bbox
-    x1 = x1 / page_bound[2]
-    y1 = y1 / page_bound[3]
-    x2 = x2 / page_bound[2]
-    y2 = y2 / page_bound[3]
-    return x1, y1, x2, y2
-
-
 def unnormalize_bbox(bbox, page_width, page_height):
-    x1, y1, x2, y2 = bbox
-    x1 = round(x1 * page_width, 1)
-    y1 = round(y1 * page_height, 1)
-    x2 = round(x2 * page_width, 1)
-    y2 = round(y2 * page_height, 1)
+    x1 = round(bbox[0] * page_width, 1)
+    y1 = round(bbox[1] * page_height, 1)
+    x2 = round(bbox[2] * page_width, 1)
+    y2 = round(bbox[3] * page_height, 1)
     return x1, y1, x2, y2
 
 
 def get_fontname(textpage, char_index):
     n_bytes = pdfium_c.FPDFText_GetFontInfo(textpage, char_index, None, 0, None)
     buffer = ctypes.create_string_buffer(n_bytes)
     # Re-interpret the type from char to unsigned short as required by the function
```

### Comparing `pdftext-0.3.8/pdftext/postprocessing.py` & `pdftext-0.3.9/pdftext/postprocessing.py`

 * *Files identical despite different names*

### Comparing `pdftext-0.3.8/pdftext/settings.py` & `pdftext-0.3.9/pdftext/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     MODEL_PATH: str = os.path.join(BASE_PATH, "models", "dt.joblib")
 
     # Fonts
     FONTNAME_SAMPLE_FREQ: int = 4
 
     # Inference
     BLOCK_THRESHOLD: float = 0.8 # Confidence threshold for block detection
-    WORKER_PAGE_THRESHOLD: int = 30 # Min number of pages per worker in parallel
+    WORKER_PAGE_THRESHOLD: int = 10 # Min number of pages per worker in parallel
 
     # Benchmark
     RESULTS_FOLDER: str = "results"
     BENCH_DATASET_NAME: str = "vikp/pdf_bench"
 
 
 settings = Settings()
```

### Comparing `pdftext-0.3.8/pyproject.toml` & `pdftext-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdftext"
-version = "0.3.8"
+version = "0.3.9"
 description = "Extract structured text from pdfs quickly"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/VikParuchuri/pdftext"
 keywords = ["pdf", "text", "extraction"]
 packages = [
```

### Comparing `pdftext-0.3.8/PKG-INFO` & `pdftext-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdftext
-Version: 0.3.8
+Version: 0.3.9
 Summary: Extract structured text from pdfs quickly
 Home-page: https://github.com/VikParuchuri/pdftext
 License: Apache-2.0
 Keywords: pdf,text,extraction
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
```

