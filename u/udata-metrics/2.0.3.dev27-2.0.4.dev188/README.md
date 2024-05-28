# Comparing `tmp/udata_metrics-2.0.3.dev27-py2.py3-none-any.whl.zip` & `tmp/udata_metrics-2.0.4.dev188-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,20 @@
-Zip file size: 3486 bytes, number of entries: 9
--rw-r--r--  2.0 unx      248 b- defN 20-Apr-15 14:10 udata_metrics/__init__.py
--rw-r--r--  2.0 unx     2140 b- defN 20-Apr-15 14:10 udata_metrics/client.py
--rw-r--r--  2.0 unx        0 b- defN 20-Apr-15 14:10 udata_metrics/models.py
--rw-r--r--  2.0 unx      551 b- defN 20-Apr-15 14:10 udata_metrics/tasks.py
--rw-r--r--  2.0 unx     1430 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/WHEEL
--rw-r--r--  2.0 unx      133 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      771 b- defN 20-Apr-15 14:11 udata_metrics-2.0.3.dev27.dist-info/RECORD
-9 files, 5397 bytes uncompressed, 2138 bytes compressed:  60.4%
+Zip file size: 14807 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      248 b- defN 24-May-28 09:41 udata_metrics/__init__.py
+-rw-r--r--  2.0 unx     4355 b- defN 24-May-28 09:41 udata_metrics/metrics.py
+-rw-r--r--  2.0 unx       87 b- defN 24-May-28 09:41 udata_metrics/settings.py
+-rw-r--r--  2.0 unx     3852 b- defN 24-May-28 09:41 udata_metrics/tasks.py
+-rw-r--r--  2.0 unx     5794 b- defN 24-May-28 09:41 udata_metrics/views.py
+-rw-r--r--  2.0 unx     1204 b- defN 24-May-28 09:41 udata_metrics/templates/dataset-metrics.html
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-28 09:41 udata_metrics/templates/organization-metrics.html
+-rw-r--r--  2.0 unx      938 b- defN 24-May-28 09:41 udata_metrics/templates/reuse-metrics.html
+-rw-r--r--  2.0 unx     2161 b- defN 24-May-28 09:41 udata_metrics/templates/site-metrics.html
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-28 09:41 udata_metrics/templates/macros/metrics.html
+-rw-r--r--  2.0 unx     3218 b- defN 24-May-28 09:41 udata_metrics/translations/udata_metrics.pot
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-28 09:42 udata_metrics/translations/fr/LC_MESSAGES/udata_metrics.mo
+-rw-r--r--  2.0 unx     3697 b- defN 24-May-28 09:41 udata_metrics/translations/fr/LC_MESSAGES/udata_metrics.po
+-rw-r--r--  2.0 unx     3397 b- defN 24-May-28 09:42 udata_metrics-2.0.4.dev188.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-28 09:42 udata_metrics-2.0.4.dev188.dist-info/WHEEL
+-rw-r--r--  2.0 unx       89 b- defN 24-May-28 09:42 udata_metrics-2.0.4.dev188.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-May-28 09:42 udata_metrics-2.0.4.dev188.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1693 b- defN 24-May-28 09:42 udata_metrics-2.0.4.dev188.dist-info/RECORD
+18 files, 35822 bytes uncompressed, 11957 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -1,28 +1,55 @@
 Filename: udata_metrics/__init__.py
 Comment: 
 
-Filename: udata_metrics/client.py
+Filename: udata_metrics/metrics.py
 Comment: 
 
-Filename: udata_metrics/models.py
+Filename: udata_metrics/settings.py
 Comment: 
 
 Filename: udata_metrics/tasks.py
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev27.dist-info/METADATA
+Filename: udata_metrics/views.py
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev27.dist-info/WHEEL
+Filename: udata_metrics/templates/dataset-metrics.html
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev27.dist-info/entry_points.txt
+Filename: udata_metrics/templates/organization-metrics.html
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev27.dist-info/top_level.txt
+Filename: udata_metrics/templates/reuse-metrics.html
 Comment: 
 
-Filename: udata_metrics-2.0.3.dev27.dist-info/RECORD
+Filename: udata_metrics/templates/site-metrics.html
+Comment: 
+
+Filename: udata_metrics/templates/macros/metrics.html
+Comment: 
+
+Filename: udata_metrics/translations/udata_metrics.pot
+Comment: 
+
+Filename: udata_metrics/translations/fr/LC_MESSAGES/udata_metrics.mo
+Comment: 
+
+Filename: udata_metrics/translations/fr/LC_MESSAGES/udata_metrics.po
+Comment: 
+
+Filename: udata_metrics-2.0.4.dev188.dist-info/METADATA
+Comment: 
+
+Filename: udata_metrics-2.0.4.dev188.dist-info/WHEEL
+Comment: 
+
+Filename: udata_metrics-2.0.4.dev188.dist-info/entry_points.txt
+Comment: 
+
+Filename: udata_metrics-2.0.4.dev188.dist-info/top_level.txt
+Comment: 
+
+Filename: udata_metrics-2.0.4.dev188.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## udata_metrics/__init__.py

```diff
@@ -1,14 +1,14 @@
 '''
 udata-metrics
 
 Connexion handler to metrics service for udata
 '''
 
 
-__version__ = '0.1.1.dev'
+__version__ = '2.0.4.dev'
 __description__ = 'Connexion handler to metrics service for udata'
 
 
 def init_app(app):
     # Do whatever you want to initialize your plugin
     pass
```

## udata_metrics/tasks.py

```diff
@@ -1,22 +1,125 @@
 import logging
+from typing import Dict, List
+import requests
+from functools import wraps
+import time
 
-from udata_metrics.client import InfluxClient
-from udata.models import Dataset
-from udata.tasks import job, task
-from udata.core.metrics.signals import on_site_metrics_computed
+from flask import current_app
 
-from udata_metrics.client import metrics_client_factory
-
-log = logging.getLogger(__name__)
+from udata.models import db, CommunityResource, Dataset, Reuse, Organization
+from udata.tasks import job
 
 
-@on_site_metrics_computed.connect
-def site_metrics_send(document, **kwargs):
-    write_object_metrics.delay(document)
+log = logging.getLogger(__name__)
 
 
-@task
-def write_object_metrics(document):
-    client = metrics_client_factory()
-    metrics = document.get_metrics()
-    client.insert(metrics)
+def log_timing(func):
+    @wraps(func)
+    def timeit_wrapper(*args, **kwargs):
+        # Better log if we're using Python 3.9
+        name = func.__name__
+        model = name.removeprefix('update_') if hasattr(name, 'removeprefix') else name
+
+        log.info(f"Processing {model}…")
+        start_time = time.perf_counter()
+        result = func(*args, **kwargs)
+        total_time = time.perf_counter() - start_time
+        log.info(f'Done in {total_time:.4f} seconds.')
+        return result
+    return timeit_wrapper
+
+
+def save_model(model: db.Document, model_id: str, metrics: Dict[str, int]) -> None:
+    try:
+        result = model.objects(id=model_id).update(**{
+            f'set__metrics__{key}': value for key, value in metrics.items()
+        })
+
+        if result is None:
+            log.debug(f'{model.__name__} not found', extra={
+                'id': model_id
+            })
+    except Exception as e:
+        log.exception(e)
+
+
+def iterate_on_metrics(target: str, value_keys: List[str], page_size: int = 50) -> dict:
+    '''
+    Yield all elements with not zero values for the keys inside `value_keys`.
+    If you pass ['visit', 'download_resource'], it will do a `OR` and get
+    metrics with one of the two values not zero.
+    '''
+    yielded = set()
+
+    for value_key in value_keys:
+        url = f'{current_app.config["METRICS_API"]}/{target}_total/data/'
+        url += f'?{value_key}__greater=1&page_size={page_size}'
+
+        with requests.Session() as session:
+            while url is not None:
+                r = session.get(url, timeout=10)
+                r.raise_for_status()
+                data = r.json()
+
+                for row in data['data']:
+                    if row['__id'] not in yielded:
+                        yielded.add(row['__id'])
+                        yield row
+
+                url = data['links'].get('next')
+
+
+@log_timing
+def update_resources_and_community_resources():
+    for data in iterate_on_metrics("resources", ["download_resource"]):
+        if data['dataset_id'] is None:
+            save_model(CommunityResource, data['resource_id'], {
+                'views': data['download_resource'],
+            })
+        else:
+            Dataset.objects(resources__id=data['resource_id']).update(
+                **{f'set__resources__$__metrics__views': data['download_resource']}
+            )
+
+
+@log_timing
+def update_datasets():
+    for data in iterate_on_metrics("datasets", ["visit", "download_resource"]):
+        save_model(Dataset, data['dataset_id'], {
+            'views': data['visit'],
+            'resources_downloads': data['download_resource'],
+        })
+
+
+@log_timing
+def update_reuses():
+    for data in iterate_on_metrics("reuses", ["visit"]):
+        save_model(Reuse, data['reuse_id'], {
+            'views': data['visit']
+        })
+
+
+@log_timing
+def update_organizations():
+    # We're currently using visit_dataset as global metric for an orga
+    for data in iterate_on_metrics("organizations", ["visit_dataset"]):
+        save_model(Organization, data['organization_id'], {
+            'views': data['visit_dataset'],
+        })
+
+
+def update_metrics_for_models():
+    log.info(f"Starting…")
+    update_datasets()
+    update_resources_and_community_resources()
+    update_reuses()
+    update_organizations()
+
+
+@job('update-metrics', route='low.metrics')
+def update_metrics(self):
+    '''Update udata objects metrics'''
+    if not current_app.config['METRICS_API']:
+        log.error('You need to set METRICS_API to run update-metrics')
+        exit(1)
+    update_metrics_for_models()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

