# Comparing `tmp/fastapi_starter-0.1.1.tar.gz` & `tmp/fastapi_starter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_starter-0.1.1.tar", last modified: Mon May 27 20:55:18 2024, max compression
+gzip compressed data, was "fastapi_starter-0.1.2.tar", last modified: Mon May 27 20:58:24 2024, max compression
```

## Comparing `fastapi_starter-0.1.1.tar` & `fastapi_starter-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 20:55:18.265019 fastapi_starter-0.1.1/
--rw-rw-rw-   0        0        0     1110 2024-05-27 15:05:42.000000 fastapi_starter-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     3011 2024-05-27 20:55:18.262120 fastapi_starter-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1267 2024-05-27 20:54:40.000000 fastapi_starter-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 20:55:18.155387 fastapi_starter-0.1.1/fastapi_starter/
--rw-rw-rw-   0        0        0        0 2024-05-27 20:28:55.000000 fastapi_starter-0.1.1/fastapi_starter/__init__.py
--rw-rw-rw-   0        0        0     1390 2024-05-27 20:30:28.000000 fastapi_starter-0.1.1/fastapi_starter/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-27 20:55:18.258113 fastapi_starter-0.1.1/fastapi_starter.egg-info/
--rw-rw-rw-   0        0        0     3011 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      356 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-27 20:55:18.000000 fastapi_starter-0.1.1/fastapi_starter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 20:55:18.265019 fastapi_starter-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1934 2024-05-27 20:55:01.000000 fastapi_starter-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:58:24.915068 fastapi_starter-0.1.2/
+-rw-rw-rw-   0        0        0     1110 2024-05-27 15:05:42.000000 fastapi_starter-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     2997 2024-05-27 20:58:24.915068 fastapi_starter-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1262 2024-05-27 20:57:20.000000 fastapi_starter-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 20:58:24.885980 fastapi_starter-0.1.2/fastapi_starter/
+-rw-rw-rw-   0        0        0        0 2024-05-27 20:28:55.000000 fastapi_starter-0.1.2/fastapi_starter/__init__.py
+-rw-rw-rw-   0        0        0     1390 2024-05-27 20:30:28.000000 fastapi_starter-0.1.2/fastapi_starter/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:58:24.911031 fastapi_starter-0.1.2/fastapi_starter.egg-info/
+-rw-rw-rw-   0        0        0     2997 2024-05-27 20:58:24.000000 fastapi_starter-0.1.2/fastapi_starter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-27 20:58:24.000000 fastapi_starter-0.1.2/fastapi_starter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:58:24.000000 fastapi_starter-0.1.2/fastapi_starter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-27 20:58:24.000000 fastapi_starter-0.1.2/fastapi_starter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      356 2024-05-27 20:58:24.000000 fastapi_starter-0.1.2/fastapi_starter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-27 20:58:24.000000 fastapi_starter-0.1.2/fastapi_starter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:58:24.915068 fastapi_starter-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1935 2024-05-27 20:58:09.000000 fastapi_starter-0.1.2/setup.py
```

### Comparing `fastapi_starter-0.1.1/LICENCE` & `fastapi_starter-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `fastapi_starter-0.1.1/PKG-INFO` & `fastapi_starter-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fastapi_starter
-Version: 0.1.1
+Version: 0.1.2
 Summary: A biblioteca fastapi_starter é uma ferramenta projetada para facilitar a criação rápida e eficiente de projetos baseados no framework FastAPI. Ele automatiza a criação da estrutura básica do projeto, incluindo diretórios, arquivos de configuração e rotas iniciais, além de instalar automaticamente todas as dependências necessárias. Com o fastapi_starter, os desenvolvedores podem iniciar novos projetos FastAPI com apenas alguns comandos, economizando tempo e esforço.
-Author: Jse Guilherme Lins Filho
+Author: Jose Guilherme Lins Filho
 Author-email: zeguilhermelins@hotmail.com
 License: MIT License
 Keywords: fastapi starter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: annotated-types
@@ -46,15 +46,15 @@
 Requires-Dist: uvicorn
 Requires-Dist: watchfiles
 Requires-Dist: websockets
 
 
 # FastAPI Starter
 
-A biblioteca **FastAPI Starter** oferece uma maneira rapida e fÃ¡cil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, vocÃª pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforÃ§o na configuraÃ§Ã£o inicial.
+A biblioteca **FastAPI Starter** oferece uma maneira rapida e facil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, voce pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforco na configuracao inicial.
 
 ## Como Instalar
 
 Para instalar a biblioteca, voce pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
 
 ```
 pip install fastapi_starter
```

### Comparing `fastapi_starter-0.1.1/README.md` & `fastapi_starter-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # FastAPI Starter
 
-A biblioteca **FastAPI Starter** oferece uma maneira rapida e fácil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, você pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforço na configuração inicial.
+A biblioteca **FastAPI Starter** oferece uma maneira rapida e facil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, voce pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforco na configuracao inicial.
 
 ## Como Instalar
 
 Para instalar a biblioteca, voce pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
 
 ```
 pip install fastapi_starter
```

### Comparing `fastapi_starter-0.1.1/fastapi_starter/cli.py` & `fastapi_starter-0.1.2/fastapi_starter/cli.py`

 * *Files identical despite different names*

### Comparing `fastapi_starter-0.1.1/fastapi_starter.egg-info/PKG-INFO` & `fastapi_starter-0.1.2/fastapi_starter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fastapi_starter
-Version: 0.1.1
+Version: 0.1.2
 Summary: A biblioteca fastapi_starter é uma ferramenta projetada para facilitar a criação rápida e eficiente de projetos baseados no framework FastAPI. Ele automatiza a criação da estrutura básica do projeto, incluindo diretórios, arquivos de configuração e rotas iniciais, além de instalar automaticamente todas as dependências necessárias. Com o fastapi_starter, os desenvolvedores podem iniciar novos projetos FastAPI com apenas alguns comandos, economizando tempo e esforço.
-Author: Jse Guilherme Lins Filho
+Author: Jose Guilherme Lins Filho
 Author-email: zeguilhermelins@hotmail.com
 License: MIT License
 Keywords: fastapi starter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: annotated-types
@@ -46,15 +46,15 @@
 Requires-Dist: uvicorn
 Requires-Dist: watchfiles
 Requires-Dist: websockets
 
 
 # FastAPI Starter
 
-A biblioteca **FastAPI Starter** oferece uma maneira rapida e fÃ¡cil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, vocÃª pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforÃ§o na configuraÃ§Ã£o inicial.
+A biblioteca **FastAPI Starter** oferece uma maneira rapida e facil de iniciar um novo projeto usando o FastAPI. Com apenas alguns comandos, voce pode criar a estrutura basica de um projeto FastAPI, economizando tempo e esforco na configuracao inicial.
 
 ## Como Instalar
 
 Para instalar a biblioteca, voce pode usar pip. Certifique-se de ter o Python e o pip instalados em seu sistema.
 
 ```
 pip install fastapi_starter
```

### Comparing `fastapi_starter-0.1.1/setup.py` & `fastapi_starter-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name='fastapi_starter',
-    version='0.1.1',
+    version='0.1.2',
     license='MIT License',
     long_description=readme,
     long_description_content_type="text/markdown",
     description='A biblioteca fastapi_starter é uma ferramenta projetada para facilitar a criação rápida e eficiente de projetos baseados no framework FastAPI. Ele automatiza a criação da estrutura básica do projeto, incluindo diretórios, arquivos de configuração e rotas iniciais, além de instalar automaticamente todas as dependências necessárias. Com o fastapi_starter, os desenvolvedores podem iniciar novos projetos FastAPI com apenas alguns comandos, economizando tempo e esforço.',
-    author='Jse Guilherme Lins Filho',
+    author='Jose Guilherme Lins Filho',
     author_email='zeguilhermelins@hotmail.com',
     keywords='fastapi starter',
     packages=['fastapi_starter'],
     python_requires='>=3.6',
     entry_points={
         "console_scripts": [
             "fastapi_starter=fastapi_starter.cli:main",
```

