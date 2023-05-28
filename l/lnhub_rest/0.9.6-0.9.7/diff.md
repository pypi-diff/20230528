# Comparing `tmp/lnhub_rest-0.9.6.tar.gz` & `tmp/lnhub_rest-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.9.6.tar", last modified: Thu May 11 18:46:37 2023, max compression
+gzip compressed data, was "lnhub_rest-0.9.7.tar", last modified: Sun May 28 12:37:23 2023, max compression
```

## Comparing `lnhub_rest-0.9.6.tar` & `lnhub_rest-0.9.7.tar`

### file list

```diff
@@ -1,201 +1,201 @@
--rw-r--r--   0        0        0     1259 2023-02-13 09:20:16.808732 lnhub_rest-0.9.6/.dockerignore
--rw-r--r--   0        0        0     3245 2023-05-09 07:39:52.841154 lnhub_rest-0.9.6/.github/workflows/build.yml
--rw-r--r--   0        0        0     5417 2023-05-09 17:53:52.208995 lnhub_rest-0.9.6/.github/workflows/google-cloudrun-docker-prod.yml
--rw-r--r--   0        0        0     5426 2023-05-09 17:53:52.209379 lnhub_rest-0.9.6/.github/workflows/google-cloudrun-docker-staging.yml
--rw-r--r--   0        0        0      133 2022-12-05 16:31:02.016205 lnhub_rest-0.9.6/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-04-12 05:33:51.441718 lnhub_rest-0.9.6/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1218 2023-05-11 18:46:14.038495 lnhub_rest-0.9.6/.gitignore
--rw-r--r--   0        0        0       73 2023-04-17 19:46:07.717815 lnhub_rest-0.9.6/.gitmodules
--rw-r--r--   0        0        0     1772 2023-04-12 05:33:51.441994 lnhub_rest-0.9.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      157 2023-04-17 19:46:07.718176 lnhub_rest-0.9.6/Dockerfile
--rw-r--r--   0        0        0     2442 2023-05-09 07:39:46.055717 lnhub_rest-0.9.6/README.md
--rw-r--r--   0        0        0     1680 2023-05-09 07:39:46.056027 lnhub_rest-0.9.6/docs/00-migrate.ipynb
--rw-r--r--   0        0        0     1189 2023-04-27 13:36:02.439632 lnhub_rest-0.9.6/docs/01-checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0     4487 2023-04-27 13:36:02.437074 lnhub_rest-0.9.6/docs/02-account/02-create-account.ipynb
--rw-r--r--   0        0        0     5566 2023-04-27 13:36:02.439987 lnhub_rest-0.9.6/docs/02-account/03-update-account.ipynb
--rw-r--r--   0        0        0     6111 2023-04-27 13:36:02.438644 lnhub_rest-0.9.6/docs/02-account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9088 2023-04-27 13:36:02.438818 lnhub_rest-0.9.6/docs/02-account/05-rls.ipynb
--rw-r--r--   0        0        0    11110 2023-05-09 17:53:43.462582 lnhub_rest-0.9.6/docs/03-instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5293 2023-05-09 17:53:43.463166 lnhub_rest-0.9.6/docs/03-instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6498 2023-04-27 13:36:02.438676 lnhub_rest-0.9.6/docs/03-instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     8667 2023-05-09 17:53:43.463571 lnhub_rest-0.9.6/docs/03-instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     7001 2023-04-27 13:36:02.439957 lnhub_rest-0.9.6/docs/03-instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19423 2023-04-27 13:36:02.438412 lnhub_rest-0.9.6/docs/03-instance/06-rls.ipynb
--rw-r--r--   0        0        0     3990 2023-05-09 07:39:52.841652 lnhub_rest-0.9.6/docs/04-storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9837 2023-04-27 13:36:02.440625 lnhub_rest-0.9.6/docs/04-storage/02-rls.ipynb
--rw-r--r--   0        0        0     3894 2023-04-27 13:36:02.435445 lnhub_rest-0.9.6/docs/05-organization/01-create-organization.ipynb
--rw-r--r--   0        0        0     4749 2023-04-27 13:36:02.437528 lnhub_rest-0.9.6/docs/05-organization/02-manage-members.ipynb
--rw-r--r--   0        0        0     5892 2023-04-27 13:36:02.435543 lnhub_rest-0.9.6/docs/05-organization/03-rls.ipynb
--rw-r--r--   0        0        0     5310 2023-05-09 17:53:43.464325 lnhub_rest-0.9.6/docs/06-integration/01-signup-signin.ipynb
--rw-r--r--   0        0        0      125 2023-04-20 08:36:06.559940 lnhub_rest-0.9.6/docs/README.md
--rw-r--r--   0        0        0    24599 2023-05-11 18:46:02.628912 lnhub_rest-0.9.6/docs/changelog.md
--rw-r--r--   0        0        0      520 2023-04-12 05:33:51.446631 lnhub_rest-0.9.6/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-04-12 05:33:51.446714 lnhub_rest-0.9.6/docs/notes/index.md
--rw-r--r--   0        0        0    26418 2023-04-12 05:33:51.447158 lnhub_rest-0.9.6/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0      137 2022-12-05 16:31:02.018378 lnhub_rest-0.9.6/lamin-project.yaml
--rw-r--r--   0        0        0     3832 2023-04-12 15:45:55.670360 lnhub_rest-0.9.6/lndb/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-04-03 19:31:19.500521 lnhub_rest-0.9.6/lndb/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-04-03 19:31:19.500584 lnhub_rest-0.9.6/lndb/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-04-03 19:31:19.500654 lnhub_rest-0.9.6/lndb/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-24 10:07:43.479664 lnhub_rest-0.9.6/lndb/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-04-03 19:31:19.500812 lnhub_rest-0.9.6/lndb/LICENSE
--rw-r--r--   0        0        0      173 2023-04-03 19:31:19.500865 lnhub_rest-0.9.6/lndb/README.md
--rw-r--r--   0        0        0       52 2023-04-03 19:31:19.500947 lnhub_rest-0.9.6/lndb/docs/api.md
--rw-r--r--   0        0        0    48486 2023-05-09 07:19:55.937616 lnhub_rest-0.9.6/lndb/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-04-03 19:31:19.501245 lnhub_rest-0.9.6/lndb/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-04-03 19:31:19.501331 lnhub_rest-0.9.6/lndb/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-04-03 19:31:19.501425 lnhub_rest-0.9.6/lndb/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-04-03 19:31:19.501475 lnhub_rest-0.9.6/lndb/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-24 10:07:43.480335 lnhub_rest-0.9.6/lndb/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-04-03 19:31:19.501612 lnhub_rest-0.9.6/lndb/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-12 15:45:55.670784 lnhub_rest-0.9.6/lndb/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-12 15:45:55.670929 lnhub_rest-0.9.6/lndb/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-03 19:31:19.501804 lnhub_rest-0.9.6/lndb/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    10238 2023-05-09 07:19:55.937971 lnhub_rest-0.9.6/lndb/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     6419 2023-05-09 07:19:55.938294 lnhub_rest-0.9.6/lndb/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6390 2023-04-24 10:07:43.480795 lnhub_rest-0.9.6/lndb/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3746 2023-04-24 11:38:30.442472 lnhub_rest-0.9.6/lndb/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-04-03 19:31:19.502118 lnhub_rest-0.9.6/lndb/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-20 09:03:40.403720 lnhub_rest-0.9.6/lndb/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-04-03 19:31:19.502231 lnhub_rest-0.9.6/lndb/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-24 10:07:43.480911 lnhub_rest-0.9.6/lndb/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-04-03 19:31:19.502354 lnhub_rest-0.9.6/lndb/docs/index.md
--rw-r--r--   0        0        0      118 2023-04-03 19:31:19.502412 lnhub_rest-0.9.6/lndb/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-05-09 07:19:55.938487 lnhub_rest-0.9.6/lndb/lndb/__init__.py
--rw-r--r--   0        0        0     4697 2023-05-09 07:19:55.938696 lnhub_rest-0.9.6/lndb/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-04-03 19:31:19.502658 lnhub_rest-0.9.6/lndb/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-12 15:45:55.671219 lnhub_rest-0.9.6/lndb/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-05-09 07:19:55.938851 lnhub_rest-0.9.6/lndb/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-12 15:45:55.671337 lnhub_rest-0.9.6/lndb/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-12 15:45:55.671440 lnhub_rest-0.9.6/lndb/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-05-09 07:19:55.939671 lnhub_rest-0.9.6/lndb/lndb/_info.py
--rw-r--r--   0        0        0     6035 2023-05-09 07:19:55.940140 lnhub_rest-0.9.6/lndb/lndb/_init_instance.py
--rw-r--r--   0        0        0     6729 2023-05-09 07:19:55.941058 lnhub_rest-0.9.6/lndb/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-12 15:45:55.671792 lnhub_rest-0.9.6/lndb/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-12 15:45:55.671882 lnhub_rest-0.9.6/lndb/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-05-09 07:19:55.941325 lnhub_rest-0.9.6/lndb/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-24 10:07:43.481621 lnhub_rest-0.9.6/lndb/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-04-03 19:31:19.503530 lnhub_rest-0.9.6/lndb/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-05-09 07:19:55.941760 lnhub_rest-0.9.6/lndb/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-12 15:45:55.672114 lnhub_rest-0.9.6/lndb/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      803 2023-05-09 07:19:55.941979 lnhub_rest-0.9.6/lndb/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-04-03 19:31:19.503661 lnhub_rest-0.9.6/lndb/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-24 10:07:43.481783 lnhub_rest-0.9.6/lndb/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-20 09:03:40.405705 lnhub_rest-0.9.6/lndb/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-04-03 19:31:19.503836 lnhub_rest-0.9.6/lndb/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-04-03 19:31:19.503900 lnhub_rest-0.9.6/lndb/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-24 10:07:43.481896 lnhub_rest-0.9.6/lndb/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-12 15:45:55.673128 lnhub_rest-0.9.6/lndb/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-04-03 19:31:19.504115 lnhub_rest-0.9.6/lndb/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-12 15:45:55.673226 lnhub_rest-0.9.6/lndb/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-04-03 19:31:19.504235 lnhub_rest-0.9.6/lndb/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-04-03 19:31:19.504287 lnhub_rest-0.9.6/lndb/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-12 15:45:55.673326 lnhub_rest-0.9.6/lndb/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-05-09 07:19:55.942199 lnhub_rest-0.9.6/lndb/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-04-03 19:31:19.504528 lnhub_rest-0.9.6/lndb/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-04-03 19:31:19.504583 lnhub_rest-0.9.6/lndb/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-12 15:45:55.673539 lnhub_rest-0.9.6/lndb/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-04-03 19:31:19.504686 lnhub_rest-0.9.6/lndb/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-04-03 19:31:19.504753 lnhub_rest-0.9.6/lndb/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-24 10:07:43.482241 lnhub_rest-0.9.6/lndb/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-24 10:07:43.482348 lnhub_rest-0.9.6/lndb/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-04-03 19:31:19.504960 lnhub_rest-0.9.6/lndb/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-12 15:45:55.673699 lnhub_rest-0.9.6/lndb/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-12 15:45:55.673790 lnhub_rest-0.9.6/lndb/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-04-03 19:31:19.505138 lnhub_rest-0.9.6/lndb/lndb/test/_env.py
--rw-r--r--   0        0        0     3911 2023-05-09 07:19:55.942579 lnhub_rest-0.9.6/lndb/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-12 15:45:55.673887 lnhub_rest-0.9.6/lndb/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-04-03 19:31:19.505348 lnhub_rest-0.9.6/lndb/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-04-03 19:31:19.505408 lnhub_rest-0.9.6/lndb/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-12 15:45:55.673980 lnhub_rest-0.9.6/lndb/noxfile.py
--rw-r--r--   0        0        0     1420 2023-05-09 07:19:55.942917 lnhub_rest-0.9.6/lndb/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-12 15:45:55.674169 lnhub_rest-0.9.6/lndb/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-04-03 19:31:19.505727 lnhub_rest-0.9.6/lndb/tests/test_init_instance.py
--rw-r--r--   0        0        0      379 2023-05-09 07:19:55.943086 lnhub_rest-0.9.6/lndb/tests/test_notebooks.py
--rw-r--r--   0        0        0      157 2023-05-11 18:45:52.109918 lnhub_rest-0.9.6/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     7054 2023-05-09 07:39:46.057772 lnhub_rest-0.9.6/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       64 2023-02-13 09:20:16.812158 lnhub_rest-0.9.6/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0     1026 2023-02-13 09:20:16.812240 lnhub_rest-0.9.6/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1109 2023-05-09 17:30:50.125171 lnhub_rest-0.9.6/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1722 2023-04-19 06:39:29.557169 lnhub_rest-0.9.6/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0     1260 2023-05-09 07:39:46.057997 lnhub_rest-0.9.6/lnhub_rest/_ci.py
--rw-r--r--   0        0        0     5726 2023-05-09 17:53:43.464877 lnhub_rest-0.9.6/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0     1620 2023-05-09 07:39:46.058080 lnhub_rest-0.9.6/lnhub_rest/config.py
--rw-r--r--   0        0        0       42 2023-04-12 05:33:51.449892 lnhub_rest-0.9.6/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      285 2023-04-17 19:46:07.724724 lnhub_rest-0.9.6/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     2542 2023-04-23 14:15:16.131687 lnhub_rest-0.9.6/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-04-12 05:33:51.450294 lnhub_rest-0.9.6/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      739 2023-04-20 08:36:06.562096 lnhub_rest-0.9.6/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3325 2023-05-09 17:53:43.465516 lnhub_rest-0.9.6/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1423 2023-04-20 08:36:06.562595 lnhub_rest-0.9.6/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-04-12 05:33:51.451054 lnhub_rest-0.9.6/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     3056 2023-04-24 12:41:04.298412 lnhub_rest-0.9.6/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-04-12 05:33:51.451365 lnhub_rest-0.9.6/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-04-12 05:33:51.451441 lnhub_rest-0.9.6/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1284 2023-04-20 08:36:06.563067 lnhub_rest-0.9.6/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6096 2023-05-09 07:39:52.843001 lnhub_rest-0.9.6/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1532 2023-04-20 08:36:06.563609 lnhub_rest-0.9.6/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1067 2023-04-20 08:36:06.563842 lnhub_rest-0.9.6/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       32 2023-04-17 19:46:07.726669 lnhub_rest-0.9.6/lnhub_rest/core/member/__init__.py
--rw-r--r--   0        0        0     2078 2023-04-17 19:46:07.726929 lnhub_rest-0.9.6/lnhub_rest/core/member/_crud.py
--rw-r--r--   0        0        0       80 2023-04-12 05:33:51.452504 lnhub_rest-0.9.6/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     3230 2023-05-09 07:39:52.843396 lnhub_rest-0.9.6/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-04-12 05:33:51.452880 lnhub_rest-0.9.6/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      849 2023-05-09 17:53:52.209990 lnhub_rest-0.9.6/lnhub_rest/main.py
--rw-r--r--   0        0        0       39 2023-04-20 08:36:06.564287 lnhub_rest-0.9.6/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      199 2023-05-09 07:39:46.058791 lnhub_rest-0.9.6/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     1968 2023-05-09 17:53:43.466525 lnhub_rest-0.9.6/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      239 2023-05-09 17:53:52.210262 lnhub_rest-0.9.6/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     4661 2023-04-24 12:41:04.298691 lnhub_rest-0.9.6/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-05-09 17:53:43.467343 lnhub_rest-0.9.6/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0     2313 2023-05-09 17:53:52.210493 lnhub_rest-0.9.6/lnhub_rest/routers/collaborator.py
--rw-r--r--   0        0        0      408 2023-04-12 05:33:51.454427 lnhub_rest-0.9.6/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     5233 2023-04-24 12:41:04.298930 lnhub_rest-0.9.6/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     2617 2023-04-17 19:46:07.729123 lnhub_rest-0.9.6/lnhub_rest/routers/organization.py
--rw-r--r--   0        0        0     1074 2023-04-20 08:36:06.565374 lnhub_rest-0.9.6/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      249 2023-04-19 06:39:29.557427 lnhub_rest-0.9.6/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     4986 2023-04-17 19:46:07.730209 lnhub_rest-0.9.6/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-03-02 11:17:31.752043 lnhub_rest-0.9.6/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      262 2023-04-17 19:46:07.730671 lnhub_rest-0.9.6/lnhub_rest/schema/_type.py
--rw-r--r--   0        0        0      252 2023-03-02 11:17:31.752112 lnhub_rest-0.9.6/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-04-12 05:33:51.456009 lnhub_rest-0.9.6/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-02-13 09:20:16.814087 lnhub_rest-0.9.6/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       40 2023-05-09 07:39:46.059338 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     6020 2023-04-17 19:46:07.731439 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/clone.py
--rw-r--r--   0        0        0     3033 2023-05-09 07:39:46.059588 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-04-12 05:33:51.456564 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0     1319 2023-04-17 19:46:07.731951 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1667 2023-04-17 19:46:07.732205 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0       39 2023-04-12 05:33:51.457356 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-04-12 05:33:51.457588 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-04-12 05:33:51.457841 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      214 2023-04-17 19:46:07.732575 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0      192 2023-04-17 19:46:07.732918 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
--rw-r--r--   0        0        0     7619 2023-04-17 19:46:07.733294 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
--rw-r--r--   0        0        0     1408 2023-04-17 19:46:07.733539 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
--rw-r--r--   0        0        0      880 2023-04-19 06:39:29.557590 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
--rw-r--r--   0        0        0       33 2023-04-12 05:33:51.459308 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-02-13 09:20:16.814349 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0     5258 2023-05-09 07:39:46.059864 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/testing.py
--rw-r--r--   0        0        0     9882 2023-04-20 08:36:06.566134 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-04-20 08:36:06.566367 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-04-12 05:33:51.460064 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-04-12 05:33:51.460238 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      542 2023-04-17 19:46:07.734101 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0     1199 2023-04-17 19:46:07.734436 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
--rw-r--r--   0        0        0      733 2023-04-17 19:46:07.734632 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
--rw-r--r--   0        0        0     5143 2023-04-17 19:46:07.734875 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
--rw-r--r--   0        0        0      593 2023-04-19 06:39:29.557744 lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
--rw-r--r--   0        0        0       60 2023-03-02 11:17:31.752459 lnhub_rest-0.9.6/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0       13 2023-04-17 19:46:07.735238 lnhub_rest-0.9.6/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-04-12 05:33:51.461642 lnhub_rest-0.9.6/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      352 2023-04-17 19:46:07.735507 lnhub_rest-0.9.6/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-04-12 05:33:51.461902 lnhub_rest-0.9.6/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3820 2023-04-20 08:36:06.566596 lnhub_rest-0.9.6/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1714 2023-05-09 07:39:46.060173 lnhub_rest-0.9.6/noxfile.py
--rw-r--r--   0        0        0     1248 2023-05-11 18:30:01.899844 lnhub_rest-0.9.6/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-04-12 05:33:51.462685 lnhub_rest-0.9.6/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-04-12 05:33:51.462759 lnhub_rest-0.9.6/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-04-12 05:33:51.462840 lnhub_rest-0.9.6/supabase/config.toml
--rw-r--r--   0        0        0     1212 2023-05-09 07:39:46.060630 lnhub_rest-0.9.6/tests/test_notebooks.py
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 lnhub_rest-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.9.7/.dockerignore
+-rw-r--r--   0        0        0     3245 2023-05-25 20:34:20.149969 lnhub_rest-0.9.7/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5417 2023-05-25 20:34:20.150136 lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-prod.yml
+-rw-r--r--   0        0        0     5426 2023-05-25 20:34:20.150292 lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-staging.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.9.7/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.9.7/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.9.7/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.9.7/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.9.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.9.7/Dockerfile
+-rw-r--r--   0        0        0     2442 2023-04-25 15:29:32.847024 lnhub_rest-0.9.7/README.md
+-rw-r--r--   0        0        0     1680 2023-04-27 03:39:31.402324 lnhub_rest-0.9.7/docs/00-migrate.ipynb
+-rw-r--r--   0        0        0     1189 2023-04-27 03:39:31.402860 lnhub_rest-0.9.7/docs/01-checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0     4487 2023-04-27 03:39:31.414955 lnhub_rest-0.9.7/docs/02-account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5566 2023-04-27 03:39:31.419067 lnhub_rest-0.9.7/docs/02-account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6111 2023-04-27 03:39:31.418992 lnhub_rest-0.9.7/docs/02-account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9088 2023-04-27 03:39:31.419398 lnhub_rest-0.9.7/docs/02-account/05-rls.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-27 04:21:53.504972 lnhub_rest-0.9.7/docs/03-instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5293 2023-04-27 03:39:31.415575 lnhub_rest-0.9.7/docs/03-instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6498 2023-04-27 03:39:31.417147 lnhub_rest-0.9.7/docs/03-instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8667 2023-04-27 03:39:31.417306 lnhub_rest-0.9.7/docs/03-instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     7001 2023-04-27 03:39:31.420904 lnhub_rest-0.9.7/docs/03-instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19423 2023-04-27 03:39:31.401299 lnhub_rest-0.9.7/docs/03-instance/06-rls.ipynb
+-rw-r--r--   0        0        0     3990 2023-04-27 04:21:53.505189 lnhub_rest-0.9.7/docs/04-storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9837 2023-04-27 03:39:31.421340 lnhub_rest-0.9.7/docs/04-storage/02-rls.ipynb
+-rw-r--r--   0        0        0     3894 2023-04-27 03:39:31.415314 lnhub_rest-0.9.7/docs/05-organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     4749 2023-04-27 03:39:31.413247 lnhub_rest-0.9.7/docs/05-organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5892 2023-04-27 03:39:31.413014 lnhub_rest-0.9.7/docs/05-organization/03-rls.ipynb
+-rw-r--r--   0        0        0     5310 2023-04-27 03:39:31.417221 lnhub_rest-0.9.7/docs/06-integration/01-signup-signin.ipynb
+-rw-r--r--   0        0        0      125 2023-04-18 16:52:57.348114 lnhub_rest-0.9.7/docs/README.md
+-rw-r--r--   0        0        0    25029 2023-05-28 12:37:03.229477 lnhub_rest-0.9.7/docs/changelog.md
+-rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.9.7/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.9.7/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.9.7/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.9.7/lamin-project.yaml
+-rw-r--r--   0        0        0     3832 2023-04-18 16:53:14.549682 lnhub_rest-0.9.7/lndb/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.9.7/lndb/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.9.7/lndb/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.9.7/lndb/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-25 15:29:40.845175 lnhub_rest-0.9.7/lndb/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.9.7/lndb/LICENSE
+-rw-r--r--   0        0        0      173 2023-04-18 16:53:14.549987 lnhub_rest-0.9.7/lndb/README.md
+-rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.9.7/lndb/docs/api.md
+-rw-r--r--   0        0        0    47755 2023-04-27 03:47:05.803728 lnhub_rest-0.9.7/lndb/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.9.7/lndb/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.9.7/lndb/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-04-18 16:53:14.550717 lnhub_rest-0.9.7/lndb/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-04-18 16:53:14.551192 lnhub_rest-0.9.7/lndb/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-25 15:29:40.845949 lnhub_rest-0.9.7/lndb/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.9.7/lndb/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-18 16:53:14.551375 lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-18 16:53:14.551472 lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-18 16:53:14.551612 lnhub_rest-0.9.7/lndb/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10370 2023-04-27 04:20:38.053396 lnhub_rest-0.9.7/lndb/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-25 15:29:40.846776 lnhub_rest-0.9.7/lndb/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-25 15:29:40.846861 lnhub_rest-0.9.7/lndb/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-25 15:29:40.846961 lnhub_rest-0.9.7/lndb/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-04-18 16:53:14.552137 lnhub_rest-0.9.7/lndb/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-25 15:29:40.847226 lnhub_rest-0.9.7/lndb/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.9.7/lndb/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-25 15:29:40.847416 lnhub_rest-0.9.7/lndb/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.9.7/lndb/docs/index.md
+-rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.9.7/lndb/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-27 03:47:05.803990 lnhub_rest-0.9.7/lndb/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-25 15:29:40.847751 lnhub_rest-0.9.7/lndb/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.9.7/lndb/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-18 16:53:14.553281 lnhub_rest-0.9.7/lndb/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-25 15:29:40.847842 lnhub_rest-0.9.7/lndb/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-18 16:53:14.553610 lnhub_rest-0.9.7/lndb/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-18 16:53:14.553765 lnhub_rest-0.9.7/lndb/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-25 15:29:40.848070 lnhub_rest-0.9.7/lndb/lndb/_info.py
+-rw-r--r--   0        0        0     6035 2023-04-27 03:52:24.150379 lnhub_rest-0.9.7/lndb/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6485 2023-04-27 03:49:23.883095 lnhub_rest-0.9.7/lndb/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-18 16:53:14.554421 lnhub_rest-0.9.7/lndb/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-18 16:53:14.554545 lnhub_rest-0.9.7/lndb/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-25 15:29:40.848442 lnhub_rest-0.9.7/lndb/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-25 15:29:40.848595 lnhub_rest-0.9.7/lndb/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.9.7/lndb/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-25 15:29:40.848722 lnhub_rest-0.9.7/lndb/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-18 16:53:14.554944 lnhub_rest-0.9.7/lndb/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      803 2023-04-27 04:20:38.053795 lnhub_rest-0.9.7/lndb/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.9.7/lndb/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-25 15:29:40.849016 lnhub_rest-0.9.7/lndb/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 21:34:53.593994 lnhub_rest-0.9.7/lndb/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.9.7/lndb/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.9.7/lndb/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-25 15:29:40.849262 lnhub_rest-0.9.7/lndb/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-18 16:53:14.555545 lnhub_rest-0.9.7/lndb/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-04-18 16:53:14.555802 lnhub_rest-0.9.7/lndb/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-18 16:53:14.555956 lnhub_rest-0.9.7/lndb/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.9.7/lndb/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.9.7/lndb/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-18 16:53:14.556103 lnhub_rest-0.9.7/lndb/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-04-27 03:49:23.883399 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-04-18 16:53:14.556382 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-18 16:53:14.556505 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.9.7/lndb/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-04-18 16:53:14.556633 lnhub_rest-0.9.7/lndb/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-25 15:29:40.849676 lnhub_rest-0.9.7/lndb/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-25 15:29:40.849829 lnhub_rest-0.9.7/lndb/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.9.7/lndb/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-18 16:53:14.557004 lnhub_rest-0.9.7/lndb/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-18 16:53:14.557144 lnhub_rest-0.9.7/lndb/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.9.7/lndb/lndb/test/_env.py
+-rw-r--r--   0        0        0     3911 2023-04-27 03:52:24.153553 lnhub_rest-0.9.7/lndb/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-18 16:53:14.557417 lnhub_rest-0.9.7/lndb/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.9.7/lndb/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.9.7/lndb/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-18 16:53:14.557535 lnhub_rest-0.9.7/lndb/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-27 04:20:38.053974 lnhub_rest-0.9.7/lndb/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-18 16:53:14.557862 lnhub_rest-0.9.7/lndb/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.9.7/lndb/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-18 16:53:14.558657 lnhub_rest-0.9.7/lndb/tests/test_notebooks.py
+-rw-r--r--   0        0        0      157 2023-05-28 12:36:54.490184 lnhub_rest-0.9.7/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     7054 2023-04-25 15:29:32.854635 lnhub_rest-0.9.7/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.9.7/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0      706 2023-05-28 12:36:10.508939 lnhub_rest-0.9.7/lnhub_rest/_assets/_instances.py
+-rw-r--r--   0        0        0     1109 2023-05-25 20:34:20.151651 lnhub_rest-0.9.7/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.9.7/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0     1260 2023-04-25 15:29:32.854787 lnhub_rest-0.9.7/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5726 2023-04-19 15:57:22.490723 lnhub_rest-0.9.7/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0     1626 2023-05-28 12:14:52.784375 lnhub_rest-0.9.7/lnhub_rest/config.py
+-rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.9.7/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.9.7/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2542 2023-04-21 10:12:34.724799 lnhub_rest-0.9.7/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.9.7/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      739 2023-04-19 15:57:22.491329 lnhub_rest-0.9.7/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3325 2023-04-19 15:57:22.491711 lnhub_rest-0.9.7/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1423 2023-04-19 15:57:22.491949 lnhub_rest-0.9.7/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.9.7/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     3056 2023-04-25 15:29:32.855696 lnhub_rest-0.9.7/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.9.7/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.9.7/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1284 2023-04-19 15:57:22.492340 lnhub_rest-0.9.7/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6096 2023-04-27 04:21:53.505412 lnhub_rest-0.9.7/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1532 2023-04-19 15:57:22.492860 lnhub_rest-0.9.7/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1067 2023-04-19 15:57:22.493104 lnhub_rest-0.9.7/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.9.7/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.9.7/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.9.7/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     3427 2023-05-28 12:14:52.784992 lnhub_rest-0.9.7/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.9.7/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      849 2023-05-25 20:34:20.151769 lnhub_rest-0.9.7/lnhub_rest/main.py
+-rw-r--r--   0        0        0       39 2023-04-19 15:57:22.493742 lnhub_rest-0.9.7/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      199 2023-04-25 15:29:32.856194 lnhub_rest-0.9.7/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     1968 2023-04-25 15:29:32.856453 lnhub_rest-0.9.7/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      239 2023-05-25 20:34:20.152255 lnhub_rest-0.9.7/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4661 2023-04-25 15:29:32.856734 lnhub_rest-0.9.7/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.9.7/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0     2313 2023-05-25 20:34:20.152366 lnhub_rest-0.9.7/lnhub_rest/routers/collaborator.py
+-rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.9.7/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     5233 2023-04-25 15:29:32.856998 lnhub_rest-0.9.7/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.9.7/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1074 2023-04-19 15:57:22.494317 lnhub_rest-0.9.7/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.9.7/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.9.7/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.9.7/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.9.7/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.9.7/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.9.7/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.9.7/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       40 2023-04-25 15:29:32.857365 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     3033 2023-04-25 15:29:32.857603 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0     5258 2023-04-25 15:29:32.857771 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     9882 2023-04-18 16:52:57.349405 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-04-18 16:52:57.349781 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.9.7/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.9.7/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.9.7/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.9.7/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.9.7/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3820 2023-04-19 15:57:22.494545 lnhub_rest-0.9.7/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1728 2023-05-28 12:36:10.509265 lnhub_rest-0.9.7/noxfile.py
+-rw-r--r--   0        0        0     1139 2023-05-28 12:36:10.509601 lnhub_rest-0.9.7/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.9.7/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.9.7/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.9.7/supabase/config.toml
+-rw-r--r--   0        0        0     1212 2023-04-25 15:29:32.858221 lnhub_rest-0.9.7/tests/test_notebooks.py
+-rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 lnhub_rest-0.9.7/PKG-INFO
```

### Comparing `lnhub_rest-0.9.6/.dockerignore` & `lnhub_rest-0.9.7/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/.github/workflows/build.yml` & `lnhub_rest-0.9.7/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/.github/workflows/google-cloudrun-docker-prod.yml` & `lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-prod.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/.github/workflows/google-cloudrun-docker-staging.yml` & `lnhub_rest-0.9.7/.github/workflows/google-cloudrun-docker-staging.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.7/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/.gitignore` & `lnhub_rest-0.9.7/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 celerybeat-schedule
 
 # SageMath parsed files
 *.sage.py
 
 # dotenv
 .env
-*.env
 
 # virtualenv
 .venv
 venv/
 ENV/
 
 # mypy
```

### Comparing `lnhub_rest-0.9.6/.pre-commit-config.yaml` & `lnhub_rest-0.9.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/README.md` & `lnhub_rest-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/00-migrate.ipynb` & `lnhub_rest-0.9.7/docs/00-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/01-checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.9.7/docs/01-checks/01-check-break-lndb.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/02-account/02-create-account.ipynb` & `lnhub_rest-0.9.7/docs/02-account/02-create-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/02-account/03-update-account.ipynb` & `lnhub_rest-0.9.7/docs/02-account/03-update-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/02-account/04-fetch-account.ipynb` & `lnhub_rest-0.9.7/docs/02-account/04-fetch-account.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/02-account/05-rls.ipynb` & `lnhub_rest-0.9.7/docs/02-account/05-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/03-instance/01-init-instance.ipynb` & `lnhub_rest-0.9.7/docs/03-instance/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/03-instance/02-load-instance.ipynb` & `lnhub_rest-0.9.7/docs/03-instance/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/03-instance/03-update-instance.ipynb` & `lnhub_rest-0.9.7/docs/03-instance/03-update-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/03-instance/04-delete-instance.ipynb` & `lnhub_rest-0.9.7/docs/03-instance/04-delete-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/03-instance/05-fetch-instance.ipynb` & `lnhub_rest-0.9.7/docs/03-instance/05-fetch-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/03-instance/06-rls.ipynb` & `lnhub_rest-0.9.7/docs/03-instance/06-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/04-storage/01-add-storage.ipynb` & `lnhub_rest-0.9.7/docs/04-storage/01-add-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/04-storage/02-rls.ipynb` & `lnhub_rest-0.9.7/docs/04-storage/02-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/05-organization/01-create-organization.ipynb` & `lnhub_rest-0.9.7/docs/05-organization/01-create-organization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/05-organization/02-manage-members.ipynb` & `lnhub_rest-0.9.7/docs/05-organization/02-manage-members.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/05-organization/03-rls.ipynb` & `lnhub_rest-0.9.7/docs/05-organization/03-rls.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/06-integration/01-signup-signin.ipynb` & `lnhub_rest-0.9.7/docs/06-integration/01-signup-signin.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/changelog.md` & `lnhub_rest-0.9.7/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+➖ Simplify dependencies | [208](https://github.com/laminlabs/lnhub-rest/pull/208) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.9.7
+➖ Replace boto3 with botocore | [206](https://github.com/laminlabs/lnhub-rest/pull/206) | [Koncopd](https://github.com/Koncopd) | 2023-05-26 |
+🍱 Update assets | [207](https://github.com/laminlabs/lnhub-rest/pull/207) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 |
 ➖ Streamline dependencies | [205](https://github.com/laminlabs/lnhub-rest/pull/205) | [bpenteado](https://github.com/bpenteado) | 2023-05-10 | 0.9.6
 🔖 Staging version 0.9.5 | [199](https://github.com/laminlabs/lnhub-rest/pull/199) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 | 0.9.5
 👷 Fix deployment in main branch | [201](https://github.com/laminlabs/lnhub-rest/pull/201) | [lawrlee](https://github.com/lawrlee) | 2023-05-09 |
 ✨ Create endpoints to update and delete collaborators | [197](https://github.com/laminlabs/lnhub-rest/pull/197) | [bpenteado](https://github.com/bpenteado) | 2023-05-09 |
 🍱 Register trexbio schema | [195](https://github.com/laminlabs/lnhub-rest/pull/195) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.9.4
 Remove build workflow when making a release | [193](https://github.com/laminlabs/lnhub-rest/pull/193) | [lawrlee](https://github.com/lawrlee) | 2023-04-27 |
 ✨ Allow local storage locations | [194](https://github.com/laminlabs/lnhub-rest/pull/194) | [falexwolf](https://github.com/falexwolf) | 2023-04-27 | 0.9.3
```

### Comparing `lnhub_rest-0.9.6/docs/migrations.md` & `lnhub_rest-0.9.7/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.9.7/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/.github/workflows/build.yml` & `lnhub_rest-0.9.7/lndb/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/.github/workflows/latest-changes.yml` & `lnhub_rest-0.9.7/lndb/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/.gitignore` & `lnhub_rest-0.9.7/lndb/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/.pre-commit-config.yaml` & `lnhub_rest-0.9.7/lndb/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/LICENSE` & `lnhub_rest-0.9.7/lndb/LICENSE`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/changelog.md` & `lnhub_rest-0.9.7/lndb/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
-🔊 Use lamin_logger in test_notebooks.py | [376](https://github.com/laminlabs/lndb/pull/376) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
-Add universal_pathlib to dependencies | [375](https://github.com/laminlabs/lndb/pull/375) | [Zethson](https://github.com/Zethson) | 2023-05-02 |
-⬆️ Upgrade lnhub-rest to 0.9.4 | [373](https://github.com/laminlabs/lndb/pull/373) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.44.7
-🚑 Fix load | [372](https://github.com/laminlabs/lndb/pull/372) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-27 | 0.44.6
-✨ Add `--storage` arg to `lamin load` | [370](https://github.com/laminlabs/lndb/pull/370) | [falexwolf](https://github.com/falexwolf) | 2023-04-27 |
 ⬆️ Upgrade lnhub-rest | [369](https://github.com/laminlabs/lndb/pull/369) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.44.5
 ✨ Allow to set additional fsspec kwargs for cloud instances | [366](https://github.com/laminlabs/lndb/pull/366) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 | 0.44.4
 ⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
 🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
 🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
```

### Comparing `lnhub_rest-0.9.6/lndb/docs/faq/check-synchronization.ipynb` & `lnhub_rest-0.9.7/lndb/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/faq/clone.ipynb` & `lnhub_rest-0.9.7/lndb/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/faq/edge-cases-login-init.ipynb` & `lnhub_rest-0.9.7/lndb/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/faq/manage-migrations.ipynb` & `lnhub_rest-0.9.7/lndb/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/faq/switch-environment.ipynb` & `lnhub_rest-0.9.7/lndb/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/faq/test-migrations-e2e.ipynb` & `lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/faq/test-migrations-unit.ipynb` & `lnhub_rest-0.9.7/lndb/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/01-setup-user.ipynb` & `lnhub_rest-0.9.7/lndb/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/02-init-instance.ipynb` & `lnhub_rest-0.9.7/lndb/docs/guide/02-init-instance.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897767857142857%*

 * *Differences: {"'cells'": "{2: {'attachments': OrderedDict()}, 4: {'attachments': OrderedDict()}, 7: "*

 * *            "{'attachments': OrderedDict()}, 9: {'source': {insert: [(4, 'assert "*

 * *            "ln.setup.settings.storage.cache_dir is None')], delete: [8, 7, 6, 5, 4]}}, 10: "*

 * *            "{'source': ['If you want to register it on the hub at lamin.ai, call:'], "*

 * *            "'attachments': OrderedDict()}, 14: {'attachments': OrderedDict()}, 19: "*

 * *            "{'attachments': OrderedDict()}, 21: {'attachments': Ordered […]*

```diff
@@ -17,14 +17,15 @@
             "source": [
                 "import lamindb as ln\n",
                 "from laminci.db import setup_local_test_postgres\n",
                 "from pathlib import Path"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We already set up a user account for \"testuser1@lamin.ai\" and chose handle `testuser1`."
             ]
         },
         {
@@ -33,14 +34,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.login(\"testuser1\")  # CLI: lamin login testuser1"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Local database & storage"
             ]
         },
         {
@@ -56,14 +58,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "ln.setup.init(storage=\"./mydata\")  # CLI: lamin init --storage ./mydata"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This automatically assigns an instance name that equals the name of the storage root along with a few other settings:"
             ]
         },
         {
@@ -85,29 +88,32 @@
             },
             "outputs": [],
             "source": [
                 "assert ln.setup.settings.instance.storage.is_cloud == False\n",
                 "assert ln.setup.settings.instance.owner == ln.setup.settings.user.handle\n",
                 "assert ln.setup.settings.instance.name == \"mydata\"\n",
                 "assert ln.setup.settings.storage.root.as_posix() == Path(\"mydata\").resolve().as_posix()\n",
-                "assert ln.setup.settings.storage.cache_dir is None\n",
-                "assert (\n",
-                "    ln.setup.settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/mydata.lndb\"\n",
-                ")"
+                "assert ln.setup.settings.storage.cache_dir is None"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If you want to register it on the hub at lamin.ai, call:\n",
-                "```\n",
-                "ln.setup.register()\n",
-                "```"
+                "If you want to register it on the hub at lamin.ai, call:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ln.setup.register()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Postgres"
@@ -123,14 +129,15 @@
             },
             "outputs": [],
             "source": [
                 "pgurl = setup_local_test_postgres()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "A connection string for postgres looks like this:"
             ]
         },
         {
@@ -180,14 +187,15 @@
                 "assert ln.setup.settings.instance.storage.cache_dir is None\n",
                 "\n",
                 "!lamin delete pgtest\n",
                 "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Custom instance name"
             ]
         },
         {
@@ -200,14 +208,15 @@
             },
             "outputs": [],
             "source": [
                 "pgurl = setup_local_test_postgres()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Instead of having the instance name be auto-determined from `storage` or `db`, you can provide a custom name:"
             ]
         },
         {
@@ -257,14 +266,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### AWS"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You need to have access to AWS S3 via `awscli configure`."
             ]
         },
         {
@@ -390,14 +400,15 @@
                 "# this should move up in this guide\n",
                 "pgurl = setup_local_test_postgres(name=\"pgtest-registered\")\n",
                 "ln.setup.init(storage=\"s3://lndb-setup-ci\", db=pgurl)\n",
                 "ln.setup.register()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Re-initialize an existing instance"
             ]
         },
         {
```

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/03-load-instance.ipynb` & `lnhub_rest-0.9.7/lndb/docs/guide/04-set-storage.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9354930294486216%*

 * *Differences: {"'cells'": "{0: {'source': ['# Set storage']}, 1: {'id': '33c2bb76-d61f-4866-87e2-780e61600022', "*

 * *            "'source': ['import lamindb as ln\\n', 'from pathlib import Path\\n', 'import "*

 * *            "laminci']}, 4: {'id': 'd6b0bd5e', 'source': "*

 * *            '[\'ln.setup.init(storage="./storage_1", db=pgurl)\']}, 5: {\'id\': \'ceb57cc9\', '*

 * *            "'source': ['Running \\n', '```\\n', '!lamin set --storage ./storage_2\\n', '```\\n', "*

 * *            "'on the command line runs the following Python funct […]*

```diff
@@ -3,261 +3,296 @@
         {
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Load & close an instance"
+                "# Set storage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5fd65a65-5c34-462e-a980-a5aed1a2713f",
+            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
-                "!lamin close"
+                "import lamindb as ln\n",
+                "from pathlib import Path\n",
+                "import laminci"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "a7cf42fb",
+            "metadata": {},
+            "source": [
+                "## Set storage for PostgreSQL instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "33c2bb76-d61f-4866-87e2-780e61600022",
-            "metadata": {},
+            "id": "8fd59ad3-04b9-42fb-83cc-ab7beedbec72",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "from pathlib import Path\n",
-                "import pytest\n",
-                "import lamindb as ln\n",
-                "from lamindb.setup import settings\n",
-                "from lndb.dev._settings_store import instance_settings_file"
+                "pgurl = laminci.db.setup_local_test_postgres()"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "1be836bb",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d6b0bd5e",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Load your own instance by name"
+                "ln.setup.init(storage=\"./storage_1\", db=pgurl)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a5c94e19",
+            "id": "ceb57cc9",
             "metadata": {},
             "source": [
-                "If the user is the instance owner, just load the instance by name:"
+                "Running \n",
+                "```\n",
+                "!lamin set --storage ./storage_2\n",
+                "```\n",
+                "on the command line runs the following Python function:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e7ecc665",
+            "id": "49b9ef11",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.load(\"mydata\")  # CLI: lamin load mydata"
+                "ln.setup.set.storage(\"./storage_2\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "2276e0be",
+            "id": "8e481aa0",
             "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
+                "tags": []
             },
             "outputs": [],
             "source": [
-                "assert settings.instance.storage.is_cloud == False\n",
-                "assert settings.instance.name == \"mydata\"\n",
-                "assert (\n",
-                "    settings.instance.storage.root.as_posix() == Path(\"./mydata\").resolve().as_posix()\n",
-                ")\n",
-                "assert settings.instance.storage.cache_dir is None\n",
-                "assert (\n",
-                "    settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata').resolve().as_posix()}/mydata.lndb\"\n",
-                ")"
+                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "25a13298",
+            "metadata": {},
+            "source": [
+                "Running \n",
+                "```\n",
+                "lamin set --storage s3://lndb-setup-ci\n",
+                "```\n",
+                "\n",
+                "on the command line runs the following:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "ac0d2b30",
+            "id": "8436575d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# assume we move the storage location\n",
-                "!mv mydata mydata_new_loc\n",
-                "with pytest.raises(\n",
-                "    RuntimeError\n",
-                "):  # triggers because it does not find the SQLite file anymore\n",
-                "    ln.setup.load(\"mydata\")\n",
-                "# now account for the new storage location\n",
-                "ln.setup.load(\"mydata\", storage=\"./mydata_new_loc\")\n",
-                "assert (\n",
-                "    settings.instance.storage.root.as_posix()\n",
-                "    == Path(\"./mydata_new_loc\").resolve().as_posix()\n",
-                ")\n",
-                "assert settings.instance.storage.cache_dir is None\n",
-                "assert (\n",
-                "    settings.instance.db\n",
-                "    == f\"sqlite:///{Path('./mydata_new_loc').resolve().as_posix()}/mydata.lndb\"\n",
-                ")"
+                "ln.setup.set.storage(\"s3://lndb-setup-ci\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4f179b5b",
+            "id": "d2934990",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "# another test case, this time with a manually configured instance name\n",
-                "ln.setup.load(\"pgtest-registered\")\n",
-                "assert settings.instance.storage.is_cloud == True\n",
-                "assert settings.instance.name == \"pgtest-registered\"\n",
-                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\""
+                "assert ln.setup.settings.storage.is_cloud\n",
+                "assert ln.setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\""
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "7bd9997b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# root.fs contains the underlying fsspec filesystem\n",
+                "assert (\n",
+                "    ln.setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3f47a1d4",
+            "id": "ae953b6a",
             "metadata": {},
             "source": [
-                "This also works for remote instances:"
+                "It is possible to set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "7c9698f9",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "f9294082",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "# ensure that the locally cached env file is deleted\n",
-                "instance_settings_file(\"lndb-setup-ci\", \"testuser1\").unlink()"
+                "ln.setup.set.storage(\"s3://lndb-setup-ci\", cache_regions=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "089a3832",
+            "id": "5f320819",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.load(\"lndb-setup-ci\")  # lamin load lndb-setup-ci"
+                "assert not ln.setup.settings.storage.root.fs.cache_regions"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "529e68e5-9b10-4fdb-9d4c-ac8206bbbb68",
+            "metadata": {},
+            "source": [
+                "### Set storage not by owner"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "1ebd784f",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "d6915638-db49-4d3d-bd91-819bb4719ef7",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "assert settings.instance.storage.is_cloud == True\n",
-                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
-                "assert (\n",
-                "    settings.instance._sqlite_file.as_posix() == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
+                "ln.setup.login(\n",
+                "    \"testuser2@lamin.ai\", password=\"goeoNJKE61ygbz1vhaCVynGERaRrlviPBVQsjkhz\"\n",
                 ")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "914af9a6",
-            "metadata": {},
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2ed8716f-852f-4ce9-8eef-5b824d6e92b3",
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
             "source": [
-                "## Load instance from another owner"
+                "ln.setup.set.storage(\"./storage_3\")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "65ab467e",
-            "metadata": {},
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "cad87623",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
+            "outputs": [],
             "source": [
-                "If you have the permission, you can load an instance from another owner. "
+                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8436575d",
-            "metadata": {},
+            "id": "78a819fa-48d6-4c6f-95d4-7dc7e94283bb",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ln.setup.load(\"testuser1/mydata\")  # lamin load \"testuser1/mydata\""
+                "!docker stop pgtest && docker rm pgtest"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "0986a5f3",
+            "id": "3fb6a223",
+            "metadata": {
+                "tags": []
+            },
+            "source": [
+                "## Set storage for SQLite instance"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "6ccb6573",
             "metadata": {},
             "source": [
-                "Load an instance from wrong owner."
+                "If the user tries to set the storage for an sqlite instance, an error message is raised:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "bc3568ae",
+            "id": "49309f3a-199f-40bc-b318-a396ebcaafec",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln.setup.load(\"testuser2/mydata\") == \"instance-not-reachable\""
+                "ln.setup.login(\"testuser1\")"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "e3701120",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f988a386",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Close an instance"
+                "ln.setup.load(\"mydata\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8e54d8cd",
-            "metadata": {},
+            "id": "e4f2545f",
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "ln.setup.close()"
+                "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "12db83b9-9d14-4575-876a-3d640a1c1e10",
+            "id": "4fa82d8b",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "# clean up\n",
-                "!lamin delete pgtest-registered\n",
-                "!docker stop pgtest-registered && docker rm pgtest-registered"
+                "ln.setup.set_storage(\"mydata_storage_2\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -269,18 +304,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.12"
         },
         "vscode": {
             "interpreter": {
-                "hash": "5c7b89af1651d0b8571dde13640ecdccf7d5a6204171d6ab33e7c296e100e08a"
+                "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/04-set-storage.ipynb` & `lnhub_rest-0.9.7/lndb/docs/guide/03-load-instance.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.938414558531746%*

 * *Differences: {"'cells'": "{0: {'source': ['# Load & close an instance']}, 1: {'source': {insert: [(1, 'import "*

 * *            "os\\n'), (2, 'from lamindb.setup import settings\\n'), (3, 'from "*

 * *            "lndb.dev._settings_store import instance_settings_file')], delete: [2, 1]}}, 2: "*

 * *            "{'id': '1be836bb', 'source': ['## Load your own instance by name']}, 3: {'id': "*

 * *            "'a5c94e19', 'source': ['If the user is the instance owner, just load the instance by "*

 * *            "name:']}, 4: {'id': 'e292c512', […]*

```diff
@@ -3,296 +3,229 @@
         {
             "cell_type": "markdown",
             "id": "b43d09d5-26d3-440d-b334-9643ec5248e6",
             "metadata": {
                 "tags": []
             },
             "source": [
-                "# Set storage"
+                "# Load & close an instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "33c2bb76-d61f-4866-87e2-780e61600022",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import lamindb as ln\n",
-                "from pathlib import Path\n",
-                "import laminci"
+                "import os\n",
+                "from lamindb.setup import settings\n",
+                "from lndb.dev._settings_store import instance_settings_file"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "a7cf42fb",
+            "id": "1be836bb",
             "metadata": {},
             "source": [
-                "## Set storage for PostgreSQL instance"
+                "## Load your own instance by name"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "8fd59ad3-04b9-42fb-83cc-ab7beedbec72",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "pgurl = laminci.db.setup_local_test_postgres()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "d6b0bd5e",
+            "cell_type": "markdown",
+            "id": "a5c94e19",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ln.setup.init(storage=\"./storage_1\", db=pgurl)"
+                "If the user is the instance owner, just load the instance by name:"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ceb57cc9",
+            "id": "e292c512",
             "metadata": {},
             "source": [
-                "Running \n",
                 "```\n",
-                "!lamin set --storage ./storage_2\n",
-                "```\n",
-                "on the command line runs the following Python function:"
+                "!lamin load mydata\n",
+                "```"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "49b9ef11",
+            "id": "e7ecc665",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.set.storage(\"./storage_2\")"
+                "ln.setup.load(\"mydata\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8e481aa0",
+            "id": "2276e0be",
             "metadata": {
-                "tags": []
+                "tags": [
+                    "hide-cell"
+                ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_2\""
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "25a13298",
-            "metadata": {},
-            "source": [
-                "Running \n",
-                "```\n",
-                "lamin set --storage s3://lndb-setup-ci\n",
-                "```\n",
-                "\n",
-                "on the command line runs the following:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "8436575d",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "ln.setup.set.storage(\"s3://lndb-setup-ci\")"
+                "assert settings.instance.storage.is_cloud == False\n",
+                "assert settings.instance.name == \"mydata\"\n",
+                "assert settings.instance.storage.root.as_posix() == f\"{os.getcwd()}/mydata\"\n",
+                "assert settings.instance.storage.cache_dir is None\n",
+                "assert settings.instance.db == f\"sqlite:///{os.getcwd()}/mydata/mydata.lndb\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d2934990",
+            "id": "4f179b5b",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "assert ln.setup.settings.storage.is_cloud\n",
-                "assert ln.setup.settings.storage.root_as_str == \"s3://lndb-setup-ci\""
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "7bd9997b",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# root.fs contains the underlying fsspec filesystem\n",
-                "assert (\n",
-                "    ln.setup.settings.storage.root.fs.cache_regions  # set by lamindb to True for s3 by default\n",
-                ")"
+                "# another test case, this time with a manually configured instance name\n",
+                "ln.setup.load(\"pgtest-registered\")\n",
+                "assert settings.instance.storage.is_cloud == True\n",
+                "assert settings.instance.name == \"pgtest-registered\"\n",
+                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\""
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "ae953b6a",
+            "id": "3f47a1d4",
             "metadata": {},
             "source": [
-                "It is possible to set any additional `fsspec` filesystem arguments for cloud storage, such as `profile` or `cache_regions` (for s3 only), for example:"
+                "This also works for remote instances:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "f9294082",
-            "metadata": {},
+            "id": "7c9698f9",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ln.setup.set.storage(\"s3://lndb-setup-ci\", cache_regions=False)"
+                "# ensure that the locally cached env file is deleted\n",
+                "instance_settings_file(\"lndb-setup-ci\", \"testuser1\").unlink()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "5f320819",
+            "id": "089a3832",
             "metadata": {},
             "outputs": [],
             "source": [
-                "assert not ln.setup.settings.storage.root.fs.cache_regions"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "529e68e5-9b10-4fdb-9d4c-ac8206bbbb68",
-            "metadata": {},
-            "source": [
-                "### Set storage not by owner"
+                "ln.setup.load(\"lndb-setup-ci\")  # lamin load lndb-setup-ci"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "d6915638-db49-4d3d-bd91-819bb4719ef7",
-            "metadata": {},
+            "id": "1ebd784f",
+            "metadata": {
+                "tags": [
+                    "hide-cell"
+                ]
+            },
             "outputs": [],
             "source": [
-                "ln.setup.login(\n",
-                "    \"testuser2@lamin.ai\", password=\"goeoNJKE61ygbz1vhaCVynGERaRrlviPBVQsjkhz\"\n",
+                "assert settings.instance.storage.is_cloud == True\n",
+                "assert settings.instance.storage.root_as_str == \"s3://lndb-setup-ci\"\n",
+                "assert (\n",
+                "    settings.instance._sqlite_file.as_posix() == \"s3://lndb-setup-ci/lndb-setup-ci.lndb\"\n",
                 ")"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "2ed8716f-852f-4ce9-8eef-5b824d6e92b3",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "id": "914af9a6",
+            "metadata": {},
             "source": [
-                "ln.setup.set.storage(\"./storage_3\")"
+                "## Load instance from another owner"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "cad87623",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
-            "outputs": [],
+            "cell_type": "markdown",
+            "id": "65ab467e",
+            "metadata": {},
             "source": [
-                "assert ln.setup.settings.storage.root_as_str == f\"{Path.cwd()}/storage_3\""
+                "If you have the permission, you can load an instance from another owner. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "78a819fa-48d6-4c6f-95d4-7dc7e94283bb",
-            "metadata": {
-                "tags": [
-                    "hide-cell"
-                ]
-            },
+            "id": "8436575d",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "!docker stop pgtest && docker rm pgtest"
+                "ln.setup.load(\"testuser1/mydata\")  # lamin load \"testuser1/mydata\""
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "3fb6a223",
-            "metadata": {
-                "tags": []
-            },
-            "source": [
-                "## Set storage for SQLite instance"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "6ccb6573",
+            "id": "0986a5f3",
             "metadata": {},
             "source": [
-                "If the user tries to set the storage for an sqlite instance, an error message is raised:"
+                "Load an instance from wrong owner."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "49309f3a-199f-40bc-b318-a396ebcaafec",
+            "id": "bc3568ae",
             "metadata": {},
             "outputs": [],
             "source": [
-                "ln.setup.login(\"testuser1\")"
+                "assert ln.setup.load(\"testuser2/mydata\") == \"instance-not-reachable\""
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f988a386",
+            "cell_type": "markdown",
+            "id": "e3701120",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ln.setup.load(\"mydata\")"
+                "## Close an instance"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "e4f2545f",
-            "metadata": {
-                "tags": []
-            },
+            "id": "8e54d8cd",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "assert ln.setup.set.storage(\"mydata_storage_2\") == \"set-storage-failed\""
+                "ln.setup.close()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "4fa82d8b",
+            "id": "12db83b9-9d14-4575-876a-3d640a1c1e10",
             "metadata": {
                 "tags": [
                     "hide-cell"
                 ]
             },
             "outputs": [],
             "source": [
-                "ln.setup.set_storage(\"mydata_storage_2\")"
+                "# clean up\n",
+                "!lamin delete pgtest-registered\n",
+                "!docker stop pgtest-registered && docker rm pgtest-registered"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -304,18 +237,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.15"
         },
         "vscode": {
             "interpreter": {
-                "hash": "61b4062b24dfb1010f420dad5aa3bd73a4d2af47d0ec44eafec465a35a9d7239"
+                "hash": "5c7b89af1651d0b8571dde13640ecdccf7d5a6204171d6ab33e7c296e100e08a"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/05-schema-modules.ipynb` & `lnhub_rest-0.9.7/lndb/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/06-info.ipynb` & `lnhub_rest-0.9.7/lndb/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/07-delete.ipynb` & `lnhub_rest-0.9.7/lndb/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/docs/guide/migrate.md` & `lnhub_rest-0.9.7/lndb/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/__init__.py` & `lnhub_rest-0.9.7/lndb/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.44.7"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lnhub_rest-0.9.6/lndb/lndb/__main__.py` & `lnhub_rest-0.9.7/lndb/lndb/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .dev._settings_user import user_description as user
 
 signup_help = "First time sign up."
 login_help = "Log in an already-signed-up user."
 init_help = "Init & config instance with db & storage."
 load_help = "Load instance by name."
 set_storage_help = "Set storage used by an instance."
-load_storage_help = "Load the instance with an updated default storage."
 info_help = "Show current instance information."
 close_help = "Close instance."
 migr_help = "Manage migrations."
 delete_help = "Delete an instance."
 register_help = (
     "Register instance on hub (local instances are not automatically registered)."
 )
@@ -40,37 +39,36 @@
 aa = login.add_argument
 aa(
     "user",
     type=str,
     metavar="user",
     help="Email or user handle. Email is needed at first login.",
 )  # noqa
-aa("--password", type=str, metavar="pw", default=None, help=user.password)
+aa("--password", type=str, metavar="s", default=None, help=user.password)
 
 # init instance
 init = subparsers.add_parser("init", help=init_help)
 aa = init.add_argument
 aa("--storage", type=str, metavar="s", help=instance.storage_root)
-aa("--db", type=str, metavar="d", default=None, help=instance.db)
-aa("--schema", type=str, metavar="schema", default=None, help=instance.schema)
-aa("--name", type=str, metavar="n", default=None, help=instance.name)
+aa("--db", type=str, metavar="s", default=None, help=instance.db)
+aa("--schema", type=str, metavar="s", default=None, help=instance.schema)
+aa("--name", type=str, metavar="s", default=None, help=instance.name)
 
 # load instance
 load = subparsers.add_parser("load", help=load_help)
 aa = load.add_argument
 instance_help = """
 The instance identifier can the instance name (owner is
 current user), handle/name, or the URL: https://lamin.ai/handle/name."""
-aa("instance", type=str, metavar="i", default=None, help=instance_help)
-aa("--storage", type=str, metavar="s", default=None, help=load_storage_help)
+aa("instance", type=str, metavar="s", default=None, help=instance_help)
 
 # delete instance
 delete_parser = subparsers.add_parser("delete", help=delete_help)
 aa = delete_parser.add_argument
-aa("instance", type=str, metavar="i", default=None, help=instance.name)
+aa("instance", type=str, metavar="s", default=None, help=instance.name)
 
 # show instance info
 info_parser = subparsers.add_parser("info", help=info_help)
 
 # set storage
 set_storage_parser = subparsers.add_parser("set", help=set_storage_help)
 aa = set_storage_parser.add_argument
@@ -115,15 +113,14 @@
             schema=args.schema,
             name=args.name,
         )
         return process_result(result)
     elif args.command == "load":
         result = _init_instance.load(
             identifier=args.instance,
-            storage=args.storage,
         )
         return process_result(result)
     elif args.command == "close":
         return close_instance()
     elif args.command == "register":
         return register()
     elif args.command == "delete":
```

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_check_instance_setup.py` & `lnhub_rest-0.9.7/lndb/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_close.py` & `lnhub_rest-0.9.7/lndb/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_delete.py` & `lnhub_rest-0.9.7/lndb/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_init_instance.py` & `lnhub_rest-0.9.7/lndb/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_load_instance.py` & `lnhub_rest-0.9.7/lndb/lndb/_load_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,41 +137,38 @@
 
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: Union[str, Path, UPath]
 ) -> None:
     isettings._persist()  # this is temporary for import of lnschema_core
     ssettings = StorageSettings(storage, instance_settings=isettings)
     if ssettings.is_cloud:
-        try:  # triggering ssettings.id makes a lookup in the storage table
+        try:
             logger.success(f"Loaded storage: {ssettings.id} / {ssettings.root_as_str}")
         except RuntimeError:
             raise RuntimeError(
                 "Storage not registered!\n"
                 "Load instance without the `storage` arg and register storage root: "
                 f"`lamin set storage --storage {storage}`"
             )
     else:
         # local storage
         # assumption is you want to merely update the storage location
         from lnschema_core import Storage
 
-        isettings._storage = ssettings  # need this here already
         if isettings.dialect == "sqlite":
-            isettings._engine = sqm.create_engine(isettings.db)
             with sqm.Session(isettings.engine) as session:
                 storage = session.exec(
                     sqm.select(Storage).where(Storage.root == ssettings.root_as_str)
                 ).one_or_none()
             if storage is None:
                 with sqm.Session(isettings.engine) as session:
                     storage_record = session.exec(sqm.select(Storage)).one()
                     storage_record.root = ssettings.root_as_str
                     session.add(storage_record)
                     session.commit()
-                    session.refresh(storage_record)
                 logger.success(
                     f"Updated storage root {storage_record.id} to"
                     f" {ssettings.root_as_str}"
                 )
         else:
             raise RuntimeError(
                 "Cannot currently not update local storage of sqlite upon load. Use"
```

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_migrate/alembic.ini` & `lnhub_rest-0.9.7/lndb/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_migrate/core.py` & `lnhub_rest-0.9.7/lndb/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_migrate/deploy.py` & `lnhub_rest-0.9.7/lndb/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_migrate/env.py` & `lnhub_rest-0.9.7/lndb/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_migrate/utils.py` & `lnhub_rest-0.9.7/lndb/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_register_instance.py` & `lnhub_rest-0.9.7/lndb/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_schema.py` & `lnhub_rest-0.9.7/lndb/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_set.py` & `lnhub_rest-0.9.7/lndb/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_settings.py` & `lnhub_rest-0.9.7/lndb/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/_setup_user.py` & `lnhub_rest-0.9.7/lndb/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/__init__.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_clone.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_db.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_deprecated.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_exclusion.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_settings_instance.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_settings_load.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_settings_save.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_settings_store.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_settings_user.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_setup_knowledge.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_setup_schema.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/_storage.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/dev/upath.py` & `lnhub_rest-0.9.7/lndb/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/test/_migrations_e2e.py` & `lnhub_rest-0.9.7/lndb/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/lndb/test/_migrations_unit.py` & `lnhub_rest-0.9.7/lndb/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/noxfile.py` & `lnhub_rest-0.9.7/lndb/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/pyproject.toml` & `lnhub_rest-0.9.7/lndb/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.4",
+    "lnhub_rest==0.9.2",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.28.0",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
@@ -24,15 +24,14 @@
     "appdirs",
     "python-dotenv",
     "erdiagram",
     "alembic",
     "natsort",
     "pandas",
     "python-dateutil",
-    "universal_pathlib"
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lndb"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `lnhub_rest-0.9.6/lndb/tests/test_bionty.py` & `lnhub_rest-0.9.7/lndb/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lndb/tests/test_init_instance.py` & `lnhub_rest-0.9.7/lndb/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/__main__.py` & `lnhub_rest-0.9.7/lnhub_rest/__main__.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.9.7/lnhub_rest/_assets/_schemas.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.9.7/lnhub_rest/_check_breaks_lndb.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/_ci.py` & `lnhub_rest-0.9.7/lnhub_rest/_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.9.7/lnhub_rest/_clean_ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/config.py` & `lnhub_rest-0.9.7/lnhub_rest/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 from urllib.request import urlretrieve
 
 from pydantic import BaseSettings, PostgresDsn
 
 
 class Connector(BaseSettings):
     url: str
     key: str
 
 
-def lamindb_client_config_settings(settings: BaseSettings) -> dict[str, Any]:
+def lamindb_client_config_settings(settings: BaseSettings) -> Dict[str, Any]:
     connector_file, _ = urlretrieve(
         "https://lamin-site-assets.s3.amazonaws.com/connector.env"
     )
     connector = Connector(_env_file=connector_file)
     return dict(
         lamin_env="client",
         supabase_api_url=connector.url,
```

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.9.7/lnhub_rest/core/account/_create_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.9.7/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.9.7/lnhub_rest/core/account/_delete_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.9.7/lnhub_rest/core/account/_signup_signin.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.9.7/lnhub_rest/core/account/_update_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/collaborator/_crud.py` & `lnhub_rest-0.9.7/lnhub_rest/core/collaborator/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.9.7/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.9.7/lnhub_rest/core/instance/_delete_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.9.7/lnhub_rest/core/instance/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.9.7/lnhub_rest/core/instance/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.9.7/lnhub_rest/core/instance/_update_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/member/_crud.py` & `lnhub_rest-0.9.7/lnhub_rest/core/member/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.9.7/lnhub_rest/core/storage/_add_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 
         # check if storage exists already
         storage = sb_select_storage_by_root(root, hub)
         if storage is not None:
             return storage["id"], None
 
         # add storage
-        if "LNHUB_NOT_USE_BOTO3" in os.environ:
+        # LNHUB_NOT_USE_BOTO3 is legacy
+        if (
+            "LNHUB_NOT_USE_BOTOCORE" in os.environ
+            or "LNHUB_NOT_USE_BOTO3" in os.environ  # noqa
+        ):
             storage_region = None
         else:
             storage_region = get_storage_region(root)
         storage_type = get_storage_type(root)
         storage = sb_insert_storage(
             {
                 "id": uuid4().hex,
@@ -73,18 +77,20 @@
 
 
 def get_storage_region(storage_root: str) -> Optional[str]:
     storage_root_str = str(storage_root)
     storage_region = None
 
     if storage_root_str.startswith("s3://"):
-        import boto3
+        import botocore.session
 
-        response = boto3.client("s3").get_bucket_location(
-            Bucket=storage_root_str.replace("s3://", "")
+        response = (
+            botocore.session.get_session()
+            .create_client("s3")
+            .get_bucket_location(Bucket=storage_root_str.replace("s3://", ""))
         )
         # returns `None` for us-east-1
         # returns a string like "eu-central-1" etc. for all other regions
         storage_region = response["LocationConstraint"]
         if storage_region is None:
             storage_region = "us-east-1"
```

### Comparing `lnhub_rest-0.9.6/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.9.7/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/main.py` & `lnhub_rest-0.9.7/lnhub_rest/main.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.9.7/lnhub_rest/orm/_sbclient.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/routers/account.py` & `lnhub_rest-0.9.7/lnhub_rest/routers/account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/routers/ci.py` & `lnhub_rest-0.9.7/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/routers/collaborator.py` & `lnhub_rest-0.9.7/lnhub_rest/routers/collaborator.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/routers/instance.py` & `lnhub_rest-0.9.7/lnhub_rest/routers/instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/routers/organization.py` & `lnhub_rest-0.9.7/lnhub_rest/routers/organization.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/routers/utils.py` & `lnhub_rest-0.9.7/lnhub_rest/routers/utils.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/_core.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/_core.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/alembic.ini` & `lnhub_rest-0.9.7/lnhub_rest/schema/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/clone.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/clone.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/testing.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/testing.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-15-8d91d067cc7d-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py` & `lnhub_rest-0.9.7/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/lnhub_rest/utils/_test.py` & `lnhub_rest-0.9.7/lnhub_rest/utils/_test.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/noxfile.py` & `lnhub_rest-0.9.7/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     session.run("pre-commit", "run", "--all-files")
 
 
 @nox.session
 @nox.parametrize("package", ["lnhub-rest", "lndb"])
 def test_local(session: nox.Session, package: str):
     session.install("./lndb[dev,test]")
-    session.install(".[dev,test]")
+    session.install(".[dev,test,server]")
     session.run(
         "pytest",
         "-s",
         "-m",
         "not integration",
         "--cov=lnhub_rest",
         "--cov-append",
@@ -36,15 +36,15 @@
 
 
 @nox.session
 @nox.parametrize("package", ["lnhub-rest", "lndb"])
 @nox.parametrize("lamin_env", ["staging"])
 def test_integrations(session: nox.Session, package: str, lamin_env: str):
     session.install("./lndb[dev,test]")
-    session.install(".[dev,test]")
+    session.install(".[dev,test,server]")
     session.run(
         "pytest",
         "-s",
         "-m",
         "integration",
         "--cov=lnhub_rest",
         "--cov-append",
```

### Comparing `lnhub_rest-0.9.6/pyproject.toml` & `lnhub_rest-0.9.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,41 +7,39 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # Do NOT add any lamin package as a dependency here!
     # Neither laminci nor lndb nor lnschema_core etc.
     # lnhub_rest needs to be upstream
-    "lamin_logger>=0.2.3",
-    "supabase==1.0.2",
-    "fastapi",
-    "uvicorn",
-    "sqlmodel",
-    "pandas",
-    "python-dotenv",
-    "alembic",
-    "psycopg2-binary",
-    "pyjwt",
-    "pytest_alembic==0.9.1",  # let's pin this as we use internals
-    "boto3", # for aiobotocore inside s3fs, to fix deps resolution
-    "deepdiff",
+    "lamin_logger",
+    "supabase==1.0.3",
 ]
 
 [project.urls]
 Home = "https://github.com/laminlabs/lnhub-rest"
 
 [project.optional-dependencies]
+server = [
+    "fastapi",
+    "uvicorn",
+    "sqlmodel",
+    "alembic",
+    "pytest_alembic==0.9.1",  # let's pin this as we use internals
+    "psycopg2-binary",
+]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
     "pytest>=6.0",
     "pytest-cov",
     "nbproject",
+    "botocore",
 ]
 
 [project.scripts]
 lnhub = "lnhub_rest.__main__:main"
 
 [tool.black]
 preview = true
```

### Comparing `lnhub_rest-0.9.6/supabase/config.toml` & `lnhub_rest-0.9.7/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/tests/test_notebooks.py` & `lnhub_rest-0.9.7/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.9.6/PKG-INFO` & `lnhub_rest-0.9.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.9.6
+Version: 0.9.7
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lamin_logger>=0.2.3
-Requires-Dist: supabase==1.0.2
-Requires-Dist: fastapi
-Requires-Dist: uvicorn
-Requires-Dist: sqlmodel
-Requires-Dist: pandas
-Requires-Dist: python-dotenv
-Requires-Dist: alembic
-Requires-Dist: psycopg2-binary
-Requires-Dist: pyjwt
-Requires-Dist: pytest_alembic==0.9.1
-Requires-Dist: boto3
-Requires-Dist: deepdiff
+Requires-Dist: lamin_logger
+Requires-Dist: supabase==1.0.3
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
+Requires-Dist: fastapi ; extra == "server"
+Requires-Dist: uvicorn ; extra == "server"
+Requires-Dist: sqlmodel ; extra == "server"
+Requires-Dist: alembic ; extra == "server"
+Requires-Dist: pytest_alembic==0.9.1 ; extra == "server"
+Requires-Dist: psycopg2-binary ; extra == "server"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
+Requires-Dist: botocore ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnhub-rest
 Provides-Extra: dev
+Provides-Extra: server
 Provides-Extra: test
 
 # lnhub-rest: Cross-instance management
 
 Note: For more extensive documentation & testing, see [docs](docs).
 
 ## Summary
```

