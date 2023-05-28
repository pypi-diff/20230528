# Comparing `tmp/dbnd-test-scenarios-1.0.8.1.tar.gz` & `tmp/dbnd-test-scenarios-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-test-scenarios-1.0.8.1.tar", last modified: Tue Nov 22 15:16:25 2022, max compression
+gzip compressed data, was "dbnd-test-scenarios-1.0.9.1.tar", last modified: Tue Nov 22 16:26:51 2022, max compression
```

## Comparing `dbnd-test-scenarios-1.0.8.1.tar` & `dbnd-test-scenarios-1.0.9.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.723791 dbnd-test-scenarios-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      453 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1434 2022-11-22 15:16:25.723791 dbnd-test-scenarios-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.708789 dbnd-test-scenarios-1.0.8.1/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      719 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/scripts/trigger_ui_functionality.sh
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:25.724791 dbnd-test-scenarios-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      406 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.704789 dbnd-test-scenarios-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.708789 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/
--rw-rw-rw-   0 root         (0) root         (0)      415 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.710790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/airflow_int_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.710790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3271 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/ingest_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2468 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/staging_env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.713790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/bad_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.714790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/client_scoring/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/client_scoring/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6446 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/client_scoring/ingest_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6897 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/client_scoring/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.714790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/common/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/common/pandas_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.716790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/canceled_run_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_deco_extra_param.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_deco_unknown_type.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_double_fault.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_fetch_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_read_custom_dict_types.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_write_read_db_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/handle_error.py
--rw-rw-rw-   0 root         (0) root         (0)     2649 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/heartbeat_error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/large_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      762 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/large_subpipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     1137 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/pipe_4tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/preview_pipeline_values.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/retry_scenario.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/scheduler_scenarios.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/simple_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/simple_read_write_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/task_examples.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/tasks_within_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1822 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/ui_functionality.py
--rw-rw-rw-   0 root         (0) root         (0)     1906 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/scenarios_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.717790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6446 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/ingest_and_train_with_spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.718790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2027 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/ingest_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1666 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count.py
--rw-rw-rw-   0 root         (0) root         (0)     1577 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count_with_error.py
--rw-rw-rw-   0 root         (0) root         (0)     2069 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/spark_io_inline.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/spark_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/spark_tasks_inline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.719791 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.720790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/complex_package_structure/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/complex_package_structure/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.720790 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/complex_package_structure/complex_package/
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/complex_package_structure/complex_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      190 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/complex_package_structure/complex_package/complex_structure_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     2749 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/custom_parameter_feature_store.py
--rw-rw-rw-   0 root         (0) root         (0)     2846 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/custom_parameter_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     6071 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/histogram_tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.721791 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/targets/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/targets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7069 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/targets/base_target_test_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/targets/target_test_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.721791 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/task/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/task/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2680 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/task/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/user_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.722791 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/tracking/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/tracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/tracking/mlflow_example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.722791 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.723791 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/airflow_utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/airflow_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/airflow_utils/af1_get_dbnd_config_token.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.723791 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/chaos_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/client_scoring_chaos.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/data_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1208 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/subprocess_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:25.709789 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1434 2022-11-22 15:16:25.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4389 2022-11-22 15:16:25.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:25.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:25.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 15:16:25.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-22 15:16:25.000000 dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1228 2022-11-22 15:16:09.000000 dbnd-test-scenarios-1.0.8.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.073163 dbnd-test-scenarios-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      453 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1434 2022-11-22 16:26:51.073163 dbnd-test-scenarios-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      132 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.054161 dbnd-test-scenarios-1.0.9.1/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      719 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/scripts/trigger_ui_functionality.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:51.075163 dbnd-test-scenarios-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      406 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.050161 dbnd-test-scenarios-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.055161 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)      415 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.057161 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/airflow_int_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.057161 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/ingest_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/staging_env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.061162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/bad_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.062162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/client_scoring/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/client_scoring/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6446 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/client_scoring/ingest_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6897 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/client_scoring/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.062162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/common/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/common/pandas_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.065162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/canceled_run_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_deco_extra_param.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_deco_unknown_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_double_fault.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_fetch_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_read_custom_dict_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_write_read_db_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/handle_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     2649 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/heartbeat_error_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/large_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      762 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/large_subpipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1137 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/pipe_4tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/preview_pipeline_values.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/retry_scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/scheduler_scenarios.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/simple_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/simple_read_write_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/task_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/tasks_within_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1822 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/ui_functionality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/scenarios_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.067162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6446 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/ingest_and_train_with_spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.068162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2027 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/ingest_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count.py
+-rw-rw-rw-   0 root         (0) root         (0)     1577 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count_with_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/spark_io_inline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/spark_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      818 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/spark_tasks_inline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.069162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.069162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/complex_package_structure/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/complex_package_structure/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.069162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/complex_package_structure/complex_package/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/complex_package_structure/complex_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      190 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/complex_package_structure/complex_package/complex_structure_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2749 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/custom_parameter_feature_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     2846 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/custom_parameter_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     6071 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/histogram_tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.070162 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/targets/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/targets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7069 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/targets/base_target_test_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/targets/target_test_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.071163 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/task/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/task/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2680 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/task/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/user_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.071163 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/tracking/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/tracking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/tracking/mlflow_example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.072163 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.072163 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/airflow_utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/airflow_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1186 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/airflow_utils/af1_get_dbnd_config_token.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.073163 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/chaos_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/client_scoring_chaos.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/data_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/subprocess_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:51.056161 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1434 2022-11-22 16:26:50.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4389 2022-11-22 16:26:51.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:50.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:50.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 16:26:50.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-11-22 16:26:50.000000 dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2022-11-22 16:26:26.000000 dbnd-test-scenarios-1.0.9.1/tox.ini
```

### Comparing `dbnd-test-scenarios-1.0.8.1/LICENSE` & `dbnd-test-scenarios-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/PKG-INFO` & `dbnd-test-scenarios-1.0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-test-scenarios
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

### Comparing `dbnd-test-scenarios-1.0.8.1/scripts/trigger_ui_functionality.sh` & `dbnd-test-scenarios-1.0.9.1/scripts/trigger_ui_functionality.sh`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/setup.cfg` & `dbnd-test-scenarios-1.0.9.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.8.1
+version = 1.0.9.1
 license_file = LICENSE
 description = Machine Learning Orchestration
 long_description_content_type = text/markdown
 long_description = file: README.md
 platforms = any
 author = Evgeny Shulman
 author_email = evgeny.shulman@databand.ai
```

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/airflow_int_test_utils.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/airflow_int_test_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/ingest_data.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/client_scoring/ingest_data.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/airflow_scenarios/staging_env.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/airflow_scenarios/staging_env.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/client_scoring/ingest_data.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/client_scoring/ingest_data.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/client_scoring/train.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/client_scoring/train.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/common/pandas_tasks.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/common/pandas_tasks.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/canceled_run_pipeline.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/canceled_run_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_double_fault.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_double_fault.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_fetch_data.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_fetch_data.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_pipelines.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/error_write_read_db_pipeline.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/error_write_read_db_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/handle_error.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/handle_error.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/errors/heartbeat_error_handling.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/errors/heartbeat_error_handling.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/large_pipeline.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/large_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/large_subpipelines.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/large_subpipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/pipe_4tasks.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/pipe_4tasks.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/preview_pipeline_values.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/preview_pipeline_values.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/retry_scenario.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/retry_scenario.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/scheduler_scenarios.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/scheduler_scenarios.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/simple_read_write_pipeline.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/simple_read_write_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/task_examples.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/task_examples.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/pipelines/ui_functionality.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/pipelines/ui_functionality.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/scenarios_repo.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/scenarios_repo.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/ingest_and_train_with_spark.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/ingest_and_train_with_spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/ingest_pipeline.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/ingest_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count_with_error.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/pyspark_scripts/word_count_with_error.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/spark_io_inline.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/spark_io_inline.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/spark_tasks.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/spark_tasks.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/spark/spark_tasks_inline.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/spark/spark_tasks_inline.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/custom_parameter_feature_store.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/custom_parameter_feature_store.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/custom_parameter_hdf5.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/custom_parameter_hdf5.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/histogram_tests.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/histogram_tests.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/targets/base_target_test_mixin.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/targets/base_target_test_mixin.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/targets/target_test_base.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/targets/target_test_base.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/test_common/task/factories.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/test_common/task/factories.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/tracking/mlflow_example.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/tracking/mlflow_example.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/airflow_utils/af1_get_dbnd_config_token.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/airflow_utils/af1_get_dbnd_config_token.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/chaos_utils.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/chaos_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/client_scoring_chaos.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/data_chaos_monkey/client_scoring_chaos.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios/utils/subprocess_utils.py` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/PKG-INFO` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-test-scenarios
-Version: 1.0.8.1
+Version: 1.0.9.1
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 License: UNKNOWN
```

### Comparing `dbnd-test-scenarios-1.0.8.1/src/dbnd_test_scenarios.egg-info/SOURCES.txt` & `dbnd-test-scenarios-1.0.9.1/src/dbnd_test_scenarios.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbnd-test-scenarios-1.0.8.1/tox.ini` & `dbnd-test-scenarios-1.0.9.1/tox.ini`

 * *Files identical despite different names*

