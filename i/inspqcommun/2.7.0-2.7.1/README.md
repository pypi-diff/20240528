# Comparing `tmp/inspqcommun-2.7.0.tar.gz` & `tmp/inspqcommun-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspqcommun-2.7.0.tar", last modified: Mon May 27 20:41:22 2024, max compression
+gzip compressed data, was "inspqcommun-2.7.1.tar", last modified: Tue May 28 15:24:29 2024, max compression
```

## Comparing `inspqcommun-2.7.0.tar` & `inspqcommun-2.7.1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/
--rw-r--r--   0 jenkins    (114) jenkins    (119)    12567 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/LICENSE
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/PKG-INFO
--rw-r--r--   0 jenkins    (114) jenkins    (119)      509 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/README.md
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.092912 inspqcommun-2.7.0/inspqcommun/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/__init__.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.092912 inspqcommun-2.7.0/inspqcommun/fa/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9076 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/chargement_service.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1337 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/chargeur_fichiers.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3747 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/fa/configuration.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.096912 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5077 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      514 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_base.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4638 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_usager.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9403 2024-05-16 21:04:23.000000 inspqcommun-2.7.0/inspqcommun/fa/injecteur.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.100912 inspqcommun-2.7.0/inspqcommun/fa/ressources/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/acte_vaccinal.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      515 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/lieu_vaccination.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      318 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/organisation.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      983 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/ressource.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/usager.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      567 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/ressources/vaccinateur.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.100912 inspqcommun-2.7.0/inspqcommun/fa/validateurs/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1351 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    12238 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9263 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_usager.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.100912 inspqcommun-2.7.0/inspqcommun/fhir/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/__init__.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.104912 inspqcommun-2.7.0/inspqcommun/fhir/clients/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2831 2024-05-16 21:04:23.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/base_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5013 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/immunization_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4539 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/location_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1344 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/medication_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4890 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/organization_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5202 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/patient_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2557 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/practitioner_client.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3800 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/clients/value_set_client.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.112912 inspqcommun-2.7.0/inspqcommun/fhir/visitors/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     3226 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/base.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1668 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/bundle.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2233 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/condition.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    21783 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/immunization.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     4624 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/location.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2516 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/medication.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      972 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/operation_outcome.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5399 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/organization.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1257 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/parameters.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    11042 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/patient.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)      859 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/practitioner.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1364 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/fhir/visitors/value_set.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.116912 inspqcommun-2.7.0/inspqcommun/identity/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/identity/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)   164019 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/identity/keycloak.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1413 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/identity/keycloak_token.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)    11219 2024-05-27 20:41:09.000000 inspqcommun-2.7.0/inspqcommun/identity/keycloak_tools.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.116912 inspqcommun-2.7.0/inspqcommun/kafka/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/kafka/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     7943 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/kafka/consommateur.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     5280 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/kafka/producteur.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/inspqcommun/userprovisioning/
--rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/userprovisioning/__init__.py
--rw-r--r--   0 jenkins    (114) jenkins    (119)     9944 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/inspqcommun/userprovisioning/scim.py
-drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/inspqcommun.egg-info/
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (114) jenkins    (119)     2321 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)        1 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)      104 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/requires.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)       12 2024-05-27 20:41:22.000000 inspqcommun-2.7.0/inspqcommun.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (114) jenkins    (119)       38 2024-05-27 20:41:22.120912 inspqcommun-2.7.0/setup.cfg
--rw-r--r--   0 jenkins    (114) jenkins    (119)     1373 2024-05-09 15:48:27.000000 inspqcommun-2.7.0/setup.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.046946 inspqcommun-2.7.1/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    12567 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/LICENSE
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-28 15:24:29.046946 inspqcommun-2.7.1/PKG-INFO
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      509 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/README.md
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.022946 inspqcommun-2.7.1/inspqcommun/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/__init__.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.022946 inspqcommun-2.7.1/inspqcommun/fa/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9076 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/chargement_service.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1337 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/chargeur_fichiers.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3789 2024-05-28 15:24:15.000000 inspqcommun-2.7.1/inspqcommun/fa/configuration.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.026946 inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5077 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      514 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/convertisseur_base.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4638 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/convertisseur_usager.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9403 2024-05-16 21:04:23.000000 inspqcommun-2.7.1/inspqcommun/fa/injecteur.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.030946 inspqcommun-2.7.1/inspqcommun/fa/ressources/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/ressources/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/ressources/acte_vaccinal.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      515 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/ressources/lieu_vaccination.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      318 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/ressources/organisation.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      983 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/ressources/ressource.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2610 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/ressources/usager.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      567 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/ressources/vaccinateur.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.030946 inspqcommun-2.7.1/inspqcommun/fa/validateurs/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/validateurs/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1351 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/validateurs/validateur.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    12238 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9263 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fa/validateurs/validateur_usager.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.030946 inspqcommun-2.7.1/inspqcommun/fhir/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/__init__.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.034946 inspqcommun-2.7.1/inspqcommun/fhir/clients/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2831 2024-05-16 21:04:23.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/base_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5013 2024-05-27 20:41:09.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/immunization_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4539 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/location_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1344 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/medication_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4890 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/organization_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5202 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/patient_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2557 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/practitioner_client.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3800 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/clients/value_set_client.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.042946 inspqcommun-2.7.1/inspqcommun/fhir/visitors/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     3226 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/base.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1668 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/bundle.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2233 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/condition.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    21783 2024-05-27 20:41:09.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/immunization.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     4624 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/location.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2516 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/medication.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      972 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/operation_outcome.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5399 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/organization.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1257 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/parameters.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    11042 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/patient.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      859 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/practitioner.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1364 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/fhir/visitors/value_set.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.042946 inspqcommun-2.7.1/inspqcommun/identity/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/identity/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)   164019 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/identity/keycloak.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1413 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/identity/keycloak_token.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)    11219 2024-05-27 20:41:09.000000 inspqcommun-2.7.1/inspqcommun/identity/keycloak_tools.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.046946 inspqcommun-2.7.1/inspqcommun/kafka/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/kafka/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     7943 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/kafka/consommateur.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     5280 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/kafka/producteur.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.046946 inspqcommun-2.7.1/inspqcommun/userprovisioning/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        0 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/userprovisioning/__init__.py
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     9944 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/inspqcommun/userprovisioning/scim.py
+drwxr-xr-x   0 jenkins    (114) jenkins    (119)        0 2024-05-28 15:24:29.046946 inspqcommun-2.7.1/inspqcommun.egg-info/
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1059 2024-05-28 15:24:28.000000 inspqcommun-2.7.1/inspqcommun.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     2321 2024-05-28 15:24:28.000000 inspqcommun-2.7.1/inspqcommun.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)        1 2024-05-28 15:24:28.000000 inspqcommun-2.7.1/inspqcommun.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)      104 2024-05-28 15:24:28.000000 inspqcommun-2.7.1/inspqcommun.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)       12 2024-05-28 15:24:28.000000 inspqcommun-2.7.1/inspqcommun.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (114) jenkins    (119)       38 2024-05-28 15:24:29.046946 inspqcommun-2.7.1/setup.cfg
+-rw-r--r--   0 jenkins    (114) jenkins    (119)     1373 2024-05-09 15:48:27.000000 inspqcommun-2.7.1/setup.py
```

### Comparing `inspqcommun-2.7.0/LICENSE` & `inspqcommun-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/PKG-INFO` & `inspqcommun-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspqcommun
-Version: 2.7.0
+Version: 2.7.1
 Summary: Librairies communes de INSPQ
 Home-page: https://gitlab.forge.gouv.qc.ca/inspq/commun/python/inspqcommun.git
 Author: Philippe Gauthier
 Author-email: philippe.gauthier@inspq.qc.ca
 License: LiLiQ
 License-File: LICENSE
 Requires-Dist: fhirclient==1.0.3
```

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/chargement_service.py` & `inspqcommun-2.7.1/inspqcommun/fa/chargement_service.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/chargeur_fichiers.py` & `inspqcommun-2.7.1/inspqcommun/fa/chargeur_fichiers.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/configuration.py` & `inspqcommun-2.7.1/inspqcommun/fa/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 DEFAULT_KEYCLOAK_AUTH_USER: str = 'PERMISSIONS'
 DEFAULT_KEYCLOAK_AUTH_PASSWORD: str = ''
 DEFAULT_KEYCLOAK_AUTH_CLIENT_ID: str = "admin-cli"
 DEFAULT_KEYCLOAK_ENABLED: str = "False"
 DEFAULT_VALIDATE_CERTS: str = "true"
 class Configuration:
     client_roles = ["fa-utilisateur", "fa-saisie"]
+    username = None
+    password = None
     def __init__(self, client_roles:list=None, username:str=None, password=None) -> None:
         if client_roles is not None and len(client_roles) > 0:
             self.client_roles = client_roles
         
         self.username = username
         self.password = password
```

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py` & `inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/convertisseur_acte_vaccinal.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_base.py` & `inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/convertisseur_base.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/convertisseurs/convertisseur_usager.py` & `inspqcommun-2.7.1/inspqcommun/fa/convertisseurs/convertisseur_usager.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/injecteur.py` & `inspqcommun-2.7.1/inspqcommun/fa/injecteur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/ressources/acte_vaccinal.py` & `inspqcommun-2.7.1/inspqcommun/fa/ressources/acte_vaccinal.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/ressources/lieu_vaccination.py` & `inspqcommun-2.7.1/inspqcommun/fa/ressources/lieu_vaccination.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/ressources/ressource.py` & `inspqcommun-2.7.1/inspqcommun/fa/ressources/ressource.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/ressources/usager.py` & `inspqcommun-2.7.1/inspqcommun/fa/ressources/usager.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/ressources/vaccinateur.py` & `inspqcommun-2.7.1/inspqcommun/fa/ressources/vaccinateur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur.py` & `inspqcommun-2.7.1/inspqcommun/fa/validateurs/validateur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py` & `inspqcommun-2.7.1/inspqcommun/fa/validateurs/validateur_acte_vaccinal.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fa/validateurs/validateur_usager.py` & `inspqcommun-2.7.1/inspqcommun/fa/validateurs/validateur_usager.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/base_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/base_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/immunization_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/immunization_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/location_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/location_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/medication_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/medication_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/organization_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/organization_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/patient_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/patient_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/practitioner_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/practitioner_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/clients/value_set_client.py` & `inspqcommun-2.7.1/inspqcommun/fhir/clients/value_set_client.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/base.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/base.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/bundle.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/bundle.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/condition.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/condition.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/immunization.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/immunization.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/location.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/location.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/medication.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/medication.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/operation_outcome.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/operation_outcome.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/organization.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/organization.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/parameters.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/parameters.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/patient.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/patient.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/practitioner.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/practitioner.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/fhir/visitors/value_set.py` & `inspqcommun-2.7.1/inspqcommun/fhir/visitors/value_set.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/identity/keycloak.py` & `inspqcommun-2.7.1/inspqcommun/identity/keycloak.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/identity/keycloak_token.py` & `inspqcommun-2.7.1/inspqcommun/identity/keycloak_token.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/identity/keycloak_tools.py` & `inspqcommun-2.7.1/inspqcommun/identity/keycloak_tools.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/kafka/consommateur.py` & `inspqcommun-2.7.1/inspqcommun/kafka/consommateur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/kafka/producteur.py` & `inspqcommun-2.7.1/inspqcommun/kafka/producteur.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun/userprovisioning/scim.py` & `inspqcommun-2.7.1/inspqcommun/userprovisioning/scim.py`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/inspqcommun.egg-info/PKG-INFO` & `inspqcommun-2.7.1/inspqcommun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspqcommun
-Version: 2.7.0
+Version: 2.7.1
 Summary: Librairies communes de INSPQ
 Home-page: https://gitlab.forge.gouv.qc.ca/inspq/commun/python/inspqcommun.git
 Author: Philippe Gauthier
 Author-email: philippe.gauthier@inspq.qc.ca
 License: LiLiQ
 License-File: LICENSE
 Requires-Dist: fhirclient==1.0.3
```

### Comparing `inspqcommun-2.7.0/inspqcommun.egg-info/SOURCES.txt` & `inspqcommun-2.7.1/inspqcommun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inspqcommun-2.7.0/setup.py` & `inspqcommun-2.7.1/setup.py`

 * *Files identical despite different names*

