# Comparing `tmp/netbox_plugin_webhook_receiver-0.4.0.tar.gz` & `tmp/netbox_plugin_webhook_receiver-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_webhook_receiver-0.4.0.tar", max compression
+gzip compressed data, was "netbox_plugin_webhook_receiver-0.4.1.tar", max compression
```

## Comparing `netbox_plugin_webhook_receiver-0.4.0.tar` & `netbox_plugin_webhook_receiver-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1076 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/LICENSE
--rw-r--r--   0        0        0     2311 2023-07-06 10:02:50.221980 netbox_plugin_webhook_receiver-0.4.0/README.md
--rw-r--r--   0        0        0      502 2024-05-17 09:36:34.482282 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 09:47:06.597516 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/__init__.py
--rw-r--r--   0        0        0     1358 2024-05-17 10:32:54.491861 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/serializers.py
--rw-r--r--   0        0        0      274 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/urls.py
--rw-r--r--   0        0        0      621 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/views.py
--rw-r--r--   0        0        0      441 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/choices.py
--rw-r--r--   0        0        0      733 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/filtersets.py
--rw-r--r--   0        0        0     2930 2024-05-17 09:51:37.476254 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/forms.py
--rw-r--r--   0        0        0     4903 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/0001_initial.py
--rw-r--r--   0        0        0      428 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/0002_webhookreceiver_hash_algorithm.py
--rw-r--r--   0        0        0        0 2023-07-03 12:00:32.102516 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/__init__.py
--rw-r--r--   0        0        0     3261 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/models.py
--rw-r--r--   0        0        0      840 2024-05-17 09:55:22.379420 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/navigation.py
--rw-r--r--   0        0        0     1172 2023-07-04 15:19:05.740989 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/tables.py
--rw-r--r--   0        0        0     2929 2024-05-17 13:01:52.483716 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html
--rw-r--r--   0        0        0     1264 2024-05-17 10:02:32.566523 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html
--rw-r--r--   0        0        0     1789 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/urls.py
--rw-r--r--   0        0        0      133 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/__init__.py
--rw-r--r--   0        0        0     3819 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/views.py
--rw-r--r--   0        0        0      765 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceiver.py
--rw-r--r--   0        0        0     1122 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceivergroup.py
--rw-r--r--   0        0        0      736 2024-05-17 12:06:08.905691 netbox_plugin_webhook_receiver-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 netbox_plugin_webhook_receiver-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2311 2024-05-20 09:45:13.078022 netbox_plugin_webhook_receiver-0.4.1/README.md
+-rw-r--r--   0        0        0      502 2024-05-17 13:40:47.388893 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 09:47:06.597516 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/api/__init__.py
+-rw-r--r--   0        0        0     1358 2024-05-17 13:40:47.388893 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/api/serializers.py
+-rw-r--r--   0        0        0      274 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/api/urls.py
+-rw-r--r--   0        0        0      621 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/api/views.py
+-rw-r--r--   0        0        0      441 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/choices.py
+-rw-r--r--   0        0        0      733 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/filtersets.py
+-rw-r--r--   0        0        0     2986 2024-05-17 13:40:47.388893 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/forms.py
+-rw-r--r--   0        0        0     4903 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/migrations/0001_initial.py
+-rw-r--r--   0        0        0      428 2023-07-04 12:21:13.426684 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/migrations/0002_webhookreceiver_hash_algorithm.py
+-rw-r--r--   0        0        0        0 2023-07-03 12:00:32.102516 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/migrations/__init__.py
+-rw-r--r--   0        0        0     3261 2023-07-04 22:34:07.963776 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/models.py
+-rw-r--r--   0        0        0      840 2024-05-17 13:40:47.388893 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/navigation.py
+-rw-r--r--   0        0        0     1172 2023-07-04 15:19:05.740989 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/tables.py
+-rw-r--r--   0        0        0     3097 2024-05-20 09:46:15.733636 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html
+-rw-r--r--   0        0        0     1264 2024-05-17 13:40:47.388893 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html
+-rw-r--r--   0        0        0     1789 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/urls.py
+-rw-r--r--   0        0        0      133 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/views/__init__.py
+-rw-r--r--   0        0        0     3805 2024-05-28 15:42:47.864480 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/views/views.py
+-rw-r--r--   0        0        0      765 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/views/webhookreceiver.py
+-rw-r--r--   0        0        0     1122 2023-06-30 11:05:38.653389 netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/views/webhookreceivergroup.py
+-rw-r--r--   0        0        0      736 2024-05-28 15:46:30.816893 netbox_plugin_webhook_receiver-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3042 1970-01-01 00:00:00.000000 netbox_plugin_webhook_receiver-0.4.1/PKG-INFO
```

### Comparing `netbox_plugin_webhook_receiver-0.4.0/LICENSE` & `netbox_plugin_webhook_receiver-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/README.md` & `netbox_plugin_webhook_receiver-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - [x] Custom actions execution on successfully receving authenticated webhook message. Currently only one action available: Synchronize Netbox git 'Data Source'
 - [x] Use of standard Netbox jobs to queue webhook actions in the workers.
 - [ ] Additional actions to be implemented
 - [ ] Plugin configuration parameters
 
 ## Requirements
 
-* NetBox 3.5 or higher
+* NetBox 4.0 or higher
 * Python 3.10 or higher
 
 ## Installation & Configuration
 
 For general knowledge about netbox plugin installation please refer to the official guide: [Using Plugins - NetBox Documentation](https://netbox.readthedocs.io/en/stable/plugins/)
 
 Install NetBox Webhook Receiver:
```

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/serializers.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/api/views.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/filtersets.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/forms.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,22 +9,29 @@
 
 
 class WebhookReceiverForm(NetBoxModelForm):
     comments = CommentField()
 
     fieldsets = (
         FieldSet(
-                "name",
-                "receiver_group",
-                "description",
-                "uuid",
-                "store_payload",
-                name="Webhook definition"
-            ),
-        FieldSet("auth_method", "auth_header", "secret_key", "token", "hash_algorithm", name="Authentication"),
+            "name",
+            "receiver_group",
+            "description",
+            "uuid",
+            "store_payload",
+            name="Webhook definition",
+        ),
+        FieldSet(
+            "auth_method",
+            "auth_header",
+            "secret_key",
+            "token",
+            "hash_algorithm",
+            name="Authentication",
+        ),
         FieldSet("datasource", name="Trigger action"),
         FieldSet("tags", name="Extra"),
     )
 
     # Thanks to Dillon Henschen for his netbox pull #12675
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/migrations/0001_initial.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/models.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/models.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/navigation.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/tables.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceiver.html`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,19 @@
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Webhook Receiver URL</h5>
         <table class="table">
           <tr>
-            <td>{{request.headers.referer | split:"/" | slice:"5" | join:"/" }}/webhooks/{{ object.uuid}}/</td>
+            <td id="webhook_endpoint">{{request.headers.referer | split:"/" | slice:"5" | join:"/" }}/webhooks/{{ object.uuid}}/</td>
+            <td>
+              <div class="float-end">
+              {% copy_content "webhook_endpoint" %}
+              </div>
+            </td>
           </tr>
         </table>
       </div>
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -13,10 +13,11 @@
 {% include 'inc/panels/custom_fields.html' %}
 **** WWeebbhhooookk aaccttiioonnss ****
 SSttoorree ppaayyllooaadd     {{ object.store_payload|placeholder }}
 UUppddaattee ddaattaassoouurrccee _{_{_ _o_b_j_e_c_t_._d_a_t_a_s_o_u_r_c_e_|_p_l_a_c_e_h_o_l_d_e_r_ _}_}
 RRuunn CCuussttoomm SSccrriipptt {{ object.customscript|placeholder }}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 **** WWeebbhhooookk RReecceeiivveerr UURRLL ****
-{{request.headers.referer | split:"/" | slice:"5" | join:"/" }}/webhooks/{
+{{request.headers.referer | split:"/" |
+slice:"5" | join:"/" }}/webhooks/{      {% copy_content "webhook_endpoint" %}
 { object.uuid}}/
 {% endblock content %}
```

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/templates/netbox_webhook_receiver/webhookreceivergroup.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/urls.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/views.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/views/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import datetime as dt
 import json
 import logging
 
-from django.contrib.auth.models import User
 from django.db.transaction import atomic, non_atomic_requests
 from django.http import (
     HttpResponse,
     HttpResponseForbidden,
     HttpResponseNotFound,
 )
 from django.utils import timezone
 from django.views.decorators.csrf import csrf_exempt
 from django.views.decorators.http import require_POST
 from netbox_webhook_receiver.models import WebhookMessage, WebhookReceiver
 from secrets import compare_digest
+from users.models import User
 
 logger = logging.getLogger(__name__)
 
 
 @csrf_exempt
 @require_POST
 @non_atomic_requests
```

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceiver.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/views/webhookreceiver.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/netbox_webhook_receiver/views/webhookreceivergroup.py` & `netbox_plugin_webhook_receiver-0.4.1/netbox_webhook_receiver/views/webhookreceivergroup.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_webhook_receiver-0.4.0/pyproject.toml` & `netbox_plugin_webhook_receiver-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netbox-plugin-webhook-receiver"
-version = "0.4.0"
+version = "0.4.1"
 description = "NetBox Webhook is a plugin for managing webhook receivers in NetBox."
 authors = ["Łukasz Polański <wookasz@gmail.com>"]
 homepage = "https://github.com/LuPo/netbox-plugin-webhook-receiver"
 repository = "https://github.com/LuPo/netbox-plugin-webhook-receiver"
 license = "MIT"
 readme = "README.md"
 packages = [{include = "netbox_webhook_receiver"}]
```

### Comparing `netbox_plugin_webhook_receiver-0.4.0/PKG-INFO` & `netbox_plugin_webhook_receiver-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-webhook-receiver
-Version: 0.4.0
+Version: 0.4.1
 Summary: NetBox Webhook is a plugin for managing webhook receivers in NetBox.
 Home-page: https://github.com/LuPo/netbox-plugin-webhook-receiver
 License: MIT
 Keywords: netbox,netbox-plugin,webhook
 Author: Łukasz Polański
 Author-email: wookasz@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -31,15 +31,15 @@
 - [x] Custom actions execution on successfully receving authenticated webhook message. Currently only one action available: Synchronize Netbox git 'Data Source'
 - [x] Use of standard Netbox jobs to queue webhook actions in the workers.
 - [ ] Additional actions to be implemented
 - [ ] Plugin configuration parameters
 
 ## Requirements
 
-* NetBox 3.5 or higher
+* NetBox 4.0 or higher
 * Python 3.10 or higher
 
 ## Installation & Configuration
 
 For general knowledge about netbox plugin installation please refer to the official guide: [Using Plugins - NetBox Documentation](https://netbox.readthedocs.io/en/stable/plugins/)
 
 Install NetBox Webhook Receiver:
```

