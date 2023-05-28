# Comparing `tmp/lnhub_rest-0.9.7.tar.gz` & `tmp/lnhub_rest-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.9.7.tar", last modified: Sun May 28 12:37:23 2023, max compression
+gzip compressed data, was "lnhub_rest-0.9.8.tar", last modified: Sun May 28 13:31:31 2023, max compression
```

## Comparing `lnhub_rest-0.9.7.tar` & `lnhub_rest-0.9.8.tar`

### file list

```diff
@@ -1,201 +1,201 @@
--rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.9.7/.dockerignore
--rw-r--r--   0        0        0     3245 2023-05-25 20:34:20.149969 lnhub_rest-0.9.7/.github/workflows/build.yml
--rw-r--r--   0        0        0     5417 2023-05-25 20:34:20.150136 lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-prod.yml
--rw-r--r--   0        0        0     5426 2023-05-25 20:34:20.150292 lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-staging.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.9.7/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.9.7/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.9.7/.gitignore
--rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.9.7/.gitmodules
--rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.9.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.9.7/Dockerfile
--rw-r--r--   0        0        0     2442 2023-04-25 15:29:32.847024 lnhub_rest-0.9.7/README.md
--rw-r--r--   0        0        0     1680 2023-04-27 03:39:31.402324 lnhub_rest-0.9.7/docs/00-migrate.ipynb
--rw-r--r--   0        0        0     1189 2023-04-27 03:39:31.402860 lnhub_rest-0.9.7/docs/01-checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0     4487 2023-04-27 03:39:31.414955 lnhub_rest-0.9.7/docs/02-account/02-create-account.ipynb
--rw-r--r--   0        0        0     5566 2023-04-27 03:39:31.419067 lnhub_rest-0.9.7/docs/02-account/03-update-account.ipynb
--rw-r--r--   0        0        0     6111 2023-04-27 03:39:31.418992 lnhub_rest-0.9.7/docs/02-account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9088 2023-04-27 03:39:31.419398 lnhub_rest-0.9.7/docs/02-account/05-rls.ipynb
--rw-r--r--   0        0        0    11110 2023-04-27 04:21:53.504972 lnhub_rest-0.9.7/docs/03-instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5293 2023-04-27 03:39:31.415575 lnhub_rest-0.9.7/docs/03-instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6498 2023-04-27 03:39:31.417147 lnhub_rest-0.9.7/docs/03-instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     8667 2023-04-27 03:39:31.417306 lnhub_rest-0.9.7/docs/03-instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     7001 2023-04-27 03:39:31.420904 lnhub_rest-0.9.7/docs/03-instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19423 2023-04-27 03:39:31.401299 lnhub_rest-0.9.7/docs/03-instance/06-rls.ipynb
--rw-r--r--   0        0        0     3990 2023-04-27 04:21:53.505189 lnhub_rest-0.9.7/docs/04-storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9837 2023-04-27 03:39:31.421340 lnhub_rest-0.9.7/docs/04-storage/02-rls.ipynb
--rw-r--r--   0        0        0     3894 2023-04-27 03:39:31.415314 lnhub_rest-0.9.7/docs/05-organization/01-create-organization.ipynb
--rw-r--r--   0        0        0     4749 2023-04-27 03:39:31.413247 lnhub_rest-0.9.7/docs/05-organization/02-manage-members.ipynb
--rw-r--r--   0        0        0     5892 2023-04-27 03:39:31.413014 lnhub_rest-0.9.7/docs/05-organization/03-rls.ipynb
--rw-r--r--   0        0        0     5310 2023-04-27 03:39:31.417221 lnhub_rest-0.9.7/docs/06-integration/01-signup-signin.ipynb
--rw-r--r--   0        0        0      125 2023-04-18 16:52:57.348114 lnhub_rest-0.9.7/docs/README.md
--rw-r--r--   0        0        0    25029 2023-05-28 12:37:03.229477 lnhub_rest-0.9.7/docs/changelog.md
--rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.9.7/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.9.7/docs/notes/index.md
--rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.9.7/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.9.7/lamin-project.yaml
--rw-r--r--   0        0        0     3832 2023-04-18 16:53:14.549682 lnhub_rest-0.9.7/lndb/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.9.7/lndb/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.9.7/lndb/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.9.7/lndb/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-25 15:29:40.845175 lnhub_rest-0.9.7/lndb/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.9.7/lndb/LICENSE
--rw-r--r--   0        0        0      173 2023-04-18 16:53:14.549987 lnhub_rest-0.9.7/lndb/README.md
--rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.9.7/lndb/docs/api.md
--rw-r--r--   0        0        0    47755 2023-04-27 03:47:05.803728 lnhub_rest-0.9.7/lndb/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.9.7/lndb/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.9.7/lndb/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-04-18 16:53:14.550717 lnhub_rest-0.9.7/lndb/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-04-18 16:53:14.551192 lnhub_rest-0.9.7/lndb/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-25 15:29:40.845949 lnhub_rest-0.9.7/lndb/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.9.7/lndb/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-18 16:53:14.551375 lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-18 16:53:14.551472 lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-18 16:53:14.551612 lnhub_rest-0.9.7/lndb/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10370 2023-04-27 04:20:38.053396 lnhub_rest-0.9.7/lndb/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5355 2023-04-25 15:29:40.846776 lnhub_rest-0.9.7/lndb/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6390 2023-04-25 15:29:40.846861 lnhub_rest-0.9.7/lndb/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3746 2023-04-25 15:29:40.846961 lnhub_rest-0.9.7/lndb/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-04-18 16:53:14.552137 lnhub_rest-0.9.7/lndb/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-25 15:29:40.847226 lnhub_rest-0.9.7/lndb/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.9.7/lndb/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-25 15:29:40.847416 lnhub_rest-0.9.7/lndb/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.9.7/lndb/docs/index.md
--rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.9.7/lndb/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-27 03:47:05.803990 lnhub_rest-0.9.7/lndb/lndb/__init__.py
--rw-r--r--   0        0        0     4507 2023-04-25 15:29:40.847751 lnhub_rest-0.9.7/lndb/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.9.7/lndb/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-18 16:53:14.553281 lnhub_rest-0.9.7/lndb/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-25 15:29:40.847842 lnhub_rest-0.9.7/lndb/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-18 16:53:14.553610 lnhub_rest-0.9.7/lndb/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-18 16:53:14.553765 lnhub_rest-0.9.7/lndb/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-25 15:29:40.848070 lnhub_rest-0.9.7/lndb/lndb/_info.py
--rw-r--r--   0        0        0     6035 2023-04-27 03:52:24.150379 lnhub_rest-0.9.7/lndb/lndb/_init_instance.py
--rw-r--r--   0        0        0     6485 2023-04-27 03:49:23.883095 lnhub_rest-0.9.7/lndb/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-18 16:53:14.554421 lnhub_rest-0.9.7/lndb/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-18 16:53:14.554545 lnhub_rest-0.9.7/lndb/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-25 15:29:40.848442 lnhub_rest-0.9.7/lndb/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-25 15:29:40.848595 lnhub_rest-0.9.7/lndb/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.9.7/lndb/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-25 15:29:40.848722 lnhub_rest-0.9.7/lndb/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-18 16:53:14.554944 lnhub_rest-0.9.7/lndb/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      803 2023-04-27 04:20:38.053795 lnhub_rest-0.9.7/lndb/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.9.7/lndb/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-25 15:29:40.849016 lnhub_rest-0.9.7/lndb/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 21:34:53.593994 lnhub_rest-0.9.7/lndb/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.9.7/lndb/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.9.7/lndb/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-25 15:29:40.849262 lnhub_rest-0.9.7/lndb/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-18 16:53:14.555545 lnhub_rest-0.9.7/lndb/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-04-18 16:53:14.555802 lnhub_rest-0.9.7/lndb/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-18 16:53:14.555956 lnhub_rest-0.9.7/lndb/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.9.7/lndb/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.9.7/lndb/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-18 16:53:14.556103 lnhub_rest-0.9.7/lndb/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-04-27 03:49:23.883399 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-04-18 16:53:14.556382 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-18 16:53:14.556505 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-04-18 16:53:14.556633 lnhub_rest-0.9.7/lndb/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-25 15:29:40.849676 lnhub_rest-0.9.7/lndb/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-25 15:29:40.849829 lnhub_rest-0.9.7/lndb/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.9.7/lndb/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-18 16:53:14.557004 lnhub_rest-0.9.7/lndb/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-18 16:53:14.557144 lnhub_rest-0.9.7/lndb/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.9.7/lndb/lndb/test/_env.py
--rw-r--r--   0        0        0     3911 2023-04-27 03:52:24.153553 lnhub_rest-0.9.7/lndb/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-18 16:53:14.557417 lnhub_rest-0.9.7/lndb/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.9.7/lndb/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.9.7/lndb/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-18 16:53:14.557535 lnhub_rest-0.9.7/lndb/noxfile.py
--rw-r--r--   0        0        0     1396 2023-04-27 04:20:38.053974 lnhub_rest-0.9.7/lndb/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-18 16:53:14.557862 lnhub_rest-0.9.7/lndb/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.9.7/lndb/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:53:14.558657 lnhub_rest-0.9.7/lndb/tests/test_notebooks.py
--rw-r--r--   0        0        0      157 2023-05-28 12:36:54.490184 lnhub_rest-0.9.7/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     7054 2023-04-25 15:29:32.854635 lnhub_rest-0.9.7/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.9.7/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0      706 2023-05-28 12:36:10.508939 lnhub_rest-0.9.7/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1109 2023-05-25 20:34:20.151651 lnhub_rest-0.9.7/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.9.7/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0     1260 2023-04-25 15:29:32.854787 lnhub_rest-0.9.7/lnhub_rest/_ci.py
--rw-r--r--   0        0        0     5726 2023-04-19 15:57:22.490723 lnhub_rest-0.9.7/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0     1626 2023-05-28 12:14:52.784375 lnhub_rest-0.9.7/lnhub_rest/config.py
--rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.9.7/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.9.7/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     2542 2023-04-21 10:12:34.724799 lnhub_rest-0.9.7/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.9.7/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      739 2023-04-19 15:57:22.491329 lnhub_rest-0.9.7/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3325 2023-04-19 15:57:22.491711 lnhub_rest-0.9.7/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1423 2023-04-19 15:57:22.491949 lnhub_rest-0.9.7/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.9.7/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     3056 2023-04-25 15:29:32.855696 lnhub_rest-0.9.7/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.9.7/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.9.7/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1284 2023-04-19 15:57:22.492340 lnhub_rest-0.9.7/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6096 2023-04-27 04:21:53.505412 lnhub_rest-0.9.7/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1532 2023-04-19 15:57:22.492860 lnhub_rest-0.9.7/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1067 2023-04-19 15:57:22.493104 lnhub_rest-0.9.7/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.9.7/lnhub_rest/core/member/__init__.py
--rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.9.7/lnhub_rest/core/member/_crud.py
--rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.9.7/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     3427 2023-05-28 12:14:52.784992 lnhub_rest-0.9.7/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.9.7/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      849 2023-05-25 20:34:20.151769 lnhub_rest-0.9.7/lnhub_rest/main.py
--rw-r--r--   0        0        0       39 2023-04-19 15:57:22.493742 lnhub_rest-0.9.7/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      199 2023-04-25 15:29:32.856194 lnhub_rest-0.9.7/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     1968 2023-04-25 15:29:32.856453 lnhub_rest-0.9.7/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      239 2023-05-25 20:34:20.152255 lnhub_rest-0.9.7/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     4661 2023-04-25 15:29:32.856734 lnhub_rest-0.9.7/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.9.7/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0     2313 2023-05-25 20:34:20.152366 lnhub_rest-0.9.7/lnhub_rest/routers/collaborator.py
--rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.9.7/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     5233 2023-04-25 15:29:32.856998 lnhub_rest-0.9.7/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.9.7/lnhub_rest/routers/organization.py
--rw-r--r--   0        0        0     1074 2023-04-19 15:57:22.494317 lnhub_rest-0.9.7/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.9.7/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.9.7/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.9.7/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.9.7/lnhub_rest/schema/_type.py
--rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.9.7/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.9.7/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.9.7/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       40 2023-04-25 15:29:32.857365 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/clone.py
--rw-r--r--   0        0        0     3033 2023-04-25 15:29:32.857603 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
--rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
--rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0     5258 2023-04-25 15:29:32.857771 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/testing.py
--rw-r--r--   0        0        0     9882 2023-04-18 16:52:57.349405 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-04-18 16:52:57.349781 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
--rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
--rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
--rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
--rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.9.7/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.9.7/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.9.7/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.9.7/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.9.7/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3820 2023-04-19 15:57:22.494545 lnhub_rest-0.9.7/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1728 2023-05-28 12:36:10.509265 lnhub_rest-0.9.7/noxfile.py
--rw-r--r--   0        0        0     1139 2023-05-28 12:36:10.509601 lnhub_rest-0.9.7/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.9.7/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.9.7/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.9.7/supabase/config.toml
--rw-r--r--   0        0        0     1212 2023-04-25 15:29:32.858221 lnhub_rest-0.9.7/tests/test_notebooks.py
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 lnhub_rest-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.9.8/.dockerignore
+-rw-r--r--   0        0        0     3245 2023-05-25 20:34:20.149969 lnhub_rest-0.9.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5417 2023-05-25 20:34:20.150136 lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-prod.yml
+-rw-r--r--   0        0        0     5426 2023-05-25 20:34:20.150292 lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-staging.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.9.8/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.9.8/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.9.8/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.9.8/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.9.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.9.8/Dockerfile
+-rw-r--r--   0        0        0     2442 2023-04-25 15:29:32.847024 lnhub_rest-0.9.8/README.md
+-rw-r--r--   0        0        0     1680 2023-04-27 03:39:31.402324 lnhub_rest-0.9.8/docs/00-migrate.ipynb
+-rw-r--r--   0        0        0     1189 2023-04-27 03:39:31.402860 lnhub_rest-0.9.8/docs/01-checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0     4487 2023-04-27 03:39:31.414955 lnhub_rest-0.9.8/docs/02-account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5566 2023-04-27 03:39:31.419067 lnhub_rest-0.9.8/docs/02-account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6111 2023-04-27 03:39:31.418992 lnhub_rest-0.9.8/docs/02-account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9088 2023-04-27 03:39:31.419398 lnhub_rest-0.9.8/docs/02-account/05-rls.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-27 04:21:53.504972 lnhub_rest-0.9.8/docs/03-instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5293 2023-04-27 03:39:31.415575 lnhub_rest-0.9.8/docs/03-instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6498 2023-04-27 03:39:31.417147 lnhub_rest-0.9.8/docs/03-instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8667 2023-04-27 03:39:31.417306 lnhub_rest-0.9.8/docs/03-instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     7001 2023-04-27 03:39:31.420904 lnhub_rest-0.9.8/docs/03-instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19423 2023-04-27 03:39:31.401299 lnhub_rest-0.9.8/docs/03-instance/06-rls.ipynb
+-rw-r--r--   0        0        0     3990 2023-04-27 04:21:53.505189 lnhub_rest-0.9.8/docs/04-storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9837 2023-04-27 03:39:31.421340 lnhub_rest-0.9.8/docs/04-storage/02-rls.ipynb
+-rw-r--r--   0        0        0     3894 2023-04-27 03:39:31.415314 lnhub_rest-0.9.8/docs/05-organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     4749 2023-04-27 03:39:31.413247 lnhub_rest-0.9.8/docs/05-organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5892 2023-04-27 03:39:31.413014 lnhub_rest-0.9.8/docs/05-organization/03-rls.ipynb
+-rw-r--r--   0        0        0     5310 2023-04-27 03:39:31.417221 lnhub_rest-0.9.8/docs/06-integration/01-signup-signin.ipynb
+-rw-r--r--   0        0        0      125 2023-04-18 16:52:57.348114 lnhub_rest-0.9.8/docs/README.md
+-rw-r--r--   0        0        0    25029 2023-05-28 13:31:14.587869 lnhub_rest-0.9.8/docs/changelog.md
+-rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.9.8/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.9.8/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.9.8/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.9.8/lamin-project.yaml
+-rw-r--r--   0        0        0     3832 2023-04-18 16:53:14.549682 lnhub_rest-0.9.8/lndb/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.9.8/lndb/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.9.8/lndb/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.9.8/lndb/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-25 15:29:40.845175 lnhub_rest-0.9.8/lndb/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.9.8/lndb/LICENSE
+-rw-r--r--   0        0        0      173 2023-04-18 16:53:14.549987 lnhub_rest-0.9.8/lndb/README.md
+-rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.9.8/lndb/docs/api.md
+-rw-r--r--   0        0        0    47755 2023-04-27 03:47:05.803728 lnhub_rest-0.9.8/lndb/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.9.8/lndb/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.9.8/lndb/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-04-18 16:53:14.550717 lnhub_rest-0.9.8/lndb/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-04-18 16:53:14.551192 lnhub_rest-0.9.8/lndb/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-25 15:29:40.845949 lnhub_rest-0.9.8/lndb/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.9.8/lndb/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-18 16:53:14.551375 lnhub_rest-0.9.8/lndb/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-18 16:53:14.551472 lnhub_rest-0.9.8/lndb/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-18 16:53:14.551612 lnhub_rest-0.9.8/lndb/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10370 2023-04-27 04:20:38.053396 lnhub_rest-0.9.8/lndb/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-25 15:29:40.846776 lnhub_rest-0.9.8/lndb/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-25 15:29:40.846861 lnhub_rest-0.9.8/lndb/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-25 15:29:40.846961 lnhub_rest-0.9.8/lndb/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-04-18 16:53:14.552137 lnhub_rest-0.9.8/lndb/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-25 15:29:40.847226 lnhub_rest-0.9.8/lndb/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.9.8/lndb/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-25 15:29:40.847416 lnhub_rest-0.9.8/lndb/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.9.8/lndb/docs/index.md
+-rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.9.8/lndb/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-27 03:47:05.803990 lnhub_rest-0.9.8/lndb/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-25 15:29:40.847751 lnhub_rest-0.9.8/lndb/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.9.8/lndb/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-18 16:53:14.553281 lnhub_rest-0.9.8/lndb/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-25 15:29:40.847842 lnhub_rest-0.9.8/lndb/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-18 16:53:14.553610 lnhub_rest-0.9.8/lndb/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-18 16:53:14.553765 lnhub_rest-0.9.8/lndb/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-25 15:29:40.848070 lnhub_rest-0.9.8/lndb/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-04-27 03:52:24.150379 lnhub_rest-0.9.8/lndb/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6485 2023-04-27 03:49:23.883095 lnhub_rest-0.9.8/lndb/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-18 16:53:14.554421 lnhub_rest-0.9.8/lndb/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-18 16:53:14.554545 lnhub_rest-0.9.8/lndb/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-25 15:29:40.848442 lnhub_rest-0.9.8/lndb/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-25 15:29:40.848595 lnhub_rest-0.9.8/lndb/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.9.8/lndb/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-25 15:29:40.848722 lnhub_rest-0.9.8/lndb/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-18 16:53:14.554944 lnhub_rest-0.9.8/lndb/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      803 2023-04-27 04:20:38.053795 lnhub_rest-0.9.8/lndb/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.9.8/lndb/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-25 15:29:40.849016 lnhub_rest-0.9.8/lndb/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 21:34:53.593994 lnhub_rest-0.9.8/lndb/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.9.8/lndb/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.9.8/lndb/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-25 15:29:40.849262 lnhub_rest-0.9.8/lndb/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-18 16:53:14.555545 lnhub_rest-0.9.8/lndb/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-04-18 16:53:14.555802 lnhub_rest-0.9.8/lndb/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-18 16:53:14.555956 lnhub_rest-0.9.8/lndb/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.9.8/lndb/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.9.8/lndb/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-18 16:53:14.556103 lnhub_rest-0.9.8/lndb/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-04-27 03:49:23.883399 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-04-18 16:53:14.556382 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-18 16:53:14.556505 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.9.8/lndb/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-04-18 16:53:14.556633 lnhub_rest-0.9.8/lndb/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-25 15:29:40.849676 lnhub_rest-0.9.8/lndb/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-25 15:29:40.849829 lnhub_rest-0.9.8/lndb/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.9.8/lndb/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-18 16:53:14.557004 lnhub_rest-0.9.8/lndb/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-18 16:53:14.557144 lnhub_rest-0.9.8/lndb/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.9.8/lndb/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-04-27 03:52:24.153553 lnhub_rest-0.9.8/lndb/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-18 16:53:14.557417 lnhub_rest-0.9.8/lndb/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.9.8/lndb/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.9.8/lndb/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-18 16:53:14.557535 lnhub_rest-0.9.8/lndb/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-27 04:20:38.053974 lnhub_rest-0.9.8/lndb/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-18 16:53:14.557862 lnhub_rest-0.9.8/lndb/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.9.8/lndb/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:53:14.558657 lnhub_rest-0.9.8/lndb/tests/test_notebooks.py
+-rw-r--r--   0        0        0      157 2023-05-28 13:31:08.333660 lnhub_rest-0.9.8/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     7054 2023-04-25 15:29:32.854635 lnhub_rest-0.9.8/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.9.8/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0      706 2023-05-28 12:36:10.508939 lnhub_rest-0.9.8/lnhub_rest/_assets/_instances.py
+-rw-r--r--   0        0        0     1109 2023-05-25 20:34:20.151651 lnhub_rest-0.9.8/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.9.8/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0     1260 2023-04-25 15:29:32.854787 lnhub_rest-0.9.8/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5726 2023-04-19 15:57:22.490723 lnhub_rest-0.9.8/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0     1626 2023-05-28 12:14:52.784375 lnhub_rest-0.9.8/lnhub_rest/config.py
+-rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.9.8/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.9.8/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2542 2023-04-21 10:12:34.724799 lnhub_rest-0.9.8/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.9.8/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      739 2023-04-19 15:57:22.491329 lnhub_rest-0.9.8/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3325 2023-04-19 15:57:22.491711 lnhub_rest-0.9.8/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1423 2023-04-19 15:57:22.491949 lnhub_rest-0.9.8/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.9.8/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     3056 2023-04-25 15:29:32.855696 lnhub_rest-0.9.8/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.9.8/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.9.8/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1284 2023-04-19 15:57:22.492340 lnhub_rest-0.9.8/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6096 2023-04-27 04:21:53.505412 lnhub_rest-0.9.8/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1532 2023-04-19 15:57:22.492860 lnhub_rest-0.9.8/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1067 2023-04-19 15:57:22.493104 lnhub_rest-0.9.8/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.9.8/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.9.8/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.9.8/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     3427 2023-05-28 12:14:52.784992 lnhub_rest-0.9.8/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.9.8/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      849 2023-05-25 20:34:20.151769 lnhub_rest-0.9.8/lnhub_rest/main.py
+-rw-r--r--   0        0        0       39 2023-04-19 15:57:22.493742 lnhub_rest-0.9.8/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      199 2023-04-25 15:29:32.856194 lnhub_rest-0.9.8/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     1968 2023-04-25 15:29:32.856453 lnhub_rest-0.9.8/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      239 2023-05-25 20:34:20.152255 lnhub_rest-0.9.8/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4661 2023-04-25 15:29:32.856734 lnhub_rest-0.9.8/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.9.8/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0     2313 2023-05-25 20:34:20.152366 lnhub_rest-0.9.8/lnhub_rest/routers/collaborator.py
+-rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.9.8/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     5233 2023-04-25 15:29:32.856998 lnhub_rest-0.9.8/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.9.8/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1074 2023-04-19 15:57:22.494317 lnhub_rest-0.9.8/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.9.8/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.9.8/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.9.8/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.9.8/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.9.8/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.9.8/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.9.8/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       40 2023-04-25 15:29:32.857365 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     3033 2023-04-25 15:29:32.857603 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0     5258 2023-04-25 15:29:32.857771 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     9882 2023-04-18 16:52:57.349405 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-04-18 16:52:57.349781 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.9.8/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.9.8/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.9.8/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.9.8/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.9.8/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3820 2023-04-19 15:57:22.494545 lnhub_rest-0.9.8/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1728 2023-05-28 12:36:10.509265 lnhub_rest-0.9.8/noxfile.py
+-rw-r--r--   0        0        0     1152 2023-05-28 13:30:17.362252 lnhub_rest-0.9.8/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.9.8/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.9.8/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.9.8/supabase/config.toml
+-rw-r--r--   0        0        0     1212 2023-04-25 15:29:32.858221 lnhub_rest-0.9.8/tests/test_notebooks.py
+-rw-r--r--   0        0        0     3353 1970-01-01 00:00:00.000000 lnhub_rest-0.9.8/PKG-INFO
```

### Comparing `lnhub_rest-0.9.7/.dockerignore` & `lnhub_rest-0.9.8/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/.github/workflows/build.yml` & `lnhub_rest-0.9.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-prod.yml` & `lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-prod.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-staging.yml` & `lnhub_rest-0.9.8/.github/workflows/google-cloudrun-docker-staging.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.8/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/.gitignore` & `lnhub_rest-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/.pre-commit-config.yaml` & `lnhub_rest-0.9.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/README.md` & `lnhub_rest-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/00-migrate.ipynb` & `lnhub_rest-0.9.8/docs/00-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/01-checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.9.8/docs/01-checks/01-check-break-lndb.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/02-account/02-create-account.ipynb` & `lnhub_rest-0.9.8/docs/02-account/02-create-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/02-account/03-update-account.ipynb` & `lnhub_rest-0.9.8/docs/02-account/03-update-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/02-account/04-fetch-account.ipynb` & `lnhub_rest-0.9.8/docs/02-account/04-fetch-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/02-account/05-rls.ipynb` & `lnhub_rest-0.9.8/docs/02-account/05-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/03-instance/01-init-instance.ipynb` & `lnhub_rest-0.9.8/docs/03-instance/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/03-instance/02-load-instance.ipynb` & `lnhub_rest-0.9.8/docs/03-instance/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/03-instance/03-update-instance.ipynb` & `lnhub_rest-0.9.8/docs/03-instance/03-update-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/03-instance/04-delete-instance.ipynb` & `lnhub_rest-0.9.8/docs/03-instance/04-delete-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/03-instance/05-fetch-instance.ipynb` & `lnhub_rest-0.9.8/docs/03-instance/05-fetch-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/03-instance/06-rls.ipynb` & `lnhub_rest-0.9.8/docs/03-instance/06-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/04-storage/01-add-storage.ipynb` & `lnhub_rest-0.9.8/docs/04-storage/01-add-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/04-storage/02-rls.ipynb` & `lnhub_rest-0.9.8/docs/04-storage/02-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/05-organization/01-create-organization.ipynb` & `lnhub_rest-0.9.8/docs/05-organization/01-create-organization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/05-organization/02-manage-members.ipynb` & `lnhub_rest-0.9.8/docs/05-organization/02-manage-members.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/05-organization/03-rls.ipynb` & `lnhub_rest-0.9.8/docs/05-organization/03-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/06-integration/01-signup-signin.ipynb` & `lnhub_rest-0.9.8/docs/06-integration/01-signup-signin.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/changelog.md` & `lnhub_rest-0.9.8/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-➖ Simplify dependencies | [208](https://github.com/laminlabs/lnhub-rest/pull/208) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.9.7
+➖ Simplify dependencies | [208](https://github.com/laminlabs/lnhub-rest/pull/208) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.9.8
 ➖ Replace boto3 with botocore | [206](https://github.com/laminlabs/lnhub-rest/pull/206) | [Koncopd](https://github.com/Koncopd) | 2023-05-26 |
 🍱 Update assets | [207](https://github.com/laminlabs/lnhub-rest/pull/207) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 |
 ➖ Streamline dependencies | [205](https://github.com/laminlabs/lnhub-rest/pull/205) | [bpenteado](https://github.com/bpenteado) | 2023-05-10 | 0.9.6
 🔖 Staging version 0.9.5 | [199](https://github.com/laminlabs/lnhub-rest/pull/199) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 | 0.9.5
 👷 Fix deployment in main branch | [201](https://github.com/laminlabs/lnhub-rest/pull/201) | [lawrlee](https://github.com/lawrlee) | 2023-05-09 |
 ✨ Create endpoints to update and delete collaborators | [197](https://github.com/laminlabs/lnhub-rest/pull/197) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 |
 🍱 Register trexbio schema | [195](https://github.com/laminlabs/lnhub-rest/pull/195) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.9.4
```

### Comparing `lnhub_rest-0.9.7/docs/migrations.md` & `lnhub_rest-0.9.8/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.9.8/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/.github/workflows/build.yml` & `lnhub_rest-0.9.8/lndb/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.8/lndb/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/.gitignore` & `lnhub_rest-0.9.8/lndb/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/.pre-commit-config.yaml` & `lnhub_rest-0.9.8/lndb/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/LICENSE` & `lnhub_rest-0.9.8/lndb/LICENSE`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/changelog.md` & `lnhub_rest-0.9.8/lndb/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/faq/check-synchronization.ipynb` & `lnhub_rest-0.9.8/lndb/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/faq/clone.ipynb` & `lnhub_rest-0.9.8/lndb/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/faq/edge-cases-login-init.ipynb` & `lnhub_rest-0.9.8/lndb/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/faq/manage-migrations.ipynb` & `lnhub_rest-0.9.8/lndb/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/faq/switch-environment.ipynb` & `lnhub_rest-0.9.8/lndb/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-e2e.ipynb` & `lnhub_rest-0.9.8/lndb/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-unit.ipynb` & `lnhub_rest-0.9.8/lndb/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/01-setup-user.ipynb` & `lnhub_rest-0.9.8/lndb/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/02-init-instance.ipynb` & `lnhub_rest-0.9.8/lndb/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/03-load-instance.ipynb` & `lnhub_rest-0.9.8/lndb/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/04-set-storage.ipynb` & `lnhub_rest-0.9.8/lndb/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/05-schema-modules.ipynb` & `lnhub_rest-0.9.8/lndb/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/06-info.ipynb` & `lnhub_rest-0.9.8/lndb/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/07-delete.ipynb` & `lnhub_rest-0.9.8/lndb/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/docs/guide/migrate.md` & `lnhub_rest-0.9.8/lndb/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/__init__.py` & `lnhub_rest-0.9.8/lndb/lndb/__init__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/__main__.py` & `lnhub_rest-0.9.8/lndb/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_check_instance_setup.py` & `lnhub_rest-0.9.8/lndb/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_close.py` & `lnhub_rest-0.9.8/lndb/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_delete.py` & `lnhub_rest-0.9.8/lndb/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_init_instance.py` & `lnhub_rest-0.9.8/lndb/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_load_instance.py` & `lnhub_rest-0.9.8/lndb/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_migrate/alembic.ini` & `lnhub_rest-0.9.8/lndb/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_migrate/core.py` & `lnhub_rest-0.9.8/lndb/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_migrate/deploy.py` & `lnhub_rest-0.9.8/lndb/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_migrate/env.py` & `lnhub_rest-0.9.8/lndb/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_migrate/utils.py` & `lnhub_rest-0.9.8/lndb/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_register_instance.py` & `lnhub_rest-0.9.8/lndb/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_schema.py` & `lnhub_rest-0.9.8/lndb/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_set.py` & `lnhub_rest-0.9.8/lndb/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_settings.py` & `lnhub_rest-0.9.8/lndb/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/_setup_user.py` & `lnhub_rest-0.9.8/lndb/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/__init__.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_clone.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_db.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_deprecated.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_exclusion.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_instance.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_load.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_save.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_store.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_user.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_setup_knowledge.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_setup_schema.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/_storage.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/dev/upath.py` & `lnhub_rest-0.9.8/lndb/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/test/_migrations_e2e.py` & `lnhub_rest-0.9.8/lndb/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/lndb/test/_migrations_unit.py` & `lnhub_rest-0.9.8/lndb/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/noxfile.py` & `lnhub_rest-0.9.8/lndb/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/pyproject.toml` & `lnhub_rest-0.9.8/lndb/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/tests/test_bionty.py` & `lnhub_rest-0.9.8/lndb/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lndb/tests/test_init_instance.py` & `lnhub_rest-0.9.8/lndb/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/__main__.py` & `lnhub_rest-0.9.8/lnhub_rest/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/_assets/_instances.py` & `lnhub_rest-0.9.8/lnhub_rest/_assets/_instances.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.9.8/lnhub_rest/_assets/_schemas.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.9.8/lnhub_rest/_check_breaks_lndb.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/_ci.py` & `lnhub_rest-0.9.8/lnhub_rest/_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.9.8/lnhub_rest/_clean_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/config.py` & `lnhub_rest-0.9.8/lnhub_rest/config.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.9.8/lnhub_rest/core/account/_create_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.9.8/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.9.8/lnhub_rest/core/account/_delete_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.9.8/lnhub_rest/core/account/_signup_signin.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.9.8/lnhub_rest/core/account/_update_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/collaborator/_crud.py` & `lnhub_rest-0.9.8/lnhub_rest/core/collaborator/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.9.8/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.9.8/lnhub_rest/core/instance/_delete_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.9.8/lnhub_rest/core/instance/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.9.8/lnhub_rest/core/instance/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.9.8/lnhub_rest/core/instance/_update_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/member/_crud.py` & `lnhub_rest-0.9.8/lnhub_rest/core/member/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.9.8/lnhub_rest/core/storage/_add_storage.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.9.8/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/main.py` & `lnhub_rest-0.9.8/lnhub_rest/main.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.9.8/lnhub_rest/orm/_sbclient.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/routers/account.py` & `lnhub_rest-0.9.8/lnhub_rest/routers/account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/routers/ci.py` & `lnhub_rest-0.9.8/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/routers/collaborator.py` & `lnhub_rest-0.9.8/lnhub_rest/routers/collaborator.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/routers/instance.py` & `lnhub_rest-0.9.8/lnhub_rest/routers/instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/routers/organization.py` & `lnhub_rest-0.9.8/lnhub_rest/routers/organization.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/routers/utils.py` & `lnhub_rest-0.9.8/lnhub_rest/routers/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/_core.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/alembic.ini` & `lnhub_rest-0.9.8/lnhub_rest/schema/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/clone.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/testing.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/testing.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py` & `lnhub_rest-0.9.8/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/lnhub_rest/utils/_test.py` & `lnhub_rest-0.9.8/lnhub_rest/utils/_test.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/noxfile.py` & `lnhub_rest-0.9.8/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/pyproject.toml` & `lnhub_rest-0.9.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dynamic = ["version", "description"]
 dependencies = [
     # Do NOT add any lamin package as a dependency here!
     # Neither laminci nor lndb nor lnschema_core etc.
     # lnhub_rest needs to be upstream
     "lamin_logger",
     "supabase==1.0.3",
+    "pyjwt",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnhub-rest"
 
 [project.optional-dependencies]
 server = [
```

### Comparing `lnhub_rest-0.9.7/supabase/config.toml` & `lnhub_rest-0.9.8/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/tests/test_notebooks.py` & `lnhub_rest-0.9.8/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.7/PKG-INFO` & `lnhub_rest-0.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.9.7
+Version: 0.9.8
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamin_logger
 Requires-Dist: supabase==1.0.3
+Requires-Dist: pyjwt
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: fastapi ; extra == "server"
 Requires-Dist: uvicorn ; extra == "server"
 Requires-Dist: sqlmodel ; extra == "server"
 Requires-Dist: alembic ; extra == "server"
 Requires-Dist: pytest_alembic==0.9.1 ; extra == "server"
```

