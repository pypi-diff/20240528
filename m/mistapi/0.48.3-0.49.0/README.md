# Comparing `tmp/mistapi-0.48.3.tar.gz` & `tmp/mistapi-0.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.48.3.tar", last modified: Fri May 24 11:02:18 2024, max compression
+gzip compressed data, was "mistapi-0.49.0.tar", last modified: Tue May 28 17:48:14 2024, max compression
```

## Comparing `mistapi-0.48.3.tar` & `mistapi-0.49.0.tar`

### file list

```diff
@@ -1,255 +1,256 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.766155 mistapi-0.48.3/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.48.3/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-24 11:02:18.766001 mistapi-0.48.3/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10541 2023-10-05 14:00:29.000000 mistapi-0.48.3/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      977 2024-05-24 11:00:59.000000 mistapi-0.48.3/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2024-05-24 11:02:18.766462 mistapi-0.48.3/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.676361 mistapi-0.48.3/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.682055 mistapi-0.48.3/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)    15410 2023-10-10 06:25:01.000000 mistapi-0.48.3/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3275 2023-10-10 08:14:00.000000 mistapi-0.48.3/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    34436 2024-05-14 11:10:23.000000 mistapi-0.48.3/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      615 2024-05-24 11:00:59.000000 mistapi-0.48.3/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2297 2023-10-19 16:39:16.000000 mistapi-0.48.3/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.683752 mistapi-0.48.3/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.48.3/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.48.3/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2079 2023-10-10 06:34:01.000000 mistapi-0.48.3/src/mistapi/__pagination.py
--rw-r--r--   0 tmunzer    (502) staff       (20)       74 2024-05-24 11:00:59.000000 mistapi-0.48.3/src/mistapi/__version.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.684131 mistapi-0.48.3/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.684364 mistapi-0.48.3/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.689532 mistapi-0.48.3/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1490 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1757 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2045 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1795 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/app_categories.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1816 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/app_subcategories.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1741 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1735 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1274 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1792 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/gateway_applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1757 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1740 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/license_types.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1777 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/nac_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1833 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/otherdevice_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1823 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/otherdevice_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/system_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.689699 mistapi-0.48.3/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.691026 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1986 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2302 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11080 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1990 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1965 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1958 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7996 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.691405 mistapi-0.48.3/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.691682 mistapi-0.48.3/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.692455 mistapi-0.48.3/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.692761 mistapi-0.48.3/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      999 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.697301 mistapi-0.48.3/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.714212 mistapi-0.48.3/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3923 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1625 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2651 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4390 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4723 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6587 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1662 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4046 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7394 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3705 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/suggestion.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3267 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.738781 mistapi-0.48.3/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3465 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3286 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8408 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4723 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5211 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5243 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6578 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    11110 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7159 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    18232 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5293 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5351 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6599 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5211 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/idpprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2878 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6362 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7000 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5170 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1931 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1293 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/mist_nac.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5235 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    22918 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5155 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    10477 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/nac_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9105 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/nacportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5383 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1323 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3018 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9485 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4818 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    10496 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8446 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5211 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6962 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4768 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5202 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5306 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    19138 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5183 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8773 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5269 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8750 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5754 2024-05-24 11:01:02.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    29808 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5938 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7359 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1592 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5122 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/usermacs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1611 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/vars.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5022 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1780 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4604 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7350 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3553 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7462 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5727 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6383 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5155 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.739310 mistapi-0.48.3/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.739891 mistapi-0.48.3/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      555 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1308 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/register/recaptcha.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.741549 mistapi-0.48.3/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4315 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2652 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1771 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1890 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.764468 mistapi-0.48.3/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2837 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8111 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1879 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5278 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6627 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5140 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    17220 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2270 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    66069 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3933 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4898 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1331 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8941 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9224 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6914 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    16636 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8708 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    10279 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/nac_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2228 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1331 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5706 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5829 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7694 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5113 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4704 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5192 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2277 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6103 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6746 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1322 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3624 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    18950 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    63589 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1751 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3150 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5423 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5164 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2176 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2200 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1786 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4622 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7210 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3770 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8664 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5770 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6432 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5192 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5080 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.765211 mistapi-0.48.3/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2024-05-24 11:01:03.000000 mistapi-0.48.3/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    13223 2023-10-11 11:11:09.000000 mistapi-0.48.3/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 11:02:18.765531 mistapi-0.48.3/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-24 11:02:18.000000 mistapi-0.48.3/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     8512 2024-05-24 11:02:18.000000 mistapi-0.48.3/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2024-05-24 11:02:18.000000 mistapi-0.48.3/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2024-05-24 11:02:18.000000 mistapi-0.48.3/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2024-05-24 11:02:18.000000 mistapi-0.48.3/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.192721 mistapi-0.49.0/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.49.0/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-28 17:48:14.192572 mistapi-0.49.0/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10541 2023-10-05 14:00:29.000000 mistapi-0.49.0/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      977 2024-05-28 17:47:43.000000 mistapi-0.49.0/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2024-05-28 17:48:14.192967 mistapi-0.49.0/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.141197 mistapi-0.49.0/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.146234 mistapi-0.49.0/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15410 2023-10-10 06:25:01.000000 mistapi-0.49.0/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3275 2023-10-10 08:14:00.000000 mistapi-0.49.0/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    34436 2024-05-14 11:10:23.000000 mistapi-0.49.0/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      615 2024-05-28 17:47:43.000000 mistapi-0.49.0/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2297 2023-10-19 16:39:16.000000 mistapi-0.49.0/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.147563 mistapi-0.49.0/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.49.0/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.49.0/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2079 2023-10-10 06:34:01.000000 mistapi-0.49.0/src/mistapi/__pagination.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)       74 2024-05-28 17:47:43.000000 mistapi-0.49.0/src/mistapi/__version.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.147805 mistapi-0.49.0/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.147951 mistapi-0.49.0/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.151344 mistapi-0.49.0/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1490 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1757 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2045 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1758 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1795 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/app_categories.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1816 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/app_subcategories.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1741 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1735 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1274 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1792 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/gateway_applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1757 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1740 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1777 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/nac_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1833 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/otherdevice_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1823 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/otherdevice_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1798 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/system_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.151482 mistapi-0.49.0/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.152729 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      743 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1986 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2302 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11080 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1990 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1958 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7996 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.153050 mistapi-0.49.0/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.153362 mistapi-0.49.0/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.154070 mistapi-0.49.0/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.154360 mistapi-0.49.0/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      999 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.154640 mistapi-0.49.0/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.157804 mistapi-0.49.0/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3923 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1625 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2651 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4390 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4723 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6587 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1662 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4046 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7394 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3705 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3267 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.174003 mistapi-0.49.0/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3505 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3286 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8408 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4723 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5211 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5243 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6578 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11110 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7159 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    18232 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1607 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5293 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5351 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6599 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5211 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/idpprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2878 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6362 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7000 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5170 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1931 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1293 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/mist_nac.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5235 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    22918 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5155 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10477 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/nac_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9105 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/nacportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5535 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1323 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3018 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9485 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4818 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    12968 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9171 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5211 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6962 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4768 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5202 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5306 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    19138 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5183 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8773 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5269 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5127 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8750 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5754 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    29808 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5938 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7359 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1592 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5122 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/usermacs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1611 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/vars.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5022 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1780 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4690 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8983 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3553 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7462 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5727 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6383 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5155 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.174531 mistapi-0.49.0/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.175235 mistapi-0.49.0/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      555 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1308 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/register/recaptcha.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.176927 mistapi-0.49.0/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4315 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2652 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1771 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1890 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.191457 mistapi-0.49.0/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2882 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8171 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1879 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5278 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6627 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5140 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17220 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2270 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    70846 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3933 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4898 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1331 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8941 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9224 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6914 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    16636 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8708 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10832 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/nac_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2228 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1331 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5706 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5829 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7694 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5113 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4782 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5192 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2277 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6103 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6746 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1322 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3624 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    18950 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    63589 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1751 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3150 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5423 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5164 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2176 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2200 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1786 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4622 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4124 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wan_usages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9038 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3770 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8664 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5770 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6432 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5192 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5080 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.191999 mistapi-0.49.0/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2024-05-28 17:47:46.000000 mistapi-0.49.0/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    13223 2023-10-11 11:11:09.000000 mistapi-0.49.0/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-28 17:48:14.192222 mistapi-0.49.0/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-28 17:48:14.000000 mistapi-0.49.0/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8536 2024-05-28 17:48:14.000000 mistapi-0.49.0/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2024-05-28 17:48:14.000000 mistapi-0.49.0/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2024-05-28 17:48:14.000000 mistapi-0.49.0/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2024-05-28 17:48:14.000000 mistapi-0.49.0/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.48.3/LICENSE` & `mistapi-0.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/PKG-INFO` & `mistapi-0.49.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.48.3
+Version: 0.49.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.48.3/README.md` & `mistapi-0.49.0/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/pyproject.toml` & `mistapi-0.49.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.48.3"
+version = "0.49.0"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mistapi-0.48.3/src/mistapi/__api_request.py` & `mistapi-0.49.0/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/__api_response.py` & `mistapi-0.49.0/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/__api_session.py` & `mistapi-0.49.0/src/mistapi/__api_session.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/__init__.py` & `mistapi-0.49.0/src/mistapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/__logger.py` & `mistapi-0.49.0/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/__models/privilege.py` & `mistapi-0.49.0/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/__pagination.py` & `mistapi-0.49.0/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listAlarmDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listAlarmDefinitions")
 def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listApChannels")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listApChannels")
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listApLedDefinition")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listApLedDefinition")
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/app_categories.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/app_categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listAppCategoryDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listAppCategoryDefinitions")
 def getAppCategoryDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAppCategoryDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/app_subcategories.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/app_subcategories.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listAppSubCategoryDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listAppSubCategoryDefinitions")
 def getAppSubCategoryDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAppSubCategoryDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/applications.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listApplications")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listApplications")
 def getApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/client_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listClientEventsDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listClientEventsDefinitions")
 def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/countries.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/countries.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listCountryCodes")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listCountryCodes")
 def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/device_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listDeviceEventsDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listDeviceEventsDefinitions")
 def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/device_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listDeviceModels")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listDeviceModels")
 def getDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/gateway_applications.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/gateway_applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listGatewayApplications")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listGatewayApplications")
 def getGatewayApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listGatewayApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInsightMetrics")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInsightMetrics")
 def getInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInsightMetrics
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/languages.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/languages.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteLanguages")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteLanguages")
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/license_types.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/license_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMxEdgeEventsDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMxEdgeEventsDefinitions")
 def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMxEdgeModels")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMxEdgeModels")
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/nac_events.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/nac_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listNacEventsDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listNacEventsDefinitions")
 def getNacEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listNacEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/otherdevice_events.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/otherdevice_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOtherDeviceEventsDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOtherDeviceEventsDefinitions")
 def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/otherdevice_models.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/otherdevice_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSupportedOtherDeviceModels")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSupportedOtherDeviceModels")
 def getSupportedOtherDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSupportedOtherDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/system_events.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/system_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSystemEventsDefinitions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSystemEventsDefinitions")
 def getSystemEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSystemEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.49.0/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listTrafficTypes")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listTrafficTypes")
 def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,10 +10,9 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi.api.v1.installer.orgs import alarmtemplates
 from mistapi.api.v1.installer.orgs import deviceprofiles
 from mistapi.api.v1.installer.orgs import devices
 from mistapi.api.v1.installer.orgs import rftemplates
-from mistapi.api.v1.installer.orgs import secpolicies
 from mistapi.api.v1.installer.orgs import sitegroups
 from mistapi.api.v1.installer.orgs import sites
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerAlarmTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInstallerAlarmTemplates")
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerDeviceProfiles")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInstallerDeviceProfiles")
 def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerListOfRenctlyClaimedDevices")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInstallerListOfRenctlyClaimedDevices")
 def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str, model:str=None, site_name:str=None, site_id:str=None, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerRfTemplatesNames")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInstallerRfTemplatesNames")
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/licenses.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerSecPolicies")
-def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgLicencesSummary(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
+    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesSummary
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +28,49 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/secpolicies"
+    uri = f"/api/v1/orgs/{org_id}/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def moveOrDeleteOrgLicenseToAnotherOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
+    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteOrgLicenseToAnotherOrg
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/licenses"
+    resp = mist_session.mist_put(uri=uri, body=body)
+    return resp
+    
+def getOrgLicencesBySite(mist_session:_APISession, org_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesBySite
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,12 +78,12 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/secpolicies"
+    uri = f"/api/v1/orgs/{org_id}/licenses/usages"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerSiteGroups")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInstallerSiteGroups")
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerSites")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInstallerSites")
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -85,15 +85,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listInstallerMaps")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listInstallerMaps")
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.49.0/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.49.0/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/login/login.py` & `mistapi-0.49.0/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.49.0/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.49.0/src/mistapi/api/v1/login/oauth.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.49.0/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.49.0/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.49.0/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/admins.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspAdmins")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspAdmins")
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/licenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspLicenses")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspLicenses")
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspLogs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspLogs")
 def getMspLogs(mist_session:_APISession, msp_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspOrgGroups")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspOrgGroups")
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/orgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspOrgs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspOrgs")
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/search.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/search.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspSsoRoles")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspSsoRoles")
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspSsos")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspSsos")
 def getMspSsos(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -160,15 +160,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspSsoLatestFailures")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspSsoLatestFailures")
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspOrgLicenses")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspOrgLicenses")
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -57,15 +57,15 @@
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspOrgStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspOrgStats")
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/suggestion.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/suggestion.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.49.0/src/mistapi/api/v1/msps/tickets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listMspTickets")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listMspTickets")
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
     This package is licensed under the MIT License.
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi.api.v1.orgs import orgs
+from mistapi.api.v1.orgs import events
 from mistapi.api.v1.orgs import ssr
 from mistapi.api.v1.orgs import admins
 from mistapi.api.v1.orgs import alarms
 from mistapi.api.v1.orgs import alarmtemplates
 from mistapi.api.v1.orgs import apitokens
 from mistapi.api.v1.orgs import aptemplates
 from mistapi.api.v1.orgs import assetfilters
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/admins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgAdmins")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgAdmins")
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgAlarmTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgAlarmTemplates")
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSuppressedAlarms")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSuppressedAlarms")
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str, scope:str="site") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgApiTokens")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgApiTokens")
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgAptemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgAptemplates")
 def getOrgAptemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgAssetFilters")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgAssetFilters")
 def getOrgAssetFilters(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgAssets")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgAssets")
 def getOrgAssets(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgDeviceProfiles")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgDeviceProfiles")
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgDevices")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgDevices")
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -295,15 +295,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgApsMacs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgApsMacs")
 def getOrgApsMacs(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -430,15 +430,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgMultiSitesDevicesUpgrades")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgMultiSitesDevicesUpgrades")
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgEvpnTopologies")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgEvpnTopologies")
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgGatewayTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgGatewayTemplates")
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgGuestAuthorizations")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgGuestAuthorizations")
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/idpprofiles.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/idpprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgIdpProfiles")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgIdpProfiles")
 def getOrgIdpProfiles(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgIdpProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/insights.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgJsiDevices")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgJsiDevices")
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -157,15 +157,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgJsiPastPurchases")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgJsiPastPurchases")
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/oauth.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,80 +10,62 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOrgLicencesSummary(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOauth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesSummary
+    API doc: https://doc.mist-lab.fr/#operation/getOauth2UrlForLinking
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    provider : str        
+    
+    QUERY PARAMS
+    ------------
+    forward : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/licenses"
-    query_params={}
+    uri = f"/api/v1/self/oauth/{provider}"
+    query_params={}
+    if forward: query_params["forward"]=forward
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def moveOrDeleteOrgLicenseToAnotherOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def linkOauth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteOrgLicenseToAnotherOrg
+    API doc: https://doc.mist-lab.fr/#operation/linkOauth2MistAccount
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    provider : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/licenses"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
-def getOrgLicencesBySite(mist_session:_APISession, org_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesBySite
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/licenses/usages"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/oauth/{provider}"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgLogs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgLogs")
 def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/maps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/mist_nac.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/mist_nac.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgMxEdgeClusters")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgMxEdgeClusters")
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgMxEdges")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgMxEdges")
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -375,15 +375,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgMxEdgeUpgrades")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgMxEdgeUpgrades")
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgMxTunnels")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgMxTunnels")
 def getOrgMxTunnels(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/nac_clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/nac_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/nacportals.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/nacportals.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgNacPortals")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgNacPortals")
 def getOrgNacPortals(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacPortals
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -174,15 +174,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nacportals/{nacportal_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgNacPortalSsoLatestFailures")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgNacPortalSsoLatestFailures")
 def getOrgNacPortalSsoLatestFailures(mist_session:_APISession, org_id:str, nacportal_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacPortalSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgNacRules")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgNacRules")
 def getOrgNacRules(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/nactags.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgNacTags")
-def getOrgNacTags(mist_session:_APISession, org_id:str, type:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgNacTags")
+def getOrgNacTags(mist_session:_APISession, org_id:str, type:str=None, name:str=None, match:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -28,32 +28,34 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     type : str
     name : str
+    match : str
     page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nactags"
     query_params={}
     if type: query_params["type"]=type
     if name: query_params["name"]=name
+    if match: query_params["match"]=match
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgNacTags(mist_session:_APISession, org_id:str, type:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
+def listOrgNacTags(mist_session:_APISession, org_id:str, type:str=None, name:str=None, match:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -62,26 +64,28 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     type : str
     name : str
+    match : str
     page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/nactags"
     query_params={}
     if type: query_params["type"]=type
     if name: query_params["name"]=name
+    if match: query_params["match"]=match
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def createOrgNacTag(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgNetworks")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgNetworks")
 def getOrgNetworks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgNetworkTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgNetworkTemplates")
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgOtherDevices")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgOtherDevices")
 def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/pcaps.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/pcaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgPacketCaptures")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgPacketCaptures")
 def getOrgPacketCaptures(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPacketCaptures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/pma.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgPmaDashboards")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgPmaDashboards")
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgPskPortals")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgPskPortals")
 def getOrgPskPortals(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/pskportals"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgPskPortalLogs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgPskPortalLogs")
 def getOrgPskPortalLogs(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortalLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -334,8 +334,94 @@
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
+    
+def deleteOrgPskPortalImage(mist_session:_APISession, org_id:str, pskportal_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgPskPortalImage
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str
+    pskportal_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}/portal_image"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def uploadOrgPskPortalImageFile(mist_session:_APISession, org_id:str, pskportal_id:str, file:str=None, json:str=None) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/uploadOrgPskPortalImage
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str
+    pskportal_id : str        
+    
+    BODY PARAMS
+    -----------
+    file : str
+        path to the file to upload. Binary file
+    json : str
+        JSON string describing the upload
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    multipart_form_data = {
+        "file":file,
+        "json":json,
+    }
+    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}/portal_image"
+    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    return resp
+
+def updateOrgPskPortalTemplate(mist_session:_APISession, org_id:str, pskportal_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgPskPortalTemplate
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str
+    pskportal_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/pskportals/{pskportal_id}/portal_template"
+    resp = mist_session.mist_put(uri=uri, body=body)
+    return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/psks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgPsks")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgPsks")
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -137,14 +137,41 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/psks"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
+def deleteOrgPskList(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgPskList
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/psks/delete"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def importOrgPsksFile(mist_session:_APISession, org_id:str, file:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/importOrgPsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgRfTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgRfTemplates")
 def getOrgRfTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSdkInvites")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSdkInvites")
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSdkTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSdkTemplates")
 def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSecPolicies")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSecPolicies")
 def getOrgSecPolicies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgServicePolicies")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgServicePolicies")
 def getOrgServicePolicies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgServices")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgServices")
 def getOrgServices(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSiteGroups")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSiteGroups")
 def getOrgSiteGroups(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/sites.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSites")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSites")
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSiteTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSiteTemplates")
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSsoRoles")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSsoRoles")
 def getOrgSsoRoles(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSsos")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSsos")
 def getOrgSsos(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -174,15 +174,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSsoLatestFailures")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSsoLatestFailures")
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgSsrUpgrades")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgSsrUpgrades")
 def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -135,15 +135,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssr/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgAvailableSsrVersions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgAvailableSsrVersions")
 def getOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgAssetsStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgAssetsStats")
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -255,15 +255,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgDevicesStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgDevicesStats")
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None, fields:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -356,15 +356,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgMxEdgesStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgMxEdgesStats")
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgTemplates")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgTemplates")
 def getOrgTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgTickets")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgTickets")
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/usermacs.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/usermacs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgUserMacs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgUserMacs")
 def getOrgUserMacs(mist_session:_APISession, org_id:str, blacklisted:bool=None, for_guest_wifi:bool=None, cross_site:bool=None, site_id:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgUserMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/vars.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/vars.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgsVpns")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgsVpns")
 def getOrgsVpns(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/wan_client.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/wan_clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/wan_clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgWanClients(mist_session:_APISession, org_id:str, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchOrgWanClients(mist_session:_APISession, org_id:str, mac:str=None, hostname:str=None, ip:str=None, network:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgWanClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -112,14 +112,15 @@
     org_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
     hostname : str
     ip : str
+    network : str
     mfg : str
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
@@ -129,14 +130,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wan_clients/search"
     query_params={}
     if mac: query_params["mac"]=mac
     if hostname: query_params["hostname"]=hostname
     if ip: query_params["ip"]=ip
+    if network: query_params["network"]=network
     if mfg: query_params["mfg"]=mfg
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgWebhooks")
-def getOrgWebhooks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgWlans")
+def getOrgWlans(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,24 +34,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/orgs/{org_id}/wlans"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgWebhooks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listOrgWlans(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -64,24 +64,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/orgs/{org_id}/wlans"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgWebhook(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgWlan(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/createOrgWlan
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,156 +94,173 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks"
+    uri = f"/api/v1/orgs/{org_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
+def getOrgWLAN(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/getOrgWLAN
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    webhook_id : str        
+    wlan_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
+def deleteOrgWlan(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWlan
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    webhook_id : str        
+    wlan_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str, body:object) -> _APIResponse:
+def updateOrgWlan(mist_session:_APISession, org_id:str, wlan_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgWebhook
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgWlan
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    webhook_id : str        
+    wlan_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def searchOrgWebhooksDeliveries(mist_session:_APISession, org_id:str, webhook_id:str, site_id:str=None, error:str=None, status_code:int=None, status:str=None, topic:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
+def deleteOrgWlanPortalImage(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgWebhooksDeliveries
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWlanPortalImage
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    webhook_id : str        
-    
-    QUERY PARAMS
-    ------------
-    site_id : str
-    error : str
-    status_code : int
-    status : str{'success', 'failure'}
-    topic : str{'alarms', 'audits', 'device-updowns', 'occupancy-alerts', 'ping'}
-      webhook topic
-    start : int
-    end : int
-    duration : str, default: 1d
-    limit : int, default: 100        
+    wlan_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}/events/search"
-    query_params={}
-    if site_id: query_params["site_id"]=site_id
-    if error: query_params["error"]=error
-    if status_code: query_params["status_code"]=status_code
-    if status: query_params["status"]=status
-    if topic: query_params["topic"]=topic
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_image"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def pingOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
+def uploadOrgWlanPortalImageFile(mist_session:_APISession, org_id:str, wlan_id:str, file:str=None, json:str=None) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/uploadOrgWlanPortalImage
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str
+    wlan_id : str        
+    
+    BODY PARAMS
+    -----------
+    file : str
+        path to the file to upload. binary file
+    json : str
+        JSON string describing your upload
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
     """
-    API doc: https://doc.mist-lab.fr/#operation/pingOrgWebhook
+    multipart_form_data = {
+        "file":file,
+        "json":json,
+    }
+    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_image"
+    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    return resp
+
+def updateOrgWlanPortalTemplate(mist_session:_APISession, org_id:str, wlan_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgWlanPortalTemplate
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    webhook_id : str        
+    wlan_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}/ping"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_template"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgWlans")
-def getOrgWlans(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgWebhooks")
+def getOrgWebhooks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,24 +34,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans"
+    uri = f"/api/v1/orgs/{org_id}/webhooks"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgWlans(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listOrgWebhooks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
+    API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -64,24 +64,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans"
+    uri = f"/api/v1/orgs/{org_id}/webhooks"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgWlan(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgWebhook(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgWlan
+    API doc: https://doc.mist-lab.fr/#operation/createOrgWebhook
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,173 +94,202 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans"
+    uri = f"/api/v1/orgs/{org_id}/webhooks"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgWLAN(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
+def getOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgWLAN
+    API doc: https://doc.mist-lab.fr/#operation/getOrgWebhook
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    wlan_id : str        
+    webhook_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}"
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgWlan(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
+def deleteOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWlan
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWebhook
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    wlan_id : str        
+    webhook_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}"
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgWlan(mist_session:_APISession, org_id:str, wlan_id:str, body:object) -> _APIResponse:
+def updateOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgWlan
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgWebhook
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    wlan_id : str        
+    webhook_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}"
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def deleteOrgWlanPortalImage(mist_session:_APISession, org_id:str, wlan_id:str) -> _APIResponse:
+def countOrgWebhooksDeliveries(mist_session:_APISession, org_id:str, webhook_id:str, error:str=None, status_code:int=None, status:str=None, topic:str=None, distinct:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgWlanPortalImage
+    API doc: https://doc.mist-lab.fr/#operation/countOrgWebhooksDeliveries
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    wlan_id : str        
+    webhook_id : str        
+    
+    QUERY PARAMS
+    ------------
+    error : str
+    status_code : int
+    status : str{'success', 'failure'}
+      webhook delivery status
+    topic : str{'alarms', 'audits', 'device-updowns', 'occupancy-alerts', 'ping'}
+      webhook topic
+    distinct : str{'status', 'topic', 'status_code', 'webhook_id'}
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_image"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}/events/count"
+    query_params={}
+    if error: query_params["error"]=error
+    if status_code: query_params["status_code"]=status_code
+    if status: query_params["status"]=status
+    if topic: query_params["topic"]=topic
+    if distinct: query_params["distinct"]=distinct
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def uploadOrgWlanPortalImageFile(mist_session:_APISession, org_id:str, wlan_id:str, file:str=None, json:str=None) -> _APIResponse:
+def searchOrgWebhooksDeliveries(mist_session:_APISession, org_id:str, webhook_id:str, error:str=None, status_code:int=None, status:str=None, topic:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/uploadOrgWlanPortalImage
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgWebhooksDeliveries
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    wlan_id : str        
+    webhook_id : str        
     
-    BODY PARAMS
-    -----------
-    file : str
-        path to the file to upload. binary file
-    json : str
-        JSON string describing your upload
+    QUERY PARAMS
+    ------------
+    error : str
+    status_code : int
+    status : str{'success', 'failure'}
+      webhook delivery status
+    topic : str{'alarms', 'audits', 'device-updowns', 'occupancy-alerts', 'ping'}
+      webhook topic
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    multipart_form_data = {
-        "file":file,
-        "json":json,
-    }
-    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_image"
-    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}/events/search"
+    query_params={}
+    if error: query_params["error"]=error
+    if status_code: query_params["status_code"]=status_code
+    if status: query_params["status"]=status
+    if topic: query_params["topic"]=topic
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
-
-def updateOrgWlanPortalTemplate(mist_session:_APISession, org_id:str, wlan_id:str, body:object) -> _APIResponse:
+    
+def pingOrgWebhook(mist_session:_APISession, org_id:str, webhook_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgWlanPortalTemplate
+    API doc: https://doc.mist-lab.fr/#operation/pingOrgWebhook
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    wlan_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    webhook_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wlans/{wlan_id}/portal_template"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}/ping"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgWxRules")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgWxRules")
 def getOrgWxRules(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgWxTags")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgWxTags")
 def getOrgWxTags(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listOrgWxTunnels")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listOrgWxTunnels")
 def getOrgWxTunnels(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.49.0/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.49.0/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/register/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/register/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/register/recaptcha.py` & `mistapi-0.49.0/src/mistapi/api/v1/register/recaptcha.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/register/register.py` & `mistapi-0.49.0/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/register/verify.py` & `mistapi-0.49.0/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listApiTokens")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listApiTokens")
 def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/logs.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSelfAuditLogs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSelfAuditLogs")
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/two_factor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,62 +10,54 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOauth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
+def generateSecretFor2faVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOauth2UrlForLinking
+    API doc: https://doc.mist-lab.fr/#operation/generateSecretFor2faVerification
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    provider : str        
-    
     QUERY PARAMS
     ------------
-    forward : str        
+    by : str{'qrcode'}, default: qrcode        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/oauth/{provider}"
+    uri = f"/api/v1/self/two_factor/token"
     query_params={}
-    if forward: query_params["forward"]=forward
+    if by: query_params["by"]=by
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def linkOauth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
+def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/linkOauth2MistAccount
+    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    provider : str        
-    
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/oauth/{provider}"
+    uri = f"/api/v1/self/two_factor/verify"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/self.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listAlarmSubscriptions")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listAlarmSubscriptions")
 def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/sites.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,54 +10,80 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def generateSecretFor2faVerification(mist_session:_APISession, by:str="qrcode") -> _APIResponse:
+def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/generateSecretFor2faVerification
+    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    QUERY PARAMS
-    ------------
-    by : str{'qrcode'}, default: qrcode        
+    PATH PARAMS
+    -----------
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/two_factor/token"
-    query_params={}
-    if by: query_params["by"]=by
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def verifyTwoFactor(mist_session:_APISession, body:object) -> _APIResponse:
+def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifyTwoFactor
+    API doc: https://doc.mist-lab.fr/#operation/deleteSite
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/two_factor/verify"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/self/update.py` & `mistapi-0.49.0/src/mistapi/api/v1/self/update.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 from mistapi.api.v1.sites import subscriptions
 from mistapi.api.v1.sites import synthetic_test
 from mistapi.api.v1.sites import uisettings
 from mistapi.api.v1.sites import vbeacons
 from mistapi.api.v1.sites import vpns
 from mistapi.api.v1.sites import wan_client
 from mistapi.api.v1.sites import wan_clients
+from mistapi.api.v1.sites import wan_usages
 from mistapi.api.v1.sites import webhooks
 from mistapi.api.v1.sites import wired_clients
 from mistapi.api.v1.sites import wlans
 from mistapi.api.v1.sites import wxrules
 from mistapi.api.v1.sites import wxtags
 from mistapi.api.v1.sites import wxtunnels
 from mistapi.api.v1.sites import zones
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/alarms.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'type', 'acked', 'severity', 'group'}, default: type
+      Group by and count the alarms by some distinct field
     ack_admin_name : str
     acked : bool
     type : str
     severity : str
     group : str
     page : int, default: 1
     limit : int, default: 100
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/networks.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,54 +10,64 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteApps")
-def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteNetworksDerived")
+def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    QUERY PARAMS
+    ------------
+    resolve : bool        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    QUERY PARAMS
+    ------------
+    resolve : bool        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/aptemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/aptemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteAssetFilters")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteAssetFilters")
 def getSiteAssetFilters(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteAssets")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteAssets")
 def getSiteAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/beacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteBeacons")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteBeacons")
 def getSiteBeacons(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/count.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/count.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/deviceprofiles.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/deviceprofiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteDeviceProfilesDerived")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteDeviceProfilesDerived")
 def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteDevices")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteDevices")
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -646,15 +646,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/send_ble_beacon"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteDevicesUpgrade")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteDevicesUpgrade")
 def getSiteDevicesUpgrade(mist_session:_APISession, site_id:str, status:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesUpgrade
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -804,15 +804,42 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade_bios"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteAvailableDeviceVersions")
+def upgradeSiteMultipleDevicesFpga(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/upgradeSiteMultipleDevicesFpga
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/upgrade_fpga"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteAvailableDeviceVersions")
 def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1164,14 +1191,42 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/clear_bpdu_error"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def clearSiteDeviceMacTable(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/clearSiteDeviceMacTable
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/clear_mac_table"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def clearAllLearnedMacsFromPortOnSwitch(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/clearAllLearnedMacsFromPortOnSwitch
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1437,35 +1492,68 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/local_port_config"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def startSiteLocateDevice(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
+def startSiteLocateDevice(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/startSiteLocateDevice
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
     device_id : str        
     
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/locate"
-    resp = mist_session.mist_post(uri=uri)
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def monitorSiteDeviceTraffic(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/monitorSiteDeviceTraffic
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/monitor_traffic"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
 def pingFromDevice(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/pingFromDevice
     
     PARAMS
@@ -1687,14 +1775,37 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/service_ping"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def createSiteDeviceShellSession(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/createSiteDeviceShellSession
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/shell"
+    resp = mist_session.mist_post(uri=uri)
+    return resp
+    
 def getSiteDeviceArpTable(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceArpTable
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1715,14 +1826,42 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/show_arp"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def getSiteDeviceBgpSummary(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceBgpSummary
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/show_bgp_rummary"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def getSiteDeviceEvpnDatabase(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceEvpnDatabase
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -2065,14 +2204,42 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/upgrade_bios"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def upgradeSiteDeviceFPGA(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/upgradeSiteDeviceFPGA
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/upgrade_fpga"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def getSiteDeviceVirtualChassis(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceVirtualChassis
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/events.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/events.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteEvpnTopologies")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteEvpnTopologies")
 def getSiteEvpnTopologies(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteEvpnTopologies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/gatewaytemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/gatewaytemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/guests.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteAllGuestAuthorizations")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteAllGuestAuthorizations")
 def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -105,15 +105,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteAllGuestAuthorizationsDerived")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteAllGuestAuthorizationsDerived")
 def getSiteAllGuestAuthorizationsDerived(mist_session:_APISession, site_id:str, wlan_id:str=None, cross_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizationsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteRogueAPs")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteRogueAPs")
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -167,15 +167,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteRogueClients")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteRogueClients")
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/location.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/location.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteMaps")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteMaps")
 def getSiteMaps(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteMxEdges")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteMxEdges")
 def getSiteMxEdges(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/nac_clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/nac_clients.py`

 * *Files 7% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searcsearcSiteNacClientEventsacClientEvents(mist_session:_APISession, site_id:str, type:str=None, nacrule_id:str=None, nacrule_matched:bool=None, dryrun_nacrule_id:str=None, dryrun_nacrule_matched:bool=None, auth_type:str=None, vlan:int=None, nas_vendor:str=None, bssid:str=None, idp_id:str=None, idp_role:str=None, resp_attrs:list=None, ssid:str=None, username:str=None, ap:str=None, random_mac:bool=None, mac:str=None, timestamp:float=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
+def searcsearcSiteNacClientEventsacClientEvents(mist_session:_APISession, site_id:str, type:str=None, nacrule_id:str=None, nacrule_matched:bool=None, dryrun_nacrule_id:str=None, dryrun_nacrule_matched:bool=None, auth_type:str=None, vlan:int=None, vlan_source:str=None, nas_vendor:str=None, bssid:str=None, idp_id:str=None, idp_role:str=None, idp_username:str=None, resp_attrs:list=None, ssid:str=None, username:str=None, usermac_labels:list=None, ap:str=None, random_mac:bool=None, mac:str=None, lookup_time_taken:float=None, timestamp:float=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searcsearcSiteNacClientEventsacClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -138,25 +138,30 @@
     type : str
     nacrule_id : str
     nacrule_matched : bool
     dryrun_nacrule_id : str
     dryrun_nacrule_matched : bool
     auth_type : str
     vlan : int
+    vlan_source : str
     nas_vendor : str
     bssid : str
     idp_id : str
     idp_role : str
+    idp_username : str
     resp_attrs : list
       Radius attributes returned by NAC to NAS Devive
     ssid : str
     username : str
+    usermac_labels : list
+      labels derived from usermac entry
     ap : str
     random_mac : bool
     mac : str
+    lookup_time_taken : float
     timestamp : float
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100        
     
     RETURN
@@ -169,59 +174,65 @@
     if type: query_params["type"]=type
     if nacrule_id: query_params["nacrule_id"]=nacrule_id
     if nacrule_matched: query_params["nacrule_matched"]=nacrule_matched
     if dryrun_nacrule_id: query_params["dryrun_nacrule_id"]=dryrun_nacrule_id
     if dryrun_nacrule_matched: query_params["dryrun_nacrule_matched"]=dryrun_nacrule_matched
     if auth_type: query_params["auth_type"]=auth_type
     if vlan: query_params["vlan"]=vlan
+    if vlan_source: query_params["vlan_source"]=vlan_source
     if nas_vendor: query_params["nas_vendor"]=nas_vendor
     if bssid: query_params["bssid"]=bssid
     if idp_id: query_params["idp_id"]=idp_id
     if idp_role: query_params["idp_role"]=idp_role
+    if idp_username: query_params["idp_username"]=idp_username
     if resp_attrs: query_params["resp_attrs"]=resp_attrs
     if ssid: query_params["ssid"]=ssid
     if username: query_params["username"]=username
+    if usermac_labels: query_params["usermac_labels"]=usermac_labels
     if ap: query_params["ap"]=ap
     if random_mac: query_params["random_mac"]=random_mac
     if mac: query_params["mac"]=mac
+    if lookup_time_taken: query_params["lookup_time_taken"]=lookup_time_taken
     if timestamp: query_params["timestamp"]=timestamp
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteNacClients(mist_session:_APISession, site_id:str, last_nacrule_id:str=None, nacrule_matched:bool=None, auth_type:str=None, last_vlan_id:str=None, last_nas_vendor:str=None, idp_id:str=None, last_ssid:str=None, last_username:str=None, timestamp:float=None, last_ap:str=None, mac:str=None, last_status:str=None, type:str=None, mdm_compliance_status:str=None, mdm_provider:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchSiteNacClients(mist_session:_APISession, site_id:str, nacrule_id:str=None, nacrule_matched:bool=None, auth_type:str=None, vlan_id:str=None, nas_vendor:str=None, idp_id:str=None, ssid:str=None, username:str=None, timestamp:float=None, ap:str=None, mac:str=None, mxedge_id:str=None, nacrule_name:str=None, status:str=None, type:str=None, mdm_compliance_status:str=None, mdm_provider:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteNacClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    last_nacrule_id : str
+    nacrule_id : str
     nacrule_matched : bool
     auth_type : str
-    last_vlan_id : str
-    last_nas_vendor : str
+    vlan_id : str
+    nas_vendor : str
     idp_id : str
-    last_ssid : str
-    last_username : str
+    ssid : str
+    username : str
     timestamp : float
-    last_ap : str
+    ap : str
     mac : str
-    last_status : str
+    mxedge_id : str
+    nacrule_name : str
+    status : str
     type : str
     mdm_compliance_status : str
     mdm_provider : str
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
@@ -230,26 +241,28 @@
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/nac_clients/search"
     query_params={}
-    if last_nacrule_id: query_params["last_nacrule_id"]=last_nacrule_id
+    if nacrule_id: query_params["nacrule_id"]=nacrule_id
     if nacrule_matched: query_params["nacrule_matched"]=nacrule_matched
     if auth_type: query_params["auth_type"]=auth_type
-    if last_vlan_id: query_params["last_vlan_id"]=last_vlan_id
-    if last_nas_vendor: query_params["last_nas_vendor"]=last_nas_vendor
+    if vlan_id: query_params["vlan_id"]=vlan_id
+    if nas_vendor: query_params["nas_vendor"]=nas_vendor
     if idp_id: query_params["idp_id"]=idp_id
-    if last_ssid: query_params["last_ssid"]=last_ssid
-    if last_username: query_params["last_username"]=last_username
+    if ssid: query_params["ssid"]=ssid
+    if username: query_params["username"]=username
     if timestamp: query_params["timestamp"]=timestamp
-    if last_ap: query_params["last_ap"]=last_ap
+    if ap: query_params["ap"]=ap
     if mac: query_params["mac"]=mac
-    if last_status: query_params["last_status"]=last_status
+    if mxedge_id: query_params["mxedge_id"]=mxedge_id
+    if nacrule_name: query_params["nacrule_name"]=nacrule_name
+    if status: query_params["status"]=status
     if type: query_params["type"]=type
     if mdm_compliance_status: query_params["mdm_compliance_status"]=mdm_compliance_status
     if mdm_provider: query_params["mdm_provider"]=mdm_provider
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/networks.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/vpns.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteNetworksDerived")
-def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteVpnsDerived")
+def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -33,23 +33,23 @@
     resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def listSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -61,13 +61,13 @@
     resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/networktemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/networktemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteOtherDevices")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteOtherDevices")
 def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSitePacketCaptures")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSitePacketCaptures")
 def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSitePsks")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSitePsks")
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/rftemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/rftemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/rogues.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/rogues.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/rrm.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,80 +59,82 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rrm/current/devices/{device_id}/band/{band}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteCurrentRrmNeighbors(mist_session:_APISession, site_id:str, device_id:str, band:str) -> _APIResponse:
+def getSiteRrmEvents(mist_session:_APISession, site_id:str, band:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentRrmNeighbors
+    API doc: https://doc.mist-lab.fr/#operation/getSiteRrmEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    device_id : str        
+    site_id : str        
     
     QUERY PARAMS
     ------------
     band : str{'24', '5', '6'}
-      802.11 Band        
+      802.11 Band
+    page : int, default: 1
+    limit : int, default: 100
+    start : int
+    end : int
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rrm/current/devices/{device_id}/neighbors"
+    uri = f"/api/v1/sites/{site_id}/rrm/events"
     query_params={}
-    if band: query_params["band"]=band
+    if band: query_params["band"]=band
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteRrmEvents(mist_session:_APISession, site_id:str, band:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def getSiteCurrentRrmNeighbors(mist_session:_APISession, site_id:str, band:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteRrmEvents
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentRrmNeighbors
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    band : str{'24', '5', '6'}
+      802.11 Band        
     
     QUERY PARAMS
     ------------
-    band : str{'24', '5', '6'}
-      802.11 Band
     page : int, default: 1
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rrm/events"
+    uri = f"/api/v1/sites/{site_id}/rrm/neighbors//band/{band}"
     query_params={}
-    if band: query_params["band"]=band
     if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def optimizeSiteRrm(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/optimizeSiteRrm
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteRssiZones")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteRssiZones")
 def getSiteRssiZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/servicepolicies.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/servicepolicies.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteServicePoliciesDerived")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteServicePoliciesDerived")
 def getSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicePoliciesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/services.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteServicesDerived")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteServicesDerived")
 def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
+def UnsubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSiteAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -28,62 +28,34 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSite
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}"
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def SubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/SubscribeSiteAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/sitetemplates.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/sitetemplates.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/skyatp.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/sle.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/sle.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/ssr.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteAssetsStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteAssetsStats")
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -262,15 +262,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteBeaconsStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteBeaconsStats")
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -505,15 +505,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteTroubleshootCalls")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteTroubleshootCalls")
 def getSiteTroubleshootCalls(mist_session:_APISession, site_id:str, client_mac:str, meeting_id:str, mac:str=None, app:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteTroubleshootCalls
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -592,15 +592,15 @@
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteWirelessClientsStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteWirelessClientsStats")
 def getSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -694,15 +694,15 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteDevicesStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteDevicesStats")
 def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -811,15 +811,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteDiscoveredAssets")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteDiscoveredAssets")
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1180,15 +1180,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteUnconnectedClientStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteUnconnectedClientStats")
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1229,15 +1229,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteMxEdgesStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteMxEdgesStats")
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1784,15 +1784,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteZonesStats")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteZonesStats")
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.49.0/src/mistapi/api/v1/orgs/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,52 +10,43 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def UnsubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
+def searchOrgEvents(mist_session:_APISession, org_id:str, type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSiteAlarms
+    API doc: https://doc.mist-lab.fr/#operation/searchOrgEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def SubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/SubscribeSiteAlarms
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
+    QUERY PARAMS
+    ------------
+    type : str
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/orgs/{org_id}//events/search"
+    query_params={}
+    if type: query_params["type"]=type
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/uisettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteUiSettings")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteUiSettings")
 def getSiteUiSettings(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUiSettings
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteVBeacons")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteVBeacons")
 def getSiteVBeacons(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/visits.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/visits.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/vpns.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/apps.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,64 +10,54 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteVpnsDerived")
-def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteApps")
+def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    resolve : bool        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vpns/derived"
-    query_params={}
-    if resolve: query_params["resolve"]=resolve
+    uri = f"/api/v1/sites/{site_id}/apps"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    resolve : bool        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vpns/derived"
-    query_params={}
-    if resolve: query_params["resolve"]=resolve
+    uri = f"/api/v1/sites/{site_id}/apps"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/wan_client.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/wan_client.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/wan_clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/wan_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteWebhooks")
-def getSiteWebhooks(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteWxTags")
+def getSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,24 +34,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks"
+    uri = f"/api/v1/sites/{site_id}/wxtags"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteWebhooks(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -64,24 +64,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks"
+    uri = f"/api/v1/sites/{site_id}/wxtags"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWebhook(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWxTag(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWebhook
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,152 +94,134 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks"
+    uri = f"/api/v1/sites/{site_id}/wxtags"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteWebhook(mist_session:_APISession, site_id:str, webhook_id:str) -> _APIResponse:
+def getSiteApplicationList(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWebhook
+    API doc: https://doc.mist-lab.fr/#operation/getSiteApplicationList
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    webhook_id : str        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtags/apps"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWebhook(mist_session:_APISession, site_id:str, webhook_id:str) -> _APIResponse:
+def getSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWebhook
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    webhook_id : str        
+    wxtag_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
     query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def updateSiteWebhook(mist_session:_APISession, site_id:str, webhook_id:str, body:object) -> _APIResponse:
+def deleteSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWebhook
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    webhook_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    wxtag_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def searchSiteWebhooksDeliveries(mist_session:_APISession, site_id:str, webhook_id:str, status_code:int=None, error:str=None, topic:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
+def updateSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteWebhooksDeliveries
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    webhook_id : str        
+    wxtag_id : str        
     
-    QUERY PARAMS
-    ------------
-    status_code : int
-    error : str
-    topic : str{'alarms', 'audits', 'device-updowns', 'occupancy-alerts', 'ping'}
-      webhook topic
-    start : int
-    end : int
-    duration : str, default: 1d
-    limit : int, default: 100        
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}/events/search"
-    query_params={}
-    if status_code: query_params["status_code"]=status_code
-    if error: query_params["error"]=error
-    if topic: query_params["topic"]=topic
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def pingSiteWebhook(mist_session:_APISession, site_id:str, webhook_id:str) -> _APIResponse:
+def getSiteCurrentMatchingClientsOfAWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/pingSiteWebhook
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentMatchingClientsOfAWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    webhook_id : str        
+    wxtag_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/webhooks/{webhook_id}/ping"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}/clients"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/wlans.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteWlans")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteWlans")
 def getSiteWlans(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteWlanDerived")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteWlanDerived")
 def getSiteWlanDerived(mist_session:_APISession, site_id:str, resolve:bool=None, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlanDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteWxRules")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteWxRules")
 def getSiteWxRules(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/zones.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteWxTags")
-def getSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteZones")
+def getSiteZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,24 +34,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listSiteZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -64,24 +64,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxTag(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTag
+    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,134 +94,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags"
+    uri = f"/api/v1/sites/{site_id}/zones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteApplicationList(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteApplicationList
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxtags/apps"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def getSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTag
+    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxtag_id : str        
+    zone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
+def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTag
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxtag_id : str        
+    zone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str, body:object) -> _APIResponse:
+def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTag
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxtag_id : str        
+    zone_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
-    
-def getSiteCurrentMatchingClientsOfAWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentMatchingClientsOfAWxTag
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str
-    wxtag_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}/clients"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.49.0/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.3", details="function replaced with listSiteWxTunnels")
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.49.0", details="function replaced with listSiteWxTunnels")
 def getSiteWxTunnels(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.49.0/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/api/v1/utils/test_twilio.py` & `mistapi-0.49.0/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi/cli.py` & `mistapi-0.49.0/src/mistapi/cli.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.48.3/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.49.0/src/mistapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.48.3
+Version: 0.49.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.48.3/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.49.0/src/mistapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 src/mistapi/api/v1/const/traffic_types.py
 src/mistapi/api/v1/installer/__init__.py
 src/mistapi/api/v1/installer/orgs/__init__.py
 src/mistapi/api/v1/installer/orgs/alarmtemplates.py
 src/mistapi/api/v1/installer/orgs/deviceprofiles.py
 src/mistapi/api/v1/installer/orgs/devices.py
 src/mistapi/api/v1/installer/orgs/rftemplates.py
-src/mistapi/api/v1/installer/orgs/secpolicies.py
 src/mistapi/api/v1/installer/orgs/sitegroups.py
 src/mistapi/api/v1/installer/orgs/sites.py
 src/mistapi/api/v1/installer/sites/__init__.py
 src/mistapi/api/v1/installer/sites/optimize.py
 src/mistapi/api/v1/invite/__init__.py
 src/mistapi/api/v1/invite/verify.py
 src/mistapi/api/v1/login/__init__.py
@@ -93,14 +92,15 @@
 src/mistapi/api/v1/orgs/cert.py
 src/mistapi/api/v1/orgs/claim.py
 src/mistapi/api/v1/orgs/clients.py
 src/mistapi/api/v1/orgs/clone.py
 src/mistapi/api/v1/orgs/crl.py
 src/mistapi/api/v1/orgs/deviceprofiles.py
 src/mistapi/api/v1/orgs/devices.py
+src/mistapi/api/v1/orgs/events.py
 src/mistapi/api/v1/orgs/evpn_topologies.py
 src/mistapi/api/v1/orgs/gatewaytemplates.py
 src/mistapi/api/v1/orgs/guests.py
 src/mistapi/api/v1/orgs/idpprofiles.py
 src/mistapi/api/v1/orgs/insights.py
 src/mistapi/api/v1/orgs/inventory.py
 src/mistapi/api/v1/orgs/invites.py
@@ -216,14 +216,15 @@
 src/mistapi/api/v1/sites/synthetic_test.py
 src/mistapi/api/v1/sites/uisettings.py
 src/mistapi/api/v1/sites/vbeacons.py
 src/mistapi/api/v1/sites/visits.py
 src/mistapi/api/v1/sites/vpns.py
 src/mistapi/api/v1/sites/wan_client.py
 src/mistapi/api/v1/sites/wan_clients.py
+src/mistapi/api/v1/sites/wan_usages.py
 src/mistapi/api/v1/sites/webhooks.py
 src/mistapi/api/v1/sites/wired_clients.py
 src/mistapi/api/v1/sites/wlans.py
 src/mistapi/api/v1/sites/wxrules.py
 src/mistapi/api/v1/sites/wxtags.py
 src/mistapi/api/v1/sites/wxtunnels.py
 src/mistapi/api/v1/sites/zones.py
```

