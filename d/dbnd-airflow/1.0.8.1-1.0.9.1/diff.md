# Comparing `tmp/dbnd-airflow-1.0.8.1.tar.gz` & `tmp/dbnd-airflow-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-airflow-1.0.8.1.tar", last modified: Tue Nov 22 15:16:14 2022, max compression
+gzip compressed data, was "dbnd-airflow-1.0.9.1.tar", last modified: Tue Nov 22 16:26:34 2022, max compression
```

## Comparing `dbnd-airflow-1.0.8.1.tar` & `dbnd-airflow-1.0.9.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.334627 dbnd-airflow-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      382 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5875 2022-11-22 15:16:14.334627 dbnd-airflow-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4056 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:14.335627 dbnd-airflow-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4124 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.310625 dbnd-airflow-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.313625 dbnd-airflow-1.0.8.1/src/dbnd_airflow/
--rw-rw-rw-   0 root         (0) root         (0)      272 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.315625 dbnd-airflow-1.0.8.1/src/dbnd_airflow/_vendor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 15:16:10.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/_vendor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4206 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/_vendor/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/_vendor/kubernetes_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.315625 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_extensions/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_extensions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_extensions/airflow_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_extensions/dal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.316625 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 15:16:10.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_aiflow_webserver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.317625 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 15:16:10.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/airflow_windows_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      477 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/getuser.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/timeout.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/operator_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2248 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/bootstrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.318626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4751 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/airflow_multi_version_shim.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/cli_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/dbnd_task_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     1573 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/kubernetes_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3768 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/config.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3116 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/db_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_airflow_main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.320626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2512 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/airflow_operator_as_dbnd.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/airflow_operators_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/converters.py
--rw-rw-rw-   0 root         (0) root         (0)     4940 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/dbnd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)    18016 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     2353 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/optimized_trigger_rule_dep.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/task_instance_state_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.320626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/
--rw-rw-rw-   0 root         (0) root         (0)      357 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.322626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8393 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     7623 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    30939 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    11671 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_watcher.py
--rw-rw-rw-   0 root         (0) root         (0)      992 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     8264 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/simple_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.324626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7971 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/api_functions.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/compat.py
--rw-rw-rw-   0 root         (0) root         (0)     2729 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/dag_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/datetime_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5693 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/dbnd_airflow_export_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     5256 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    14225 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7014 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/queries.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/request_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     3158 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/smart_dagbag.py
--rw-rw-rw-   0 root         (0) root         (0)      966 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.325626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      171 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/dbnd_airflow_operator_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/dbnd_cmd_operators.py
--rw-rw-rw-   0 root         (0) root         (0)    11842 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/dbnd_functional_dag.py
--rw-rw-rw-   0 root         (0) root         (0)     5644 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/dbnd_functional_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/xcom_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.326626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      665 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.326626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/loadable_plugins/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/loadable_plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.327626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/setup_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/raw_constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.328626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dagrun_zombies.py
--rw-rw-rw-   0 root         (0) root         (0)     1691 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dagrun_zombies_clean_job.py
--rw-rw-rw-   0 root         (0) root         (0)     4401 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dags_provider_from_databand.py
--rw-rw-rw-   0 root         (0) root         (0)     8797 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dags_provider_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)     3393 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/scheduler_dags_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    42087 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/single_dag_run_job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.328626 dbnd-airflow-1.0.8.1/src/dbnd_airflow/testing/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/testing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/testing/unittest_env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.331627 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/airflow_connections.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/airflow_patching.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/conf_operations.py
--rw-rw-rw-   0 root         (0) root         (0)     4212 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_airflow_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     7715 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_airflow_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1854 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_dag_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)     3974 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_spark_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     9915 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/execute_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)      956 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/fakes.py
--rw-rw-rw-   0 root         (0) root         (0)    13245 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/wrap_operators.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.331627 dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/airflow_app.py
--rw-rw-rw-   0 root         (0) root         (0)     6166 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/databand_versioned_dagbag.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/single_job_run_support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.314625 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5875 2022-11-22 15:16:14.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5736 2022-11-22 15:16:14.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:14.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-22 15:16:14.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:14.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     3221 2022-11-22 15:16:14.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2022-11-22 15:16:14.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.333627 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/
--rw-rw-rw-   0 root         (0) root         (0)      326 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/README.md
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/credentials_helper_aws.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/credentials_helper_azure.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/credentials_helper_gcp.py
--rw-rw-rw-   0 root         (0) root         (0)     3673 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/dbnd_airflow_default_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/dbnd_operator.py
--rw-rw-rw-   0 root         (0) root         (0)    10716 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/docker_operator.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/kubernetes_metrics_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/mng_connections.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/safe_hostname_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:14.334627 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2500 2022-11-22 15:16:09.000000 dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/utils/system_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.406454 dbnd-airflow-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      382 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5875 2022-11-22 16:26:34.406454 dbnd-airflow-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:34.408455 dbnd-airflow-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4124 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.350449 dbnd-airflow-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.357449 dbnd-airflow-1.0.9.1/src/dbnd_airflow/
+-rw-rw-rw-   0 root         (0) root         (0)      272 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.361450 dbnd-airflow-1.0.9.1/src/dbnd_airflow/_vendor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 16:26:27.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/_vendor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4206 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/_vendor/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1779 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/_vendor/kubernetes_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.363450 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_extensions/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_extensions/airflow_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_extensions/dal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.364450 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 16:26:27.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_aiflow_webserver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.367450 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-22 16:26:27.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/airflow_windows_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      477 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/getuser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1950 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/timeout.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/operator_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/bootstrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.369451 dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4751 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/airflow_multi_version_shim.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/cli_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/dbnd_task_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/kubernetes_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3768 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      785 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/db_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_airflow_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.373451 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2512 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/airflow_operator_as_dbnd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/airflow_operators_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/converters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4940 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/dbnd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)    18016 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/optimized_trigger_rule_dep.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/task_instance_state_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.374451 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.377452 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8393 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7623 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    30939 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    11671 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_watcher.py
+-rw-rw-rw-   0 root         (0) root         (0)      992 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8264 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/simple_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.382452 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7971 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/api_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     2729 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/dag_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      426 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/datetime_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5693 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/dbnd_airflow_export_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     5256 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    14225 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7014 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/request_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/smart_dagbag.py
+-rw-rw-rw-   0 root         (0) root         (0)      966 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.385452 dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/dbnd_airflow_operator_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/dbnd_cmd_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)    11842 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/dbnd_functional_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     5644 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/dbnd_functional_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/xcom_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.386452 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      665 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.387452 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/loadable_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/loadable_plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.388453 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/setup_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/raw_constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.391453 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dagrun_zombies.py
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dagrun_zombies_clean_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     4401 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dags_provider_from_databand.py
+-rw-rw-rw-   0 root         (0) root         (0)     8797 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dags_provider_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     3393 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/scheduler_dags_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    42087 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/single_dag_run_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.392453 dbnd-airflow-1.0.9.1/src/dbnd_airflow/testing/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/testing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2116 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/testing/unittest_env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.397453 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/airflow_connections.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/airflow_patching.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/conf_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4212 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_airflow_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     7715 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_airflow_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_dag_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_spark_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     9915 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/execute_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)      956 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/fakes.py
+-rw-rw-rw-   0 root         (0) root         (0)    13245 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/wrap_operators.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.400454 dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/airflow_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     6166 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/databand_versioned_dagbag.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/single_job_run_support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.360450 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5875 2022-11-22 16:26:34.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5736 2022-11-22 16:26:34.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:34.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-11-22 16:26:34.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:34.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     3221 2022-11-22 16:26:34.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2022-11-22 16:26:34.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.404454 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/
+-rw-rw-rw-   0 root         (0) root         (0)      326 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/credentials_helper_aws.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/credentials_helper_azure.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/credentials_helper_gcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/dbnd_airflow_default_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3105 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/dbnd_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/docker_operator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2689 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/kubernetes_metrics_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/mng_connections.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/safe_hostname_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:34.405454 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2022-11-22 16:26:26.000000 dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/utils/system_utils.py
```

### Comparing `dbnd-airflow-1.0.8.1/LICENSE` & `dbnd-airflow-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/PKG-INFO` & `dbnd-airflow-1.0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-airflow
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

### Comparing `dbnd-airflow-1.0.8.1/README.md` & `dbnd-airflow-1.0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/setup.cfg` & `dbnd-airflow-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-airflow-1.0.8.1/setup.py` & `dbnd-airflow-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/_vendor/database.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/_vendor/database.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/_vendor/kubernetes_utils.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/_vendor/kubernetes_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_extensions/airflow_config.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_extensions/airflow_config.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_extensions/dal.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_extensions/dal.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_aiflow_webserver.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_aiflow_webserver.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/__init__.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/__init__.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/configuration.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/timeout.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/dbnd_airflow_windows/timeout.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_override/operator_helpers.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_override/operator_helpers.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/airflow_utils.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/bootstrap.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/airflow_multi_version_shim.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/airflow_multi_version_shim.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/dbnd_task_runner.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/dbnd_task_runner.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/compat/kubernetes_executor.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/compat/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/config.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/config.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/constants.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/constants.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/db_utils.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/db_utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/airflow_operator_as_dbnd.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/airflow_operator_as_dbnd.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/airflow_operators_catcher.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/airflow_operators_catcher.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/converters.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/converters.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/dbnd_execute.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/dbnd_execute.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_executor_via_airflow.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/dbnd_task_to_airflow_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/optimized_trigger_rule_dep.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/optimized_trigger_rule_dep.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/dbnd_task_executor/task_instance_state_manager.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/dbnd_task_executor/task_instance_state_manager.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_executor.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_runtime_zombies_cleaner.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_scheduler.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_scheduler.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_watcher.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/kubernetes_watcher.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/kubernetes_executor/utils.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/kubernetes_executor/utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/executors/simple_executor.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/executors/simple_executor.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/api_functions.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/api_functions.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/compat.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/compat.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/dag_operations.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/dag_operations.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/dbnd_airflow_export_plugin.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/dbnd_airflow_export_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/helpers.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/helpers.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/metrics.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/metrics.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/models.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/models.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/queries.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/queries.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/request_processing.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/request_processing.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/smart_dagbag.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/smart_dagbag.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/export_plugin/utils.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/export_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/dbnd_cmd_operators.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/dbnd_cmd_operators.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/dbnd_functional_dag.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/dbnd_functional_dag.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/dbnd_functional_operator.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/dbnd_functional_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/functional/xcom_target.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/functional/xcom_target.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/dbnd_airflow_webserver_plugin_linkable.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/loadable_plugins/patched_versioned_bag/dbnd_versioned_dagbag_autoload.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/plugins/setup_plugins.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/plugins/setup_plugins.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dagrun_zombies.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dagrun_zombies.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dagrun_zombies_clean_job.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dagrun_zombies_clean_job.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dags_provider_from_databand.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dags_provider_from_databand.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/dags_provider_from_file.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/dags_provider_from_file.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/scheduler_dags_provider.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/scheduler_dags_provider.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/scheduler/single_dag_run_job.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/scheduler/single_dag_run_job.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/testing/unittest_env.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/testing/unittest_env.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/airflow_patching.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/airflow_patching.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/config.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/config.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_airflow_conf.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_airflow_conf.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_airflow_handler.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_airflow_handler.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_dag_tracking.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_dag_tracking.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/dbnd_spark_conf.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/dbnd_spark_conf.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/execute_tracking.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/execute_tracking.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/fakes.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/fakes.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/tracking/wrap_operators.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/tracking/wrap_operators.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/utils.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/utils.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/airflow_app.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/airflow_app.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/databand_versioned_dagbag.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/databand_versioned_dagbag.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow/web/single_job_run_support.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow/web/single_job_run_support.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/PKG-INFO` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-airflow
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

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/SOURCES.txt` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow.egg-info/requires.txt` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dbnd==1.0.8.1
+dbnd==1.0.9.1
 packaging
 
 [airflow]
 WTForms<2.3.0
 Werkzeug<1.0.0,>=0.15.0
 psycopg2-binary>=2.7.4
 SQLAlchemy==1.3.18
@@ -152,12 +152,12 @@
 psycopg2-binary>=2.7.4
 apache-airflow==2.2.3
 Markdown==3.3.4
 apache-airflow-providers-apache-spark
 SQLAlchemy<1.4
 
 [tests]
-dbnd_test_scenarios==1.0.8.1
+dbnd_test_scenarios==1.0.9.1
 pytest==4.5.0
 boto3
 mock
 sh
```

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/credentials_helper_azure.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/credentials_helper_azure.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/credentials_helper_gcp.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/credentials_helper_gcp.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/dbnd_airflow_default_logger.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/dbnd_airflow_default_logger.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/dbnd_operator.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/dbnd_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/docker_operator.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/docker_operator.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/kubernetes_metrics_logger.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/kubernetes_metrics_logger.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/mng_connections.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/mng_connections.py`

 * *Files identical despite different names*

### Comparing `dbnd-airflow-1.0.8.1/src/dbnd_airflow_contrib/utils/system_utils.py` & `dbnd-airflow-1.0.9.1/src/dbnd_airflow_contrib/utils/system_utils.py`

 * *Files identical despite different names*

