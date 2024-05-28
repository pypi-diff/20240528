# Comparing `tmp/vo-wot-0.18.3.tar.gz` & `tmp/vo_wot-0.18.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vo-wot-0.18.3.tar", last modified: Thu Jan 11 15:45:06 2024, max compression
+gzip compressed data, was "vo_wot-0.18.4.tar", last modified: Tue May 28 10:10:00 2024, max compression
```

## Comparing `vo-wot-0.18.3.tar` & `vo_wot-0.18.4.tar`

### file list

```diff
@@ -1,128 +1,132 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.768400 vo-wot-0.18.3/
--rw-r--r--   0 nick      (1000) nick      (1000)     1095 2023-10-16 19:40:05.000000 vo-wot-0.18.3/LICENSE
--rw-r--r--   0 nick      (1000) nick      (1000)     6978 2024-01-11 15:45:06.768400 vo-wot-0.18.3/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     3575 2023-10-30 11:42:09.000000 vo-wot-0.18.3/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)     2100 2024-01-11 13:29:14.000000 vo-wot-0.18.3/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)       38 2024-01-11 15:45:06.768400 vo-wot-0.18.3/setup.cfg
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.765066 vo-wot-0.18.3/vo_wot.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     6978 2024-01-11 15:45:06.000000 vo-wot-0.18.3/vo_wot.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     3144 2024-01-11 15:45:06.000000 vo-wot-0.18.3/vo_wot.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2024-01-11 15:45:06.000000 vo-wot-0.18.3/vo_wot.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       46 2024-01-11 15:45:06.000000 vo-wot-0.18.3/vo_wot.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)      551 2024-01-11 15:45:06.000000 vo-wot-0.18.3/vo_wot.egg-info/requires.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        6 2024-01-11 15:45:06.000000 vo-wot-0.18.3/vo_wot.egg-info/top_level.txt
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.738400 vo-wot-0.18.3/wotpy/
--rw-r--r--   0 nick      (1000) nick      (1000)      430 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)       23 2024-01-11 15:42:58.000000 vo-wot-0.18.3/wotpy/__version__.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.738400 vo-wot-0.18.3/wotpy/cli/
--rw-r--r--   0 nick      (1000) nick      (1000)      201 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/cli/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)    10988 2024-01-11 15:41:40.000000 vo-wot-0.18.3/wotpy/cli/cli.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9206 2023-11-02 14:23:54.000000 vo-wot-0.18.3/wotpy/cli/default_servient.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.738400 vo-wot-0.18.3/wotpy/codecs/
--rw-r--r--   0 nick      (1000) nick      (1000)      238 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/codecs/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)      744 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/codecs/base.py
--rw-r--r--   0 nick      (1000) nick      (1000)      267 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/codecs/enums.py
--rw-r--r--   0 nick      (1000) nick      (1000)      815 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/codecs/json_codec.py
--rw-r--r--   0 nick      (1000) nick      (1000)      749 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/codecs/text.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.741733 vo-wot-0.18.3/wotpy/database/
--rw-r--r--   0 nick      (1000) nick      (1000)      249 2023-10-16 19:29:51.000000 vo-wot-0.18.3/wotpy/database/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)      739 2023-10-16 18:43:23.000000 vo-wot-0.18.3/wotpy/database/database_schema.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1874 2023-10-16 19:40:05.000000 vo-wot-0.18.3/wotpy/database/influxdb_database.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1172 2023-10-16 18:43:23.000000 vo-wot-0.18.3/wotpy/database/sqlite_database.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.741733 vo-wot-0.18.3/wotpy/functions/
--rw-r--r--   0 nick      (1000) nick      (1000)      168 2023-10-16 19:29:51.000000 vo-wot-0.18.3/wotpy/functions/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4114 2023-10-16 19:40:05.000000 vo-wot-0.18.3/wotpy/functions/functions.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.745066 vo-wot-0.18.3/wotpy/protocols/
--rw-r--r--   0 nick      (1000) nick      (1000)      395 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2102 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/client.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.745066 vo-wot-0.18.3/wotpy/protocols/coap/
--rw-r--r--   0 nick      (1000) nick      (1000)      496 2023-10-16 19:40:05.000000 vo-wot-0.18.3/wotpy/protocols/coap/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4469 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/coap/authenticator.py
--rw-r--r--   0 nick      (1000) nick      (1000)    13529 2023-11-14 16:03:09.000000 vo-wot-0.18.3/wotpy/protocols/coap/client.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4400 2023-11-14 16:05:19.000000 vo-wot-0.18.3/wotpy/protocols/coap/credential.py
--rw-r--r--   0 nick      (1000) nick      (1000)      262 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/coap/enums.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.745066 vo-wot-0.18.3/wotpy/protocols/coap/resources/
--rw-r--r--   0 nick      (1000) nick      (1000)      328 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/coap/resources/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5970 2023-11-03 11:45:56.000000 vo-wot-0.18.3/wotpy/protocols/coap/resources/action.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3402 2023-11-03 11:46:01.000000 vo-wot-0.18.3/wotpy/protocols/coap/resources/event.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4016 2023-11-03 11:46:04.000000 vo-wot-0.18.3/wotpy/protocols/coap/resources/property.py
--rw-r--r--   0 nick      (1000) nick      (1000)      397 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/coap/resources/utils.py
--rw-r--r--   0 nick      (1000) nick      (1000)     8867 2023-11-03 11:45:53.000000 vo-wot-0.18.3/wotpy/protocols/coap/server.py
--rw-r--r--   0 nick      (1000) nick      (1000)      811 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/enums.py
--rw-r--r--   0 nick      (1000) nick      (1000)      855 2023-11-03 11:45:45.000000 vo-wot-0.18.3/wotpy/protocols/exceptions.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.748400 vo-wot-0.18.3/wotpy/protocols/http/
--rw-r--r--   0 nick      (1000) nick      (1000)      336 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/http/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6212 2023-10-23 13:24:47.000000 vo-wot-0.18.3/wotpy/protocols/http/authenticator.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9711 2023-11-14 16:03:47.000000 vo-wot-0.18.3/wotpy/protocols/http/client.py
--rw-r--r--   0 nick      (1000) nick      (1000)     8387 2023-11-14 16:04:35.000000 vo-wot-0.18.3/wotpy/protocols/http/credential.py
--rw-r--r--   0 nick      (1000) nick      (1000)      262 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/http/enums.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.751733 vo-wot-0.18.3/wotpy/protocols/http/handlers/
--rw-r--r--   0 nick      (1000) nick      (1000)      330 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/http/handlers/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1173 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/http/handlers/action.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1939 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/http/handlers/event.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3367 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/http/handlers/property.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1493 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/http/handlers/utils.py
--rw-r--r--   0 nick      (1000) nick      (1000)     7522 2023-11-03 12:00:15.000000 vo-wot-0.18.3/wotpy/protocols/http/server.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.751733 vo-wot-0.18.3/wotpy/protocols/mqtt/
--rw-r--r--   0 nick      (1000) nick      (1000)      452 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)    25350 2023-09-15 10:35:47.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/client.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1054 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/enums.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.755066 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/
--rw-r--r--   0 nick      (1000) nick      (1000)      429 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3215 2023-11-03 11:49:32.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/action.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1365 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/base.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2810 2023-11-03 11:49:34.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/event.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1149 2023-11-03 11:49:37.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/ping.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6381 2023-11-03 11:49:40.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/property.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3675 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/subs.py
--rw-r--r--   0 nick      (1000) nick      (1000)     9024 2023-09-15 10:33:44.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/runner.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5728 2023-11-03 11:49:29.000000 vo-wot-0.18.3/wotpy/protocols/mqtt/server.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1396 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/refs.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3353 2023-11-02 11:06:09.000000 vo-wot-0.18.3/wotpy/protocols/server.py
--rw-r--r--   0 nick      (1000) nick      (1000)      984 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/utils.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.755066 vo-wot-0.18.3/wotpy/protocols/ws/
--rw-r--r--   0 nick      (1000) nick      (1000)      319 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/ws/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)    16315 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/ws/client.py
--rw-r--r--   0 nick      (1000) nick      (1000)      881 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/ws/enums.py
--rw-r--r--   0 nick      (1000) nick      (1000)    11124 2023-11-03 11:49:43.000000 vo-wot-0.18.3/wotpy/protocols/ws/handler.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6820 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/ws/messages.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4592 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/protocols/ws/schemas.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3195 2023-11-03 11:49:47.000000 vo-wot-0.18.3/wotpy/protocols/ws/server.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1386 2023-10-30 11:42:20.000000 vo-wot-0.18.3/wotpy/support.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.758400 vo-wot-0.18.3/wotpy/utils/
--rw-r--r--   0 nick      (1000) nick      (1000)      192 2023-10-16 19:29:51.000000 vo-wot-0.18.3/wotpy/utils/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)      586 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/utils/enums.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2690 2023-10-16 19:29:51.000000 vo-wot-0.18.3/wotpy/utils/proxy.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3944 2023-10-16 19:29:51.000000 vo-wot-0.18.3/wotpy/utils/utils.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.761733 vo-wot-0.18.3/wotpy/wot/
--rw-r--r--   0 nick      (1000) nick      (1000)      458 2023-10-30 11:42:25.000000 vo-wot-0.18.3/wotpy/wot/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)      233 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/constants.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.761733 vo-wot-0.18.3/wotpy/wot/consumed/
--rw-r--r--   0 nick      (1000) nick      (1000)      202 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/consumed/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     7255 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/consumed/interaction_map.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5363 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/consumed/thing.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.765066 vo-wot-0.18.3/wotpy/wot/dictionaries/
--rw-r--r--   0 nick      (1000) nick      (1000)      485 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2587 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/base.py
--rw-r--r--   0 nick      (1000) nick      (1000)      570 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/filter.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6280 2023-11-03 11:50:08.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/interaction.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2424 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/link.py
--rw-r--r--   0 nick      (1000) nick      (1000)      818 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/response.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4563 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/schema.py
--rw-r--r--   0 nick      (1000) nick      (1000)     7279 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/security.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6140 2023-11-03 11:50:12.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/thing.py
--rw-r--r--   0 nick      (1000) nick      (1000)      584 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/dictionaries/version.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1657 2023-10-30 11:42:11.000000 vo-wot-0.18.3/wotpy/wot/enums.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3247 2023-11-03 11:49:55.000000 vo-wot-0.18.3/wotpy/wot/events.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-01-11 15:45:06.765066 vo-wot-0.18.3/wotpy/wot/exposed/
--rw-r--r--   0 nick      (1000) nick      (1000)      230 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/exposed/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6668 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/exposed/interaction_map.py
--rw-r--r--   0 nick      (1000) nick      (1000)    19845 2023-11-03 11:50:15.000000 vo-wot-0.18.3/wotpy/wot/exposed/thing.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2102 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/exposed/thing_set.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1548 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/form.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4591 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/interaction.py
--rw-r--r--   0 nick      (1000) nick      (1000)    18759 2023-10-30 11:42:15.000000 vo-wot-0.18.3/wotpy/wot/servient.py
--rw-r--r--   0 nick      (1000) nick      (1000)     3084 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/td.py
--rw-r--r--   0 nick      (1000) nick      (1000)     6668 2023-11-03 11:50:01.000000 vo-wot-0.18.3/wotpy/wot/thing.py
--rw-r--r--   0 nick      (1000) nick      (1000)    47598 2023-09-12 15:07:16.000000 vo-wot-0.18.3/wotpy/wot/validation.py
--rw-r--r--   0 nick      (1000) nick      (1000)     7169 2023-11-03 13:08:04.000000 vo-wot-0.18.3/wotpy/wot/wot.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.912056 vo_wot-0.18.4/
+-rw-r--r--   0 nick      (1000) nick      (1000)     1095 2023-10-16 19:40:05.000000 vo_wot-0.18.4/LICENSE
+-rw-r--r--   0 nick      (1000) nick      (1000)     6978 2024-05-28 10:10:00.912056 vo_wot-0.18.4/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)     3575 2023-10-30 11:42:09.000000 vo_wot-0.18.4/README.md
+-rw-r--r--   0 nick      (1000) nick      (1000)     2100 2024-05-13 13:23:43.000000 vo_wot-0.18.4/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)       38 2024-05-28 10:10:00.912056 vo_wot-0.18.4/setup.cfg
+-rw-r--r--   0 nick      (1000) nick      (1000)       92 2024-05-13 12:55:19.000000 vo_wot-0.18.4/setup.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.908722 vo_wot-0.18.4/vo_wot.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     6978 2024-05-28 10:10:00.000000 vo_wot-0.18.4/vo_wot.egg-info/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)     3222 2024-05-28 10:10:00.000000 vo_wot-0.18.4/vo_wot.egg-info/SOURCES.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2024-05-28 10:10:00.000000 vo_wot-0.18.4/vo_wot.egg-info/dependency_links.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)       46 2024-05-28 10:10:00.000000 vo_wot-0.18.4/vo_wot.egg-info/entry_points.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)      551 2024-05-28 10:10:00.000000 vo_wot-0.18.4/vo_wot.egg-info/requires.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        6 2024-05-28 10:10:00.000000 vo_wot-0.18.4/vo_wot.egg-info/top_level.txt
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.878722 vo_wot-0.18.4/wotpy/
+-rw-r--r--   0 nick      (1000) nick      (1000)      430 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)       23 2024-05-28 10:07:28.000000 vo_wot-0.18.4/wotpy/__version__.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.878722 vo_wot-0.18.4/wotpy/cli/
+-rw-r--r--   0 nick      (1000) nick      (1000)      201 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/cli/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    11514 2024-04-25 11:28:32.000000 vo_wot-0.18.4/wotpy/cli/cli.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    10467 2024-04-25 11:07:58.000000 vo_wot-0.18.4/wotpy/cli/default_servient.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.878722 vo_wot-0.18.4/wotpy/codecs/
+-rw-r--r--   0 nick      (1000) nick      (1000)      238 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/codecs/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      744 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/codecs/base.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      267 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/codecs/enums.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      815 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/codecs/json_codec.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      749 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/codecs/text.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.882055 vo_wot-0.18.4/wotpy/database/
+-rw-r--r--   0 nick      (1000) nick      (1000)      249 2024-04-25 10:25:42.000000 vo_wot-0.18.4/wotpy/database/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      739 2023-10-16 18:43:23.000000 vo_wot-0.18.4/wotpy/database/database_schema.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1874 2023-10-16 19:40:05.000000 vo_wot-0.18.4/wotpy/database/influxdb_database.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2484 2024-05-23 15:25:53.000000 vo_wot-0.18.4/wotpy/database/sqlite_database.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.882055 vo_wot-0.18.4/wotpy/functions/
+-rw-r--r--   0 nick      (1000) nick      (1000)      168 2023-10-16 19:29:51.000000 vo_wot-0.18.4/wotpy/functions/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4106 2024-05-13 14:31:24.000000 vo_wot-0.18.4/wotpy/functions/functions.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.885389 vo_wot-0.18.4/wotpy/protocols/
+-rw-r--r--   0 nick      (1000) nick      (1000)      423 2024-03-19 18:30:11.000000 vo_wot-0.18.4/wotpy/protocols/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2102 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/client.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.885389 vo_wot-0.18.4/wotpy/protocols/coap/
+-rw-r--r--   0 nick      (1000) nick      (1000)      496 2023-10-16 19:40:05.000000 vo_wot-0.18.4/wotpy/protocols/coap/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4469 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/coap/authenticator.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    13529 2023-11-14 16:03:09.000000 vo_wot-0.18.4/wotpy/protocols/coap/client.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4400 2023-11-14 16:05:19.000000 vo_wot-0.18.4/wotpy/protocols/coap/credential.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      262 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/coap/enums.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.888722 vo_wot-0.18.4/wotpy/protocols/coap/resources/
+-rw-r--r--   0 nick      (1000) nick      (1000)      328 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/coap/resources/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5970 2023-11-03 11:45:56.000000 vo_wot-0.18.4/wotpy/protocols/coap/resources/action.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3402 2023-11-03 11:46:01.000000 vo_wot-0.18.4/wotpy/protocols/coap/resources/event.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4016 2023-11-03 11:46:04.000000 vo_wot-0.18.4/wotpy/protocols/coap/resources/property.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      397 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/coap/resources/utils.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     8867 2023-11-03 11:45:53.000000 vo_wot-0.18.4/wotpy/protocols/coap/server.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      811 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/enums.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      855 2023-11-03 11:45:45.000000 vo_wot-0.18.4/wotpy/protocols/exceptions.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.888722 vo_wot-0.18.4/wotpy/protocols/http/
+-rw-r--r--   0 nick      (1000) nick      (1000)      336 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/http/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6212 2023-10-23 13:24:47.000000 vo_wot-0.18.4/wotpy/protocols/http/authenticator.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9711 2023-11-14 16:03:47.000000 vo_wot-0.18.4/wotpy/protocols/http/client.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     8387 2023-11-14 16:04:35.000000 vo_wot-0.18.4/wotpy/protocols/http/credential.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      262 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/http/enums.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.892056 vo_wot-0.18.4/wotpy/protocols/http/handlers/
+-rw-r--r--   0 nick      (1000) nick      (1000)      330 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/http/handlers/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1173 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/http/handlers/action.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1939 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/http/handlers/event.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3367 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/http/handlers/property.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1493 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/http/handlers/utils.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     7661 2024-04-25 10:52:42.000000 vo_wot-0.18.4/wotpy/protocols/http/server.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.895389 vo_wot-0.18.4/wotpy/protocols/mqtt/
+-rw-r--r--   0 nick      (1000) nick      (1000)      452 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    25350 2023-09-15 10:35:47.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/client.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1054 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/enums.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.898722 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/
+-rw-r--r--   0 nick      (1000) nick      (1000)      429 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3215 2023-11-03 11:49:32.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/action.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1365 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/base.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2810 2023-11-03 11:49:34.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/event.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1149 2023-11-03 11:49:37.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/ping.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6381 2023-11-03 11:49:40.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/property.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3675 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/subs.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     9024 2023-09-15 10:33:44.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/runner.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5728 2023-11-03 11:49:29.000000 vo_wot-0.18.4/wotpy/protocols/mqtt/server.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.898722 vo_wot-0.18.4/wotpy/protocols/netconf/
+-rw-r--r--   0 nick      (1000) nick      (1000)      158 2024-03-19 18:34:03.000000 vo_wot-0.18.4/wotpy/protocols/netconf/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5039 2024-03-27 13:58:36.000000 vo_wot-0.18.4/wotpy/protocols/netconf/utils.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1396 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/refs.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3355 2024-01-22 17:08:16.000000 vo_wot-0.18.4/wotpy/protocols/server.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      984 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/utils.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.902056 vo_wot-0.18.4/wotpy/protocols/ws/
+-rw-r--r--   0 nick      (1000) nick      (1000)      319 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/ws/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    16315 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/ws/client.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      881 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/ws/enums.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    11124 2023-11-03 11:49:43.000000 vo_wot-0.18.4/wotpy/protocols/ws/handler.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6820 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/ws/messages.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4592 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/protocols/ws/schemas.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3195 2023-11-03 11:49:47.000000 vo_wot-0.18.4/wotpy/protocols/ws/server.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1386 2023-10-30 11:42:20.000000 vo_wot-0.18.4/wotpy/support.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.902056 vo_wot-0.18.4/wotpy/utils/
+-rw-r--r--   0 nick      (1000) nick      (1000)      192 2023-10-16 19:29:51.000000 vo_wot-0.18.4/wotpy/utils/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      586 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/utils/enums.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2690 2023-10-16 19:29:51.000000 vo_wot-0.18.4/wotpy/utils/proxy.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3944 2023-10-16 19:29:51.000000 vo_wot-0.18.4/wotpy/utils/utils.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.905389 vo_wot-0.18.4/wotpy/wot/
+-rw-r--r--   0 nick      (1000) nick      (1000)      458 2023-10-30 11:42:25.000000 vo_wot-0.18.4/wotpy/wot/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      233 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/constants.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.905389 vo_wot-0.18.4/wotpy/wot/consumed/
+-rw-r--r--   0 nick      (1000) nick      (1000)      202 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/consumed/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     7255 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/consumed/interaction_map.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5363 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/consumed/thing.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.908722 vo_wot-0.18.4/wotpy/wot/dictionaries/
+-rw-r--r--   0 nick      (1000) nick      (1000)      485 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2587 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/base.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      570 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/filter.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6280 2023-11-03 11:50:08.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/interaction.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2424 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/link.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      818 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/response.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4563 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/schema.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     7279 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/security.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6140 2023-11-03 11:50:12.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/thing.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      584 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/dictionaries/version.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1657 2023-10-30 11:42:11.000000 vo_wot-0.18.4/wotpy/wot/enums.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3247 2023-11-03 11:49:55.000000 vo_wot-0.18.4/wotpy/wot/events.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-28 10:10:00.908722 vo_wot-0.18.4/wotpy/wot/exposed/
+-rw-r--r--   0 nick      (1000) nick      (1000)      230 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/exposed/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6668 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/exposed/interaction_map.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    19845 2023-11-03 11:50:15.000000 vo_wot-0.18.4/wotpy/wot/exposed/thing.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2102 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/exposed/thing_set.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     1548 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/form.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     4591 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/interaction.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    18598 2024-04-25 11:21:43.000000 vo_wot-0.18.4/wotpy/wot/servient.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     3084 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/td.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     6668 2023-11-03 11:50:01.000000 vo_wot-0.18.4/wotpy/wot/thing.py
+-rw-r--r--   0 nick      (1000) nick      (1000)    47598 2023-09-12 15:07:16.000000 vo_wot-0.18.4/wotpy/wot/validation.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     7169 2023-11-03 13:08:04.000000 vo_wot-0.18.4/wotpy/wot/wot.py
```

### Comparing `vo-wot-0.18.3/LICENSE` & `vo_wot-0.18.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/PKG-INFO` & `vo_wot-0.18.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vo-wot
-Version: 0.18.3
+Version: 0.18.4
 Summary: Virtual Object python implementation using a W3C WoT Runtime and the WoT Scripting API
 Author-email: Andres Garcia Mangas <andres.garcia@fundacionctic.org>
 Maintainer-email: Nikos Filinis <nfilinis@netmode.ntua.gr>, Dimitris Spatharakis <dspatharakis@netmode.ntua.gr>
 License: MIT License
         
         Copyright (c) 2023 National Technical University of Athens
         
@@ -42,16 +42,16 @@
 License-File: LICENSE
 Requires-Dist: tornado<7.0,>=6.2
 Requires-Dist: jsonschema<5.0,>=4.17.3
 Requires-Dist: reactivex<5.0,>=4.0.4
 Requires-Dist: python-slugify<9.0,>=8.0.0
 Requires-Dist: requests-oauthlib<1.4,>=1.3.1
 Requires-Dist: influxdb-client<1.37,>=1.36.1
-Requires-Dist: pmdarima==2.0.3
-Requires-Dist: pandas==2.0.1
+Requires-Dist: pmdarima==2.0.4
+Requires-Dist: numpy==1.26.4
 Requires-Dist: pyOpenSSL<24.0.0,>=23.0.0
 Requires-Dist: aiocoap[linkheader,oscore]==0.4.7; platform_system != "Darwin"
 Requires-Dist: amqtt==0.11.0b1
 Requires-Dist: websockets>=8.0
 Provides-Extra: tests
 Requires-Dist: pytest>=7.2.1; extra == "tests"
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "tests"
```

### Comparing `vo-wot-0.18.3/README.md` & `vo_wot-0.18.4/README.md`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/pyproject.toml` & `vo_wot-0.18.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 dependencies = [
   'tornado>=6.2,<7.0',
   'jsonschema>=4.17.3,<5.0',
   'reactivex>=4.0.4,<5.0',
   'python-slugify>=8.0.0,<9.0',
   'requests-oauthlib>=1.3.1,<1.4',
   'influxdb-client>=1.36.1,<1.37',
-  'pmdarima==2.0.3',
-  'pandas==2.0.1',
+  'pmdarima==2.0.4',
+  'numpy==1.26.4',
   'pyOpenSSL>=23.0.0,<24.0.0',
   'aiocoap[linkheader,oscore]==0.4.7 ; platform_system != "Darwin"',
   'amqtt==0.11.0b1',
   'websockets>=8.0'
 ]
 
 [project.optional-dependencies]
```

### Comparing `vo-wot-0.18.3/vo_wot.egg-info/PKG-INFO` & `vo_wot-0.18.4/vo_wot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vo-wot
-Version: 0.18.3
+Version: 0.18.4
 Summary: Virtual Object python implementation using a W3C WoT Runtime and the WoT Scripting API
 Author-email: Andres Garcia Mangas <andres.garcia@fundacionctic.org>
 Maintainer-email: Nikos Filinis <nfilinis@netmode.ntua.gr>, Dimitris Spatharakis <dspatharakis@netmode.ntua.gr>
 License: MIT License
         
         Copyright (c) 2023 National Technical University of Athens
         
@@ -42,16 +42,16 @@
 License-File: LICENSE
 Requires-Dist: tornado<7.0,>=6.2
 Requires-Dist: jsonschema<5.0,>=4.17.3
 Requires-Dist: reactivex<5.0,>=4.0.4
 Requires-Dist: python-slugify<9.0,>=8.0.0
 Requires-Dist: requests-oauthlib<1.4,>=1.3.1
 Requires-Dist: influxdb-client<1.37,>=1.36.1
-Requires-Dist: pmdarima==2.0.3
-Requires-Dist: pandas==2.0.1
+Requires-Dist: pmdarima==2.0.4
+Requires-Dist: numpy==1.26.4
 Requires-Dist: pyOpenSSL<24.0.0,>=23.0.0
 Requires-Dist: aiocoap[linkheader,oscore]==0.4.7; platform_system != "Darwin"
 Requires-Dist: amqtt==0.11.0b1
 Requires-Dist: websockets>=8.0
 Provides-Extra: tests
 Requires-Dist: pytest>=7.2.1; extra == "tests"
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == "tests"
```

### Comparing `vo-wot-0.18.3/vo_wot.egg-info/SOURCES.txt` & `vo_wot-0.18.4/vo_wot.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.py
 vo_wot.egg-info/PKG-INFO
 vo_wot.egg-info/SOURCES.txt
 vo_wot.egg-info/dependency_links.txt
 vo_wot.egg-info/entry_points.txt
 vo_wot.egg-info/requires.txt
 vo_wot.egg-info/top_level.txt
 wotpy/__init__.py
@@ -61,14 +62,16 @@
 wotpy/protocols/mqtt/handlers/__init__.py
 wotpy/protocols/mqtt/handlers/action.py
 wotpy/protocols/mqtt/handlers/base.py
 wotpy/protocols/mqtt/handlers/event.py
 wotpy/protocols/mqtt/handlers/ping.py
 wotpy/protocols/mqtt/handlers/property.py
 wotpy/protocols/mqtt/handlers/subs.py
+wotpy/protocols/netconf/__init__.py
+wotpy/protocols/netconf/utils.py
 wotpy/protocols/ws/__init__.py
 wotpy/protocols/ws/client.py
 wotpy/protocols/ws/enums.py
 wotpy/protocols/ws/handler.py
 wotpy/protocols/ws/messages.py
 wotpy/protocols/ws/schemas.py
 wotpy/protocols/ws/server.py
```

### Comparing `vo-wot-0.18.3/vo_wot.egg-info/requires.txt` & `vo_wot-0.18.4/vo_wot.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 tornado<7.0,>=6.2
 jsonschema<5.0,>=4.17.3
 reactivex<5.0,>=4.0.4
 python-slugify<9.0,>=8.0.0
 requests-oauthlib<1.4,>=1.3.1
 influxdb-client<1.37,>=1.36.1
-pmdarima==2.0.3
-pandas==2.0.1
+pmdarima==2.0.4
+numpy==1.26.4
 pyOpenSSL<24.0.0,>=23.0.0
 amqtt==0.11.0b1
 websockets>=8.0
 
 [:platform_system != "Darwin"]
 aiocoap[linkheader,oscore]==0.4.7
```

### Comparing `vo-wot-0.18.3/wotpy/cli/cli.py` & `vo_wot-0.18.4/wotpy/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,29 @@
 """
 CLI for the WoT runtime that handles servient configuration and execution of WoT runtime scripts.
 """
 
 import argparse
 import asyncio
 import json
+import logging
 import time
 import yaml
 import importlib.util
 
 from tornado.httpclient import HTTPClientError
 from tornado.ioloop import PeriodicCallback
 
 from wotpy.functions import functions
 from wotpy.cli.default_servient import DefaultServient
-from wotpy.utils.proxy import build_prop_read_proxy, build_prop_write_proxy,\
+from wotpy.protocols.netconf.utils import inject_netconf_properties
+from wotpy.utils.proxy import build_prop_read_proxy, build_prop_write_proxy, \
     build_action_invoke_proxy, subscribe_event
 
+
 def create_proxy_functions(consumed_vos, proxy_dict, exposed_thing):
     """
     Creates proxy functions that propagate interactions with properties, actions
     and events to another thing. The operations that are proxied are:
 
     - Properties:
         - property read
@@ -54,14 +57,15 @@
                 build_action_invoke_proxy(consumed_vos[target_vo], action)
             )
 
     if "eventsMap" in proxy_dict and proxy_dict["eventsMap"] is not None:
         for event, target_vo in proxy_dict["eventsMap"].items():
             subscribe_event(consumed_vos[target_vo], exposed_thing, event)
 
+
 async def consume_vos(consumed_vos_dict, wot, credentials_dict):
     """Consume VOs from the given URLs."""
 
     consumed_vos = {}
 
     for vo_name, vo_dict in consumed_vos_dict.items():
         url = vo_dict["url"]
@@ -75,14 +79,15 @@
                     raise ConnectionError(
                         f"Connection failed after {max_retries} retries"
                     ) from exception
                 time.sleep(retry_interval)
 
     return consumed_vos
 
+
 async def subscribe_remote_events(consumed_vos, consumed_vos_dict, module):
     """Maps remote events/property changes to the corresponding user-defined functions."""
 
     for vo_name, vo_dict in consumed_vos_dict.items():
         events = vo_dict.get("events", [])
         for event in events:
             on_next_handler_name = event + "_" + vo_name + "_on_next"
@@ -110,14 +115,15 @@
 
             consumed_vos[vo_name].properties[proprty].subscribe(
                 on_next=on_next_handler,
                 on_completed=on_completed_handler,
                 on_error=on_error_handler
             )
 
+
 async def map_user_defined_code(TD, exposed_thing, module):
     """
     Maps the following user-defined code to the corresponding WoT constructs:
 
     - Properties:
         - initial values
         - property read handler
@@ -184,32 +190,35 @@
         if on_next_handler is not None:
             exposed_thing.events[event].subscribe(
                 on_next=on_next_handler,
                 on_completed=on_completed_handler,
                 on_error=on_error_handler
             )
 
+
 def schedule_periodic_functions(periodic_function_data, module):
     """Schedules functions to run periodically."""
 
     for periodic_function, periodicity in periodic_function_data.items():
         function = getattr(module, periodic_function, None)
         if function is not None:
             periodic_callback = PeriodicCallback(function, periodicity)
             periodic_callback.start()
         else:
             raise TypeError(f"Function {function} definition needs to be declared")
 
+
 def inject_generic_function(generic_function_data, module):
     """Inject generic function in the user-defined module's functions"""
 
     for generic_function in generic_function_data:
         function = getattr(functions, generic_function)
         setattr(module, generic_function, function)
 
+
 async def run_script(thing_description_path, script_path, config_path):
     """Creates a Servient based on the config file and initializes the WoT runtime"""
 
     config = {}
     if config_path is not None:
         with open(config_path, "r") as config_file:
             config = yaml.safe_load(config_file)
@@ -246,31 +255,47 @@
 
     proxy_data = default_servient.config.get("proxy", {})
     create_proxy_functions(consumed_vos, proxy_data, exposed_thing)
 
     generic_function_data = default_servient.config.get("genericFunction", [])
     inject_generic_function(generic_function_data, module)
 
+    if default_servient.config["bindingNB"]["netconf"]["enabled"]:
+        inject_netconf_properties(
+            exposed_thing,
+            default_servient.config["bindingNB"]["netconf"]["schedulerURL"],
+            default_servient.config["bindingNB"]["netconf"]["netconfServerURL"]
+        )
+
     # Make instances available to user-defined code
     module.exposed_thing = exposed_thing
     module.consumed_vos = consumed_vos
 
     await map_user_defined_code(TD, exposed_thing, module)
 
     exposed_thing.expose()
 
     periodic_function_data = default_servient.config.get("periodicFunction", {})
     schedule_periodic_functions(periodic_function_data, module)
 
+
+def setup_logging():
+    logging.basicConfig()
+    LOGGER = logging.getLogger()
+    LOGGER.setLevel(logging.INFO)
+
+
 def main():
+    setup_logging()
     parser = argparse.ArgumentParser(description="Run a WoT script optionally preconfigured by a config file.")
     parser.add_argument("script", help="user python script file")
     parser.add_argument("-f", "--config-file", help="path to the configuration file")
     parser.add_argument("-t", "--thing-description", help="path to the thing description")
     args = parser.parse_args()
 
     loop = asyncio.get_event_loop()
     loop.create_task(run_script(args.thing_description, args.script, args.config_file))
     loop.run_forever()
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `vo-wot-0.18.3/wotpy/cli/default_servient.py` & `vo_wot-0.18.4/wotpy/cli/default_servient.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from wotpy.utils.utils import dict_merge
 from wotpy.protocols.http.client import HTTPClient
 from wotpy.protocols.http.server import HTTPServer
 from wotpy.protocols.coap.client import CoAPClient
 from wotpy.protocols.coap.server import CoAPServer
 from wotpy.protocols.mqtt.client import MQTTClient
 from wotpy.protocols.mqtt.server import MQTTServer
+from wotpy.protocols.ws.client import WebsocketClient
+from wotpy.protocols.ws.server import WebsocketServer
 from wotpy.wot.servient import Servient
 
 
 class DefaultServient(Servient):
     """Servient with preconfigured values."""
 
     DEFAULT_CONFIG = {
@@ -29,14 +31,19 @@
         "bindingNB": {
             "bindingModeNB": ["U", "H"],
             "hostname": None,
             "ports": {
                 "coapPort": 5683,
                 "httpPort": 8080
             },
+            "netconf": {
+                "enabled": False,
+                "schedulerURL": None,
+                "netconfServerURL": None
+            },
             "brokerIP": None,
             "serverCert": None,
             "serverKey": None,
             "mqttCAFile": None,
             "OSCORECredentialsMap": None,
             "securityNB": {
                 "securityScheme": "nosec",
@@ -111,27 +118,30 @@
             credentials_dict_north[vo_name]["password"] = password_north
 
         if token_north is not None:
             credentials_dict_north[vo_name]["token"] = token_north
 
         if "H" in binding_modes_north:
             port = int(server_bindings_north["ports"]["httpPort"])
+            proxy_port = None
+            if "httpProxyPort" in server_bindings_north["ports"]:
+                proxy_port = int(server_bindings_north["ports"]["httpProxyPort"])
 
             ssl_context = None
             if server_bindings_north["serverCert"] is not None and\
                 server_bindings_north["serverKey"] is not None:
                 certfile = server_bindings_north["serverCert"]
                 keyfile = server_bindings_north["serverKey"]
 
                 ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
                 ssl_context.load_cert_chain(certfile=certfile, keyfile=keyfile)
 
             servers.append(HTTPServer(
                 port=port, security_scheme=security_scheme,
-                ssl_context=ssl_context
+                ssl_context=ssl_context, form_port=proxy_port
             ))
 
         if "U" in binding_modes_north:
             port = int(server_bindings_north["ports"]["coapPort"])
 
             oscore_credentials_map_north = None
             if server_bindings_north["OSCORECredentialsMap"] is not None:
@@ -151,14 +161,30 @@
 
             if username_north is not None and password_north is not None:
                 url_parts = list(urllib.parse.urlparse(broker_url))
                 url_parts[1] = f"{username_north}:{password_north}@{url_parts[1]}"
                 broker_url = urllib.parse.urlunparse(url_parts)
             servers.append(MQTTServer(broker_url, ca_file=mqtt_ca_file_north))
 
+        if "WS" in binding_modes_north:
+            port = int(server_bindings_north["ports"]["websocketPort"])
+
+            ssl_context = None
+            if server_bindings_north["serverCert"] is not None and\
+                    server_bindings_north["serverKey"] is not None:
+                certfile = server_bindings_north["serverCert"]
+                keyfile = server_bindings_north["serverKey"]
+
+                ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
+                ssl_context.load_cert_chain(certfile=certfile, keyfile=keyfile)
+
+            servers.append(WebsocketServer(
+                port=port, ssl_context=ssl_context
+            ))
+
         catalogue_port = int(self.config["catalogue"])
         server_bindings_south = self.config["bindingSB"]
         binding_modes_south = server_bindings_south["bindingModeSB"]\
             if server_bindings_south["bindingModeSB"] is not None else []
 
         security_south = server_bindings_south["securitySB"]
         security_south_http = security_south["securitySBHTTP"]
@@ -207,14 +233,18 @@
 
         if "M" in binding_modes_south:
             mqtt_ca_file_south = None
             if server_bindings_south["mqttCAFile"] is not None:
                 mqtt_ca_file_north = server_bindings_south["mqttCAFile"]
             clients.append(MQTTClient(ca_file=mqtt_ca_file_south))
 
+        if "WS" in binding_modes_south:
+            ws_client = WebsocketClient()
+            clients.append(ws_client)
+
         database_config = self.config["databaseConfig"]
 
         timeseries_db = database_config["timeseriesDB"]
         influxdb_enabled = (timeseries_db["influxDB"] == "enabled")
         influxdb_url = timeseries_db["address"]
         influxdb_token = timeseries_db["dbToken"]
```

### Comparing `vo-wot-0.18.3/wotpy/codecs/base.py` & `vo_wot-0.18.4/wotpy/codecs/base.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/codecs/json_codec.py` & `vo_wot-0.18.4/wotpy/codecs/json_codec.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/codecs/text.py` & `vo_wot-0.18.4/wotpy/codecs/text.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/database/database_schema.py` & `vo_wot-0.18.4/wotpy/database/database_schema.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/database/influxdb_database.py` & `vo_wot-0.18.4/wotpy/database/influxdb_database.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/functions/functions.py` & `vo_wot-0.18.4/wotpy/functions/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 Generic function definitions.
 """
 
 import time
 import datetime
 
-import pandas as pd
+import numpy as np
 import pmdarima as pm
 import tornado.httpclient
 
 
 async def forecasting(exposed_thing, property_name):
     servient = exposed_thing.servient
 
@@ -20,29 +20,29 @@
     |> range(start: -10m)'.format((property_name)) #TODO change limit of query
     tables = servient.influxdb.execute_query(query)
 
     # Serialize to values
     output = tables.to_values(columns=["_value"])
     flat_list = [item for sublist in output for item in sublist]
 
-    df = pd.DataFrame(flat_list)
-    model = pm.auto_arima(df, start_p=1, start_q=1, test="adf",       # use adftest to find optimal "d"
+    arr = np.array(flat_list)
+    model = pm.auto_arima(arr, start_p=1, start_q=1, test="adf",       # use adftest to find optimal "d"
                           max_p=3, max_q=3, # maximum p and q
                           m=1,              # frequency of series
                           d=None,           # let model determine "d"
                           seasonal=False,   # No Seasonality
                           start_P=0,
                           D=0,
                           trace=False,
                           error_action="ignore",
                           suppress_warnings=True,
                           stepwise=True)
     predicted_value = model.predict(n_periods=1)
 
-    return float(predicted_value.iloc[0])
+    return float(predicted_value[0])
 
 async def mean_value(exposed_thing, property_name, horizon):
     """Queries the influxdb database and averages the data
     for the given property."""
 
     servient = exposed_thing.servient
```

### Comparing `vo-wot-0.18.3/wotpy/protocols/client.py` & `vo_wot-0.18.4/wotpy/protocols/client.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/coap/authenticator.py` & `vo_wot-0.18.4/wotpy/protocols/coap/authenticator.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/coap/client.py` & `vo_wot-0.18.4/wotpy/protocols/coap/client.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/coap/credential.py` & `vo_wot-0.18.4/wotpy/protocols/coap/credential.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/coap/resources/action.py` & `vo_wot-0.18.4/wotpy/protocols/coap/resources/action.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/coap/resources/event.py` & `vo_wot-0.18.4/wotpy/protocols/coap/resources/event.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/coap/resources/property.py` & `vo_wot-0.18.4/wotpy/protocols/coap/resources/property.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/coap/server.py` & `vo_wot-0.18.4/wotpy/protocols/coap/server.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/enums.py` & `vo_wot-0.18.4/wotpy/protocols/enums.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/exceptions.py` & `vo_wot-0.18.4/wotpy/protocols/exceptions.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/authenticator.py` & `vo_wot-0.18.4/wotpy/protocols/http/authenticator.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/client.py` & `vo_wot-0.18.4/wotpy/protocols/http/client.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/credential.py` & `vo_wot-0.18.4/wotpy/protocols/http/credential.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/handlers/action.py` & `vo_wot-0.18.4/wotpy/protocols/http/handlers/action.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/handlers/event.py` & `vo_wot-0.18.4/wotpy/protocols/http/handlers/event.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/handlers/property.py` & `vo_wot-0.18.4/wotpy/protocols/http/handlers/property.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/handlers/utils.py` & `vo_wot-0.18.4/wotpy/protocols/http/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/http/server.py` & `vo_wot-0.18.4/wotpy/protocols/http/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
 Class that implements the HTTP server.
 """
 
+import logging
+
 import tornado.httpserver
 import tornado.web
 
 from wotpy.codecs.enums import MediaTypes
 from wotpy.protocols.enums import Protocols, InteractionVerbs
 from wotpy.protocols.http.authenticator import BaseAuthenticator
 from wotpy.protocols.http.enums import HTTPSchemes
@@ -30,14 +32,15 @@
                  security_scheme=DEFAULT_SECURITY_SCHEME, form_port=None):
         super().__init__(port=port, form_port=form_port)
         self._server = None
         self._servient = None
         self._app = self._build_app()
         self._ssl_context = ssl_context
         self._scheme = HTTPSchemes.HTTPS if ssl_context is not None else HTTPSchemes.HTTP
+        self._logr = logging.getLogger(__name__)
         self._action_ttl_secs = action_ttl_secs
         self._pending_actions = {}
         self._invocation_check_times = {}
         self._security_scheme = security_scheme if security_scheme.get("scheme", None) in\
             SecuritySchemeType.list() else self.DEFAULT_SECURITY_SCHEME
 
     @property
@@ -198,14 +201,16 @@
             self.form_port, thing.url_name)
 
     async def start(self, servient=None):
         """Starts the HTTP server."""
 
         self._servient = servient
 
+        self._logr.info("Starting HTTP server on: {}".format(self.port))
+
         self._server = tornado.httpserver.HTTPServer(self.app, ssl_options=self._ssl_context)
         self._server.listen(self.port)
 
     async def stop(self):
         """Stops the HTTP server."""
 
         if not self._server:
```

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/client.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/client.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/enums.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/enums.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/action.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/action.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/base.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/base.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/event.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/event.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/ping.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/ping.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/property.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/property.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/handlers/subs.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/handlers/subs.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/runner.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/runner.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/mqtt/server.py` & `vo_wot-0.18.4/wotpy/protocols/mqtt/server.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/refs.py` & `vo_wot-0.18.4/wotpy/protocols/refs.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/server.py` & `vo_wot-0.18.4/wotpy/protocols/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 
 class BaseProtocolServer(metaclass=ABCMeta):
     """Base protocol server class.
     This is the interface that must be implemented by all server classes."""
 
     def __init__(self, port, form_port=None):
-        if form_port is None:
-            self._form_port = port
+        self._form_port = port if form_port is None else form_port
         self._port = port
         self._codecs = []
         self._exposed_thing_set = ExposedThingSet()
 
     @property
     @abstractmethod
     def protocol(self):
```

### Comparing `vo-wot-0.18.3/wotpy/protocols/utils.py` & `vo_wot-0.18.4/wotpy/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/ws/client.py` & `vo_wot-0.18.4/wotpy/protocols/ws/client.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/ws/enums.py` & `vo_wot-0.18.4/wotpy/protocols/ws/enums.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/ws/handler.py` & `vo_wot-0.18.4/wotpy/protocols/ws/handler.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/ws/messages.py` & `vo_wot-0.18.4/wotpy/protocols/ws/messages.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/ws/schemas.py` & `vo_wot-0.18.4/wotpy/protocols/ws/schemas.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/protocols/ws/server.py` & `vo_wot-0.18.4/wotpy/protocols/ws/server.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/support.py` & `vo_wot-0.18.4/wotpy/support.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/utils/enums.py` & `vo_wot-0.18.4/wotpy/utils/enums.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/utils/proxy.py` & `vo_wot-0.18.4/wotpy/utils/proxy.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/utils/utils.py` & `vo_wot-0.18.4/wotpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/consumed/interaction_map.py` & `vo_wot-0.18.4/wotpy/wot/consumed/interaction_map.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/consumed/thing.py` & `vo_wot-0.18.4/wotpy/wot/consumed/thing.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/base.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/base.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/filter.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/filter.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/interaction.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/interaction.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/link.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/link.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/response.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/response.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/schema.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/schema.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/security.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/security.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/thing.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/thing.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/dictionaries/version.py` & `vo_wot-0.18.4/wotpy/wot/dictionaries/version.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/enums.py` & `vo_wot-0.18.4/wotpy/wot/enums.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/events.py` & `vo_wot-0.18.4/wotpy/wot/events.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/exposed/interaction_map.py` & `vo_wot-0.18.4/wotpy/wot/exposed/interaction_map.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/exposed/thing.py` & `vo_wot-0.18.4/wotpy/wot/exposed/thing.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/exposed/thing_set.py` & `vo_wot-0.18.4/wotpy/wot/exposed/thing_set.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/form.py` & `vo_wot-0.18.4/wotpy/wot/form.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/interaction.py` & `vo_wot-0.18.4/wotpy/wot/interaction.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/servient.py` & `vo_wot-0.18.4/wotpy/wot/servient.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 """
 Class that represents a WoT servient.
 """
 
 import asyncio
 import functools
-import logging
 import re
 import socket
 
 import tornado.web
 from influxdb_client import InfluxDBClient
 from wotpy.protocols.enums import Protocols
 from wotpy.protocols.http.client import HTTPClient
@@ -115,15 +114,15 @@
     WoT clients are entities that are able to understand the WoT Interface to
     send requests and interact with IoT devices exposed by other WoT servients
     or servers using the capabilities of a Web client such as Web browser."""
 
     def __init__(self, hostname=None, catalogue_port=9090,
                  clients=None, clients_config=None, create_default_forms=True,
                  influxdb_enabled=False, influxdb_token=None, influxdb_url=None,
-                 sqlite_db_path=None, init_logging=True):
+                 sqlite_db_path=None):
         self._hostname = hostname if hostname is not None else _get_hostname_fallback()
 
         if not isinstance(self._hostname, str):
             raise ValueError("Invalid hostname: {}".format(self._hostname))
 
         if isinstance(clients, list):
             clients = {item.protocol: item for item in clients}
@@ -142,18 +141,14 @@
         self._influxdb_enabled = influxdb_enabled
         self._sqlite_db = SQLiteDatabase(sqlite_db_path)
         self._influxdb = None
         if influxdb_enabled:
             self._influxdb = InfluxDB(url=influxdb_url, org="wot", token=influxdb_token)
             if not self._influxdb.is_reachable:
                 raise ConnectionError(f"Connection to the InfluxDB database failed")
-        if init_logging:
-            logging.basicConfig()
-            LOGGER = logging.getLogger()
-            LOGGER.setLevel(logging.INFO)
 
         if not len(self._clients):
             self._build_default_clients()
 
     @staticmethod
     def _default_select_client(clients, td, name):
         """Default implementation of the function to select
@@ -189,15 +184,15 @@
             InteractionTypes.PROPERTY: td.properties.keys(),
             InteractionTypes.ACTION: td.actions.keys(),
             InteractionTypes.EVENT: td.events.keys()
         }
 
         try:
             intrct_type = next(key for key, names in
-                intrct_names.items() if name in names)
+                               intrct_names.items() if name in names)
         except StopIteration:
             raise ValueError("Unknown interaction: {}".format(name))
 
         protocol_prefs = protocol_preference_map[intrct_type]
         protocol_choices = set(protocol_prefs).intersection(
             set(supported_protocols))
```

### Comparing `vo-wot-0.18.3/wotpy/wot/td.py` & `vo_wot-0.18.4/wotpy/wot/td.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/thing.py` & `vo_wot-0.18.4/wotpy/wot/thing.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/validation.py` & `vo_wot-0.18.4/wotpy/wot/validation.py`

 * *Files identical despite different names*

### Comparing `vo-wot-0.18.3/wotpy/wot/wot.py` & `vo_wot-0.18.4/wotpy/wot/wot.py`

 * *Files identical despite different names*

