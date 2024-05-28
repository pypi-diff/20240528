# Comparing `tmp/falco_cli-0.8.0.tar.gz` & `tmp/falco_cli-0.9.0.tar.gz`

## Comparing `falco_cli-0.8.0.tar` & `falco_cli-0.9.0.tar`

### file list

```diff
@@ -1,225 +1,141 @@
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.all-contributorsrc
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.editorconfig
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.gitmodules
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 falco_cli-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 falco_cli-0.8.0/all-contributorsrc
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.github/workflows/pre-commit-auto-update.yml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.vscode/settings.json
--rw-r--r--   0        0        0   370518 2020-02-02 00:00:00.000000 falco_cli-0.8.0/assets/falco-logo.svg
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/.git
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/LICENSE
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/README.md
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/cookiecutter.json
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/.github/workflows/pre-commit-auto-update.yml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/.env.template
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/.gitignore
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/README.md
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/manage.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/playground.ipynb
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/.github/dependabot.yml
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/.github/workflows/ci.yml
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/create.html
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/detail.html
--rw-r--r--   0        0        0     6670 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/list.html
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/update.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/config/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/config/asgi.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/config/settings.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/config/urls.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/config/wsgi.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/deploy/Dockerfile
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/deploy/entrypoint.sh
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/deploy/gunicorn.conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/tests/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/tests/test_assert_true.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/core/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/core/apps.py
--rw-r--r--   0        0        0    47108 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/static/vendors/htmx/htmx.min.js
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/403.html
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/403_csrf.html
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/404.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/500.html
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/base.html
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/base_email.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/pages/about.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/pages/home.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/__init__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/admin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/apps.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/forms.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/models.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/migrations/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/.git
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/LICENSE
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/README.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/.github/workflows/ci.yml
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/.env.template
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/.gitignore
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/README.md
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/manage.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/playground.ipynb
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/pyproject.toml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/.github/dependabot.yml
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/config/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/config/asgi.py
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/config/settings.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/config/urls.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/config/wsgi.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/deploy/Dockerfile
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/deploy/entrypoint.sh
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/deploy/gunicorn.conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/tests/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/tests/test_assert_true.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/core/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/core/apps.py
--rw-r--r--   0        0        0    47108 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/static/vendors/htmx/htmx.min.js
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/base.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/templates/home.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/__init__.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/admin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/apps.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/forms.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/models.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/blueprints/falco_blueprint_basic_bootstrap/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/migrations/__init__.py
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/manage.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/config/__init__.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/config/asgi.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/config/settings.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/config/urls.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/config/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/core/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/core/apps.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/core/types.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/orders/__init__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/orders/apps.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/orders/models.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/orders/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/orders/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/admin.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/apps.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/forms.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/models.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/tests.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/urls.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/views.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/products/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/users/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/users/admin.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/users/apps.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/users/models.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/users/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/demo/users/migrations/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/templates/base.html
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/templates/products/product_create.html
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/templates/products/product_detail.html
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/templates/products/product_list.html
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 falco_cli-0.8.0/demo/templates/products/product_update.html
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/.rich-codex.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/Makefile
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/changelog.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/codeofconduct.rst
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/conf.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/contributing.rst
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/index.rst
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/install.rst
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/license.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/make.bat
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/_static/custom.css
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/_templates/partials/globaltoc-above.html
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/avoiding_god_models.rst
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/database_tips.rst
--rw-r--r--   0        0        0    30470 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/deployment.rst
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/dynamic_model_schema.rst
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/index.rst
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/interactive_user_interfaces.rst
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/logging_and_monitoring.rst
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/multitenancy.rst
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/optimizing_database_access.rst
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/permissions_and_authorization.rst
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/realtime.rst
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/running_project_in_a_container.rst
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/task_queues_and_schedulers.rst
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/tips_and_extra.rst
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/use_sqlite_in_production.rst
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/writing_async_code.rst
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/writing_documentation.rst
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/guides/writing_tests.rst
--rw-r--r--   0        0        0   235559 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/images/deployment.png
--rw-r--r--   0        0        0   370845 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/images/logo_with_text.svg
--rw-r--r--   0        0        0    41281 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/images/project-tree.svg
--rw-r--r--   0        0        0   186221 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/images/task_queue.png
--rw-r--r--   0        0        0    10400 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/crud.rst
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/htmx.rst
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/index.rst
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/migrations.rst
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/setup_admin.rst
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/start_app.rst
--rw-r--r--   0        0        0    23646 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/start_project.rst
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/sync_dotenv.rst
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/usage.rst
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 falco_cli-0.8.0/docs/the_cli/work.rst
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 falco_cli-0.8.0/scripts/project_tree.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 falco_cli-0.8.0/scripts/update_readme_guides.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/__about__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/__main__.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/utils.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/checks.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/htmx.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/htmx_extension.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/reset_migrations.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/rm_migrations.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/setup_admin.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/start_app.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/start_project.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/sync_dotenv.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/work.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/crud/__init__.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/crud/install_crud_utils.py
--rw-r--r--   0        0        0    18458 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/crud/model_crud.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/commands/crud/utils.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/html/create.html
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/html/detail.html
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/html/list.html
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/html/update.html
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/python/forms.py.jinja
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/python/views.py.jinja
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/utils/types.py.jinja
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 falco_cli-0.8.0/src/falco/crud/utils/utils.py.jinja
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_crud.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_htmx.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_htmx_extension.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_install_crud_utils.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_reset_migrations.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_rm_migrations.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_setup_admin.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_start_app.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_start_project.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 falco_cli-0.8.0/tests/commands/test_sync_dotenv.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 falco_cli-0.8.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 falco_cli-0.8.0/LICENSE
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 falco_cli-0.8.0/README.md
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 falco_cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 falco_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.all-contributorsrc
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.editorconfig
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.gitmodules
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 falco_cli-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 falco_cli-0.9.0/all-contributorsrc
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.github/workflows/pre-commit-auto-update.yml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0   370518 2020-02-02 00:00:00.000000 falco_cli-0.9.0/assets/falco-logo.svg
+-rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/manage.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/config/__init__.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/config/asgi.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/config/settings.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/config/urls.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/config/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/core/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/core/apps.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/core/types.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/orders/__init__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/orders/apps.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/orders/models.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/orders/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/orders/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/admin.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/apps.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/forms.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/models.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/tests.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/urls.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/views.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/products/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/users/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/users/admin.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/users/apps.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/users/models.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/demo/users/migrations/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/templates/base.html
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/templates/products/product_create.html
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/templates/products/product_detail.html
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/templates/products/product_list.html
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 falco_cli-0.9.0/demo/templates/products/product_update.html
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/.rich-codex.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/changelog.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/codeofconduct.rst
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/contributing.rst
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/install.rst
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/license.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/_static/custom.css
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/_templates/partials/globaltoc-above.html
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/avoiding_god_models.rst
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/database_tips.rst
+-rw-r--r--   0        0        0    30470 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/deployment.rst
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/dynamic_model_schema.rst
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/index.rst
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/interactive_user_interfaces.rst
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/logging_and_monitoring.rst
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/multitenancy.rst
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/optimizing_database_access.rst
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/permissions_and_authorization.rst
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/realtime.rst
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/running_project_in_a_container.rst
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/task_queues_and_schedulers.rst
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/tips_and_extra.rst
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/use_sqlite_in_production.rst
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/writing_async_code.rst
+-rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/writing_documentation.rst
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/guides/writing_tests.rst
+-rw-r--r--   0        0        0   235559 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/images/deployment.png
+-rw-r--r--   0        0        0   370845 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/images/logo_with_text.svg
+-rw-r--r--   0        0        0    41281 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/images/project-tree.svg
+-rw-r--r--   0        0        0   186221 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/images/task_queue.png
+-rw-r--r--   0        0        0    12422 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/crud.rst
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/htmx.rst
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/index.rst
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/migrations.rst
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/setup_admin.rst
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/start_app.rst
+-rw-r--r--   0        0        0    23646 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/start_project.rst
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/sync_dotenv.rst
+-rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/usage.rst
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 falco_cli-0.9.0/docs/the_cli/work.rst
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 falco_cli-0.9.0/scripts/project_tree.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 falco_cli-0.9.0/scripts/update_readme_guides.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/__about__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/__main__.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/config.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/utils.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/checks.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/htmx.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/htmx_extension.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/reset_migrations.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/rm_migrations.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/setup_admin.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/start_app.py
+-rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/start_project.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/sync_dotenv.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/work.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/crud/__init__.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/crud/install_crud_utils.py
+-rw-r--r--   0        0        0    19348 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/crud/model_crud.py
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/commands/crud/utils.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/html/create.html
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/html/detail.html
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/html/list.html
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/html/update.html
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/python/forms.py.jinja
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/python/views.py.jinja
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/utils/types.py.jinja
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 falco_cli-0.9.0/src/falco/crud/utils/utils.py.jinja
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_crud.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_htmx.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_htmx_extension.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_install_crud_utils.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_reset_migrations.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_rm_migrations.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_setup_admin.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_start_app.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_start_project.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 falco_cli-0.9.0/tests/commands/test_sync_dotenv.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 falco_cli-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 falco_cli-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 falco_cli-0.9.0/README.md
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 falco_cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 falco_cli-0.9.0/PKG-INFO
```

### Comparing `falco_cli-0.8.0/.all-contributorsrc` & `falco_cli-0.9.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/.pre-commit-config.yaml` & `falco_cli-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/CODE_OF_CONDUCT.md` & `falco_cli-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/.github/workflows/documentation.yml` & `falco_cli-0.9.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/.github/workflows/pre-commit-auto-update.yml` & `falco_cli-0.9.0/.github/workflows/pre-commit-auto-update.yml`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/.github/workflows/publish.yml` & `falco_cli-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/assets/falco-logo.svg` & `falco_cli-0.9.0/assets/falco-logo.svg`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/LICENSE` & `falco_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/.gitignore` & `falco_cli-0.9.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -124,9 +124,13 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
-# Pycharm
+.DS_Store
 .idea/
+.idea/sonarlint/
+
+
+test_projects/
```

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/manage.py` & `falco_cli-0.9.0/demo/manage.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import sys
 
 
 def main():
     """Run administrative tasks."""
     os.environ.setdefault("DJANGO_SETTINGS_MODULE", "config.settings")
     try:
-        from django.core.management import (  # pylint: disable=import-outside-toplevel
-            execute_from_command_line,
-        )
+        from django.core.management import execute_from_command_line
     except ImportError as exc:
         raise ImportError(
             "Couldn't import Django. Are you sure it's installed and "
             "available on your PYTHONPATH environment variable? Did you "
             "forget to activate a virtual environment?"
         ) from exc
     execute_from_command_line(sys.argv)
```

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/create.html` & `falco_cli-0.9.0/src/falco/crud/html/create.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {% raw %}
 {% extends "base.html" %}
 {% load crispy_forms_tags %}
 
-{% block content %}
+{% block main_content %}
 {% endraw %}
     <h1 class="text-lg font-bold py-4">Create {{ model_name }}</h1>
 
     {% raw %}
 
     <form method="post">
         {% csrf_token %}
         {{form|crispy}}
 
         <button type="submit" class="cursor-pointer py-2 px-4 bg-blue-600 hover:bg-blue-700 focus:ring-blue-500 focus:ring-offset-blue-200 text-white text-center text-base font-semibold focus:outline-none focus:ring-2 focus:ring-offset-2  rounded-lg">
             Save
         </button>
     </form>
-{% endblock content %}
+{% endblock main_content %}
 {% endraw %}
```

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/detail.html` & `falco_cli-0.9.0/src/falco/crud/html/detail.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% raw %}
 {% extends "base.html" %}
 
-{% block content %}
+{% block main_content %}
 
     <section class="flex justify-between">
 {% endraw %}
         <h1 class="text-lg font-bold">{{ model_name}} - {% raw %}{{ {% endraw %} {{ model_name|lower }} {% raw %} }}{% endraw %} </h1>
 
         <a href="{{list_view_url|safe}}" class="text-blue-600 hover:underline hover:text-blue-500">
             All {{model_verbose_name_plural|capitalize}}
@@ -21,9 +21,9 @@
     </ul>
 
 
     <a class="py-2 px-4 bg-blue-600 hover:bg-blue-700 focus:ring-blue-500 focus:ring-offset-blue-200 text-white text-center text-base font-semibold focus:outline-none focus:ring-2 focus:ring-offset-2  rounded-lg"
        href="{{ update_view_url|safe }}">Edit</a>
 
 {% raw %}
-{% endblock content %}
+{% endblock main_content %}
 {% endraw %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% raw %} {% extends "base.html" %} {% block content %} {% endraw %}
+{% raw %} {% extends "base.html" %} {% block main_content %} {% endraw %}
 ************ {{{{ mmooddeell__nnaammee}}}} -- {{%% rraaww %%}}{{{{ {{%% eennddrraaww %%}} {{{{ mmooddeell__nnaammee||lloowweerr }}}} {{%% rraaww
 %%}} }}}}{{%% eennddrraaww %%}} ************
 _A_l_l_ _{_{_m_o_d_e_l___v_e_r_b_o_s_e___n_a_m_e___p_l_u_r_a_l_|_c_a_p_i_t_a_l_i_z_e_}_}
     * {% for field_verbose_name, field_accessor in
       fields_verbose_name_with_accessor.items() %}
     * {{ field_verbose_name }}: {{ field_accessor }}
     * {% endfor %}
-_E_d_i_t {% raw %} {% endblock content %} {% endraw %}
+_E_d_i_t {% raw %} {% endblock main_content %} {% endraw %}
```

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/list.html` & `falco_cli-0.9.0/src/falco/crud/html/list.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% raw %}
 {% extends 'base.html' %}
 {% load partials %}
 
 
-{% block content %}
+{% block main_content %}
 {% endraw %}
     <section class="flex justify-between">
         <h1 class="text-lg font-bold">{{ model_verbose_name_plural|capitalize }}</h1>
 
         <a href="{{ create_view_url|safe }}"
            class="cursor-pointer py-2 px-4 bg-blue-600 hover:bg-blue-700 focus:ring-blue-500 focus:ring-offset-blue-200 text-white text-center text-base font-semibold focus:outline-none focus:ring-2 focus:ring-offset-2 rounded-lg">
             New {{ model_name|capitalize }}
@@ -33,15 +33,15 @@
                                     {% endfor %}
                                 </tr>
                             {% raw %}
                             {% endwith %}
                         </thead>
                         <tbody>
                             {% with td_class="px-6 py-4 whitespace-nowrap text-sm font-medium border-r text-gray-900" %}
-                                {% for {% endraw %} {{ model_name|lower }} in {{model_name|lower}}s_page {% raw %} %}
+                                {% for {% endraw %}{{ model_name|lower }} in {{model_name|lower}}s_page {% raw %} %}
                                   {% endraw %}
                                     <tr class="border">
                                         {% for _, field_accessor in fields_verbose_name_with_accessor.items() %}
                                         <td class="{% raw -%} {{ td_class }} {%- endraw %}">{{field_accessor}}</td>
                                        {% endfor %}
 
                                         <td class="{% raw %} {{ td_class }} {% endraw %}">
@@ -123,9 +123,9 @@
                 {% endwith %}
             </ul>
         </div>
     {% endif %}
     </div>
 
 {% endpartialdef %}
-{% endblock content %}
+{% endblock main_content %}
 {% endraw %}
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-{% raw %} {% extends 'base.html' %} {% load partials %} {% block content %} {%
-endraw %}
+{% raw %} {% extends 'base.html' %} {% load partials %} {% block main_content
+%} {% endraw %}
 ************ {{{{ mmooddeell__vveerrbboossee__nnaammee__pplluurraall||ccaappiittaalliizzee }}}} ************
 _N_e_w_ _{_{_ _m_o_d_e_l___n_a_m_e_|_c_a_p_i_t_a_l_i_z_e_ _}_}_ {% raw %} {% partialdef table inline=True %}
 {{{{ ffiieelldd__vveerrbboossee__nnaammee }}}}
                          {% raw %} {% with href_class="text-blue-600 hover:
                          underline hover:text-blue-500" %} {% endraw %}
                          % raw %} class="{{ href_class }}" {% endraw %} href="{
                          { detail_view_url|safe }}">View
@@ -32,8 +32,8 @@
     * {{ num }}
     * {% endif %} {% endfor %} {% if{% endraw %} {
       {model_name|lower}}s_page.has_next {% raw %}%}
     * Next
     * Last
     * {% endif %} {% endwith %}
 {% endif %}
-{% endpartialdef %} {% endblock content %} {% endraw %}
+{% endpartialdef %} {% endblock main_content %} {% endraw %}
```

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/blueprints/update.html` & `falco_cli-0.9.0/src/falco/crud/html/update.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% raw %}
 {%  extends "base.html" %}
 {% load crispy_forms_tags %}
 
-{% block content %}
+{% block main_content %}
 
     <section class="flex justify-between">
         {% endraw %}
         <h1 class="text-lg font-bold py-4"> {{ model_name}} Update - {% raw %}{{{% endraw %} {{ model_name|lower }} {% raw %}}}{% endraw %}</h1>
 
         <a href="{{list_view_url|safe}}" class="text-blue-600 hover:underline hover:text-blue-500">
             All {{model_verbose_name_plural|capitalize}}
@@ -18,9 +18,9 @@
         {% csrf_token %}
         {{form|crispy}}
 
         <button type="submit" class="cursor-pointer py-2 px-4 bg-blue-600 hover:bg-blue-700 focus:ring-blue-500 focus:ring-offset-blue-200 text-white text-center text-base font-semibold focus:outline-none focus:ring-2 focus:ring-offset-2  rounded-lg">
             Save
         </button>
     </form>
-{% endblock content %}
+{% endblock main_content %}
 {% endraw %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% raw %} {% extends "base.html" %} {% load crispy_forms_tags %} {% block
-content %} {% endraw %}
+main_content %} {% endraw %}
 ************ {{{{ mmooddeell__nnaammee}}}} UUppddaattee -- {{%% rraaww %%}}{{{{{{%% eennddrraaww %%}} {{{{ mmooddeell__nnaammee||lloowweerr }}}}
 {{%% rraaww %%}}}}}}{{%% eennddrraaww %%}} ************
 _A_l_l_ _{_{_m_o_d_e_l___v_e_r_b_o_s_e___n_a_m_e___p_l_u_r_a_l_|_c_a_p_i_t_a_l_i_z_e_}_}_ {% raw %}
 {% csrf_token %} {{form|crispy}} Save
-{% endblock content %} {% endraw %}
+{% endblock main_content %} {% endraw %}
```

### Comparing `falco_cli-0.8.0/blueprints/falco_blueprint_basic/{{ cookiecutter.project_name }}/{{ cookiecutter.project_name }}/users/migrations/0001_initial.py` & `falco_cli-0.9.0/demo/demo/users/migrations/0001_initial.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Generated by Django 5.0.1 on 2024-01-11 23:44
+# Generated by Django 4.2.8 on 2024-01-23 13:01
+import django.contrib.auth.models
+import django.contrib.auth.validators
 import django.utils.timezone
-import {{ cookiecutter.project_name }}.users.models
 from django.db import migrations
 from django.db import models
 
 
 class Migration(migrations.Migration):
     initial = True
 
@@ -12,26 +13,60 @@
         ("auth", "0012_alter_user_first_name_max_length"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="User",
             fields=[
-                ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name="ID")),
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
                 ("password", models.CharField(max_length=128, verbose_name="password")),
-                ("last_login", models.DateTimeField(blank=True, null=True, verbose_name="last login")),
+                (
+                    "last_login",
+                    models.DateTimeField(blank=True, null=True, verbose_name="last login"),
+                ),
                 (
                     "is_superuser",
                     models.BooleanField(
                         default=False,
                         help_text="Designates that this user has all permissions without explicitly assigning them.",
                         verbose_name="superuser status",
                     ),
                 ),
                 (
+                    "username",
+                    models.CharField(
+                        error_messages={"unique": "A user with that username already exists."},
+                        help_text="Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.",
+                        max_length=150,
+                        unique=True,
+                        validators=[django.contrib.auth.validators.UnicodeUsernameValidator()],
+                        verbose_name="username",
+                    ),
+                ),
+                (
+                    "first_name",
+                    models.CharField(blank=True, max_length=150, verbose_name="first name"),
+                ),
+                (
+                    "last_name",
+                    models.CharField(blank=True, max_length=150, verbose_name="last name"),
+                ),
+                (
+                    "email",
+                    models.EmailField(blank=True, max_length=254, verbose_name="email address"),
+                ),
+                (
                     "is_staff",
                     models.BooleanField(
                         default=False,
                         help_text="Designates whether the user can log into this admin site.",
                         verbose_name="staff status",
                     ),
                 ),
@@ -39,16 +74,18 @@
                     "is_active",
                     models.BooleanField(
                         default=True,
                         help_text="Designates whether this user should be treated as active. Unselect this instead of deleting accounts.",
                         verbose_name="active",
                     ),
                 ),
-                ("date_joined", models.DateTimeField(default=django.utils.timezone.now, verbose_name="date joined")),
-                ("email", models.EmailField(max_length=254, unique=True, verbose_name="email address")),
+                (
+                    "date_joined",
+                    models.DateTimeField(default=django.utils.timezone.now, verbose_name="date joined"),
+                ),
                 (
                     "groups",
                     models.ManyToManyField(
                         blank=True,
                         help_text="The groups this user belongs to. A user will get all permissions granted to each of their groups.",
                         related_name="user_set",
                         related_query_name="user",
@@ -70,11 +107,11 @@
             ],
             options={
                 "verbose_name": "user",
                 "verbose_name_plural": "users",
                 "abstract": False,
             },
             managers=[
-                ("objects", {{ cookiecutter.project_name }}.users.models.UserManager()),
+                ("objects", django.contrib.auth.models.UserManager()),
             ],
         ),
     ]
```

### Comparing `falco_cli-0.8.0/demo/config/settings.py` & `falco_cli-0.9.0/demo/config/settings.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/demo/core/utils.py` & `falco_cli-0.9.0/demo/demo/core/utils.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/demo/orders/migrations/0001_initial.py` & `falco_cli-0.9.0/demo/demo/orders/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/demo/products/views.py` & `falco_cli-0.9.0/demo/demo/products/views.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/demo/products/migrations/0001_initial.py` & `falco_cli-0.9.0/demo/demo/products/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/templates/base.html` & `falco_cli-0.9.0/demo/templates/base.html`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/templates/products/product_create.html` & `falco_cli-0.9.0/demo/templates/products/product_create.html`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/templates/products/product_detail.html` & `falco_cli-0.9.0/demo/templates/products/product_detail.html`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/templates/products/product_list.html` & `falco_cli-0.9.0/demo/templates/products/product_list.html`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/demo/templates/products/product_update.html` & `falco_cli-0.9.0/demo/templates/products/product_update.html`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/Makefile` & `falco_cli-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/conf.py` & `falco_cli-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/contributing.rst` & `falco_cli-0.9.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/index.rst` & `falco_cli-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/install.rst` & `falco_cli-0.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/make.bat` & `falco_cli-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/_static/custom.css` & `falco_cli-0.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/_templates/partials/globaltoc-above.html` & `falco_cli-0.9.0/docs/_templates/partials/globaltoc-above.html`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/avoiding_god_models.rst` & `falco_cli-0.9.0/docs/guides/avoiding_god_models.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/database_tips.rst` & `falco_cli-0.9.0/docs/guides/database_tips.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/deployment.rst` & `falco_cli-0.9.0/docs/guides/deployment.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/index.rst` & `falco_cli-0.9.0/docs/guides/index.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/interactive_user_interfaces.rst` & `falco_cli-0.9.0/docs/guides/interactive_user_interfaces.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/logging_and_monitoring.rst` & `falco_cli-0.9.0/docs/guides/logging_and_monitoring.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/optimizing_database_access.rst` & `falco_cli-0.9.0/docs/guides/optimizing_database_access.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/permissions_and_authorization.rst` & `falco_cli-0.9.0/docs/guides/permissions_and_authorization.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/realtime.rst` & `falco_cli-0.9.0/docs/guides/realtime.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/running_project_in_a_container.rst` & `falco_cli-0.9.0/docs/guides/running_project_in_a_container.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/task_queues_and_schedulers.rst` & `falco_cli-0.9.0/docs/guides/task_queues_and_schedulers.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/tips_and_extra.rst` & `falco_cli-0.9.0/docs/guides/tips_and_extra.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/guides/writing_documentation.rst` & `falco_cli-0.9.0/docs/guides/writing_documentation.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/images/deployment.png` & `falco_cli-0.9.0/docs/images/deployment.png`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/images/logo_with_text.svg` & `falco_cli-0.9.0/docs/images/logo_with_text.svg`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/images/project-tree.svg` & `falco_cli-0.9.0/docs/images/project-tree.svg`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/images/task_queue.png` & `falco_cli-0.9.0/docs/images/task_queue.png`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/crud.rst` & `falco_cli-0.9.0/docs/the_cli/crud.rst`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,60 @@
     :class: hint dropdown
 
     I think class-based views get complex faster than function-based views. Both have their use cases, but function-based views
     stay simpler to manage longer in my experience. There is an excellent document on the topic, read `django views the right way <https://spookylukey.github.io/django-views-the-right-way/>`_.
 
 If you want to see an example of the generated code, check out the `source code of the demo project <https://github.com/Tobi-De/falco/tree/main/demo/demo/products>`_.
 
+Configuration
+^^^^^^^^^^^^^
+
+There are some options that you may want to set each time you generate ``CRUD`` views for a model. For instance, most of your views might require user
+login, or you might have a specific set of HTML templates that you use every time you run the command. Typing the same options repeatedly can be tedious. 
+For such scenarios, some of the CLI options can be configured via the ``pyproject.toml`` file.
+
+Here is an example illustrating all available configurations:
+
+.. tabs::
+
+    .. tab:: ``pyproject.toml``
+
+        .. code-block:: toml
+
+            [tool.falco.crud]
+            utils-path = "apps_dir/core"
+            blueprints = "blueprints"
+            login-required = true
+            skip-git-check = true
+            always-migrate = true
+
+        .. note::
+
+            All options are optional.
+
+    .. tab:: description
+
+        .. admonition:: Keys description
+            :class: note
+
+            **utils-path**: This will be written by the ``install-crud-utils`` command. Unless you are changing where the utils are installed, you don't need to worry about this.
+
+            **blueprints**: If you are using custom blueprints for your ``html``, set the path here. It works exactly the same as the equivalent CLI option.
+
+            **login-required**: Always generate views that are decorated with the ``login_required`` decorator.
+
+            **skip-git-check**: (Not recommended) This option is for those who like to live dangerously. It will always skip the git check.
+
+            **always-migrate**: This option can only be set in the ``pyproject.toml`` file. My current workflow is to create a new app, add fields to a model and then run ``crud``. 
+            I often forget to ``makemigrations`` and ``migrate``. This can cause the ``admin`` generation code to fail. With this option set, the ``crud`` command will first try to
+            run ``makemigrations`` and ``migrate``. If either of these operations fails, the command will stop and print the error.
+
+
+
+
 Python code
 ^^^^^^^^^^^
 
 All Python code added by this command will be in **append** mode, meaning it won't override the content of your existing files.
 Instead, it will add code at the end or create the files if they are missing. The files that will be modified
 are ``forms.py``, ``urls.py``, ``admin.py`` (if you have `django-extension <https://django-extensions.readthedocs.io/en/latest/index.html>`_ installed),
 ``views.py`` and your project root ``urls.py``.
```

### Comparing `falco_cli-0.8.0/docs/the_cli/htmx.rst` & `falco_cli-0.9.0/docs/the_cli/htmx.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/index.rst` & `falco_cli-0.9.0/docs/the_cli/index.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/migrations.rst` & `falco_cli-0.9.0/docs/the_cli/migrations.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/setup_admin.rst` & `falco_cli-0.9.0/docs/the_cli/setup_admin.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/start_app.rst` & `falco_cli-0.9.0/docs/the_cli/start_app.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/start_project.rst` & `falco_cli-0.9.0/docs/the_cli/start_project.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/sync_dotenv.rst` & `falco_cli-0.9.0/docs/the_cli/sync_dotenv.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/usage.rst` & `falco_cli-0.9.0/docs/the_cli/usage.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/docs/the_cli/work.rst` & `falco_cli-0.9.0/docs/the_cli/work.rst`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/scripts/project_tree.py` & `falco_cli-0.9.0/scripts/project_tree.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/scripts/update_readme_guides.py` & `falco_cli-0.9.0/scripts/update_readme_guides.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/__main__.py` & `falco_cli-0.9.0/src/falco/__main__.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/utils.py` & `falco_cli-0.9.0/src/falco/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,23 @@
 import ast
 import subprocess
 from contextlib import contextmanager
 from pathlib import Path
-from typing import cast
-from typing import TypedDict
-
-try:
-    from typing import Unpack
-except ImportError:
-    from typing_extensions import Unpack
 
 import cappa
 import httpx
 import tomlkit
 from falco import falco_version
 from rich.progress import Progress
 from rich.progress import SpinnerColumn
 from rich.progress import TextColumn
 
 RICH_SUCCESS_MARKER = "[green]SUCCESS:"
 RICH_ERROR_MARKER = "[red]ERROR:"
 RICH_INFO_MARKER = "[blue]INFO:"
-RICH_COMMAND_MARKER = "[yellow]"
-RICH_COMMAND_MARKER_END = "[/yellow]"
-
-
-class FalcoConfig(TypedDict, total=False):
-    revision: str
-    blueprint: str
-    skip: list[str]
-    work: dict[str, str]
-    htmx: str
-    crud_utils: str
-
-
-def write_falco_config(pyproject_path: Path, **kwargs: Unpack[TypedDict]) -> FalcoConfig:
-    pyproject = tomlkit.parse(pyproject_path.read_text())
-    existing_config = pyproject.get("tool", {}).get("falco", {})
-    existing_config.update(**kwargs)
-    tool = pyproject.get("tool", {})
-    tool.update({"falco": existing_config})
-    pyproject["tool"] = tool
-    pyproject_path.write_text(tomlkit.dumps(pyproject))
-    return pyproject
-
-
-def read_falco_config(pyproject_path: Path) -> FalcoConfig:
-    pyproject = tomlkit.parse(pyproject_path.read_text())
-    return cast(FalcoConfig, pyproject.get("tool", {}).get("falco", {}))
 
 
 def clean_project_name(val: str) -> str:
     return val.strip().replace(" ", "_").replace("-", "_")
 
 
 def get_pyproject_file() -> Path:
```

### Comparing `falco_cli-0.8.0/src/falco/commands/htmx.py` & `falco_cli-0.9.0/src/falco/commands/htmx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Annotated
 
 import cappa
+from falco.config import read_falco_config
+from falco.config import write_falco_config
 from falco.utils import get_pyproject_file
 from falco.utils import network_request_with_progress
-from falco.utils import read_falco_config
-from falco.utils import write_falco_config
 from httpx import codes
 from rich import print as rich_print
 from rich.panel import Panel
 
 HTMX_DOWNLOAD_URL = "https://unpkg.com/htmx.org@{version}/dist/htmx.min.js"
 HTMX_GH_RELEASE_LATEST_URL = "https://api.github.com/repos/bigskysoftware/htmx/releases/latest"
```

### Comparing `falco_cli-0.8.0/src/falco/commands/htmx_extension.py` & `falco_cli-0.9.0/src/falco/commands/htmx_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Annotated
 
 import cappa
 import httpx
+from falco.config import read_falco_config
 from falco.utils import get_pyproject_file
 from falco.utils import network_request_with_progress
-from falco.utils import read_falco_config
 from falco.utils import simple_progress
 from rich import print as rich_print
 from rich.console import Console
 from rich.panel import Panel
 from rich.table import Table
 
 from .htmx import Htmx
```

### Comparing `falco_cli-0.8.0/src/falco/commands/reset_migrations.py` & `falco_cli-0.9.0/src/falco/commands/reset_migrations.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/commands/rm_migrations.py` & `falco_cli-0.9.0/src/falco/commands/rm_migrations.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/commands/setup_admin.py` & `falco_cli-0.9.0/src/falco/commands/setup_admin.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/commands/start_app.py` & `falco_cli-0.9.0/src/falco/commands/start_app.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/commands/start_project.py` & `falco_cli-0.9.0/src/falco/commands/start_project.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 from cookiecutter.exceptions import CookiecutterException
 from cruft import create
 from cruft.exceptions import InvalidCookiecutterRepository
 from falco.commands import InstallCrudUtils
 from falco.commands.crud.utils import run_html_formatters
 from falco.commands.htmx import get_latest_tag as htmx_latest_tag
 from falco.commands.htmx import Htmx
+from falco.config import read_falco_config
+from falco.config import write_falco_config
 from falco.utils import clean_project_name
 from falco.utils import is_new_falco_cli_available
-from falco.utils import read_falco_config
 from falco.utils import RICH_INFO_MARKER
 from falco.utils import RICH_SUCCESS_MARKER
 from falco.utils import simple_progress
-from falco.utils import write_falco_config
 from rich import print as rich_print
 from rich.prompt import Prompt
 
 DEFAULT_SKIP = [
     "playground.ipynb",
     "README.md",
 ]
```

### Comparing `falco_cli-0.8.0/src/falco/commands/sync_dotenv.py` & `falco_cli-0.9.0/src/falco/commands/sync_dotenv.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/commands/work.py` & `falco_cli-0.9.0/src/falco/commands/work.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/commands/crud/install_crud_utils.py` & `falco_cli-0.9.0/src/falco/commands/crud/install_crud_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 from typing import Annotated
 
 import cappa
-from falco.utils import FalcoConfig
+from falco.config import FalcoConfig
+from falco.config import read_falco_config
+from falco.config import write_falco_config
 from falco.utils import get_project_name
 from falco.utils import get_pyproject_file
-from falco.utils import read_falco_config
 from falco.utils import simple_progress
-from falco.utils import write_falco_config
 from rich import print as rich_print
 
 from .utils import extract_python_file_templates
 from .utils import get_crud_blueprints_path
 from .utils import render_to_string
 from .utils import run_python_formatters
 
@@ -29,15 +29,15 @@
             falco_config = read_falco_config(pyproject_path)
         except cappa.Exit:
             falco_config = {}
             pyproject_path = None
 
         output_dir = self.install(project_name=project_name, falco_config=falco_config)
         if pyproject_path:
-            write_falco_config(pyproject_path=pyproject_path, crud_utils=str(output_dir))
+            write_falco_config(pyproject_path=pyproject_path, crud={"utils_path": str(output_dir)})
 
         rich_print(f"[green]CRUD Utils installed successfully to {output_dir}.")
 
     def install(self, project_name: str, falco_config: FalcoConfig) -> Path:
         output_dir = self.output_dir or self.get_install_path(project_name=project_name, falco_config=falco_config)[0]
 
         output_dir.mkdir(parents=True, exist_ok=True)
@@ -62,10 +62,10 @@
         for file in generated_files:
             run_python_formatters(str(file))
 
         return output_dir
 
     @classmethod
     def get_install_path(cls, project_name: str, falco_config: FalcoConfig) -> tuple[Path, bool]:
-        if _import_path := falco_config.get("crud_utils"):
+        if _import_path := falco_config.get("crud", {}).get("utils_path"):
             return Path(_import_path), True
         return Path(f"{project_name}/core"), False
```

### Comparing `falco_cli-0.8.0/src/falco/commands/crud/model_crud.py` & `falco_cli-0.9.0/src/falco/commands/crud/model_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from pathlib import Path
 from typing import Annotated
 from typing import cast
 from typing import TypedDict
 
 import cappa
 import parso
+from falco.config import CRUDConfig
+from falco.config import read_falco_config
 from falco.utils import get_project_name
-from falco.utils import read_falco_config
 from falco.utils import RICH_ERROR_MARKER
 from falco.utils import RICH_INFO_MARKER
 from falco.utils import RICH_SUCCESS_MARKER
 from falco.utils import run_in_shell
 from falco.utils import simple_progress
 from rich import print as rich_print
 
@@ -20,217 +21,14 @@
 from .utils import extract_python_file_templates
 from .utils import get_crud_blueprints_path
 from .utils import render_to_string
 from .utils import run_html_formatters
 from .utils import run_python_formatters
 
 
-class PythonBlueprintContext(TypedDict):
-    project_name: str
-    login_required: bool
-    app_label: str
-    model_name: str
-    model_verbose_name_plural: str
-    model_fields: dict[str, str]
-    excluded_fields: list[str]
-    crud_utils_import: str
-
-
-class UrlsForContext(TypedDict):
-    list_view_url: str
-    create_view_url: str
-    detail_view_url: str
-    update_view_url: str
-    delete_view_url: str
-
-
-class HtmlBlueprintContext(UrlsForContext):
-    app_label: str
-    model_name: str
-    model_verbose_name_plural: str
-    model_fields: dict[str, str]
-    # a example of the dict: {"Name": "{{product.name}}", "Price": "{{product.price}}"}
-    fields_verbose_name_with_accessor: dict[str, str]
-
-
-class DjangoModel(TypedDict):
-    name: str
-    verbose_name_plural: str
-    fields: dict[str, str]
-
-
-models_data_code = """
-from django.apps import apps
-models = apps.get_app_config("{}").get_models()
-def get_model_dict(model):
-    name = model.__name__
-    verbose_name_plural = getattr(model._meta, 'verbose_name_plural', f"{{name}}s")
-    fields = {{field.name: field.verbose_name for field in model._meta.fields}}
-    return {{"name": name, "fields": fields, "verbose_name_plural": verbose_name_plural}}
-print([get_model_dict(model) for model in models])
-"""
-
-app_path_name_and_templates_dir_code = """
-from django.apps import apps
-from django.conf import settings
-from pathlib import Path
-app = apps.get_app_config("{}")
-dirs = settings.TEMPLATES[0].get("DIRS", [])
-templates_dir = Path(dirs[0]) if dirs else Path(app.path) / "templates"
-app_templates_dir = templates_dir / "{}"
-print((str(app.path), str(app.name), str(app_templates_dir)))
-"""
-
-root_url_config_path_code = """
-from django.conf import settings
-root_urlconf = settings.ROOT_URLCONF
-print(root_urlconf)
-"""
-
-
-def get_urls(model_name_lower: str, urlsafe_model_verbose_name_plural: str) -> str:
-    prefix = urlsafe_model_verbose_name_plural
-    return f"""
-        path('{prefix}/', views.{model_name_lower}_list, name='{model_name_lower}_list'),
-        path('{prefix}/create/', views.{model_name_lower}_create, name='{model_name_lower}_create'),
-        path('{prefix}/<int:pk>/', views.{model_name_lower}_detail, name='{model_name_lower}_detail'),
-        path('{prefix}/<int:pk>/update/', views.{model_name_lower}_update, name='{model_name_lower}_update'),
-        path('{prefix}/<int:pk>/delete/', views.{model_name_lower}_delete, name='{model_name_lower}_delete'),
-    """
-
-
-def get_urls_template_string(app_label: str, model_name_lower: str) -> UrlsForContext:
-    return {
-        "list_view_url": f"{{% url '{app_label}:{model_name_lower}_list' %}}",
-        "create_view_url": f"{{% url '{app_label}:{model_name_lower}_create' %}}",
-        "detail_view_url": f"{{% url '{app_label}:{model_name_lower}_detail' {model_name_lower}.pk %}}",
-        "update_view_url": f"{{% url '{app_label}:{model_name_lower}_update' {model_name_lower}.pk %}}",
-        "delete_view_url": f"{{% url '{app_label}:{model_name_lower}_delete' {model_name_lower}.pk %}}",
-    }
-
-
-def initial_urls_content(app_label: str, urls_content: str) -> str:
-    return f"""
-from django.urls import path
-from . import views
-
-app_name = "{app_label}"
-
-urlpatterns = [
-{urls_content}
-]
-        """
-
-
-def register_app_urls(app_label: str, app_name: str) -> Path:
-    root_url = run_in_shell(root_url_config_path_code, eval_result=False)
-    root_url = root_url.strip().replace(".", "/")
-    rool_url_path = Path(f"{root_url}.py")
-    module = parso.parse(rool_url_path.read_text())
-    new_path = parso.parse(f"path('{app_label}/', include('{app_name}.urls', namespace='{app_label}'))")
-
-    for node in module.children:
-        try:
-            if (
-                node.children[0].type == parso.python.tree.ExprStmt.type
-                and node.children[0].children[0].value == "urlpatterns"
-            ):
-                patterns = node.children[0].children[2]
-                elements = patterns.children[1]
-                elements.children.append(new_path)
-                new_content = module.get_code()
-                new_content = "from django.urls import include\n" + new_content
-                rool_url_path.write_text(new_content)
-                break
-        except AttributeError:
-            continue
-
-    return rool_url_path
-
-
-def register_models_in_admin(app_folder_path: Path, app_label: str, model_name: str | None = None) -> Path:
-    admin_file = app_folder_path / "admin.py"
-    admin_file.touch(exist_ok=True)
-    cmd_args = [app_label]
-    if model_name:
-        cmd_args.append(model_name)
-
-    result = subprocess.run(
-        ["python", "manage.py", "admin_generator", *cmd_args],
-        capture_output=True,
-        text=True,
-        check=False,
-    )
-    if result.returncode != 0:
-        msg = result.stderr.split("\n")[-2]
-        rich_print(f"{RICH_ERROR_MARKER}Admin failed to generate: {msg}")
-        return admin_file
-
-    # the first set the encoding, it is useless
-    admin_code = result.stdout.split("\n", 1)[1]
-    admin_file.write_text(admin_file.read_text() + admin_code)
-
-    if not model_name:
-        # we probably don't need to reorder the imports if the admin code is being generated for all models
-        return admin_file
-
-    # if this is not the first time running this, the imports will be messed up, move all
-    # of them to the top
-    admin_lines = admin_file.read_text().split("\n")
-    _imports = []
-    _code = []
-    for line in admin_lines:
-        if line.startswith("from"):
-            _imports.append(line)
-        else:
-            _code.append(line)
-    admin_file.write_text("\n" + "\n".join(_imports) + "\n" + "\n".join(_code))
-
-    return admin_file
-
-
-def get_python_blueprint_context(
-    project_name: str,
-    app_label: str,
-    django_model: DjangoModel,
-    excluded_fields: list[str],
-    crud_utils_import: str,
-    *,
-    login_required: bool,
-) -> PythonBlueprintContext:
-    return {
-        "project_name": project_name,
-        "app_label": app_label,
-        "login_required": login_required,
-        "model_name": django_model["name"],
-        "model_verbose_name_plural": django_model["verbose_name_plural"],
-        "model_fields": django_model["fields"],
-        "excluded_fields": excluded_fields,
-        "crud_utils_import": crud_utils_import,
-    }
-
-
-def get_html_blueprint_context(app_label: str, django_model: DjangoModel) -> HtmlBlueprintContext:
-    model_name_lower = django_model["name"].lower()
-    return {
-        "app_label": app_label,
-        "model_name": django_model["name"],
-        "model_verbose_name_plural": django_model["verbose_name_plural"],
-        "model_fields": django_model["fields"],
-        "fields_verbose_name_with_accessor": {
-            verbose_name: "{{" + f"{model_name_lower}.{name}" + "}}"
-            for name, verbose_name in django_model["fields"].items()
-        },
-        **get_urls_template_string(
-            app_label=app_label,
-            model_name_lower=django_model["name"].lower(),
-        ),
-    }
-
-
 @cappa.command(help="Generate CRUD (Create, Read, Update, Delete) views for a model.", name="crud")
 class ModelCRUD:
     model_path: Annotated[
         str,
         cappa.Arg(
             help="The path (<app_label>.<model_name>) of the model to generate CRUD views for. Ex: myapp.product"
         ),
@@ -280,27 +78,45 @@
             default=False,
             long="--skip-git-check",
             help="Do not check if your git repo is clean.",
         ),
     ]
 
     def __call__(self, project_name: Annotated[str, cappa.Dep(get_project_name)]):
+        pyproject_path = Path("pyproject.toml")
+        falco_config = read_falco_config(pyproject_path=pyproject_path) if pyproject_path.exists() else {}
+        crud_config: CRUDConfig = falco_config.get("crud", {})
+
+        self.blueprints = self.blueprints or crud_config.get("blueprints")
+        self.login_required = crud_config.get("login_required", self.login_required)
+        self.skip_git_check = crud_config.get("skip_git_check", self.skip_git_check)
+
         checks.clean_git_repo(ignore_dirty=self.skip_git_check)
 
         v = self.model_path.split(".")
 
         excluded_fields = [*self.excluded_fields, "created", "modified"]
 
         if len(v) == 1:
             name = None
             app_label = v[0]
         else:
             name = v.pop()
             app_label = ".".join(v)
 
+        if crud_config.get("always_migrate", False):
+            commands = [f"python manage.py makemigrations {app_label}", f"python manage.py migrate {app_label}"]
+            with simple_progress("Running migrations"):
+                for cmd in commands:
+                    result = subprocess.run(cmd.split(), capture_output=True, check=False, text=True)
+
+                    if result.returncode != 0:
+                        msg = result.stderr
+                        raise cappa.Exit("migrations step failed\n" + msg, code=1)
+
         if self.entry_point and not name:
             raise cappa.Exit("The --entry-point option requires a full model path.", code=1)
 
         with simple_progress("Getting models info"):
             all_django_models = cast(
                 list[DjangoModel],
                 run_in_shell(models_data_code.format(app_label)),
@@ -319,16 +135,14 @@
         )
         if name and not django_models:
             msg = f"Model {name} not found in app {app_label}"
             raise cappa.Exit(msg, code=1)
 
         python_blueprint_context: list[PythonBlueprintContext] = []
         html_blueprint_context: list[HtmlBlueprintContext] = []
-        pyproject_path = Path("pyproject.toml")
-        falco_config = read_falco_config(pyproject_path=pyproject_path) if pyproject_path.exists() else {}
         install_path, crud_utils_installed = InstallCrudUtils.get_install_path(
             project_name=project_name,
             falco_config=falco_config,
         )
         crud_utils_import = str(install_path).replace("/", ".")
 
         for django_model in django_models:
@@ -401,15 +215,15 @@
 
     @simple_progress("Generating python code")
     def generate_python_code(
         self,
         app_label: str,
         app_folder_path: Path,
         blueprints: list[Path],
-        contexts: list[PythonBlueprintContext],
+        contexts: list["PythonBlueprintContext"],
         *,
         entry_point: bool,
     ) -> list[Path]:
         updated_files = []
 
         for blueprint in blueprints:
             imports_template, code_template = extract_python_file_templates(blueprint.read_text())
@@ -444,15 +258,15 @@
 
     @simple_progress("Generating urls")
     def generating_urls(
         self,
         app_folder_path: Path,
         app_label: str,
         app_name: str,
-        django_models: list[DjangoModel],
+        django_models: list["DjangoModel"],
         *,
         entry_point: bool,
     ) -> list[Path]:
         urls_content = ""
         for django_model in django_models:
             model_name_lower = django_model["name"].lower()
             urlsafe_model_verbose_name_plural = django_model["verbose_name_plural"].lower().replace(" ", "-")
@@ -477,15 +291,15 @@
         return updated_files
 
     @simple_progress("Generating html templates")
     def generate_html_templates(
         self,
         templates_dir: Path,
         blueprints: list[Path],
-        contexts: list[HtmlBlueprintContext],
+        contexts: list["HtmlBlueprintContext"],
         *,
         entry_point: bool,
     ) -> list[Path]:
         updated_files = []
         templates_dir.mkdir(exist_ok=True, parents=True)
         for blueprint in blueprints:
             filecontent = blueprint.read_text()
@@ -504,7 +318,210 @@
                 if entry_point:
                     views_content = views_content.replace(f"{model_name_lower}_", "")
                     views_content = views_content.replace("list", "index")
                 file_to_write_to.write_text(views_content)
                 updated_files.append(file_to_write_to)
 
         return updated_files
+
+
+class PythonBlueprintContext(TypedDict):
+    project_name: str
+    login_required: bool
+    app_label: str
+    model_name: str
+    model_verbose_name_plural: str
+    model_fields: dict[str, str]
+    excluded_fields: list[str]
+    crud_utils_import: str
+
+
+class UrlsForContext(TypedDict):
+    list_view_url: str
+    create_view_url: str
+    detail_view_url: str
+    update_view_url: str
+    delete_view_url: str
+
+
+class HtmlBlueprintContext(UrlsForContext):
+    app_label: str
+    model_name: str
+    model_verbose_name_plural: str
+    model_fields: dict[str, str]
+    # a example of the dict: {"Name": "{{product.name}}", "Price": "{{product.price}}"}
+    fields_verbose_name_with_accessor: dict[str, str]
+
+
+class DjangoModel(TypedDict):
+    name: str
+    verbose_name_plural: str
+    fields: dict[str, str]
+
+
+models_data_code = """
+from django.apps import apps
+models = apps.get_app_config("{}").get_models()
+def get_model_dict(model):
+    name = model.__name__
+    verbose_name_plural = getattr(model._meta, 'verbose_name_plural', f"{{name}}s")
+    fields = {{field.name: field.verbose_name for field in model._meta.fields}}
+    return {{"name": name, "fields": fields, "verbose_name_plural": verbose_name_plural}}
+print([get_model_dict(model) for model in models])
+"""
+
+app_path_name_and_templates_dir_code = """
+from django.apps import apps
+from django.conf import settings
+from pathlib import Path
+app = apps.get_app_config("{}")
+dirs = settings.TEMPLATES[0].get("DIRS", [])
+templates_dir = Path(dirs[0]) if dirs else Path(app.path) / "templates"
+app_templates_dir = templates_dir / "{}"
+print((str(app.path), str(app.name), str(app_templates_dir)))
+"""
+
+root_url_config_path_code = """
+from django.conf import settings
+root_urlconf = settings.ROOT_URLCONF
+print(root_urlconf)
+"""
+
+
+def get_urls(model_name_lower: str, urlsafe_model_verbose_name_plural: str) -> str:
+    prefix = urlsafe_model_verbose_name_plural
+    return f"""
+        path('{prefix}/', views.{model_name_lower}_list, name='{model_name_lower}_list'),
+        path('{prefix}/create/', views.{model_name_lower}_create, name='{model_name_lower}_create'),
+        path('{prefix}/<int:pk>/', views.{model_name_lower}_detail, name='{model_name_lower}_detail'),
+        path('{prefix}/<int:pk>/update/', views.{model_name_lower}_update, name='{model_name_lower}_update'),
+        path('{prefix}/<int:pk>/delete/', views.{model_name_lower}_delete, name='{model_name_lower}_delete'),
+    """
+
+
+def get_urls_template_string(app_label: str, model_name_lower: str) -> UrlsForContext:
+    return {
+        "list_view_url": f"{{% url '{app_label}:{model_name_lower}_list' %}}",
+        "create_view_url": f"{{% url '{app_label}:{model_name_lower}_create' %}}",
+        "detail_view_url": f"{{% url '{app_label}:{model_name_lower}_detail' {model_name_lower}.pk %}}",
+        "update_view_url": f"{{% url '{app_label}:{model_name_lower}_update' {model_name_lower}.pk %}}",
+        "delete_view_url": f"{{% url '{app_label}:{model_name_lower}_delete' {model_name_lower}.pk %}}",
+    }
+
+
+def initial_urls_content(app_label: str, urls_content: str) -> str:
+    return f"""
+from django.urls import path
+from . import views
+
+app_name = "{app_label}"
+
+urlpatterns = [
+{urls_content}
+]
+        """
+
+
+def register_app_urls(app_label: str, app_name: str) -> Path:
+    root_url = run_in_shell(root_url_config_path_code, eval_result=False)
+    root_url = root_url.strip().replace(".", "/")
+    rool_url_path = Path(f"{root_url}.py")
+    module = parso.parse(rool_url_path.read_text())
+    new_path = parso.parse(f"path('{app_label}/', include('{app_name}.urls', namespace='{app_label}'))")
+
+    for node in module.children:
+        try:
+            if (
+                node.children[0].type == parso.python.tree.ExprStmt.type
+                and node.children[0].children[0].value == "urlpatterns"
+            ):
+                patterns = node.children[0].children[2]
+                elements = patterns.children[1]
+                elements.children.append(new_path)
+                new_content = module.get_code()
+                new_content = "from django.urls import include\n" + new_content
+                rool_url_path.write_text(new_content)
+                break
+        except AttributeError:
+            continue
+
+    return rool_url_path
+
+
+def register_models_in_admin(app_folder_path: Path, app_label: str, model_name: str | None = None) -> Path:
+    admin_file = app_folder_path / "admin.py"
+    admin_file.touch(exist_ok=True)
+    cmd_args = [app_label]
+    if model_name:
+        cmd_args.append(model_name)
+
+    result = subprocess.run(
+        ["python", "manage.py", "admin_generator", *cmd_args],
+        capture_output=True,
+        text=True,
+        check=False,
+    )
+    if result.returncode != 0:
+        msg = result.stderr.split("\n")[-2]
+        rich_print(f"{RICH_ERROR_MARKER}Admin failed to generate: {msg}")
+        return admin_file
+
+    # the first set the encoding, it is useless
+    admin_code = result.stdout.split("\n", 1)[1]
+    admin_file.write_text(admin_file.read_text() + admin_code)
+
+    if not model_name:
+        # we probably don't need to reorder the imports if the admin code is being generated for all models
+        return admin_file
+
+    # if this is not the first time running this, the imports will be messed up, move all
+    # of them to the top
+    admin_lines = admin_file.read_text().split("\n")
+    _imports = []
+    _code = []
+    for line in admin_lines:
+        if line.startswith("from"):
+            _imports.append(line)
+        else:
+            _code.append(line)
+    admin_file.write_text("\n" + "\n".join(_imports) + "\n" + "\n".join(_code))
+
+    return admin_file
+
+
+def get_python_blueprint_context(
+    project_name: str,
+    app_label: str,
+    django_model: DjangoModel,
+    excluded_fields: list[str],
+    crud_utils_import: str,
+    *,
+    login_required: bool,
+) -> PythonBlueprintContext:
+    return {
+        "project_name": project_name,
+        "app_label": app_label,
+        "login_required": login_required,
+        "model_name": django_model["name"],
+        "model_verbose_name_plural": django_model["verbose_name_plural"],
+        "model_fields": django_model["fields"],
+        "excluded_fields": excluded_fields,
+        "crud_utils_import": crud_utils_import,
+    }
+
+
+def get_html_blueprint_context(app_label: str, django_model: DjangoModel) -> HtmlBlueprintContext:
+    model_name_lower = django_model["name"].lower()
+    return {
+        "app_label": app_label,
+        "model_name": django_model["name"],
+        "model_verbose_name_plural": django_model["verbose_name_plural"],
+        "model_fields": django_model["fields"],
+        "fields_verbose_name_with_accessor": {
+            verbose_name: "{{" + f"{model_name_lower}.{name}" + "}}"
+            for name, verbose_name in django_model["fields"].items()
+        },
+        **get_urls_template_string(
+            app_label=app_label,
+            model_name_lower=django_model["name"].lower(),
+        ),
+    }
```

### Comparing `falco_cli-0.8.0/src/falco/commands/crud/utils.py` & `falco_cli-0.9.0/src/falco/commands/crud/utils.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/crud/python/views.py.jinja` & `falco_cli-0.9.0/src/falco/crud/python/views.py.jinja`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/src/falco/crud/utils/utils.py.jinja` & `falco_cli-0.9.0/src/falco/crud/utils/utils.py.jinja`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/tests/conftest.py` & `falco_cli-0.9.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,18 +41,18 @@
     settings_file = project_dir / "myproject" / "settings.py"
     settings_content = settings_file.read_text()
     settings_file.write_text(settings_content + "\n" + "INSTALLED_APPS += ['blog', 'django_extensions']\n")
 
     # create a pyproject.toml
     (project_dir / "pyproject.toml").write_text(
         """
-        [project]
-        name = "myproject"
-        version = "0.1.0"
-        """
+[project]
+name = "myproject"
+version = "0.1.0"
+"""
     )
 
     yield project_dir
     os.chdir(tmp_path)
 
 
 @pytest.fixture
```

### Comparing `falco_cli-0.8.0/tests/commands/test_crud.py` & `falco_cli-0.9.0/tests/commands/test_crud.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import subprocess
 from pathlib import Path
 
 import cappa
 import pytest
 from cappa.testing import CommandRunner
+from falco.config import write_falco_config
 
 views_functions = ["post_list", "post_detail", "post_update", "post_create"]
 html_templates = [
     "post_list.html",
     "post_detail.html",
     "post_update.html",
     "post_create.html",
@@ -19,14 +20,20 @@
     "update.html",
     "create.html",
 ]
 forms_attributes = ["PostForm", "Post", "title", "content"]
 admin_attributes = ["PostAdmin", "Post", "title", "content"]
 
 
+def create_pyproject_crud_config(**kwargs):
+    pyproject_toml = Path("pyproject.toml")
+    pyproject_toml.touch()
+    write_falco_config(pyproject_path=pyproject_toml, crud=kwargs)
+
+
 def healthy_django_project() -> bool:
     result = subprocess.run(
         ["python", "manage.py", "check"],
         check=False,
         capture_output=True,
         text=True,
     )
@@ -171,8 +178,51 @@
     runner.invoke("crud", "blog.post", "--login-required")
     assert healthy_django_project()
     views = (Path("blog") / "views.py").read_text()
     assert "@login_required" in views
     assert "AuthenticatedHttpRequest" in views
 
 
-# TODO: write more tests, test that test all options, example login_required
+def test_crud_config_pyproject_skip_git_check_set(django_project, runner: CommandRunner):
+    create_pyproject_crud_config(skip_git_check=True)
+    install_crud_utils(runner)
+    runner.invoke("crud", "blog.post")
+    assert healthy_django_project()
+    views = (Path("blog") / "views.py").read_text()
+    assert "post_list" in views
+
+
+def test_crud_config_pyproject_login_required(django_project, runner: CommandRunner):
+    create_pyproject_crud_config(skip_git_check=True, login_required=True)
+    install_crud_utils(runner)
+    runner.invoke("crud", "blog.post")
+    assert healthy_django_project()
+    views = (Path("blog") / "views.py").read_text()
+    assert "@login_required" in views
+    assert "AuthenticatedHttpRequest" in views
+
+
+def test_crud_config_pyproject_blueprints(django_project, runner: CommandRunner):
+    bp = django_project / "blueprints"
+    bp.mkdir()
+    html_file = bp / "dummy.html"
+    html_file.touch()
+    html_file.write_text("{{ model_name }}")
+    create_pyproject_crud_config(blueprints=str(Path("blueprints")), skip_git_check=True)
+    install_crud_utils(runner)
+    runner.invoke("crud", "blog.post")
+    views = (Path("blog") / "views.py").read_text()
+    rendered_file = Path("blog") / "templates" / "blog" / "post_dummy.html"
+    assert rendered_file.exists()
+    assert "Post" in rendered_file.read_text()
+    assert "Post" in views
+
+
+def test_crud_always_migrate(django_project, runner: CommandRunner, set_git_repo_to_clean):
+    create_pyproject_crud_config(always_migrate=True)
+    settings = django_project / "myproject" / "settings.py"
+    settings.write_text(settings.read_text() + "\n\n" + "INSTALLED_APPS += ['non_existent_app']\n")
+    install_crud_utils(runner)
+    with pytest.raises(cappa.Exit):
+        runner.invoke("crud", "blog.post")
+    assert "post_list" not in Path("blog/views.py").read_text()
+    assert not healthy_django_project()
```

### Comparing `falco_cli-0.8.0/tests/commands/test_htmx.py` & `falco_cli-0.9.0/tests/commands/test_htmx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 
 from cappa.testing import CommandRunner
 from falco.commands.htmx import Htmx
-from falco.utils import write_falco_config, read_falco_config
+from falco.config import read_falco_config
+from falco.config import write_falco_config
 
 
 def test_htmx_download(runner: CommandRunner):
     runner.invoke("htmx")
     assert Path("htmx.min.js").exists()
```

### Comparing `falco_cli-0.8.0/tests/commands/test_htmx_extension.py` & `falco_cli-0.9.0/tests/commands/test_htmx_extension.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 from cappa.testing import CommandRunner
-from falco.utils import write_falco_config
+from falco.config import write_falco_config
 
 
 def test_htmx_ext_download(runner: CommandRunner):
     runner.invoke("htmx-ext", "sse")
     assert Path("sse.js").exists()
```

### Comparing `falco_cli-0.8.0/tests/commands/test_install_crud_utils.py` & `falco_cli-0.9.0/tests/commands/test_install_crud_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 from cappa.testing import CommandRunner
-from falco.utils import write_falco_config
+from falco.config import write_falco_config
 
 
 def test_install_crud_utils(runner: CommandRunner, pyproject_toml):
     runner.invoke("install-crud-utils", ".")
     assert Path("utils.py").exists()
     assert Path("types.py").exists()
     assert Path("__init__.py").exists()
@@ -17,13 +17,13 @@
     assert (output / "utils.py").exists()
     assert (output / "types.py").exists()
     assert (output / "__init__.py").exists()
 
 
 def test_install_crud_utils_to_existing_config(runner: CommandRunner, pyproject_toml):
     pyproject_toml = Path("pyproject.toml")
-    write_falco_config(pyproject_path=pyproject_toml, crud_utils="myproject/special_utils_dir")
+    write_falco_config(pyproject_path=pyproject_toml, crud={"utils_path": "myproject/special_utils_dir"})
     output = Path("myproject/special_utils_dir")
     runner.invoke("install-crud-utils")
     assert (output / "utils.py").exists()
     assert (output / "types.py").exists()
     assert (output / "__init__.py").exists()
```

### Comparing `falco_cli-0.8.0/tests/commands/test_reset_migrations.py` & `falco_cli-0.9.0/tests/commands/test_reset_migrations.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/tests/commands/test_rm_migrations.py` & `falco_cli-0.9.0/tests/commands/test_rm_migrations.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/tests/commands/test_setup_admin.py` & `falco_cli-0.9.0/tests/commands/test_setup_admin.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/tests/commands/test_start_project.py` & `falco_cli-0.9.0/tests/commands/test_start_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
 from cappa.testing import CommandRunner
-from falco.utils import read_falco_config
+from falco.config import read_falco_config
 
 
 def generated_project_files(project_name) -> list[str]:
     return [
         project_name,
         "pyproject.toml",
         "README.md",
```

### Comparing `falco_cli-0.8.0/tests/commands/test_sync_dotenv.py` & `falco_cli-0.9.0/tests/commands/test_sync_dotenv.py`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/README.md` & `falco_cli-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/pyproject.toml` & `falco_cli-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `falco_cli-0.8.0/PKG-INFO` & `falco_cli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falco-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: Enhance your Django developer experience: CLI and Guides for the Modern Developer.
 Project-URL: Homepage, https://falco.oluwatobi.dev/
 Project-URL: Documentation, https://falco.oluwatobi.dev/
 Project-URL: Issues, https://github.com/tobi-de/falco/issues
 Project-URL: Source, https://github.com/tobi-de/falco
 Author-email: Tobi DEGNON <tobidegnon@proton.me>
 License-Expression: MIT
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: falco-cli Version: 0.8.0 Summary: Enhance your
+Metadata-Version: 2.1 Name: falco-cli Version: 0.9.0 Summary: Enhance your
 Django developer experience: CLI and Guides for the Modern Developer. Project-
 URL: Homepage, https://falco.oluwatobi.dev/ Project-URL: Documentation, https:/
 /falco.oluwatobi.dev/ Project-URL: Issues, https://github.com/tobi-de/falco/
 issues Project-URL: Source, https://github.com/tobi-de/falco Author-email: Tobi
 DEGNON
 proton.me> License-Expression: MIT License-File: LICENSE Keywords:
 cookiecutter,django,project-template,python Classifier: Development Status :: 4
```

