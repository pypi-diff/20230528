# Comparing `tmp/feature_forger-0.1.1.tar.gz` & `tmp/feature_forger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_forger-0.1.1.tar", max compression
+gzip compressed data, was "feature_forger-0.1.2.tar", max compression
```

## Comparing `feature_forger-0.1.1.tar` & `feature_forger-0.1.2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0       37 2023-05-28 10:27:09.265284 feature_forger-0.1.1/README.md
--rw-r--r--   0        0        0      184 2023-05-08 14:22:42.702762 feature_forger-0.1.1/feature_forger/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 14:44:16.918515 feature_forger-0.1.1/feature_forger/application/__init__.py
--rw-r--r--   0        0        0      166 2023-05-06 15:00:24.558491 feature_forger-0.1.1/feature_forger/application/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2447 2023-05-28 08:58:43.848518 feature_forger-0.1.1/feature_forger/application/__pycache__/blacksmith.cpython-310.pyc
--rw-r--r--   0        0        0      532 2023-05-06 15:00:24.559130 feature_forger-0.1.1/feature_forger/application/__pycache__/container.cpython-310.pyc
--rw-r--r--   0        0        0     2056 2023-05-28 10:27:09.258157 feature_forger-0.1.1/feature_forger/application/blacksmith.py
--rw-r--r--   0        0        0      232 2023-05-28 10:27:09.283986 feature_forger-0.1.1/feature_forger/application/container.py
--rw-r--r--   0        0        0        0 2023-05-08 14:11:53.498473 feature_forger-0.1.1/feature_forger/application/models/__init__.py
--rw-r--r--   0        0        0      173 2023-05-08 14:22:53.451248 feature_forger-0.1.1/feature_forger/application/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1922 2023-05-15 22:26:37.952904 feature_forger-0.1.1/feature_forger/application/models/__pycache__/recipe.cpython-310.pyc
--rw-r--r--   0        0        0      986 2023-05-28 10:27:09.272373 feature_forger-0.1.1/feature_forger/application/models/recipe.py
--rw-r--r--   0        0        0        0 2023-05-06 14:46:44.015607 feature_forger-0.1.1/feature_forger/domain/__init__.py
--rw-r--r--   0        0        0      161 2023-05-06 15:00:24.667962 feature_forger-0.1.1/feature_forger/domain/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2647 2023-05-15 08:10:32.606009 feature_forger-0.1.1/feature_forger/domain/__pycache__/composite_task.cpython-310.pyc
--rw-r--r--   0        0        0      944 2023-05-28 08:47:04.508653 feature_forger-0.1.1/feature_forger/domain/__pycache__/container.cpython-310.pyc
--rw-r--r--   0        0        0     3495 2023-05-15 22:36:37.048916 feature_forger-0.1.1/feature_forger/domain/__pycache__/dag_builder.cpython-310.pyc
--rw-r--r--   0        0        0     1087 2023-05-06 20:34:20.913720 feature_forger-0.1.1/feature_forger/domain/__pycache__/dataset_model_builder.cpython-310.pyc
--rw-r--r--   0        0        0     1442 2023-05-28 09:28:14.698710 feature_forger-0.1.1/feature_forger/domain/__pycache__/feature_validator.cpython-310.pyc
--rw-r--r--   0        0        0     9808 2023-05-28 10:14:58.975100 feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_builder.cpython-310.pyc
--rw-r--r--   0        0        0      746 2023-05-15 22:36:39.287566 feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_runner.cpython-310.pyc
--rw-r--r--   0        0        0     1380 2023-05-28 10:27:09.271165 feature_forger-0.1.1/feature_forger/domain/composite_task.py
--rw-r--r--   0        0        0      722 2023-05-28 10:27:09.269670 feature_forger-0.1.1/feature_forger/domain/container.py
--rw-r--r--   0        0        0     3448 2023-05-28 10:27:09.292544 feature_forger-0.1.1/feature_forger/domain/dag_builder.py
--rw-r--r--   0        0        0      384 2023-05-28 10:27:09.313904 feature_forger-0.1.1/feature_forger/domain/dataset_model_builder.py
--rw-r--r--   0        0        0        0 2023-05-06 20:38:54.076868 feature_forger-0.1.1/feature_forger/domain/datasets/__init__.py
--rw-r--r--   0        0        0      170 2023-05-06 21:39:00.674650 feature_forger-0.1.1/feature_forger/domain/datasets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1052 2023-05-14 22:26:19.549545 feature_forger-0.1.1/feature_forger/domain/datasets/__pycache__/bank.cpython-310.pyc
--rw-r--r--   0        0        0      661 2023-05-28 10:27:09.295618 feature_forger-0.1.1/feature_forger/domain/datasets/bank.py
--rw-r--r--   0        0        0        0 2023-05-06 14:46:51.020635 feature_forger-0.1.1/feature_forger/domain/entities/__init__.py
--rw-r--r--   0        0        0      170 2023-05-06 15:03:15.967190 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      948 2023-05-28 09:21:12.252157 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/dataset.cpython-310.pyc
--rw-r--r--   0        0        0     1150 2023-05-28 09:26:56.898679 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/entity_model.cpython-310.pyc
--rw-r--r--   0        0        0     1800 2023-05-28 10:18:23.127374 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/feature.cpython-310.pyc
--rw-r--r--   0        0        0      867 2023-05-16 09:02:20.028928 feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/pipeline.cpython-310.pyc
--rw-r--r--   0        0        0      467 2023-05-28 10:27:09.278297 feature_forger-0.1.1/feature_forger/domain/entities/dataset.py
--rw-r--r--   0        0        0      466 2023-05-28 09:26:56.100433 feature_forger-0.1.1/feature_forger/domain/entities/entity_model.py
--rw-r--r--   0        0        0     1174 2023-05-28 10:27:09.276091 feature_forger-0.1.1/feature_forger/domain/entities/feature.py
--rw-r--r--   0        0        0      450 2023-05-28 10:27:09.290717 feature_forger-0.1.1/feature_forger/domain/entities/pipeline.py
--rw-r--r--   0        0        0        0 2023-05-06 15:13:09.178992 feature_forger-0.1.1/feature_forger/domain/entity_models/__init__.py
--rw-r--r--   0        0        0      170 2023-05-06 15:45:52.277290 feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      454 2023-05-06 22:25:35.699458 feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/account.cpython-310.pyc
--rw-r--r--   0        0        0      939 2023-05-06 23:27:01.177121 feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/transaction.cpython-310.pyc
--rw-r--r--   0        0        0      118 2023-05-28 10:27:09.282211 feature_forger-0.1.1/feature_forger/domain/entity_models/account.py
--rw-r--r--   0        0        0      574 2023-05-28 10:27:09.268313 feature_forger-0.1.1/feature_forger/domain/entity_models/transaction.py
--rw-r--r--   0        0        0     1046 2023-05-28 10:27:09.274969 feature_forger-0.1.1/feature_forger/domain/feature_validator.py
--rw-r--r--   0        0        0      636 2023-05-08 14:22:42.700026 feature_forger-0.1.1/feature_forger/domain/features/__init__.py
--rw-r--r--   0        0        0      717 2023-05-08 14:22:53.702483 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1589 2023-05-28 09:07:55.252110 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc
--rw-r--r--   0        0        0     1543 2023-05-28 09:25:17.438330 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc
--rw-r--r--   0        0        0     1837 2023-05-28 09:15:19.332966 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc
--rw-r--r--   0        0        0     1683 2023-05-28 09:08:32.733441 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc
--rw-r--r--   0        0        0     1490 2023-05-28 10:19:09.730833 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_month.cpython-310.pyc
--rw-r--r--   0        0        0     1673 2023-05-28 09:35:59.222751 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc
--rw-r--r--   0        0        0     1459 2023-05-28 09:08:56.703063 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc
--rw-r--r--   0        0        0     1618 2023-05-28 09:36:31.151403 feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc
--rw-r--r--   0        0        0     1016 2023-05-28 10:27:09.263768 feature_forger-0.1.1/feature_forger/domain/features/halved_rounded_amount_change.py
--rw-r--r--   0        0        0      976 2023-05-28 10:27:09.285112 feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change.py
--rw-r--r--   0        0        0     1344 2023-05-28 10:27:09.266603 feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change_difference.py
--rw-r--r--   0        0        0     1298 2023-05-28 10:27:09.277112 feature_forger-0.1.1/feature_forger/domain/features/transaction_amount_change.py
--rw-r--r--   0        0        0      904 2023-05-28 10:27:09.273579 feature_forger-0.1.1/feature_forger/domain/features/transaction_month.py
--rw-r--r--   0        0        0     1135 2023-05-28 10:27:09.262462 feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_doubled.py
--rw-r--r--   0        0        0      976 2023-05-28 10:27:09.280725 feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_squared.py
--rw-r--r--   0        0        0     1088 2023-05-28 10:27:09.288165 feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_doubled.py
--rw-r--r--   0        0        0     8767 2023-05-28 10:27:09.260919 feature_forger-0.1.1/feature_forger/domain/pipeline_builder.py
--rw-r--r--   0        0        0      401 2023-05-28 10:27:09.279433 feature_forger-0.1.1/feature_forger/domain/pipeline_runner.py
--rw-r--r--   0        0        0      623 2023-05-28 10:27:34.075962 feature_forger-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 feature_forger-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2023-05-28 10:27:09.265284 feature_forger-0.1.2/README.md
+-rw-r--r--   0        0        0      184 2023-05-08 14:22:42.702762 feature_forger-0.1.2/feature_forger/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:44:16.918515 feature_forger-0.1.2/feature_forger/application/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-06 15:00:24.558491 feature_forger-0.1.2/feature_forger/application/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2447 2023-05-28 08:58:43.848518 feature_forger-0.1.2/feature_forger/application/__pycache__/blacksmith.cpython-310.pyc
+-rw-r--r--   0        0        0      532 2023-05-06 15:00:24.559130 feature_forger-0.1.2/feature_forger/application/__pycache__/container.cpython-310.pyc
+-rw-r--r--   0        0        0     2056 2023-05-28 10:27:09.258157 feature_forger-0.1.2/feature_forger/application/blacksmith.py
+-rw-r--r--   0        0        0      232 2023-05-28 10:27:09.283986 feature_forger-0.1.2/feature_forger/application/container.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:11:53.498473 feature_forger-0.1.2/feature_forger/application/models/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-08 14:22:53.451248 feature_forger-0.1.2/feature_forger/application/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1922 2023-05-15 22:26:37.952904 feature_forger-0.1.2/feature_forger/application/models/__pycache__/recipe.cpython-310.pyc
+-rw-r--r--   0        0        0      907 2023-05-28 11:16:36.650938 feature_forger-0.1.2/feature_forger/application/models/recipe.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:46:44.015607 feature_forger-0.1.2/feature_forger/domain/__init__.py
+-rw-r--r--   0        0        0      161 2023-05-06 15:00:24.667962 feature_forger-0.1.2/feature_forger/domain/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2647 2023-05-15 08:10:32.606009 feature_forger-0.1.2/feature_forger/domain/__pycache__/composite_task.cpython-310.pyc
+-rw-r--r--   0        0        0      944 2023-05-28 08:47:04.508653 feature_forger-0.1.2/feature_forger/domain/__pycache__/container.cpython-310.pyc
+-rw-r--r--   0        0        0     3495 2023-05-15 22:36:37.048916 feature_forger-0.1.2/feature_forger/domain/__pycache__/dag_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     1087 2023-05-06 20:34:20.913720 feature_forger-0.1.2/feature_forger/domain/__pycache__/dataset_model_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     1442 2023-05-28 09:28:14.698710 feature_forger-0.1.2/feature_forger/domain/__pycache__/feature_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     9808 2023-05-28 10:14:58.975100 feature_forger-0.1.2/feature_forger/domain/__pycache__/pipeline_builder.cpython-310.pyc
+-rw-r--r--   0        0        0      746 2023-05-15 22:36:39.287566 feature_forger-0.1.2/feature_forger/domain/__pycache__/pipeline_runner.cpython-310.pyc
+-rw-r--r--   0        0        0     1380 2023-05-28 10:27:09.271165 feature_forger-0.1.2/feature_forger/domain/composite_task.py
+-rw-r--r--   0        0        0      722 2023-05-28 10:27:09.269670 feature_forger-0.1.2/feature_forger/domain/container.py
+-rw-r--r--   0        0        0     3448 2023-05-28 10:27:09.292544 feature_forger-0.1.2/feature_forger/domain/dag_builder.py
+-rw-r--r--   0        0        0      384 2023-05-28 10:27:09.313904 feature_forger-0.1.2/feature_forger/domain/dataset_model_builder.py
+-rw-r--r--   0        0        0        0 2023-05-06 20:38:54.076868 feature_forger-0.1.2/feature_forger/domain/datasets/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-06 21:39:00.674650 feature_forger-0.1.2/feature_forger/domain/datasets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1052 2023-05-14 22:26:19.549545 feature_forger-0.1.2/feature_forger/domain/datasets/__pycache__/bank.cpython-310.pyc
+-rw-r--r--   0        0        0      661 2023-05-28 10:27:09.295618 feature_forger-0.1.2/feature_forger/domain/datasets/bank.py
+-rw-r--r--   0        0        0        0 2023-05-06 14:46:51.020635 feature_forger-0.1.2/feature_forger/domain/entities/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-06 15:03:15.967190 feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2023-05-28 09:21:12.252157 feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     1150 2023-05-28 09:26:56.898679 feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/entity_model.cpython-310.pyc
+-rw-r--r--   0        0        0     1800 2023-05-28 10:18:23.127374 feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/feature.cpython-310.pyc
+-rw-r--r--   0        0        0      867 2023-05-16 09:02:20.028928 feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/pipeline.cpython-310.pyc
+-rw-r--r--   0        0        0      467 2023-05-28 10:27:09.278297 feature_forger-0.1.2/feature_forger/domain/entities/dataset.py
+-rw-r--r--   0        0        0      466 2023-05-28 09:26:56.100433 feature_forger-0.1.2/feature_forger/domain/entities/entity_model.py
+-rw-r--r--   0        0        0     1174 2023-05-28 10:27:09.276091 feature_forger-0.1.2/feature_forger/domain/entities/feature.py
+-rw-r--r--   0        0        0      450 2023-05-28 10:27:09.290717 feature_forger-0.1.2/feature_forger/domain/entities/pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-06 15:13:09.178992 feature_forger-0.1.2/feature_forger/domain/entity_models/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-06 15:45:52.277290 feature_forger-0.1.2/feature_forger/domain/entity_models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      454 2023-05-06 22:25:35.699458 feature_forger-0.1.2/feature_forger/domain/entity_models/__pycache__/account.cpython-310.pyc
+-rw-r--r--   0        0        0      939 2023-05-06 23:27:01.177121 feature_forger-0.1.2/feature_forger/domain/entity_models/__pycache__/transaction.cpython-310.pyc
+-rw-r--r--   0        0        0      118 2023-05-28 10:27:09.282211 feature_forger-0.1.2/feature_forger/domain/entity_models/account.py
+-rw-r--r--   0        0        0      574 2023-05-28 10:27:09.268313 feature_forger-0.1.2/feature_forger/domain/entity_models/transaction.py
+-rw-r--r--   0        0        0     1046 2023-05-28 10:27:09.274969 feature_forger-0.1.2/feature_forger/domain/feature_validator.py
+-rw-r--r--   0        0        0      636 2023-05-08 14:22:42.700026 feature_forger-0.1.2/feature_forger/domain/features/__init__.py
+-rw-r--r--   0        0        0      717 2023-05-08 14:22:53.702483 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1589 2023-05-28 09:07:55.252110 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc
+-rw-r--r--   0        0        0     1543 2023-05-28 09:25:17.438330 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc
+-rw-r--r--   0        0        0     1837 2023-05-28 09:15:19.332966 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc
+-rw-r--r--   0        0        0     1683 2023-05-28 09:08:32.733441 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc
+-rw-r--r--   0        0        0     1490 2023-05-28 10:19:09.730833 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_month.cpython-310.pyc
+-rw-r--r--   0        0        0     1673 2023-05-28 09:35:59.222751 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc
+-rw-r--r--   0        0        0     1459 2023-05-28 09:08:56.703063 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc
+-rw-r--r--   0        0        0     1618 2023-05-28 09:36:31.151403 feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc
+-rw-r--r--   0        0        0     1016 2023-05-28 10:27:09.263768 feature_forger-0.1.2/feature_forger/domain/features/halved_rounded_amount_change.py
+-rw-r--r--   0        0        0      976 2023-05-28 10:27:09.285112 feature_forger-0.1.2/feature_forger/domain/features/rounded_amount_change.py
+-rw-r--r--   0        0        0     1344 2023-05-28 10:27:09.266603 feature_forger-0.1.2/feature_forger/domain/features/rounded_amount_change_difference.py
+-rw-r--r--   0        0        0     1298 2023-05-28 10:27:09.277112 feature_forger-0.1.2/feature_forger/domain/features/transaction_amount_change.py
+-rw-r--r--   0        0        0      904 2023-05-28 10:27:09.273579 feature_forger-0.1.2/feature_forger/domain/features/transaction_month.py
+-rw-r--r--   0        0        0     1135 2023-05-28 10:27:09.262462 feature_forger-0.1.2/feature_forger/domain/features/transaction_rounded_amount_change_diff_doubled.py
+-rw-r--r--   0        0        0      976 2023-05-28 10:27:09.280725 feature_forger-0.1.2/feature_forger/domain/features/transaction_rounded_amount_change_diff_squared.py
+-rw-r--r--   0        0        0     1088 2023-05-28 10:27:09.288165 feature_forger-0.1.2/feature_forger/domain/features/transaction_rounded_amount_change_doubled.py
+-rw-r--r--   0        0        0     8767 2023-05-28 10:27:09.260919 feature_forger-0.1.2/feature_forger/domain/pipeline_builder.py
+-rw-r--r--   0        0        0      401 2023-05-28 10:27:09.279433 feature_forger-0.1.2/feature_forger/domain/pipeline_runner.py
+-rw-r--r--   0        0        0      710 2023-05-28 11:18:44.597882 feature_forger-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 feature_forger-0.1.2/PKG-INFO
```

### Comparing `feature_forger-0.1.1/feature_forger/application/__pycache__/blacksmith.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/application/__pycache__/blacksmith.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/application/__pycache__/container.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/application/__pycache__/container.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/application/blacksmith.py` & `feature_forger-0.1.2/feature_forger/application/blacksmith.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/application/models/__pycache__/recipe.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/application/models/__pycache__/recipe.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/application/models/recipe.py` & `feature_forger-0.1.2/feature_forger/application/models/recipe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import io
 from typing import Type, List, Callable
 
-import matplotlib.pyplot
 import pandas as pd
 from PIL import Image
-from networkx import DiGraph
-from prefect import Flow
 from pydantic import BaseModel
 from pydot import Dot
 
 from feature_forger.domain.entities.dataset import Dataset
 from feature_forger.domain.entities.entity_model import EntityModel
 
 
@@ -29,10 +26,10 @@
         return self.__repr__()
 
     def __repr_args__(self):
         return [(a, v) if a not in ['dataset']
                 else (a, self.dataset.__class__.__name__)
                 for a, v in super().__repr_args__()]
 
-    def show(self):
+    def view(self):
         image = Image.open(io.BytesIO(self.graph.create_png()))
         image.show()
```

### Comparing `feature_forger-0.1.1/feature_forger/domain/__pycache__/composite_task.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/__pycache__/composite_task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/__pycache__/container.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/__pycache__/container.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/__pycache__/dag_builder.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/__pycache__/dag_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/__pycache__/dataset_model_builder.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/__pycache__/dataset_model_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/__pycache__/feature_validator.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/__pycache__/feature_validator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_builder.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/__pycache__/pipeline_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/__pycache__/pipeline_runner.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/__pycache__/pipeline_runner.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/composite_task.py` & `feature_forger-0.1.2/feature_forger/domain/composite_task.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/container.py` & `feature_forger-0.1.2/feature_forger/domain/container.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/dag_builder.py` & `feature_forger-0.1.2/feature_forger/domain/dag_builder.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/datasets/__pycache__/bank.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/datasets/__pycache__/bank.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/datasets/bank.py` & `feature_forger-0.1.2/feature_forger/domain/datasets/bank.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/dataset.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/entity_model.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/entity_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/feature.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/feature.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/entities/__pycache__/pipeline.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/entities/__pycache__/pipeline.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/entities/feature.py` & `feature_forger-0.1.2/feature_forger/domain/entities/feature.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/entity_models/__pycache__/transaction.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/entity_models/__pycache__/transaction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/entity_models/transaction.py` & `feature_forger-0.1.2/feature_forger/domain/entity_models/transaction.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/feature_validator.py` & `feature_forger-0.1.2/feature_forger/domain/feature_validator.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__init__.py` & `feature_forger-0.1.2/feature_forger/domain/features/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/__init__.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/halved_rounded_amount_change.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/rounded_amount_change.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/rounded_amount_change_difference.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_amount_change.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_month.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_month.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_doubled.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_diff_squared.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc` & `feature_forger-0.1.2/feature_forger/domain/features/__pycache__/transaction_rounded_amount_change_doubled.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/halved_rounded_amount_change.py` & `feature_forger-0.1.2/feature_forger/domain/features/halved_rounded_amount_change.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change.py` & `feature_forger-0.1.2/feature_forger/domain/features/rounded_amount_change.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/rounded_amount_change_difference.py` & `feature_forger-0.1.2/feature_forger/domain/features/rounded_amount_change_difference.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/transaction_amount_change.py` & `feature_forger-0.1.2/feature_forger/domain/features/transaction_amount_change.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/transaction_month.py` & `feature_forger-0.1.2/feature_forger/domain/features/transaction_month.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_doubled.py` & `feature_forger-0.1.2/feature_forger/domain/features/transaction_rounded_amount_change_diff_doubled.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_diff_squared.py` & `feature_forger-0.1.2/feature_forger/domain/features/transaction_rounded_amount_change_diff_squared.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/features/transaction_rounded_amount_change_doubled.py` & `feature_forger-0.1.2/feature_forger/domain/features/transaction_rounded_amount_change_doubled.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/feature_forger/domain/pipeline_builder.py` & `feature_forger-0.1.2/feature_forger/domain/pipeline_builder.py`

 * *Files identical despite different names*

### Comparing `feature_forger-0.1.1/pyproject.toml` & `feature_forger-0.1.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "feature-forger"
-version = "0.1.1"
-description = ""
+version = "0.1.2"
+description = "A feature building framework to extend with your common features and compute on demand."
 authors = ["iccyp <shingle.knitter.0i@icloud.com>"]
 readme = "README.md"
 packages = [{include = "feature_forger"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 prefect = "^2.10.7"
```

### Comparing `feature_forger-0.1.1/PKG-INFO` & `feature_forger-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: feature-forger
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: A feature building framework to extend with your common features and compute on demand.
 Author: iccyp
 Author-email: shingle.knitter.0i@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dependency-injector (>=4.41.0,<5.0.0)
```

