# Comparing `tmp/librus_apix-1.0.3.tar.gz` & `tmp/librus_apix-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-1.0.3.tar", last modified: Sat May 25 09:35:06 2024, max compression
+gzip compressed data, was "librus_apix-1.0.4.tar", last modified: Tue May 28 21:25:40 2024, max compression
```

## Comparing `librus_apix-1.0.3.tar` & `librus_apix-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:35:06.422921 librus_apix-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 09:35:03.000000 librus_apix-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 09:35:06.422921 librus_apix-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-25 09:35:03.000000 librus_apix-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:35:06.422921 librus_apix-1.0.3/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-25 09:35:03.000000 librus_apix-1.0.3/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:35:06.422921 librus_apix-1.0.3/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 09:35:06.000000 librus_apix-1.0.3/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 09:35:03.000000 librus_apix-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-25 09:35:06.422921 librus_apix-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:35:03.000000 librus_apix-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:25:40.104798 librus_apix-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 21:25:37.000000 librus_apix-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-28 21:25:40.104798 librus_apix-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-28 21:25:37.000000 librus_apix-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:25:40.100798 librus_apix-1.0.4/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-28 21:25:37.000000 librus_apix-1.0.4/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:25:40.104798 librus_apix-1.0.4/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 21:25:40.000000 librus_apix-1.0.4/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 21:25:37.000000 librus_apix-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-28 21:25:40.104798 librus_apix-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:25:37.000000 librus_apix-1.0.4/setup.py
```

### Comparing `librus_apix-1.0.3/LICENSE` & `librus_apix-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/README.md` & `librus_apix-1.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -140,15 +140,14 @@
 recipients = get_recipients(client, groups[0])
 my_recipient = recipients["John Brown"]
 my_second_recipient = recipients["Barbara Brown"]
 
 sent = send_message(client,
                    "Message Title",
                    "Message\n content",
-                   "teachers",
                    [my_recipient, my_second_recipient]
 )
 if sent == True:
   print("Sent!")
 else:
   print("Error sending a message!")
 ```
@@ -192,14 +191,23 @@
 timetable = get_timetable(client, monday_datetime)
 for weekday in timetable:
   for period in timetable[weekday]:
     print(period.subject, period.teacher_and_classroom)
 
 ```
 
+### Notifications (a.k.a. spamming endpoints)
+```
+# initial should be always called with a new token
+initial_notifications, new_ids = get_initial_notification_data(client)
+sleep(150)
+# after that you retrieve the new Notifications with new_ids filtered out 
+new_notifications, new_ids = get_new_notification_data(client, new_ids)
+# see more in docs
+```
 
 ### Getting the lucky number
 ```py
 from librus_apix.student_information import student_information
 
 info = student_information(client)
 print(info.lucky_number)
```

### Comparing `librus_apix-1.0.3/librus_apix/__init__.py` & `librus_apix-1.0.4/librus_apix/__init__.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/announcements.py` & `librus_apix-1.0.4/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/attendance.py` & `librus_apix-1.0.4/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/client.py` & `librus_apix-1.0.4/librus_apix/client.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/completed_lessons.py` & `librus_apix-1.0.4/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/exceptions.py` & `librus_apix-1.0.4/librus_apix/exceptions.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/grades.py` & `librus_apix-1.0.4/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/helpers.py` & `librus_apix-1.0.4/librus_apix/helpers.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/homework.py` & `librus_apix-1.0.4/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/messages.py` & `librus_apix-1.0.4/librus_apix/messages.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/schedule.py` & `librus_apix-1.0.4/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/student_information.py` & `librus_apix-1.0.4/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/timetable.py` & `librus_apix-1.0.4/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix/urls.py` & `librus_apix-1.0.4/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/librus_apix.egg-info/SOURCES.txt` & `librus_apix-1.0.4/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.3/setup.cfg` & `librus_apix-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v1.0.3
+version = v1.0.4
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

