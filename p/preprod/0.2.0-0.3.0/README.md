# Comparing `tmp/preprod-0.2.0.tar.gz` & `tmp/preprod-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprod-0.2.0.tar", max compression
+gzip compressed data, was "preprod-0.3.0.tar", max compression
```

## Comparing `preprod-0.2.0.tar` & `preprod-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2024-05-04 07:46:13.142433 preprod-0.2.0/LICENSE
--rw-r--r--   0        0        0      313 2024-05-26 18:08:54.806898 preprod-0.2.0/README.md
--rw-r--r--   0        0        0      144 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/__init__.py
--rw-r--r--   0        0        0     9742 2024-05-26 18:03:08.573887 preprod-0.2.0/preprod/commons.py
--rw-r--r--   0        0        0     4579 2024-05-26 17:09:10.902231 preprod-0.2.0/preprod/core.py
--rw-r--r--   0        0        0      424 2024-05-26 18:06:43.770894 preprod-0.2.0/preprod/locale/en/LC_MESSAGES/preprod.mo
--rw-r--r--   0        0        0      738 2024-05-04 07:46:13.144433 preprod-0.2.0/preprod/locale/en.po
--rw-r--r--   0        0        0     1480 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/locale/es/LC_MESSAGES/preprod.mo
--rw-r--r--   0        0        0     2662 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/locale/es.po
--rw-r--r--   0        0        0     2026 2024-05-26 18:08:54.806898 preprod-0.2.0/preprod/locale/preprod.pot
--rw-r--r--   0        0        0     1253 2024-05-21 19:06:48.612820 preprod-0.2.0/preprod/poethepoet.py
--rw-r--r--   0        0        0      167 2024-05-04 08:31:09.575065 preprod-0.2.0/preprod/tests/test_commons.py
--rw-r--r--   0        0        0      827 2024-05-26 18:08:54.807898 preprod-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 preprod-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-01 20:15:11.507022 preprod-0.3.0/LICENSE
+-rw-r--r--   0        0        0      517 2024-05-28 17:20:53.661343 preprod-0.3.0/README.md
+-rw-r--r--   0        0        0      144 2024-05-28 17:20:53.662343 preprod-0.3.0/preprod/__init__.py
+-rw-r--r--   0        0        0    11126 2024-05-28 08:41:05.649081 preprod-0.3.0/preprod/commons.py
+-rw-r--r--   0        0        0     4932 2024-05-28 17:13:07.735303 preprod-0.3.0/preprod/core.py
+-rw-r--r--   0        0        0      424 2024-05-28 17:16:19.884319 preprod-0.3.0/preprod/locale/en/LC_MESSAGES/preprod.mo
+-rw-r--r--   0        0        0      738 2023-10-13 06:59:07.290649 preprod-0.3.0/preprod/locale/en.po
+-rw-r--r--   0        0        0     2202 2024-05-28 17:16:19.871319 preprod-0.3.0/preprod/locale/es/LC_MESSAGES/preprod.mo
+-rw-r--r--   0        0        0     3400 2024-05-28 17:20:53.662343 preprod-0.3.0/preprod/locale/es.po
+-rw-r--r--   0        0        0     2489 2024-05-28 17:20:53.662343 preprod-0.3.0/preprod/locale/preprod.pot
+-rw-r--r--   0        0        0     1306 2024-05-28 17:13:07.735303 preprod-0.3.0/preprod/poethepoet.py
+-rw-r--r--   0        0        0     2175 2024-05-28 17:13:07.736303 preprod-0.3.0/preprod/tests/test_commons.py
+-rw-r--r--   0        0        0      831 2024-05-28 17:20:53.662343 preprod-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1039 1970-01-01 00:00:00.000000 preprod-0.3.0/PKG-INFO
```

### Comparing `preprod-0.2.0/LICENSE` & `preprod-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `preprod-0.2.0/preprod/commons.py` & `preprod-0.3.0/preprod/commons.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from colorama import Fore,  Style
 from gettext import translation
 from importlib.resources import files
-from os import getuid, path, listdir, remove, chdir as os_chdir, system  as os_system
+from os import getuid, path, listdir, remove, chdir as os_chdir, system  as os_system, makedirs as os_makedirs
 from shutil import copyfile as shutil_copyfile, rmtree as shutil_rmtree
 from socket import create_connection
 from subprocess import run
 from sys import exit, stdout
 
+"""
+    Each command should have these parameters
+    - description: (None: Doesn't show anything, "": Show default description, "something": "Shows something as description")
+
+"""
 
 
 try:
     t=translation('preprod', files("preprod") / 'locale')
     _=t.gettext
 except:
     _=str
@@ -31,14 +36,28 @@
 
 def press_a_key_to_continue():
     from preprod.core import concurrent_log
     concurrent_log("Before press a key to continue...")
     system("read -p '{0}'".format(_("Press a key to continue...")))
     concurrent_log("After press a key to continue...")
 
+def makedirs(dirname, description=""):
+    """
+        Create directories to last child. If it's already created ignores error
+    """
+    from preprod.core import concurrent_log
+    log=_("Created {0} directory").format(dirname)
+    description=log if description=="" else description
+    print_before(description, description is not None)
+    os_makedirs(dirname,  exist_ok=True)
+    concurrent_log(log)
+    print_after_ok(description is not None)
+    
+
+
 def nmcli_net_change(netname, check_host,  check_port, description=""):
     """
         Parameters:
             - netname with Networkmanager: str
             - ip to check: str or name
             - port to check: int
             - description="" Default description. None doesn't print anything
@@ -65,69 +84,55 @@
                     s=f"[Retrying {retry}]"
                     print("\b"*len(s)+ yellow(s),  end="")
                     stdout.flush()
                     retry+=1
 
 
 def replace_in_file(filename, s, r,description=""):
-    if description is not None:
-        print_before(_("Replacing values in {0}").format(filename))
+    description=_("Replacing values in {0}").format(filename) if description=="" else description
+    print_before(description, description is not None)
     data=open(filename,"r").read()
     remove(filename)
     data=data.replace(s,r)
     with open(filename, "w") as f:
         f.write(data)
-    
-    if description is not None:
-        print_after_ok()
+    print_after_ok(description is not None)
     from preprod.core import concurrent_log
     concurrent_log(f"Replaced in file '{filename}', '{s}' by '{r}'")
 
 def lines_at_the_end_of_file(filename, s, description=""):
-    if description is not None:
-        print_before(_("Appending text at the end of {0}").format(filename))
+    print_before(_("Appending text at the end of {0}").format(filename), description is not None)
     with open(filename, 'a') as f:
         f.write(s)
-    if description is not None:
-        print_after_ok()
+    print_after_ok(description is not None)
     from preprod.core import concurrent_log
     concurrent_log(f"Added at the of file '{filename}'", s)
 
-def run_and_check(command,  description=None,  expected_returncode=0,  expected_stdout=None):
+def run_and_check(command,  description="",  expected_returncode=0,  expected_stdout=None):
     """
         Executes a comand and returns a boolean if command was executed as expected
-        
-        Parameters:
-            - verbose. If true shows stdout and stderr
-            - description. None makes not output, "" print command, else prints else
     """
-    if description is not None:
-        if description=="":
-            description=command
-        
-        print (f"  - {description} ",  end="")
-        stdout.flush()
+    description=_("Running '{0}'").format(command) if description=="" else description
+    print_before(description, description is not None)
     
     p=run(command, shell=True, capture_output=True)
     
     #Check if process is valid
     r=False
     if expected_stdout is not None:
         print(expected_stdout, )
         r= expected_stdout in p.stdout.decode('utf-8')
         r=True
     elif p.returncode==expected_returncode:
         r=True
     
-        
-    if description is not None:
-        if r is True:
-            print (f"[{green('OK')}]")
-        else:
-            print (f"[{red('ERROR')}]")
+    if r is True:
+        print_after_ok(description is not None)
+    else:
+        print_after_error(description is not None)
             
     from preprod.core import concurrent_log
     stdout_=p.stdout.decode('utf-8')
     stderr_=p.stderr.decode('utf-8')
     concurrent_log(f"run_and_check('{command}')",  stdout_, stderr_)
 
     return r
@@ -141,17 +146,23 @@
     if show:
         print (f"[{green('OK')}]")
 
 def print_after_error(show=True):
     if show:
         print (f"[{red('ERROR')}]")
 
-def system(command):
+def system(command, description=""):
+    """
+        Runs a command with system
+    """
+    log=_("Running with system '{0}'").format(command) 
+    description=log if description=="" else description
+    print_before(description, description is not None)
     from preprod.core import concurrent_log
-    concurrent_log(f"system('{command}')")
+    concurrent_log(log)
     os_system(command)
 
 def rmtree(directory, show=True):
     print_before(_("Deleting directory {0}").format(directory),show)
     shutil_rmtree(directory, ignore_errors=True)
     print_after_ok(show)
     from preprod.core import concurrent_log
@@ -160,19 +171,21 @@
 def chdir(directory, show=True):
     from preprod.core import concurrent_log
     print_before(_("Changing to directory {0}").format(directory),show)
     concurrent_log(f"chdir('{directory}')")
     os_chdir(directory)
     print_after_ok(show)
 
-def git_clone(url):
-    run_and_check(f"git clone {url}", description=f"Cloning git repository {url}")
-
-def git_pull():
-    run_and_check("git pull", description="Pulling git repository")
+def git_clone(url,  output_directory="", description=""):
+    description=_("Cloning git repository {0}").format(url) if description=="" else description
+    run_and_check(f"git clone {url} {output_directory}", description=description)
+
+def git_pull(description=""):    
+    description=_("Pulling git repository") if description=="" else description
+    run_and_check("git pull", description=description)
 
 def insert_at_line(file_path, line_number, text, description=""):
     """
         Parameters
           - line_number is the number of lines not a zero-based index
           - text must be the content of a line without \n
     """
@@ -276,30 +289,33 @@
         Parameters:
            - python_version_name: str: python3.11
     """
     str_sss="--system-site-packages" if system_site_packages else ""
     run_and_check(f"{python_version_name} -m venv {str_sss} .{python_version_name}", description= f"Creating virtual env at .{python_version_name}")
     return path.abspath(".python3.11/bin/python3"), path.abspath(".python3.11/bin/pip")
 
-def apache_initd_restart():
-    run_and_check("/etc/init.d/apache2 restart", "Restarting apache server")
-    
-def chown_recursive(path,  user="root",  group="root"):
-    run_and_check(f"find {path} -type f -exec chown -R {user}:{group} {{}} +")
-
-def chmod_recursive(path,  directory_permissions="755",  file_permissions="644" ):
-    run_and_check(f"find {path} -type d -exec chmod -R {directory_permissions} {{}} +")
-    run_and_check(f"find {path} -type f -exec chmod -R {file_permissions} {{}} +")
+def apache_initd_restart(description=""):
+    description=_("Restarting apache server") if description=="" else description
+    run_and_check("/etc/init.d/apache2 restart", description)
+    
+def chown_recursive(path,  user="root",  group="root", description=""):
+    description=_("Changing '{0}' to owner {1}:{2}").format(path, user,  group) if description=="" else description
+    run_and_check(f"find {path} -type f -exec chown -R {user}:{group} {{}} +", description)
+
+def chmod_recursive(path,  directory_permissions="755",  file_permissions="644",  description=""):
+    description=_("Changing directories permissions to {0} and files to {1}").format(directory_permissions, file_permissions) if description=="" else description
+    run_and_check(f"find {path} -type d -exec chmod -R {directory_permissions} {{}} +", None)
+    run_and_check(f"find {path} -type f -exec chmod -R {file_permissions} {{}} +", description)
 
-def npm_install():
-    run_and_check("npm install")
+def npm_install(description=""):
+    run_and_check("npm install", description)
     
-def rsync(from_,  to_,  delete_after=False):
+def rsync(from_,  to_,  delete_after=False, description=""):
     str_delete_after="--delete-after" if delete_after else ""
-    run_and_check(f"rsync -avzPH {from_} {to_} {str_delete_after}")
+    run_and_check(f"rsync -avzPH {from_} {to_} {str_delete_after}", description)
     
-def poetry_install():
-    run_and_check("poetry install")
+def poetry_install(description=""):
+    run_and_check("poetry install", description)
     
 def poetry_env_info():
     p=run("poetry env info -e", shell=True, capture_output=True)
     return p.stdout.decode('utf-8')
```

### Comparing `preprod-0.2.0/preprod/core.py` & `preprod-0.3.0/preprod/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-#!/usr/bin/python3
 from argparse import ArgumentParser
 from datetime import datetime
 from gettext import translation
 from importlib.resources import files
 from multiprocessing import Lock
 from os import path, makedirs
 from preprod import commons
 from sys import exit
-
+from preprod import __version__, __versiondate__
 
 try:
     t=translation('preprod', files("preprod") / 'locale')
     _=t.gettext
 except:
     _=str
 
+def argparse_epilog():
+    return _("Developed by Mariano Muñoz 2023-{}").format(__versiondate__.year)
 
 def concurrent_log(title, stdout=None,  stderr=None):
     def parse_std(std):
         arr=std.split("\n")
         r=""
         for line in arr:
             r+=f"      {line}\n"
@@ -30,35 +31,39 @@
             f.write(commons.yellow(f"{datetime.now()} [{args.project}/{args.action}] {title}\n"))
             if stdout!="" and stdout is not None:
                 f.write(commons.green("      STDOUT\n"))
                 f.write(parse_std(stdout))
             if stderr!="" and stderr is not None:
                 f.write(commons.red("      STDERR\n"))
                 f.write(parse_std(stderr))
-            
-def main():
+
+## If arguments is None, launches with sys.argc parameters. Entry point is toomanyfiles:main
+## You can call with main(['--pretend']). It's equivalento to os.system('program --pretend')
+## @param arguments is an array with parser arguments. For example: ['--argument','9'].
+def main(arguments=None):
     global lock
     lock=Lock()
-
-    parser=ArgumentParser(description=_("ProPred manager"))
+    
+    global args
+    parser=ArgumentParser(description=_("Preprod manager"), epilog= argparse_epilog())
+    parser.add_argument('--version', action='version', version=__version__)
     parser.add_argument('--pretend', default=False, help=_("Prints action code without running it"),  action='store_true')
 
-    parser.add_argument('project',nargs='?', default=None, help=_("Project identification"),  action='store')
-    parser.add_argument('action',nargs='?', default=None, help=_("Action identification"),  action='store')
+    parser.add_argument('project', nargs='?', default=None, help=_("Project identification"),  action='store')
+    parser.add_argument('action', nargs='?', default=None, help=_("Action identification"),  action='store')
 
-    global args
-    args=parser.parse_args()
+    args=parser.parse_args(arguments)
     
     commons.check_repository_path(verbose=True)
     repository_path=commons.repository_path()
     project_path=f"{repository_path}/{args.project}/"
     action_path=f"{project_path}/{args.action}"
     
     if args.project is None and args.action is None:
-        list()
+        list_repository()
         exit(10)
     
 
     print(commons.yellow(_("Reading repository from {0}").format(repository_path)))
     if not (args.project and path.exists(project_path)):
         print(commons.red(_("Project wasn't found in {0}").format(project_path)))
         exit(5)
@@ -89,15 +94,16 @@
             print(commons.white(_("Executing project '{0}' and action '{1}'").format(args.project,  args.action)))
             exec(commands)
             print(commons.white(_("Executed project '{0}' and action '{1}' took {2}").format(args.project,  args.action, datetime.now()-start)))
 
 
 def create():
 
-    parser=ArgumentParser(description=_("ProPre manager"))
+    parser=ArgumentParser(description=_("Preprod manager"), epilog= argparse_epilog())
+    parser.add_argument('--version', action='version', version=__version__)
     parser.parse_args()
     
     if commons.check_repository_path():
         print(_("Repository already created in {}").format(commons.repository_path()))
         exit(6)
     rp=commons.repository_path()
     
@@ -117,26 +123,18 @@
     print("I'm root")
 else:
     print("I'm a normal user")
 repository_commons.foo()
 
 """)
 
-def list():
-
-    parser=ArgumentParser(description=_("ProPre manager"))    
-    parser.add_argument('--repository_commons', default=False, help=_("Shows repository_commons.py file in repository pathh"),  action='store_true')
-
-    args=parser.parse_args()
-    
+def list_repository():
     commons.check_repository_path(verbose=True)
     rp=commons.repository_path()
     print(commons.yellow(_("Reading repository from {0} and listing available preprod scripts").format(rp)))
 
-    if args.repository_commons:
-        with open(f"{rp}/repository_commons.py", "r") as f:
-            print(f.read())
-            exit(0)
-        
+    dictionary_=commons.dictionary_project_actions()
+    ordered_values=list(dictionary_.keys())
+    ordered_values.sort()
 
-    for key, value in commons.dictionary_project_actions().items():
-        print(commons.white(key), commons.green(str(value)))
+    for key in ordered_values:
+        print(commons.white(key), commons.green(str(dictionary_[key])))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `preprod-0.2.0/preprod/locale/en.po` & `preprod-0.3.0/preprod/locale/en.po`

 * *Files identical despite different names*

### Comparing `preprod-0.2.0/preprod/locale/es/LC_MESSAGES/preprod.mo` & `preprod-0.3.0/preprod/locale/es/LC_MESSAGES/preprod.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -11,42 +11,69 @@
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Lokalize 19.12.3\n"
 
 msgid "Action identification"
 msgstr "Identificación de la acción"
 
+msgid "Action wasn't found in {0}"
+msgstr "La acción no fue encontrada en {0}"
+
 msgid "Appending text at the end of {0}"
 msgstr "Añadiendo texto al final de {0}"
 
 msgid "Changing net to {0}"
 msgstr "Cambiando red a {0}"
 
 msgid "Changing to directory {0}"
 msgstr "Cambiando a directorio {0}"
 
+msgid "Created {0} directory"
+msgstr "Directorio {0} creado"
+
 msgid "Deleting directory {0}"
-msgstr "Borarando directorio {0}"
+msgstr "Borrando directorio {0}"
+
+msgid "Executed project '{0}' and action '{1}' took {2}"
+msgstr "La ejecución del proyecto '{0}' y acción '{1}' tardó {2}"
+
+msgid "Executing project '{0}' and action '{1}'"
+msgstr "Ejecutando proyecto '{0}' y la acción '{1}'"
 
 msgid "Line number is out of range"
 msgstr "El número de línea está fuera de rango"
 
+msgid "Preprod manager"
+msgstr "Gestor Preprod"
+
 msgid "Press a key to continue..."
 msgstr "Pulsa una tecla para continuar..."
 
 msgid "Prints action code without running it"
 msgstr "Muestra el código de la acción sin ejecutarlo"
 
 msgid "Project identification"
 msgstr "Identificación del proyecto"
 
 msgid "Project wasn't found in {0}"
 msgstr "El proyecto no fue encontrado en {0}"
 
+msgid "Reading repository from {0}"
+msgstr "Leyendo el repository de {0}"
+
 msgid "Replacing values in {0}"
 msgstr "Remplazando valores en {0}"
 
 msgid "Repository already created in {}"
 msgstr "El repositorio ya está creado en {}"
 
+msgid "Restarting apache server"
+msgstr "Reiniciando el servidor Apache"
+
+msgid "Running '{0}'"
+msgstr "Ejecutando '{0}'"
+
+msgid "Running with system '{0}'"
+msgstr "Ejecutando con system '{0}'"
+
 msgid "You must create repository path"
 msgstr "Debe crear el directory del repositorio"
```

### Comparing `preprod-0.2.0/preprod/locale/es.po` & `preprod-0.3.0/preprod/locale/es.po`

 * *Files 18% similar despite different names*

```diff
@@ -4,102 +4,129 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # root <turulomio@yahoo.es>, 2015, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: TooManyFiles\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-26 20:05+0200\n"
+"POT-Creation-Date: 2024-05-28 19:16+0200\n"
 "PO-Revision-Date: 2020-04-03 08:54+0200\n"
 "Last-Translator: trabajo <turulomio@yahoo.es>\n"
 "Language-Team: Spanish <kde-i18n-doc@kde.org>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Lokalize 19.12.3\n"
 
 msgid "Press a key to continue..."
 msgstr "Pulsa una tecla para continuar..."
 
 #, python-brace-format
+msgid "Created {0} directory"
+msgstr "Directorio {0} creado"
+
+#, python-brace-format
 msgid "Changing net to {0}"
 msgstr "Cambiando red a {0}"
 
 #, python-brace-format
 msgid "Replacing values in {0}"
 msgstr "Remplazando valores en {0}"
 
 #, python-brace-format
 msgid "Appending text at the end of {0}"
 msgstr "Añadiendo texto al final de {0}"
 
 #, python-brace-format
+msgid "Running '{0}'"
+msgstr "Ejecutando '{0}'"
+
+#, python-brace-format
+msgid "Running with system '{0}'"
+msgstr "Ejecutando con system '{0}'"
+
+#, python-brace-format
 msgid "Deleting directory {0}"
-msgstr "Borarando directorio {0}"
+msgstr "Borrando directorio {0}"
 
 #, python-brace-format
 msgid "Changing to directory {0}"
 msgstr "Cambiando a directorio {0}"
 
 #, python-brace-format
+msgid "Cloning git repository {0}"
+msgstr ""
+
+msgid "Pulling git repository"
+msgstr ""
+
+#, python-brace-format
 msgid "Insert text at line {0} in {1}"
 msgstr ""
 
 msgid "Line number is out of range"
 msgstr "El número de línea está fuera de rango"
 
 #, python-brace-format
 msgid "Deleting line {0} in {1}"
 msgstr ""
 
 msgid "You must create repository path"
 msgstr "Debe crear el directory del repositorio"
 
-msgid "ProPred manager"
+msgid "Restarting apache server"
+msgstr "Reiniciando el servidor Apache"
+
+#, python-brace-format
+msgid "Changing '{0}' to owner {1}:{2}"
 msgstr ""
 
+#, python-brace-format
+msgid "Changing directories permissions to {0} and files to {1}"
+msgstr ""
+
+msgid "Developed by Mariano Muñoz 2023-{}"
+msgstr ""
+
+msgid "Preprod manager"
+msgstr "Gestor Preprod"
+
 msgid "Prints action code without running it"
 msgstr "Muestra el código de la acción sin ejecutarlo"
 
 msgid "Project identification"
 msgstr "Identificación del proyecto"
 
 msgid "Action identification"
 msgstr "Identificación de la acción"
 
 #, python-brace-format
 msgid "Reading repository from {0}"
-msgstr ""
+msgstr "Leyendo el repository de {0}"
 
 #, python-brace-format
 msgid "Project wasn't found in {0}"
 msgstr "El proyecto no fue encontrado en {0}"
 
 #, python-brace-format
 msgid "Action wasn't found in {0}"
-msgstr ""
+msgstr "La acción no fue encontrada en {0}"
 
 #, python-brace-format
 msgid "Executing project '{0}' and action '{1}'"
-msgstr ""
+msgstr "Ejecutando proyecto '{0}' y la acción '{1}'"
 
 #, python-brace-format
 msgid "Executed project '{0}' and action '{1}' took {2}"
-msgstr ""
-
-msgid "ProPre manager"
-msgstr ""
+msgstr "La ejecución del proyecto '{0}' y acción '{1}' tardó {2}"
 
 msgid "Repository already created in {}"
 msgstr "El repositorio ya está creado en {}"
 
-msgid "Shows repository_commons.py file in repository pathh"
-msgstr ""
-
 #, python-brace-format
 msgid "Reading repository from {0} and listing available preprod scripts"
 msgstr ""
 
 #~ msgid "Exiting propred..."
 #~ msgstr "Saliendo de propred..."
```

### Comparing `preprod-0.2.0/preprod/locale/preprod.pot` & `preprod-0.3.0/preprod/locale/preprod.pot`

 * *Files 9% similar despite different names*

```diff
@@ -4,61 +4,94 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-05-26 20:06+0200\n"
+"POT-Creation-Date: 2024-05-28 19:16+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=CHARSET\n"
+"Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "Press a key to continue..."
 msgstr ""
 
 #, python-brace-format
+msgid "Created {0} directory"
+msgstr ""
+
+#, python-brace-format
 msgid "Changing net to {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Replacing values in {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Appending text at the end of {0}"
 msgstr ""
 
 #, python-brace-format
+msgid "Running '{0}'"
+msgstr ""
+
+#, python-brace-format
+msgid "Running with system '{0}'"
+msgstr ""
+
+#, python-brace-format
 msgid "Deleting directory {0}"
 msgstr ""
 
 #, python-brace-format
 msgid "Changing to directory {0}"
 msgstr ""
 
 #, python-brace-format
+msgid "Cloning git repository {0}"
+msgstr ""
+
+msgid "Pulling git repository"
+msgstr ""
+
+#, python-brace-format
 msgid "Insert text at line {0} in {1}"
 msgstr ""
 
 msgid "Line number is out of range"
 msgstr ""
 
 #, python-brace-format
 msgid "Deleting line {0} in {1}"
 msgstr ""
 
 msgid "You must create repository path"
 msgstr ""
 
-msgid "ProPred manager"
+msgid "Restarting apache server"
+msgstr ""
+
+#, python-brace-format
+msgid "Changing '{0}' to owner {1}:{2}"
+msgstr ""
+
+#, python-brace-format
+msgid "Changing directories permissions to {0} and files to {1}"
+msgstr ""
+
+msgid "Developed by Mariano Muñoz 2023-{}"
+msgstr ""
+
+msgid "Preprod manager"
 msgstr ""
 
 msgid "Prints action code without running it"
 msgstr ""
 
 msgid "Project identification"
 msgstr ""
@@ -82,19 +115,13 @@
 msgid "Executing project '{0}' and action '{1}'"
 msgstr ""
 
 #, python-brace-format
 msgid "Executed project '{0}' and action '{1}' took {2}"
 msgstr ""
 
-msgid "ProPre manager"
-msgstr ""
-
 msgid "Repository already created in {}"
 msgstr ""
 
-msgid "Shows repository_commons.py file in repository pathh"
-msgstr ""
-
 #, python-brace-format
 msgid "Reading repository from {0} and listing available preprod scripts"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `preprod-0.2.0/preprod/poethepoet.py` & `preprod-0.3.0/preprod/poethepoet.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   * Cambiar la versión y la fecha en __init__.py
   * Editar README.md to add CHANGELOG
   * Ejecutar otra vez poe release
   * git checkout -b preprod-{0}
   * poe translate
   * linguist
   * poe translate
-  * poe test
+  * poe coverage
   * git commit -a -m 'preprod-{0}'
   * git push --set-upstream origin preprod-{0}
   * Hacer un pull request con los cambios a main
   * Hacer un nuevo tag en GitHub
   * git checkout main
   * git pull
   * poetry build
@@ -23,18 +23,19 @@
   * Crea un nuevo ebuild de preprod en Gentoo con la nueva versión
   * Subelo al repositorio myportage
 
 """.format(__version__))
 
     
 def coverage():
-    system("coverage run --omit='*uno.py' -m pytest && coverage report && coverage html")
+    system("coverage run --omit='*repository_commons.py' -m pytest && coverage report && coverage html")
 
 
 def translate():
     #es
     system("xgettext -L Python --no-wrap --no-location --from-code='UTF-8' -o preprod/locale/preprod.pot preprod/*.py")
     system("msgmerge -N --no-wrap -U preprod/locale/es.po preprod/locale/preprod.pot")
     system("msgfmt -cv -o preprod/locale/es/LC_MESSAGES/preprod.mo preprod/locale/es.po")
     system("msgfmt -cv -o preprod/locale/en/LC_MESSAGES/preprod.mo preprod/locale/en.po")
     
-
+def pytest():
+    system("pytest")
```

### Comparing `preprod-0.2.0/pyproject.toml` & `preprod-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "preprod"
-version = "0.2.0"
+version = "0.3.0"
 description = "Easily creation of pre-production and production scripts to automete your deployment"
 authors = ["turulomio <turulomio@yahoo.es>"]
 license = "GPL-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -23,10 +23,10 @@
 
 [tool.poetry.scripts]
 preprod='preprod.core:main'
 preprod_create_repository='preprod.core:create'
 
 [tool.poe.tasks]
 coverage = { script = "preprod.poethepoet:coverage" }
-test = { script = "preprod.poethepoet:test" }
+pytest = { script = "preprod.poethepoet:pytest" }
 release = { script = "preprod.poethepoet:release" }
 translate = { script = "preprod.poethepoet:translate" }
```

### Comparing `preprod-0.2.0/PKG-INFO` & `preprod-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprod
-Version: 0.2.0
+Version: 0.3.0
 Summary: Easily creation of pre-production and production scripts to automete your deployment
 License: GPL-3
 Author: turulomio
 Author-email: turulomio@yahoo.es
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,13 +14,20 @@
 Description-Content-Type: text/markdown
 
 # preprod
 Easily creation of pre-production and production scripts to automete your deployment
 
 ## Changelog
 
+### 0.3.0 (2024-05-28(
+- Improved description system
+- Added makedirs and git clone in different directory
+- Improved spanish translations
+- Added --version to commands
+- Added test with a 84% coverture
+
 ### 0.2.0 (2024-05-26)
 - Added logs in /tmp/preprod_logs/
 - Added chown_recursive, chmod_recursive, rsync, poetry_install, poetry_env_info methods to commons
 
 ### 0.1.0 (2024-05-21)
 - Basic functionality
```

