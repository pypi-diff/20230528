# Comparing `tmp/dbnd-examples-1.0.8.1.tar.gz` & `tmp/dbnd-examples-1.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-examples-1.0.8.1.tar", last modified: Tue Nov 22 15:16:28 2022, max compression
+gzip compressed data, was "dbnd-examples-1.0.9.1.tar", last modified: Tue Nov 22 16:26:54 2022, max compression
```

## Comparing `dbnd-examples-1.0.8.1.tar` & `dbnd-examples-1.0.9.1.tar`

### file list

```diff
@@ -1,284 +1,284 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.203044 dbnd-examples-1.0.8.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 15:16:28.203044 dbnd-examples-1.0.8.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      276 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.163040 dbnd-examples-1.0.8.1/data/
--rw-rw-rw-   0 root         (0) root         (0)      707 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/examples_config.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.153039 dbnd-examples-1.0.8.1/data/partitioned_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.163040 dbnd-examples-1.0.8.1/data/partitioned_data/2018-09-01/
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/partitioned_data/2018-09-01/file.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.163040 dbnd-examples-1.0.8.1/data/partitioned_data/2018-09-02/
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/partitioned_data/2018-09-02/file.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.164040 dbnd-examples-1.0.8.1/data/partitioned_data/2018-09-03/
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/partitioned_data/2018-09-03/file.csv
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/partitioned_data/2018-09-03/file2.csv
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/people.txt
--rw-rw-rw-   0 root         (0) root         (0)    33543 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/pipeline_train_seed_data.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.164040 dbnd-examples-1.0.8.1/data/raw_logs/
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/raw_logs/2018-06-20.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/raw_logs/2018-06-21.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/raw_logs/2018-06-22.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/vegetables_for_greek_salad.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/vegetables_for_pasta_salad.txt
--rw-rw-rw-   0 root         (0) root         (0)   264426 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/wine_quality.csv
--rw-rw-rw-   0 root         (0) root         (0)    69193 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/wine_quality.csv.gz
--rw-rw-rw-   0 root         (0) root         (0)    79704 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/wine_quality.py27.parquet
--rw-rw-rw-   0 root         (0) root         (0)    19832 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/wine_quality.py36.parquet
--rw-rw-rw-   0 root         (0) root         (0)    33543 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/data/wine_quality_minimized.csv
--rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 15:16:28.205044 dbnd-examples-1.0.8.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      979 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.153039 dbnd-examples-1.0.8.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.165040 dbnd-examples-1.0.8.1/src/dbnd_examples/
--rw-rw-rw-   0 root         (0) root         (0)      408 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      605 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2179 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.167040 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1441 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/bash_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/clear_dag.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/dbnd_dags_from_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.168041 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/
--rw-rw-rw-   0 root         (0) root         (0)     4574 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_cluster_monitor_template.py
--rw-rw-rw-   0 root         (0) root         (0)     2439 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_table_monitor_template.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/python_op_dag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.168041 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/snowflake/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/snowflake/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2977 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_dag.py
--rw-rw-rw-   0 root         (0) root         (0)     3282 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_log_hook_dag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.168041 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/
--rw-rw-rw-   0 root         (0) root         (0)      185 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.169041 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/
--rw-rw-rw-   0 root         (0) root         (0)     3600 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/pom.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.154039 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.154039 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.154039 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.155039 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.155039 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.169041 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/
--rw-rw-rw-   0 root         (0) root         (0)       60 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/AddDressing.java
--rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java
--rw-rw-rw-   0 root         (0) root         (0)     2073 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java
--rw-rw-rw-   0 root         (0) root         (0)     2438 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.170041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.172041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      791 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_decorator2.py
--rw-rw-rw-   0 root         (0) root         (0)      929 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1834 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_excel.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_override.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_output_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_output_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1294 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_paramester_user_object.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_target.py
--rw-rw-rw-   0 root         (0) root         (0)     2171 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_value_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.173041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_airflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1457 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_airflow/scheduled_dbnd_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.173041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.173041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2166 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/scheduled_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     3573 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/ingest_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     2707 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/sync_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.174041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_docker/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_docker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_docker/docker_run_task_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_docker/dockerized_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.174041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.175041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_bigquery/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_bigquery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_bigquery/wine_quality_big_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.175041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py
--rw-rw-rw-   0 root         (0) root         (0)     4971 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.176041 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.177042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2339 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/read_from_multiple_sources.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/salad_spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.178042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      149 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/add_dressing.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/cut_salad.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/word_count.py
--rw-rw-rw-   0 root         (0) root         (0)     3679 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/spark_config_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     3031 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/word_count.py
--rw-rw-rw-   0 root         (0) root         (0)     2768 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/word_count_with_deequ.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.179042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2540 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/report.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/salad.py
--rw-rw-rw-   0 root         (0) root         (0)     2046 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/top_artists.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/top_artists__as_task_class.py
--rw-rw-rw-   0 root         (0) root         (0)     5882 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality_as_notebook.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5287 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality_as_task_class.py
--rw-rw-rw-   0 root         (0) root         (0)   123099 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality_pipeline.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.181042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/dynamic_tasks_with_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/example_dict_of_data_frames.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/example_folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/example_output_per_id.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_by_day.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_calculations_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_data_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     2131 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/pipeline_with_sub_runs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.182042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/
--rw-rw-rw-   0 root         (0) root         (0)      209 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2630 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/data.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_digit_mnist.py
--rw-rw-rw-   0 root         (0) root         (0)     4454 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_fashion_mnist.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.183042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/
--rw-rw-rw-   0 root         (0) root         (0)      233 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8579 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/amazon_video_reviews.py
--rw-rw-rw-   0 root         (0) root         (0)     9476 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist_pytorch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.184042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3338 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/run_example.sh
--rw-rw-rw-   0 root         (0) root         (0)     2617 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/sklearn_example.py
--rw-rw-rw-   0 root         (0) root         (0)     7671 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/train_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     5608 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/train_via_spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.185042 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/
--rw-rw-rw-   0 root         (0) root         (0)      137 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3034 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/iris.py
--rw-rw-rw-   0 root         (0) root         (0)     3951 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_iris.py
--rw-rw-rw-   0 root         (0) root         (0)     4692 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.187043 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T02_task_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T03_task_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T11_data_wiring.py
--rw-rw-rw-   0 root         (0) root         (0)     1773 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T22_user_class_as_task.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.187043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.187043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.189043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.189043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/environment_configuration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/environment_configuration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.189043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.190043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/object_configuration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/object_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/object_configuration/test_doc_configuration_layers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.190043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3735 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.191043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1251 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_run_results.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_overriding_configuration_in_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_running_pipelines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.193043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_engine_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_task_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.195043 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2959 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     4439 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py
--rw-rw-rw-   0 root         (0) root         (0)     3311 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2207 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_faq.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_object_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      947 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_configuration_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_object.py
--rw-rw-rw-   0 root         (0) root         (0)     3389 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_quick_start_wine_quality.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.198044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4720 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_airflow_and_snowflake.py
--rw-rw-rw-   0 root         (0) root         (0)     1673 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_explicit_dataset_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_functions.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_performant_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1189 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_pyspark_dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)     1452 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_python_scripts.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_airflow_dags.py
--rw-rw-rw-   0 root         (0) root         (0)     1172 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_databricks.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_mlflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1621 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_pandas_dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)     7903 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_quickstart.py
--rw-rw-rw-   0 root         (0) root         (0)     1287 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_redshift.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_snowflake_guide.py
--rw-rw-rw-   0 root         (0) root         (0)     1304 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_spark_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.198044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.199044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/customizations/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/customizations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/customizations/test_custom_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2557 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/customizations/test_feature_custom.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/customizations/test_run_with_custom_targets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.200044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/dbnd_spark/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/dbnd_spark/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/dbnd_spark/test_spark_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.201044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_example_salad.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_report.py
--rw-rw-rw-   0 root         (0) root         (0)      345 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_salad.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_top_artist.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_wine_quality.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.202044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/test_dynamic_tasks_with_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/test_feature_by_day_prod.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/test_feature_input_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1552 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/test_feature_partitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.202044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tool_sklearn/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tool_sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tool_sklearn/test_sklearn_linear_reg_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.202044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T12_pandas_numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.203044 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/tracking/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/tracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/tracking/test_redshift_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tests/tracking/test_tool_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.203044 dbnd-examples-1.0.8.1/src/dbnd_examples/tracking/
--rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tracking/tracking_mlflow.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/src/dbnd_examples/tracking/tracking_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 15:16:28.166041 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 15:16:28.000000 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14529 2022-11-22 15:16:28.000000 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:28.000000 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2022-11-22 15:16:28.000000 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 15:16:28.000000 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      206 2022-11-22 15:16:28.000000 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 15:16:28.000000 dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2241 2022-11-22 15:16:09.000000 dbnd-examples-1.0.8.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.691536 dbnd-examples-1.0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 16:26:54.691536 dbnd-examples-1.0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      276 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.628530 dbnd-examples-1.0.9.1/data/
+-rw-rw-rw-   0 root         (0) root         (0)      707 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/examples_config.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.605527 dbnd-examples-1.0.9.1/data/partitioned_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.628530 dbnd-examples-1.0.9.1/data/partitioned_data/2018-09-01/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/partitioned_data/2018-09-01/file.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.628530 dbnd-examples-1.0.9.1/data/partitioned_data/2018-09-02/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/partitioned_data/2018-09-02/file.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.630530 dbnd-examples-1.0.9.1/data/partitioned_data/2018-09-03/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/partitioned_data/2018-09-03/file.csv
+-rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/partitioned_data/2018-09-03/file2.csv
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/people.txt
+-rw-rw-rw-   0 root         (0) root         (0)    33543 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/pipeline_train_seed_data.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.632530 dbnd-examples-1.0.9.1/data/raw_logs/
+-rw-rw-rw-   0 root         (0) root         (0)        8 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/raw_logs/2018-06-20.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/raw_logs/2018-06-21.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/raw_logs/2018-06-22.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/vegetables_for_greek_salad.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/vegetables_for_pasta_salad.txt
+-rw-rw-rw-   0 root         (0) root         (0)   264426 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/wine_quality.csv
+-rw-rw-rw-   0 root         (0) root         (0)    69193 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/wine_quality.csv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    79704 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/wine_quality.py27.parquet
+-rw-rw-rw-   0 root         (0) root         (0)    19832 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/wine_quality.py36.parquet
+-rw-rw-rw-   0 root         (0) root         (0)    33543 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/data/wine_quality_minimized.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2117 2022-11-22 16:26:54.692536 dbnd-examples-1.0.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      979 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.606527 dbnd-examples-1.0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.634530 dbnd-examples-1.0.9.1/src/dbnd_examples/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      605 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2179 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.636530 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/bash_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/clear_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/dbnd_dags_from_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.637530 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     4574 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_cluster_monitor_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2439 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_table_monitor_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/python_op_dag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.637530 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/snowflake/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/snowflake/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2977 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     3282 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_log_hook_dag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.638531 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.639531 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/
+-rw-rw-rw-   0 root         (0) root         (0)     3600 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/pom.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.607527 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.607527 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.607527 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.607527 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.607527 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.640531 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/AddDressing.java
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java
+-rw-rw-rw-   0 root         (0) root         (0)     2438 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.640531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.642531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      791 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_decorator2.py
+-rw-rw-rw-   0 root         (0) root         (0)      929 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_excel.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_override.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_output_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_output_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1294 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_paramester_user_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_target.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_value_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.642531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_airflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_airflow/scheduled_dbnd_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.643531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.643531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2166 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/scheduled_sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3573 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/ingest_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/sync_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.644531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_docker/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_docker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_docker/docker_run_task_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_docker/dockerized_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.644531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.644531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_bigquery/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_bigquery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_bigquery/wine_quality_big_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.645531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.646531 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.648532 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2339 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/read_from_multiple_sources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/salad_spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.650532 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/add_dressing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/cut_salad.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/word_count.py
+-rw-rw-rw-   0 root         (0) root         (0)     3679 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/spark_config_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/word_count.py
+-rw-rw-rw-   0 root         (0) root         (0)     2768 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/word_count_with_deequ.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.653532 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/salad.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/top_artists.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/top_artists__as_task_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     5882 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality_as_notebook.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5287 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality_as_task_class.py
+-rw-rw-rw-   0 root         (0) root         (0)   123099 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality_pipeline.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.657533 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/dynamic_tasks_with_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/example_dict_of_data_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/example_folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/example_output_per_id.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_by_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_calculations_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_data_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2131 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/pipeline_with_sub_runs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.658533 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_digit_mnist.py
+-rw-rw-rw-   0 root         (0) root         (0)     4454 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_fashion_mnist.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.659533 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8579 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/amazon_video_reviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     9476 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist_pytorch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.661533 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/run_example.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/sklearn_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     7671 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/train_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     5608 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/train_via_spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.662533 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3034 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/iris.py
+-rw-rw-rw-   0 root         (0) root         (0)     3951 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_iris.py
+-rw-rw-rw-   0 root         (0) root         (0)     4692 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.666534 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T02_task_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T03_task_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T11_data_wiring.py
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T22_user_class_as_task.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.666534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.666534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.668534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.668534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/environment_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/environment_configuration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.669534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.670534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/object_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/object_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/object_configuration/test_doc_configuration_layers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.670534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3735 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.672534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1251 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_run_results.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_overriding_configuration_in_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_running_pipelines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.674534 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_engine_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_task_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.676535 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2959 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     4439 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2207 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_faq.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_object_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      947 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_configuration_defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     3389 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_quick_start_wine_quality.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.681535 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4720 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_airflow_and_snowflake.py
+-rw-rw-rw-   0 root         (0) root         (0)     1673 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_explicit_dataset_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_functions.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_performant_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_pyspark_dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_python_scripts.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_airflow_dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1172 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_databricks.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_mlflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1621 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_pandas_dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)     7903 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_quickstart.py
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_redshift.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_snowflake_guide.py
+-rw-rw-rw-   0 root         (0) root         (0)     1304 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_spark_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.681535 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.683535 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/customizations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/customizations/test_custom_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2557 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/customizations/test_feature_custom.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/customizations/test_run_with_custom_targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.683535 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/dbnd_spark/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/dbnd_spark/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/dbnd_spark/test_spark_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.685536 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      916 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_example_salad.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_salad.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_top_artist.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_wine_quality.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.686535 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/test_dynamic_tasks_with_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/test_feature_by_day_prod.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/test_feature_input_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1552 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/test_feature_partitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.687536 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tool_sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tool_sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tool_sklearn/test_sklearn_linear_reg_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.689536 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T12_pandas_numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.689536 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/tracking/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/tracking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/tracking/test_redshift_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tests/tracking/test_tool_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.690536 dbnd-examples-1.0.9.1/src/dbnd_examples/tracking/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tracking/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tracking/tracking_mlflow.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/src/dbnd_examples/tracking/tracking_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 16:26:54.635530 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1699 2022-11-22 16:26:54.000000 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14529 2022-11-22 16:26:54.000000 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:54.000000 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2022-11-22 16:26:54.000000 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 16:26:54.000000 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      206 2022-11-22 16:26:54.000000 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-11-22 16:26:54.000000 dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2241 2022-11-22 16:26:26.000000 dbnd-examples-1.0.9.1/tox.ini
```

### Comparing `dbnd-examples-1.0.8.1/LICENSE` & `dbnd-examples-1.0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/PKG-INFO` & `dbnd-examples-1.0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-examples
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

### Comparing `dbnd-examples-1.0.8.1/data/examples_config.cfg` & `dbnd-examples-1.0.9.1/data/examples_config.cfg`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/data/pipeline_train_seed_data.csv` & `dbnd-examples-1.0.9.1/data/pipeline_train_seed_data.csv`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/data/wine_quality.csv` & `dbnd-examples-1.0.9.1/data/wine_quality.csv`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/data/wine_quality.csv.gz` & `dbnd-examples-1.0.9.1/data/wine_quality.csv.gz`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/data/wine_quality.py27.parquet` & `dbnd-examples-1.0.9.1/data/wine_quality.py27.parquet`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/data/wine_quality.py36.parquet` & `dbnd-examples-1.0.9.1/data/wine_quality.py36.parquet`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/data/wine_quality_minimized.csv` & `dbnd-examples-1.0.9.1/data/wine_quality_minimized.csv`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/setup.cfg` & `dbnd-examples-1.0.9.1/setup.cfg`

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

### Comparing `dbnd-examples-1.0.8.1/setup.py` & `dbnd-examples-1.0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/_plugin.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/data.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/data.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/bash_dag.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/bash_dag.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/clear_dag.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/clear_dag.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_cluster_monitor_template.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_cluster_monitor_template.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_table_monitor_template.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/monitoring_templates/redshift_table_monitor_template.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/python_op_dag.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/python_op_dag.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_dag.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_dag.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_log_hook_dag.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_airflow/snowflake/snowflake_log_hook_dag.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/pom.xml` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/pom.xml`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java` & `dbnd-examples-1.0.9.1/src/dbnd_examples/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_decorator.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_decorator.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_decorator2.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_decorator2.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_logging.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_logging.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_excel.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_excel.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_override.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_marshaller_override.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_output_factory.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_output_factory.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_output_location.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_output_location.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_paramester_user_object.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_paramester_user_object.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_target.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_target.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/customizations/custom_value_type.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/customizations/custom_value_type.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_airflow/scheduled_dbnd_check.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_airflow/scheduled_dbnd_check.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/scheduled_sensor.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/airflow/scheduled_sensor.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/ingest_pipeline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/ingest_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_aws/sync_operators.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_aws/sync_operators.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_docker/dockerized_pipeline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_docker/dockerized_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/read_from_multiple_sources.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/read_from_multiple_sources.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/salad_spark.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/salad_spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/add_dressing.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/add_dressing.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/cut_salad.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/cut_salad.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/word_count.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/scripts/word_count.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/spark_config_examples.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/spark_config_examples.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/word_count.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/word_count.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/dbnd_spark/word_count_with_deequ.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/dbnd_spark/word_count_with_deequ.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/report.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/report.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/salad.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/salad.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/top_artists.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/top_artists.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/top_artists__as_task_class.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/top_artists__as_task_class.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality_as_notebook.ipynb` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality_as_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality_as_task_class.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality_as_task_class.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/examples/wine_quality_pipeline.png` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/examples/wine_quality_pipeline.png`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/dynamic_tasks_with_pipeline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/dynamic_tasks_with_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/example_folder.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/example_folder.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/example_output_per_id.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/example_output_per_id.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_by_day.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_by_day.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_calculations_pipeline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_calculations_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_data_pipeline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/partitioned_inputs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/partitioned_inputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/features/pipeline_with_sub_runs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/features/pipeline_with_sub_runs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/data.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/data.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_digit_mnist.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_digit_mnist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_fashion_mnist.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_task.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_mxnet/mxnet_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/amazon_video_reviews.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/amazon_video_reviews.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist_pytorch.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sagemaker/mnist_pytorch.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/generate.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/generate.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/run_example.sh` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/run_example.sh`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/sklearn_example.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/sklearn_example.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/train_pipeline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_sklearn/train_via_spark.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_sklearn/train_via_spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/iris.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/iris.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_iris.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_iris.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_simple.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tool_tensorflow/tf_simple.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T02_task_parameters.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T02_task_parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T03_task_outputs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T03_task_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T11_data_wiring.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T11_data_wiring.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/orchestration/tutorial_syntax/T22_user_class_as_task.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/orchestration/tutorial_syntax/T22_user_class_as_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_run_results.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_run_results.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_object_configuration.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_object_configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_configuration_defaults.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_configuration_defaults.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_object.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_doc_task_object.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/orchestration/test_quick_start_wine_quality.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/orchestration/test_quick_start_wine_quality.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_airflow_and_snowflake.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_airflow_and_snowflake.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_explicit_dataset_logging.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_explicit_dataset_logging.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_functions.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_functions.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_performant_logging.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_performant_logging.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_pyspark_dataframe.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_pyspark_dataframe.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_python_scripts.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_python_scripts.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_airflow_dags.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_airflow_dags.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_databricks.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_databricks.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_mlflow.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_mlflow.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_pandas_dataframe.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_quickstart.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_quickstart.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_redshift.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_redshift.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_snowflake_guide.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_snowflake_guide.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_spark_jobs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_spark_jobs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_sql.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/documentation/tracking/test_doc_tracking_sql.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/customizations/test_feature_custom.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/customizations/test_feature_custom.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/dbnd_spark/test_spark_task.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/dbnd_spark/test_spark_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_example_salad.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_example_salad.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_top_artist.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_top_artist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/examples/test_wine_quality.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/examples/test_wine_quality.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/test_feature_by_day_prod.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/test_feature_by_day_prod.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/test_feature_input_outputs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/test_feature_input_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/features/test_feature_partitions.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/features/test_feature_partitions.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/tracking/test_redshift_tracking.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/tracking/test_redshift_tracking.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tests/tracking/test_tool_script.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tests/tracking/test_tool_script.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples/tracking/tracking_mlflow.py` & `dbnd-examples-1.0.9.1/src/dbnd_examples/tracking/tracking_mlflow.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/PKG-INFO` & `dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-examples
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

### Comparing `dbnd-examples-1.0.8.1/src/dbnd_examples.egg-info/SOURCES.txt` & `dbnd-examples-1.0.9.1/src/dbnd_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbnd-examples-1.0.8.1/tox.ini` & `dbnd-examples-1.0.9.1/tox.ini`

 * *Files identical despite different names*

