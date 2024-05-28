# Comparing `tmp/frformat-0.2.2.tar.gz` & `tmp/frformat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frformat-0.2.2.tar", max compression
+gzip compressed data, was "frformat-0.3.0.tar", max compression
```

## Comparing `frformat-0.2.2.tar` & `frformat-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
--rw-r--r--   0        0        0    34523 2024-05-13 08:57:59.801746 frformat-0.2.2/LICENSE
--rw-r--r--   0        0        0      456 2024-05-13 08:57:59.801746 frformat-0.2.2/README.md
--rw-r--r--   0        0        0      690 2024-05-13 08:58:11.621797 frformat-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      950 2024-05-13 08:57:59.801746 frformat-0.2.2/src/frformat/__init__.py
--rw-r--r--   0        0        0      463 2024-05-13 08:57:59.801746 frformat-0.2.2/src/frformat/common.py
--rw-r--r--   0        0        0     1200 2024-05-13 08:57:59.801746 frformat-0.2.2/src/frformat/custom_format.py
--rw-r--r--   0        0        0      983 2024-05-13 08:57:59.801746 frformat-0.2.2/src/frformat/enum_format.py
--rw-r--r--   0        0        0      263 2024-05-13 08:57:59.801746 frformat-0.2.2/src/frformat/geo/canton.py
--rw-r--r--   0        0        0    45742 2024-05-13 08:57:59.801746 frformat-0.2.2/src/frformat/geo/canton_set.py
--rw-r--r--   0        0        0      298 2024-05-13 08:57:59.801746 frformat-0.2.2/src/frformat/geo/code_commune_insee.py
--rw-r--r--   0        0        0   488829 2024-05-13 08:57:59.805746 frformat-0.2.2/src/frformat/geo/code_commune_insee_set.py
--rw-r--r--   0        0        0      720 2024-05-13 08:57:59.805746 frformat-0.2.2/src/frformat/geo/code_fantoir.py
--rw-r--r--   0        0        0   313495 2024-05-13 08:57:59.805746 frformat-0.2.2/src/frformat/geo/code_fantoir_set.py
--rw-r--r--   0        0        0      403 2024-05-13 08:57:59.805746 frformat-0.2.2/src/frformat/geo/code_pays.py
--rw-r--r--   0        0        0     4566 2024-05-13 08:57:59.805746 frformat-0.2.2/src/frformat/geo/code_pays_set.py
--rw-r--r--   0        0        0      256 2024-05-13 08:57:59.805746 frformat-0.2.2/src/frformat/geo/code_postal.py
--rw-r--r--   0        0        0   478708 2024-05-13 08:57:59.809746 frformat-0.2.2/src/frformat/geo/code_postal_set.py
--rw-r--r--   0        0        0      431 2024-05-13 08:57:59.809746 frformat-0.2.2/src/frformat/geo/code_region.py
--rw-r--r--   0        0        0      319 2024-05-13 08:57:59.809746 frformat-0.2.2/src/frformat/geo/commune.py
--rw-r--r--   0        0        0   761291 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/commune_set.py
--rw-r--r--   0        0        0     4556 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/coordonnees_gps_francaises.py
--rw-r--r--   0        0        0      291 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/departement.py
--rw-r--r--   0        0        0     1766 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/departement_set.py
--rw-r--r--   0        0        0      453 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/numero_departement.py
--rw-r--r--   0        0        0      238 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/pays.py
--rw-r--r--   0        0        0     4390 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/pays_set.py
--rw-r--r--   0        0        0      304 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/region.py
--rw-r--r--   0        0        0     1315 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/geo/region_set.py
--rw-r--r--   0        0        0     2593 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/nomenclature_acte_format.py
--rw-r--r--   0        0        0      516 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/siren.py
--rw-r--r--   0        0        0      503 2024-05-13 08:57:59.813746 frformat-0.2.2/src/frformat/siret.py
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 frformat-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-28 08:45:31.527325 frformat-0.3.0/LICENSE
+-rw-r--r--   0        0        0      538 2024-05-28 08:45:31.527325 frformat-0.3.0/README.md
+-rw-r--r--   0        0        0      690 2024-05-28 08:45:41.507514 frformat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1108 2024-05-28 08:45:31.527325 frformat-0.3.0/src/frformat/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-28 08:45:31.527325 frformat-0.3.0/src/frformat/code_rna.py
+-rw-r--r--   0        0        0      548 2024-05-28 08:45:31.527325 frformat-0.3.0/src/frformat/common.py
+-rw-r--r--   0        0        0      836 2024-05-28 08:45:31.527325 frformat-0.3.0/src/frformat/custom_format.py
+-rw-r--r--   0        0        0      881 2024-05-28 08:45:31.527325 frformat-0.3.0/src/frformat/enum_format.py
+-rw-r--r--   0        0        0     1125 2024-05-28 08:45:31.527325 frformat-0.3.0/src/frformat/formatter.py
+-rw-r--r--   0        0        0      263 2024-05-28 08:45:31.527325 frformat-0.3.0/src/frformat/geo/canton.py
+-rw-r--r--   0        0        0    45742 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/canton_set.py
+-rw-r--r--   0        0        0      298 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/code_commune_insee.py
+-rw-r--r--   0        0        0   488829 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/code_commune_insee_set.py
+-rw-r--r--   0        0        0      741 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/code_fantoir.py
+-rw-r--r--   0        0        0   313495 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/code_fantoir_set.py
+-rw-r--r--   0        0        0      403 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/code_pays.py
+-rw-r--r--   0        0        0     4566 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/code_pays_set.py
+-rw-r--r--   0        0        0      256 2024-05-28 08:45:31.531325 frformat-0.3.0/src/frformat/geo/code_postal.py
+-rw-r--r--   0        0        0   478708 2024-05-28 08:45:31.535325 frformat-0.3.0/src/frformat/geo/code_postal_set.py
+-rw-r--r--   0        0        0      431 2024-05-28 08:45:31.535325 frformat-0.3.0/src/frformat/geo/code_region.py
+-rw-r--r--   0        0        0      319 2024-05-28 08:45:31.535325 frformat-0.3.0/src/frformat/geo/commune.py
+-rw-r--r--   0        0        0   761291 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/commune_set.py
+-rw-r--r--   0        0        0     4524 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/coordonnees_gps_francaises.py
+-rw-r--r--   0        0        0      291 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/departement.py
+-rw-r--r--   0        0        0     1766 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/departement_set.py
+-rw-r--r--   0        0        0      471 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/latitude_l93.py
+-rw-r--r--   0        0        0      482 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/longitude_l93.py
+-rw-r--r--   0        0        0      453 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/numero_departement.py
+-rw-r--r--   0        0        0      238 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/pays.py
+-rw-r--r--   0        0        0     4390 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/pays_set.py
+-rw-r--r--   0        0        0      304 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/region.py
+-rw-r--r--   0        0        0     1315 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/geo/region_set.py
+-rw-r--r--   0        0        0     2548 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/nomenclature_acte_format.py
+-rw-r--r--   0        0        0      623 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/siren.py
+-rw-r--r--   0        0        0      602 2024-05-28 08:45:31.539325 frformat-0.3.0/src/frformat/siret.py
+-rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 frformat-0.3.0/PKG-INFO
```

### Comparing `frformat-0.2.2/LICENSE` & `frformat-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/pyproject.toml` & `frformat-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frformat"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 authors = [
   "Pierre Camilleri <22995923+pierrecamilleri@users.noreply.github.com>",
   "Amélie Rondot"
 ]
 license = "AGPL-3.0"
 readme = "README.md"
```

### Comparing `frformat-0.2.2/src/frformat/__init__.py` & `frformat-0.3.0/src/frformat/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # flake8: noqa
 from .custom_format import *  # isort:skip
 
+from .code_rna import CodeRNA as CodeRNA
 from .geo.canton import Canton as Canton
 from .geo.code_commune_insee import CodeCommuneInsee as CodeCommuneInsee
 from .geo.code_fantoir import CodeFantoir as CodeFantoir
 from .geo.code_pays import CodePaysISO2 as CodePaysISO2
 from .geo.code_pays import CodePaysISO3 as CodePaysISO3
 from .geo.code_postal import CodePostal as CodePostal
 from .geo.code_region import CodeRegion as CodeRegion
 from .geo.commune import Commune as Commune
 from .geo.coordonnees_gps_francaises import (
     CoordonneesGPSFrancaises as CoordonneesGPSFrancaises,
 )
 from .geo.departement import Departement as Departement
+from .geo.latitude_l93 import LatitudeL93 as LatitudeL93
+from .geo.longitude_l93 import LongitudeL93 as LongitudeL93
 from .geo.numero_departement import NumeroDepartement as NumeroDepartement
 from .geo.pays import Pays as Pays
 from .geo.region import Region as Region
 from .nomenclature_acte_format import NomenclatureActe as NomenclatureActe
 from .siren import Siren as Siren
 from .siret import Siret as Siret
```

### Comparing `frformat-0.2.2/src/frformat/enum_format.py` & `frformat-0.3.0/src/frformat/enum_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 from typing import Optional, Set
 
-from frformat import CustomFormat
+from frformat import CustomStrFormat, Metadata
 from frformat.common import normalize_text
 
 
 def new(
     name: str,
     description: str,
     strict_enum: Set[str],
     lenient_enum: Optional[Set[str]] = None,
 ):
     if not lenient_enum:
         lenient_enum = {normalize_text(e) for e in strict_enum}
 
-    class EnumFormat(CustomFormat):
+    class EnumFormat(CustomStrFormat):
         """Checks if a value is in a given list
 
         May check with or without string normalization with the "strict"
         validation.
         """
 
-        @classmethod
-        def name(cls) -> str:
-            return name
-
-        @classmethod
-        def description(cls) -> str:
-            return description
+        metadata = Metadata(name, description)
 
         @classmethod
         def is_valid(cls, value: str, strict: bool = True) -> bool:
             if not strict:
                 norm_value = normalize_text(value)
                 return norm_value in lenient_enum
             else:
```

### Comparing `frformat-0.2.2/src/frformat/geo/canton_set.py` & `frformat-0.3.0/src/frformat/geo/canton_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/code_commune_insee_set.py` & `frformat-0.3.0/src/frformat/geo/code_commune_insee_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/code_fantoir.py` & `frformat-0.3.0/src/frformat/geo/code_fantoir.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import string
 
-from frformat import CustomFormat
+from frformat import CustomStrFormat, Metadata
+from frformat.formatter import Formatter
 from frformat.geo.code_fantoir_set import PARTIAL_CODE_FANTOIR_SET
 
 name = "Code fantoir"
 description = "Vérifie les codes fantoirs valides"
 
 UPPER_LETTERS = string.ascii_uppercase
 
 
-class CodeFantoir(CustomFormat):
-    @classmethod
-    def name(cls) -> str:
-        return name
+class CodeFantoirFormatter(Formatter):
+    def format(self, value: str) -> str:
+        return f"{value[0:3]} {value[3:6]} {value[6:]}"
 
-    @classmethod
-    def description(cls) -> str:
-        return description
+
+class CodeFantoir(CustomStrFormat):
+    metadata = Metadata(name, description)
+    formatter = CodeFantoirFormatter()
 
     @classmethod
     def is_valid(cls, value: str) -> bool:
         if len(value) != 5:
             return False
 
         return value[4] in UPPER_LETTERS and value[:4] in PARTIAL_CODE_FANTOIR_SET
-
-    @classmethod
-    def _format(cls, value: str) -> str:
-        return f"{value[0:3]} {value[3:6]} {value[6:]}"
```

### Comparing `frformat-0.2.2/src/frformat/geo/code_fantoir_set.py` & `frformat-0.3.0/src/frformat/geo/code_fantoir_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/code_pays_set.py` & `frformat-0.3.0/src/frformat/geo/code_pays_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/code_postal_set.py` & `frformat-0.3.0/src/frformat/geo/code_postal_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/commune_set.py` & `frformat-0.3.0/src/frformat/geo/commune_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/coordonnees_gps_francaises.py` & `frformat-0.3.0/src/frformat/geo/coordonnees_gps_francaises.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from shapely.geometry import Point, shape
 
+from frformat import Metadata
 
-class CoordonneesGPSFrancaises:
-    @classmethod
-    def name(cls) -> str:
-        return "Coordonnées GPS françaises"
+name = "Coordonnées GPS françaises"
+description = """Check that GPS coordinates are in a bounding box approximating France (including DOM)"""
 
-    @classmethod
-    def description(cls) -> str:
-        return """Check that GPS coordinates are in a bounding box approximating
-    France (including DOM)"""
+
+class CoordonneesGPSFrancaises:
+    metadata = Metadata(name, description)
 
     @classmethod
     def is_valid(cls, lon: float, lat: float) -> bool:
         return is_point_in_france((lon, lat))
 
 
 def is_point_in_france(coordonnees_xy: tuple[float, float]) -> bool:
```

### Comparing `frformat-0.2.2/src/frformat/geo/departement_set.py` & `frformat-0.3.0/src/frformat/geo/departement_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/pays_set.py` & `frformat-0.3.0/src/frformat/geo/pays_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/geo/region_set.py` & `frformat-0.3.0/src/frformat/geo/region_set.py`

 * *Files identical despite different names*

### Comparing `frformat-0.2.2/src/frformat/nomenclature_acte_format.py` & `frformat-0.3.0/src/frformat/nomenclature_acte_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Literal, Tuple, Union
 
-from frformat import CustomFormat
+from frformat import CustomStrFormat, Metadata
 
 AUTHORIZED_VALUES = {
     "Commande publique",
     "Urbanisme",
     "Domaine et patrimoine",
     "Fonction publique",
     "Institutions et vie politique",
@@ -23,22 +23,17 @@
     return f"le préfixe de nomenclature Actes {prefix!r} n'est pas reconnu"
 
 
 ValidWithoutDetails = Tuple[Literal[True], None]
 InvalidWithDetails = Tuple[Literal[False], List[str]]
 
 
-class NomenclatureActe(CustomFormat):
-    @classmethod
-    def name(cls) -> str:
-        return "Nomenclature des actes"
+name = "Nomenclature des actes"
 
-    @classmethod
-    def description(cls) -> str:
-        return """
+description = """
         Document de référence dans les spécifications SCDL :
         http://www.moselle.gouv.fr/content/download/1107/7994/file/nomenclature.pdf
 
         Dans la nomenclature Actes, les valeurs avant le '/' sont :
 
         Commande publique
         Urbanisme
@@ -47,15 +42,19 @@
         Institutions et vie politique
         Libertés publiques et pouvoirs de police
         Finances locales
         Domaines de compétences par thèmes
         Autres domaines de compétences
 
         La validation devra accepter minuscules et majuscules, accents et sans accents ...
-    """
+"""
+
+
+class NomenclatureActe(CustomStrFormat):
+    metadata = Metadata(name, description)
 
     @classmethod
     def is_valid(cls, value: str) -> bool:
         nomenc = cls._nomenclature(value)
 
         # Nomenclature reconnue et pas d'espace après l'oblique
         return "/ " not in value and nomenc in AUTHORIZED_VALUES
```

