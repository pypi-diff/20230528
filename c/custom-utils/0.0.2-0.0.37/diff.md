# Comparing `tmp/custom-utils-0.0.2.tar.gz` & `tmp/custom-utils-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom-utils-0.0.2.tar", last modified: Mon Nov 15 09:37:13 2021, max compression
+gzip compressed data, was "custom-utils-0.0.37.tar", last modified: Sat May 27 15:27:13 2023, max compression
```

## Comparing `custom-utils-0.0.2.tar` & `custom-utils-0.0.37.tar`

### file list

```diff
@@ -1,21 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-11-15 09:37:13.363798 custom-utils-0.0.2/
--rwxrwxrwx   0 root         (0) root         (0)    20543 2021-11-15 09:37:13.363645 custom-utils-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    16342 2021-11-15 09:29:43.000000 custom-utils-0.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-11-15 09:37:13.360513 custom-utils-0.0.2/custom_utils/
--rwxrwxrwx   0 root         (0) root         (0)      249 2021-10-17 12:01:46.000000 custom-utils-0.0.2/custom_utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       54 2021-10-17 10:04:55.000000 custom-utils-0.0.2/custom_utils/config.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-11-15 09:37:13.363029 custom-utils-0.0.2/custom_utils/connector/
--rwxrwxrwx   0 root         (0) root         (0)        0 2021-11-15 09:26:37.000000 custom-utils-0.0.2/custom_utils/connector/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6071 2021-11-15 09:28:24.000000 custom-utils-0.0.2/custom_utils/connector/bigquery.py
--rwxrwxrwx   0 root         (0) root         (0)     8732 2021-10-17 13:49:58.000000 custom-utils-0.0.2/custom_utils/connector/mongodb.py
--rwxrwxrwx   0 root         (0) root         (0)     2200 2021-10-17 13:49:48.000000 custom-utils-0.0.2/custom_utils/connector/mysql.py
--rwxrwxrwx   0 root         (0) root         (0)     2902 2021-10-17 11:52:53.000000 custom-utils-0.0.2/custom_utils/connector/s3.py
--rwxrwxrwx   0 root         (0) root         (0)      919 2021-10-17 11:57:47.000000 custom-utils-0.0.2/custom_utils/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2021-11-15 09:37:13.361583 custom-utils-0.0.2/custom_utils.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    20543 2021-11-15 09:37:13.000000 custom-utils-0.0.2/custom_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      437 2021-11-15 09:37:13.000000 custom-utils-0.0.2/custom_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2021-11-15 09:37:13.000000 custom-utils-0.0.2/custom_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      466 2021-11-15 09:37:13.000000 custom-utils-0.0.2/custom_utils.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       13 2021-11-15 09:37:13.000000 custom-utils-0.0.2/custom_utils.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2021-11-15 09:37:13.363855 custom-utils-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1401 2021-11-15 09:27:03.000000 custom-utils-0.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.837412 custom-utils-0.0.37/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1068 2023-05-18 07:57:45.000000 custom-utils-0.0.37/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-27 15:27:13.837412 custom-utils-0.0.37/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15705 2023-05-27 15:26:46.000000 custom-utils-0.0.37/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.821412 custom-utils-0.0.37/custom_utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      249 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.829412 custom-utils-0.0.37/custom_utils/alerter/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.37/custom_utils/alerter/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1258 2023-05-27 14:34:54.000000 custom-utils-0.0.37/custom_utils/alerter/slack.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/config.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.829412 custom-utils-0.0.37/custom_utils/configurer/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.37/custom_utils/configurer/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2138 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/configurer/profiler.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2473 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/configurer/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.833413 custom-utils-0.0.37/custom_utils/connector/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-18 07:58:13.000000 custom-utils-0.0.37/custom_utils/connector/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7285 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/connector/bigquery.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8750 2023-05-18 07:57:45.000000 custom-utils-0.0.37/custom_utils/connector/mongodb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2232 2023-05-27 13:04:17.000000 custom-utils-0.0.37/custom_utils/connector/mysql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4066 2023-05-27 13:15:15.000000 custom-utils-0.0.37/custom_utils/connector/s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1017 2023-05-27 10:52:53.000000 custom-utils-0.0.37/custom_utils/exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      568 2023-05-27 12:41:24.000000 custom-utils-0.0.37/custom_utils/utils.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-27 15:27:13.825412 custom-utils-0.0.37/custom_utils.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    16335 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      484 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-05-27 15:27:13.000000 custom-utils-0.0.37/custom_utils.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-27 15:27:13.837412 custom-utils-0.0.37/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1402 2023-05-27 15:27:02.000000 custom-utils-0.0.37/setup.py
```

### Comparing `custom-utils-0.0.2/PKG-INFO` & `custom-utils-0.0.37/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,466 +1,470 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.2
+Version: 0.0.37
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
-License: UNKNOWN
-Description: # custom-utils
-        Pip Package for Database Connectors, Alerter, Log Formatter etc
-        
-        
-        ***
-        
-        <p float="left">
-          <img src=https://img.shields.io/pypi/v/custom-utils />
-          <img src=https://www.code-inspector.com/project/29426/score/svg />
-          <img src=https://img.shields.io/pypi/dm/custom-utils?logo=Python&style=social /> 
-          <a href="https://github.com/RahulnKumar/custom-utils/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/RahulnKumar/custom-utils"></a>
-        </p>
-         
-        
-        ## Table of Contents
-        
-        - [Installation](#Installation)
-        - [Connector](#Connector)
-          - [S3 Connector](#S3_Connector)
-          - [MySQL Connector](#MySQL_Connector)
-          - [MongoDB Connector](#MongoDB_Connector)
-          - [BigQuery Connector](#BigQuery_Connector)
-         
-        - [Configurer](#Configurer)
-          - [Log Formatter](#Log_Formatter)
-          - [Profile Decorator](#Profile_Decorator)
-          
-        - [Alerter](#Alerter)
-          - [Slack Alerter](#Slack_Alerter)
-        
-        ***
-        
-        ## 1.  Installation<a id="Installation" name="Installation">    
-        
-        - **Installation from Pypi repository** (Any one)
-        	
-            `pip install custom-utils`  --> minimal installation  
-            `pip install custom-utils[full]` --> full installation  
-            `pip install custom-utils[s3,mysql,bigquery,mongodb]`  --> selective installation 
-        - **Installation from github repository** (Any one)  
-        	
-            `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
-            `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
-            `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
-            
-        ---
-            
-        	
-        ## 2. Connector<a id="Connector" name="Connector">
-        
-            
-        ### 1. S3 Connector<a id="S3_Connector" name="S3_Connector">     
-        
-        **Code Snippet Sample :**
-        ```python
-        from custom_utils.connector.s3 import S3
-        
-        # Uplaoding data to S3
-        demo = {"Name": "Trell", "Age": 4}
-        S3.write_to_s3_bucket(python_data_object=demo,
-                                     bucket='data-science-datas',
-                                     sub_bucket='models/', file_name="demo.pickle")
-                                     
-        # Doownlaoding data from S3
-        
-        demo = S3.read_from_s3_bucket(bucket='data-science-datas',          
-                                                 sub_bucket='models/',
-                                                 file_name="demo.pickle")
-        ```
-        
-        **S3 Connector Documentation**
-            
-        ```
-        class S3(builtins.object)
-         |  AWS S3 utility functions
-         |  
-         |  Static methods defined here:
-         |  
-         |  read_from_s3_bucket(bucket, sub_bucket, file_name)
-         |      read data stored in S3 bucket
-         |      :param string bucket: bucket name
-         |      :param string sub_bucket: sub-bucket name
-         |      :param string file_name: name of the file to be read
-         |      :return old_data : python object stored in the S3
-         |  
-         |  upload_data_from_local_to_s3(model_file_name, bucket, sub_bucket)
-         |      write data stored in local machine into S3 bucket from
-         |      :param string bucket: bucket name
-         |      :param string sub_bucket: sub-bucket name
-         |      :param string file_name: name of the file to be written
-         |      :return None
-         |  
-         |  write_to_s3_bucket(python_data_object, bucket, sub_bucket, file_name)
-         |      write python objects/variables etc  into S3 bucket
-         |      :param string bucket: bucket name
-         |      :param string sub_bucket: sub-bucket name
-         |      :param string file_name: name of the file to be written
-         |      :return None
-        ```
-        ---
-            
-        
-        ---
-           
-        ### 2. MySQL Connector<a id="MySQL_Connector" name="MySQL_Connector">  
-          
-        **Code Snippet Sample :**  
-        ```python
-        # Query from Custom MySQL Database
-        from custom_utils.connector.mysql import MySQL 
-        user = "***"
-        password = "***"
-        host = "***"
-        port = "***"
-        database = "***"
-        db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}"
-        query = "select * from table_name limit 10"
-        mysql = MySQL(db_string=db_string)
-        df = mysql.get_data(query = query) 
-        ```
-            
-        **MySQL Connector Documentaion**
-        ```
-        class MySQL(builtins.object)
-         |  MySQL(db_string)
-         |  
-         |  MySQL database utility functions
-         |  
-         |  Methods defined here:
-         |  
-         |  __init__(self, db_string)
-         |      initialisation method for MySQL Connector
-         |      :param string db_string: mysql database connection string
-         |  
-         |  dump_data(self, data, table_name, mode='append')
-         |      Execute a query in the mysql table
-         |      :param pd.DataFrame data: dataframe to be appended or replaced
-         |      :param string table_name: name of the the target table
-         |      :param string mode: it can be either replace or append
-         |      :return None
-         |  
-         |  execute_query(self, query)
-         |      Execute a query in the mysql table
-         |      :param string query: query for execution in the table
-         |      :return :
-         |  
-         |  get_data(self, query)
-         |      Fetch data from mysql as a dataframe.
-         |      :param string query: query for fetching data from table
-         |      :return pd.DataFrame data
-        ```
-            
-        ---
-            
-            
-        ### 3.  MongoDB Connector<a id="MongoDB_Connector" name="MongoDB_Connector">
-            
-        **Code Snippet Sample :**  
-        ```python
-        from custom_utils.connector.mongodb import MongoDB
-        uri = "****"
-        db = "***"
-        collection = "****"
-        mongo = MongoDb(uri = uri, db = db)
-        
-        #Reading with pull method
-        data =  mongo.pull_data(collection=collection, list_dict=list_dict)
-        
-        # Reading with fetch method
-        query = {'id': {'$in': [1,2]}}
-        data = mongo.fetch_data(collection, query=query, only_include_keys=["name"])
-        
-        #Writing inot MongoDB
-        mongo.push_data(collection = collection, data = data)
-        
-        #Updating value
-        id_dict = {"id":"2"}
-        set_dict = {"$set": {"name":"ram"}}
-        mongo.update_value(id_dict, set_dict,collection=collection, upsert=True)
-        
-        # Deleting data
-        mongo.delete_data(collection=collection, overall=False, condition_dict= {"id":None})
-        
-        ```
-        
-         **MongoDB Connector Documentaion**
-        ```    
-        class MongoDB(builtins.object)
-         |  MongoDB(db=None, uri=None)
-         |  
-         |  MongoDB utility functions.
-         |  
-         |  Methods defined here:
-         |  
-         |  __init__(self, db=None, uri=None)
-         |      initialisation method for MongoDB connector
-         |      :param str db: database name
-         |      :param str uri: mongo uri string for establishing connection
-         |  
-         |  delete_data(self, collection, db=None, overall=False, condition_dict=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param bool overall : delete whole collection if True
-         |      :param dict condition_dict : query for deletion
-         |      :return:
-         |  
-         |  fetch_data(self, collection, db=None, query={}, only_include_keys=[])
-         |      function to fetch data from the given database and collection on given query
-         |      :param str db : db_name in mongo
-         |      :param str collection: collection name in mongo for database db
-         |      :param dict query : execution query statement; default is {} which means fetch
-         |                         all without any filters
-         |      :param list only_include_keys : list of keys to be included while fetching rows
-         |      :return: pd.DataFrame
-         |  
-         |  fetch_data_sorted(self, collection, db=None, pipeline=[])
-         |      function to fetch data from the given database and collection on given query
-         |      :param str db: db_name in mongo
-         |      :param str collection: collection name in mongo for database db
-         |      :param list pipeline: pipeline required to aggregate
-         |      :return: pd.DataFrame
-         |  
-         |  pull_data(self, list_dict, collection, db=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param list list_dict : query for fetching data
-         |      :return: pd.DataFrame
-         |  
-         |  push_data(self, data, collection, db=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param list/pd.DataFrame data : data to be inserted in the form of
-         |                                      dataframe or list of dictionaries
-         |      :return:
-         |  
-         |  update_value(self, id_dict, set_dict, collection, db=None, upsert=None)
-         |      Function for updating data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param dict id_dict : query for updation
-         |      :param dict set_dict : key and value dictionary to be updated
-         |      :param bool upsert : whether to upsert or just update
-         |      :return:
-         |  
-         |  upsert_json(self, output_json, upsert_keys, collection, db=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param dict output_json : list of dictionaries where each dictionary is
-         |                                a row with keys as column names
-         |      :param list upsert_keys : keys to be upserted
-         |      :return:
-         |  
-         |  ----------------------------------------------------------------------
-        ```
-        ---
-        	
-        ### 4.  BigQuery Connector<a id="BigQuery_Connector" name="BigQuery_Connector">
-            
-        **Code Snippet Sample :**  
-        ```python
-        
-        # Fetching data from BigQuery
-        from custom_utils.connector.bigquery import BigQuery
-        bq = BigQuery(read_big_query_project = "****",
-                            service_account_file_path="***.json")
-        query = "select * from `trellatale.trellDbDump.userLanguages` limit 2"
-        df = bq.get_data(query)
-        
-        # Dumping Dataframe in BigQuery
-        bq.dump_data(database="rahul_temp", table="demo", dataframe=df, mode="append")
-        
-        # Executing any query in BigQuery
-        query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
-        BigQuery.execute_query(query)
-        
-        # Streaming insert in BigQuery
-        row_to_insert = [{"id": 1, "userid": 1, "languageId": 58,
-                     "mode":0,"active":1}]
-        BigQuery.insert_rows_in_bigquery(dataset="rahul_temp", table="Demo", rows_to_insert=row_to_insert)
-        
-        ```
-            
-        **BigQuery Connector Documentaion**
-        ```
-        class BigQuery(builtins.object)
-         |  BigQuery(read_big_query_project, write_big_query_project, service_account_file_path)
-         |  
-         |  BigQuery database utility functions
-         |  
-         |  Methods defined here:
-         |  
-         |  __init__(self, read_big_query_project, write_big_query_project, service_account_file_path)
-         |      initialisation method for BigQuery Connector
-         |      :param str read_big_query_project : project used while reading from BigQuery
-         |      :param str write_big_query_project: project used while writing into BigQuery
-         |      :param str service_account_file_path: project specific BigQuery Credential
-         |  
-         |  dump_data(self, database=None, table=None, dataframe=None, mode='append')
-         |      Dumps data into from BigQuery
-         |      :param string database: target bigquery database
-         |      :param string table: target table name
-         |      :param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery
-         |      :param string mode: it can be either append or replace
-         |  
-         |  execute_query(self, query, query_config=None, timeout=900, max_retries=0, time_interval=5)
-         |      Executes query from from BigQuery table
-         |      :param string query: query for execution
-         |      :param string query_cofig: config for parameterised query
-         |      :param integer timeout : maximum bigquery execution timeout
-         |      :param string max_retries: maximum retries if data is not fetched
-         |      :param integer time_interval : time interval between retries
-         |  
-         |  get_data(self, query=None, query_config=None, max_retries=0, time_interval=5)
-         |      Fetches data from from BigQuery
-         |      :param string query: query for fetching data from table
-         |      :param string query_cofig: config for parameterised query
-         |      :param string max_retries: maximum retries if data is not fetched
-         |      :param integer time_interval : time interval between retries
-         |  
-         |  insert_rows_array(self, dataset=None, table=None, rows_to_insert=None)
-         |      Streaming insert into from BigQuery
-         |      :param string dataset: target bigquery database
-         |      :param string table: target table name
-         |      :param list rows_to_insert: list of dictionaries where each dictionary is a
-         |                                  row with keys as column names
-         |  
-         |  insert_rows_in_bigquery(self, dataset=None, table=None, rows_to_insert=None)
-         |      Streaming insert into from BigQuery
-         |      :param string dataset: target bigquery database
-         |      :param string table: target table name
-         |      :param  rows_to_insert: list of dictionaries where each dictionary is a
-         |                              row with keys as column names
-        ```
-        ---
-        	
-        	
-        ## 3. Configurer<a id="Configurer" name="Configurer">   
-        	
-        ### 1. Profile Decorator<a id="Profile_Decorator" name="Profile_Decorator">    
-            
-        **Code Snippet Sample :**  
-        ```python
-        from custom_utils.configurer.profiler import profiler
-        @profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
-        def product_counter_v3():
-            return [1, 2, 3, 4, 5]
-        ```
-        **Profiler Documentaion**
-        ```python
-        def profiler(output_file=None, sort_by='cumulative', lines_to_print=None, strip_dirs=False):
-            """
-            A time profiler decorator
-        
-            :param str output_file: Path of the output file. If only name of the file is given, it's saved in the current
-            directory. If it's None, the name of the decorated function is used.
-            :param str sort_by: SortKey enum or tuple/list of str/SortKey enum Sorting criteria for the Stats object. For a list
-            of valid string and SortKey refer to: https://docs.python.org/3/library/profile.html#pstats.Stats.sort_stats
-            :param int lines_to_print: Number of lines to print. Default (None) is for all the lines. This is useful in reducing
-            the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
-            the top of the file.
-            :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
-            size of the printout
-            :return: Profile of the decorated function
-            """
-        ```
-        ###  2.  Log Formatter<a id="Log_Formatter" name="Log_Formatter">
-         
-        **Code Snippet Sample :**
-        ```python
-        from custom_utils.configurer.utils import LogFormatter
-        LogFormatter.apply()
-        ```
-            
-        **Log Formatter Documentation**
-        ```
-        class LogFormatter(logging.Formatter):
-            """Log Formatter class for trell ai usage"""
-        
-            __date_format = '%d/%b/%Y:%H:%M:%S %Z'
-        
-            @staticmethod
-            def apply(level=logging.INFO):
-                """
-                Start logging in json format.
-                :return:
-        ```
-        ---
-        	
-        	
-        ## 4. Alerter<a id="Alerter" name="Alerter">    
-        	
-        ###  1.  Slack Alerter<a id="Slack_Alerter" name="Slack_Alerter">  
-            
-            
-        **Code Snippet Sample :**
-        ```
-        from custom_utils.slack_alerter import Alerter
-        try:
-            """Write your code"""
-        except:
-            """Catch exceptions"""
-            Alerter.send_alert(message=message, url=url, userId=userId, send_error=True) 
-        ```
-            
-        **Alerter Documentation :**
-        ```python
-        class Alerter(builtins.object)
-             |  Class for sending alerts and monitoring stats to a slack channel
-             |  
-             |  Static methods defined here:
-             |  
-             |  send_alert(message: str, url: str, user_id: str = None, send_error: bool = False)
-             |      This function send alert to a target channel tagging a user
-             |                         with a alert message and traceback error.
-             |      args:
-             |              message     : Pass the message to be displayed in the channel
-             |              url         : Pass webhook of target channel
-             |              user_id     : Slack user_id of user who needs to be tagged (
-             |              send_error  : This should be set True,
-             |                           if slack_alert is called while catching exception
-             |      returns: Nothing
-             |  
-             |  send_monitoring_stats(start: tuple, stop: tuple, message: str, url: str, user_id: str = None)
-             |      This function send run time and RAM usage for a cronjob
-             |      to a target channel tagging a user with a  message
-             |      
-             |      Args:
-             |              message : Pass the message to be displayed in the channel
-             |              url : Pass webhook of target channel
-             |              user_id : Slack user_id of user who needs to be tagged
-             |              start : this should be set to output of start_monitoring function
-             |              stop : this should be set to output of start_monitoring function
-             |  
-             |  start_monitoring()
-             |      function for initiating monitoring
-             |  
-             |  stop_monitoring()
-             |      function for end monitoring
-             |  
-             |  ----------------------------------------------------------------------
-        ```
-        ---
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
+Provides-Extra: s3
+Provides-Extra: mysql
 Provides-Extra: bigquery
-Provides-Extra: full
 Provides-Extra: mongodb
-Provides-Extra: mysql
-Provides-Extra: s3
+Provides-Extra: slack
+Provides-Extra: full
+License-File: LICENSE
+
+# custom-utils
+Pip Package for Database Connectors, Alerter, Log Formatter etc
+
+
+***
+
+<p float="left">
+  <img src=https://img.shields.io/pypi/v/custom-utils />
+  <img src=https://www.code-inspector.com/project/29426/score/svg />
+  <img src=https://img.shields.io/pypi/dm/custom-utils?logo=Python&style=social /> 
+  <a href="https://github.com/RahulnKumar/custom-utils/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/RahulnKumar/custom-utils"></a>
+</p>
+ 
+
+## Table of Contents
+
+- [custom-utils](#custom-utils)
+  - [Table of Contents](#table-of-contents)
+  - [1.  Installation](#1--installation)
+  - [2. Connector](#2-connector)
+    - [1. S3 Connector](#1-s3-connector)
+    - [2. MySQL Connector](#2-mysql-connector)
+    - [3.  MongoDB Connector](#3--mongodb-connector)
+    - [4.  BigQuery Connector](#4--bigquery-connector)
+  - [3. Configurer](#3-configurer)
+    - [1. Profile Decorator](#1-profile-decorator)
+    - [2.  Log Formatter](#2--log-formatter)
+  - [4. Alerter](#4-alerter)
+    - [1.  Slack Alerter](#1--slack-alerter)
+
+***
+
+## 1.  Installation<a id="1--installation">    
+
+- **Installation from Pypi repository** (Any one)
+	
+    `pip install custom-utils`  --> minimal installation  
+    `pip install custom-utils[full]` --> full installation  
+    `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
+- **Installation from github repository** (Any one)  
+	
+    `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
+    `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
+    `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
+
+<img src="https://i.ibb.co/WHwqTpr/pip-cu.gif" alt="pip-cu" border="0">
+    
+---
+    
+	
+## 2. Connector<a id="2-connector">
+
+    
+### 1. S3 Connector<a id="1-s3-connector">     
+
+**Code Snippet Sample :**
+```python
+## To use S3 either setup AWS CLI or set the credentials from pip package only
+
+## Setup AWS CLI
+sudo apt install awscli && aws configure
+
+## Setup Credentials from pip package
+from custom_utils.configurer.utils import Credential
+Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********")
+
+
+from custom_utils.connector.s3 import S3
+
+# Uplaoding data to S3
+S3.push_local_data(file_path, s3_uri)
+                             
+# Doownlaoding data from S3
+S3.pull_s3_data(file_path, s3_uri)
+```
+
+**S3 Connector Documentation**
+    
+```
+class S3(builtins.object)
+ |  AWS S3 utility functions
+ |  
+ |  Static methods defined here:
+ |  
+ |  pull_python_object(s3_uri)
+ |      read python object stored in S3 bucket
+ |      :param string s3_uri: s3 uri of the object
+ |      :return python_object : python object stored in the S3
+ |  
+ |  pull_s3_data(file_path, s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: target s3 uri
+ |      :param string file_path:  local path of the file 
+ |      :return None
+ |  
+ |  push_local_data(file_path, s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: target s3 uri
+ |      :param string file_path:  local path of the file 
+ |      :return None
+ |  
+ |  push_python_object(python_object, s3_uri)
+ |      write python objects/variables etc  into S3 bucket
+ |      :param string bucket: bucket name
+ |      :param string sub_bucket: sub-bucket name
+ |      :param string file_name: name of the file to be written
+ |      :return None
+ |  
+ |  read_csv(s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: csv file S3 URI
+ |      :return df : pandas dataframe
+ |  
+ |  ----------------------------------------------------------------------
+  
+```
+---
+    
+
+---
+   
+### 2. MySQL Connector<a id="2-mysql-connector">  
+  
+**Code Snippet Sample :**  
+```python
+# Query from Custom MySQL Database
+from custom_utils.connector.mysql import MySQL 
+user = "***"
+password = "***"
+host = "***"
+port = "***"
+database = "***"
+db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}"
+query = "select * from table_name limit 10"
+mysql = MySQL(db_string=db_string)
+df = mysql.pull_data(query = query) 
+```
+    
+**MySQL Connector Documentaion**
+```
+class MySQL(builtins.object)
+ |  MySQL(db_string)
+ |  
+ |  MySQL database utility functions
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, db_string)
+ |      initialisation method for MySQL Connector
+ |      :param string db_string: mysql database connection string
+ |  
+ |  push_data(self, data, table_name, mode='append')
+ |      Execute a query in the mysql table
+ |      :param pd.DataFrame data: dataframe to be appended or replaced
+ |      :param string table_name: name of the the target table
+ |      :param string mode: it can be either replace or append
+ |      :return None
+ |  
+ |  execute_query(self, query)
+ |      Execute a query in the mysql table
+ |      :param string query: query for execution in the table
+ |      :return :
+ |  
+ |  pull_data(self, query)
+ |      Fetch data from mysql as a dataframe.
+ |      :param string query: query for fetching data from table
+ |      :return pd.DataFrame data
+```
+    
+---
+    
+    
+### 3.  MongoDB Connector<a id="3--mongodb-connector">
+    
+**Code Snippet Sample :**  
+```python
+from custom_utils.connector.mongodb import MongoDB
+uri = "****"
+db = "***"
+collection = "****"
+mongo = MongoDb(uri = uri, db = db)
+
+#Reading with pull method
+data =  mongo.pull_data(collection=collection, list_dict=list_dict)
+
+# Reading with fetch method
+query = {'id': {'$in': [1,2]}}
+data = mongo.fetch_data(collection, query=query, only_include_keys=["name"])
+
+#Writing into MongoDB
+mongo.push_data(collection = collection, data = data)
+
+#Updating value
+id_dict = {"id":"2"}
+set_dict = {"$set": {"name":"ram"}}
+mongo.update_value(id_dict, set_dict,collection=collection, upsert=True)
+
+# Deleting data
+mongo.delete_data(collection=collection, overall=False, condition_dict= {"id":None})
+
+```
+
+ **MongoDB Connector Documentaion**
+```    
+class MongoDB(builtins.object)
+ |  MongoDB(db=None, uri=None)
+ |  
+ |  MongoDB utility functions.
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, db=None, uri=None)
+ |      initialisation method for MongoDB connector
+ |      :param str db: database name
+ |      :param str uri: mongo uri string for establishing connection
+ |  
+ |  delete_data(self, collection, db=None, overall=False, condition_dict=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param bool overall : delete whole collection if True
+ |      :param dict condition_dict : query for deletion
+ |      :return:
+ |  
+ |  fetch_data(self, collection, db=None, query={}, only_include_keys=[])
+ |      function to fetch data from the given database and collection on given query
+ |      :param str db : db_name in mongo
+ |      :param str collection: collection name in mongo for database db
+ |      :param dict query : execution query statement; default is {} which means fetch
+ |                         all without any filters
+ |      :param list only_include_keys : list of keys to be included while fetching rows
+ |      :return: pd.DataFrame
+ |  
+ |  fetch_data_sorted(self, collection, db=None, pipeline=[])
+ |      function to fetch data from the given database and collection on given query
+ |      :param str db: db_name in mongo
+ |      :param str collection: collection name in mongo for database db
+ |      :param list pipeline: pipeline required to aggregate
+ |      :return: pd.DataFrame
+ |  
+ |  pull_data(self, list_dict, collection, db=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param list list_dict : query for fetching data
+ |      :return: pd.DataFrame
+ |  
+ |  push_data(self, data, collection, db=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param list/pd.DataFrame data : data to be inserted in the form of
+ |                                      dataframe or list of dictionaries
+ |      :return:
+ |  
+ |  update_value(self, id_dict, set_dict, collection, db=None, upsert=None)
+ |      Function for updating data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param dict id_dict : query for updation
+ |      :param dict set_dict : key and value dictionary to be updated
+ |      :param bool upsert : whether to upsert or just update
+ |      :return:
+ |  
+ |  upsert_json(self, output_json, upsert_keys, collection, db=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param dict output_json : list of dictionaries where each dictionary is
+ |                                a row with keys as column names
+ |      :param list upsert_keys : keys to be upserted
+ |      :return:
+ |  
+ |  ----------------------------------------------------------------------
+```
+---
+	
+### 4.  BigQuery Connector<a id="4--bigquery-connector">
+    
+**Code Snippet Sample :**  
+```python
+
+# Fetching data from BigQuery
+from custom_utils.connector.bigquery import BigQuery
+bq = BigQuery(read_big_query_project = "****",
+                    service_account_file_path="***.json")
+query = "select * from table_name"
+df = bq.pull_data(query)
+
+# Dumping Dataframe in BigQuery
+bq.push_data(database="rahul_temp", table="demo", dataframe=df, mode="append")
+
+# Executing any query in BigQuery
+query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
+BigQuery.execute_query(query)
+
+# Streaming insert in BigQuery
+row_to_insert = [{"id": 1, "userid": 1, "languageId": 58,
+             "mode":0,"active":1}]
+BigQuery.insert_rows_in_bigquery(dataset="rahul_temp", table="Demo", rows_to_insert=row_to_insert)
+
+```
+    
+**BigQuery Connector Documentaion**
+```
+class BigQuery(builtins.object)
+ |  BigQuery(read_big_query_project, write_big_query_project, service_account_file_path)
+ |  
+ |  BigQuery database utility functions
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, read_big_query_project, write_big_query_project, service_account_file_path)
+ |      initialisation method for BigQuery Connector
+ |      :param str read_big_query_project : project used while reading from BigQuery
+ |      :param str write_big_query_project: project used while writing into BigQuery
+ |      :param str service_account_file_path: project specific BigQuery Credential
+ |  
+ |  push_data(self, database=None, table=None, dataframe=None, mode='append')
+ |      Dumps data into from BigQuery
+ |      :param string database: target bigquery database
+ |      :param string table: target table name
+ |      :param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery
+ |      :param string mode: it can be either append or replace
+ |  
+ |  execute_query(self, query, job_config=None, timeout=900, max_retries=0, time_interval=5)
+ |      Executes query from from BigQuery table
+ |      :param string query: query for execution
+ |      :param string query_cofig: config for parameterised query
+ |      :param integer timeout : maximum bigquery execution timeout
+ |      :param string max_retries: maximum retries if data is not fetched
+ |      :param integer time_interval : time interval between retries
+ |  
+ |  pull_data(self, query=None, job_config=None, max_retries=0, time_interval=5)
+ |      Fetches data from from BigQuery
+ |      :param string query: query for fetching data from table
+ |      :param string query_cofig: config for parameterised query
+ |      :param string max_retries: maximum retries if data is not fetched
+ |      :param integer time_interval : time interval between retries
+ |  
+ |  insert_rows_array(self, dataset=None, table=None, rows_to_insert=None)
+ |      Streaming insert into from BigQuery
+ |      :param string dataset: target bigquery database
+ |      :param string table: target table name
+ |      :param list rows_to_insert: list of dictionaries where each dictionary is a
+ |                                  row with keys as column names
+ |  
+ |  insert_rows_in_bigquery(self, dataset=None, table=None, rows_to_insert=None)
+ |      Streaming insert into from BigQuery
+ |      :param string dataset: target bigquery database
+ |      :param string table: target table name
+ |      :param  rows_to_insert: list of dictionaries where each dictionary is a
+ |                              row with keys as column names
+```
+---
+	
+	
+## 3. Configurer<a id="3-configurer">   
+	
+### 1. Profile Decorator<a id="1-profile-decorator">    
+    
+**Code Snippet Sample :**  
+```python
+from custom_utils.configurer.profiler import profiler
+@profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
+def product_counter_v3():
+    return [1, 2, 3, 4, 5]
+```
+**Profiler Documentaion**
+```python
+def profiler(output_file=None, sort_by='cumulative', lines_to_print=None, strip_dirs=False):
+    """
+    A time profiler decorator
+
+    :param str output_file: Path of the output file. If only name of the file is given, it's saved in the current
+    directory. If it's None, the name of the decorated function is used.
+    :param str sort_by: SortKey enum or tuple/list of str/SortKey enum Sorting criteria for the Stats object. For a list
+    of valid string and SortKey refer to: https://docs.python.org/3/library/profile.html#pstats.Stats.sort_stats
+    :param int lines_to_print: Number of lines to print. Default (None) is for all the lines. This is useful in reducing
+    the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
+    the top of the file.
+    :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
+    size of the printout
+    :return: Profile of the decorated function
+    """
+```
+###  2.  Log Formatter<a id="2--log-formatter">
+ 
+**Code Snippet Sample :**
+```python
+from custom_utils.configurer.utils import LogFormatter
+LogFormatter.apply()
+```
+    
+**Log Formatter Documentation**
+```
+class LogFormatter(logging.Formatter):
+    """Log Formatter class for custom-utils package"""
+
+    __date_format = '%d/%b/%Y:%H:%M:%S %Z'
+
+    @staticmethod
+    def apply(level=logging.INFO):
+        """
+        Start logging in json format.
+        :return:
+```
+---
+	
+	
+## 4. Alerter<a id="4-alerter">    
+	
+###  1.  Slack Alerter<a id="1--slack-alerter">  
+    
+    
+**Code Snippet Sample :**
+```python3
+from custom_utils.alerter.slack import Slack
+slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
+channel="#shield"
+message = "testing"
+uids = ["U03PAP8C1RC", "U03PAP8C1RC"]
+slack.send_alert(channel, message, uids)
+```
+    
+**Alerter Documentation :**
+```python
+class Slack(builtins.object)
+ |  Slack(token=None)
+ |
+ |  Class for sending alerts and monitoring stats to a slack channel
+ |
+ |  Methods defined here:
+ |
+ |  __init__(self, token=None)
+ |      Initialize self.  See help(type(self)) for accurate signature.
+ |
+ |  send_alert(self, channel: str, message: str, uids: list = [])
+ |      This function send alert to a target channel tagging a user
+ |                          with a alert message and traceback error.
+ |      args:
+ |          channel     : Name of the channel (ex : #channel_name)
+ |          message     : Pass the message to be displayed in the channel
+ |          uids        : List of Slack user_ids  who needs to be tagged
+ |
+ |      returns: Nothing
+ |
+ |  ----------------------------------------------------------------------
+```
+---
```

#### html2text {}

```diff
@@ -1,69 +1,80 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.2 Summary: Utilities for
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.37 Summary: Utilities for
 database connectors, slack alerter, loggers etc Home-page: https://github.com/
 RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
-rahulnkumar7@gmail.com License: UNKNOWN Description: # custom-utils Pip Package
-for Database Connectors, Alerter, Log Formatter etc ***
+rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
+Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
+mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
+Provides-Extra: full License-File: LICENSE # custom-utils Pip Package for
+Database Connectors, Alerter, Log Formatter etc ***
 [https://img.shields.io/pypi/v/custom-utils] [https://www.code-inspector.com/
 project/29426/score/svg] [https://img.shields.io/pypi/dm/custom-
 utils?logo=Python&style=social] [GitHub_license]
-## Table of Contents - [Installation](#Installation) - [Connector](#Connector)
-- [S3 Connector](#S3_Connector) - [MySQL Connector](#MySQL_Connector) -
-[MongoDB Connector](#MongoDB_Connector) - [BigQuery Connector]
-(#BigQuery_Connector) - [Configurer](#Configurer) - [Log Formatter]
-(#Log_Formatter) - [Profile Decorator](#Profile_Decorator) - [Alerter]
-(#Alerter) - [Slack Alerter](#Slack_Alerter) *** ## 1. Installation-
-**Installation from Pypi repository** (Any one) `pip install custom-utils` --
-> minimal installation `pip install custom-utils[full]` --> full installation
-`pip install custom-utils[s3,mysql,bigquery,mongodb]` --> selective
-installation - **Installation from github repository** (Any one) `pip install
-git+https://github.com/rahulnkumar/custom-utils.git` `pip install git+https://
-github.com/rahulnkumar/custom-utils.git@` `pip install git+https://github.com/
-rahulnkumar/custom-utils.git@` --- ## 2. Connector### 1. S3 Connector**Code
-Snippet Sample :** ```python from custom_utils.connector.s3 import S3 #
-Uplaoding data to S3 demo = {"Name": "Trell", "Age": 4} S3.write_to_s3_bucket
-(python_data_object=demo, bucket='data-science-datas', sub_bucket='models/',
-file_name="demo.pickle") # Doownlaoding data from S3 demo =
-S3.read_from_s3_bucket(bucket='data-science-datas', sub_bucket='models/',
-file_name="demo.pickle") ``` **S3 Connector Documentation** ``` class S3
-(builtins.object) | AWS S3 utility functions | | Static methods defined here: |
-| read_from_s3_bucket(bucket, sub_bucket, file_name) | read data stored in S3
-bucket | :param string bucket: bucket name | :param string sub_bucket: sub-
-bucket name | :param string file_name: name of the file to be read | :return
-old_data : python object stored in the S3 | | upload_data_from_local_to_s3
-(model_file_name, bucket, sub_bucket) | write data stored in local machine into
-S3 bucket from | :param string bucket: bucket name | :param string sub_bucket:
-sub-bucket name | :param string file_name: name of the file to be written | :
-return None | | write_to_s3_bucket(python_data_object, bucket, sub_bucket,
-file_name) | write python objects/variables etc into S3 bucket | :param string
-bucket: bucket name | :param string sub_bucket: sub-bucket name | :param string
-file_name: name of the file to be written | :return None ``` --- --- ### 2.
-MySQL Connector**Code Snippet Sample :** ```python # Query from Custom MySQL
-Database from custom_utils.connector.mysql import MySQL user = "***" password =
-"***" host = "***" port = "***" database = "***" db_string =
-f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}" query =
-"select * from table_name limit 10" mysql = MySQL(db_string=db_string) df =
-mysql.get_data(query = query) ``` **MySQL Connector Documentaion** ``` class
-MySQL(builtins.object) | MySQL(db_string) | | MySQL database utility functions
-| | Methods defined here: | | __init__(self, db_string) | initialisation method
-for MySQL Connector | :param string db_string: mysql database connection string
-| | dump_data(self, data, table_name, mode='append') | Execute a query in the
-mysql table | :param pd.DataFrame data: dataframe to be appended or replaced |
-:param string table_name: name of the the target table | :param string mode: it
-can be either replace or append | :return None | | execute_query(self, query) |
-Execute a query in the mysql table | :param string query: query for execution
-in the table | :return : | | get_data(self, query) | Fetch data from mysql as a
+## Table of Contents - [custom-utils](#custom-utils) - [Table of Contents]
+(#table-of-contents) - [1. Installation](#1--installation) - [2. Connector](#2-
+connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
+mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
+Connector](#4--bigquery-connector) - [3. Configurer](#3-configurer) - [1.
+Profile Decorator](#1-profile-decorator) - [2. Log Formatter](#2--log-
+formatter) - [4. Alerter](#4-alerter) - [1. Slack Alerter](#1--slack-alerter)
+*** ## 1. Installation- **Installation from Pypi repository** (Any one) `pip
+install custom-utils` --> minimal installation `pip install custom-utils[full]`
+--> full installation `pip install custom-utils
+[s3,mysql,bigquery,mongodb,slack]` --> selective installation - **Installation
+from github repository** (Any one) `pip install git+https://github.com/
+rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
+custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
+utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
+Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
+from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
+## Setup Credentials from pip package from custom_utils.configurer.utils import
+Credential Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********") from
+custom_utils.connector.s3 import S3 # Uplaoding data to S3 S3.push_local_data
+(file_path, s3_uri) # Doownlaoding data from S3 S3.pull_s3_data(file_path,
+s3_uri) ``` **S3 Connector Documentation** ``` class S3(builtins.object) | AWS
+S3 utility functions | | Static methods defined here: | | pull_python_object
+(s3_uri) | read python object stored in S3 bucket | :param string s3_uri: s3
+uri of the object | :return python_object : python object stored in the S3 | |
+pull_s3_data(file_path, s3_uri) | write data stored in local machine into S3
+bucket from | :param string s3_uri: target s3 uri | :param string file_path:
+local path of the file | :return None | | push_local_data(file_path, s3_uri) |
+write data stored in local machine into S3 bucket from | :param string s3_uri:
+target s3 uri | :param string file_path: local path of the file | :return None
+| | push_python_object(python_object, s3_uri) | write python objects/variables
+etc into S3 bucket | :param string bucket: bucket name | :param string
+sub_bucket: sub-bucket name | :param string file_name: name of the file to be
+written | :return None | | read_csv(s3_uri) | write data stored in local
+machine into S3 bucket from | :param string s3_uri: csv file S3 URI | :return
+df : pandas dataframe | | -----------------------------------------------------
+----------------- ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :**
+```python # Query from Custom MySQL Database from custom_utils.connector.mysql
+import MySQL user = "***" password = "***" host = "***" port = "***" database =
+"***" db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
+{database}" query = "select * from table_name limit 10" mysql = MySQL
+(db_string=db_string) df = mysql.pull_data(query = query) ``` **MySQL Connector
+Documentaion** ``` class MySQL(builtins.object) | MySQL(db_string) | | MySQL
+database utility functions | | Methods defined here: | | __init__(self,
+db_string) | initialisation method for MySQL Connector | :param string
+db_string: mysql database connection string | | push_data(self, data,
+table_name, mode='append') | Execute a query in the mysql table | :param
+pd.DataFrame data: dataframe to be appended or replaced | :param string
+table_name: name of the the target table | :param string mode: it can be either
+replace or append | :return None | | execute_query(self, query) | Execute a
+query in the mysql table | :param string query: query for execution in the
+table | :return : | | pull_data(self, query) | Fetch data from mysql as a
 dataframe. | :param string query: query for fetching data from table | :return
 pd.DataFrame data ``` --- ### 3. MongoDB Connector**Code Snippet Sample :**
 ```python from custom_utils.connector.mongodb import MongoDB uri = "****" db =
 "***" collection = "****" mongo = MongoDb(uri = uri, db = db) #Reading with
 pull method data = mongo.pull_data(collection=collection, list_dict=list_dict)
 # Reading with fetch method query = {'id': {'$in': [1,2]}} data =
 mongo.fetch_data(collection, query=query, only_include_keys=["name"]) #Writing
-inot MongoDB mongo.push_data(collection = collection, data = data) #Updating
+into MongoDB mongo.push_data(collection = collection, data = data) #Updating
 value id_dict = {"id":"2"} set_dict = {"$set": {"name":"ram"}}
 mongo.update_value(id_dict, set_dict,collection=collection, upsert=True) #
 Deleting data mongo.delete_data(collection=collection, overall=False,
 condition_dict= {"id":None}) ``` **MongoDB Connector Documentaion** ``` class
 MongoDB(builtins.object) | MongoDB(db=None, uri=None) | | MongoDB utility
 functions. | | Methods defined here: | | __init__(self, db=None, uri=None) |
 initialisation method for MongoDB connector | :param str db: database name | :
@@ -98,55 +109,55 @@
 str collection : collection name | :param dict output_json : list of
 dictionaries where each dictionary is | a row with keys as column names | :
 param list upsert_keys : keys to be upserted | :return: | | -------------------
 --------------------------------------------------- ``` --- ### 4. BigQuery
 Connector**Code Snippet Sample :** ```python # Fetching data from BigQuery from
 custom_utils.connector.bigquery import BigQuery bq = BigQuery
 (read_big_query_project = "****", service_account_file_path="***.json") query =
-"select * from `trellatale.trellDbDump.userLanguages` limit 2" df = bq.get_data
-(query) # Dumping Dataframe in BigQuery bq.dump_data(database="rahul_temp",
-table="demo", dataframe=df, mode="append") # Executing any query in BigQuery
-query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
-BigQuery.execute_query(query) # Streaming insert in BigQuery row_to_insert = [
-{"id": 1, "userid": 1, "languageId": 58, "mode":0,"active":1}]
-BigQuery.insert_rows_in_bigquery(dataset="rahul_temp", table="Demo",
-rows_to_insert=row_to_insert) ``` **BigQuery Connector Documentaion** ``` class
-BigQuery(builtins.object) | BigQuery(read_big_query_project,
-write_big_query_project, service_account_file_path) | | BigQuery database
-utility functions | | Methods defined here: | | __init__(self,
-read_big_query_project, write_big_query_project, service_account_file_path) |
-initialisation method for BigQuery Connector | :param str
-read_big_query_project : project used while reading from BigQuery | :param str
-write_big_query_project: project used while writing into BigQuery | :param str
-service_account_file_path: project specific BigQuery Credential | | dump_data
-(self, database=None, table=None, dataframe=None, mode='append') | Dumps data
-into from BigQuery | :param string database: target bigquery database | :param
-string table: target table name | :param pd.DataFrame dataframe: pandas
-dataframe for dumping into bigquery | :param string mode: it can be either
-append or replace | | execute_query(self, query, query_config=None,
-timeout=900, max_retries=0, time_interval=5) | Executes query from from
-BigQuery table | :param string query: query for execution | :param string
-query_cofig: config for parameterised query | :param integer timeout : maximum
-bigquery execution timeout | :param string max_retries: maximum retries if data
-is not fetched | :param integer time_interval : time interval between retries |
-| get_data(self, query=None, query_config=None, max_retries=0, time_interval=5)
-| Fetches data from from BigQuery | :param string query: query for fetching
-data from table | :param string query_cofig: config for parameterised query | :
-param string max_retries: maximum retries if data is not fetched | :param
-integer time_interval : time interval between retries | | insert_rows_array
-(self, dataset=None, table=None, rows_to_insert=None) | Streaming insert into
-from BigQuery | :param string dataset: target bigquery database | :param string
-table: target table name | :param list rows_to_insert: list of dictionaries
-where each dictionary is a | row with keys as column names | |
-insert_rows_in_bigquery(self, dataset=None, table=None, rows_to_insert=None) |
-Streaming insert into from BigQuery | :param string dataset: target bigquery
-database | :param string table: target table name | :param rows_to_insert: list
-of dictionaries where each dictionary is a | row with keys as column names ```
---- ## 3. Configurer### 1. Profile Decorator**Code Snippet Sample :** ```python
-from custom_utils.configurer.profiler import profiler @profiler
+"select * from table_name" df = bq.pull_data(query) # Dumping Dataframe in
+BigQuery bq.push_data(database="rahul_temp", table="demo", dataframe=df,
+mode="append") # Executing any query in BigQuery query = "INSERT
+rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)" BigQuery.execute_query(query) #
+Streaming insert in BigQuery row_to_insert = [{"id": 1, "userid": 1,
+"languageId": 58, "mode":0,"active":1}] BigQuery.insert_rows_in_bigquery
+(dataset="rahul_temp", table="Demo", rows_to_insert=row_to_insert) ```
+**BigQuery Connector Documentaion** ``` class BigQuery(builtins.object) |
+BigQuery(read_big_query_project, write_big_query_project,
+service_account_file_path) | | BigQuery database utility functions | | Methods
+defined here: | | __init__(self, read_big_query_project,
+write_big_query_project, service_account_file_path) | initialisation method for
+BigQuery Connector | :param str read_big_query_project : project used while
+reading from BigQuery | :param str write_big_query_project: project used while
+writing into BigQuery | :param str service_account_file_path: project specific
+BigQuery Credential | | push_data(self, database=None, table=None,
+dataframe=None, mode='append') | Dumps data into from BigQuery | :param string
+database: target bigquery database | :param string table: target table name | :
+param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery | :
+param string mode: it can be either append or replace | | execute_query(self,
+query, job_config=None, timeout=900, max_retries=0, time_interval=5) | Executes
+query from from BigQuery table | :param string query: query for execution | :
+param string query_cofig: config for parameterised query | :param integer
+timeout : maximum bigquery execution timeout | :param string max_retries:
+maximum retries if data is not fetched | :param integer time_interval : time
+interval between retries | | pull_data(self, query=None, job_config=None,
+max_retries=0, time_interval=5) | Fetches data from from BigQuery | :param
+string query: query for fetching data from table | :param string query_cofig:
+config for parameterised query | :param string max_retries: maximum retries if
+data is not fetched | :param integer time_interval : time interval between
+retries | | insert_rows_array(self, dataset=None, table=None,
+rows_to_insert=None) | Streaming insert into from BigQuery | :param string
+dataset: target bigquery database | :param string table: target table name | :
+param list rows_to_insert: list of dictionaries where each dictionary is a |
+row with keys as column names | | insert_rows_in_bigquery(self, dataset=None,
+table=None, rows_to_insert=None) | Streaming insert into from BigQuery | :param
+string dataset: target bigquery database | :param string table: target table
+name | :param rows_to_insert: list of dictionaries where each dictionary is a |
+row with keys as column names ``` --- ## 3. Configurer### 1. Profile
+Decorator**Code Snippet Sample :** ```python from
+custom_utils.configurer.profiler import profiler @profiler
 (sort_by='cumulative', lines_to_print=10, strip_dirs=True) def
 product_counter_v3(): return [1, 2, 3, 4, 5] ``` **Profiler Documentaion**
 ```python def profiler(output_file=None, sort_by='cumulative',
 lines_to_print=None, strip_dirs=False): """ A time profiler decorator :param
 str output_file: Path of the output file. If only name of the file is given,
 it's saved in the current directory. If it's None, the name of the decorated
 function is used. :param str sort_by: SortKey enum or tuple/list of str/SortKey
@@ -157,36 +168,24 @@
 size of the printout, especially that sorting by 'cumulative', the time
 consuming operations are printed toward the top of the file. :param bool
 strip_dirs: Whether to remove the leading path info from file names. This is
 also useful in reducing the size of the printout :return: Profile of the
 decorated function """ ``` ### 2. Log Formatter**Code Snippet Sample :**
 ```python from custom_utils.configurer.utils import LogFormatter
 LogFormatter.apply() ``` **Log Formatter Documentation** ``` class LogFormatter
-(logging.Formatter): """Log Formatter class for trell ai usage""" __date_format
-= '%d/%b/%Y:%H:%M:%S %Z' @staticmethod def apply(level=logging.INFO): """ Start
-logging in json format. :return: ``` --- ## 4. Alerter### 1. Slack
-Alerter**Code Snippet Sample :** ``` from custom_utils.slack_alerter import
-Alerter try: """Write your code""" except: """Catch exceptions"""
-Alerter.send_alert(message=message, url=url, userId=userId, send_error=True)
-``` **Alerter Documentation :** ```python class Alerter(builtins.object) |
-Class for sending alerts and monitoring stats to a slack channel | | Static
-methods defined here: | | send_alert(message: str, url: str, user_id: str =
-None, send_error: bool = False) | This function send alert to a target channel
-tagging a user | with a alert message and traceback error. | args: | message :
-Pass the message to be displayed in the channel | url : Pass webhook of target
-channel | user_id : Slack user_id of user who needs to be tagged ( | send_error
-: This should be set True, | if slack_alert is called while catching exception
-| returns: Nothing | | send_monitoring_stats(start: tuple, stop: tuple,
-message: str, url: str, user_id: str = None) | This function send run time and
-RAM usage for a cronjob | to a target channel tagging a user with a message | |
-Args: | message : Pass the message to be displayed in the channel | url : Pass
-webhook of target channel | user_id : Slack user_id of user who needs to be
-tagged | start : this should be set to output of start_monitoring function |
-stop : this should be set to output of start_monitoring function | |
-start_monitoring() | function for initiating monitoring | | stop_monitoring() |
-function for end monitoring | | -----------------------------------------------
------------------------ ``` --- Platform: UNKNOWN Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6.9 Description-Content-Type: text/markdown Provides-
-Extra: bigquery Provides-Extra: full Provides-Extra: mongodb Provides-Extra:
-mysql Provides-Extra: s3
+(logging.Formatter): """Log Formatter class for custom-utils package"""
+__date_format = '%d/%b/%Y:%H:%M:%S %Z' @staticmethod def apply
+(level=logging.INFO): """ Start logging in json format. :return: ``` --- ## 4.
+Alerter### 1. Slack Alerter**Code Snippet Sample :** ```python3 from
+custom_utils.alerter.slack import Slack slack = Slack(token=SLACK_BOT_TOKEN) #
+OR Slack() with SLACK_BOT_TOKEN as env variable channel="#shield" message =
+"testing" uids = ["U03PAP8C1RC", "U03PAP8C1RC"] slack.send_alert(channel,
+message, uids) ``` **Alerter Documentation :** ```python class Slack
+(builtins.object) | Slack(token=None) | | Class for sending alerts and
+monitoring stats to a slack channel | | Methods defined here: | | __init__
+(self, token=None) | Initialize self. See help(type(self)) for accurate
+signature. | | send_alert(self, channel: str, message: str, uids: list = []) |
+This function send alert to a target channel tagging a user | with a alert
+message and traceback error. | args: | channel : Name of the channel (ex :
+#channel_name) | message : Pass the message to be displayed in the channel |
+uids : List of Slack user_ids who needs to be tagged | | returns: Nothing | | -
+--------------------------------------------------------------------- ``` ---
```

### Comparing `custom-utils-0.0.2/README.md` & `custom-utils-0.0.37/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -10,117 +10,134 @@
   <img src=https://img.shields.io/pypi/dm/custom-utils?logo=Python&style=social /> 
   <a href="https://github.com/RahulnKumar/custom-utils/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/RahulnKumar/custom-utils"></a>
 </p>
  
 
 ## Table of Contents
 
-- [Installation](#Installation)
-- [Connector](#Connector)
-  - [S3 Connector](#S3_Connector)
-  - [MySQL Connector](#MySQL_Connector)
-  - [MongoDB Connector](#MongoDB_Connector)
-  - [BigQuery Connector](#BigQuery_Connector)
- 
-- [Configurer](#Configurer)
-  - [Log Formatter](#Log_Formatter)
-  - [Profile Decorator](#Profile_Decorator)
-  
-- [Alerter](#Alerter)
-  - [Slack Alerter](#Slack_Alerter)
+- [custom-utils](#custom-utils)
+  - [Table of Contents](#table-of-contents)
+  - [1.  Installation](#1--installation)
+  - [2. Connector](#2-connector)
+    - [1. S3 Connector](#1-s3-connector)
+    - [2. MySQL Connector](#2-mysql-connector)
+    - [3.  MongoDB Connector](#3--mongodb-connector)
+    - [4.  BigQuery Connector](#4--bigquery-connector)
+  - [3. Configurer](#3-configurer)
+    - [1. Profile Decorator](#1-profile-decorator)
+    - [2.  Log Formatter](#2--log-formatter)
+  - [4. Alerter](#4-alerter)
+    - [1.  Slack Alerter](#1--slack-alerter)
 
 ***
 
-## 1.  Installation<a id="Installation" name="Installation">    
+## 1.  Installation<a id="1--installation">    
 
 - **Installation from Pypi repository** (Any one)
 	
     `pip install custom-utils`  --> minimal installation  
     `pip install custom-utils[full]` --> full installation  
-    `pip install custom-utils[s3,mysql,bigquery,mongodb]`  --> selective installation 
+    `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
 - **Installation from github repository** (Any one)  
 	
     `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
     `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
+
+<img src="https://i.ibb.co/WHwqTpr/pip-cu.gif" alt="pip-cu" border="0">
     
 ---
     
 	
-## 2. Connector<a id="Connector" name="Connector">
+## 2. Connector<a id="2-connector">
 
     
-### 1. S3 Connector<a id="S3_Connector" name="S3_Connector">     
+### 1. S3 Connector<a id="1-s3-connector">     
 
 **Code Snippet Sample :**
 ```python
+## To use S3 either setup AWS CLI or set the credentials from pip package only
+
+## Setup AWS CLI
+sudo apt install awscli && aws configure
+
+## Setup Credentials from pip package
+from custom_utils.configurer.utils import Credential
+Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********")
+
+
 from custom_utils.connector.s3 import S3
 
 # Uplaoding data to S3
-demo = {"Name": "Trell", "Age": 4}
-S3.write_to_s3_bucket(python_data_object=demo,
-                             bucket='data-science-datas',
-                             sub_bucket='models/', file_name="demo.pickle")
+S3.push_local_data(file_path, s3_uri)
                              
 # Doownlaoding data from S3
-
-demo = S3.read_from_s3_bucket(bucket='data-science-datas',          
-                                         sub_bucket='models/',
-                                         file_name="demo.pickle")
+S3.pull_s3_data(file_path, s3_uri)
 ```
 
 **S3 Connector Documentation**
     
 ```
 class S3(builtins.object)
  |  AWS S3 utility functions
  |  
  |  Static methods defined here:
  |  
- |  read_from_s3_bucket(bucket, sub_bucket, file_name)
- |      read data stored in S3 bucket
- |      :param string bucket: bucket name
- |      :param string sub_bucket: sub-bucket name
- |      :param string file_name: name of the file to be read
- |      :return old_data : python object stored in the S3
+ |  pull_python_object(s3_uri)
+ |      read python object stored in S3 bucket
+ |      :param string s3_uri: s3 uri of the object
+ |      :return python_object : python object stored in the S3
  |  
- |  upload_data_from_local_to_s3(model_file_name, bucket, sub_bucket)
+ |  pull_s3_data(file_path, s3_uri)
  |      write data stored in local machine into S3 bucket from
- |      :param string bucket: bucket name
- |      :param string sub_bucket: sub-bucket name
- |      :param string file_name: name of the file to be written
+ |      :param string s3_uri: target s3 uri
+ |      :param string file_path:  local path of the file 
+ |      :return None
+ |  
+ |  push_local_data(file_path, s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: target s3 uri
+ |      :param string file_path:  local path of the file 
  |      :return None
  |  
- |  write_to_s3_bucket(python_data_object, bucket, sub_bucket, file_name)
+ |  push_python_object(python_object, s3_uri)
  |      write python objects/variables etc  into S3 bucket
  |      :param string bucket: bucket name
  |      :param string sub_bucket: sub-bucket name
  |      :param string file_name: name of the file to be written
  |      :return None
+ |  
+ |  read_csv(s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: csv file S3 URI
+ |      :return df : pandas dataframe
+ |  
+ |  ----------------------------------------------------------------------
+  
 ```
 ---
     
 
 ---
    
-### 2. MySQL Connector<a id="MySQL_Connector" name="MySQL_Connector">  
+### 2. MySQL Connector<a id="2-mysql-connector">  
   
 **Code Snippet Sample :**  
 ```python
 # Query from Custom MySQL Database
 from custom_utils.connector.mysql import MySQL 
 user = "***"
 password = "***"
 host = "***"
 port = "***"
 database = "***"
 db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}"
 query = "select * from table_name limit 10"
 mysql = MySQL(db_string=db_string)
-df = mysql.get_data(query = query) 
+df = mysql.pull_data(query = query) 
 ```
     
 **MySQL Connector Documentaion**
 ```
 class MySQL(builtins.object)
  |  MySQL(db_string)
  |  
@@ -128,36 +145,36 @@
  |  
  |  Methods defined here:
  |  
  |  __init__(self, db_string)
  |      initialisation method for MySQL Connector
  |      :param string db_string: mysql database connection string
  |  
- |  dump_data(self, data, table_name, mode='append')
+ |  push_data(self, data, table_name, mode='append')
  |      Execute a query in the mysql table
  |      :param pd.DataFrame data: dataframe to be appended or replaced
  |      :param string table_name: name of the the target table
  |      :param string mode: it can be either replace or append
  |      :return None
  |  
  |  execute_query(self, query)
  |      Execute a query in the mysql table
  |      :param string query: query for execution in the table
  |      :return :
  |  
- |  get_data(self, query)
+ |  pull_data(self, query)
  |      Fetch data from mysql as a dataframe.
  |      :param string query: query for fetching data from table
  |      :return pd.DataFrame data
 ```
     
 ---
     
     
-### 3.  MongoDB Connector<a id="MongoDB_Connector" name="MongoDB_Connector">
+### 3.  MongoDB Connector<a id="3--mongodb-connector">
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.connector.mongodb import MongoDB
 uri = "****"
 db = "***"
 collection = "****"
@@ -166,15 +183,15 @@
 #Reading with pull method
 data =  mongo.pull_data(collection=collection, list_dict=list_dict)
 
 # Reading with fetch method
 query = {'id': {'$in': [1,2]}}
 data = mongo.fetch_data(collection, query=query, only_include_keys=["name"])
 
-#Writing inot MongoDB
+#Writing into MongoDB
 mongo.push_data(collection = collection, data = data)
 
 #Updating value
 id_dict = {"id":"2"}
 set_dict = {"$set": {"name":"ram"}}
 mongo.update_value(id_dict, set_dict,collection=collection, upsert=True)
 
@@ -254,28 +271,28 @@
  |      :param list upsert_keys : keys to be upserted
  |      :return:
  |  
  |  ----------------------------------------------------------------------
 ```
 ---
 	
-### 4.  BigQuery Connector<a id="BigQuery_Connector" name="BigQuery_Connector">
+### 4.  BigQuery Connector<a id="4--bigquery-connector">
     
 **Code Snippet Sample :**  
 ```python
 
 # Fetching data from BigQuery
 from custom_utils.connector.bigquery import BigQuery
 bq = BigQuery(read_big_query_project = "****",
                     service_account_file_path="***.json")
-query = "select * from `trellatale.trellDbDump.userLanguages` limit 2"
-df = bq.get_data(query)
+query = "select * from table_name"
+df = bq.pull_data(query)
 
 # Dumping Dataframe in BigQuery
-bq.dump_data(database="rahul_temp", table="demo", dataframe=df, mode="append")
+bq.push_data(database="rahul_temp", table="demo", dataframe=df, mode="append")
 
 # Executing any query in BigQuery
 query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
 BigQuery.execute_query(query)
 
 # Streaming insert in BigQuery
 row_to_insert = [{"id": 1, "userid": 1, "languageId": 58,
@@ -295,30 +312,30 @@
  |  
  |  __init__(self, read_big_query_project, write_big_query_project, service_account_file_path)
  |      initialisation method for BigQuery Connector
  |      :param str read_big_query_project : project used while reading from BigQuery
  |      :param str write_big_query_project: project used while writing into BigQuery
  |      :param str service_account_file_path: project specific BigQuery Credential
  |  
- |  dump_data(self, database=None, table=None, dataframe=None, mode='append')
+ |  push_data(self, database=None, table=None, dataframe=None, mode='append')
  |      Dumps data into from BigQuery
  |      :param string database: target bigquery database
  |      :param string table: target table name
  |      :param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery
  |      :param string mode: it can be either append or replace
  |  
- |  execute_query(self, query, query_config=None, timeout=900, max_retries=0, time_interval=5)
+ |  execute_query(self, query, job_config=None, timeout=900, max_retries=0, time_interval=5)
  |      Executes query from from BigQuery table
  |      :param string query: query for execution
  |      :param string query_cofig: config for parameterised query
  |      :param integer timeout : maximum bigquery execution timeout
  |      :param string max_retries: maximum retries if data is not fetched
  |      :param integer time_interval : time interval between retries
  |  
- |  get_data(self, query=None, query_config=None, max_retries=0, time_interval=5)
+ |  pull_data(self, query=None, job_config=None, max_retries=0, time_interval=5)
  |      Fetches data from from BigQuery
  |      :param string query: query for fetching data from table
  |      :param string query_cofig: config for parameterised query
  |      :param string max_retries: maximum retries if data is not fetched
  |      :param integer time_interval : time interval between retries
  |  
  |  insert_rows_array(self, dataset=None, table=None, rows_to_insert=None)
@@ -334,17 +351,17 @@
  |      :param string table: target table name
  |      :param  rows_to_insert: list of dictionaries where each dictionary is a
  |                              row with keys as column names
 ```
 ---
 	
 	
-## 3. Configurer<a id="Configurer" name="Configurer">   
+## 3. Configurer<a id="3-configurer">   
 	
-### 1. Profile Decorator<a id="Profile_Decorator" name="Profile_Decorator">    
+### 1. Profile Decorator<a id="1-profile-decorator">    
     
 **Code Snippet Sample :**  
 ```python
 from custom_utils.configurer.profiler import profiler
 @profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
 def product_counter_v3():
     return [1, 2, 3, 4, 5]
@@ -363,84 +380,71 @@
     the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
     the top of the file.
     :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
     size of the printout
     :return: Profile of the decorated function
     """
 ```
-###  2.  Log Formatter<a id="Log_Formatter" name="Log_Formatter">
+###  2.  Log Formatter<a id="2--log-formatter">
  
 **Code Snippet Sample :**
 ```python
 from custom_utils.configurer.utils import LogFormatter
 LogFormatter.apply()
 ```
     
 **Log Formatter Documentation**
 ```
 class LogFormatter(logging.Formatter):
-    """Log Formatter class for trell ai usage"""
+    """Log Formatter class for custom-utils package"""
 
     __date_format = '%d/%b/%Y:%H:%M:%S %Z'
 
     @staticmethod
     def apply(level=logging.INFO):
         """
         Start logging in json format.
         :return:
 ```
 ---
 	
 	
-## 4. Alerter<a id="Alerter" name="Alerter">    
+## 4. Alerter<a id="4-alerter">    
 	
-###  1.  Slack Alerter<a id="Slack_Alerter" name="Slack_Alerter">  
+###  1.  Slack Alerter<a id="1--slack-alerter">  
     
     
 **Code Snippet Sample :**
-```
-from custom_utils.slack_alerter import Alerter
-try:
-    """Write your code"""
-except:
-    """Catch exceptions"""
-    Alerter.send_alert(message=message, url=url, userId=userId, send_error=True) 
+```python3
+from custom_utils.alerter.slack import Slack
+slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
+channel="#shield"
+message = "testing"
+uids = ["U03PAP8C1RC", "U03PAP8C1RC"]
+slack.send_alert(channel, message, uids)
 ```
     
 **Alerter Documentation :**
 ```python
-class Alerter(builtins.object)
-     |  Class for sending alerts and monitoring stats to a slack channel
-     |  
-     |  Static methods defined here:
-     |  
-     |  send_alert(message: str, url: str, user_id: str = None, send_error: bool = False)
-     |      This function send alert to a target channel tagging a user
-     |                         with a alert message and traceback error.
-     |      args:
-     |              message     : Pass the message to be displayed in the channel
-     |              url         : Pass webhook of target channel
-     |              user_id     : Slack user_id of user who needs to be tagged (
-     |              send_error  : This should be set True,
-     |                           if slack_alert is called while catching exception
-     |      returns: Nothing
-     |  
-     |  send_monitoring_stats(start: tuple, stop: tuple, message: str, url: str, user_id: str = None)
-     |      This function send run time and RAM usage for a cronjob
-     |      to a target channel tagging a user with a  message
-     |      
-     |      Args:
-     |              message : Pass the message to be displayed in the channel
-     |              url : Pass webhook of target channel
-     |              user_id : Slack user_id of user who needs to be tagged
-     |              start : this should be set to output of start_monitoring function
-     |              stop : this should be set to output of start_monitoring function
-     |  
-     |  start_monitoring()
-     |      function for initiating monitoring
-     |  
-     |  stop_monitoring()
-     |      function for end monitoring
-     |  
-     |  ----------------------------------------------------------------------
+class Slack(builtins.object)
+ |  Slack(token=None)
+ |
+ |  Class for sending alerts and monitoring stats to a slack channel
+ |
+ |  Methods defined here:
+ |
+ |  __init__(self, token=None)
+ |      Initialize self.  See help(type(self)) for accurate signature.
+ |
+ |  send_alert(self, channel: str, message: str, uids: list = [])
+ |      This function send alert to a target channel tagging a user
+ |                          with a alert message and traceback error.
+ |      args:
+ |          channel     : Name of the channel (ex : #channel_name)
+ |          message     : Pass the message to be displayed in the channel
+ |          uids        : List of Slack user_ids  who needs to be tagged
+ |
+ |      returns: Nothing
+ |
+ |  ----------------------------------------------------------------------
 ```
 ---
```

#### html2text {}

```diff
@@ -1,66 +1,72 @@
 # custom-utils Pip Package for Database Connectors, Alerter, Log Formatter etc
 ***
 [https://img.shields.io/pypi/v/custom-utils] [https://www.code-inspector.com/
 project/29426/score/svg] [https://img.shields.io/pypi/dm/custom-
 utils?logo=Python&style=social] [GitHub_license]
-## Table of Contents - [Installation](#Installation) - [Connector](#Connector)
-- [S3 Connector](#S3_Connector) - [MySQL Connector](#MySQL_Connector) -
-[MongoDB Connector](#MongoDB_Connector) - [BigQuery Connector]
-(#BigQuery_Connector) - [Configurer](#Configurer) - [Log Formatter]
-(#Log_Formatter) - [Profile Decorator](#Profile_Decorator) - [Alerter]
-(#Alerter) - [Slack Alerter](#Slack_Alerter) *** ## 1. Installation-
-**Installation from Pypi repository** (Any one) `pip install custom-utils` --
-> minimal installation `pip install custom-utils[full]` --> full installation
-`pip install custom-utils[s3,mysql,bigquery,mongodb]` --> selective
-installation - **Installation from github repository** (Any one) `pip install
-git+https://github.com/rahulnkumar/custom-utils.git` `pip install git+https://
-github.com/rahulnkumar/custom-utils.git@` `pip install git+https://github.com/
-rahulnkumar/custom-utils.git@` --- ## 2. Connector### 1. S3 Connector**Code
-Snippet Sample :** ```python from custom_utils.connector.s3 import S3 #
-Uplaoding data to S3 demo = {"Name": "Trell", "Age": 4} S3.write_to_s3_bucket
-(python_data_object=demo, bucket='data-science-datas', sub_bucket='models/',
-file_name="demo.pickle") # Doownlaoding data from S3 demo =
-S3.read_from_s3_bucket(bucket='data-science-datas', sub_bucket='models/',
-file_name="demo.pickle") ``` **S3 Connector Documentation** ``` class S3
-(builtins.object) | AWS S3 utility functions | | Static methods defined here: |
-| read_from_s3_bucket(bucket, sub_bucket, file_name) | read data stored in S3
-bucket | :param string bucket: bucket name | :param string sub_bucket: sub-
-bucket name | :param string file_name: name of the file to be read | :return
-old_data : python object stored in the S3 | | upload_data_from_local_to_s3
-(model_file_name, bucket, sub_bucket) | write data stored in local machine into
-S3 bucket from | :param string bucket: bucket name | :param string sub_bucket:
-sub-bucket name | :param string file_name: name of the file to be written | :
-return None | | write_to_s3_bucket(python_data_object, bucket, sub_bucket,
-file_name) | write python objects/variables etc into S3 bucket | :param string
-bucket: bucket name | :param string sub_bucket: sub-bucket name | :param string
-file_name: name of the file to be written | :return None ``` --- --- ### 2.
-MySQL Connector**Code Snippet Sample :** ```python # Query from Custom MySQL
-Database from custom_utils.connector.mysql import MySQL user = "***" password =
-"***" host = "***" port = "***" database = "***" db_string =
-f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}" query =
-"select * from table_name limit 10" mysql = MySQL(db_string=db_string) df =
-mysql.get_data(query = query) ``` **MySQL Connector Documentaion** ``` class
-MySQL(builtins.object) | MySQL(db_string) | | MySQL database utility functions
-| | Methods defined here: | | __init__(self, db_string) | initialisation method
-for MySQL Connector | :param string db_string: mysql database connection string
-| | dump_data(self, data, table_name, mode='append') | Execute a query in the
-mysql table | :param pd.DataFrame data: dataframe to be appended or replaced |
-:param string table_name: name of the the target table | :param string mode: it
-can be either replace or append | :return None | | execute_query(self, query) |
-Execute a query in the mysql table | :param string query: query for execution
-in the table | :return : | | get_data(self, query) | Fetch data from mysql as a
+## Table of Contents - [custom-utils](#custom-utils) - [Table of Contents]
+(#table-of-contents) - [1. Installation](#1--installation) - [2. Connector](#2-
+connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
+mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
+Connector](#4--bigquery-connector) - [3. Configurer](#3-configurer) - [1.
+Profile Decorator](#1-profile-decorator) - [2. Log Formatter](#2--log-
+formatter) - [4. Alerter](#4-alerter) - [1. Slack Alerter](#1--slack-alerter)
+*** ## 1. Installation- **Installation from Pypi repository** (Any one) `pip
+install custom-utils` --> minimal installation `pip install custom-utils[full]`
+--> full installation `pip install custom-utils
+[s3,mysql,bigquery,mongodb,slack]` --> selective installation - **Installation
+from github repository** (Any one) `pip install git+https://github.com/
+rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
+custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
+utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
+Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
+from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
+## Setup Credentials from pip package from custom_utils.configurer.utils import
+Credential Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********") from
+custom_utils.connector.s3 import S3 # Uplaoding data to S3 S3.push_local_data
+(file_path, s3_uri) # Doownlaoding data from S3 S3.pull_s3_data(file_path,
+s3_uri) ``` **S3 Connector Documentation** ``` class S3(builtins.object) | AWS
+S3 utility functions | | Static methods defined here: | | pull_python_object
+(s3_uri) | read python object stored in S3 bucket | :param string s3_uri: s3
+uri of the object | :return python_object : python object stored in the S3 | |
+pull_s3_data(file_path, s3_uri) | write data stored in local machine into S3
+bucket from | :param string s3_uri: target s3 uri | :param string file_path:
+local path of the file | :return None | | push_local_data(file_path, s3_uri) |
+write data stored in local machine into S3 bucket from | :param string s3_uri:
+target s3 uri | :param string file_path: local path of the file | :return None
+| | push_python_object(python_object, s3_uri) | write python objects/variables
+etc into S3 bucket | :param string bucket: bucket name | :param string
+sub_bucket: sub-bucket name | :param string file_name: name of the file to be
+written | :return None | | read_csv(s3_uri) | write data stored in local
+machine into S3 bucket from | :param string s3_uri: csv file S3 URI | :return
+df : pandas dataframe | | -----------------------------------------------------
+----------------- ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :**
+```python # Query from Custom MySQL Database from custom_utils.connector.mysql
+import MySQL user = "***" password = "***" host = "***" port = "***" database =
+"***" db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
+{database}" query = "select * from table_name limit 10" mysql = MySQL
+(db_string=db_string) df = mysql.pull_data(query = query) ``` **MySQL Connector
+Documentaion** ``` class MySQL(builtins.object) | MySQL(db_string) | | MySQL
+database utility functions | | Methods defined here: | | __init__(self,
+db_string) | initialisation method for MySQL Connector | :param string
+db_string: mysql database connection string | | push_data(self, data,
+table_name, mode='append') | Execute a query in the mysql table | :param
+pd.DataFrame data: dataframe to be appended or replaced | :param string
+table_name: name of the the target table | :param string mode: it can be either
+replace or append | :return None | | execute_query(self, query) | Execute a
+query in the mysql table | :param string query: query for execution in the
+table | :return : | | pull_data(self, query) | Fetch data from mysql as a
 dataframe. | :param string query: query for fetching data from table | :return
 pd.DataFrame data ``` --- ### 3. MongoDB Connector**Code Snippet Sample :**
 ```python from custom_utils.connector.mongodb import MongoDB uri = "****" db =
 "***" collection = "****" mongo = MongoDb(uri = uri, db = db) #Reading with
 pull method data = mongo.pull_data(collection=collection, list_dict=list_dict)
 # Reading with fetch method query = {'id': {'$in': [1,2]}} data =
 mongo.fetch_data(collection, query=query, only_include_keys=["name"]) #Writing
-inot MongoDB mongo.push_data(collection = collection, data = data) #Updating
+into MongoDB mongo.push_data(collection = collection, data = data) #Updating
 value id_dict = {"id":"2"} set_dict = {"$set": {"name":"ram"}}
 mongo.update_value(id_dict, set_dict,collection=collection, upsert=True) #
 Deleting data mongo.delete_data(collection=collection, overall=False,
 condition_dict= {"id":None}) ``` **MongoDB Connector Documentaion** ``` class
 MongoDB(builtins.object) | MongoDB(db=None, uri=None) | | MongoDB utility
 functions. | | Methods defined here: | | __init__(self, db=None, uri=None) |
 initialisation method for MongoDB connector | :param str db: database name | :
@@ -95,55 +101,55 @@
 str collection : collection name | :param dict output_json : list of
 dictionaries where each dictionary is | a row with keys as column names | :
 param list upsert_keys : keys to be upserted | :return: | | -------------------
 --------------------------------------------------- ``` --- ### 4. BigQuery
 Connector**Code Snippet Sample :** ```python # Fetching data from BigQuery from
 custom_utils.connector.bigquery import BigQuery bq = BigQuery
 (read_big_query_project = "****", service_account_file_path="***.json") query =
-"select * from `trellatale.trellDbDump.userLanguages` limit 2" df = bq.get_data
-(query) # Dumping Dataframe in BigQuery bq.dump_data(database="rahul_temp",
-table="demo", dataframe=df, mode="append") # Executing any query in BigQuery
-query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
-BigQuery.execute_query(query) # Streaming insert in BigQuery row_to_insert = [
-{"id": 1, "userid": 1, "languageId": 58, "mode":0,"active":1}]
-BigQuery.insert_rows_in_bigquery(dataset="rahul_temp", table="Demo",
-rows_to_insert=row_to_insert) ``` **BigQuery Connector Documentaion** ``` class
-BigQuery(builtins.object) | BigQuery(read_big_query_project,
-write_big_query_project, service_account_file_path) | | BigQuery database
-utility functions | | Methods defined here: | | __init__(self,
-read_big_query_project, write_big_query_project, service_account_file_path) |
-initialisation method for BigQuery Connector | :param str
-read_big_query_project : project used while reading from BigQuery | :param str
-write_big_query_project: project used while writing into BigQuery | :param str
-service_account_file_path: project specific BigQuery Credential | | dump_data
-(self, database=None, table=None, dataframe=None, mode='append') | Dumps data
-into from BigQuery | :param string database: target bigquery database | :param
-string table: target table name | :param pd.DataFrame dataframe: pandas
-dataframe for dumping into bigquery | :param string mode: it can be either
-append or replace | | execute_query(self, query, query_config=None,
-timeout=900, max_retries=0, time_interval=5) | Executes query from from
-BigQuery table | :param string query: query for execution | :param string
-query_cofig: config for parameterised query | :param integer timeout : maximum
-bigquery execution timeout | :param string max_retries: maximum retries if data
-is not fetched | :param integer time_interval : time interval between retries |
-| get_data(self, query=None, query_config=None, max_retries=0, time_interval=5)
-| Fetches data from from BigQuery | :param string query: query for fetching
-data from table | :param string query_cofig: config for parameterised query | :
-param string max_retries: maximum retries if data is not fetched | :param
-integer time_interval : time interval between retries | | insert_rows_array
-(self, dataset=None, table=None, rows_to_insert=None) | Streaming insert into
-from BigQuery | :param string dataset: target bigquery database | :param string
-table: target table name | :param list rows_to_insert: list of dictionaries
-where each dictionary is a | row with keys as column names | |
-insert_rows_in_bigquery(self, dataset=None, table=None, rows_to_insert=None) |
-Streaming insert into from BigQuery | :param string dataset: target bigquery
-database | :param string table: target table name | :param rows_to_insert: list
-of dictionaries where each dictionary is a | row with keys as column names ```
---- ## 3. Configurer### 1. Profile Decorator**Code Snippet Sample :** ```python
-from custom_utils.configurer.profiler import profiler @profiler
+"select * from table_name" df = bq.pull_data(query) # Dumping Dataframe in
+BigQuery bq.push_data(database="rahul_temp", table="demo", dataframe=df,
+mode="append") # Executing any query in BigQuery query = "INSERT
+rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)" BigQuery.execute_query(query) #
+Streaming insert in BigQuery row_to_insert = [{"id": 1, "userid": 1,
+"languageId": 58, "mode":0,"active":1}] BigQuery.insert_rows_in_bigquery
+(dataset="rahul_temp", table="Demo", rows_to_insert=row_to_insert) ```
+**BigQuery Connector Documentaion** ``` class BigQuery(builtins.object) |
+BigQuery(read_big_query_project, write_big_query_project,
+service_account_file_path) | | BigQuery database utility functions | | Methods
+defined here: | | __init__(self, read_big_query_project,
+write_big_query_project, service_account_file_path) | initialisation method for
+BigQuery Connector | :param str read_big_query_project : project used while
+reading from BigQuery | :param str write_big_query_project: project used while
+writing into BigQuery | :param str service_account_file_path: project specific
+BigQuery Credential | | push_data(self, database=None, table=None,
+dataframe=None, mode='append') | Dumps data into from BigQuery | :param string
+database: target bigquery database | :param string table: target table name | :
+param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery | :
+param string mode: it can be either append or replace | | execute_query(self,
+query, job_config=None, timeout=900, max_retries=0, time_interval=5) | Executes
+query from from BigQuery table | :param string query: query for execution | :
+param string query_cofig: config for parameterised query | :param integer
+timeout : maximum bigquery execution timeout | :param string max_retries:
+maximum retries if data is not fetched | :param integer time_interval : time
+interval between retries | | pull_data(self, query=None, job_config=None,
+max_retries=0, time_interval=5) | Fetches data from from BigQuery | :param
+string query: query for fetching data from table | :param string query_cofig:
+config for parameterised query | :param string max_retries: maximum retries if
+data is not fetched | :param integer time_interval : time interval between
+retries | | insert_rows_array(self, dataset=None, table=None,
+rows_to_insert=None) | Streaming insert into from BigQuery | :param string
+dataset: target bigquery database | :param string table: target table name | :
+param list rows_to_insert: list of dictionaries where each dictionary is a |
+row with keys as column names | | insert_rows_in_bigquery(self, dataset=None,
+table=None, rows_to_insert=None) | Streaming insert into from BigQuery | :param
+string dataset: target bigquery database | :param string table: target table
+name | :param rows_to_insert: list of dictionaries where each dictionary is a |
+row with keys as column names ``` --- ## 3. Configurer### 1. Profile
+Decorator**Code Snippet Sample :** ```python from
+custom_utils.configurer.profiler import profiler @profiler
 (sort_by='cumulative', lines_to_print=10, strip_dirs=True) def
 product_counter_v3(): return [1, 2, 3, 4, 5] ``` **Profiler Documentaion**
 ```python def profiler(output_file=None, sort_by='cumulative',
 lines_to_print=None, strip_dirs=False): """ A time profiler decorator :param
 str output_file: Path of the output file. If only name of the file is given,
 it's saved in the current directory. If it's None, the name of the decorated
 function is used. :param str sort_by: SortKey enum or tuple/list of str/SortKey
@@ -154,31 +160,24 @@
 size of the printout, especially that sorting by 'cumulative', the time
 consuming operations are printed toward the top of the file. :param bool
 strip_dirs: Whether to remove the leading path info from file names. This is
 also useful in reducing the size of the printout :return: Profile of the
 decorated function """ ``` ### 2. Log Formatter**Code Snippet Sample :**
 ```python from custom_utils.configurer.utils import LogFormatter
 LogFormatter.apply() ``` **Log Formatter Documentation** ``` class LogFormatter
-(logging.Formatter): """Log Formatter class for trell ai usage""" __date_format
-= '%d/%b/%Y:%H:%M:%S %Z' @staticmethod def apply(level=logging.INFO): """ Start
-logging in json format. :return: ``` --- ## 4. Alerter### 1. Slack
-Alerter**Code Snippet Sample :** ``` from custom_utils.slack_alerter import
-Alerter try: """Write your code""" except: """Catch exceptions"""
-Alerter.send_alert(message=message, url=url, userId=userId, send_error=True)
-``` **Alerter Documentation :** ```python class Alerter(builtins.object) |
-Class for sending alerts and monitoring stats to a slack channel | | Static
-methods defined here: | | send_alert(message: str, url: str, user_id: str =
-None, send_error: bool = False) | This function send alert to a target channel
-tagging a user | with a alert message and traceback error. | args: | message :
-Pass the message to be displayed in the channel | url : Pass webhook of target
-channel | user_id : Slack user_id of user who needs to be tagged ( | send_error
-: This should be set True, | if slack_alert is called while catching exception
-| returns: Nothing | | send_monitoring_stats(start: tuple, stop: tuple,
-message: str, url: str, user_id: str = None) | This function send run time and
-RAM usage for a cronjob | to a target channel tagging a user with a message | |
-Args: | message : Pass the message to be displayed in the channel | url : Pass
-webhook of target channel | user_id : Slack user_id of user who needs to be
-tagged | start : this should be set to output of start_monitoring function |
-stop : this should be set to output of start_monitoring function | |
-start_monitoring() | function for initiating monitoring | | stop_monitoring() |
-function for end monitoring | | -----------------------------------------------
------------------------ ``` ---
+(logging.Formatter): """Log Formatter class for custom-utils package"""
+__date_format = '%d/%b/%Y:%H:%M:%S %Z' @staticmethod def apply
+(level=logging.INFO): """ Start logging in json format. :return: ``` --- ## 4.
+Alerter### 1. Slack Alerter**Code Snippet Sample :** ```python3 from
+custom_utils.alerter.slack import Slack slack = Slack(token=SLACK_BOT_TOKEN) #
+OR Slack() with SLACK_BOT_TOKEN as env variable channel="#shield" message =
+"testing" uids = ["U03PAP8C1RC", "U03PAP8C1RC"] slack.send_alert(channel,
+message, uids) ``` **Alerter Documentation :** ```python class Slack
+(builtins.object) | Slack(token=None) | | Class for sending alerts and
+monitoring stats to a slack channel | | Methods defined here: | | __init__
+(self, token=None) | Initialize self. See help(type(self)) for accurate
+signature. | | send_alert(self, channel: str, message: str, uids: list = []) |
+This function send alert to a target channel tagging a user | with a alert
+message and traceback error. | args: | channel : Name of the channel (ex :
+#channel_name) | message : Pass the message to be displayed in the channel |
+uids : List of Slack user_ids who needs to be tagged | | returns: Nothing | | -
+--------------------------------------------------------------------- ``` ---
```

### Comparing `custom-utils-0.0.2/custom_utils/connector/mongodb.py` & `custom-utils-0.0.37/custom_utils/connector/mongodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Module containing mongodb utility functions"""
 
 import time
-import logging
 import pandas as pd
 from pymongo import MongoClient
-
+from custom_utils.configurer.utils import logger
 from custom_utils.exceptions import MongodbConnectionError
 
 
 class MongoDB:
     """
     MongoDB utility functions.
     """
@@ -20,15 +19,15 @@
         :param str uri: mongo uri string for establishing connection
         """
 
         self.db = db
         self.uri = uri
         try:
             self.client = MongoClient(self.uri)
-            logging.debug("Mongo Connection set successfully ")
+            logger.debug("Mongo Connection set successfully ")
         except Exception as err:
             raise MongodbConnectionError(err) from err
 
 
     def push_data(self, data, collection, db=None):
         """
         Function for inserting data into db
@@ -47,17 +46,17 @@
             try:
                 client_db = self.client[db]
                 collection = client_db[collection]
                 if isinstance(data, pd.DataFrame):
                     data_dict = data.to_dict("records")
                 collection.insert_many(data_dict)
                 pushed = True
-                logging.debug("data pushed successfully ")
+                logger.debug("data pushed successfully ")
             except Exception as err:
-                logging.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
+                logger.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
                 time.sleep(2)
                 self.client = MongoClient(self.uri)
 
     def pull_data(self, list_dict, collection, db=None):
         """
         Function for inserting data into db
         :param str db : database name
@@ -79,18 +78,18 @@
                     for j in collection.find():
                         data.append(j)
                 else:
                     for i in list_dict:
                         for j in collection.find(i):
                             data.append(j)
                 pulled = True
-                logging.debug("data pulled successfully")
+                logger.debug("data pulled successfully")
                 return pd.DataFrame(data=data)
             except Exception as err:
-                logging.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
+                logger.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
                 time.sleep(2)
                 self.client = MongoClient(self.uri)
 
     def update_value(self, id_dict, set_dict, collection, db=None, upsert=None):
 
         """
         Function for updating data into db
@@ -106,18 +105,18 @@
             db = self.db
 
         updated = False
         while not updated:
             try:
                 client_db = self.client[db]
                 client_db[collection].update_many(id_dict, set_dict, upsert=upsert)
-                logging.debug("data updated successfully")
+                logger.debug("data updated successfully")
                 updated = True
             except Exception as err:
-                logging.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
+                logger.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
                 time.sleep(1)
                 self.client = MongoClient(self.uri)
 
     def upsert_json(self, output_json, upsert_keys, collection, db=None):
 
         """
         Function for inserting data into db
@@ -137,18 +136,18 @@
             try:
                 client_db = self.client[db]
                 for record in output_json:
                     filter_query = dict()
                     for filter_key in upsert_keys:
                         filter_query[filter_key] = record[filter_key]
                     client_db[collection].replace_one(filter_query, record, upsert=True)
-                logging.debug("data inserted successfully")
+                logger.debug("data inserted successfully")
                 inserted = True
             except Exception as err:
-                logging.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
+                logger.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
                 time.sleep(1)
                 self.client = MongoClient(self.uri)
 
 
     def delete_data(self,collection, db=None, overall=False, condition_dict=None):
 
         """
@@ -168,18 +167,18 @@
             try:
                 client_db = self.client[db]
                 if overall:
                     client_db[collection].remove({})
                     print('Overall data deleted.')
                 else:
                     client_db[collection].delete_many(condition_dict)
-                logging.debug("data deleted successfully")
+                logger.debug("data deleted successfully")
                 deleted = True
             except Exception as err:
-                logging.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
+                logger.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
                 time.sleep(1)
                 self.client = MongoClient(self.uri)
 
     def fetch_data(self, collection, db=None, query={}, only_include_keys=[]):
         """
         function to fetch data from the given database and collection on given query
         :param str db : db_name in mongo
@@ -203,19 +202,19 @@
                 for key in only_include_keys:
                     projections[key] = 1
                 projections["_id"] = 0
                 if collection in all_collection_names:
                     cursor = client_db[collection]
                     for row in cursor.find(query, projections):
                         results.append(row)
-                logging.debug("data fetched successfully")
+                logger.debug("data fetched successfully")
                 fetched = True
                 return results
             except Exception as err:
-                logging.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
+                logger.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
                 time.sleep(1)
                 self.client = MongoClient(self.uri)
 
     def fetch_data_sorted(self, collection, db=None, pipeline=[]):
         """
         function to fetch data from the given database and collection on given query
         :param str db: db_name in mongo
@@ -231,13 +230,13 @@
         while not fetched:
             try:
                 results = []
                 client_db = self.client[db]
                 client_collection = client_db[collection]
                 results = client_collection.aggregate(pipeline=pipeline)
                 fetched = True
-                logging.debug("data fetched successfully")
+                logger.debug("data fetched successfully")
                 return results
             except Exception as err:
-                logging.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
+                logger.error(f"Got Exception.. {err}\nReconnecting.. Retrying..")
                 time.sleep(1)
                 self.client = MongoClient(self.uri)
```

### Comparing `custom-utils-0.0.2/custom_utils/connector/mysql.py` & `custom-utils-0.0.37/custom_utils/connector/mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """MySQL database utility functions"""
 
-import logging
 import sqlalchemy
 import pandas as pd
+from custom_utils.configurer.utils import logger
 from custom_utils.exceptions import MysqlConnectionError, MysqlDataFetchError, MysqlGenericError
 
 
 class MySQL:
     """MySQL database utility functions"""
 
     def __init__(self, db_string):
@@ -17,26 +17,26 @@
 
         try:
             self.connection = sqlalchemy.create_engine(db_string)
         except Exception as err:
             raise MysqlConnectionError(err) from err
 
 
-    def get_data(self, query):
+    def pull_data(self, query):
 
         """
         Fetch data from mysql as a dataframe.
         :param string query: query for fetching data from table
         :return pd.DataFrame data
         """
 
 
         try:
             data = pd.read_sql(query + " ;", self.connection)
-            logging.debug("data fetched successfully")
+            logger.debug("data fetched successfully")
             return data
         except Exception as err:
             raise MysqlDataFetchError(err) from err
         finally:
             self.connection.dispose()
 
 
@@ -46,32 +46,32 @@
         Execute a query in the mysql table
         :param string query: query for execution in the table
         :return :
         """
 
         try:
             self.connection.execute(query)
-            logging.debug("query executed successfully")
+            logger.debug("query executed successfully")
         except Exception as err:
             raise MysqlGenericError(err) from err
         finally:
             self.connection.dispose()
 
-    def dump_data(self, data, table_name, mode="append"):
+    def push_data(self, data, table_name, mode="append"):
 
         """
         Execute a query in the mysql table
         :param pd.DataFrame data: dataframe to be appended or replaced
         :param string table_name: name of the the target table
         :param string mode: it can be either replace or append
         :return None
         """
 
 
         try:
             connection = self.connection
             data.to_sql(name=table_name, con=connection, if_exists=mode, index=False)
-            logging.debug("data dumped successfully")
+            logger.debug("data dumped successfully")
         except Exception as err:
             raise MysqlGenericError(err) from err
         finally:
             connection.dispose()
```

### Comparing `custom-utils-0.0.2/custom_utils/exceptions.py` & `custom-utils-0.0.37/custom_utils/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,7 +22,10 @@
     """Raised when data from MongoDB connection is failed"""
 
 class MongodbDataFetchError(Exception):
     """Raised when fetching data from MongoDB is failed"""
 
 class MongodbGenericError(Exception):
     """Raised when there MongoDB API is falied"""
+
+class SlackError(Exception):
+    """Raised when there SLACK_BOT_TOKEN is not passed or invalid"""
```

### Comparing `custom-utils-0.0.2/custom_utils.egg-info/PKG-INFO` & `custom-utils-0.0.37/custom_utils.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,466 +1,470 @@
 Metadata-Version: 2.1
 Name: custom-utils
-Version: 0.0.2
+Version: 0.0.37
 Summary: Utilities for database connectors, slack alerter, loggers etc
 Home-page: https://github.com/RahulnKumar/custom-utils
 Author: Rahul Kumar
 Author-email: rahulnkumar7@gmail.com
-License: UNKNOWN
-Description: # custom-utils
-        Pip Package for Database Connectors, Alerter, Log Formatter etc
-        
-        
-        ***
-        
-        <p float="left">
-          <img src=https://img.shields.io/pypi/v/custom-utils />
-          <img src=https://www.code-inspector.com/project/29426/score/svg />
-          <img src=https://img.shields.io/pypi/dm/custom-utils?logo=Python&style=social /> 
-          <a href="https://github.com/RahulnKumar/custom-utils/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/RahulnKumar/custom-utils"></a>
-        </p>
-         
-        
-        ## Table of Contents
-        
-        - [Installation](#Installation)
-        - [Connector](#Connector)
-          - [S3 Connector](#S3_Connector)
-          - [MySQL Connector](#MySQL_Connector)
-          - [MongoDB Connector](#MongoDB_Connector)
-          - [BigQuery Connector](#BigQuery_Connector)
-         
-        - [Configurer](#Configurer)
-          - [Log Formatter](#Log_Formatter)
-          - [Profile Decorator](#Profile_Decorator)
-          
-        - [Alerter](#Alerter)
-          - [Slack Alerter](#Slack_Alerter)
-        
-        ***
-        
-        ## 1.  Installation<a id="Installation" name="Installation">    
-        
-        - **Installation from Pypi repository** (Any one)
-        	
-            `pip install custom-utils`  --> minimal installation  
-            `pip install custom-utils[full]` --> full installation  
-            `pip install custom-utils[s3,mysql,bigquery,mongodb]`  --> selective installation 
-        - **Installation from github repository** (Any one)  
-        	
-            `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
-            `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
-            `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
-            
-        ---
-            
-        	
-        ## 2. Connector<a id="Connector" name="Connector">
-        
-            
-        ### 1. S3 Connector<a id="S3_Connector" name="S3_Connector">     
-        
-        **Code Snippet Sample :**
-        ```python
-        from custom_utils.connector.s3 import S3
-        
-        # Uplaoding data to S3
-        demo = {"Name": "Trell", "Age": 4}
-        S3.write_to_s3_bucket(python_data_object=demo,
-                                     bucket='data-science-datas',
-                                     sub_bucket='models/', file_name="demo.pickle")
-                                     
-        # Doownlaoding data from S3
-        
-        demo = S3.read_from_s3_bucket(bucket='data-science-datas',          
-                                                 sub_bucket='models/',
-                                                 file_name="demo.pickle")
-        ```
-        
-        **S3 Connector Documentation**
-            
-        ```
-        class S3(builtins.object)
-         |  AWS S3 utility functions
-         |  
-         |  Static methods defined here:
-         |  
-         |  read_from_s3_bucket(bucket, sub_bucket, file_name)
-         |      read data stored in S3 bucket
-         |      :param string bucket: bucket name
-         |      :param string sub_bucket: sub-bucket name
-         |      :param string file_name: name of the file to be read
-         |      :return old_data : python object stored in the S3
-         |  
-         |  upload_data_from_local_to_s3(model_file_name, bucket, sub_bucket)
-         |      write data stored in local machine into S3 bucket from
-         |      :param string bucket: bucket name
-         |      :param string sub_bucket: sub-bucket name
-         |      :param string file_name: name of the file to be written
-         |      :return None
-         |  
-         |  write_to_s3_bucket(python_data_object, bucket, sub_bucket, file_name)
-         |      write python objects/variables etc  into S3 bucket
-         |      :param string bucket: bucket name
-         |      :param string sub_bucket: sub-bucket name
-         |      :param string file_name: name of the file to be written
-         |      :return None
-        ```
-        ---
-            
-        
-        ---
-           
-        ### 2. MySQL Connector<a id="MySQL_Connector" name="MySQL_Connector">  
-          
-        **Code Snippet Sample :**  
-        ```python
-        # Query from Custom MySQL Database
-        from custom_utils.connector.mysql import MySQL 
-        user = "***"
-        password = "***"
-        host = "***"
-        port = "***"
-        database = "***"
-        db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}"
-        query = "select * from table_name limit 10"
-        mysql = MySQL(db_string=db_string)
-        df = mysql.get_data(query = query) 
-        ```
-            
-        **MySQL Connector Documentaion**
-        ```
-        class MySQL(builtins.object)
-         |  MySQL(db_string)
-         |  
-         |  MySQL database utility functions
-         |  
-         |  Methods defined here:
-         |  
-         |  __init__(self, db_string)
-         |      initialisation method for MySQL Connector
-         |      :param string db_string: mysql database connection string
-         |  
-         |  dump_data(self, data, table_name, mode='append')
-         |      Execute a query in the mysql table
-         |      :param pd.DataFrame data: dataframe to be appended or replaced
-         |      :param string table_name: name of the the target table
-         |      :param string mode: it can be either replace or append
-         |      :return None
-         |  
-         |  execute_query(self, query)
-         |      Execute a query in the mysql table
-         |      :param string query: query for execution in the table
-         |      :return :
-         |  
-         |  get_data(self, query)
-         |      Fetch data from mysql as a dataframe.
-         |      :param string query: query for fetching data from table
-         |      :return pd.DataFrame data
-        ```
-            
-        ---
-            
-            
-        ### 3.  MongoDB Connector<a id="MongoDB_Connector" name="MongoDB_Connector">
-            
-        **Code Snippet Sample :**  
-        ```python
-        from custom_utils.connector.mongodb import MongoDB
-        uri = "****"
-        db = "***"
-        collection = "****"
-        mongo = MongoDb(uri = uri, db = db)
-        
-        #Reading with pull method
-        data =  mongo.pull_data(collection=collection, list_dict=list_dict)
-        
-        # Reading with fetch method
-        query = {'id': {'$in': [1,2]}}
-        data = mongo.fetch_data(collection, query=query, only_include_keys=["name"])
-        
-        #Writing inot MongoDB
-        mongo.push_data(collection = collection, data = data)
-        
-        #Updating value
-        id_dict = {"id":"2"}
-        set_dict = {"$set": {"name":"ram"}}
-        mongo.update_value(id_dict, set_dict,collection=collection, upsert=True)
-        
-        # Deleting data
-        mongo.delete_data(collection=collection, overall=False, condition_dict= {"id":None})
-        
-        ```
-        
-         **MongoDB Connector Documentaion**
-        ```    
-        class MongoDB(builtins.object)
-         |  MongoDB(db=None, uri=None)
-         |  
-         |  MongoDB utility functions.
-         |  
-         |  Methods defined here:
-         |  
-         |  __init__(self, db=None, uri=None)
-         |      initialisation method for MongoDB connector
-         |      :param str db: database name
-         |      :param str uri: mongo uri string for establishing connection
-         |  
-         |  delete_data(self, collection, db=None, overall=False, condition_dict=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param bool overall : delete whole collection if True
-         |      :param dict condition_dict : query for deletion
-         |      :return:
-         |  
-         |  fetch_data(self, collection, db=None, query={}, only_include_keys=[])
-         |      function to fetch data from the given database and collection on given query
-         |      :param str db : db_name in mongo
-         |      :param str collection: collection name in mongo for database db
-         |      :param dict query : execution query statement; default is {} which means fetch
-         |                         all without any filters
-         |      :param list only_include_keys : list of keys to be included while fetching rows
-         |      :return: pd.DataFrame
-         |  
-         |  fetch_data_sorted(self, collection, db=None, pipeline=[])
-         |      function to fetch data from the given database and collection on given query
-         |      :param str db: db_name in mongo
-         |      :param str collection: collection name in mongo for database db
-         |      :param list pipeline: pipeline required to aggregate
-         |      :return: pd.DataFrame
-         |  
-         |  pull_data(self, list_dict, collection, db=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param list list_dict : query for fetching data
-         |      :return: pd.DataFrame
-         |  
-         |  push_data(self, data, collection, db=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param list/pd.DataFrame data : data to be inserted in the form of
-         |                                      dataframe or list of dictionaries
-         |      :return:
-         |  
-         |  update_value(self, id_dict, set_dict, collection, db=None, upsert=None)
-         |      Function for updating data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param dict id_dict : query for updation
-         |      :param dict set_dict : key and value dictionary to be updated
-         |      :param bool upsert : whether to upsert or just update
-         |      :return:
-         |  
-         |  upsert_json(self, output_json, upsert_keys, collection, db=None)
-         |      Function for inserting data into db
-         |      :param str db : database name
-         |      :param str collection : collection name
-         |      :param dict output_json : list of dictionaries where each dictionary is
-         |                                a row with keys as column names
-         |      :param list upsert_keys : keys to be upserted
-         |      :return:
-         |  
-         |  ----------------------------------------------------------------------
-        ```
-        ---
-        	
-        ### 4.  BigQuery Connector<a id="BigQuery_Connector" name="BigQuery_Connector">
-            
-        **Code Snippet Sample :**  
-        ```python
-        
-        # Fetching data from BigQuery
-        from custom_utils.connector.bigquery import BigQuery
-        bq = BigQuery(read_big_query_project = "****",
-                            service_account_file_path="***.json")
-        query = "select * from `trellatale.trellDbDump.userLanguages` limit 2"
-        df = bq.get_data(query)
-        
-        # Dumping Dataframe in BigQuery
-        bq.dump_data(database="rahul_temp", table="demo", dataframe=df, mode="append")
-        
-        # Executing any query in BigQuery
-        query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
-        BigQuery.execute_query(query)
-        
-        # Streaming insert in BigQuery
-        row_to_insert = [{"id": 1, "userid": 1, "languageId": 58,
-                     "mode":0,"active":1}]
-        BigQuery.insert_rows_in_bigquery(dataset="rahul_temp", table="Demo", rows_to_insert=row_to_insert)
-        
-        ```
-            
-        **BigQuery Connector Documentaion**
-        ```
-        class BigQuery(builtins.object)
-         |  BigQuery(read_big_query_project, write_big_query_project, service_account_file_path)
-         |  
-         |  BigQuery database utility functions
-         |  
-         |  Methods defined here:
-         |  
-         |  __init__(self, read_big_query_project, write_big_query_project, service_account_file_path)
-         |      initialisation method for BigQuery Connector
-         |      :param str read_big_query_project : project used while reading from BigQuery
-         |      :param str write_big_query_project: project used while writing into BigQuery
-         |      :param str service_account_file_path: project specific BigQuery Credential
-         |  
-         |  dump_data(self, database=None, table=None, dataframe=None, mode='append')
-         |      Dumps data into from BigQuery
-         |      :param string database: target bigquery database
-         |      :param string table: target table name
-         |      :param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery
-         |      :param string mode: it can be either append or replace
-         |  
-         |  execute_query(self, query, query_config=None, timeout=900, max_retries=0, time_interval=5)
-         |      Executes query from from BigQuery table
-         |      :param string query: query for execution
-         |      :param string query_cofig: config for parameterised query
-         |      :param integer timeout : maximum bigquery execution timeout
-         |      :param string max_retries: maximum retries if data is not fetched
-         |      :param integer time_interval : time interval between retries
-         |  
-         |  get_data(self, query=None, query_config=None, max_retries=0, time_interval=5)
-         |      Fetches data from from BigQuery
-         |      :param string query: query for fetching data from table
-         |      :param string query_cofig: config for parameterised query
-         |      :param string max_retries: maximum retries if data is not fetched
-         |      :param integer time_interval : time interval between retries
-         |  
-         |  insert_rows_array(self, dataset=None, table=None, rows_to_insert=None)
-         |      Streaming insert into from BigQuery
-         |      :param string dataset: target bigquery database
-         |      :param string table: target table name
-         |      :param list rows_to_insert: list of dictionaries where each dictionary is a
-         |                                  row with keys as column names
-         |  
-         |  insert_rows_in_bigquery(self, dataset=None, table=None, rows_to_insert=None)
-         |      Streaming insert into from BigQuery
-         |      :param string dataset: target bigquery database
-         |      :param string table: target table name
-         |      :param  rows_to_insert: list of dictionaries where each dictionary is a
-         |                              row with keys as column names
-        ```
-        ---
-        	
-        	
-        ## 3. Configurer<a id="Configurer" name="Configurer">   
-        	
-        ### 1. Profile Decorator<a id="Profile_Decorator" name="Profile_Decorator">    
-            
-        **Code Snippet Sample :**  
-        ```python
-        from custom_utils.configurer.profiler import profiler
-        @profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
-        def product_counter_v3():
-            return [1, 2, 3, 4, 5]
-        ```
-        **Profiler Documentaion**
-        ```python
-        def profiler(output_file=None, sort_by='cumulative', lines_to_print=None, strip_dirs=False):
-            """
-            A time profiler decorator
-        
-            :param str output_file: Path of the output file. If only name of the file is given, it's saved in the current
-            directory. If it's None, the name of the decorated function is used.
-            :param str sort_by: SortKey enum or tuple/list of str/SortKey enum Sorting criteria for the Stats object. For a list
-            of valid string and SortKey refer to: https://docs.python.org/3/library/profile.html#pstats.Stats.sort_stats
-            :param int lines_to_print: Number of lines to print. Default (None) is for all the lines. This is useful in reducing
-            the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
-            the top of the file.
-            :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
-            size of the printout
-            :return: Profile of the decorated function
-            """
-        ```
-        ###  2.  Log Formatter<a id="Log_Formatter" name="Log_Formatter">
-         
-        **Code Snippet Sample :**
-        ```python
-        from custom_utils.configurer.utils import LogFormatter
-        LogFormatter.apply()
-        ```
-            
-        **Log Formatter Documentation**
-        ```
-        class LogFormatter(logging.Formatter):
-            """Log Formatter class for trell ai usage"""
-        
-            __date_format = '%d/%b/%Y:%H:%M:%S %Z'
-        
-            @staticmethod
-            def apply(level=logging.INFO):
-                """
-                Start logging in json format.
-                :return:
-        ```
-        ---
-        	
-        	
-        ## 4. Alerter<a id="Alerter" name="Alerter">    
-        	
-        ###  1.  Slack Alerter<a id="Slack_Alerter" name="Slack_Alerter">  
-            
-            
-        **Code Snippet Sample :**
-        ```
-        from custom_utils.slack_alerter import Alerter
-        try:
-            """Write your code"""
-        except:
-            """Catch exceptions"""
-            Alerter.send_alert(message=message, url=url, userId=userId, send_error=True) 
-        ```
-            
-        **Alerter Documentation :**
-        ```python
-        class Alerter(builtins.object)
-             |  Class for sending alerts and monitoring stats to a slack channel
-             |  
-             |  Static methods defined here:
-             |  
-             |  send_alert(message: str, url: str, user_id: str = None, send_error: bool = False)
-             |      This function send alert to a target channel tagging a user
-             |                         with a alert message and traceback error.
-             |      args:
-             |              message     : Pass the message to be displayed in the channel
-             |              url         : Pass webhook of target channel
-             |              user_id     : Slack user_id of user who needs to be tagged (
-             |              send_error  : This should be set True,
-             |                           if slack_alert is called while catching exception
-             |      returns: Nothing
-             |  
-             |  send_monitoring_stats(start: tuple, stop: tuple, message: str, url: str, user_id: str = None)
-             |      This function send run time and RAM usage for a cronjob
-             |      to a target channel tagging a user with a  message
-             |      
-             |      Args:
-             |              message : Pass the message to be displayed in the channel
-             |              url : Pass webhook of target channel
-             |              user_id : Slack user_id of user who needs to be tagged
-             |              start : this should be set to output of start_monitoring function
-             |              stop : this should be set to output of start_monitoring function
-             |  
-             |  start_monitoring()
-             |      function for initiating monitoring
-             |  
-             |  stop_monitoring()
-             |      function for end monitoring
-             |  
-             |  ----------------------------------------------------------------------
-        ```
-        ---
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown
+Provides-Extra: s3
+Provides-Extra: mysql
 Provides-Extra: bigquery
-Provides-Extra: full
 Provides-Extra: mongodb
-Provides-Extra: mysql
-Provides-Extra: s3
+Provides-Extra: slack
+Provides-Extra: full
+License-File: LICENSE
+
+# custom-utils
+Pip Package for Database Connectors, Alerter, Log Formatter etc
+
+
+***
+
+<p float="left">
+  <img src=https://img.shields.io/pypi/v/custom-utils />
+  <img src=https://www.code-inspector.com/project/29426/score/svg />
+  <img src=https://img.shields.io/pypi/dm/custom-utils?logo=Python&style=social /> 
+  <a href="https://github.com/RahulnKumar/custom-utils/blob/main/LICENSE"><img alt="GitHub license" src="https://img.shields.io/github/license/RahulnKumar/custom-utils"></a>
+</p>
+ 
+
+## Table of Contents
+
+- [custom-utils](#custom-utils)
+  - [Table of Contents](#table-of-contents)
+  - [1.  Installation](#1--installation)
+  - [2. Connector](#2-connector)
+    - [1. S3 Connector](#1-s3-connector)
+    - [2. MySQL Connector](#2-mysql-connector)
+    - [3.  MongoDB Connector](#3--mongodb-connector)
+    - [4.  BigQuery Connector](#4--bigquery-connector)
+  - [3. Configurer](#3-configurer)
+    - [1. Profile Decorator](#1-profile-decorator)
+    - [2.  Log Formatter](#2--log-formatter)
+  - [4. Alerter](#4-alerter)
+    - [1.  Slack Alerter](#1--slack-alerter)
+
+***
+
+## 1.  Installation<a id="1--installation">    
+
+- **Installation from Pypi repository** (Any one)
+	
+    `pip install custom-utils`  --> minimal installation  
+    `pip install custom-utils[full]` --> full installation  
+    `pip install custom-utils[s3,mysql,bigquery,mongodb,slack]`  --> selective installation 
+- **Installation from github repository** (Any one)  
+	
+    `pip install git+https://github.com/rahulnkumar/custom-utils.git`  
+    `pip install git+https://github.com/rahulnkumar/custom-utils.git@<tag_no>`  
+    `pip install git+https://github.com/rahulnkumar/custom-utils.git@<branch_name>`    
+
+<img src="https://i.ibb.co/WHwqTpr/pip-cu.gif" alt="pip-cu" border="0">
+    
+---
+    
+	
+## 2. Connector<a id="2-connector">
+
+    
+### 1. S3 Connector<a id="1-s3-connector">     
+
+**Code Snippet Sample :**
+```python
+## To use S3 either setup AWS CLI or set the credentials from pip package only
+
+## Setup AWS CLI
+sudo apt install awscli && aws configure
+
+## Setup Credentials from pip package
+from custom_utils.configurer.utils import Credential
+Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********")
+
+
+from custom_utils.connector.s3 import S3
+
+# Uplaoding data to S3
+S3.push_local_data(file_path, s3_uri)
+                             
+# Doownlaoding data from S3
+S3.pull_s3_data(file_path, s3_uri)
+```
+
+**S3 Connector Documentation**
+    
+```
+class S3(builtins.object)
+ |  AWS S3 utility functions
+ |  
+ |  Static methods defined here:
+ |  
+ |  pull_python_object(s3_uri)
+ |      read python object stored in S3 bucket
+ |      :param string s3_uri: s3 uri of the object
+ |      :return python_object : python object stored in the S3
+ |  
+ |  pull_s3_data(file_path, s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: target s3 uri
+ |      :param string file_path:  local path of the file 
+ |      :return None
+ |  
+ |  push_local_data(file_path, s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: target s3 uri
+ |      :param string file_path:  local path of the file 
+ |      :return None
+ |  
+ |  push_python_object(python_object, s3_uri)
+ |      write python objects/variables etc  into S3 bucket
+ |      :param string bucket: bucket name
+ |      :param string sub_bucket: sub-bucket name
+ |      :param string file_name: name of the file to be written
+ |      :return None
+ |  
+ |  read_csv(s3_uri)
+ |      write data stored in local machine into S3 bucket from
+ |      :param string s3_uri: csv file S3 URI
+ |      :return df : pandas dataframe
+ |  
+ |  ----------------------------------------------------------------------
+  
+```
+---
+    
+
+---
+   
+### 2. MySQL Connector<a id="2-mysql-connector">  
+  
+**Code Snippet Sample :**  
+```python
+# Query from Custom MySQL Database
+from custom_utils.connector.mysql import MySQL 
+user = "***"
+password = "***"
+host = "***"
+port = "***"
+database = "***"
+db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}"
+query = "select * from table_name limit 10"
+mysql = MySQL(db_string=db_string)
+df = mysql.pull_data(query = query) 
+```
+    
+**MySQL Connector Documentaion**
+```
+class MySQL(builtins.object)
+ |  MySQL(db_string)
+ |  
+ |  MySQL database utility functions
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, db_string)
+ |      initialisation method for MySQL Connector
+ |      :param string db_string: mysql database connection string
+ |  
+ |  push_data(self, data, table_name, mode='append')
+ |      Execute a query in the mysql table
+ |      :param pd.DataFrame data: dataframe to be appended or replaced
+ |      :param string table_name: name of the the target table
+ |      :param string mode: it can be either replace or append
+ |      :return None
+ |  
+ |  execute_query(self, query)
+ |      Execute a query in the mysql table
+ |      :param string query: query for execution in the table
+ |      :return :
+ |  
+ |  pull_data(self, query)
+ |      Fetch data from mysql as a dataframe.
+ |      :param string query: query for fetching data from table
+ |      :return pd.DataFrame data
+```
+    
+---
+    
+    
+### 3.  MongoDB Connector<a id="3--mongodb-connector">
+    
+**Code Snippet Sample :**  
+```python
+from custom_utils.connector.mongodb import MongoDB
+uri = "****"
+db = "***"
+collection = "****"
+mongo = MongoDb(uri = uri, db = db)
+
+#Reading with pull method
+data =  mongo.pull_data(collection=collection, list_dict=list_dict)
+
+# Reading with fetch method
+query = {'id': {'$in': [1,2]}}
+data = mongo.fetch_data(collection, query=query, only_include_keys=["name"])
+
+#Writing into MongoDB
+mongo.push_data(collection = collection, data = data)
+
+#Updating value
+id_dict = {"id":"2"}
+set_dict = {"$set": {"name":"ram"}}
+mongo.update_value(id_dict, set_dict,collection=collection, upsert=True)
+
+# Deleting data
+mongo.delete_data(collection=collection, overall=False, condition_dict= {"id":None})
+
+```
+
+ **MongoDB Connector Documentaion**
+```    
+class MongoDB(builtins.object)
+ |  MongoDB(db=None, uri=None)
+ |  
+ |  MongoDB utility functions.
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, db=None, uri=None)
+ |      initialisation method for MongoDB connector
+ |      :param str db: database name
+ |      :param str uri: mongo uri string for establishing connection
+ |  
+ |  delete_data(self, collection, db=None, overall=False, condition_dict=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param bool overall : delete whole collection if True
+ |      :param dict condition_dict : query for deletion
+ |      :return:
+ |  
+ |  fetch_data(self, collection, db=None, query={}, only_include_keys=[])
+ |      function to fetch data from the given database and collection on given query
+ |      :param str db : db_name in mongo
+ |      :param str collection: collection name in mongo for database db
+ |      :param dict query : execution query statement; default is {} which means fetch
+ |                         all without any filters
+ |      :param list only_include_keys : list of keys to be included while fetching rows
+ |      :return: pd.DataFrame
+ |  
+ |  fetch_data_sorted(self, collection, db=None, pipeline=[])
+ |      function to fetch data from the given database and collection on given query
+ |      :param str db: db_name in mongo
+ |      :param str collection: collection name in mongo for database db
+ |      :param list pipeline: pipeline required to aggregate
+ |      :return: pd.DataFrame
+ |  
+ |  pull_data(self, list_dict, collection, db=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param list list_dict : query for fetching data
+ |      :return: pd.DataFrame
+ |  
+ |  push_data(self, data, collection, db=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param list/pd.DataFrame data : data to be inserted in the form of
+ |                                      dataframe or list of dictionaries
+ |      :return:
+ |  
+ |  update_value(self, id_dict, set_dict, collection, db=None, upsert=None)
+ |      Function for updating data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param dict id_dict : query for updation
+ |      :param dict set_dict : key and value dictionary to be updated
+ |      :param bool upsert : whether to upsert or just update
+ |      :return:
+ |  
+ |  upsert_json(self, output_json, upsert_keys, collection, db=None)
+ |      Function for inserting data into db
+ |      :param str db : database name
+ |      :param str collection : collection name
+ |      :param dict output_json : list of dictionaries where each dictionary is
+ |                                a row with keys as column names
+ |      :param list upsert_keys : keys to be upserted
+ |      :return:
+ |  
+ |  ----------------------------------------------------------------------
+```
+---
+	
+### 4.  BigQuery Connector<a id="4--bigquery-connector">
+    
+**Code Snippet Sample :**  
+```python
+
+# Fetching data from BigQuery
+from custom_utils.connector.bigquery import BigQuery
+bq = BigQuery(read_big_query_project = "****",
+                    service_account_file_path="***.json")
+query = "select * from table_name"
+df = bq.pull_data(query)
+
+# Dumping Dataframe in BigQuery
+bq.push_data(database="rahul_temp", table="demo", dataframe=df, mode="append")
+
+# Executing any query in BigQuery
+query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
+BigQuery.execute_query(query)
+
+# Streaming insert in BigQuery
+row_to_insert = [{"id": 1, "userid": 1, "languageId": 58,
+             "mode":0,"active":1}]
+BigQuery.insert_rows_in_bigquery(dataset="rahul_temp", table="Demo", rows_to_insert=row_to_insert)
+
+```
+    
+**BigQuery Connector Documentaion**
+```
+class BigQuery(builtins.object)
+ |  BigQuery(read_big_query_project, write_big_query_project, service_account_file_path)
+ |  
+ |  BigQuery database utility functions
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, read_big_query_project, write_big_query_project, service_account_file_path)
+ |      initialisation method for BigQuery Connector
+ |      :param str read_big_query_project : project used while reading from BigQuery
+ |      :param str write_big_query_project: project used while writing into BigQuery
+ |      :param str service_account_file_path: project specific BigQuery Credential
+ |  
+ |  push_data(self, database=None, table=None, dataframe=None, mode='append')
+ |      Dumps data into from BigQuery
+ |      :param string database: target bigquery database
+ |      :param string table: target table name
+ |      :param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery
+ |      :param string mode: it can be either append or replace
+ |  
+ |  execute_query(self, query, job_config=None, timeout=900, max_retries=0, time_interval=5)
+ |      Executes query from from BigQuery table
+ |      :param string query: query for execution
+ |      :param string query_cofig: config for parameterised query
+ |      :param integer timeout : maximum bigquery execution timeout
+ |      :param string max_retries: maximum retries if data is not fetched
+ |      :param integer time_interval : time interval between retries
+ |  
+ |  pull_data(self, query=None, job_config=None, max_retries=0, time_interval=5)
+ |      Fetches data from from BigQuery
+ |      :param string query: query for fetching data from table
+ |      :param string query_cofig: config for parameterised query
+ |      :param string max_retries: maximum retries if data is not fetched
+ |      :param integer time_interval : time interval between retries
+ |  
+ |  insert_rows_array(self, dataset=None, table=None, rows_to_insert=None)
+ |      Streaming insert into from BigQuery
+ |      :param string dataset: target bigquery database
+ |      :param string table: target table name
+ |      :param list rows_to_insert: list of dictionaries where each dictionary is a
+ |                                  row with keys as column names
+ |  
+ |  insert_rows_in_bigquery(self, dataset=None, table=None, rows_to_insert=None)
+ |      Streaming insert into from BigQuery
+ |      :param string dataset: target bigquery database
+ |      :param string table: target table name
+ |      :param  rows_to_insert: list of dictionaries where each dictionary is a
+ |                              row with keys as column names
+```
+---
+	
+	
+## 3. Configurer<a id="3-configurer">   
+	
+### 1. Profile Decorator<a id="1-profile-decorator">    
+    
+**Code Snippet Sample :**  
+```python
+from custom_utils.configurer.profiler import profiler
+@profiler(sort_by='cumulative', lines_to_print=10, strip_dirs=True)
+def product_counter_v3():
+    return [1, 2, 3, 4, 5]
+```
+**Profiler Documentaion**
+```python
+def profiler(output_file=None, sort_by='cumulative', lines_to_print=None, strip_dirs=False):
+    """
+    A time profiler decorator
+
+    :param str output_file: Path of the output file. If only name of the file is given, it's saved in the current
+    directory. If it's None, the name of the decorated function is used.
+    :param str sort_by: SortKey enum or tuple/list of str/SortKey enum Sorting criteria for the Stats object. For a list
+    of valid string and SortKey refer to: https://docs.python.org/3/library/profile.html#pstats.Stats.sort_stats
+    :param int lines_to_print: Number of lines to print. Default (None) is for all the lines. This is useful in reducing
+    the size of the printout, especially that sorting by 'cumulative', the time consuming operations are printed toward
+    the top of the file.
+    :param bool strip_dirs: Whether to remove the leading path info from file names. This is also useful in reducing the
+    size of the printout
+    :return: Profile of the decorated function
+    """
+```
+###  2.  Log Formatter<a id="2--log-formatter">
+ 
+**Code Snippet Sample :**
+```python
+from custom_utils.configurer.utils import LogFormatter
+LogFormatter.apply()
+```
+    
+**Log Formatter Documentation**
+```
+class LogFormatter(logging.Formatter):
+    """Log Formatter class for custom-utils package"""
+
+    __date_format = '%d/%b/%Y:%H:%M:%S %Z'
+
+    @staticmethod
+    def apply(level=logging.INFO):
+        """
+        Start logging in json format.
+        :return:
+```
+---
+	
+	
+## 4. Alerter<a id="4-alerter">    
+	
+###  1.  Slack Alerter<a id="1--slack-alerter">  
+    
+    
+**Code Snippet Sample :**
+```python3
+from custom_utils.alerter.slack import Slack
+slack = Slack(token=SLACK_BOT_TOKEN) # OR Slack() with  SLACK_BOT_TOKEN as env variable
+channel="#shield"
+message = "testing"
+uids = ["U03PAP8C1RC", "U03PAP8C1RC"]
+slack.send_alert(channel, message, uids)
+```
+    
+**Alerter Documentation :**
+```python
+class Slack(builtins.object)
+ |  Slack(token=None)
+ |
+ |  Class for sending alerts and monitoring stats to a slack channel
+ |
+ |  Methods defined here:
+ |
+ |  __init__(self, token=None)
+ |      Initialize self.  See help(type(self)) for accurate signature.
+ |
+ |  send_alert(self, channel: str, message: str, uids: list = [])
+ |      This function send alert to a target channel tagging a user
+ |                          with a alert message and traceback error.
+ |      args:
+ |          channel     : Name of the channel (ex : #channel_name)
+ |          message     : Pass the message to be displayed in the channel
+ |          uids        : List of Slack user_ids  who needs to be tagged
+ |
+ |      returns: Nothing
+ |
+ |  ----------------------------------------------------------------------
+```
+---
```

#### html2text {}

```diff
@@ -1,69 +1,80 @@
-Metadata-Version: 2.1 Name: custom-utils Version: 0.0.2 Summary: Utilities for
+Metadata-Version: 2.1 Name: custom-utils Version: 0.0.37 Summary: Utilities for
 database connectors, slack alerter, loggers etc Home-page: https://github.com/
 RahulnKumar/custom-utils Author: Rahul Kumar Author-email:
-rahulnkumar7@gmail.com License: UNKNOWN Description: # custom-utils Pip Package
-for Database Connectors, Alerter, Log Formatter etc ***
+rahulnkumar7@gmail.com Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.6.9
+Description-Content-Type: text/markdown Provides-Extra: s3 Provides-Extra:
+mysql Provides-Extra: bigquery Provides-Extra: mongodb Provides-Extra: slack
+Provides-Extra: full License-File: LICENSE # custom-utils Pip Package for
+Database Connectors, Alerter, Log Formatter etc ***
 [https://img.shields.io/pypi/v/custom-utils] [https://www.code-inspector.com/
 project/29426/score/svg] [https://img.shields.io/pypi/dm/custom-
 utils?logo=Python&style=social] [GitHub_license]
-## Table of Contents - [Installation](#Installation) - [Connector](#Connector)
-- [S3 Connector](#S3_Connector) - [MySQL Connector](#MySQL_Connector) -
-[MongoDB Connector](#MongoDB_Connector) - [BigQuery Connector]
-(#BigQuery_Connector) - [Configurer](#Configurer) - [Log Formatter]
-(#Log_Formatter) - [Profile Decorator](#Profile_Decorator) - [Alerter]
-(#Alerter) - [Slack Alerter](#Slack_Alerter) *** ## 1. Installation-
-**Installation from Pypi repository** (Any one) `pip install custom-utils` --
-> minimal installation `pip install custom-utils[full]` --> full installation
-`pip install custom-utils[s3,mysql,bigquery,mongodb]` --> selective
-installation - **Installation from github repository** (Any one) `pip install
-git+https://github.com/rahulnkumar/custom-utils.git` `pip install git+https://
-github.com/rahulnkumar/custom-utils.git@` `pip install git+https://github.com/
-rahulnkumar/custom-utils.git@` --- ## 2. Connector### 1. S3 Connector**Code
-Snippet Sample :** ```python from custom_utils.connector.s3 import S3 #
-Uplaoding data to S3 demo = {"Name": "Trell", "Age": 4} S3.write_to_s3_bucket
-(python_data_object=demo, bucket='data-science-datas', sub_bucket='models/',
-file_name="demo.pickle") # Doownlaoding data from S3 demo =
-S3.read_from_s3_bucket(bucket='data-science-datas', sub_bucket='models/',
-file_name="demo.pickle") ``` **S3 Connector Documentation** ``` class S3
-(builtins.object) | AWS S3 utility functions | | Static methods defined here: |
-| read_from_s3_bucket(bucket, sub_bucket, file_name) | read data stored in S3
-bucket | :param string bucket: bucket name | :param string sub_bucket: sub-
-bucket name | :param string file_name: name of the file to be read | :return
-old_data : python object stored in the S3 | | upload_data_from_local_to_s3
-(model_file_name, bucket, sub_bucket) | write data stored in local machine into
-S3 bucket from | :param string bucket: bucket name | :param string sub_bucket:
-sub-bucket name | :param string file_name: name of the file to be written | :
-return None | | write_to_s3_bucket(python_data_object, bucket, sub_bucket,
-file_name) | write python objects/variables etc into S3 bucket | :param string
-bucket: bucket name | :param string sub_bucket: sub-bucket name | :param string
-file_name: name of the file to be written | :return None ``` --- --- ### 2.
-MySQL Connector**Code Snippet Sample :** ```python # Query from Custom MySQL
-Database from custom_utils.connector.mysql import MySQL user = "***" password =
-"***" host = "***" port = "***" database = "***" db_string =
-f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}" query =
-"select * from table_name limit 10" mysql = MySQL(db_string=db_string) df =
-mysql.get_data(query = query) ``` **MySQL Connector Documentaion** ``` class
-MySQL(builtins.object) | MySQL(db_string) | | MySQL database utility functions
-| | Methods defined here: | | __init__(self, db_string) | initialisation method
-for MySQL Connector | :param string db_string: mysql database connection string
-| | dump_data(self, data, table_name, mode='append') | Execute a query in the
-mysql table | :param pd.DataFrame data: dataframe to be appended or replaced |
-:param string table_name: name of the the target table | :param string mode: it
-can be either replace or append | :return None | | execute_query(self, query) |
-Execute a query in the mysql table | :param string query: query for execution
-in the table | :return : | | get_data(self, query) | Fetch data from mysql as a
+## Table of Contents - [custom-utils](#custom-utils) - [Table of Contents]
+(#table-of-contents) - [1. Installation](#1--installation) - [2. Connector](#2-
+connector) - [1. S3 Connector](#1-s3-connector) - [2. MySQL Connector](#2-
+mysql-connector) - [3. MongoDB Connector](#3--mongodb-connector) - [4. BigQuery
+Connector](#4--bigquery-connector) - [3. Configurer](#3-configurer) - [1.
+Profile Decorator](#1-profile-decorator) - [2. Log Formatter](#2--log-
+formatter) - [4. Alerter](#4-alerter) - [1. Slack Alerter](#1--slack-alerter)
+*** ## 1. Installation- **Installation from Pypi repository** (Any one) `pip
+install custom-utils` --> minimal installation `pip install custom-utils[full]`
+--> full installation `pip install custom-utils
+[s3,mysql,bigquery,mongodb,slack]` --> selective installation - **Installation
+from github repository** (Any one) `pip install git+https://github.com/
+rahulnkumar/custom-utils.git` `pip install git+https://github.com/rahulnkumar/
+custom-utils.git@` `pip install git+https://github.com/rahulnkumar/custom-
+utils.git@` [pip-cu] --- ## 2. Connector### 1. S3 Connector**Code Snippet
+Sample :** ```python ## To use S3 either setup AWS CLI or set the credentials
+from pip package only ## Setup AWS CLI sudo apt install awscli && aws configure
+## Setup Credentials from pip package from custom_utils.configurer.utils import
+Credential Credential.set(ACCESS_KEY="*********", SECRET_KEY="*********") from
+custom_utils.connector.s3 import S3 # Uplaoding data to S3 S3.push_local_data
+(file_path, s3_uri) # Doownlaoding data from S3 S3.pull_s3_data(file_path,
+s3_uri) ``` **S3 Connector Documentation** ``` class S3(builtins.object) | AWS
+S3 utility functions | | Static methods defined here: | | pull_python_object
+(s3_uri) | read python object stored in S3 bucket | :param string s3_uri: s3
+uri of the object | :return python_object : python object stored in the S3 | |
+pull_s3_data(file_path, s3_uri) | write data stored in local machine into S3
+bucket from | :param string s3_uri: target s3 uri | :param string file_path:
+local path of the file | :return None | | push_local_data(file_path, s3_uri) |
+write data stored in local machine into S3 bucket from | :param string s3_uri:
+target s3 uri | :param string file_path: local path of the file | :return None
+| | push_python_object(python_object, s3_uri) | write python objects/variables
+etc into S3 bucket | :param string bucket: bucket name | :param string
+sub_bucket: sub-bucket name | :param string file_name: name of the file to be
+written | :return None | | read_csv(s3_uri) | write data stored in local
+machine into S3 bucket from | :param string s3_uri: csv file S3 URI | :return
+df : pandas dataframe | | -----------------------------------------------------
+----------------- ``` --- --- ### 2. MySQL Connector**Code Snippet Sample :**
+```python # Query from Custom MySQL Database from custom_utils.connector.mysql
+import MySQL user = "***" password = "***" host = "***" port = "***" database =
+"***" db_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/
+{database}" query = "select * from table_name limit 10" mysql = MySQL
+(db_string=db_string) df = mysql.pull_data(query = query) ``` **MySQL Connector
+Documentaion** ``` class MySQL(builtins.object) | MySQL(db_string) | | MySQL
+database utility functions | | Methods defined here: | | __init__(self,
+db_string) | initialisation method for MySQL Connector | :param string
+db_string: mysql database connection string | | push_data(self, data,
+table_name, mode='append') | Execute a query in the mysql table | :param
+pd.DataFrame data: dataframe to be appended or replaced | :param string
+table_name: name of the the target table | :param string mode: it can be either
+replace or append | :return None | | execute_query(self, query) | Execute a
+query in the mysql table | :param string query: query for execution in the
+table | :return : | | pull_data(self, query) | Fetch data from mysql as a
 dataframe. | :param string query: query for fetching data from table | :return
 pd.DataFrame data ``` --- ### 3. MongoDB Connector**Code Snippet Sample :**
 ```python from custom_utils.connector.mongodb import MongoDB uri = "****" db =
 "***" collection = "****" mongo = MongoDb(uri = uri, db = db) #Reading with
 pull method data = mongo.pull_data(collection=collection, list_dict=list_dict)
 # Reading with fetch method query = {'id': {'$in': [1,2]}} data =
 mongo.fetch_data(collection, query=query, only_include_keys=["name"]) #Writing
-inot MongoDB mongo.push_data(collection = collection, data = data) #Updating
+into MongoDB mongo.push_data(collection = collection, data = data) #Updating
 value id_dict = {"id":"2"} set_dict = {"$set": {"name":"ram"}}
 mongo.update_value(id_dict, set_dict,collection=collection, upsert=True) #
 Deleting data mongo.delete_data(collection=collection, overall=False,
 condition_dict= {"id":None}) ``` **MongoDB Connector Documentaion** ``` class
 MongoDB(builtins.object) | MongoDB(db=None, uri=None) | | MongoDB utility
 functions. | | Methods defined here: | | __init__(self, db=None, uri=None) |
 initialisation method for MongoDB connector | :param str db: database name | :
@@ -98,55 +109,55 @@
 str collection : collection name | :param dict output_json : list of
 dictionaries where each dictionary is | a row with keys as column names | :
 param list upsert_keys : keys to be upserted | :return: | | -------------------
 --------------------------------------------------- ``` --- ### 4. BigQuery
 Connector**Code Snippet Sample :** ```python # Fetching data from BigQuery from
 custom_utils.connector.bigquery import BigQuery bq = BigQuery
 (read_big_query_project = "****", service_account_file_path="***.json") query =
-"select * from `trellatale.trellDbDump.userLanguages` limit 2" df = bq.get_data
-(query) # Dumping Dataframe in BigQuery bq.dump_data(database="rahul_temp",
-table="demo", dataframe=df, mode="append") # Executing any query in BigQuery
-query = "INSERT rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)"
-BigQuery.execute_query(query) # Streaming insert in BigQuery row_to_insert = [
-{"id": 1, "userid": 1, "languageId": 58, "mode":0,"active":1}]
-BigQuery.insert_rows_in_bigquery(dataset="rahul_temp", table="Demo",
-rows_to_insert=row_to_insert) ``` **BigQuery Connector Documentaion** ``` class
-BigQuery(builtins.object) | BigQuery(read_big_query_project,
-write_big_query_project, service_account_file_path) | | BigQuery database
-utility functions | | Methods defined here: | | __init__(self,
-read_big_query_project, write_big_query_project, service_account_file_path) |
-initialisation method for BigQuery Connector | :param str
-read_big_query_project : project used while reading from BigQuery | :param str
-write_big_query_project: project used while writing into BigQuery | :param str
-service_account_file_path: project specific BigQuery Credential | | dump_data
-(self, database=None, table=None, dataframe=None, mode='append') | Dumps data
-into from BigQuery | :param string database: target bigquery database | :param
-string table: target table name | :param pd.DataFrame dataframe: pandas
-dataframe for dumping into bigquery | :param string mode: it can be either
-append or replace | | execute_query(self, query, query_config=None,
-timeout=900, max_retries=0, time_interval=5) | Executes query from from
-BigQuery table | :param string query: query for execution | :param string
-query_cofig: config for parameterised query | :param integer timeout : maximum
-bigquery execution timeout | :param string max_retries: maximum retries if data
-is not fetched | :param integer time_interval : time interval between retries |
-| get_data(self, query=None, query_config=None, max_retries=0, time_interval=5)
-| Fetches data from from BigQuery | :param string query: query for fetching
-data from table | :param string query_cofig: config for parameterised query | :
-param string max_retries: maximum retries if data is not fetched | :param
-integer time_interval : time interval between retries | | insert_rows_array
-(self, dataset=None, table=None, rows_to_insert=None) | Streaming insert into
-from BigQuery | :param string dataset: target bigquery database | :param string
-table: target table name | :param list rows_to_insert: list of dictionaries
-where each dictionary is a | row with keys as column names | |
-insert_rows_in_bigquery(self, dataset=None, table=None, rows_to_insert=None) |
-Streaming insert into from BigQuery | :param string dataset: target bigquery
-database | :param string table: target table name | :param rows_to_insert: list
-of dictionaries where each dictionary is a | row with keys as column names ```
---- ## 3. Configurer### 1. Profile Decorator**Code Snippet Sample :** ```python
-from custom_utils.configurer.profiler import profiler @profiler
+"select * from table_name" df = bq.pull_data(query) # Dumping Dataframe in
+BigQuery bq.push_data(database="rahul_temp", table="demo", dataframe=df,
+mode="append") # Executing any query in BigQuery query = "INSERT
+rahul_temp.Demo (id, userId) VALUES(1,1),(1,1)" BigQuery.execute_query(query) #
+Streaming insert in BigQuery row_to_insert = [{"id": 1, "userid": 1,
+"languageId": 58, "mode":0,"active":1}] BigQuery.insert_rows_in_bigquery
+(dataset="rahul_temp", table="Demo", rows_to_insert=row_to_insert) ```
+**BigQuery Connector Documentaion** ``` class BigQuery(builtins.object) |
+BigQuery(read_big_query_project, write_big_query_project,
+service_account_file_path) | | BigQuery database utility functions | | Methods
+defined here: | | __init__(self, read_big_query_project,
+write_big_query_project, service_account_file_path) | initialisation method for
+BigQuery Connector | :param str read_big_query_project : project used while
+reading from BigQuery | :param str write_big_query_project: project used while
+writing into BigQuery | :param str service_account_file_path: project specific
+BigQuery Credential | | push_data(self, database=None, table=None,
+dataframe=None, mode='append') | Dumps data into from BigQuery | :param string
+database: target bigquery database | :param string table: target table name | :
+param pd.DataFrame dataframe: pandas dataframe for dumping into bigquery | :
+param string mode: it can be either append or replace | | execute_query(self,
+query, job_config=None, timeout=900, max_retries=0, time_interval=5) | Executes
+query from from BigQuery table | :param string query: query for execution | :
+param string query_cofig: config for parameterised query | :param integer
+timeout : maximum bigquery execution timeout | :param string max_retries:
+maximum retries if data is not fetched | :param integer time_interval : time
+interval between retries | | pull_data(self, query=None, job_config=None,
+max_retries=0, time_interval=5) | Fetches data from from BigQuery | :param
+string query: query for fetching data from table | :param string query_cofig:
+config for parameterised query | :param string max_retries: maximum retries if
+data is not fetched | :param integer time_interval : time interval between
+retries | | insert_rows_array(self, dataset=None, table=None,
+rows_to_insert=None) | Streaming insert into from BigQuery | :param string
+dataset: target bigquery database | :param string table: target table name | :
+param list rows_to_insert: list of dictionaries where each dictionary is a |
+row with keys as column names | | insert_rows_in_bigquery(self, dataset=None,
+table=None, rows_to_insert=None) | Streaming insert into from BigQuery | :param
+string dataset: target bigquery database | :param string table: target table
+name | :param rows_to_insert: list of dictionaries where each dictionary is a |
+row with keys as column names ``` --- ## 3. Configurer### 1. Profile
+Decorator**Code Snippet Sample :** ```python from
+custom_utils.configurer.profiler import profiler @profiler
 (sort_by='cumulative', lines_to_print=10, strip_dirs=True) def
 product_counter_v3(): return [1, 2, 3, 4, 5] ``` **Profiler Documentaion**
 ```python def profiler(output_file=None, sort_by='cumulative',
 lines_to_print=None, strip_dirs=False): """ A time profiler decorator :param
 str output_file: Path of the output file. If only name of the file is given,
 it's saved in the current directory. If it's None, the name of the decorated
 function is used. :param str sort_by: SortKey enum or tuple/list of str/SortKey
@@ -157,36 +168,24 @@
 size of the printout, especially that sorting by 'cumulative', the time
 consuming operations are printed toward the top of the file. :param bool
 strip_dirs: Whether to remove the leading path info from file names. This is
 also useful in reducing the size of the printout :return: Profile of the
 decorated function """ ``` ### 2. Log Formatter**Code Snippet Sample :**
 ```python from custom_utils.configurer.utils import LogFormatter
 LogFormatter.apply() ``` **Log Formatter Documentation** ``` class LogFormatter
-(logging.Formatter): """Log Formatter class for trell ai usage""" __date_format
-= '%d/%b/%Y:%H:%M:%S %Z' @staticmethod def apply(level=logging.INFO): """ Start
-logging in json format. :return: ``` --- ## 4. Alerter### 1. Slack
-Alerter**Code Snippet Sample :** ``` from custom_utils.slack_alerter import
-Alerter try: """Write your code""" except: """Catch exceptions"""
-Alerter.send_alert(message=message, url=url, userId=userId, send_error=True)
-``` **Alerter Documentation :** ```python class Alerter(builtins.object) |
-Class for sending alerts and monitoring stats to a slack channel | | Static
-methods defined here: | | send_alert(message: str, url: str, user_id: str =
-None, send_error: bool = False) | This function send alert to a target channel
-tagging a user | with a alert message and traceback error. | args: | message :
-Pass the message to be displayed in the channel | url : Pass webhook of target
-channel | user_id : Slack user_id of user who needs to be tagged ( | send_error
-: This should be set True, | if slack_alert is called while catching exception
-| returns: Nothing | | send_monitoring_stats(start: tuple, stop: tuple,
-message: str, url: str, user_id: str = None) | This function send run time and
-RAM usage for a cronjob | to a target channel tagging a user with a message | |
-Args: | message : Pass the message to be displayed in the channel | url : Pass
-webhook of target channel | user_id : Slack user_id of user who needs to be
-tagged | start : this should be set to output of start_monitoring function |
-stop : this should be set to output of start_monitoring function | |
-start_monitoring() | function for initiating monitoring | | stop_monitoring() |
-function for end monitoring | | -----------------------------------------------
------------------------ ``` --- Platform: UNKNOWN Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.6.9 Description-Content-Type: text/markdown Provides-
-Extra: bigquery Provides-Extra: full Provides-Extra: mongodb Provides-Extra:
-mysql Provides-Extra: s3
+(logging.Formatter): """Log Formatter class for custom-utils package"""
+__date_format = '%d/%b/%Y:%H:%M:%S %Z' @staticmethod def apply
+(level=logging.INFO): """ Start logging in json format. :return: ``` --- ## 4.
+Alerter### 1. Slack Alerter**Code Snippet Sample :** ```python3 from
+custom_utils.alerter.slack import Slack slack = Slack(token=SLACK_BOT_TOKEN) #
+OR Slack() with SLACK_BOT_TOKEN as env variable channel="#shield" message =
+"testing" uids = ["U03PAP8C1RC", "U03PAP8C1RC"] slack.send_alert(channel,
+message, uids) ``` **Alerter Documentation :** ```python class Slack
+(builtins.object) | Slack(token=None) | | Class for sending alerts and
+monitoring stats to a slack channel | | Methods defined here: | | __init__
+(self, token=None) | Initialize self. See help(type(self)) for accurate
+signature. | | send_alert(self, channel: str, message: str, uids: list = []) |
+This function send alert to a target channel tagging a user | with a alert
+message and traceback error. | args: | channel : Name of the channel (ex :
+#channel_name) | message : Pass the message to be displayed in the channel |
+uids : List of Slack user_ids who needs to be tagged | | returns: Nothing | | -
+--------------------------------------------------------------------- ``` ---
```

### Comparing `custom-utils-0.0.2/setup.py` & `custom-utils-0.0.37/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 
 EXTRAS_REQUIRE = {
     's3' : [ 'boto', 'boto3', 'joblib'],
     'mysql':  ['SQLAlchemy', 'SQLAlchemy-JSONField',
                'SQLAlchemy-Utils', 'mysql-connector', 'mysql-replication',],
     'bigquery': ['tqdm==4.49.0','google-cloud-bigquery==2.1.0', 'pandas_gbq', 'google-cloud' ],
     'mongodb': ['pymongo==3.10.0'],
+    'slack': ['slack-sdk==3.21.3'],
 }
 
 # construct special 'full' extra that adds requirements for all built-in
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     author="Rahul Kumar",
     author_email="rahulnkumar7@gmail.com",
     name='custom-utils',
     description='Utilities for database connectors, slack alerter, loggers etc',
-    version="0.0.2",
+    version="0.0.37",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RahulnKumar/custom-utils',
     packages=find_packages(),
     python_requires=">=3.6.9",
-    install_requires=['requests', 'json-utils', 'python-dotenv', 'subprocess32', 'psutil',],
+    install_requires=['python-dotenv', 'subprocess32',],
     extras_require=EXTRAS_REQUIRE,
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Programming Language :: Python :: 3.6',
         'Topic :: Scientific/Engineering :: Artificial Intelligence'
     ],
 )
```

