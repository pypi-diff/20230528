# Comparing `tmp/django-ninja-0.9.6.tar.gz` & `tmp/django-ninja-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ninja-0.9.6.tar", last modified: Mon Dec 21 07:53:28 2020, max compression
+gzip compressed data, was "django-ninja-0.9.7.tar", last modified: Fri Dec 25 12:49:03 2020, max compression
```

## Comparing `django-ninja-0.9.6.tar` & `django-ninja-0.9.7.tar`

### file list

```diff
@@ -1,150 +1,150 @@
--rw-r--r--   0        0        0       35 2020-12-21 07:52:54.633646 django-ninja-0.9.6/.coveragerc
--rw-r--r--   0        0        0       66 2020-12-21 07:52:54.633646 django-ninja-0.9.6/.dockerignore
--rw-r--r--   0        0        0      554 2020-12-21 07:52:54.637646 django-ninja-0.9.6/.github/workflows/publish.yml
--rw-r--r--   0        0        0      617 2020-12-21 07:52:54.637646 django-ninja-0.9.6/.github/workflows/test.yml
--rw-r--r--   0        0        0       85 2020-12-21 07:52:54.637646 django-ninja-0.9.6/.gitignore
--rw-r--r--   0        0        0      930 2020-12-21 07:52:54.637646 django-ninja-0.9.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1086 2020-12-21 07:52:54.637646 django-ninja-0.9.6/LICENSE
--rw-r--r--   0        0        0     2816 2020-12-21 07:52:54.637646 django-ninja-0.9.6/README.md
--rw-r--r--   0        0        0     5904 2020-12-21 07:52:54.637646 django-ninja-0.9.6/docs/docs/async-support.md
--rw-r--r--   0        0        0     1001 2020-12-21 07:52:54.637646 django-ninja-0.9.6/docs/docs/help.md
--rw-r--r--   0        0        0    28154 2020-12-21 07:52:54.637646 django-ninja-0.9.6/docs/docs/img/auth-swagger-ui-prompt.png
--rw-r--r--   0        0        0    27900 2020-12-21 07:52:54.637646 django-ninja-0.9.6/docs/docs/img/auth-swagger-ui.png
--rw-r--r--   0        0        0    51900 2020-12-21 07:52:54.637646 django-ninja-0.9.6/docs/docs/img/benchmark.png
--rw-r--r--   0        0        0   654914 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/body-editor.gif
--rw-r--r--   0        0        0    46786 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/body-schema-doc.png
--rw-r--r--   0        0        0    55925 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/body-schema-doc2.png
--rw-r--r--   0        0        0    44459 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/deprecated.png
--rw-r--r--   0        0        0     2717 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/docs-logo.png
--rw-r--r--   0        0        0     6234 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/favicon.png
--rw-r--r--   0        0        0     3439 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/github-star.png
--rw-r--r--   0        0        0    18865 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/hero.png
--rw-r--r--   0        0        0    95509 2020-12-21 07:52:54.641646 django-ninja-0.9.6/docs/docs/img/index-swagger-ui.png
--rw-r--r--   0        0        0    12028 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/logo-big.png
--rw-r--r--   0        0        0   122725 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/nested-routers-swagger.png
--rw-r--r--   0        0        0    45259 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/operation_description.png
--rw-r--r--   0        0        0    53995 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/operation_description_docstring.png
--rw-r--r--   0        0        0    28482 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/operation_summary.png
--rw-r--r--   0        0        0    22627 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/operation_summary_default.png
--rw-r--r--   0        0        0    48354 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/operation_tags.png
--rw-r--r--   0        0        0    65000 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/simple-routers-swagger.png
--rw-r--r--   0        0        0   115803 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/img/tutorial-path-swagger.png
--rw-r--r--   0        0        0     3304 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/index.md
--rw-r--r--   0        0        0     2956 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/motivation.md
--rw-r--r--   0        0        0     4653 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/proposals/cbv.md
--rw-r--r--   0        0        0      492 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/proposals/index.md
--rw-r--r--   0        0        0     3873 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/proposals/models.md
--rw-r--r--   0        0        0      114 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/releases.md
--rw-r--r--   0        0        0     3991 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/tutorial/authentication.md
--rw-r--r--   0        0        0     4569 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/tutorial/body.md
--rw-r--r--   0        0        0     5805 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/tutorial/crud.md
--rw-r--r--   0        0        0      816 2020-12-21 07:52:54.645646 django-ninja-0.9.6/docs/docs/tutorial/csrf.md
--rw-r--r--   0        0        0     1800 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/docs/tutorial/index.md
--rw-r--r--   0        0        0     3221 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/docs/tutorial/operation_params.md
--rw-r--r--   0        0        0     2844 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     2812 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     5289 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/docs/tutorial/response-schema.md
--rw-r--r--   0        0        0     4145 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/docs/tutorial/routers.md
--rw-r--r--   0        0        0     1480 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/docs/tutorial/versioning.md
--rw-r--r--   0        0        0     1113 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/mkdocs.yml
--rw-r--r--   0        0        0      274 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/index001.py
--rw-r--r--   0        0        0      442 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/apikey01.py
--rw-r--r--   0        0        0      322 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/apikey02.py
--rw-r--r--   0        0        0      298 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/apikey03.py
--rw-r--r--   0        0        0      314 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/basic01.py
--rw-r--r--   0        0        0      271 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/bearer01.py
--rw-r--r--   0        0        0      198 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/code001.py
--rw-r--r--   0        0        0      231 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/code002.py
--rw-r--r--   0        0        0      542 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/global01.py
--rw-r--r--   0        0        0      390 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/multiple01.py
--rw-r--r--   0        0        0        0 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/authentication/schema01.py
--rw-r--r--   0        0        0      195 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/body/code01.py
--rw-r--r--   0        0        0      255 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/body/code02.py
--rw-r--r--   0        0        0      272 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/body/code03.py
--rw-r--r--   0        0        0       94 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/path/code01.py
--rw-r--r--   0        0        0      325 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/path/code010.py
--rw-r--r--   0        0        0       99 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/path/code02.py
--rw-r--r--   0        0        0      209 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/query/code01.py
--rw-r--r--   0        0        0      252 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/query/code010.py
--rw-r--r--   0        0        0      281 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/query/code02.py
--rw-r--r--   0        0        0      157 2020-12-21 07:52:54.649646 django-ninja-0.9.6/docs/src/tutorial/query/code03.py
--rw-r--r--   0        0        0      233 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/__init__.py
--rw-r--r--   0        0        0       52 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/compatibility/__init__.py
--rw-r--r--   0        0        0     1734 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/compatibility/datastructures.py
--rw-r--r--   0        0        0     1326 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/compatibility/request.py
--rw-r--r--   0        0        0       19 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/constants.py
--rw-r--r--   0        0        0      525 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/errors.py
--rw-r--r--   0        0        0     7653 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/main.py
--rw-r--r--   0        0        0       44 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/openapi/__init__.py
--rw-r--r--   0        0        0     6824 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/openapi/schema.py
--rw-r--r--   0        0        0      891 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/openapi/urls.py
--rw-r--r--   0        0        0     1424 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/openapi/views.py
--rw-r--r--   0        0        0     8806 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/operation.py
--rw-r--r--   0        0        0     1631 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/params.py
--rw-r--r--   0        0        0     2213 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/params_models.py
--rw-r--r--   0        0        0      448 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/responses.py
--rw-r--r--   0        0        0     6510 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/router.py
--rw-r--r--   0        0        0     1135 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/schema.py
--rw-r--r--   0        0        0      209 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/security/__init__.py
--rw-r--r--   0        0        0      981 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/security/apikey.py
--rw-r--r--   0        0        0      693 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/security/base.py
--rw-r--r--   0        0        0     2171 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/security/http.py
--rw-r--r--   0        0        0      322 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/security/session.py
--rw-r--r--   0        0        0       93 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/signature/__init__.py
--rw-r--r--   0        0        0     5115 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/signature/details.py
--rw-r--r--   0        0        0     1429 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/signature/utils.py
--rw-r--r--   0        0        0      956 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/templates/ninja/swagger.html
--rw-r--r--   0        0        0      440 2020-12-21 07:52:54.649646 django-ninja-0.9.6/ninja/utils.py
--rw-r--r--   0        0        0     1883 2020-12-21 07:52:54.649646 django-ninja-0.9.6/pyproject.toml
--rwxr-xr-x   0        0        0      131 2020-12-21 07:52:54.649646 django-ninja-0.9.6/scripts/build-docs.sh
--rw-r--r--   0        0        0     3774 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/client.py
--rw-r--r--   0        0        0      451 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/demo/__init__.py
--rw-r--r--   0        0        0      424 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/demo/asgi.py
--rw-r--r--   0        0        0     1645 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/demo/settings.py
--rw-r--r--   0        0        0      695 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/demo/urls.py
--rw-r--r--   0        0        0      424 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/demo/wsgi.py
--rwxr-xr-x   0        0        0      657 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/manage.py
--rw-r--r--   0        0        0        0 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/someapp/__init__.py
--rw-r--r--   0        0        0       63 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/someapp/admin.py
--rw-r--r--   0        0        0      707 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/someapp/api.py
--rw-r--r--   0        0        0      308 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/someapp/models.py
--rw-r--r--   0        0        0       63 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/demo_project/someapp/views.py
--rw-r--r--   0        0        0     1519 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/env-matrix/Dockerfile
--rw-r--r--   0        0        0     1865 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/env-matrix/Dockerfile.backup
--rw-r--r--   0        0        0      291 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/env-matrix/README.md
--rw-r--r--   0        0        0     1136 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/env-matrix/create_docker.py
--rw-r--r--   0        0        0      111 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/env-matrix/docker-compose.yml
--rw-r--r--   0        0        0      245 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/env-matrix/install_env.sh
--rw-r--r--   0        0        0      132 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/env-matrix/run.sh
--rw-r--r--   0        0        0     4248 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/main.py
--rw-r--r--   0        0        0      106 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/pytest.ini
--rw-r--r--   0        0        0      459 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_api_instance.py
--rw-r--r--   0        0        0     2383 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_app.py
--rw-r--r--   0        0        0     1394 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_async.py
--rw-r--r--   0        0        0     4386 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_auth.py
--rw-r--r--   0        0        0     2208 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_auth_global.py
--rw-r--r--   0        0        0     1836 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_csrf.py
--rw-r--r--   0        0        0      810 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_django_models.py
--rw-r--r--   0        0        0        0 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_docs/__init__.py
--rw-r--r--   0        0        0     3607 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_docs/test_auth.py
--rw-r--r--   0        0        0     1326 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_docs/test_body.py
--rw-r--r--   0        0        0      197 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_docs/test_index.py
--rw-r--r--   0        0        0     1182 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_docs/test_path.py
--rw-r--r--   0        0        0     3259 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_docs/test_query.py
--rw-r--r--   0        0        0     2545 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_enum.py
--rw-r--r--   0        0        0      932 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_inheritance_routers.py
--rw-r--r--   0        0        0     2377 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_lists.py
--rw-r--r--   0        0        0      247 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_misc.py
--rw-r--r--   0        0        0     3397 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_models.py
--rw-r--r--   0        0        0     1742 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_openapi_params.py
--rw-r--r--   0        0        0     2810 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_openapi_schema.py
--rw-r--r--   0        0        0     7643 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_path.py
--rw-r--r--   0        0        0     2168 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_query.py
--rw-r--r--   0        0        0     1410 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_request.py
--rw-r--r--   0        0        0     1985 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_response.py
--rw-r--r--   0        0        0     3783 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_response_multiple.py
--rw-r--r--   0        0        0     1823 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_schema.py
--rw-r--r--   0        0        0      465 2020-12-21 07:52:54.649646 django-ninja-0.9.6/tests/test_union.py
--rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 django-ninja-0.9.6/setup.py
--rw-r--r--   0        0        0      221 1970-01-01 00:00:00.000000 django-ninja-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.coveragerc
+-rw-r--r--   0        0        0       66 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.dockerignore
+-rw-r--r--   0        0        0      554 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      617 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.github/workflows/test.yml
+-rw-r--r--   0        0        0       85 2020-12-25 12:48:38.391175 django-ninja-0.9.7/.gitignore
+-rw-r--r--   0        0        0      930 2020-12-25 12:48:38.391175 django-ninja-0.9.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1086 2020-12-25 12:48:38.391175 django-ninja-0.9.7/LICENSE
+-rw-r--r--   0        0        0     2816 2020-12-25 12:48:38.391175 django-ninja-0.9.7/README.md
+-rw-r--r--   0        0        0     5904 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/async-support.md
+-rw-r--r--   0        0        0     1001 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/help.md
+-rw-r--r--   0        0        0    28154 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/img/auth-swagger-ui-prompt.png
+-rw-r--r--   0        0        0    27900 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/img/auth-swagger-ui.png
+-rw-r--r--   0        0        0    51900 2020-12-25 12:48:38.391175 django-ninja-0.9.7/docs/docs/img/benchmark.png
+-rw-r--r--   0        0        0   654914 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/body-editor.gif
+-rw-r--r--   0        0        0    46786 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/body-schema-doc.png
+-rw-r--r--   0        0        0    55925 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/body-schema-doc2.png
+-rw-r--r--   0        0        0    44459 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/deprecated.png
+-rw-r--r--   0        0        0     2717 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/docs-logo.png
+-rw-r--r--   0        0        0     6234 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/favicon.png
+-rw-r--r--   0        0        0     3439 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/github-star.png
+-rw-r--r--   0        0        0    18865 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/hero.png
+-rw-r--r--   0        0        0    95509 2020-12-25 12:48:38.395175 django-ninja-0.9.7/docs/docs/img/index-swagger-ui.png
+-rw-r--r--   0        0        0    12028 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/logo-big.png
+-rw-r--r--   0        0        0   122725 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/nested-routers-swagger.png
+-rw-r--r--   0        0        0    45259 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_description.png
+-rw-r--r--   0        0        0    53995 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_description_docstring.png
+-rw-r--r--   0        0        0    28482 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_summary.png
+-rw-r--r--   0        0        0    22627 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_summary_default.png
+-rw-r--r--   0        0        0    48354 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/operation_tags.png
+-rw-r--r--   0        0        0    65000 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/simple-routers-swagger.png
+-rw-r--r--   0        0        0   115803 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/img/tutorial-path-swagger.png
+-rw-r--r--   0        0        0     3304 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/index.md
+-rw-r--r--   0        0        0     2956 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/motivation.md
+-rw-r--r--   0        0        0     4653 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/proposals/cbv.md
+-rw-r--r--   0        0        0      492 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/proposals/index.md
+-rw-r--r--   0        0        0     3873 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/proposals/models.md
+-rw-r--r--   0        0        0      114 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/releases.md
+-rw-r--r--   0        0        0     3991 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/authentication.md
+-rw-r--r--   0        0        0     4569 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/body.md
+-rw-r--r--   0        0        0     5805 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/crud.md
+-rw-r--r--   0        0        0      816 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/csrf.md
+-rw-r--r--   0        0        0     1800 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/index.md
+-rw-r--r--   0        0        0     3221 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/operation_params.md
+-rw-r--r--   0        0        0     2844 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     2812 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     5289 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/response-schema.md
+-rw-r--r--   0        0        0     4145 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/routers.md
+-rw-r--r--   0        0        0     1480 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/docs/tutorial/versioning.md
+-rw-r--r--   0        0        0     1113 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/mkdocs.yml
+-rw-r--r--   0        0        0      274 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/index001.py
+-rw-r--r--   0        0        0      442 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/apikey01.py
+-rw-r--r--   0        0        0      322 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/apikey02.py
+-rw-r--r--   0        0        0      298 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/apikey03.py
+-rw-r--r--   0        0        0      314 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/basic01.py
+-rw-r--r--   0        0        0      271 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/bearer01.py
+-rw-r--r--   0        0        0      198 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/code001.py
+-rw-r--r--   0        0        0      231 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/code002.py
+-rw-r--r--   0        0        0      542 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/global01.py
+-rw-r--r--   0        0        0      390 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/multiple01.py
+-rw-r--r--   0        0        0        0 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/authentication/schema01.py
+-rw-r--r--   0        0        0      195 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/body/code01.py
+-rw-r--r--   0        0        0      255 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/body/code02.py
+-rw-r--r--   0        0        0      272 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/body/code03.py
+-rw-r--r--   0        0        0       94 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/path/code01.py
+-rw-r--r--   0        0        0      325 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/path/code010.py
+-rw-r--r--   0        0        0       99 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/path/code02.py
+-rw-r--r--   0        0        0      209 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code01.py
+-rw-r--r--   0        0        0      252 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code010.py
+-rw-r--r--   0        0        0      281 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code02.py
+-rw-r--r--   0        0        0      157 2020-12-25 12:48:38.399175 django-ninja-0.9.7/docs/src/tutorial/query/code03.py
+-rw-r--r--   0        0        0      233 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/__init__.py
+-rw-r--r--   0        0        0       52 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/compatibility/__init__.py
+-rw-r--r--   0        0        0     1734 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/compatibility/datastructures.py
+-rw-r--r--   0        0        0     1326 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/compatibility/request.py
+-rw-r--r--   0        0        0       19 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/constants.py
+-rw-r--r--   0        0        0      525 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/errors.py
+-rw-r--r--   0        0        0     7751 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/main.py
+-rw-r--r--   0        0        0       44 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/__init__.py
+-rw-r--r--   0        0        0     6824 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/schema.py
+-rw-r--r--   0        0        0      891 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/urls.py
+-rw-r--r--   0        0        0     1424 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/openapi/views.py
+-rw-r--r--   0        0        0     8806 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/operation.py
+-rw-r--r--   0        0        0     1631 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/params.py
+-rw-r--r--   0        0        0     2213 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/params_models.py
+-rw-r--r--   0        0        0      448 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/responses.py
+-rw-r--r--   0        0        0     6510 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/router.py
+-rw-r--r--   0        0        0     1135 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/schema.py
+-rw-r--r--   0        0        0      209 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/__init__.py
+-rw-r--r--   0        0        0      981 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/apikey.py
+-rw-r--r--   0        0        0      693 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/base.py
+-rw-r--r--   0        0        0     2171 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/http.py
+-rw-r--r--   0        0        0      322 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/security/session.py
+-rw-r--r--   0        0        0       93 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/signature/__init__.py
+-rw-r--r--   0        0        0     5115 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/signature/details.py
+-rw-r--r--   0        0        0     1429 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/signature/utils.py
+-rw-r--r--   0        0        0      956 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/templates/ninja/swagger.html
+-rw-r--r--   0        0        0      440 2020-12-25 12:48:38.403175 django-ninja-0.9.7/ninja/utils.py
+-rw-r--r--   0        0        0     1883 2020-12-25 12:48:38.403175 django-ninja-0.9.7/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2020-12-25 12:48:38.403175 django-ninja-0.9.7/scripts/build-docs.sh
+-rw-r--r--   0        0        0     3774 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/client.py
+-rw-r--r--   0        0        0      451 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/__init__.py
+-rw-r--r--   0        0        0      424 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/asgi.py
+-rw-r--r--   0        0        0     1645 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/settings.py
+-rw-r--r--   0        0        0      695 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/urls.py
+-rw-r--r--   0        0        0      424 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/demo/wsgi.py
+-rwxr-xr-x   0        0        0      657 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/manage.py
+-rw-r--r--   0        0        0        0 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/__init__.py
+-rw-r--r--   0        0        0       63 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/admin.py
+-rw-r--r--   0        0        0      707 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/api.py
+-rw-r--r--   0        0        0      308 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/models.py
+-rw-r--r--   0        0        0       63 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/demo_project/someapp/views.py
+-rw-r--r--   0        0        0     1519 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/Dockerfile
+-rw-r--r--   0        0        0     1865 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/Dockerfile.backup
+-rw-r--r--   0        0        0      291 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/README.md
+-rw-r--r--   0        0        0     1136 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/create_docker.py
+-rw-r--r--   0        0        0      111 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/docker-compose.yml
+-rw-r--r--   0        0        0      245 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/install_env.sh
+-rw-r--r--   0        0        0      132 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/env-matrix/run.sh
+-rw-r--r--   0        0        0     4248 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/main.py
+-rw-r--r--   0        0        0      106 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/pytest.ini
+-rw-r--r--   0        0        0      459 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_api_instance.py
+-rw-r--r--   0        0        0     2383 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_app.py
+-rw-r--r--   0        0        0     1394 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_async.py
+-rw-r--r--   0        0        0     4386 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_auth.py
+-rw-r--r--   0        0        0     2208 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_auth_global.py
+-rw-r--r--   0        0        0     1836 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_csrf.py
+-rw-r--r--   0        0        0      810 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_django_models.py
+-rw-r--r--   0        0        0        0 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/__init__.py
+-rw-r--r--   0        0        0     3607 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_auth.py
+-rw-r--r--   0        0        0     1326 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_body.py
+-rw-r--r--   0        0        0      197 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_index.py
+-rw-r--r--   0        0        0     1182 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_path.py
+-rw-r--r--   0        0        0     3259 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_docs/test_query.py
+-rw-r--r--   0        0        0     2545 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_enum.py
+-rw-r--r--   0        0        0      932 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_inheritance_routers.py
+-rw-r--r--   0        0        0     2377 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_lists.py
+-rw-r--r--   0        0        0      247 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_misc.py
+-rw-r--r--   0        0        0     3397 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_models.py
+-rw-r--r--   0        0        0     1742 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_openapi_params.py
+-rw-r--r--   0        0        0     2810 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_openapi_schema.py
+-rw-r--r--   0        0        0     7643 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_path.py
+-rw-r--r--   0        0        0     2168 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_query.py
+-rw-r--r--   0        0        0     1410 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_request.py
+-rw-r--r--   0        0        0     1985 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_response.py
+-rw-r--r--   0        0        0     3783 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_response_multiple.py
+-rw-r--r--   0        0        0     1823 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_schema.py
+-rw-r--r--   0        0        0      465 2020-12-25 12:48:38.403175 django-ninja-0.9.7/tests/test_union.py
+-rw-r--r--   0        0        0      947 1970-01-01 00:00:00.000000 django-ninja-0.9.7/setup.py
+-rw-r--r--   0        0        0      221 1970-01-01 00:00:00.000000 django-ninja-0.9.7/PKG-INFO
```

### Comparing `django-ninja-0.9.6/.github/workflows/publish.yml` & `django-ninja-0.9.7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/.github/workflows/test.yml` & `django-ninja-0.9.7/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/CONTRIBUTING.md` & `django-ninja-0.9.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/LICENSE` & `django-ninja-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/README.md` & `django-ninja-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/async-support.md` & `django-ninja-0.9.7/docs/docs/async-support.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/help.md` & `django-ninja-0.9.7/docs/docs/help.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/auth-swagger-ui-prompt.png` & `django-ninja-0.9.7/docs/docs/img/auth-swagger-ui-prompt.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/auth-swagger-ui.png` & `django-ninja-0.9.7/docs/docs/img/auth-swagger-ui.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/benchmark.png` & `django-ninja-0.9.7/docs/docs/img/benchmark.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/body-editor.gif` & `django-ninja-0.9.7/docs/docs/img/body-editor.gif`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/body-schema-doc.png` & `django-ninja-0.9.7/docs/docs/img/body-schema-doc.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/body-schema-doc2.png` & `django-ninja-0.9.7/docs/docs/img/body-schema-doc2.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/deprecated.png` & `django-ninja-0.9.7/docs/docs/img/deprecated.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/docs-logo.png` & `django-ninja-0.9.7/docs/docs/img/docs-logo.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/favicon.png` & `django-ninja-0.9.7/docs/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/github-star.png` & `django-ninja-0.9.7/docs/docs/img/github-star.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/hero.png` & `django-ninja-0.9.7/docs/docs/img/hero.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/index-swagger-ui.png` & `django-ninja-0.9.7/docs/docs/img/index-swagger-ui.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/logo-big.png` & `django-ninja-0.9.7/docs/docs/img/logo-big.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/nested-routers-swagger.png` & `django-ninja-0.9.7/docs/docs/img/nested-routers-swagger.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/operation_description.png` & `django-ninja-0.9.7/docs/docs/img/operation_description.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/operation_description_docstring.png` & `django-ninja-0.9.7/docs/docs/img/operation_description_docstring.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/operation_summary.png` & `django-ninja-0.9.7/docs/docs/img/operation_summary.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/operation_summary_default.png` & `django-ninja-0.9.7/docs/docs/img/operation_summary_default.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/operation_tags.png` & `django-ninja-0.9.7/docs/docs/img/operation_tags.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/simple-routers-swagger.png` & `django-ninja-0.9.7/docs/docs/img/simple-routers-swagger.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/img/tutorial-path-swagger.png` & `django-ninja-0.9.7/docs/docs/img/tutorial-path-swagger.png`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/index.md` & `django-ninja-0.9.7/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/motivation.md` & `django-ninja-0.9.7/docs/docs/motivation.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/proposals/cbv.md` & `django-ninja-0.9.7/docs/docs/proposals/cbv.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/proposals/models.md` & `django-ninja-0.9.7/docs/docs/proposals/models.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/authentication.md` & `django-ninja-0.9.7/docs/docs/tutorial/authentication.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/body.md` & `django-ninja-0.9.7/docs/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/crud.md` & `django-ninja-0.9.7/docs/docs/tutorial/crud.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/csrf.md` & `django-ninja-0.9.7/docs/docs/tutorial/csrf.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/index.md` & `django-ninja-0.9.7/docs/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/operation_params.md` & `django-ninja-0.9.7/docs/docs/tutorial/operation_params.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/path-params.md` & `django-ninja-0.9.7/docs/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/query-params.md` & `django-ninja-0.9.7/docs/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/response-schema.md` & `django-ninja-0.9.7/docs/docs/tutorial/response-schema.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/routers.md` & `django-ninja-0.9.7/docs/docs/tutorial/routers.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/docs/tutorial/versioning.md` & `django-ninja-0.9.7/docs/docs/tutorial/versioning.md`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/mkdocs.yml` & `django-ninja-0.9.7/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/docs/src/tutorial/authentication/global01.py` & `django-ninja-0.9.7/docs/src/tutorial/authentication/global01.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/compatibility/datastructures.py` & `django-ninja-0.9.7/ninja/compatibility/datastructures.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/compatibility/request.py` & `django-ninja-0.9.7/ninja/compatibility/request.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/errors.py` & `django-ninja-0.9.7/ninja/errors.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/main.py` & `django-ninja-0.9.7/ninja/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,16 @@
 
     @property
     def urls(self):
         self._validate()
         return (
             self._get_urls(),
             "ninja",
-            self.urls_namespace,
+            self.urls_namespace.split(":")[-1],
+            # ^ if api included into nested urls, we only care about last bit here
         )
 
     def _get_urls(self):
         result = get_openapi_urls(self)
 
         for prefix, router in self._routers:
             for path in router.urls_paths(prefix):
```

### Comparing `django-ninja-0.9.6/ninja/openapi/schema.py` & `django-ninja-0.9.7/ninja/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/openapi/urls.py` & `django-ninja-0.9.7/ninja/openapi/urls.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/openapi/views.py` & `django-ninja-0.9.7/ninja/openapi/views.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/operation.py` & `django-ninja-0.9.7/ninja/operation.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/params.py` & `django-ninja-0.9.7/ninja/params.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/params_models.py` & `django-ninja-0.9.7/ninja/params_models.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/router.py` & `django-ninja-0.9.7/ninja/router.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/schema.py` & `django-ninja-0.9.7/ninja/schema.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/security/apikey.py` & `django-ninja-0.9.7/ninja/security/apikey.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/security/base.py` & `django-ninja-0.9.7/ninja/security/base.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/security/http.py` & `django-ninja-0.9.7/ninja/security/http.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/signature/details.py` & `django-ninja-0.9.7/ninja/signature/details.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/signature/utils.py` & `django-ninja-0.9.7/ninja/signature/utils.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/ninja/templates/ninja/swagger.html` & `django-ninja-0.9.7/ninja/templates/ninja/swagger.html`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/pyproject.toml` & `django-ninja-0.9.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/client.py` & `django-ninja-0.9.7/tests/client.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/demo_project/demo/settings.py` & `django-ninja-0.9.7/tests/demo_project/demo/settings.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/demo_project/demo/urls.py` & `django-ninja-0.9.7/tests/demo_project/demo/urls.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/demo_project/manage.py` & `django-ninja-0.9.7/tests/demo_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/demo_project/someapp/api.py` & `django-ninja-0.9.7/tests/demo_project/someapp/api.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/env-matrix/Dockerfile` & `django-ninja-0.9.7/tests/env-matrix/Dockerfile`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/env-matrix/Dockerfile.backup` & `django-ninja-0.9.7/tests/env-matrix/Dockerfile.backup`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/env-matrix/create_docker.py` & `django-ninja-0.9.7/tests/env-matrix/create_docker.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/main.py` & `django-ninja-0.9.7/tests/main.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_app.py` & `django-ninja-0.9.7/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_async.py` & `django-ninja-0.9.7/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_auth.py` & `django-ninja-0.9.7/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_auth_global.py` & `django-ninja-0.9.7/tests/test_auth_global.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_csrf.py` & `django-ninja-0.9.7/tests/test_csrf.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_django_models.py` & `django-ninja-0.9.7/tests/test_django_models.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_docs/test_auth.py` & `django-ninja-0.9.7/tests/test_docs/test_auth.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_docs/test_body.py` & `django-ninja-0.9.7/tests/test_docs/test_body.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_docs/test_path.py` & `django-ninja-0.9.7/tests/test_docs/test_path.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_docs/test_query.py` & `django-ninja-0.9.7/tests/test_docs/test_query.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_enum.py` & `django-ninja-0.9.7/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_inheritance_routers.py` & `django-ninja-0.9.7/tests/test_inheritance_routers.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_lists.py` & `django-ninja-0.9.7/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_models.py` & `django-ninja-0.9.7/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_openapi_params.py` & `django-ninja-0.9.7/tests/test_openapi_params.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_openapi_schema.py` & `django-ninja-0.9.7/tests/test_openapi_schema.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_path.py` & `django-ninja-0.9.7/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_query.py` & `django-ninja-0.9.7/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_request.py` & `django-ninja-0.9.7/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_response.py` & `django-ninja-0.9.7/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_response_multiple.py` & `django-ninja-0.9.7/tests/test_response_multiple.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/tests/test_schema.py` & `django-ninja-0.9.7/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `django-ninja-0.9.6/setup.py` & `django-ninja-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['Django >=2.0.13', 'pydantic >=1.6,<1.8']
 
 extras_require = \
 {'doc': ['mkdocs', 'mkdocs-material', 'markdown-include'],
  'test': ['pytest', 'pytest-cov', 'pytest-django', 'pytest-asyncio', 'black']}
 
 setup(name='django-ninja',
-      version='0.9.6',
+      version='0.9.7',
       description='Django Ninja - Fast Django REST framework',
       author='Vitaliy Kucheryaviy',
       author_email='ppr.vitaly@gmail.com',
       url='https://django-ninja.rest-framework.com',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

