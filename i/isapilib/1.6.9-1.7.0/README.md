# Comparing `tmp/isapilib-1.6.9.tar.gz` & `tmp/isapilib-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isapilib-1.6.9.tar", last modified: Mon Apr  1 16:21:37 2024, max compression
+gzip compressed data, was "isapilib-1.7.0.tar", last modified: Tue May 28 21:26:12 2024, max compression
```

## Comparing `isapilib-1.6.9.tar` & `isapilib-1.7.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.840210 isapilib-1.6.9/
--rw-rw-rw-   0        0        0       67 2024-02-19 22:40:27.000000 isapilib-1.6.9/MANIFEST.in
--rw-rw-rw-   0        0        0      209 2024-04-01 16:21:37.838146 isapilib-1.6.9/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-10-30 17:02:35.000000 isapilib-1.6.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.786300 isapilib-1.6.9/app/
--rw-rw-rw-   0        0        0        0 2024-01-19 19:11:10.000000 isapilib-1.6.9/app/__init__.py
--rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.6.9/app/asgi.py
--rw-rw-rw-   0        0        0     3416 2024-01-19 19:13:38.000000 isapilib-1.6.9/app/settings.py
--rw-rw-rw-   0        0        0      781 2024-02-19 17:24:37.000000 isapilib-1.6.9/app/urls.py
--rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.6.9/app/wsgi.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.805418 isapilib-1.6.9/isapilib/
--rw-rw-rw-   0        0        0     3364 2024-02-20 15:50:12.000000 isapilib-1.6.9/isapilib/Connection.py
--rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.9/isapilib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.816019 isapilib-1.6.9/isapilib/api/
--rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.9/isapilib/api/__init__.py
--rw-rw-rw-   0        0        0    32245 2024-03-27 20:02:07.000000 isapilib-1.6.9/isapilib/api/models.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.819674 isapilib-1.6.9/isapilib/core/
--rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.9/isapilib/core/__init__.py
--rw-rw-rw-   0        0        0     2047 2024-04-01 14:35:05.000000 isapilib-1.6.9/isapilib/core/models.py
--rw-rw-rw-   0        0        0     1404 2024-03-21 18:17:56.000000 isapilib-1.6.9/isapilib/decorators.py
--rw-rw-rw-   0        0        0      378 2024-03-12 17:04:53.000000 isapilib-1.6.9/isapilib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.821189 isapilib-1.6.9/isapilib/management/
--rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.9/isapilib/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.825924 isapilib-1.6.9/isapilib/management/commands/
--rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.6.9/isapilib/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1167 2024-03-07 23:41:08.000000 isapilib-1.6.9/isapilib/management/commands/check_branch.py
--rw-rw-rw-   0        0        0     1360 2024-03-07 23:25:53.000000 isapilib-1.6.9/isapilib/management/commands/external_migrate.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.829935 isapilib-1.6.9/isapilib/migrations/
--rw-rw-rw-   0        0        0    46380 2024-02-19 17:39:52.000000 isapilib-1.6.9/isapilib/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.6.9/isapilib/migrations/__init__.py
--rw-rw-rw-   0        0        0     8155 2024-02-20 18:28:12.000000 isapilib-1.6.9/isapilib/models.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.774554 isapilib-1.6.9/isapilib/static/
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.831538 isapilib-1.6.9/isapilib/static/css/
--rw-rw-rw-   0        0        0   232948 2024-02-19 22:23:07.000000 isapilib-1.6.9/isapilib/static/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.833460 isapilib-1.6.9/isapilib/static/img/
--rw-rw-rw-   0        0        0     1638 2024-02-19 17:54:17.000000 isapilib-1.6.9/isapilib/static/img/intelisis128.png
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.834514 isapilib-1.6.9/isapilib/templates/
--rw-rw-rw-   0        0        0     1836 2024-02-20 00:24:37.000000 isapilib-1.6.9/isapilib/templates/index.html
--rw-rw-rw-   0        0        0      124 2024-02-19 23:15:50.000000 isapilib-1.6.9/isapilib/urls.py
--rw-rw-rw-   0        0        0     3873 2024-03-21 18:17:56.000000 isapilib-1.6.9/isapilib/utilities.py
--rw-rw-rw-   0        0        0     1414 2024-03-25 16:51:47.000000 isapilib-1.6.9/isapilib/views.py
-drwxrwxrwx   0        0        0        0 2024-04-01 16:21:37.837051 isapilib-1.6.9/isapilib.egg-info/
--rw-rw-rw-   0        0        0      209 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-01 16:21:37.000000 isapilib-1.6.9/isapilib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-01 16:21:37.840210 isapilib-1.6.9/setup.cfg
--rw-rw-rw-   0        0        0      435 2024-04-01 16:21:36.000000 isapilib-1.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:12.009469 isapilib-1.7.0/
+-rw-rw-rw-   0        0        0       67 2024-02-19 22:40:27.000000 isapilib-1.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      209 2024-05-28 21:26:12.007290 isapilib-1.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-10-30 17:02:35.000000 isapilib-1.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.957956 isapilib-1.7.0/app/
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:11:10.000000 isapilib-1.7.0/app/__init__.py
+-rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.7.0/app/asgi.py
+-rw-rw-rw-   0        0        0     3416 2024-01-19 19:13:38.000000 isapilib-1.7.0/app/settings.py
+-rw-rw-rw-   0        0        0      781 2024-02-19 17:24:37.000000 isapilib-1.7.0/app/urls.py
+-rw-rw-rw-   0        0        0      399 2024-01-19 19:11:10.000000 isapilib-1.7.0/app/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.972447 isapilib-1.7.0/isapilib/
+-rw-rw-rw-   0        0        0     3364 2024-02-20 15:50:12.000000 isapilib-1.7.0/isapilib/Connection.py
+-rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.7.0/isapilib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.984520 isapilib-1.7.0/isapilib/api/
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.7.0/isapilib/api/__init__.py
+-rw-rw-rw-   0        0        0    32311 2024-05-28 21:01:41.000000 isapilib-1.7.0/isapilib/api/models.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.986960 isapilib-1.7.0/isapilib/core/
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.7.0/isapilib/core/__init__.py
+-rw-rw-rw-   0        0        0     2047 2024-04-01 14:35:05.000000 isapilib-1.7.0/isapilib/core/models.py
+-rw-rw-rw-   0        0        0     1404 2024-03-21 18:17:56.000000 isapilib-1.7.0/isapilib/decorators.py
+-rw-rw-rw-   0        0        0      378 2024-03-12 17:04:53.000000 isapilib-1.7.0/isapilib/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.987972 isapilib-1.7.0/isapilib/management/
+-rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.7.0/isapilib/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.992823 isapilib-1.7.0/isapilib/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-10-30 17:02:35.000000 isapilib-1.7.0/isapilib/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1167 2024-03-07 23:41:08.000000 isapilib-1.7.0/isapilib/management/commands/check_branch.py
+-rw-rw-rw-   0        0        0     1360 2024-03-07 23:25:53.000000 isapilib-1.7.0/isapilib/management/commands/external_migrate.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.997269 isapilib-1.7.0/isapilib/migrations/
+-rw-rw-rw-   0        0        0    46380 2024-02-19 17:39:52.000000 isapilib-1.7.0/isapilib/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-01-19 19:12:02.000000 isapilib-1.7.0/isapilib/migrations/__init__.py
+-rw-rw-rw-   0        0        0     8155 2024-02-20 18:28:12.000000 isapilib-1.7.0/isapilib/models.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.942832 isapilib-1.7.0/isapilib/static/
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:11.998271 isapilib-1.7.0/isapilib/static/css/
+-rw-rw-rw-   0        0        0   232948 2024-02-19 22:23:07.000000 isapilib-1.7.0/isapilib/static/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:12.001379 isapilib-1.7.0/isapilib/static/img/
+-rw-rw-rw-   0        0        0     1638 2024-02-19 17:54:17.000000 isapilib-1.7.0/isapilib/static/img/intelisis128.png
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:12.003443 isapilib-1.7.0/isapilib/templates/
+-rw-rw-rw-   0        0        0     1836 2024-02-20 00:24:37.000000 isapilib-1.7.0/isapilib/templates/index.html
+-rw-rw-rw-   0        0        0      124 2024-02-19 23:15:50.000000 isapilib-1.7.0/isapilib/urls.py
+-rw-rw-rw-   0        0        0     4179 2024-05-28 21:02:15.000000 isapilib-1.7.0/isapilib/utilities.py
+-rw-rw-rw-   0        0        0     1414 2024-03-25 16:51:47.000000 isapilib-1.7.0/isapilib/views.py
+drwxrwxrwx   0        0        0        0 2024-05-28 21:26:12.005868 isapilib-1.7.0/isapilib.egg-info/
+-rw-rw-rw-   0        0        0      209 2024-05-28 21:26:11.000000 isapilib-1.7.0/isapilib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2024-05-28 21:26:11.000000 isapilib-1.7.0/isapilib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 21:26:11.000000 isapilib-1.7.0/isapilib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-05-28 21:26:11.000000 isapilib-1.7.0/isapilib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-28 21:26:11.000000 isapilib-1.7.0/isapilib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 21:26:12.009469 isapilib-1.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      435 2024-05-28 21:25:57.000000 isapilib-1.7.0/setup.py
```

### Comparing `isapilib-1.6.9/app/settings.py` & `isapilib-1.7.0/app/settings.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/app/urls.py` & `isapilib-1.7.0/app/urls.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/Connection.py` & `isapilib-1.7.0/isapilib/Connection.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/api/models.py` & `isapilib-1.7.0/isapilib/api/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,106 @@
 from django.db import models
 
 from isapilib.core.models import BaseModel
-from isapilib.utilities import execute_sp
+
+
+class Art(BaseModel):
+    articulo = models.CharField(db_column='Articulo', primary_key=True, max_length=20)
+    descripcion1 = models.CharField(db_column='Descripcion1', max_length=100, blank=True, null=True)
+    descripcion2 = models.CharField(db_column='Descripcion2', max_length=255, blank=True, null=True)
+    grupo = models.CharField(db_column='Grupo', max_length=50, blank=True, null=True)
+    categoria = models.CharField(db_column='Categoria', max_length=50, blank=True, null=True)
+    impuesto1 = models.FloatField(db_column='Impuesto1')
+    impuesto2 = models.FloatField(db_column='Impuesto2', blank=True, null=True)
+    impuesto3 = models.FloatField(db_column='Impuesto3', blank=True, null=True)
+    tipo = models.CharField(db_column='Tipo', max_length=20)
+    precio_lista = models.DecimalField(db_column='PrecioLista', max_digits=19, decimal_places=4, blank=True, null=True)
+    estatus = models.CharField(db_column='Estatus', max_length=15)
+    usuario = models.CharField(db_column='Usuario', max_length=10, blank=True, null=True)
+    precio2 = models.DecimalField(db_column='Precio2', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio3 = models.DecimalField(db_column='Precio3', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio4 = models.DecimalField(db_column='Precio4', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio5 = models.DecimalField(db_column='Precio5', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio6 = models.DecimalField(db_column='Precio6', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio7 = models.DecimalField(db_column='Precio7', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio8 = models.DecimalField(db_column='Precio8', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio9 = models.DecimalField(db_column='Precio9', max_digits=19, decimal_places=4, blank=True, null=True)
+    precio10 = models.DecimalField(db_column='Precio10', max_digits=19, decimal_places=4, blank=True, null=True)
+    situacion = models.CharField(db_column='Situacion', max_length=50, blank=True, null=True)
+    tipo_compra = models.CharField(db_column='TipoCompra', max_length=20, blank=True, null=True)
+    retencion1 = models.FloatField(db_column='Retencion1', blank=True, null=True)
+    retencion2 = models.FloatField(db_column='Retencion2', blank=True, null=True)
+    retencion3 = models.FloatField(db_column='Retencion3', blank=True, null=True)
+    modelo = models.CharField(db_column='Modelo', max_length=4, blank=True, null=True)
+    direccion = models.CharField(db_column='Direccion', max_length=100, blank=True, null=True)
+    direccion_numero = models.CharField(db_column='DireccionNumero', max_length=20, blank=True, null=True)
+    direccion_numero_int = models.CharField(db_column='DireccionNumeroInt', max_length=20, blank=True, null=True)
+    observaciones = models.CharField(db_column='Observaciones', max_length=100, blank=True, null=True)
+    colonia = models.CharField(db_column='Colonia', max_length=100, blank=True, null=True)
+    delegacion = models.CharField(db_column='Delegacion', max_length=100, blank=True, null=True)
+    poblacion = models.CharField(db_column='Poblacion', max_length=100, blank=True, null=True)
+    estado = models.CharField(db_column='Estado', max_length=30, blank=True, null=True)
+    pais = models.CharField(db_column='Pais', max_length=30, blank=True, null=True)
+    codigo_postal = models.CharField(db_column='CodigoPostal', max_length=15, blank=True, null=True)
+    tipo_impuesto1 = models.CharField(db_column='TipoImpuesto1', max_length=10, blank=True, null=True)
+    tipo_impuesto2 = models.CharField(db_column='TipoImpuesto2', max_length=10, blank=True, null=True)
+    tipo_impuesto3 = models.CharField(db_column='TipoImpuesto3', max_length=10, blank=True, null=True)
+
+    class Meta:
+        db_table = 'Art'
+        managed = False
+
+
+class VentaD(BaseModel):
+    id_venta = models.IntegerField(db_column='ID')
+    renglon = models.FloatField(db_column='Renglon')
+    renglon_sub = models.IntegerField(db_column='RenglonSub')
+    renglon_id = models.IntegerField(db_column='RenglonID', blank=True, null=True)
+    renglon_tipo = models.CharField(db_column='RenglonTipo', max_length=1, blank=True, null=True)
+    cantidad = models.FloatField(db_column='Cantidad', blank=True, null=True)
+    almacen = models.CharField(db_column='Almacen', max_length=10, blank=True, null=True)
+    articulo = models.CharField(db_column='Articulo', max_length=20)
+    precio = models.FloatField(db_column='Precio', blank=True, null=True)
+    precio_sugerido = models.FloatField(db_column='PrecioSugerido', blank=True, null=True)
+    impuesto1 = models.FloatField(db_column='Impuesto1', blank=True, null=True)
+    impuesto2 = models.FloatField(db_column='Impuesto2', blank=True, null=True)
+    impuesto3 = models.FloatField(db_column='Impuesto3', blank=True, null=True)
+    descripcion_extra = models.CharField(db_column='DescripcionExtra', max_length=100, blank=True, null=True)
+    costo = models.DecimalField(db_column='Costo', max_digits=19, decimal_places=4, blank=True, null=True)
+    aplica = models.CharField(db_column='Aplica', max_length=20, blank=True, null=True)
+    aplica_id = models.CharField(db_column='AplicaID', max_length=20, blank=True, null=True)
+    unidad = models.CharField(db_column='Unidad', max_length=50, blank=True, null=True)
+    fecha_requerida = models.DateTimeField(db_column='FechaRequerida', blank=True, null=True)
+    hora_requerida = models.CharField(db_column='HoraRequerida', max_length=5, blank=True, null=True)
+    agente = models.CharField(db_column='Agente', max_length=10, blank=True, null=True)
+    departamento = models.IntegerField(db_column='Departamento', blank=True, null=True)
+    sucursal = models.IntegerField(db_column='Sucursal')
+    sucursal_origen = models.IntegerField(db_column='SucursalOrigen', blank=True, null=True)
+    uen = models.IntegerField(db_column='UEN', blank=True, null=True)
+    precio_lista = models.DecimalField(db_column='PrecioLista', max_digits=19, decimal_places=4, blank=True, null=True)
+    tipo_impuesto1 = models.CharField(db_column='TipoImpuesto1', max_length=10, blank=True, null=True)
+    tipo_impuesto2 = models.CharField(db_column='TipoImpuesto2', max_length=10, blank=True, null=True)
+    tipo_impuesto3 = models.CharField(db_column='TipoImpuesto3', max_length=10, blank=True, null=True)
+    retencion1 = models.FloatField(db_column='Retencion1', blank=True, null=True)
+    retencion2 = models.FloatField(db_column='Retencion2', blank=True, null=True)
+    retencion3 = models.FloatField(db_column='Retencion3', blank=True, null=True)
+    tipo_retencion1 = models.CharField(db_column='TipoRetencion1', max_length=10, blank=True, null=True)
+    tipo_retencion2 = models.CharField(db_column='TipoRetencion2', max_length=10, blank=True, null=True)
+    tipo_retencion3 = models.CharField(db_column='TipoRetencion3', max_length=10, blank=True, null=True)
+    comentarios = models.CharField(db_column='Comentarios', max_length=250, blank=True, null=True)
+    servicio_tipo_orden = models.CharField(db_column='ServicioTipoOrden', max_length=20, blank=True, null=True)
+    articulo_actual = models.CharField(db_column='ArticuloActual', max_length=20, blank=True, null=True)
+    ut = models.FloatField(db_column='UT', blank=True, null=True)
+    cc_tiempo_tab = models.FloatField(db_column='CCTiempoTab', blank=True, null=True)
+    paquete = models.IntegerField(db_column='Paquete')
+
+    class Meta:
+        db_table = 'VentaD'
+        managed = False
+        unique_together = (('id', 'renglon', 'renglon_sub'),)
 
 
 class Venta(BaseModel):
     id = models.AutoField(db_column='ID', primary_key=True)
     empresa = models.CharField(db_column='Empresa', max_length=5)
     mov = models.CharField(db_column='Mov', max_length=20)
     mov_id = models.CharField(db_column='MovID', max_length=20, blank=True, null=True)
@@ -63,84 +158,35 @@
     fecha_entrega = models.DateTimeField(db_column='FechaEntrega', blank=True, null=True)
     hora_recepcion = models.CharField(db_column='HoraRecepcion', max_length=5, blank=True, null=True)
 
     class Meta:
         db_table = 'Venta'
         managed = False
 
-    def afectar(self, **kwargs):
-        db_name = kwargs.get('using', 'default')
-
-        params = dict(
-            ID=self.id,
-            Modulo=kwargs.get('modulo', 'VTAS'),
-            Accion=kwargs.get('accion', 'AFECTAR'),
-            Base=kwargs.get('base', 'Todo'),
-            GenerarMov=kwargs.get('generarmov', False),
-            Usuario=kwargs.get('usuario', 'SOPDESA'),
-            SincroFinal=kwargs.get('sincrofinal', False),
-            EnSilencio=kwargs.get('ensilencio', 0),
-            FechaRegistro=kwargs.get('fecharegistro', False),
-            Conexion=kwargs.get('conexion', False),
-            Estacion=kwargs.get('estacion', 1000),
-            FueraLinea=kwargs.get('fueralinea', False)
-        )
-        params = {key: value for key, value in params.items() if value}
-        result = execute_sp('spAfectar', params, using=db_name)
-        self.refresh_from_db()
-        return result
-
-
-class VentaD(BaseModel):
-    id_venta = models.IntegerField(db_column='ID')
-    renglon = models.FloatField(db_column='Renglon')
-    renglon_sub = models.IntegerField(db_column='RenglonSub')
-    renglon_id = models.IntegerField(db_column='RenglonID', blank=True, null=True)
-    renglon_tipo = models.CharField(db_column='RenglonTipo', max_length=1, blank=True, null=True)
-    cantidad = models.FloatField(db_column='Cantidad', blank=True, null=True)
-    almacen = models.CharField(db_column='Almacen', max_length=10, blank=True, null=True)
-    articulo = models.CharField(db_column='Articulo', max_length=20)
-    precio = models.FloatField(db_column='Precio', blank=True, null=True)
-    precio_sugerido = models.FloatField(db_column='PrecioSugerido', blank=True, null=True)
-    impuesto1 = models.FloatField(db_column='Impuesto1', blank=True, null=True)
-    impuesto2 = models.FloatField(db_column='Impuesto2', blank=True, null=True)
-    impuesto3 = models.FloatField(db_column='Impuesto3', blank=True, null=True)
-    descripcion_extra = models.CharField(db_column='DescripcionExtra', max_length=100, blank=True, null=True)
-    costo = models.DecimalField(db_column='Costo', max_digits=19, decimal_places=4, blank=True, null=True)
-    aplica = models.CharField(db_column='Aplica', max_length=20, blank=True, null=True)
-    aplica_id = models.CharField(db_column='AplicaID', max_length=20, blank=True, null=True)
-    unidad = models.CharField(db_column='Unidad', max_length=50, blank=True, null=True)
-    fecha_requerida = models.DateTimeField(db_column='FechaRequerida', blank=True, null=True)
-    hora_requerida = models.CharField(db_column='HoraRequerida', max_length=5, blank=True, null=True)
-    agente = models.CharField(db_column='Agente', max_length=10, blank=True, null=True)
-    departamento = models.IntegerField(db_column='Departamento', blank=True, null=True)
-    sucursal = models.IntegerField(db_column='Sucursal')
-    sucursal_origen = models.IntegerField(db_column='SucursalOrigen', blank=True, null=True)
-    uen = models.IntegerField(db_column='UEN', blank=True, null=True)
-    precio_lista = models.DecimalField(db_column='PrecioLista', max_digits=19, decimal_places=4, blank=True, null=True)
-    tipo_impuesto1 = models.CharField(db_column='TipoImpuesto1', max_length=10, blank=True, null=True)
-    tipo_impuesto2 = models.CharField(db_column='TipoImpuesto2', max_length=10, blank=True, null=True)
-    tipo_impuesto3 = models.CharField(db_column='TipoImpuesto3', max_length=10, blank=True, null=True)
-    retencion1 = models.FloatField(db_column='Retencion1', blank=True, null=True)
-    retencion2 = models.FloatField(db_column='Retencion2', blank=True, null=True)
-    retencion3 = models.FloatField(db_column='Retencion3', blank=True, null=True)
-    tipo_retencion1 = models.CharField(db_column='TipoRetencion1', max_length=10, blank=True, null=True)
-    tipo_retencion2 = models.CharField(db_column='TipoRetencion2', max_length=10, blank=True, null=True)
-    tipo_retencion3 = models.CharField(db_column='TipoRetencion3', max_length=10, blank=True, null=True)
-    comentarios = models.CharField(db_column='Comentarios', max_length=250, blank=True, null=True)
-    servicio_tipo_orden = models.CharField(db_column='ServicioTipoOrden', max_length=20, blank=True, null=True)
-    articulo_actual = models.CharField(db_column='ArticuloActual', max_length=20, blank=True, null=True)
-    ut = models.FloatField(db_column='UT', blank=True, null=True)
-    cc_tiempo_tab = models.FloatField(db_column='CCTiempoTab', blank=True, null=True)
-    paquete = models.IntegerField(db_column='Paquete')
-
-    class Meta:
-        db_table = 'VentaD'
-        managed = False
-        unique_together = (('id', 'renglon', 'renglon_sub'),)
+    def create_ventad(self, art: Art, i: int) -> VentaD:
+        service_detail = VentaD()
+        service_detail.id_venta = self.id
+        service_detail.renglon_sub = 0
+        service_detail.renglon_tipo = 'N'
+        service_detail.almacen = self.almacen
+        service_detail.uen = self.uen
+        service_detail.sucursal = self.sucursal
+        service_detail.sucursal_origen = self.sucursal
+        service_detail.agente = self.agente
+        service_detail.hora_requerida = self.hora_requerida
+        service_detail.renglon = 2048 * i
+        service_detail.renglon_id = i
+        service_detail.articulo = art.articulo
+        service_detail.impuesto1 = art.impuesto1
+        service_detail.descripcion_extra = art.descripcion1
+        service_detail.comentarios = art.descripcion1
+        service_detail.precio = 0
+        service_detail.ut = 1
+        service_detail.cc_tiempo_tab = 1
+        return service_detail
 
 
 class Vin(BaseModel):
     vin = models.CharField(db_column='VIN', primary_key=True, max_length=20)
     articulo = models.CharField(db_column='Articulo', max_length=20, blank=True, null=True)
     km = models.IntegerField(db_column='Km', blank=True, null=True)
     motor = models.CharField(db_column='Motor', max_length=20, blank=True, null=True)
@@ -326,67 +372,21 @@
     poblacion = models.CharField(db_column='Poblacion', max_length=30, blank=True, null=True)
     estado = models.CharField(db_column='Estado', max_length=30, blank=True, null=True)
     pais = models.CharField(db_column='Pais', max_length=30, blank=True, null=True)
     codigo_postal = models.CharField(db_column='CodigoPostal', max_length=15, blank=True, null=True)
     rfc = models.CharField(db_column='RFC', max_length=20, blank=True, null=True)
     curp = models.CharField(db_column='CURP', max_length=30, blank=True, null=True)
     email = models.CharField(db_column='eMail', max_length=50, blank=True, null=True)
+    id_planta = models.CharField(db_column='IdPlanta', max_length=10, blank=True, null=True)
 
     class Meta:
         db_table = 'Agente'
         managed = False
 
 
-class Art(BaseModel):
-    articulo = models.CharField(db_column='Articulo', primary_key=True, max_length=20)
-    descripcion1 = models.CharField(db_column='Descripcion1', max_length=100, blank=True, null=True)
-    descripcion2 = models.CharField(db_column='Descripcion2', max_length=255, blank=True, null=True)
-    grupo = models.CharField(db_column='Grupo', max_length=50, blank=True, null=True)
-    categoria = models.CharField(db_column='Categoria', max_length=50, blank=True, null=True)
-    impuesto1 = models.FloatField(db_column='Impuesto1')
-    impuesto2 = models.FloatField(db_column='Impuesto2', blank=True, null=True)
-    impuesto3 = models.FloatField(db_column='Impuesto3', blank=True, null=True)
-    tipo = models.CharField(db_column='Tipo', max_length=20)
-    precio_lista = models.DecimalField(db_column='PrecioLista', max_digits=19, decimal_places=4, blank=True, null=True)
-    estatus = models.CharField(db_column='Estatus', max_length=15)
-    usuario = models.CharField(db_column='Usuario', max_length=10, blank=True, null=True)
-    precio2 = models.DecimalField(db_column='Precio2', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio3 = models.DecimalField(db_column='Precio3', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio4 = models.DecimalField(db_column='Precio4', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio5 = models.DecimalField(db_column='Precio5', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio6 = models.DecimalField(db_column='Precio6', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio7 = models.DecimalField(db_column='Precio7', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio8 = models.DecimalField(db_column='Precio8', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio9 = models.DecimalField(db_column='Precio9', max_digits=19, decimal_places=4, blank=True, null=True)
-    precio10 = models.DecimalField(db_column='Precio10', max_digits=19, decimal_places=4, blank=True, null=True)
-    situacion = models.CharField(db_column='Situacion', max_length=50, blank=True, null=True)
-    tipo_compra = models.CharField(db_column='TipoCompra', max_length=20, blank=True, null=True)
-    retencion1 = models.FloatField(db_column='Retencion1', blank=True, null=True)
-    retencion2 = models.FloatField(db_column='Retencion2', blank=True, null=True)
-    retencion3 = models.FloatField(db_column='Retencion3', blank=True, null=True)
-    modelo = models.CharField(db_column='Modelo', max_length=4, blank=True, null=True)
-    direccion = models.CharField(db_column='Direccion', max_length=100, blank=True, null=True)
-    direccion_numero = models.CharField(db_column='DireccionNumero', max_length=20, blank=True, null=True)
-    direccion_numero_int = models.CharField(db_column='DireccionNumeroInt', max_length=20, blank=True, null=True)
-    observaciones = models.CharField(db_column='Observaciones', max_length=100, blank=True, null=True)
-    colonia = models.CharField(db_column='Colonia', max_length=100, blank=True, null=True)
-    delegacion = models.CharField(db_column='Delegacion', max_length=100, blank=True, null=True)
-    poblacion = models.CharField(db_column='Poblacion', max_length=100, blank=True, null=True)
-    estado = models.CharField(db_column='Estado', max_length=30, blank=True, null=True)
-    pais = models.CharField(db_column='Pais', max_length=30, blank=True, null=True)
-    codigo_postal = models.CharField(db_column='CodigoPostal', max_length=15, blank=True, null=True)
-    tipo_impuesto1 = models.CharField(db_column='TipoImpuesto1', max_length=10, blank=True, null=True)
-    tipo_impuesto2 = models.CharField(db_column='TipoImpuesto2', max_length=10, blank=True, null=True)
-    tipo_impuesto3 = models.CharField(db_column='TipoImpuesto3', max_length=10, blank=True, null=True)
-
-    class Meta:
-        db_table = 'Art'
-        managed = False
-
-
 class Sucursal(BaseModel):
     sucursal = models.IntegerField(db_column='Sucursal', primary_key=True)
     nombre = models.CharField(db_column='Nombre', max_length=100, blank=True, null=True)
     prefijo = models.CharField(db_column='Prefijo', max_length=5, blank=True, null=True)
     estatus = models.CharField(db_column='Estatus', max_length=15)
     rfc = models.CharField(db_column='RFC', max_length=20, blank=True, null=True)
     alta = models.DateTimeField(db_column='Alta', blank=True, null=True)
```

### Comparing `isapilib-1.6.9/isapilib/core/models.py` & `isapilib-1.7.0/isapilib/core/models.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/decorators.py` & `isapilib-1.7.0/isapilib/decorators.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/management/commands/check_branch.py` & `isapilib-1.7.0/isapilib/management/commands/check_branch.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/management/commands/external_migrate.py` & `isapilib-1.7.0/isapilib/management/commands/external_migrate.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/migrations/0001_initial.py` & `isapilib-1.7.0/isapilib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/models.py` & `isapilib-1.7.0/isapilib/models.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/static/css/bootstrap.min.css` & `isapilib-1.7.0/isapilib/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/static/img/intelisis128.png` & `isapilib-1.7.0/isapilib/static/img/intelisis128.png`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/templates/index.html` & `isapilib-1.7.0/isapilib/templates/index.html`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib/utilities.py` & `isapilib-1.7.0/isapilib/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,7 +103,21 @@
         log.request = str(json.dumps(request.data) if isinstance(request.data, dict) else request.data or '')
         log.response = str(response.decode('utf-8') or '')
         log.url = request.build_absolute_uri()
         log.interfaz = str(interfaz or '')
         log.save()
     except Exception as e:
         print(f'Warning: Failed to save logs', e)
+
+
+def clean_request_json(request: dict) -> dict:
+    cleaned_request = {}
+    for k, v in request.items():
+        if v is None or v == '':
+            continue
+
+        if isinstance(v, dict):
+            v = clean_request_json(v)
+
+        cleaned_request[k] = v
+
+    return cleaned_request
```

### Comparing `isapilib-1.6.9/isapilib/views.py` & `isapilib-1.7.0/isapilib/views.py`

 * *Files identical despite different names*

### Comparing `isapilib-1.6.9/isapilib.egg-info/SOURCES.txt` & `isapilib-1.7.0/isapilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

