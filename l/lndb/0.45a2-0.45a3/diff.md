# Comparing `tmp/lndb-0.45a2.tar.gz` & `tmp/lndb-0.45a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.45a2.tar", last modified: Fri May 26 09:56:30 2023, max compression
+gzip compressed data, was "lndb-0.45a3.tar", last modified: Sun May 28 12:53:45 2023, max compression
```

## Comparing `lndb-0.45a2.tar` & `lndb-0.45a3.tar`

### file list

```diff
@@ -1,79 +1,78 @@
--rw-r--r--   0        0        0     3832 2023-05-24 18:13:34.371502 lndb-0.45a2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-24 18:13:34.371611 lndb-0.45a2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-24 18:13:34.371684 lndb-0.45a2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-24 18:13:34.371770 lndb-0.45a2/.gitignore
--rw-r--r--   0        0        0     1777 2023-05-24 18:13:34.371851 lndb-0.45a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-24 18:13:34.371968 lndb-0.45a2/LICENSE
--rw-r--r--   0        0        0      173 2023-05-24 18:13:34.372033 lndb-0.45a2/README.md
--rw-r--r--   0        0        0       52 2023-05-24 18:13:34.372124 lndb-0.45a2/docs/api.md
--rw-r--r--   0        0        0    49086 2023-05-26 09:55:24.478970 lndb-0.45a2/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-05-24 18:13:34.372476 lndb-0.45a2/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-05-24 18:13:34.372565 lndb-0.45a2/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-05-24 18:13:34.372660 lndb-0.45a2/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-05-24 18:13:34.372727 lndb-0.45a2/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-05-24 18:13:34.372809 lndb-0.45a2/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-05-24 18:13:34.372876 lndb-0.45a2/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2589 2023-05-25 22:02:47.332671 lndb-0.45a2/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-05-24 18:13:34.373075 lndb-0.45a2/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5025 2023-05-25 13:55:42.990512 lndb-0.45a2/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11082 2023-05-26 09:53:42.760584 lndb-0.45a2/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     6639 2023-05-25 13:55:42.990928 lndb-0.45a2/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     7616 2023-05-25 13:56:23.677378 lndb-0.45a2/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3724 2023-05-25 15:46:50.017574 lndb-0.45a2/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-05-25 13:55:42.991225 lndb-0.45a2/docs/guide/index.md
--rw-r--r--   0        0        0     3331 2023-05-24 18:13:34.373961 lndb-0.45a2/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-05-24 18:13:34.374075 lndb-0.45a2/docs/index.md
--rw-r--r--   0        0        0      118 2023-05-24 18:13:34.374173 lndb-0.45a2/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-05-26 09:54:53.204802 lndb-0.45a2/lndb/__init__.py
--rw-r--r--   0        0        0     5268 2023-05-24 18:13:34.374405 lndb-0.45a2/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-05-24 18:13:34.374517 lndb-0.45a2/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-24 18:13:34.374613 lndb-0.45a2/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-05-26 09:08:58.517667 lndb-0.45a2/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-05-24 18:13:34.374754 lndb-0.45a2/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-05-24 18:13:34.374825 lndb-0.45a2/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-05-24 18:13:34.374892 lndb-0.45a2/lndb/_info.py
--rw-r--r--   0        0        0     6035 2023-05-25 12:49:05.083933 lndb-0.45a2/lndb/_init_instance.py
--rw-r--r--   0        0        0     6729 2023-05-24 18:13:34.375083 lndb-0.45a2/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-05-24 18:13:34.375181 lndb-0.45a2/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-05-24 18:13:34.375248 lndb-0.45a2/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-05-24 18:13:34.375322 lndb-0.45a2/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7555 2023-05-26 09:53:47.457599 lndb-0.45a2/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-05-24 18:13:34.375498 lndb-0.45a2/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-05-24 18:13:34.375575 lndb-0.45a2/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-05-24 18:13:34.375787 lndb-0.45a2/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      790 2023-05-24 18:13:34.375906 lndb-0.45a2/lndb/_notebook.py
--rw-r--r--   0        0        0      803 2023-05-24 18:13:34.375990 lndb-0.45a2/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-05-24 18:13:34.376692 lndb-0.45a2/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-05-24 18:13:34.377124 lndb-0.45a2/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-05-24 18:13:34.377222 lndb-0.45a2/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-05-24 18:13:34.377292 lndb-0.45a2/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-05-24 18:13:34.377359 lndb-0.45a2/lndb/_settings_store.py
--rw-r--r--   0        0        0     3905 2023-05-24 18:13:34.377464 lndb-0.45a2/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-05-24 18:13:34.377571 lndb-0.45a2/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-05-24 18:13:34.377656 lndb-0.45a2/lndb/dev/_clone.py
--rw-r--r--   0        0        0     7299 2023-05-26 07:50:36.465517 lndb-0.45a2/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-05-24 18:13:34.397245 lndb-0.45a2/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-05-24 18:13:34.397345 lndb-0.45a2/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-05-24 18:13:34.397862 lndb-0.45a2/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8946 2023-05-24 18:13:34.397995 lndb-0.45a2/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-05-24 18:13:34.398092 lndb-0.45a2/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-05-24 18:13:34.398168 lndb-0.45a2/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-05-24 18:13:34.398249 lndb-0.45a2/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-05-24 18:13:34.398328 lndb-0.45a2/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2710 2023-05-25 21:55:19.754812 lndb-0.45a2/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     4466 2023-05-26 09:53:47.457948 lndb-0.45a2/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-05-24 18:13:34.398603 lndb-0.45a2/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-05-24 18:13:34.398679 lndb-0.45a2/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-05-24 18:13:34.398758 lndb-0.45a2/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-05-24 18:13:34.398886 lndb-0.45a2/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-05-24 18:13:34.398951 lndb-0.45a2/lndb/test/_env.py
--rw-r--r--   0        0        0     3911 2023-05-24 18:13:34.399040 lndb-0.45a2/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-05-24 18:13:34.399143 lndb-0.45a2/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-05-24 18:13:34.399213 lndb-0.45a2/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-05-24 18:13:34.399292 lndb-0.45a2/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-05-24 18:13:34.399371 lndb-0.45a2/noxfile.py
--rw-r--r--   0        0        0     1419 2023-05-26 09:53:47.458248 lndb-0.45a2/pyproject.toml
--rw-r--r--   0        0        0      513 2023-05-24 18:13:34.399557 lndb-0.45a2/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-05-24 18:13:34.399639 lndb-0.45a2/tests/test_init_instance.py
--rw-r--r--   0        0        0      379 2023-05-24 18:13:34.399723 lndb-0.45a2/tests/test_notebooks.py
--rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 lndb-0.45a2/PKG-INFO
+-rw-r--r--   0        0        0     3804 2023-05-27 08:31:20.462437 lndb-0.45a3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.45a3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.45a3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.45a3/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-23 22:02:46.131957 lndb-0.45a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.45a3/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.45a3/README.md
+-rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.45a3/docs/api.md
+-rw-r--r--   0        0        0    49387 2023-05-28 12:53:18.343383 lndb-0.45a3/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.45a3/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.45a3/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8795 2023-05-26 18:42:19.597992 lndb-0.45a3/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.45a3/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.45a3/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.45a3/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2589 2023-05-27 05:58:01.864810 lndb-0.45a3/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.45a3/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     8540 2023-05-27 09:10:15.195959 lndb-0.45a3/docs/guide/00-index.ipynb
+-rw-r--r--   0        0        0     5025 2023-05-26 16:29:38.650577 lndb-0.45a3/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11082 2023-05-26 16:29:38.651219 lndb-0.45a3/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     6639 2023-05-26 16:29:38.651368 lndb-0.45a3/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     7616 2023-05-26 16:29:38.651991 lndb-0.45a3/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-05-26 16:29:38.652557 lndb-0.45a3/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     3331 2023-05-24 18:12:34.768903 lndb-0.45a3/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.45a3/docs/index.md
+-rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.45a3/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-05-28 12:53:10.436966 lndb-0.45a3/lndb/__init__.py
+-rw-r--r--   0        0        0     5268 2023-05-24 18:12:34.769088 lndb-0.45a3/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.45a3/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.45a3/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-05-28 12:52:47.657543 lndb-0.45a3/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.45a3/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.45a3/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-24 17:57:29.952669 lndb-0.45a3/lndb/_info.py
+-rw-r--r--   0        0        0     6247 2023-05-26 16:29:38.653812 lndb-0.45a3/lndb/_init_instance.py
+-rw-r--r--   0        0        0     6661 2023-05-26 16:29:38.653964 lndb-0.45a3/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.45a3/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.45a3/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-24 17:08:25.124000 lndb-0.45a3/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7611 2023-05-27 05:58:01.865831 lndb-0.45a3/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.45a3/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-24 17:25:24.780147 lndb-0.45a3/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.45a3/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      790 2023-05-24 18:12:34.769186 lndb-0.45a3/lndb/_notebook.py
+-rw-r--r--   0        0        0      803 2023-04-28 18:11:00.215484 lndb-0.45a3/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.45a3/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-23 22:02:46.133073 lndb-0.45a3/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.45a3/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.45a3/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.45a3/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3905 2023-05-12 07:21:12.821554 lndb-0.45a3/lndb/_setup_user.py
+-rw-r--r--   0        0        0      456 2023-05-26 16:29:43.073569 lndb-0.45a3/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     3886 2023-05-26 16:39:31.260401 lndb-0.45a3/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     7299 2023-05-26 16:40:04.945302 lndb-0.45a3/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.45a3/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.45a3/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.45a3/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8946 2023-04-28 18:11:00.215703 lndb-0.45a3/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.45a3/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.45a3/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.45a3/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.45a3/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2710 2023-05-26 16:29:38.655499 lndb-0.45a3/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     4466 2023-05-26 16:29:38.655928 lndb-0.45a3/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-23 22:02:46.133274 lndb-0.45a3/lndb/dev/_storage.py
+-rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.45a3/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.45a3/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.45a3/lndb/test/_env.py
+-rw-r--r--   0        0        0     3913 2023-05-26 16:40:53.833999 lndb-0.45a3/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.45a3/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      254 2023-05-26 16:43:38.785220 lndb-0.45a3/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.45a3/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.45a3/noxfile.py
+-rw-r--r--   0        0        0     1318 2023-05-28 12:52:50.543577 lndb-0.45a3/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.45a3/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.45a3/tests/test_init_instance.py
+-rw-r--r--   0        0        0      379 2023-05-12 07:21:08.563165 lndb-0.45a3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1187 1970-01-01 00:00:00.000000 lndb-0.45a3/PKG-INFO
```

### Comparing `lndb-0.45a2/.github/workflows/build.yml` & `lndb-0.45a3/.github/workflows/build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -56,16 +56,15 @@
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: Cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
       - name: Install Python dependencies
         run: |
           python -m pip install -U pip
-          pip install -U laminci
-          pip install -U lamindb
+          pip install lamindb==0.41a3
       - name: Install apt-get dependencies
         run: |
           sudo apt-get -y install graphviz
           sudo apt-get install sqlite3-tools=3.37.2-2
           sudo apt-get install libpq-dev
       - name: Lint
         run: |
```

### Comparing `lndb-0.45a2/.github/workflows/latest-changes.yml` & `lndb-0.45a3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/.gitignore` & `lndb-0.45a3/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/.pre-commit-config.yaml` & `lndb-0.45a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/LICENSE` & `lndb-0.45a3/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/changelog.md` & `lndb-0.45a3/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⬆️ Upgrade lnhub-rest to 0.9.7 | [383](https://github.com/laminlabs/lndb/pull/383) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 | 0.45a3
+📝 Add setup overview from lamindb | [382](https://github.com/laminlabs/lndb/pull/382) | [falexwolf](https://github.com/falexwolf) | 2023-05-27 |
 🔥 Remove schema modules logic from `setup_schema` | [381](https://github.com/laminlabs/lndb/pull/381) | [falexwolf](https://github.com/falexwolf) | 2023-05-26 | 0.45a2
 🏗️ Remove SQL-level schema modules | [380](https://github.com/laminlabs/lndb/pull/380) | [falexwolf](https://github.com/falexwolf) | 2023-05-25 | 0.45a1
 ✨ Add track command to CLI | [378](https://github.com/laminlabs/lndb/pull/378) | [Koncopd](https://github.com/Koncopd) | 2023-05-23 |
 📝 Improve migration docs | [379](https://github.com/laminlabs/lndb/pull/379) | [Zethson](https://github.com/Zethson) | 2023-05-22 |
 🔊 Use lamin_logger in test_notebooks.py | [376](https://github.com/laminlabs/lndb/pull/376) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 Add universal_pathlib to dependencies | [375](https://github.com/laminlabs/lndb/pull/375) | [Zethson](https://github.com/Zethson) | 2023-05-02 |
 ⬆️ Upgrade lnhub-rest to 0.9.4 | [373](https://github.com/laminlabs/lndb/pull/373) | [sunnyosun](https://github.com/sunnyosun) | 2023-04-28 | 0.44.7
```

### Comparing `lndb-0.45a2/docs/faq/check-synchronization.ipynb` & `lndb-0.45a3/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/faq/clone.ipynb` & `lndb-0.45a3/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.45a3/docs/faq/edge-cases-login-init.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9855368589743589%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'source': {insert: [(8, 'from laminci.db "*

 * *            "import setup_local_test_postgres\\n')], delete: [8]}}, 2: {'attachments': "*

 * *            "OrderedDict()}, 4: {'attachments': OrderedDict()}, 6: {'attachments': OrderedDict()}, "*

 * *            "8: {'attachments': OrderedDict()}, 10: {'attachments': OrderedDict()}, 12: "*

 * *            "{'attachments': OrderedDict()}, 14: {'attachments': OrderedDict()}, 16: "*

 * *            "{'attachments': OrderedDict()}, 18:  […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Edge cases for login, init, load"
             ]
         },
         {
@@ -17,24 +18,25 @@
                 "from lamindb.setup import settings\n",
                 "from lndb.dev._settings_store import (\n",
                 "    current_instance_settings_file,\n",
                 "    current_user_settings_file,\n",
                 "    get_settings_file_name_prefix,\n",
                 "    settings_dir,\n",
                 ")\n",
-                "from lndb.dev import setup_local_test_postgres\n",
+                "from laminci.db import setup_local_test_postgres\n",
                 "from lndb.dev._settings_store import instance_settings_file\n",
                 "import nbproject\n",
                 "import pytest\n",
                 "import os\n",
                 "\n",
                 "nbproject.header()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Log in with in-sufficient information"
             ]
         },
         {
@@ -44,14 +46,15 @@
             "outputs": [],
             "source": [
                 "with pytest.raises(TypeError):\n",
                 "    lnsetup.login()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If we add an email or handle it looks up the password from the stored env file (`lamin login testuser1@lamin.ai`):"
             ]
         },
         {
@@ -60,14 +63,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "lnsetup.login(\"testuser1@lamin.ai\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now, let's start with a fresh environment without any user profiles stored."
             ]
         },
         {
@@ -80,14 +84,15 @@
                 "    settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1@lamin.ai.env\"\n",
                 ").unlink()\n",
                 "(settings_dir / f\"{get_settings_file_name_prefix()}user-testuser1.env\").unlink()\n",
                 "current_user_settings_file().unlink()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If we try to login with a handle at first login, this will error:"
             ]
         },
         {
@@ -97,14 +102,15 @@
             "outputs": [],
             "source": [
                 "with pytest.raises(RuntimeError):\n",
                 "    lnsetup.login(\"testuser1\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If we try to login without password, this will error:"
             ]
         },
         {
@@ -114,14 +120,15 @@
             "outputs": [],
             "source": [
                 "with pytest.raises(RuntimeError):\n",
                 "    lnsetup.login(\"testuser1@lamin.ai\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "If we try login with a wrong password, this will error:"
             ]
         },
         {
@@ -131,14 +138,15 @@
             "outputs": [],
             "source": [
                 "result = lnsetup.login(\"testuser1@lamin.ai\", password=\"hello\")\n",
                 "assert result == \"could-not-login\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Hence, we need to login once with email and password:"
             ]
         },
         {
@@ -150,14 +158,15 @@
                 "result = lnsetup.login(\n",
                 "    \"testuser1@lamin.ai\", password=\"cEvcwMJFX4OwbsYVaMt2Os6GxxGgDUlBGILs2RyS\"\n",
                 ")\n",
                 "assert result is None"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "And now we can have the convenient login just with the handle."
             ]
         },
         {
@@ -167,14 +176,15 @@
             "outputs": [],
             "source": [
                 "result = lnsetup.login(\"testuser1\")\n",
                 "assert result is None"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Configuration with insufficient information"
             ]
         },
         {
@@ -183,14 +193,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "current_user_settings_file().unlink()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We'd also get an error about not being logged in if we try to init an instance without it being set:"
             ]
         },
         {
@@ -200,14 +211,15 @@
             "outputs": [],
             "source": [
                 "with pytest.raises(RuntimeError):\n",
                 "    lnsetup.init(storage=\"mydata\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's log in again."
             ]
         },
         {
@@ -217,14 +229,15 @@
             "outputs": [],
             "source": [
                 "result = lnsetup.login(\"testuser1\")\n",
                 "assert result is None"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's now try to init without providing storage (`lamin init`):"
             ]
         },
         {
@@ -234,14 +247,15 @@
             "outputs": [],
             "source": [
                 "with pytest.raises(TypeError):\n",
                 "    lnsetup.init()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "However, if we set a location (`lamin init --storage \"mydata\"`)"
             ]
         },
         {
@@ -250,21 +264,23 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "lnsetup.init(storage=\"mydata\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Local instances can not be loaded via the hub"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "It's not possible to load an instance from the hub if it has a local component, say, local storage."
             ]
         },
         {
@@ -283,14 +299,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "assert lnsetup.load(\"local_storage_instance\") == \"instance-not-reachable\""
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "It's not possible to load an instance from the hub if it's using a local db."
             ]
         },
         {
@@ -333,14 +350,15 @@
             },
             "outputs": [],
             "source": [
                 "!docker stop pgtest_remote_storage && docker rm pgtest_remote_storage"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Invalid command"
             ]
         },
         {
```

### Comparing `lndb-0.45a2/docs/faq/manage-migrations.ipynb` & `lndb-0.45a3/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/faq/switch-environment.ipynb` & `lndb-0.45a3/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.45a3/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/faq/test-migrations-unit.ipynb` & `lndb-0.45a3/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/guide/01-setup-user.ipynb` & `lndb-0.45a3/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/guide/02-init-instance.ipynb` & `lndb-0.45a3/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/guide/03-load-instance.ipynb` & `lndb-0.45a3/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/guide/04-set-storage.ipynb` & `lndb-0.45a3/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/guide/05-schema-modules.ipynb` & `lndb-0.45a3/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/docs/guide/migrate.md` & `lndb-0.45a3/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/__init__.py` & `lndb-0.45a3/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.45a2"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.45a3"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.45a2/lndb/__main__.py` & `lndb-0.45a3/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_check_instance_setup.py` & `lndb-0.45a3/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_close.py` & `lndb-0.45a3/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_delete.py` & `lndb-0.45a3/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_init_instance.py` & `lndb-0.45a3/lndb/_init_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,24 @@
 
 def register(isettings: InstanceSettings, usettings):
     """Register user & storage in DB."""
     upsert.user(usettings.email, usettings.id, usettings.handle, usettings.name)
     insert_if_not_exists.storage(isettings.storage)
 
 
-def reload_lamindb():
+def reload_lamindb(isettings: InstanceSettings):
     # only touch lamindb if we're operating from lamindb
     if "lamindb" in sys.modules:
         import lamindb
 
         importlib.reload(lamindb)
+    else:
+        # only log if we're outside lamindb
+        # lamindb itself logs upon import!
+        logger.success(f"Loaded instance: {isettings.owner}/{isettings.name}")
 
 
 def persist_settings_load_schema(isettings: InstanceSettings):
     # The reason for why the following two calls should always come together
     # is that the schema modules need information about what type of database
     # (sqlite or not) is mounted at time of importing the module!
     # hence, the schema modules look for the settings file that is generated
@@ -153,15 +157,15 @@
     else:
         # we're currently using this for testing migrations
         # passing connection strings of databases that need to be tested
         # for migrations
         logger.warning("Your instance seems already set up, attempt load:")
         message = load_from_isettings(isettings, migrate=_migrate)
 
-    reload_lamindb()
+    reload_lamindb(isettings)
     logger.success(
         f"Created & loaded instance: {settings.user.handle}/{isettings.name}"
     )
     return message
 
 
 def infer_instance_name(
```

### Comparing `lndb-0.45a2/lndb/_load_instance.py` & `lndb-0.45a3/lndb/_load_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,19 +86,16 @@
             logger.warning(
                 "Instance metadata exists, but DB might have been corrupted or deleted."
                 " Re-initializing the DB."
             )
             return "instance-not-reachable"
 
     message = load_from_isettings(isettings, migrate)
-
     if not message == "migrate-failed":
         os.environ["LAMINDB_INSTANCE_LOADED"] = "1"
-
-    logger.success(f"Loaded instance: {isettings.owner}/{isettings.name}")
     return message
 
 
 def get_owner_name_from_identifier(identifier: str):
     if "/" in identifier:
         if identifier.startswith("https://lamin.ai/"):
             identifier = identifier.replace("https://lamin.ai/", "")
@@ -127,15 +124,15 @@
     message = check_deploy_migration(
         usettings=settings.user, isettings=isettings, attempt_deploy=migrate
     )
     if message == "migrate-failed":
         return message
     register(isettings, settings.user)
     load_bionty_versions(isettings)
-    reload_lamindb()
+    reload_lamindb(isettings)
     return message
 
 
 def update_isettings_with_storage(
     isettings: InstanceSettings, storage: Union[str, Path, UPath]
 ) -> None:
     isettings._persist()  # this is temporary for import of lnschema_core
```

### Comparing `lndb-0.45a2/lndb/_migrate/alembic.ini` & `lndb-0.45a3/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_migrate/core.py` & `lndb-0.45a3/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_migrate/deploy.py` & `lndb-0.45a3/lndb/_migrate/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,18 @@
             )
     else:  # if the current version is higher or equal to the latest deployed version
         # no need to worry if current migration is same as deployed migration
         if current_migration == deployed_migration:
             deploy_migration = False
         else:
             logger.warning(
-                f"Deployed schema {schema_name} v{deployed_version} (migration"
-                f" {deployed_migration}) is not up to date with installed"
-                f" v{current_version} (migration {current_migration})"
+                f"In instance {isettings.identifier}, deployed schema"
+                f" {schema_name} v{deployed_version} (migration {deployed_migration})"
+                f" is not up to date with installed v{current_version} (migration"
+                f" {current_migration})"
             )
             # if migration is confirmed, continue
             if "PYTEST_CURRENT_TEST" not in os.environ:
                 logger.warning(
                     "You might need to run the command in a shell if you can't respond"
                     " to the following dialogue"
                 )
```

### Comparing `lndb-0.45a2/lndb/_migrate/env.py` & `lndb-0.45a3/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_migrate/utils.py` & `lndb-0.45a3/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_notebook.py` & `lndb-0.45a3/lndb/_notebook.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_register_instance.py` & `lndb-0.45a3/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_schema.py` & `lndb-0.45a3/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_set.py` & `lndb-0.45a3/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_settings.py` & `lndb-0.45a3/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/_setup_user.py` & `lndb-0.45a3/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_clone.py` & `lndb-0.45a3/lndb/dev/_clone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """Clone a database to a test database, with built in fetch-depth."""
 # This starts out with https://stackoverflow.com/questions/70392123
 from typing import Optional
 
 import sqlalchemy as sa
+from laminci.db import setup_local_test_postgres, setup_local_test_sqlite_file  # noqa
 from sqlalchemy import MetaData, create_engine, func, select
 
 from .._settings import settings
 from ._settings_instance import InstanceSettings
-from ._testdb import (
-    setup_local_test_postgres,
-    setup_local_test_postgres_supabase,
-    setup_local_test_sqlite_file,
-)
 
 
 def clone_schema(
     schema, src_conn, src_metadata, tgt_conn, tgt_metadata, tgt_engine, n_rows: int
 ):
     n_rows_test = n_rows
     # !!! switch off foreign key integrity !!!
@@ -54,26 +50,23 @@
             tgt_conn.execute(table.insert(), values)
             tgt_conn.commit()
 
 
 def clone_test(
     src_settings: Optional[InstanceSettings] = None,
     n_rows: int = 10000,
-    supabase: bool = False,
 ):
     """Clone from current instance to a test instance."""
     if src_settings is None:
         src_settings = settings.instance
     src_engine = create_engine(src_settings.db)
     src_metadata = MetaData()
 
     if src_settings.dialect == "sqlite":
         tgt_db = setup_local_test_sqlite_file(src_settings)
-    elif supabase:
-        tgt_db = setup_local_test_postgres_supabase()
     else:
         tgt_db = setup_local_test_postgres()
 
     assert tgt_db != src_settings.db
 
     tgt_engine = create_engine(tgt_db, future=True)
     tgt_metadata = MetaData()
```

### Comparing `lndb-0.45a2/lndb/dev/_db.py` & `lndb-0.45a3/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_deprecated.py` & `lndb-0.45a3/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_exclusion.py` & `lndb-0.45a3/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_settings_instance.py` & `lndb-0.45a3/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_settings_load.py` & `lndb-0.45a3/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_settings_save.py` & `lndb-0.45a3/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_settings_store.py` & `lndb-0.45a3/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_settings_user.py` & `lndb-0.45a3/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_setup_knowledge.py` & `lndb-0.45a3/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_setup_schema.py` & `lndb-0.45a3/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/_storage.py` & `lndb-0.45a3/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/dev/upath.py` & `lndb-0.45a3/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/lndb/test/_migrations_e2e.py` & `lndb-0.45a3/lndb/test/_migrations_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from subprocess import run
 from typing import Optional
 
 from lamin_logger import logger
+from laminci.db import setup_local_test_sqlite_file
 from lnhub_rest._assets import instances as test_instances
 from lnhub_rest.core.instance._init_instance import validate_db_arg, validate_schema_arg
 from lnhub_rest.core.storage._add_storage import validate_storage_root_arg
 
 from lndb._init_instance import infer_instance_name, init
 from lndb._settings import settings
-from lndb.dev import setup_local_test_sqlite_file
 from lndb.dev._clone import clone_test
 from lndb.dev._settings_instance import InstanceSettings
 
 # from ._migrations_unit import model_definitions_match_ddl
 
 
 def migrate_clones(
```

### Comparing `lndb-0.45a2/lndb/test/_migrations_unit.py` & `lndb-0.45a3/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/noxfile.py` & `lndb-0.45a3/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/pyproject.toml` & `lndb-0.45a3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.9.4",
+    "lnhub_rest==0.9.7",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.34a2",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
-    "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
     "sqlmodel>=0.0.8",
     "psycopg2-binary",
     "appdirs",
     "python-dotenv",
     "erdiagram",
     "alembic",
     "natsort",
@@ -36,15 +35,15 @@
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
-    "lamindb[bionty,lamin1]>=0.41a1",
+    "lnschema_lamin1",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject-test>=0.4.3",
     "nbproject",
 ]
 
 [project.scripts]
```

### Comparing `lndb-0.45a2/tests/test_bionty.py` & `lndb-0.45a3/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/tests/test_init_instance.py` & `lndb-0.45a3/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.45a2/PKG-INFO` & `lndb-0.45a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.45a2
+Version: 0.45a3
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.9.4
+Requires-Dist: lnhub_rest==0.9.7
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.34a2
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
-Requires-Dist: cloudpathlib
 Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
 Requires-Dist: appdirs
 Requires-Dist: python-dotenv
 Requires-Dist: erdiagram
 Requires-Dist: alembic
 Requires-Dist: natsort
 Requires-Dist: pandas
 Requires-Dist: python-dateutil
 Requires-Dist: universal_pathlib
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
-Requires-Dist: lamindb[bionty,lamin1]>=0.41a1 ; extra == "test"
+Requires-Dist: lnschema_lamin1 ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject-test>=0.4.3 ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb
 Provides-Extra: dev
 Provides-Extra: test
```

