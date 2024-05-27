# Comparing `tmp/slack_time_localization_bot-0.1.8.tar.gz` & `tmp/slack_time_localization_bot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_time_localization_bot-0.1.8.tar", max compression
+gzip compressed data, was "slack_time_localization_bot-0.1.9.tar", max compression
```

## Comparing `slack_time_localization_bot-0.1.8.tar` & `slack_time_localization_bot-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5810 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/LICENSE
--rw-r--r--   0        0        0     4399 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/README.md
--rw-r--r--   0        0        0     1000 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/__init__.py
--rw-r--r--   0        0        0     5236 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/app.py
--rw-r--r--   0        0        0     3951 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/app_test.py
--rw-r--r--   0        0        0     1159 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/cli.py
--rw-r--r--   0        0        0      865 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/cli_test.py
--rw-r--r--   0        0        0     7091 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/parsing.py
--rw-r--r--   0        0        0     3543 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/parsing_test.py
--rw-r--r--   0        0        0      197 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/utils.py
--rw-r--r--   0        0        0      412 2024-02-29 12:51:20.747979 slack_time_localization_bot-0.1.8/slack_time_localization_bot/utils_test.py
--rw-r--r--   0        0        0     5614 1970-01-01 00:00:00.000000 slack_time_localization_bot-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     6684 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4399 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/README.md
+-rw-r--r--   0        0        0     1000 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/__init__.py
+-rw-r--r--   0        0        0     5365 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/app.py
+-rw-r--r--   0        0        0     3951 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/app_test.py
+-rw-r--r--   0        0        0     1159 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/cli.py
+-rw-r--r--   0        0        0      865 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/cli_test.py
+-rw-r--r--   0        0        0     8634 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/parsing.py
+-rw-r--r--   0        0        0     4411 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/parsing_test.py
+-rw-r--r--   0        0        0      197 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/utils.py
+-rw-r--r--   0        0        0      412 2024-03-01 09:52:30.075922 slack_time_localization_bot-0.1.9/slack_time_localization_bot/utils_test.py
+-rw-r--r--   0        0        0     5614 1970-01-01 00:00:00.000000 slack_time_localization_bot-0.1.9/PKG-INFO
```

### Comparing `slack_time_localization_bot-0.1.8/CHANGELOG.md` & `slack_time_localization_bot-0.1.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## [v0.1.9](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/tree/v0.1.9) (2024-03-01)
+
+[Full Changelog](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/compare/v0.1.8...v0.1.9)
+
+**Merged pull requests:**
+
+- Omit UTC time from message if original temporal expression already was in UTC [\#20](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/pull/20) ([phihos](https://github.com/phihos))
+- Split fake intervals like "15:00 \(UTC\) / 16:00 \(CET\)" into separate expressions [\#19](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/pull/19) ([phihos](https://github.com/phihos))
+- Support timezones in round braces like \("15:00 \(UTC\)"\) [\#18](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/pull/18) ([phihos](https://github.com/phihos))
+
 ## [v0.1.8](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/tree/v0.1.8) (2024-02-29)
 
 [Full Changelog](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/compare/v0.1.7...v0.1.8)
 
 **Merged pull requests:**
 
 - Support half-intervals \("since 9:00", "until 9:00"\) [\#17](https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot/pull/17) ([phihos](https://github.com/phihos))
```

### Comparing `slack_time_localization_bot-0.1.8/LICENSE` & `slack_time_localization_bot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_time_localization_bot-0.1.8/README.md` & `slack_time_localization_bot-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `slack_time_localization_bot-0.1.8/pyproject.toml` & `slack_time_localization_bot-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slack-time-localization-bot"
-version = "0.1.8"
+version = "0.1.9"
 description = "Detect temporal expressions in Slack messages (\"tomorrow at 5 pm\") and translate them for readers in other timezones."
 authors = ["Philipp Hossner <philipp.hossner@posteo.de>"]
 readme = "README.md"
 repository = "https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot"
 license = "MIT"
 include = ["CHANGELOG.md"]
```

### Comparing `slack_time_localization_bot-0.1.8/slack_time_localization_bot/app.py` & `slack_time_localization_bot-0.1.9/slack_time_localization_bot/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -53,21 +53,24 @@
         )
 
     def time_comparison_to_text(
         self,
         temporal_expression: TemporalExpression,
         user_timezone: datetime.tzinfo,
     ) -> str:
-        return (
+        message = (
             f"> {temporal_expression.text}\n"
             f"_{temporal_expression.datetime.astimezone(temporal_expression.timezone).strftime(self.time_format)} "
             f"({temporal_expression.timezone})_ ➔ "
-            f"_{temporal_expression.datetime.astimezone(user_timezone).strftime(self.time_format)} ({user_timezone})_ "
-            f"or _{temporal_expression.datetime.astimezone(ZoneInfo('UTC')).strftime(self.time_format)} (UTC)_"
+            f"_{temporal_expression.datetime.astimezone(user_timezone).strftime(self.time_format)} ({user_timezone})_"
         )
+        if temporal_expression.timezone != ZoneInfo("UTC"):
+            utc_time = temporal_expression.datetime.astimezone(ZoneInfo('UTC')).strftime(self.time_format)
+            message += f" or _{utc_time} (UTC)_"
+        return message
 
     def process_message(self, client: WebClient, message):
         channel_id = message["channel"]
         thread_id = message.get("thread_ts", None)
         poster_id = message["user"]
         text = sanitize_message_text(message["text"])
```

### Comparing `slack_time_localization_bot-0.1.8/slack_time_localization_bot/app_test.py` & `slack_time_localization_bot-0.1.9/slack_time_localization_bot/app_test.py`

 * *Files identical despite different names*

### Comparing `slack_time_localization_bot-0.1.8/slack_time_localization_bot/cli.py` & `slack_time_localization_bot-0.1.9/slack_time_localization_bot/cli.py`

 * *Files identical despite different names*

### Comparing `slack_time_localization_bot-0.1.8/slack_time_localization_bot/cli_test.py` & `slack_time_localization_bot-0.1.9/slack_time_localization_bot/cli_test.py`

 * *Files identical despite different names*

### Comparing `slack_time_localization_bot-0.1.8/slack_time_localization_bot/parsing.py` & `slack_time_localization_bot-0.1.9/slack_time_localization_bot/parsing.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     .with_minimum_relative_distance(0.3)
     .build()
 )
 time_zones = load_time_zones("/usr/share/zoneinfo")
 
 # initializations that should be done once on module load
 logger = logging.getLogger(__name__)
-timezone_regex = re.compile(r" (\L<tz>)", tz=zoneinfo.available_timezones())
+timezone_regex = re.compile(r"[ (]((?i)\L<tz>)", tz=zoneinfo.available_timezones())
+timezone_case_insensitive_search_map = {
+    timezone.lower(): timezone for timezone in zoneinfo.available_timezones()
+}
 
 
 @dataclass
 class TemporalExpression:
     text: str
     datetime: datetime.datetime
     timezone: datetime.tzinfo
@@ -42,18 +45,26 @@
     if len(text) >= 5:
         language = detector.detect_language_of(text)
         if language:
             return language.iso_code_639_1.name
     return "EN"
 
 
-def detect_timezone(text: str) -> Optional[datetime.tzinfo]:
-    match = timezone_regex.search(text)
-    if match:
-        return ZoneInfo(match.group(1))
+def detect_timezones(text: str) -> List[datetime.tzinfo]:
+    matches = timezone_regex.findall(text)
+    return [
+        ZoneInfo(timezone_case_insensitive_search_map[match.lower()])
+        for match in matches
+    ]
+
+
+def detect_single_timezone(text: str) -> Optional[datetime.tzinfo]:
+    timezones = detect_timezones(text)
+    if timezones:
+        return timezones[0]
     return None
 
 
 def select_time_values_based_on_24h_preference(
     candidates: List[datetime.datetime],
 ):
     """Pick the datetime which is most likely correct for a text written in 24h format.
@@ -107,72 +118,101 @@
                     if prefer_24h_interpretation
                     else candidates[0]
                 )
                 return_value.append(
                     TemporalExpression(
                         text=result["body"],
                         datetime=chosen_datetime,
-                        timezone=detect_timezone(result["body"])
+                        timezone=detect_single_timezone(result["body"])
                         or reference_time.tzinfo,
                     )
                 )
         elif result["value"]["type"] == "interval":
-            interval_timezone = detect_timezone(result["body"])
+            interval_timezones = detect_timezones(result["body"])
+            if len(interval_timezones) >= 2:
+                # this is very likely not a real interval, but two temporal expressions falsely recognized as such
+                # for example 15:00 (UTC) / 16:00 (CET)
+                # we split this into two expressions and rerun this logic for each individually
+                parts = re.split(
+                    f"({str(interval_timezones[0])}[^ ])",
+                    text,
+                    maxsplit=1,
+                    flags=re.IGNORECASE,
+                )
+                first_expression = (
+                    parts[0]
+                    + parts[
+                        1
+                    ]  # given the example above this will contain "15:00 (UTC)"
+                )
+                second_expression = parts[-1]
+                return_value += text_to_temporal_expressions(
+                    first_expression,
+                    reference_time.astimezone(interval_timezones[0]),
+                    prefer_24h_interpretation,
+                )
+                return_value += text_to_temporal_expressions(
+                    second_expression,
+                    reference_time.astimezone(interval_timezones[1]),
+                    prefer_24h_interpretation,
+                )
+                continue
+            interval_timezone = interval_timezones[0] if interval_timezones else None
             if interval_timezone and interval_timezone != reference_time.tzinfo:
                 return_value += text_to_temporal_expressions(
                     result["body"],
                     reference_time.astimezone(interval_timezone),
                     prefer_24h_interpretation,
                 )
-            else:
-                if "from" in result["value"]:
-                    from_candidates = [
-                        isoparse(x["from"]["value"])
-                        for x in result["value"]["values"]
-                        if x["from"]["grain"] != "day"
-                    ]
-                    if from_candidates:
-                        chosen_from_datetime = (
-                            select_time_values_based_on_24h_preference(from_candidates)
-                            if prefer_24h_interpretation
-                            else from_candidates[0]
+                continue
+            if "from" in result["value"]:
+                from_candidates = [
+                    isoparse(x["from"]["value"])
+                    for x in result["value"]["values"]
+                    if x["from"]["grain"] != "day"
+                ]
+                if from_candidates:
+                    chosen_from_datetime = (
+                        select_time_values_based_on_24h_preference(from_candidates)
+                        if prefer_24h_interpretation
+                        else from_candidates[0]
+                    )
+                    return_value.append(
+                        TemporalExpression(
+                            text=result["body"],
+                            datetime=chosen_from_datetime,
+                            timezone=detect_single_timezone(result["body"])
+                            or reference_time.tzinfo,
                         )
-                        return_value.append(
-                            TemporalExpression(
-                                text=result["body"],
-                                datetime=chosen_from_datetime,
-                                timezone=detect_timezone(result["body"])
-                                or reference_time.tzinfo,
+                    )
+            if "to" in result["value"]:
+                to_candidates = [
+                    isoparse(x["to"]["value"])
+                    for x in result["value"]["values"]
+                    if x["to"]["grain"] != "day"
+                ]
+                if to_candidates:
+                    chosen_to_datetime = (
+                        select_time_values_based_on_24h_preference(to_candidates)
+                        if prefer_24h_interpretation
+                        else to_candidates[0]
+                    )
+                    # correct interval end datetime
+                    if "from" in result["value"]:
+                        # for unknown reasons the time does not need to be corrected in half-intervals
+                        if result["value"]["to"]["grain"] == "minute":
+                            chosen_to_datetime = (
+                                chosen_to_datetime - datetime.timedelta(minutes=1)
                             )
-                        )
-                if "to" in result["value"]:
-                    to_candidates = [
-                        isoparse(x["to"]["value"])
-                        for x in result["value"]["values"]
-                        if x["to"]["grain"] != "day"
-                    ]
-                    if to_candidates:
-                        chosen_to_datetime = (
-                            select_time_values_based_on_24h_preference(to_candidates)
-                            if prefer_24h_interpretation
-                            else to_candidates[0]
-                        )
-                        # correct interval end datetime
-                        if "from" in result["value"]:
-                            # for unknown reasons the time does not need to be corrected in half-intervals
-                            if result["value"]["to"]["grain"] == "minute":
-                                chosen_to_datetime = (
-                                    chosen_to_datetime - datetime.timedelta(minutes=1)
-                                )
-                            elif result["value"]["to"]["grain"] == "hour":
-                                chosen_to_datetime = (
-                                    chosen_to_datetime - datetime.timedelta(hours=1)
-                                )
-                        return_value.append(
-                            TemporalExpression(
-                                text=result["body"],
-                                datetime=chosen_to_datetime,
-                                timezone=detect_timezone(result["body"])
-                                or reference_time.tzinfo,
+                        elif result["value"]["to"]["grain"] == "hour":
+                            chosen_to_datetime = (
+                                chosen_to_datetime - datetime.timedelta(hours=1)
                             )
+                    return_value.append(
+                        TemporalExpression(
+                            text=result["body"],
+                            datetime=chosen_to_datetime,
+                            timezone=detect_single_timezone(result["body"])
+                            or reference_time.tzinfo,
                         )
+                    )
     return return_value
```

### Comparing `slack_time_localization_bot-0.1.8/slack_time_localization_bot/parsing_test.py` & `slack_time_localization_bot-0.1.9/slack_time_localization_bot/parsing_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from zoneinfo import ZoneInfo
 
 import pytest
 
 from slack_time_localization_bot.parsing import (
     detect_language,
     text_to_temporal_expressions,
-    detect_timezone,
+    detect_single_timezone,
 )
 
 TEST_DETECT = [
     ("Let us meet at 11 am or 1 pm.", "EN"),
     ("Lass uns um 11 oder 13 Uhr treffen.", "DE"),
     ("F", "EN"),
     ("10:00 GMT", "EN"),
@@ -27,15 +27,15 @@
     ("Let us meet at 11 am.", None),
     ("Let us meet at 11 UTC.", ZoneInfo("UTC")),
 ]
 
 
 @pytest.mark.parametrize("test_input,expected", TEST_DETECT_TZ)
 def test_detect_timezone(test_input, expected):
-    assert detect_timezone(test_input) == expected
+    assert detect_single_timezone(test_input) == expected
 
 
 REFERENCE_TZ = ZoneInfo("CET")
 REFERENCE_DATETIME = datetime.datetime(2023, 2, 17, 18, 17, tzinfo=REFERENCE_TZ)
 
 
 def today(hour: int = 0, minute: int = 0, tzinfo=REFERENCE_TZ) -> datetime.datetime:
@@ -63,14 +63,22 @@
         True,
     ),
     (
         "Let us meet today at 20:53 UTC.",
         [today(20, 53, tzinfo=ZoneInfo("UTC"))],
         True,
     ),
+    (
+        "15:00 (UTC) / 16:00 (CET)",
+        [
+            tomorrow(15, 00, tzinfo=ZoneInfo("UTC")),
+            tomorrow(16, 00, tzinfo=ZoneInfo("CET")),
+        ],
+        True,
+    ),
     ("Lass uns morgen um 11 oder 13 Uhr treffen.", [tomorrow(11), tomorrow(13)], True),
     ("Lasst uns heute um 11 treffen.", [today(11)], True),
     (
         "Lasst uns morgen um 11:00 EST treffen.",
         [tomorrow(11, tzinfo=ZoneInfo("EST"))],
         True,
     ),
@@ -123,7 +131,32 @@
 )
 def test_text_to_times(test_input, expected, prefer_24h_interpretation):
     results = text_to_temporal_expressions(
         test_input, REFERENCE_DATETIME, prefer_24h_interpretation
     )
     all_datetimes = [result.datetime for result in results]
     assert all_datetimes == expected
+
+
+TEST_TEXT_TO_TIMES_TIMEZONES = [
+    (
+        "15:00 (UTC) / 16:00 (CET)",
+        [ZoneInfo("UTC"), ZoneInfo("CET")],
+        True,
+    ),
+    (
+        "15:00 (utc) / 16:00 (cet)",
+        [ZoneInfo("UTC"), ZoneInfo("CET")],
+        True,
+    ),
+]
+
+
+@pytest.mark.parametrize(
+    "test_input,expected,prefer_24h_interpretation", TEST_TEXT_TO_TIMES_TIMEZONES
+)
+def test_text_to_times_timezones(test_input, expected, prefer_24h_interpretation):
+    results = text_to_temporal_expressions(
+        test_input, REFERENCE_DATETIME, prefer_24h_interpretation
+    )
+    all_timezones = [result.timezone for result in results]
+    assert all_timezones == expected
```

### Comparing `slack_time_localization_bot-0.1.8/PKG-INFO` & `slack_time_localization_bot-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-time-localization-bot
-Version: 0.1.8
+Version: 0.1.9
 Summary: Detect temporal expressions in Slack messages ("tomorrow at 5 pm") and translate them for readers in other timezones.
 Home-page: https://github.com/Slack-Time-Localization-Bot/Slack-Time-Localization-Bot
 License: MIT
 Author: Philipp Hossner
 Author-email: philipp.hossner@posteo.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

