# Comparing `tmp/kalente-0.1.3.tar.gz` & `tmp/kalente-0.2.0.tar.gz`

## Comparing `kalente-0.1.3.tar` & `kalente-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 kalente-0.1.3/.gitlab-ci.yml
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kalente-0.1.3/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kalente-0.1.3/src/kalente/__init__.py
--rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 kalente-0.1.3/src/kalente/__main__.py
--rw-r--r--   0        0        0  3147977 2020-02-02 00:00:00.000000 kalente-0.1.3/src/kalente/static/logo.png
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 kalente-0.1.3/src/kalente/templates/daily.html
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 kalente-0.1.3/src/kalente/templates/monthly.html
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kalente-0.1.3/src/kalente/templates/weekly.html
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 kalente-0.1.3/src/kalente/templates/yearly.html
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 kalente-0.1.3/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 kalente-0.1.3/LICENSE
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 kalente-0.1.3/README.md
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 kalente-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 kalente-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 kalente-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 kalente-0.2.0/.forgejo/workflows/release.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/__init__.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/__main__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/classes/__init__.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/classes/calendar.py
+-rw-r--r--   0        0        0  3147977 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/static/logo.png
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/templates/daily.html
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/templates/monthly.html
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/templates/weekly.html
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 kalente-0.2.0/src/kalente/templates/yearly.html
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 kalente-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 kalente-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 kalente-0.2.0/README.md
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 kalente-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 kalente-0.2.0/PKG-INFO
```

### Comparing `kalente-0.1.3/src/kalente/static/logo.png` & `kalente-0.2.0/src/kalente/static/logo.png`

 * *Files identical despite different names*

### Comparing `kalente-0.1.3/src/kalente/templates/daily.html` & `kalente-0.2.0/src/kalente/templates/daily.html`

 * *Files 10% similar despite different names*

```diff
@@ -40,25 +40,25 @@
                 top: 0px;
                 right: 10px;
                 height: 65px;
       }
     </style>
   </head>
   <body>
-    {% if logo %}
-      <img class="logo" src="{{ logo }}" alt="Logo"> 
-    {% endif %}
+    {% if logo %}<img class="logo" src="{{ logo }}" alt="Logo">{% endif %}
     <h2>Day Planner</h2>
     <table>
       <tr>
-        <th class="{% if day.holiday %}holiday{% elif day.is_weekend and day.day == 'Saturday' %}saturday{% elif day.is_weekend and day.day == 'Sunday' %}sunday{% endif %}">{{ day.day }}<br />{{ day.date }}</th>
+        <th class="{% if day.holiday %}holiday{% elif day.is_weekend and day.day == 'Saturday' %}saturday{% elif day.is_weekend and day.day == 'Sunday' %}sunday{% endif %}">
+          {{ day.day }}
+          <br />
+          {{ day.date }}
+        </th>
       </tr>
       <tr>
         <td>
-          {% if day.holiday %}
-          <b>{{ day.holiday }}</b>
-          {% endif %}
+          {% if day.holiday %}<b>{{ day.holiday }}</b>{% endif %}
         </td>
       </tr>
     </table>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
-{% if logo %} [Logo]{% endif %}
+{% if logo %}[Logo]{% endif %}
 ********** DDaayy PPllaannnneerr **********
 {{{{ ddaayy..ddaayy }}}}
 {{{{ ddaayy..ddaattee }}}}
-{% if day.holiday %} {{{{ ddaayy..hhoolliiddaayy }}}} {% endif %}
+{% if day.holiday %}{{{{ ddaayy..hhoolliiddaayy }}}}{% endif %}
```

### Comparing `kalente-0.1.3/src/kalente/templates/monthly.html` & `kalente-0.2.0/src/kalente/templates/monthly.html`

 * *Files identical despite different names*

### Comparing `kalente-0.1.3/src/kalente/templates/weekly.html` & `kalente-0.2.0/src/kalente/templates/weekly.html`

 * *Files identical despite different names*

### Comparing `kalente-0.1.3/src/kalente/templates/yearly.html` & `kalente-0.2.0/src/kalente/templates/yearly.html`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,15 @@
       }
     </style>
   </head>
   <body>
     {% set splits = (0, 6), (6, 12) %}
     {% for start, end in splits %}
       <h2>Yearly Calendar for {{ year.1.1.1.date_obj.year }}</h2>
-      {% if logo %}
-        <img class="logo" src="{{ logo }}" alt="Logo">
-      {% endif %}
+      {% if logo %}<img class="logo" src="{{ logo }}" alt="Logo">{% endif %}
       <table class="yearly-calendar">
         <tr>
           {% for month in year %}
             {% if start <= (month[1][1].date_obj.month - 1) and
               (month[1][1].date_obj.month - 1 < end) %}
               <th>
                 <div class="month-name">{{ month[1][1].date_obj.strftime("%B") }}</div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% set splits = (0, 6), (6, 12) %} {% for start, end in splits %}
 ********** YYeeaarrllyy CCaalleennddaarr ffoorr {{{{ yyeeaarr..11..11..11..ddaattee__oobbjj..yyeeaarr }}}} **********
-{% if logo %} [Logo]{% endif %}
+{% if logo %}[Logo]{% endif %}
 {{{{ mmoonntthh[[11]][[11]]..ddaattee__oobbjj..ssttrrffttiimmee((""%%BB""))
 }}}}
                                        {{ day.date_obj.strftime("%d") }} {% if
                                        day.holiday %}{{ day.holiday }}{% endif
                                        %}
 {% endfor %}
```

### Comparing `kalente-0.1.3/LICENSE` & `kalente-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kalente-0.1.3/README.md` & `kalente-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kalente-0.1.3/pyproject.toml` & `kalente-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kalente"
-version = "0.1.3"
+version = "0.2.0"
 authors = [
   { name="Kumi Mitterer", email="kalente@kumi.email" },
 ]
 description = "Simple Python script to generate a printable calendar"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `kalente-0.1.3/PKG-INFO` & `kalente-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: kalente
-Version: 0.1.3
+Version: 0.2.0
 Summary: Simple Python script to generate a printable calendar
 Project-URL: Homepage, https://kumig.it/kumitterer/kalente
 Project-URL: Bug Tracker, https://kumig.it/kumitterer/kalente/issues
 Author-email: Kumi Mitterer <kalente@kumi.email>
 License: Copyright (c) 2023 Kumi Mitterer <kalente@kumi.email>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

