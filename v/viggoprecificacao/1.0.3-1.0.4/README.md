# Comparing `tmp/viggoprecificacao-1.0.3.tar.gz` & `tmp/viggoprecificacao-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggoprecificacao-1.0.3.tar", last modified: Tue May  7 13:47:51 2024, max compression
+gzip compressed data, was "viggoprecificacao-1.0.4.tar", last modified: Tue May 28 18:59:11 2024, max compression
```

## Comparing `viggoprecificacao-1.0.3.tar` & `viggoprecificacao-1.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.031356 viggoprecificacao-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 13:47:51.031356 viggoprecificacao-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 13:47:51.031356 viggoprecificacao-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.023356 viggoprecificacao-1.0.3/viggoprecificacao/
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.027356 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.027356 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.027356 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.027356 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.027356 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/produto_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/produto_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.027356 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/servico_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/servico_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.031356 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-07 13:46:59.000000 viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:47:51.027356 viggoprecificacao-1.0.3/viggoprecificacao.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-07 13:47:50.000000 viggoprecificacao-1.0.3/viggoprecificacao.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-07 13:47:50.000000 viggoprecificacao-1.0.3/viggoprecificacao.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:47:50.000000 viggoprecificacao-1.0.3/viggoprecificacao.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 13:47:50.000000 viggoprecificacao-1.0.3/viggoprecificacao.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 13:47:50.000000 viggoprecificacao-1.0.3/viggoprecificacao.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.008656 viggoprecificacao-1.0.4/viggoprecificacao/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.008656 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.008656 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10646 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/produto_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/produto_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/servico_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/servico_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.012656 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-28 18:58:27.000000 viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:59:11.008656 viggoprecificacao-1.0.4/viggoprecificacao.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-28 18:59:10.000000 viggoprecificacao-1.0.4/viggoprecificacao.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-28 18:59:10.000000 viggoprecificacao-1.0.4/viggoprecificacao.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:59:10.000000 viggoprecificacao-1.0.4/viggoprecificacao.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 18:59:10.000000 viggoprecificacao-1.0.4/viggoprecificacao.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 18:59:10.000000 viggoprecificacao-1.0.4/viggoprecificacao.egg-info/top_level.txt
```

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/__init__.py` & `viggoprecificacao-1.0.4/viggoprecificacao/__init__.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/controller.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/manager.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/contrato_viggo/resource.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/controller.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/manager.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/plano_viggo/resource.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/produto_viggo/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 class PRODUTO_VIGGO_TIPO(Enum):
     VENDA = 'VENDA'
     LOCACAO = 'LOCACAO'
 
 
 class ProdutoViggo(entity.Entity, db.Model):
 
+    CODIGO_SEQUENCE = 'produto_viggo_codigo_sq'
+
     attributes = ['nome', 'descricao', 'valor', 'modelo', 'identificador_prod',
-                  'config_acessorios', 'fabricante', 'qtd',
+                  'config_acessorios', 'fabricante', 'qtd', 'codigo',
                   'qtd_dias_p_entrega', 'tem_garantia', 'tipo', 'tipo_locacao',
                   'taxa_locacao_fabricante']
     read_only_attributes = ['qtd_disponivel', 'qtd_uso']
     attributes += entity.Entity.attributes
 
+    codigo = db.Column(db.Numeric(10), nullable=False, unique=True)
     nome = db.Column(db.String(60), nullable=False)
     descricao = db.Column(db.String(250), nullable=False)
     valor = db.Column(db.Numeric(17, 4), nullable=True)
     modelo = db.Column(db.String(60), nullable=True)
     identificador_prod = db.Column(db.String(50), nullable=True)
     config_acessorios = db.Column(db.String(1000), nullable=True)
     fabricante = db.Column(db.String(250), nullable=True)
@@ -37,14 +40,15 @@
                              nullable=True)
     taxa_locacao_fabricante = db.Column(db.Numeric(17, 4),
                                         nullable=True)
 
     def __init__(self, id, nome, descricao, valor, modelo, identificador_prod,
                  config_acessorios, fabricante, qtd, qtd_dias_p_entrega,
                  tem_garantia, tipo, tipo_locacao, taxa_locacao_fabricante,
+                 codigo,
                  active=True, created_at=None, created_by=None,
                  updated_at=None, updated_by=None, tag=None):
         super().__init__(id, active, created_at, created_by,
                          updated_at, updated_by, tag)
         self.nome = nome
         self.descricao = descricao
         self.valor = valor
@@ -54,14 +58,15 @@
         self.fabricante = fabricante
         self.qtd = qtd
         self.qtd_dias_p_entrega = qtd_dias_p_entrega
         self.tem_garantia = tem_garantia
         self.tipo = tipo
         self.tipo_locacao = tipo_locacao
         self.taxa_locacao_fabricante = taxa_locacao_fabricante
+        self.codigo = codigo
 
     @classmethod
     def individual(cls):
         return 'produto_viggo'
 
     @classmethod
     def collection(cls):
```

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/servico_viggo/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,48 +10,52 @@
     QUINZENAL = 'QUINZENAL'
     MENSAL = 'MENSAL'
     ANUAL = 'ANUAL'
 
 
 class ServicoViggo(entity.Entity, db.Model):
 
+    CODIGO_SEQUENCE = 'servico_viggo_codigo_sq'
+
     attributes = ['nome', 'descricao', 'v_aquisicao', 'v_recorrencia',
-                  'v_adicional', 'qtd_min_mes', 'qtd_max_mes',
+                  'v_adicional', 'qtd_min_mes', 'qtd_max_mes', 'codigo',
                   'dias_carencia', 'dias_vigencia', 'frequencia']
     attributes += entity.Entity.attributes
 
+    codigo = db.Column(db.Numeric(10), nullable=False, unique=True)
     nome = db.Column(db.String(60), nullable=False)
     descricao = db.Column(db.String(250), nullable=False)
     v_aquisicao = db.Column(db.Numeric(17, 4), nullable=True)
     v_recorrencia = db.Column(db.Numeric(17, 4), nullable=True)
     v_adicional = db.Column(db.Numeric(17, 4), nullable=True)
     qtd_min_mes = db.Column(db.Numeric(17, 4), nullable=True)
     qtd_max_mes = db.Column(db.Numeric(17, 4), nullable=True)
     dias_carencia = db.Column(db.Numeric(4), nullable=True)
     dias_vigencia = db.Column(db.Numeric(4), nullable=True)
     frequencia = db.Column(db.Enum(SERVICO_VIGGO_FREQUENCIA),
                            nullable=True)
 
     def __init__(self, id, nome, descricao, v_aquisicao, v_recorrencia,
                  v_adicional, qtd_min_mes, qtd_max_mes, dias_carencia,
-                 dias_vigencia, frequencia,
+                 dias_vigencia, frequencia, codigo,
                  active=True, created_at=None, created_by=None,
                  updated_at=None, updated_by=None, tag=None):
         super().__init__(id, active, created_at, created_by,
                          updated_at, updated_by, tag)
         self.nome = nome
         self.descricao = descricao
         self.v_aquisicao = v_aquisicao
         self.v_recorrencia = v_recorrencia
         self.v_adicional = v_adicional
         self.qtd_min_mes = qtd_min_mes
         self.qtd_max_mes = qtd_max_mes
         self.dias_carencia = dias_carencia
         self.dias_vigencia = dias_vigencia
         self.frequencia = frequencia
+        self.codigo = codigo
 
     @classmethod
     def individual(cls):
         return 'servico_viggo'
 
     @classmethod
     def collection(cls):
```

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/controller.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/manager.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py` & `viggoprecificacao-1.0.4/viggoprecificacao/subsystem/parametrizacao/termo_aceite_viggo/resource.py`

 * *Files identical despite different names*

### Comparing `viggoprecificacao-1.0.3/viggoprecificacao.egg-info/SOURCES.txt` & `viggoprecificacao-1.0.4/viggoprecificacao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

