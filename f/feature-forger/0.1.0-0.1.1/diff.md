# Comparing `tmp/feature_forger-0.1.0.tar.gz` & `tmp/feature_forger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_forger-0.1.0.tar", max compression
+gzip compressed data, was "feature_forger-0.1.1.tar", max compression
```

## Comparing `feature_forger-0.1.0.tar` & `feature_forger-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0       36 2023-05-28 09:41:07.165600 feature_forger-0.1.0/README.md
--rw-r--r--   0        0        0      184 2023-05-08 14:22:42.702762 feature_forger-0.1.0/feature_forge/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 14:44:16.918515 feature_forger-0.1.0/feature_forge/application/__init__.py
--rw-r--r--   0        0        0      166 2023-05-06 15:00:24.558491 feature_forger-0.1.0/feature_forge/application/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2447 2023-05-28 08:58:43.848518 feature_forger-0.1.0/feature_forge/application/__pycache__/blacksmith.cpython-310.pyc
--rw-r--r--   0        0        0      532 2023-05-06 15:00:24.559130 feature_forger-0.1.0/feature_forge/application/__pycache__/container.cpython-310.pyc
--rw-r--r--   0        0        0     2049 2023-05-28 08:58:43.093540 feature_forger-0.1.0/feature_forge/application/blacksmith.py
--rw-r--r--   0        0        0      231 2023-05-06 14:53:12.425390 feature_forger-0.1.0/feature_forge/application/container.py
--rw-r--r--   0        0        0        0 2023-05-08 14:11:53.498473 feature_forger-0.1.0/feature_forge/application/models/__init__.py
--rw-r--r--   0        0        0      173 2023-05-08 14:22:53.451248 feature_forger-0.1.0/feature_forge/application/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1922 2023-05-15 22:26:37.952904 feature_forger-0.1.0/feature_forge/application/models/__pycache__/recipe.cpython-310.pyc
--rw-r--r--   0        0        0      984 2023-05-15 22:26:36.152657 feature_forger-0.1.0/feature_forge/application/models/recipe.py
--rw-r--r--   0        0        0        0 2023-05-06 14:46:44.015607 feature_forger-0.1.0/feature_forge/domain/__init__.py
--rw-r--r--   0        0        0      161 2023-05-06 15:00:24.667962 feature_forger-0.1.0/feature_forge/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2647 2023-05-15 08:10:32.606009 feature_forger-0.1.0/feature_forge/domain/__pycache__/composite_task.cpython-310.pyc
--rw-r--r--   0        0        0      944 2023-05-28 08:47:04.508653 feature_forger-0.1.0/feature_forge/domain/__pycache__/container.cpython-310.pyc
--rw-r--r--   0        0        0     3495 2023-05-15 22:36:37.048916 feature_forger-0.1.0/feature_forge/domain/__pycache__/dag_builder.cpython-310.pyc
--rw-r--r--   0        0        0     1087 2023-05-06 20:34:20.913720 feature_forger-0.1.0/feature_forge/domain/__pycache__/dataset_model_builder.cpython-310.pyc
--rw-r--r--   0        0        0     1442 2023-05-28 09:28:14.698710 feature_forger-0.1.0/feature_forge/domain/__pycache__/feature_validator.cpython-310.pyc
--rw-r--r--   0        0        0     9808 2023-05-28 10:14:58.975100 feature_forger-0.1.0/feature_forge/domain/__pycache__/pipeline_builder.cpython-310.pyc
--rw-r--r--   0        0        0      746 2023-05-15 22:36:39.287566 feature_forger-0.1.0/feature_forge/domain/__pycache__/pipeline_runner.cpython-310.pyc
--rw-r--r--   0        0        0     1379 2023-05-15 08:10:30.306684 feature_forger-0.1.0/feature_forge/domain/composite_task.py
--rw-r--r--   0        0        0      717 2023-05-16 10:08:08.241876 feature_forger-0.1.0/feature_forge/domain/container.py
--rw-r--r--   0        0        0     3446 2023-05-15 22:36:32.600961 feature_forger-0.1.0/feature_forge/domain/dag_builder.py
--rw-r--r--   0        0        0      383 2023-05-06 20:28:55.286923 feature_forger-0.1.0/feature_forge/domain/dataset_model_builder.py
--rw-r--r--   0        0        0        0 2023-05-06 20:38:54.076868 feature_forger-0.1.0/feature_forge/domain/datasets/__init__.py
--rw-r--r--   0        0        0      170 2023-05-06 21:39:00.674650 feature_forger-0.1.0/feature_forge/domain/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1052 2023-05-14 22:26:19.549545 feature_forger-0.1.0/feature_forge/domain/datasets/__pycache__/bank.cpython-310.pyc
--rw-r--r--   0        0        0      657 2023-05-14 22:26:17.403782 feature_forger-0.1.0/feature_forge/domain/datasets/bank.py
--rw-r--r--   0        0        0        0 2023-05-06 14:46:51.020635 feature_forger-0.1.0/feature_forge/domain/entities/__init__.py
--rw-r--r--   0        0        0      170 2023-05-06 15:03:15.967190 feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      948 2023-05-28 09:21:12.252157 feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0        0        0     1150 2023-05-28 09:26:56.898679 feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/entity_model.cpython-310.pyc
--rw-r--r--   0        0        0     1800 2023-05-28 10:18:23.127374 feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/feature.cpython-310.pyc
--rw-r--r--   0        0        0      867 2023-05-16 09:02:20.028928 feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/pipeline.cpython-310.pyc
--rw-r--r--   0        0        0      466 2023-05-28 09:21:11.498845 feature_forger-0.1.0/feature_forge/domain/entities/dataset.py
--rw-r--r--   0        0        0      466 2023-05-28 09:26:56.100433 feature_forger-0.1.0/feature_forge/domain/entities/entity_model.py
--rw-r--r--   0        0        0     1173 2023-05-28 10:18:22.204108 feature_forger-0.1.0/feature_forge/domain/entities/feature.py
--rw-r--r--   0        0        0      448 2023-05-16 08:34:03.665828 feature_forger-0.1.0/feature_forge/domain/entities/pipeline.py
--rw-r--r--   0        0        0        0 2023-05-06 15:13:09.178992 feature_forger-0.1.0/feature_forge/domain/entity_models/__init__.py
--rw-r--r--   0        0        0      170 2023-05-06 15:45:52.277290 feature_forger-0.1.0/feature_forge/domain/entity_models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      454 2023-05-06 22:25:35.699458 feature_forger-0.1.0/feature_forge/domain/entity_models/__pycache__/account.cpython-310.pyc
--rw-r--r--   0        0        0      939 2023-05-06 23:27:01.177121 feature_forger-0.1.0/feature_forge/domain/entity_models/__pycache__/transaction.cpython-310.pyc
--rw-r--r--   0        0        0      117 2023-05-06 21:22:05.015001 feature_forger-0.1.0/feature_forge/domain/entity_models/account.py
--rw-r--r--   0        0        0      573 2023-05-06 23:27:00.089582 feature_forger-0.1.0/feature_forge/domain/entity_models/transaction.py
--rw-r--r--   0        0        0     1045 2023-05-28 09:28:14.029330 feature_forger-0.1.0/feature_forge/domain/feature_validator.py
--rw-r--r--   0        0        0      636 2023-05-08 14:22:42.700026 feature_forger-0.1.0/feature_forge/domain/features/__init__.py
--rw-r--r--   0        0        0      717 2023-05-08 14:22:53.702483 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1589 2023-05-28 09:07:55.252110 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc
--rw-r--r--   0        0        0     1543 2023-05-28 09:25:17.438330 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc
--rw-r--r--   0        0        0     1837 2023-05-28 09:15:19.332966 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc
--rw-r--r--   0        0        0     1683 2023-05-28 09:08:32.733441 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc
--rw-r--r--   0        0        0     1490 2023-05-28 10:19:09.730833 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_month.cpython-310.pyc
--rw-r--r--   0        0        0     1673 2023-05-28 09:35:59.222751 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc
--rw-r--r--   0        0        0     1459 2023-05-28 09:08:56.703063 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc
--rw-r--r--   0        0        0     1618 2023-05-28 09:36:31.151403 feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc
--rw-r--r--   0        0        0     1012 2023-05-28 09:07:51.336484 feature_forger-0.1.0/feature_forge/domain/features/halved_rounded_amount_change.py
--rw-r--r--   0        0        0      972 2023-05-28 09:25:15.355280 feature_forger-0.1.0/feature_forge/domain/features/rounded_amount_change.py
--rw-r--r--   0        0        0     1338 2023-05-28 09:15:16.807948 feature_forger-0.1.0/feature_forge/domain/features/rounded_amount_change_difference.py
--rw-r--r--   0        0        0     1295 2023-05-28 09:08:28.499769 feature_forger-0.1.0/feature_forge/domain/features/transaction_amount_change.py
--rw-r--r--   0        0        0      901 2023-05-28 10:19:07.738992 feature_forger-0.1.0/feature_forge/domain/features/transaction_month.py
--rw-r--r--   0        0        0     1131 2023-05-28 09:35:57.111622 feature_forger-0.1.0/feature_forge/domain/features/transaction_rounded_amount_change_diff_doubled.py
--rw-r--r--   0        0        0      972 2023-05-28 09:08:53.141760 feature_forger-0.1.0/feature_forge/domain/features/transaction_rounded_amount_change_diff_squared.py
--rw-r--r--   0        0        0     1084 2023-05-28 09:36:28.481178 feature_forger-0.1.0/feature_forge/domain/features/transaction_rounded_amount_change_doubled.py
--rw-r--r--   0        0        0     8760 2023-05-28 10:14:57.856934 feature_forger-0.1.0/feature_forge/domain/pipeline_builder.py
--rw-r--r--   0        0        0      400 2023-05-15 22:36:32.590178 feature_forger-0.1.0/feature_forge/domain/pipeline_runner.py
--rw-r--r--   0        0        0      622 2023-05-28 10:26:37.594555 feature_forger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 feature_forger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-05-28 10:27:09.265284 feature_forger-0.1.1/README.md
+-rw-r--r--   0        0        0      184 2023-05-08 14:22:42.702762 feature_forger-0.1.1/feature_forger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:44:16.918515 feature_forger-0.1.1/feature_forger/application/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-06 15:00:24.558491 feature_forger-0.1.1/feature_forger/application/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2447 2023-05-28 08:58:43.848518 feature_forger-0.1.1/feature_forger/application/__pycache__/blacksmith.cpython-310.pyc
+-rw-r--r--   0        0        0      532 2023-05-06 15:00:24.559130 feature_forger-0.1.1/feature_forger/application/__pycache__/container.cpython-310.pyc
+-rw-r--r--   0        0        0     2056 2023-05-28 10:27:09.258157 feature_forger-0.1.1/feature_forger/application/blacksmith.py
+-rw-r--r--   0        0        0      232 2023-05-28 10:27:09.283986 feature_forger-0.1.1/feature_forger/application/container.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:11:53.498473 feature_forger-0.1.1/feature_forger/application/models/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-08 14:22:53.451248 feature_forger-0.1.1/feature_forger/application/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1922 2023-05-15 22:26:37.952904 feature_forger-0.1.1/feature_forger/application/models/__pycache__/recipe.cpython-310.pyc
+-rw-r--r--   0        0        0      986 2023-05-28 10:27:09.272373 feature_forger-0.1.1/feature_forger/application/models/recipe.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:46:44.015607 feature_forger-0.1.1/feature_forger/domain/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-06 15:00:24.667962 feature_forger-0.1.1/feature_forger/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2647 2023-05-15 08:10:32.606009 feature_forger-0.1.1/feature_forger/domain/__pycache__/composite_task.cpython-310.pyc
+-rw-r--r--   0        0        0      944 2023-05-28 08:47:04.508653 feature_forger-0.1.1/feature_forger/domain/__pycache__/container.cpython-310.pyc
+-rw-r--r--   0        0        0     3495 2023-05-15 22:36:37.048916 feature_forger-0.1.1/feature_forger/domain/__pycache__/dag_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     1087 2023-05-06 20:34:20.913720 feature_forger-0.1.1/feature_forger/domain/__pycache__/dataset_model_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     1442 2023-05-28 09:28:14.698710 feature_forger-0.1.1/feature_forger/domain/__pycache__/feature_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     9808 2023-05-28 10:14:58.975100 feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_builder.cpython-310.pyc
+-rw-r--r--   0        0        0      746 2023-05-15 22:36:39.287566 feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_runner.cpython-310.pyc
+-rw-r--r--   0        0        0     1380 2023-05-28 10:27:09.271165 feature_forger-0.1.1/feature_forger/domain/composite_task.py
+-rw-r--r--   0        0        0      722 2023-05-28 10:27:09.269670 feature_forger-0.1.1/feature_forger/domain/container.py
+-rw-r--r--   0        0        0     3448 2023-05-28 10:27:09.292544 feature_forger-0.1.1/feature_forger/domain/dag_builder.py
+-rw-r--r--   0        0        0      384 2023-05-28 10:27:09.313904 feature_forger-0.1.1/feature_forger/domain/dataset_model_builder.py
+-rw-r--r--   0        0        0        0 2023-05-06 20:38:54.076868 feature_forger-0.1.1/feature_forger/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-06 21:39:00.674650 feature_forger-0.1.1/feature_forger/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1052 2023-05-14 22:26:19.549545 feature_forger-0.1.1/feature_forger/domain/datasets/__pycache__/bank.cpython-310.pyc
+-rw-r--r--   0        0        0      661 2023-05-28 10:27:09.295618 feature_forger-0.1.1/feature_forger/domain/datasets/bank.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:46:51.020635 feature_forger-0.1.1/feature_forger/domain/entities/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-06 15:03:15.967190 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2023-05-28 09:21:12.252157 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     1150 2023-05-28 09:26:56.898679 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/entity_model.cpython-310.pyc
+-rw-r--r--   0        0        0     1800 2023-05-28 10:18:23.127374 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/feature.cpython-310.pyc
+-rw-r--r--   0        0        0      867 2023-05-16 09:02:20.028928 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/pipeline.cpython-310.pyc
+-rw-r--r--   0        0        0      467 2023-05-28 10:27:09.278297 feature_forger-0.1.1/feature_forger/domain/entities/dataset.py
+-rw-r--r--   0        0        0      466 2023-05-28 09:26:56.100433 feature_forger-0.1.1/feature_forger/domain/entities/entity_model.py
+-rw-r--r--   0        0        0     1174 2023-05-28 10:27:09.276091 feature_forger-0.1.1/feature_forger/domain/entities/feature.py
+-rw-r--r--   0        0        0      450 2023-05-28 10:27:09.290717 feature_forger-0.1.1/feature_forger/domain/entities/pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-06 15:13:09.178992 feature_forger-0.1.1/feature_forger/domain/entity_models/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-06 15:45:52.277290 feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      454 2023-05-06 22:25:35.699458 feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/account.cpython-310.pyc
+-rw-r--r--   0        0        0      939 2023-05-06 23:27:01.177121 feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/transaction.cpython-310.pyc
+-rw-r--r--   0        0        0      118 2023-05-28 10:27:09.282211 feature_forger-0.1.1/feature_forger/domain/entity_models/account.py
+-rw-r--r--   0        0        0      574 2023-05-28 10:27:09.268313 feature_forger-0.1.1/feature_forger/domain/entity_models/transaction.py
+-rw-r--r--   0        0        0     1046 2023-05-28 10:27:09.274969 feature_forger-0.1.1/feature_forger/domain/feature_validator.py
+-rw-r--r--   0        0        0      636 2023-05-08 14:22:42.700026 feature_forger-0.1.1/feature_forger/domain/features/__init__.py
+-rw-r--r--   0        0        0      717 2023-05-08 14:22:53.702483 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1589 2023-05-28 09:07:55.252110 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc
+-rw-r--r--   0        0        0     1543 2023-05-28 09:25:17.438330 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc
+-rw-r--r--   0        0        0     1837 2023-05-28 09:15:19.332966 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc
+-rw-r--r--   0        0        0     1683 2023-05-28 09:08:32.733441 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc
+-rw-r--r--   0        0        0     1490 2023-05-28 10:19:09.730833 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_month.cpython-310.pyc
+-rw-r--r--   0        0        0     1673 2023-05-28 09:35:59.222751 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc
+-rw-r--r--   0        0        0     1459 2023-05-28 09:08:56.703063 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc
+-rw-r--r--   0        0        0     1618 2023-05-28 09:36:31.151403 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc
+-rw-r--r--   0        0        0     1016 2023-05-28 10:27:09.263768 feature_forger-0.1.1/feature_forger/domain/features/halved_rounded_amount_change.py
+-rw-r--r--   0        0        0      976 2023-05-28 10:27:09.285112 feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change.py
+-rw-r--r--   0        0        0     1344 2023-05-28 10:27:09.266603 feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change_difference.py
+-rw-r--r--   0        0        0     1298 2023-05-28 10:27:09.277112 feature_forger-0.1.1/feature_forger/domain/features/transaction_amount_change.py
+-rw-r--r--   0        0        0      904 2023-05-28 10:27:09.273579 feature_forger-0.1.1/feature_forger/domain/features/transaction_month.py
+-rw-r--r--   0        0        0     1135 2023-05-28 10:27:09.262462 feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_doubled.py
+-rw-r--r--   0        0        0      976 2023-05-28 10:27:09.280725 feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_squared.py
+-rw-r--r--   0        0        0     1088 2023-05-28 10:27:09.288165 feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_doubled.py
+-rw-r--r--   0        0        0     8767 2023-05-28 10:27:09.260919 feature_forger-0.1.1/feature_forger/domain/pipeline_builder.py
+-rw-r--r--   0        0        0      401 2023-05-28 10:27:09.279433 feature_forger-0.1.1/feature_forger/domain/pipeline_runner.py
+-rw-r--r--   0        0        0      623 2023-05-28 10:27:34.075962 feature_forger-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 feature_forger-0.1.1/PKG-INFO
```

### Comparing `feature_forger-0.1.0/feature_forge/application/__pycache__/blacksmith.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/application/__pycache__/blacksmith.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/application/__pycache__/container.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/application/__pycache__/container.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/application/blacksmith.py` & `feature_forger-0.1.1/feature_forger/application/blacksmith.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from functools import cached_property
 from typing import List, Type
 
 import pandas as pd
 
-from feature_forge.application.container import Container
-from feature_forge.domain.entities.dataset import Dataset
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entities.pipeline import Pipeline
-from feature_forge.domain.pipeline_builder import PipelineBuilder
-from feature_forge.domain.pipeline_runner import PipelineRunner
-from feature_forge.application.models.recipe import Recipe
+from feature_forger.application.container import Container
+from feature_forger.domain.entities.dataset import Dataset
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entities.pipeline import Pipeline
+from feature_forger.domain.pipeline_builder import PipelineBuilder
+from feature_forger.domain.pipeline_runner import PipelineRunner
+from feature_forger.application.models.recipe import Recipe
 
 
 class Blacksmith:
 
     def __init__(self):
         self._container = Container()
         self._container.wire([__name__])
```

### Comparing `feature_forger-0.1.0/feature_forge/application/models/__pycache__/recipe.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/application/models/__pycache__/recipe.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/application/models/recipe.py` & `feature_forger-0.1.1/feature_forger/application/models/recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pandas as pd
 from PIL import Image
 from networkx import DiGraph
 from prefect import Flow
 from pydantic import BaseModel
 from pydot import Dot
 
-from feature_forge.domain.entities.dataset import Dataset
-from feature_forge.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.dataset import Dataset
+from feature_forger.domain.entities.entity_model import EntityModel
 
 
 class Recipe(BaseModel):
     dataset: Dataset
     entity: Type[EntityModel]
     flow: Callable[[pd.DataFrame], pd.DataFrame]
     graph: Dot
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/__pycache__/composite_task.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/__pycache__/composite_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/__pycache__/container.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/__pycache__/container.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/__pycache__/dag_builder.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/__pycache__/dag_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/__pycache__/dataset_model_builder.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/__pycache__/dataset_model_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/__pycache__/feature_validator.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/__pycache__/feature_validator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/__pycache__/pipeline_builder.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/__pycache__/pipeline_runner.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_runner.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/composite_task.py` & `feature_forger-0.1.1/feature_forger/domain/composite_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from functools import reduce, cached_property
 from typing import List, Callable, Union
 
 import pandas as pd
 from prefect import task
 
-from feature_forge.domain.entities.feature import Feature
+from feature_forger.domain.entities.feature import Feature
 
 
 @dataclass
 class CompositeTask:
     type: str
     funcs: List[Union[Feature.row_compute_fn, Feature.table_compute_fn]]
     features: List[str]
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/container.py` & `feature_forger-0.1.1/feature_forger/domain/container.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dependency_injector import containers, providers
 
-from feature_forge.domain.dag_builder import DAGBuilder
-from feature_forge.domain.dataset_model_builder import DatasetModelBuilder
-from feature_forge.domain.feature_validator import FeatureValidator
-from feature_forge.domain.pipeline_builder import PipelineBuilder
-from feature_forge.domain.pipeline_runner import PipelineRunner
+from feature_forger.domain.dag_builder import DAGBuilder
+from feature_forger.domain.dataset_model_builder import DatasetModelBuilder
+from feature_forger.domain.feature_validator import FeatureValidator
+from feature_forger.domain.pipeline_builder import PipelineBuilder
+from feature_forger.domain.pipeline_runner import PipelineRunner
 
 
 class DomainContainer(containers.DeclarativeContainer):
 
     pipeline_builder = providers.Factory(
         PipelineBuilder,
         providers.Factory(DatasetModelBuilder),
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/dag_builder.py` & `feature_forger-0.1.1/feature_forger/domain/dag_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import itertools
 from typing import List, Type, Dict
 
 import networkx as nx
 from networkx import DiGraph
 from pydot import Dot
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
 
 
 class DAGBuilder:
 
     def build_simple_graph(self,
                            features: List[Feature],
                            entity: Type[EntityModel]):
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/datasets/__pycache__/bank.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/datasets/__pycache__/bank.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/datasets/bank.py` & `feature_forger-0.1.1/feature_forger/domain/datasets/bank.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Type, ClassVar
 
-from feature_forge.domain.entities.dataset import Dataset
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entity_models.account import Account
-from feature_forge.domain.entity_models.transaction import \
+from feature_forger.domain.entities.dataset import Dataset
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entity_models.account import Account
+from feature_forger.domain.entity_models.transaction import \
     Transaction
 
 
 @dataclass(frozen=True)
 class BankDataset(Dataset):
     supported_entity_models = (Transaction, Account)
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/dataset.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/entity_model.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/entity_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/feature.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/feature.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/entities/__pycache__/pipeline.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/pipeline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/entities/feature.py` & `feature_forger-0.1.1/feature_forger/domain/entities/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Type, Tuple, runtime_checkable, Protocol, Optional, Callable
 
 import pandas as pd
 from pydantic.dataclasses import dataclass
 
-from feature_forge.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.entity_model import EntityModel
 
 
 class FeatureMeta(type):
     def __repr__(cls):
         return f'{cls.__name__}'
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/entity_models/__pycache__/transaction.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/transaction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/entity_models/transaction.py` & `feature_forger-0.1.1/feature_forger/domain/entity_models/transaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 
 from pydantic import Field
 
-from feature_forge.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.entity_model import EntityModel
 
 
 class Transaction(EntityModel):
     account_no: str = Field(alias="Account No")
     date: datetime = Field(alias="DATE")
     trn_details: str = Field(alias="TRANSACTION DETAILS")
     chq_no: float = Field(alias="CHQ.NO.")
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/feature_validator.py` & `feature_forger-0.1.1/feature_forger/domain/feature_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import wraps
 from typing import Union
 
 import pandas as pd
 
-from feature_forge.domain.entities.feature import Feature
+from feature_forger.domain.entities.feature import Feature
 
 
 class FeatureValidator:
 
     def add_runtime_validation(self, compute_fn: Union[Feature.row_compute_fn,
                              Feature.table_compute_fn]):
         return self._validate_feature_compute_fn(compute_fn)
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__init__.py` & `feature_forger-0.1.1/feature_forger/domain/features/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/__init__.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_month.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_month.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc` & `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/halved_rounded_amount_change.py` & `feature_forger-0.1.1/feature_forger/domain/features/halved_rounded_amount_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from typing import Type, Tuple
 
 import pandas as pd
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import Transaction
-from feature_forge.domain.features.rounded_amount_change import \
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import Transaction
+from feature_forger.domain.features.rounded_amount_change import \
     TransactionRoundedAmountChange
 
 
 @dataclass(frozen=True)
 class TransactionHalfRoundedAmountChange(Feature):
     col_name: str = "transaction_half_rounded_amount_change"
     description: str = "half of the rounded difference between the withdrawal" \
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/rounded_amount_change.py` & `feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from typing import Type, Tuple
 
 import pandas as pd
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import Transaction
-from feature_forge.domain.features.transaction_amount_change import \
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import Transaction
+from feature_forger.domain.features.transaction_amount_change import \
     TransactionAmountChange
 
 
 @dataclass(frozen=True)
 class TransactionRoundedAmountChange(Feature):
     col_name: str = "transaction_rounded_amount_change"
     description: str = "rounded difference between withdrawal amount and desposit " \
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/rounded_amount_change_difference.py` & `feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change_difference.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from dataclasses import dataclass
 from typing import Type, Tuple
 
 import pandas as pd
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import Transaction
-from feature_forge.domain.features.transaction_month import TransactionMonth
-from feature_forge.domain.features.rounded_amount_change import \
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import Transaction
+from feature_forger.domain.features.transaction_month import TransactionMonth
+from feature_forger.domain.features.rounded_amount_change import \
     TransactionRoundedAmountChange
-from feature_forge.domain.features.transaction_amount_change import \
+from feature_forger.domain.features.transaction_amount_change import \
     TransactionAmountChange
 
 @dataclass(frozen=True)
 class TransactionRoundedAmountChangeDiff(Feature):
     col_name: str = "transaction_rounded_amount_change_diff"
     description: str = "difference of the rounded difference between the withdrawal" \
                   " amount and the deposit amount"
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/transaction_amount_change.py` & `feature_forger-0.1.1/feature_forger/domain/features/transaction_amount_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from typing import Type, Tuple
 
 import numpy as np
 import pandas as pd
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import \
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import \
     Transaction
 
 
 @dataclass(frozen=True)
 class TransactionAmountChange(Feature):
     col_name: str = "transaction_amount_change"
     description: str = "difference between witdrawal amount and deposit amount"
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/transaction_month.py` & `feature_forger-0.1.1/feature_forger/domain/features/transaction_month.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Type, Tuple, Optional
 
 import pandas as pd
 from pydantic import Field
 from pydantic.dataclasses import dataclass
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import \
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import \
     Transaction
 
 
 @dataclass(frozen=True)
 class TransactionMonth(Feature):
     col_name: str = "value_month"
     description: str = "month of the value date for the transaction"
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/transaction_rounded_amount_change_diff_doubled.py` & `feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_squared.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from dataclasses import dataclass
 from typing import Type, Tuple
 
 import pandas as pd
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import Transaction
-from feature_forge.domain.features.rounded_amount_change_difference import \
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import Transaction
+from feature_forger.domain.features.rounded_amount_change_difference import \
     TransactionRoundedAmountChangeDiff
 
 
 @dataclass(frozen=True)
-class TransactionRoundedAmountChangeDiffDoubled(Feature):
-    col_name: str = "transaction_rounded_amount_change_diff_doubled"
-    description: str = "difference of the rounded difference between the " \
-                       "withdrawal" \
-                       " amount and the deposit amount doubled"
+class TransactionRoundedAmountChangeDiffSquared(Feature):
+    col_name: str = "transaction_rounded_amount_change_diff_squared"
+    description: str = "difference of the rounded difference between the withdrawal" \
+                  " amount and the deposit amount squared"
     entity_model: Type[EntityModel] = Transaction
     dependencies: Tuple[Feature] = (TransactionRoundedAmountChangeDiff(),)
 
     def row_compute_fn(self, row: pd.Series):
-        row[self.col_name] = row[
-                                TransactionRoundedAmountChangeDiff.col_name] * 2
+        row[self.col_name] = row[TransactionRoundedAmountChangeDiff.col_name] ** 2
         return row
-
-    def table_compute_fn(self, data: pd.DataFrame):
-        return self.row_compute_fn(data)
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/transaction_rounded_amount_change_diff_squared.py` & `feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_doubled.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from dataclasses import dataclass
 from typing import Type, Tuple
 
 import pandas as pd
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import Transaction
-from feature_forge.domain.features.rounded_amount_change_difference import \
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import Transaction
+from feature_forger.domain.features.rounded_amount_change_difference import \
     TransactionRoundedAmountChangeDiff
 
 
 @dataclass(frozen=True)
-class TransactionRoundedAmountChangeDiffSquared(Feature):
-    col_name: str = "transaction_rounded_amount_change_diff_squared"
-    description: str = "difference of the rounded difference between the withdrawal" \
-                  " amount and the deposit amount squared"
+class TransactionRoundedAmountChangeDiffDoubled(Feature):
+    col_name: str = "transaction_rounded_amount_change_diff_doubled"
+    description: str = "difference of the rounded difference between the " \
+                       "withdrawal" \
+                       " amount and the deposit amount doubled"
     entity_model: Type[EntityModel] = Transaction
     dependencies: Tuple[Feature] = (TransactionRoundedAmountChangeDiff(),)
 
     def row_compute_fn(self, row: pd.Series):
-        row[self.col_name] = row[TransactionRoundedAmountChangeDiff.col_name] ** 2
+        row[self.col_name] = row[
+                                TransactionRoundedAmountChangeDiff.col_name] * 2
         return row
+
+    def table_compute_fn(self, data: pd.DataFrame):
+        return self.row_compute_fn(data)
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/features/transaction_rounded_amount_change_doubled.py` & `feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_doubled.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from typing import Type, Tuple
 
 import pandas as pd
 
-from feature_forge.domain.entities.entity_model import EntityModel
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entity_models.transaction import Transaction
-from feature_forge.domain.features import TransactionHalfRoundedAmountChange
+from feature_forger.domain.entities.entity_model import EntityModel
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entity_models.transaction import Transaction
+from feature_forger.domain.features import TransactionHalfRoundedAmountChange
 
 
 @dataclass(frozen=True)
 class TransactionRoundedAmountChangeDoubled(Feature):
     col_name: str = "transaction_rounded_amount_change_doubled"
     description: str = "difference of the rounded difference between the " \
                        "withdrawal" \
```

### Comparing `feature_forger-0.1.0/feature_forge/domain/pipeline_builder.py` & `feature_forger-0.1.1/feature_forger/domain/pipeline_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from itertools import groupby
 from typing import List, Tuple, Union
 
 import networkx as nx
 import pandas as pd
 from prefect import flow, task
 
-from feature_forge.domain.composite_task import CompositeTask
-from feature_forge.domain.dag_builder import DAGBuilder
-from feature_forge.domain.dataset_model_builder import DatasetModelBuilder
-from feature_forge.domain.entities.dataset import Dataset
-from feature_forge.domain.entities.feature import Feature
-from feature_forge.domain.entities.pipeline import Pipeline
-from feature_forge.domain.feature_validator import FeatureValidator
+from feature_forger.domain.composite_task import CompositeTask
+from feature_forger.domain.dag_builder import DAGBuilder
+from feature_forger.domain.dataset_model_builder import DatasetModelBuilder
+from feature_forger.domain.entities.dataset import Dataset
+from feature_forger.domain.entities.feature import Feature
+from feature_forger.domain.entities.pipeline import Pipeline
+from feature_forger.domain.feature_validator import FeatureValidator
 
 
 class PipelineBuilder:
 
     def __init__(self,
                  dataset_model_builder: DatasetModelBuilder,
                  dag_builder: DAGBuilder,
```

### Comparing `feature_forger-0.1.0/pyproject.toml` & `feature_forger-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "feature-forger"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["iccyp <shingle.knitter.0i@icloud.com>"]
 readme = "README.md"
-packages = [{include = "feature_forge"}]
+packages = [{include = "feature_forger"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 prefect = "^2.10.7"
 pandas = "^2.0.1"
 dependency-injector = "^4.41.0"
 openpyxl = "^3.1.2"
```

### Comparing `feature_forger-0.1.0/PKG-INFO` & `feature_forger-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-forger
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: iccyp
 Author-email: shingle.knitter.0i@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,11 +18,11 @@
 Requires-Dist: pandera (>=0.14.5,<0.15.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: prefect (>=2.10.7,<3.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pydot (>=1.4.2,<2.0.0)
 Description-Content-Type: text/markdown
 
-feature-forge
+feature-forger
 ---
 
 Page coming soon!
```

