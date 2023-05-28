# Comparing `tmp/pulp_ostree-client-2.0.0a7.dev1676776305.tar.gz` & `tmp/pulp_ostree-client-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_ostree-client-2.0.0a7.dev1676776305.tar", last modified: Sun Feb 19 03:11:56 2023, max compression
+gzip compressed data, was "pulp_ostree-client-2.1.0.tar", last modified: Sun May 28 21:30:16 2023, max compression
```

## Comparing `pulp_ostree-client-2.0.0a7.dev1676776305.tar` & `pulp_ostree-client-2.1.0.tar`

### file list

```diff
@@ -1,110 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.888874 pulp_ostree-client-2.0.0a7.dev1676776305/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-19 03:11:56.888874 pulp_ostree-client-2.0.0a7.dev1676776305/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.880874 pulp_ostree-client-2.0.0a7.dev1676776305/pulp_ostree_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-19 03:11:56.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulp_ostree_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-19 03:11:56.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulp_ostree_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 03:11:56.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulp_ostree_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-19 03:11:56.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulp_ostree_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-19 03:11:56.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulp_ostree_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.880874 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.880874 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.880874 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.884874 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15078 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_commits_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_objects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_refs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14814 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_summaries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    43198 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42462 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    70608 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32498 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.884874 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_import_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    29980 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    30373 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-19 03:11:56.892874 pulp_ostree-client-2.0.0a7.dev1676776305/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 03:11:56.888874 pulp_ostree-client-2.0.0a7.dev1676776305/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_commits_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_configs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_objects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_refs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_summaries_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_distributions_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_import_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_import_commits_to_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_commit_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_object_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_ref_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_commit_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_config_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_object_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_ref_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_summary_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_patchedostree_ostree_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_patchedostree_ostree_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_patchedostree_ostree_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_remotes_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repositories_ostree_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repositories_ostree_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-19 03:11:55.000000 pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repository_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13475 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 21:30:16.000000 pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.561306 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.565306 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_commits_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_content_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17576 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_objects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_refs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15840 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_summaries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47216 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73841 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33859 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26289 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13969 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.573306 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30086 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27467 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30479 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 21:30:16.581306 pulp_ostree-client-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_commits_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_configs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_content_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_objects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_refs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_content_summaries_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_distributions_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_import_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_import_commits_to_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_commit_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-28 21:30:14.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_object_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_ref_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_ostree_ostree_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_commit_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_config_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_object_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_ref_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_summary_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_remotes_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repositories_ostree_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repositories_ostree_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-28 21:30:15.000000 pulp_ostree-client-2.1.0/test/test_repository_version_response.py
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/README.md` & `pulp_ostree-client-2.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_ostree-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 2.0.0a7.dev1676776305
+- Package version: 2.1.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -84,24 +84,26 @@
 # Enter a context with an instance of the API client
 with pulpcore.client.pulp_ostree.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = pulpcore.client.pulp_ostree.ContentCommitsApi(api_client)
     checksum = 'checksum_example' # str | Filter results where checksum matches value (optional)
 limit = 56 # int | Number of results to return per page. (optional)
 offset = 56 # int | The initial index from which to return the results. (optional)
-ordering = ['ordering_example'] # list[str] | Ordering (optional)
+ordering = ['ordering_example'] # list[str] | Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `upstream_id` - Upstream id * `-upstream_id` - Upstream id (descending) * `timestamp_of_interest` - Timestamp of interest * `-timestamp_of_interest` - Timestamp of interest (descending) * `checksum` - Checksum * `-checksum` - Checksum (descending) * `relative_path` - Relative path * `-relative_path` - Relative path (descending) * `pk` - Pk * `-pk` - Pk (descending) (optional)
+pulp_href__in = ['pulp_href__in_example'] # list[str] | Multiple values may be separated by commas. (optional)
+pulp_id__in = ['pulp_id__in_example'] # list[str] | Multiple values may be separated by commas. (optional)
 repository_version = 'repository_version_example' # str | Repository Version referenced by HREF (optional)
 repository_version_added = 'repository_version_added_example' # str | Repository Version referenced by HREF (optional)
 repository_version_removed = 'repository_version_removed_example' # str | Repository Version referenced by HREF (optional)
 fields = ['fields_example'] # list[str] | A list of fields to include in the response. (optional)
 exclude_fields = ['exclude_fields_example'] # list[str] | A list of fields to exclude from the response. (optional)
 
     try:
         # List ostree commits
-        api_response = api_instance.list(checksum=checksum, limit=limit, offset=offset, ordering=ordering, repository_version=repository_version, repository_version_added=repository_version_added, repository_version_removed=repository_version_removed, fields=fields, exclude_fields=exclude_fields)
+        api_response = api_instance.list(checksum=checksum, limit=limit, offset=offset, ordering=ordering, pulp_href__in=pulp_href__in, pulp_id__in=pulp_id__in, repository_version=repository_version, repository_version_added=repository_version_added, repository_version_removed=repository_version_removed, fields=fields, exclude_fields=exclude_fields)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling ContentCommitsApi->list: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
@@ -110,14 +112,16 @@
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ContentCommitsApi* | [**list**](docs/ContentCommitsApi.md#list) | **GET** /pulp/api/v3/content/ostree/commits/ | List ostree commits
 *ContentCommitsApi* | [**read**](docs/ContentCommitsApi.md#read) | **GET** {ostree_ostree_commit_href} | Inspect an ostree commit
 *ContentConfigsApi* | [**list**](docs/ContentConfigsApi.md#list) | **GET** /pulp/api/v3/content/ostree/configs/ | List ostree configs
 *ContentConfigsApi* | [**read**](docs/ContentConfigsApi.md#read) | **GET** {ostree_ostree_config_href} | Inspect an ostree config
+*ContentContentApi* | [**list**](docs/ContentContentApi.md#list) | **GET** /pulp/api/v3/content/ostree/content/ | List ostree contents
+*ContentContentApi* | [**read**](docs/ContentContentApi.md#read) | **GET** {ostree_ostree_content_href} | Inspect an ostree content
 *ContentObjectsApi* | [**list**](docs/ContentObjectsApi.md#list) | **GET** /pulp/api/v3/content/ostree/objects/ | List ostree objects
 *ContentObjectsApi* | [**read**](docs/ContentObjectsApi.md#read) | **GET** {ostree_ostree_object_href} | Inspect an ostree object
 *ContentRefsApi* | [**list**](docs/ContentRefsApi.md#list) | **GET** /pulp/api/v3/content/ostree/refs/ | List ostree refs
 *ContentRefsApi* | [**read**](docs/ContentRefsApi.md#read) | **GET** {ostree_ostree_ref_href} | Inspect an ostree ref
 *ContentSummariesApi* | [**list**](docs/ContentSummariesApi.md#list) | **GET** /pulp/api/v3/content/ostree/summaries/ | List ostree summarys
 *ContentSummariesApi* | [**read**](docs/ContentSummariesApi.md#read) | **GET** {ostree_ostree_summary_href} | Inspect an ostree summary
 *DistributionsOstreeApi* | [**create**](docs/DistributionsOstreeApi.md#create) | **POST** /pulp/api/v3/distributions/ostree/ostree/ | Create an ostree distribution
@@ -152,39 +156,41 @@
 
  - [AsyncOperationResponse](docs/AsyncOperationResponse.md)
  - [ContentSummaryResponse](docs/ContentSummaryResponse.md)
  - [OstreeImportAll](docs/OstreeImportAll.md)
  - [OstreeImportCommitsToRef](docs/OstreeImportCommitsToRef.md)
  - [OstreeOstreeCommitResponse](docs/OstreeOstreeCommitResponse.md)
  - [OstreeOstreeConfigResponse](docs/OstreeOstreeConfigResponse.md)
+ - [OstreeOstreeContentResponse](docs/OstreeOstreeContentResponse.md)
  - [OstreeOstreeDistribution](docs/OstreeOstreeDistribution.md)
  - [OstreeOstreeDistributionResponse](docs/OstreeOstreeDistributionResponse.md)
  - [OstreeOstreeObjectResponse](docs/OstreeOstreeObjectResponse.md)
  - [OstreeOstreeRefResponse](docs/OstreeOstreeRefResponse.md)
  - [OstreeOstreeRemote](docs/OstreeOstreeRemote.md)
  - [OstreeOstreeRemoteResponse](docs/OstreeOstreeRemoteResponse.md)
  - [OstreeOstreeRemoteResponseHiddenFields](docs/OstreeOstreeRemoteResponseHiddenFields.md)
  - [OstreeOstreeRepository](docs/OstreeOstreeRepository.md)
  - [OstreeOstreeRepositoryResponse](docs/OstreeOstreeRepositoryResponse.md)
  - [OstreeOstreeSummaryResponse](docs/OstreeOstreeSummaryResponse.md)
- - [OstreeRepositoryAddRemoveContent](docs/OstreeRepositoryAddRemoveContent.md)
  - [PaginatedRepositoryVersionResponseList](docs/PaginatedRepositoryVersionResponseList.md)
  - [PaginatedostreeOstreeCommitResponseList](docs/PaginatedostreeOstreeCommitResponseList.md)
  - [PaginatedostreeOstreeConfigResponseList](docs/PaginatedostreeOstreeConfigResponseList.md)
+ - [PaginatedostreeOstreeContentResponseList](docs/PaginatedostreeOstreeContentResponseList.md)
  - [PaginatedostreeOstreeDistributionResponseList](docs/PaginatedostreeOstreeDistributionResponseList.md)
  - [PaginatedostreeOstreeObjectResponseList](docs/PaginatedostreeOstreeObjectResponseList.md)
  - [PaginatedostreeOstreeRefResponseList](docs/PaginatedostreeOstreeRefResponseList.md)
  - [PaginatedostreeOstreeRemoteResponseList](docs/PaginatedostreeOstreeRemoteResponseList.md)
  - [PaginatedostreeOstreeRepositoryResponseList](docs/PaginatedostreeOstreeRepositoryResponseList.md)
  - [PaginatedostreeOstreeSummaryResponseList](docs/PaginatedostreeOstreeSummaryResponseList.md)
  - [PatchedostreeOstreeDistribution](docs/PatchedostreeOstreeDistribution.md)
  - [PatchedostreeOstreeRemote](docs/PatchedostreeOstreeRemote.md)
  - [PatchedostreeOstreeRepository](docs/PatchedostreeOstreeRepository.md)
  - [PolicyEnum](docs/PolicyEnum.md)
  - [Repair](docs/Repair.md)
+ - [RepositoryAddRemoveContent](docs/RepositoryAddRemoveContent.md)
  - [RepositorySyncURL](docs/RepositorySyncURL.md)
  - [RepositoryVersionResponse](docs/RepositoryVersionResponse.md)
 
 
 ## Documentation For Authorization
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulp_ostree_client.egg-info/SOURCES.txt` & `pulp_ostree-client-2.1.0/pulp_ostree_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,90 +12,96 @@
 pulpcore/client/pulp_ostree/api_client.py
 pulpcore/client/pulp_ostree/configuration.py
 pulpcore/client/pulp_ostree/exceptions.py
 pulpcore/client/pulp_ostree/rest.py
 pulpcore/client/pulp_ostree/api/__init__.py
 pulpcore/client/pulp_ostree/api/content_commits_api.py
 pulpcore/client/pulp_ostree/api/content_configs_api.py
+pulpcore/client/pulp_ostree/api/content_content_api.py
 pulpcore/client/pulp_ostree/api/content_objects_api.py
 pulpcore/client/pulp_ostree/api/content_refs_api.py
 pulpcore/client/pulp_ostree/api/content_summaries_api.py
 pulpcore/client/pulp_ostree/api/distributions_ostree_api.py
 pulpcore/client/pulp_ostree/api/remotes_ostree_api.py
 pulpcore/client/pulp_ostree/api/repositories_ostree_api.py
 pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py
 pulpcore/client/pulp_ostree/models/__init__.py
 pulpcore/client/pulp_ostree/models/async_operation_response.py
 pulpcore/client/pulp_ostree/models/content_summary_response.py
 pulpcore/client/pulp_ostree/models/ostree_import_all.py
 pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py
+pulpcore/client/pulp_ostree/models/ostree_ostree_content_response.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py
 pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py
-pulpcore/client/pulp_ostree/models/ostree_repository_add_remove_content.py
 pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py
+pulpcore/client/pulp_ostree/models/paginatedostree_ostree_content_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py
 pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py
 pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py
 pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py
 pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py
 pulpcore/client/pulp_ostree/models/policy_enum.py
 pulpcore/client/pulp_ostree/models/repair.py
+pulpcore/client/pulp_ostree/models/repository_add_remove_content.py
 pulpcore/client/pulp_ostree/models/repository_sync_url.py
 pulpcore/client/pulp_ostree/models/repository_version_response.py
 test/test_async_operation_response.py
 test/test_content_commits_api.py
 test/test_content_configs_api.py
+test/test_content_content_api.py
 test/test_content_objects_api.py
 test/test_content_refs_api.py
 test/test_content_summaries_api.py
 test/test_content_summary_response.py
 test/test_distributions_ostree_api.py
 test/test_ostree_import_all.py
 test/test_ostree_import_commits_to_ref.py
 test/test_ostree_ostree_commit_response.py
 test/test_ostree_ostree_config_response.py
+test/test_ostree_ostree_content_response.py
 test/test_ostree_ostree_distribution.py
 test/test_ostree_ostree_distribution_response.py
 test/test_ostree_ostree_object_response.py
 test/test_ostree_ostree_ref_response.py
 test/test_ostree_ostree_remote.py
 test/test_ostree_ostree_remote_response.py
 test/test_ostree_ostree_remote_response_hidden_fields.py
 test/test_ostree_ostree_repository.py
 test/test_ostree_ostree_repository_response.py
 test/test_ostree_ostree_summary_response.py
-test/test_ostree_repository_add_remove_content.py
 test/test_paginated_repository_version_response_list.py
 test/test_paginatedostree_ostree_commit_response_list.py
 test/test_paginatedostree_ostree_config_response_list.py
+test/test_paginatedostree_ostree_content_response_list.py
 test/test_paginatedostree_ostree_distribution_response_list.py
 test/test_paginatedostree_ostree_object_response_list.py
 test/test_paginatedostree_ostree_ref_response_list.py
 test/test_paginatedostree_ostree_remote_response_list.py
 test/test_paginatedostree_ostree_repository_response_list.py
 test/test_paginatedostree_ostree_summary_response_list.py
 test/test_patchedostree_ostree_distribution.py
 test/test_patchedostree_ostree_remote.py
 test/test_patchedostree_ostree_repository.py
 test/test_policy_enum.py
 test/test_remotes_ostree_api.py
 test/test_repair.py
 test/test_repositories_ostree_api.py
 test/test_repositories_ostree_versions_api.py
+test/test_repository_add_remove_content.py
 test/test_repository_sync_url.py
 test/test_repository_version_response.py
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/__init__.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.0.0a7.dev1676776305"
+__version__ = "2.1.0"
 
 # import apis into sdk package
 from pulpcore.client.pulp_ostree.api.content_commits_api import ContentCommitsApi
 from pulpcore.client.pulp_ostree.api.content_configs_api import ContentConfigsApi
+from pulpcore.client.pulp_ostree.api.content_content_api import ContentContentApi
 from pulpcore.client.pulp_ostree.api.content_objects_api import ContentObjectsApi
 from pulpcore.client.pulp_ostree.api.content_refs_api import ContentRefsApi
 from pulpcore.client.pulp_ostree.api.content_summaries_api import ContentSummariesApi
 from pulpcore.client.pulp_ostree.api.distributions_ostree_api import DistributionsOstreeApi
 from pulpcore.client.pulp_ostree.api.remotes_ostree_api import RemotesOstreeApi
 from pulpcore.client.pulp_ostree.api.repositories_ostree_api import RepositoriesOstreeApi
 from pulpcore.client.pulp_ostree.api.repositories_ostree_versions_api import RepositoriesOstreeVersionsApi
@@ -39,35 +40,37 @@
 # import models into sdk package
 from pulpcore.client.pulp_ostree.models.async_operation_response import AsyncOperationResponse
 from pulpcore.client.pulp_ostree.models.content_summary_response import ContentSummaryResponse
 from pulpcore.client.pulp_ostree.models.ostree_import_all import OstreeImportAll
 from pulpcore.client.pulp_ostree.models.ostree_import_commits_to_ref import OstreeImportCommitsToRef
 from pulpcore.client.pulp_ostree.models.ostree_ostree_commit_response import OstreeOstreeCommitResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_config_response import OstreeOstreeConfigResponse
+from pulpcore.client.pulp_ostree.models.ostree_ostree_content_response import OstreeOstreeContentResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_distribution import OstreeOstreeDistribution
 from pulpcore.client.pulp_ostree.models.ostree_ostree_distribution_response import OstreeOstreeDistributionResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_object_response import OstreeOstreeObjectResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_ref_response import OstreeOstreeRefResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_remote import OstreeOstreeRemote
 from pulpcore.client.pulp_ostree.models.ostree_ostree_remote_response import OstreeOstreeRemoteResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_remote_response_hidden_fields import OstreeOstreeRemoteResponseHiddenFields
 from pulpcore.client.pulp_ostree.models.ostree_ostree_repository import OstreeOstreeRepository
 from pulpcore.client.pulp_ostree.models.ostree_ostree_repository_response import OstreeOstreeRepositoryResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_summary_response import OstreeOstreeSummaryResponse
-from pulpcore.client.pulp_ostree.models.ostree_repository_add_remove_content import OstreeRepositoryAddRemoveContent
 from pulpcore.client.pulp_ostree.models.paginated_repository_version_response_list import PaginatedRepositoryVersionResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_commit_response_list import PaginatedostreeOstreeCommitResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_config_response_list import PaginatedostreeOstreeConfigResponseList
+from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_content_response_list import PaginatedostreeOstreeContentResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_distribution_response_list import PaginatedostreeOstreeDistributionResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_object_response_list import PaginatedostreeOstreeObjectResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_ref_response_list import PaginatedostreeOstreeRefResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_remote_response_list import PaginatedostreeOstreeRemoteResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_repository_response_list import PaginatedostreeOstreeRepositoryResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_summary_response_list import PaginatedostreeOstreeSummaryResponseList
 from pulpcore.client.pulp_ostree.models.patchedostree_ostree_distribution import PatchedostreeOstreeDistribution
 from pulpcore.client.pulp_ostree.models.patchedostree_ostree_remote import PatchedostreeOstreeRemote
 from pulpcore.client.pulp_ostree.models.patchedostree_ostree_repository import PatchedostreeOstreeRepository
 from pulpcore.client.pulp_ostree.models.policy_enum import PolicyEnum
 from pulpcore.client.pulp_ostree.models.repair import Repair
+from pulpcore.client.pulp_ostree.models.repository_add_remove_content import RepositoryAddRemoveContent
 from pulpcore.client.pulp_ostree.models.repository_sync_url import RepositorySyncURL
 from pulpcore.client.pulp_ostree.models.repository_version_response import RepositoryVersionResponse
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/__init__.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
 from pulpcore.client.pulp_ostree.api.content_commits_api import ContentCommitsApi
 from pulpcore.client.pulp_ostree.api.content_configs_api import ContentConfigsApi
+from pulpcore.client.pulp_ostree.api.content_content_api import ContentContentApi
 from pulpcore.client.pulp_ostree.api.content_objects_api import ContentObjectsApi
 from pulpcore.client.pulp_ostree.api.content_refs_api import ContentRefsApi
 from pulpcore.client.pulp_ostree.api.content_summaries_api import ContentSummariesApi
 from pulpcore.client.pulp_ostree.api.distributions_ostree_api import DistributionsOstreeApi
 from pulpcore.client.pulp_ostree.api.remotes_ostree_api import RemotesOstreeApi
 from pulpcore.client.pulp_ostree.api.repositories_ostree_api import RepositoriesOstreeApi
 from pulpcore.client.pulp_ostree.api.repositories_ostree_versions_api import RepositoriesOstreeVersionsApi
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_commits_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_configs_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,99 +21,102 @@
 from pulpcore.client.pulp_ostree.api_client import ApiClient
 from pulpcore.client.pulp_ostree.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ContentCommitsApi(object):
+class ContentConfigsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def list(self, **kwargs):  # noqa: E501
-        """List ostree commits  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
+        """List ostree configs  # noqa: E501
 
-        A ViewSet class for OSTree commits.  # noqa: E501
+        A ViewSet class for OSTree repository configurations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str checksum: Filter results where checksum matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: PaginatedostreeOstreeCommitResponseList
+        :return: PaginatedostreeOstreeConfigResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
-        """List ostree commits  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
+        """List ostree configs  # noqa: E501
 
-        A ViewSet class for OSTree commits.  # noqa: E501
+        A ViewSet class for OSTree repository configurations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str checksum: Filter results where checksum matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(PaginatedostreeOstreeCommitResponseList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PaginatedostreeOstreeConfigResponseList, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'checksum',
             'limit',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'repository_version',
             'repository_version_added',
             'repository_version_removed',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
@@ -135,23 +138,27 @@
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'checksum' in local_var_params and local_var_params['checksum'] is not None:  # noqa: E501
-            query_params.append(('checksum', local_var_params['checksum']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'repository_version' in local_var_params and local_var_params['repository_version'] is not None:  # noqa: E501
             query_params.append(('repository_version', local_var_params['repository_version']))  # noqa: E501
         if 'repository_version_added' in local_var_params and local_var_params['repository_version_added'] is not None:  # noqa: E501
             query_params.append(('repository_version_added', local_var_params['repository_version_added']))  # noqa: E501
         if 'repository_version_removed' in local_var_params and local_var_params['repository_version_removed'] is not None:  # noqa: E501
             query_params.append(('repository_version_removed', local_var_params['repository_version_removed']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
@@ -171,87 +178,87 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/content/ostree/commits/', 'GET',
+            '/pulp/api/v3/content/ostree/configs/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedostreeOstreeCommitResponseList',  # noqa: E501
+            response_type='PaginatedostreeOstreeConfigResponseList',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_commit_href, **kwargs):  # noqa: E501
-        """Inspect an ostree commit  # noqa: E501
+    def read(self, ostree_ostree_config_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree config  # noqa: E501
 
-        A ViewSet class for OSTree commits.  # noqa: E501
+        A ViewSet class for OSTree repository configurations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read(ostree_ostree_commit_href, async_req=True)
+        >>> thread = api.read(ostree_ostree_config_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_commit_href: (required)
+        :param str ostree_ostree_config_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: OstreeOstreeCommitResponse
+        :return: OstreeOstreeConfigResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_commit_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_config_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_commit_href, **kwargs):  # noqa: E501
-        """Inspect an ostree commit  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_config_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree config  # noqa: E501
 
-        A ViewSet class for OSTree commits.  # noqa: E501
+        A ViewSet class for OSTree repository configurations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read_with_http_info(ostree_ostree_commit_href, async_req=True)
+        >>> thread = api.read_with_http_info(ostree_ostree_config_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_commit_href: (required)
+        :param str ostree_ostree_config_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(OstreeOstreeCommitResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(OstreeOstreeConfigResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'ostree_ostree_commit_href',
+            'ostree_ostree_config_href',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -264,24 +271,24 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method read" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'ostree_ostree_commit_href' is set
-        if self.api_client.client_side_validation and ('ostree_ostree_commit_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['ostree_ostree_commit_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `ostree_ostree_commit_href` when calling `read`")  # noqa: E501
+        # verify the required parameter 'ostree_ostree_config_href' is set
+        if self.api_client.client_side_validation and ('ostree_ostree_config_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['ostree_ostree_config_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `ostree_ostree_config_href` when calling `read`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'ostree_ostree_commit_href' in local_var_params:
-            path_params['ostree_ostree_commit_href'] = local_var_params['ostree_ostree_commit_href']  # noqa: E501
+        if 'ostree_ostree_config_href' in local_var_params:
+            path_params['ostree_ostree_config_href'] = local_var_params['ostree_ostree_config_href']  # noqa: E501
 
         query_params = []
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
@@ -297,21 +304,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{ostree_ostree_commit_href}', 'GET',
+            '{ostree_ostree_config_href}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='OstreeOstreeCommitResponse',  # noqa: E501
+            response_type='OstreeOstreeConfigResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_configs_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_content_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,96 +21,102 @@
 from pulpcore.client.pulp_ostree.api_client import ApiClient
 from pulpcore.client.pulp_ostree.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ContentConfigsApi(object):
+class ContentContentApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def list(self, **kwargs):  # noqa: E501
-        """List ostree configs  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
+        """List ostree contents  # noqa: E501
 
-        A ViewSet class for OSTree repository configurations.  # noqa: E501
+        A ViewSet class for uncategorized content units (e.g., static deltas).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: PaginatedostreeOstreeConfigResponseList
+        :return: PaginatedostreeOstreeContentResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
-        """List ostree configs  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
+        """List ostree contents  # noqa: E501
 
-        A ViewSet class for OSTree repository configurations.  # noqa: E501
+        A ViewSet class for uncategorized content units (e.g., static deltas).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(PaginatedostreeOstreeConfigResponseList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PaginatedostreeOstreeContentResponseList, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'limit',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'repository_version',
             'repository_version_added',
             'repository_version_removed',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
@@ -139,14 +145,20 @@
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'repository_version' in local_var_params and local_var_params['repository_version'] is not None:  # noqa: E501
             query_params.append(('repository_version', local_var_params['repository_version']))  # noqa: E501
         if 'repository_version_added' in local_var_params and local_var_params['repository_version_added'] is not None:  # noqa: E501
             query_params.append(('repository_version_added', local_var_params['repository_version_added']))  # noqa: E501
         if 'repository_version_removed' in local_var_params and local_var_params['repository_version_removed'] is not None:  # noqa: E501
             query_params.append(('repository_version_removed', local_var_params['repository_version_removed']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
@@ -166,87 +178,87 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/content/ostree/configs/', 'GET',
+            '/pulp/api/v3/content/ostree/content/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedostreeOstreeConfigResponseList',  # noqa: E501
+            response_type='PaginatedostreeOstreeContentResponseList',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_config_href, **kwargs):  # noqa: E501
-        """Inspect an ostree config  # noqa: E501
+    def read(self, ostree_ostree_content_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree content  # noqa: E501
 
-        A ViewSet class for OSTree repository configurations.  # noqa: E501
+        A ViewSet class for uncategorized content units (e.g., static deltas).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read(ostree_ostree_config_href, async_req=True)
+        >>> thread = api.read(ostree_ostree_content_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_config_href: (required)
+        :param str ostree_ostree_content_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: OstreeOstreeConfigResponse
+        :return: OstreeOstreeContentResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_config_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_content_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_config_href, **kwargs):  # noqa: E501
-        """Inspect an ostree config  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_content_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree content  # noqa: E501
 
-        A ViewSet class for OSTree repository configurations.  # noqa: E501
+        A ViewSet class for uncategorized content units (e.g., static deltas).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read_with_http_info(ostree_ostree_config_href, async_req=True)
+        >>> thread = api.read_with_http_info(ostree_ostree_content_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_config_href: (required)
+        :param str ostree_ostree_content_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(OstreeOstreeConfigResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(OstreeOstreeContentResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'ostree_ostree_config_href',
+            'ostree_ostree_content_href',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -259,24 +271,24 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method read" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'ostree_ostree_config_href' is set
-        if self.api_client.client_side_validation and ('ostree_ostree_config_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['ostree_ostree_config_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `ostree_ostree_config_href` when calling `read`")  # noqa: E501
+        # verify the required parameter 'ostree_ostree_content_href' is set
+        if self.api_client.client_side_validation and ('ostree_ostree_content_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['ostree_ostree_content_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `ostree_ostree_content_href` when calling `read`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'ostree_ostree_config_href' in local_var_params:
-            path_params['ostree_ostree_config_href'] = local_var_params['ostree_ostree_config_href']  # noqa: E501
+        if 'ostree_ostree_content_href' in local_var_params:
+            path_params['ostree_ostree_content_href'] = local_var_params['ostree_ostree_content_href']  # noqa: E501
 
         query_params = []
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
@@ -292,21 +304,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{ostree_ostree_config_href}', 'GET',
+            '{ostree_ostree_content_href}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='OstreeOstreeConfigResponse',  # noqa: E501
+            response_type='OstreeOstreeContentResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_objects_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_summaries_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,99 +21,102 @@
 from pulpcore.client.pulp_ostree.api_client import ApiClient
 from pulpcore.client.pulp_ostree.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ContentObjectsApi(object):
+class ContentSummariesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def list(self, **kwargs):  # noqa: E501
-        """List ostree objects  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
+        """List ostree summarys  # noqa: E501
 
-        A ViewSet class for OSTree objects (e.g., dirtree, dirmeta, file).  # noqa: E501
+        A ViewSet class for OSTree repository summary files.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str checksum: Filter results where checksum matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: PaginatedostreeOstreeObjectResponseList
+        :return: PaginatedostreeOstreeSummaryResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
-        """List ostree objects  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
+        """List ostree summarys  # noqa: E501
 
-        A ViewSet class for OSTree objects (e.g., dirtree, dirmeta, file).  # noqa: E501
+        A ViewSet class for OSTree repository summary files.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str checksum: Filter results where checksum matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(PaginatedostreeOstreeObjectResponseList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PaginatedostreeOstreeSummaryResponseList, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'checksum',
             'limit',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'repository_version',
             'repository_version_added',
             'repository_version_removed',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
@@ -135,23 +138,27 @@
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'checksum' in local_var_params and local_var_params['checksum'] is not None:  # noqa: E501
-            query_params.append(('checksum', local_var_params['checksum']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'repository_version' in local_var_params and local_var_params['repository_version'] is not None:  # noqa: E501
             query_params.append(('repository_version', local_var_params['repository_version']))  # noqa: E501
         if 'repository_version_added' in local_var_params and local_var_params['repository_version_added'] is not None:  # noqa: E501
             query_params.append(('repository_version_added', local_var_params['repository_version_added']))  # noqa: E501
         if 'repository_version_removed' in local_var_params and local_var_params['repository_version_removed'] is not None:  # noqa: E501
             query_params.append(('repository_version_removed', local_var_params['repository_version_removed']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
@@ -171,87 +178,87 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/content/ostree/objects/', 'GET',
+            '/pulp/api/v3/content/ostree/summaries/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedostreeOstreeObjectResponseList',  # noqa: E501
+            response_type='PaginatedostreeOstreeSummaryResponseList',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_object_href, **kwargs):  # noqa: E501
-        """Inspect an ostree object  # noqa: E501
+    def read(self, ostree_ostree_summary_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree summary  # noqa: E501
 
-        A ViewSet class for OSTree objects (e.g., dirtree, dirmeta, file).  # noqa: E501
+        A ViewSet class for OSTree repository summary files.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read(ostree_ostree_object_href, async_req=True)
+        >>> thread = api.read(ostree_ostree_summary_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_object_href: (required)
+        :param str ostree_ostree_summary_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: OstreeOstreeObjectResponse
+        :return: OstreeOstreeSummaryResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_object_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_summary_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_object_href, **kwargs):  # noqa: E501
-        """Inspect an ostree object  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_summary_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree summary  # noqa: E501
 
-        A ViewSet class for OSTree objects (e.g., dirtree, dirmeta, file).  # noqa: E501
+        A ViewSet class for OSTree repository summary files.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read_with_http_info(ostree_ostree_object_href, async_req=True)
+        >>> thread = api.read_with_http_info(ostree_ostree_summary_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_object_href: (required)
+        :param str ostree_ostree_summary_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(OstreeOstreeObjectResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(OstreeOstreeSummaryResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'ostree_ostree_object_href',
+            'ostree_ostree_summary_href',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -264,24 +271,24 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method read" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'ostree_ostree_object_href' is set
-        if self.api_client.client_side_validation and ('ostree_ostree_object_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['ostree_ostree_object_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `ostree_ostree_object_href` when calling `read`")  # noqa: E501
+        # verify the required parameter 'ostree_ostree_summary_href' is set
+        if self.api_client.client_side_validation and ('ostree_ostree_summary_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['ostree_ostree_summary_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `ostree_ostree_summary_href` when calling `read`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'ostree_ostree_object_href' in local_var_params:
-            path_params['ostree_ostree_object_href'] = local_var_params['ostree_ostree_object_href']  # noqa: E501
+        if 'ostree_ostree_summary_href' in local_var_params:
+            path_params['ostree_ostree_summary_href'] = local_var_params['ostree_ostree_summary_href']  # noqa: E501
 
         query_params = []
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
@@ -297,21 +304,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{ostree_ostree_object_href}', 'GET',
+            '{ostree_ostree_summary_href}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='OstreeOstreeObjectResponse',  # noqa: E501
+            response_type='OstreeOstreeSummaryResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_refs_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_refs_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def list(self, **kwargs):  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
         """List ostree refs  # noqa: E501
 
         A ViewSet class for OSTree head commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
@@ -51,15 +51,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `upstream_id` - Upstream id * `-upstream_id` - Upstream id (descending) * `timestamp_of_interest` - Timestamp of interest * `-timestamp_of_interest` - Timestamp of interest (descending) * `name` - Name * `-name` - Name (descending) * `relative_path` - Relative path * `-relative_path` - Relative path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -69,17 +71,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: PaginatedostreeOstreeRefResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
         """List ostree refs  # noqa: E501
 
         A ViewSet class for OSTree head commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
@@ -89,15 +91,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `upstream_id` - Upstream id * `-upstream_id` - Upstream id (descending) * `timestamp_of_interest` - Timestamp of interest * `-timestamp_of_interest` - Timestamp of interest (descending) * `name` - Name * `-name` - Name (descending) * `relative_path` - Relative path * `-relative_path` - Relative path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
@@ -121,14 +125,16 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'repository_version',
             'repository_version_added',
             'repository_version_removed',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
@@ -170,14 +176,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'repository_version' in local_var_params and local_var_params['repository_version'] is not None:  # noqa: E501
             query_params.append(('repository_version', local_var_params['repository_version']))  # noqa: E501
         if 'repository_version_added' in local_var_params and local_var_params['repository_version_added'] is not None:  # noqa: E501
             query_params.append(('repository_version_added', local_var_params['repository_version_added']))  # noqa: E501
         if 'repository_version_removed' in local_var_params and local_var_params['repository_version_removed'] is not None:  # noqa: E501
             query_params.append(('repository_version_removed', local_var_params['repository_version_removed']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
@@ -212,15 +224,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_ref_href, **kwargs):  # noqa: E501
+    def read(self, ostree_ostree_ref_href,  **kwargs):  # noqa: E501
         """Inspect an ostree ref  # noqa: E501
 
         A ViewSet class for OSTree head commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read(ostree_ostree_ref_href, async_req=True)
         >>> result = thread.get()
@@ -237,17 +249,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: OstreeOstreeRefResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_ref_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_ref_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_ref_href, **kwargs):  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_ref_href,  **kwargs):  # noqa: E501
         """Inspect an ostree ref  # noqa: E501
 
         A ViewSet class for OSTree head commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_with_http_info(ostree_ostree_ref_href, async_req=True)
         >>> result = thread.get()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/content_summaries_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/content_commits_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,96 +21,105 @@
 from pulpcore.client.pulp_ostree.api_client import ApiClient
 from pulpcore.client.pulp_ostree.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ContentSummariesApi(object):
+class ContentCommitsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def list(self, **kwargs):  # noqa: E501
-        """List ostree summarys  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
+        """List ostree commits  # noqa: E501
 
-        A ViewSet class for OSTree repository summary files.  # noqa: E501
+        A ViewSet class for OSTree commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str checksum: Filter results where checksum matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `upstream_id` - Upstream id * `-upstream_id` - Upstream id (descending) * `timestamp_of_interest` - Timestamp of interest * `-timestamp_of_interest` - Timestamp of interest (descending) * `checksum` - Checksum * `-checksum` - Checksum (descending) * `relative_path` - Relative path * `-relative_path` - Relative path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: PaginatedostreeOstreeSummaryResponseList
+        :return: PaginatedostreeOstreeCommitResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
-        """List ostree summarys  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
+        """List ostree commits  # noqa: E501
 
-        A ViewSet class for OSTree repository summary files.  # noqa: E501
+        A ViewSet class for OSTree commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str checksum: Filter results where checksum matches value
         :param int limit: Number of results to return per page.
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `upstream_id` - Upstream id * `-upstream_id` - Upstream id (descending) * `timestamp_of_interest` - Timestamp of interest * `-timestamp_of_interest` - Timestamp of interest (descending) * `checksum` - Checksum * `-checksum` - Checksum (descending) * `relative_path` - Relative path * `-relative_path` - Relative path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str repository_version: Repository Version referenced by HREF
         :param str repository_version_added: Repository Version referenced by HREF
         :param str repository_version_removed: Repository Version referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(PaginatedostreeOstreeSummaryResponseList, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(PaginatedostreeOstreeCommitResponseList, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'checksum',
             'limit',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'repository_version',
             'repository_version_added',
             'repository_version_removed',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
@@ -132,21 +141,29 @@
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'checksum' in local_var_params and local_var_params['checksum'] is not None:  # noqa: E501
+            query_params.append(('checksum', local_var_params['checksum']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'repository_version' in local_var_params and local_var_params['repository_version'] is not None:  # noqa: E501
             query_params.append(('repository_version', local_var_params['repository_version']))  # noqa: E501
         if 'repository_version_added' in local_var_params and local_var_params['repository_version_added'] is not None:  # noqa: E501
             query_params.append(('repository_version_added', local_var_params['repository_version_added']))  # noqa: E501
         if 'repository_version_removed' in local_var_params and local_var_params['repository_version_removed'] is not None:  # noqa: E501
             query_params.append(('repository_version_removed', local_var_params['repository_version_removed']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
@@ -166,87 +183,87 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '/pulp/api/v3/content/ostree/summaries/', 'GET',
+            '/pulp/api/v3/content/ostree/commits/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedostreeOstreeSummaryResponseList',  # noqa: E501
+            response_type='PaginatedostreeOstreeCommitResponseList',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_summary_href, **kwargs):  # noqa: E501
-        """Inspect an ostree summary  # noqa: E501
+    def read(self, ostree_ostree_commit_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree commit  # noqa: E501
 
-        A ViewSet class for OSTree repository summary files.  # noqa: E501
+        A ViewSet class for OSTree commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read(ostree_ostree_summary_href, async_req=True)
+        >>> thread = api.read(ostree_ostree_commit_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_summary_href: (required)
+        :param str ostree_ostree_commit_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: OstreeOstreeSummaryResponse
+        :return: OstreeOstreeCommitResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_summary_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_commit_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_summary_href, **kwargs):  # noqa: E501
-        """Inspect an ostree summary  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_commit_href,  **kwargs):  # noqa: E501
+        """Inspect an ostree commit  # noqa: E501
 
-        A ViewSet class for OSTree repository summary files.  # noqa: E501
+        A ViewSet class for OSTree commits.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.read_with_http_info(ostree_ostree_summary_href, async_req=True)
+        >>> thread = api.read_with_http_info(ostree_ostree_commit_href, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
-        :param str ostree_ostree_summary_href: (required)
+        :param str ostree_ostree_commit_href: (required)
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
-        :return: tuple(OstreeOstreeSummaryResponse, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(OstreeOstreeCommitResponse, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
-            'ostree_ostree_summary_href',
+            'ostree_ostree_commit_href',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -259,24 +276,24 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method read" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
-        # verify the required parameter 'ostree_ostree_summary_href' is set
-        if self.api_client.client_side_validation and ('ostree_ostree_summary_href' not in local_var_params or  # noqa: E501
-                                                        local_var_params['ostree_ostree_summary_href'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `ostree_ostree_summary_href` when calling `read`")  # noqa: E501
+        # verify the required parameter 'ostree_ostree_commit_href' is set
+        if self.api_client.client_side_validation and ('ostree_ostree_commit_href' not in local_var_params or  # noqa: E501
+                                                        local_var_params['ostree_ostree_commit_href'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `ostree_ostree_commit_href` when calling `read`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'ostree_ostree_summary_href' in local_var_params:
-            path_params['ostree_ostree_summary_href'] = local_var_params['ostree_ostree_summary_href']  # noqa: E501
+        if 'ostree_ostree_commit_href' in local_var_params:
+            path_params['ostree_ostree_commit_href'] = local_var_params['ostree_ostree_commit_href']  # noqa: E501
 
         query_params = []
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
@@ -292,21 +309,21 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
-            '{ostree_ostree_summary_href}', 'GET',
+            '{ostree_ostree_commit_href}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='OstreeOstreeSummaryResponse',  # noqa: E501
+            response_type='OstreeOstreeCommitResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/distributions_ostree_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create(self, ostree_ostree_distribution, **kwargs):  # noqa: E501
+    def create(self, ostree_ostree_distribution,  **kwargs):  # noqa: E501
         """Create an ostree distribution  # noqa: E501
 
         Trigger an asynchronous create task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create(ostree_ostree_distribution, async_req=True)
         >>> result = thread.get()
@@ -56,17 +56,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_with_http_info(ostree_ostree_distribution, **kwargs)  # noqa: E501
+        return self.create_with_http_info(ostree_ostree_distribution,  **kwargs)  # noqa: E501
 
-    def create_with_http_info(self, ostree_ostree_distribution, **kwargs):  # noqa: E501
+    def create_with_http_info(self, ostree_ostree_distribution,  **kwargs):  # noqa: E501
         """Create an ostree distribution  # noqa: E501
 
         Trigger an asynchronous create task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_with_http_info(ostree_ostree_distribution, async_req=True)
         >>> result = thread.get()
@@ -151,15 +151,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete(self, ostree_ostree_distribution_href, **kwargs):  # noqa: E501
+    def delete(self, ostree_ostree_distribution_href,  **kwargs):  # noqa: E501
         """Delete an ostree distribution  # noqa: E501
 
         Trigger an asynchronous delete task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete(ostree_ostree_distribution_href, async_req=True)
         >>> result = thread.get()
@@ -174,17 +174,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_with_http_info(ostree_ostree_distribution_href, **kwargs)  # noqa: E501
+        return self.delete_with_http_info(ostree_ostree_distribution_href,  **kwargs)  # noqa: E501
 
-    def delete_with_http_info(self, ostree_ostree_distribution_href, **kwargs):  # noqa: E501
+    def delete_with_http_info(self, ostree_ostree_distribution_href,  **kwargs):  # noqa: E501
         """Delete an ostree distribution  # noqa: E501
 
         Trigger an asynchronous delete task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_with_http_info(ostree_ostree_distribution_href, async_req=True)
         >>> result = thread.get()
@@ -265,15 +265,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list(self, **kwargs):  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
         """List ostree distributions  # noqa: E501
 
         A ViewSet class for OSTree distributions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
@@ -286,15 +286,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str repository: Filter results where repository matches value
         :param list[str] repository__in: Filter results where repository is in a comma-separated list of values
         :param str with_content: Filter distributions based on the content served by them
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -305,17 +307,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: PaginatedostreeOstreeDistributionResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
         """List ostree distributions  # noqa: E501
 
         A ViewSet class for OSTree distributions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
@@ -328,15 +330,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `base_path` - Base path * `-base_path` - Base path (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str repository: Filter results where repository matches value
         :param list[str] repository__in: Filter results where repository is in a comma-separated list of values
         :param str with_content: Filter distributions based on the content served by them
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
@@ -364,14 +368,16 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'pulp_label_select',
             'repository',
             'repository__in',
             'with_content',
             'fields',
             'exclude_fields'
         ]
@@ -421,14 +427,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
             query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'repository' in local_var_params and local_var_params['repository'] is not None:  # noqa: E501
             query_params.append(('repository', local_var_params['repository']))  # noqa: E501
         if 'repository__in' in local_var_params and local_var_params['repository__in'] is not None:  # noqa: E501
             query_params.append(('repository__in', local_var_params['repository__in']))  # noqa: E501
             collection_formats['repository__in'] = 'csv'  # noqa: E501
@@ -466,15 +478,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def partial_update(self, ostree_ostree_distribution_href, patchedostree_ostree_distribution, **kwargs):  # noqa: E501
+    def partial_update(self, ostree_ostree_distribution_href, patchedostree_ostree_distribution,  **kwargs):  # noqa: E501
         """Update an ostree distribution  # noqa: E501
 
         Trigger an asynchronous partial update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.partial_update(ostree_ostree_distribution_href, patchedostree_ostree_distribution, async_req=True)
         >>> result = thread.get()
@@ -490,17 +502,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.partial_update_with_http_info(ostree_ostree_distribution_href, patchedostree_ostree_distribution, **kwargs)  # noqa: E501
+        return self.partial_update_with_http_info(ostree_ostree_distribution_href, patchedostree_ostree_distribution,  **kwargs)  # noqa: E501
 
-    def partial_update_with_http_info(self, ostree_ostree_distribution_href, patchedostree_ostree_distribution, **kwargs):  # noqa: E501
+    def partial_update_with_http_info(self, ostree_ostree_distribution_href, patchedostree_ostree_distribution,  **kwargs):  # noqa: E501
         """Update an ostree distribution  # noqa: E501
 
         Trigger an asynchronous partial update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.partial_update_with_http_info(ostree_ostree_distribution_href, patchedostree_ostree_distribution, async_req=True)
         >>> result = thread.get()
@@ -593,15 +605,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_distribution_href, **kwargs):  # noqa: E501
+    def read(self, ostree_ostree_distribution_href,  **kwargs):  # noqa: E501
         """Inspect an ostree distribution  # noqa: E501
 
         A ViewSet class for OSTree distributions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read(ostree_ostree_distribution_href, async_req=True)
         >>> result = thread.get()
@@ -618,17 +630,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: OstreeOstreeDistributionResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_distribution_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_distribution_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_distribution_href, **kwargs):  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_distribution_href,  **kwargs):  # noqa: E501
         """Inspect an ostree distribution  # noqa: E501
 
         A ViewSet class for OSTree distributions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_with_http_info(ostree_ostree_distribution_href, async_req=True)
         >>> result = thread.get()
@@ -719,15 +731,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update(self, ostree_ostree_distribution_href, ostree_ostree_distribution, **kwargs):  # noqa: E501
+    def update(self, ostree_ostree_distribution_href, ostree_ostree_distribution,  **kwargs):  # noqa: E501
         """Update an ostree distribution  # noqa: E501
 
         Trigger an asynchronous update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update(ostree_ostree_distribution_href, ostree_ostree_distribution, async_req=True)
         >>> result = thread.get()
@@ -743,17 +755,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_with_http_info(ostree_ostree_distribution_href, ostree_ostree_distribution, **kwargs)  # noqa: E501
+        return self.update_with_http_info(ostree_ostree_distribution_href, ostree_ostree_distribution,  **kwargs)  # noqa: E501
 
-    def update_with_http_info(self, ostree_ostree_distribution_href, ostree_ostree_distribution, **kwargs):  # noqa: E501
+    def update_with_http_info(self, ostree_ostree_distribution_href, ostree_ostree_distribution,  **kwargs):  # noqa: E501
         """Update an ostree distribution  # noqa: E501
 
         Trigger an asynchronous update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_with_http_info(ostree_ostree_distribution_href, ostree_ostree_distribution, async_req=True)
         >>> result = thread.get()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/remotes_ostree_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create(self, ostree_ostree_remote, **kwargs):  # noqa: E501
+    def create(self, ostree_ostree_remote,  **kwargs):  # noqa: E501
         """Create an ostree remote  # noqa: E501
 
         A ViewSet class for OSTree remote repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create(ostree_ostree_remote, async_req=True)
         >>> result = thread.get()
@@ -56,17 +56,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: OstreeOstreeRemoteResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_with_http_info(ostree_ostree_remote, **kwargs)  # noqa: E501
+        return self.create_with_http_info(ostree_ostree_remote,  **kwargs)  # noqa: E501
 
-    def create_with_http_info(self, ostree_ostree_remote, **kwargs):  # noqa: E501
+    def create_with_http_info(self, ostree_ostree_remote,  **kwargs):  # noqa: E501
         """Create an ostree remote  # noqa: E501
 
         A ViewSet class for OSTree remote repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_with_http_info(ostree_ostree_remote, async_req=True)
         >>> result = thread.get()
@@ -151,15 +151,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete(self, ostree_ostree_remote_href, **kwargs):  # noqa: E501
+    def delete(self, ostree_ostree_remote_href,  **kwargs):  # noqa: E501
         """Delete an ostree remote  # noqa: E501
 
         Trigger an asynchronous delete task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete(ostree_ostree_remote_href, async_req=True)
         >>> result = thread.get()
@@ -174,17 +174,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_with_http_info(ostree_ostree_remote_href, **kwargs)  # noqa: E501
+        return self.delete_with_http_info(ostree_ostree_remote_href,  **kwargs)  # noqa: E501
 
-    def delete_with_http_info(self, ostree_ostree_remote_href, **kwargs):  # noqa: E501
+    def delete_with_http_info(self, ostree_ostree_remote_href,  **kwargs):  # noqa: E501
         """Delete an ostree remote  # noqa: E501
 
         Trigger an asynchronous delete task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_with_http_info(ostree_ostree_remote_href, async_req=True)
         >>> result = thread.get()
@@ -265,15 +265,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list(self, **kwargs):  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
         """List ostree remotes  # noqa: E501
 
         A ViewSet class for OSTree remote repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
@@ -282,15 +282,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `url` - Url * `-url` - Url (descending) * `ca_cert` - Ca cert * `-ca_cert` - Ca cert (descending) * `client_cert` - Client cert * `-client_cert` - Client cert (descending) * `client_key` - Client key * `-client_key` - Client key (descending) * `tls_validation` - Tls validation * `-tls_validation` - Tls validation (descending) * `username` - Username * `-username` - Username (descending) * `password` - Password * `-password` - Password (descending) * `proxy_url` - Proxy url * `-proxy_url` - Proxy url (descending) * `proxy_username` - Proxy username * `-proxy_username` - Proxy username (descending) * `proxy_password` - Proxy password * `-proxy_password` - Proxy password (descending) * `download_concurrency` - Download concurrency * `-download_concurrency` - Download concurrency (descending) * `max_retries` - Max retries * `-max_retries` - Max retries (descending) * `policy` - Policy * `-policy` - Policy (descending) * `total_timeout` - Total timeout * `-total_timeout` - Total timeout (descending) * `connect_timeout` - Connect timeout * `-connect_timeout` - Connect timeout (descending) * `sock_connect_timeout` - Sock connect timeout * `-sock_connect_timeout` - Sock connect timeout (descending) * `sock_read_timeout` - Sock read timeout * `-sock_read_timeout` - Sock read timeout (descending) * `headers` - Headers * `-headers` - Headers (descending) * `rate_limit` - Rate limit * `-rate_limit` - Rate limit (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param datetime pulp_last_updated: Filter results where pulp_last_updated matches value
         :param datetime pulp_last_updated__gt: Filter results where pulp_last_updated is greater than value
         :param datetime pulp_last_updated__gte: Filter results where pulp_last_updated is greater than or equal to value
         :param datetime pulp_last_updated__lt: Filter results where pulp_last_updated is less than value
         :param datetime pulp_last_updated__lte: Filter results where pulp_last_updated is less than or equal to value
         :param list[datetime] pulp_last_updated__range: Filter results where pulp_last_updated is between two comma separated values
@@ -304,17 +306,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: PaginatedostreeOstreeRemoteResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
         """List ostree remotes  # noqa: E501
 
         A ViewSet class for OSTree remote repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
@@ -323,15 +325,17 @@
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `url` - Url * `-url` - Url (descending) * `ca_cert` - Ca cert * `-ca_cert` - Ca cert (descending) * `client_cert` - Client cert * `-client_cert` - Client cert (descending) * `client_key` - Client key * `-client_key` - Client key (descending) * `tls_validation` - Tls validation * `-tls_validation` - Tls validation (descending) * `username` - Username * `-username` - Username (descending) * `password` - Password * `-password` - Password (descending) * `proxy_url` - Proxy url * `-proxy_url` - Proxy url (descending) * `proxy_username` - Proxy username * `-proxy_username` - Proxy username (descending) * `proxy_password` - Proxy password * `-proxy_password` - Proxy password (descending) * `download_concurrency` - Download concurrency * `-download_concurrency` - Download concurrency (descending) * `max_retries` - Max retries * `-max_retries` - Max retries (descending) * `policy` - Policy * `-policy` - Policy (descending) * `total_timeout` - Total timeout * `-total_timeout` - Total timeout (descending) * `connect_timeout` - Connect timeout * `-connect_timeout` - Connect timeout (descending) * `sock_connect_timeout` - Sock connect timeout * `-sock_connect_timeout` - Sock connect timeout (descending) * `sock_read_timeout` - Sock read timeout * `-sock_read_timeout` - Sock read timeout (descending) * `headers` - Headers * `-headers` - Headers (descending) * `rate_limit` - Rate limit * `-rate_limit` - Rate limit (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param datetime pulp_last_updated: Filter results where pulp_last_updated matches value
         :param datetime pulp_last_updated__gt: Filter results where pulp_last_updated is greater than value
         :param datetime pulp_last_updated__gte: Filter results where pulp_last_updated is greater than or equal to value
         :param datetime pulp_last_updated__lt: Filter results where pulp_last_updated is less than value
         :param datetime pulp_last_updated__lte: Filter results where pulp_last_updated is less than or equal to value
         :param list[datetime] pulp_last_updated__range: Filter results where pulp_last_updated is between two comma separated values
@@ -358,14 +362,16 @@
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'pulp_label_select',
             'pulp_last_updated',
             'pulp_last_updated__gt',
             'pulp_last_updated__gte',
             'pulp_last_updated__lt',
             'pulp_last_updated__lte',
             'pulp_last_updated__range',
@@ -409,14 +415,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
             query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'pulp_last_updated' in local_var_params and local_var_params['pulp_last_updated'] is not None:  # noqa: E501
             query_params.append(('pulp_last_updated', local_var_params['pulp_last_updated']))  # noqa: E501
         if 'pulp_last_updated__gt' in local_var_params and local_var_params['pulp_last_updated__gt'] is not None:  # noqa: E501
             query_params.append(('pulp_last_updated__gt', local_var_params['pulp_last_updated__gt']))  # noqa: E501
         if 'pulp_last_updated__gte' in local_var_params and local_var_params['pulp_last_updated__gte'] is not None:  # noqa: E501
@@ -460,15 +472,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def partial_update(self, ostree_ostree_remote_href, patchedostree_ostree_remote, **kwargs):  # noqa: E501
+    def partial_update(self, ostree_ostree_remote_href, patchedostree_ostree_remote,  **kwargs):  # noqa: E501
         """Update an ostree remote  # noqa: E501
 
         Trigger an asynchronous partial update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.partial_update(ostree_ostree_remote_href, patchedostree_ostree_remote, async_req=True)
         >>> result = thread.get()
@@ -484,17 +496,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.partial_update_with_http_info(ostree_ostree_remote_href, patchedostree_ostree_remote, **kwargs)  # noqa: E501
+        return self.partial_update_with_http_info(ostree_ostree_remote_href, patchedostree_ostree_remote,  **kwargs)  # noqa: E501
 
-    def partial_update_with_http_info(self, ostree_ostree_remote_href, patchedostree_ostree_remote, **kwargs):  # noqa: E501
+    def partial_update_with_http_info(self, ostree_ostree_remote_href, patchedostree_ostree_remote,  **kwargs):  # noqa: E501
         """Update an ostree remote  # noqa: E501
 
         Trigger an asynchronous partial update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.partial_update_with_http_info(ostree_ostree_remote_href, patchedostree_ostree_remote, async_req=True)
         >>> result = thread.get()
@@ -587,15 +599,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_remote_href, **kwargs):  # noqa: E501
+    def read(self, ostree_ostree_remote_href,  **kwargs):  # noqa: E501
         """Inspect an ostree remote  # noqa: E501
 
         A ViewSet class for OSTree remote repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read(ostree_ostree_remote_href, async_req=True)
         >>> result = thread.get()
@@ -612,17 +624,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: OstreeOstreeRemoteResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_remote_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_remote_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_remote_href, **kwargs):  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_remote_href,  **kwargs):  # noqa: E501
         """Inspect an ostree remote  # noqa: E501
 
         A ViewSet class for OSTree remote repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_with_http_info(ostree_ostree_remote_href, async_req=True)
         >>> result = thread.get()
@@ -713,15 +725,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update(self, ostree_ostree_remote_href, ostree_ostree_remote, **kwargs):  # noqa: E501
+    def update(self, ostree_ostree_remote_href, ostree_ostree_remote,  **kwargs):  # noqa: E501
         """Update an ostree remote  # noqa: E501
 
         Trigger an asynchronous update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update(ostree_ostree_remote_href, ostree_ostree_remote, async_req=True)
         >>> result = thread.get()
@@ -737,17 +749,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_with_http_info(ostree_ostree_remote_href, ostree_ostree_remote, **kwargs)  # noqa: E501
+        return self.update_with_http_info(ostree_ostree_remote_href, ostree_ostree_remote,  **kwargs)  # noqa: E501
 
-    def update_with_http_info(self, ostree_ostree_remote_href, ostree_ostree_remote, **kwargs):  # noqa: E501
+    def update_with_http_info(self, ostree_ostree_remote_href, ostree_ostree_remote,  **kwargs):  # noqa: E501
         """Update an ostree remote  # noqa: E501
 
         Trigger an asynchronous update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_with_http_info(ostree_ostree_remote_href, ostree_ostree_remote, async_req=True)
         >>> result = thread.get()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def create(self, ostree_ostree_repository, **kwargs):  # noqa: E501
+    def create(self, ostree_ostree_repository,  **kwargs):  # noqa: E501
         """Create an ostree repository  # noqa: E501
 
         A ViewSet class for OSTree repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create(ostree_ostree_repository, async_req=True)
         >>> result = thread.get()
@@ -56,17 +56,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: OstreeOstreeRepositoryResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_with_http_info(ostree_ostree_repository, **kwargs)  # noqa: E501
+        return self.create_with_http_info(ostree_ostree_repository,  **kwargs)  # noqa: E501
 
-    def create_with_http_info(self, ostree_ostree_repository, **kwargs):  # noqa: E501
+    def create_with_http_info(self, ostree_ostree_repository,  **kwargs):  # noqa: E501
         """Create an ostree repository  # noqa: E501
 
         A ViewSet class for OSTree repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.create_with_http_info(ostree_ostree_repository, async_req=True)
         >>> result = thread.get()
@@ -151,15 +151,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete(self, ostree_ostree_repository_href, **kwargs):  # noqa: E501
+    def delete(self, ostree_ostree_repository_href,  **kwargs):  # noqa: E501
         """Delete an ostree repository  # noqa: E501
 
         Trigger an asynchronous delete task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete(ostree_ostree_repository_href, async_req=True)
         >>> result = thread.get()
@@ -174,17 +174,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_with_http_info(ostree_ostree_repository_href, **kwargs)  # noqa: E501
+        return self.delete_with_http_info(ostree_ostree_repository_href,  **kwargs)  # noqa: E501
 
-    def delete_with_http_info(self, ostree_ostree_repository_href, **kwargs):  # noqa: E501
+    def delete_with_http_info(self, ostree_ostree_repository_href,  **kwargs):  # noqa: E501
         """Delete an ostree repository  # noqa: E501
 
         Trigger an asynchronous delete task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_with_http_info(ostree_ostree_repository_href, async_req=True)
         >>> result = thread.get()
@@ -265,15 +265,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def import_all(self, ostree_ostree_repository_href, ostree_import_all, **kwargs):  # noqa: E501
+    def import_all(self, ostree_ostree_repository_href, ostree_import_all,  **kwargs):  # noqa: E501
         """Import refs and commits to a repository  # noqa: E501
 
         Trigger an asynchronous task to import all refs and commits to a repository.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.import_all(ostree_ostree_repository_href, ostree_import_all, async_req=True)
         >>> result = thread.get()
@@ -289,17 +289,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.import_all_with_http_info(ostree_ostree_repository_href, ostree_import_all, **kwargs)  # noqa: E501
+        return self.import_all_with_http_info(ostree_ostree_repository_href, ostree_import_all,  **kwargs)  # noqa: E501
 
-    def import_all_with_http_info(self, ostree_ostree_repository_href, ostree_import_all, **kwargs):  # noqa: E501
+    def import_all_with_http_info(self, ostree_ostree_repository_href, ostree_import_all,  **kwargs):  # noqa: E501
         """Import refs and commits to a repository  # noqa: E501
 
         Trigger an asynchronous task to import all refs and commits to a repository.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.import_all_with_http_info(ostree_ostree_repository_href, ostree_import_all, async_req=True)
         >>> result = thread.get()
@@ -392,15 +392,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def import_commits(self, ostree_ostree_repository_href, ostree_import_commits_to_ref, **kwargs):  # noqa: E501
+    def import_commits(self, ostree_ostree_repository_href, ostree_import_commits_to_ref,  **kwargs):  # noqa: E501
         """Append child commits to a repository  # noqa: E501
 
         Trigger an asynchronous task to append child commits to a repository.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.import_commits(ostree_ostree_repository_href, ostree_import_commits_to_ref, async_req=True)
         >>> result = thread.get()
@@ -416,17 +416,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.import_commits_with_http_info(ostree_ostree_repository_href, ostree_import_commits_to_ref, **kwargs)  # noqa: E501
+        return self.import_commits_with_http_info(ostree_ostree_repository_href, ostree_import_commits_to_ref,  **kwargs)  # noqa: E501
 
-    def import_commits_with_http_info(self, ostree_ostree_repository_href, ostree_import_commits_to_ref, **kwargs):  # noqa: E501
+    def import_commits_with_http_info(self, ostree_ostree_repository_href, ostree_import_commits_to_ref,  **kwargs):  # noqa: E501
         """Append child commits to a repository  # noqa: E501
 
         Trigger an asynchronous task to append child commits to a repository.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.import_commits_with_http_info(ostree_ostree_repository_href, ostree_import_commits_to_ref, async_req=True)
         >>> result = thread.get()
@@ -519,86 +519,94 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list(self, **kwargs):  # noqa: E501
+    def list(self,  **kwargs):  # noqa: E501
         """List ostree repositorys  # noqa: E501
 
         A ViewSet class for OSTree repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str latest_with_content: Content Unit referenced by HREF
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `description` - Description * `-description` - Description (descending) * `next_version` - Next version * `-next_version` - Next version (descending) * `retain_repo_versions` - Retain repo versions * `-retain_repo_versions` - Retain repo versions (descending) * `user_hidden` - User hidden * `-user_hidden` - User hidden (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str remote: Foreign Key referenced by HREF
         :param int retain_repo_versions: Filter results where retain_repo_versions matches value
         :param int retain_repo_versions__gt: Filter results where retain_repo_versions is greater than value
         :param int retain_repo_versions__gte: Filter results where retain_repo_versions is greater than or equal to value
         :param bool retain_repo_versions__isnull: Filter results where retain_repo_versions has a null value
         :param int retain_repo_versions__lt: Filter results where retain_repo_versions is less than value
         :param int retain_repo_versions__lte: Filter results where retain_repo_versions is less than or equal to value
         :param int retain_repo_versions__ne: Filter results where retain_repo_versions not equal to value
         :param list[int] retain_repo_versions__range: Filter results where retain_repo_versions is between two comma separated values
+        :param str with_content: Content Unit referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: PaginatedostreeOstreeRepositoryResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(**kwargs)  # noqa: E501
+        return self.list_with_http_info( **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, **kwargs):  # noqa: E501
+    def list_with_http_info(self,  **kwargs):  # noqa: E501
         """List ostree repositorys  # noqa: E501
 
         A ViewSet class for OSTree repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param str latest_with_content: Content Unit referenced by HREF
         :param int limit: Number of results to return per page.
         :param str name: Filter results where name matches value
         :param str name__contains: Filter results where name contains value
         :param str name__icontains: Filter results where name contains value
         :param list[str] name__in: Filter results where name is in a comma-separated list of values
         :param str name__startswith: Filter results where name starts with value
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `pulp_type` - Pulp type * `-pulp_type` - Pulp type (descending) * `name` - Name * `-name` - Name (descending) * `pulp_labels` - Pulp labels * `-pulp_labels` - Pulp labels (descending) * `description` - Description * `-description` - Description (descending) * `next_version` - Next version * `-next_version` - Next version (descending) * `retain_repo_versions` - Retain repo versions * `-retain_repo_versions` - Retain repo versions (descending) * `user_hidden` - User hidden * `-user_hidden` - User hidden (descending) * `pk` - Pk * `-pk` - Pk (descending)
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
+        :param list[str] pulp_id__in: Multiple values may be separated by commas.
         :param str pulp_label_select: Filter labels by search string
         :param str remote: Foreign Key referenced by HREF
         :param int retain_repo_versions: Filter results where retain_repo_versions matches value
         :param int retain_repo_versions__gt: Filter results where retain_repo_versions is greater than value
         :param int retain_repo_versions__gte: Filter results where retain_repo_versions is greater than or equal to value
         :param bool retain_repo_versions__isnull: Filter results where retain_repo_versions has a null value
         :param int retain_repo_versions__lt: Filter results where retain_repo_versions is less than value
         :param int retain_repo_versions__lte: Filter results where retain_repo_versions is less than or equal to value
         :param int retain_repo_versions__ne: Filter results where retain_repo_versions not equal to value
         :param list[int] retain_repo_versions__range: Filter results where retain_repo_versions is between two comma separated values
+        :param str with_content: Content Unit referenced by HREF
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -610,32 +618,36 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'latest_with_content',
             'limit',
             'name',
             'name__contains',
             'name__icontains',
             'name__in',
             'name__startswith',
             'offset',
             'ordering',
+            'pulp_href__in',
+            'pulp_id__in',
             'pulp_label_select',
             'remote',
             'retain_repo_versions',
             'retain_repo_versions__gt',
             'retain_repo_versions__gte',
             'retain_repo_versions__isnull',
             'retain_repo_versions__lt',
             'retain_repo_versions__lte',
             'retain_repo_versions__ne',
             'retain_repo_versions__range',
+            'with_content',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -654,14 +666,16 @@
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'latest_with_content' in local_var_params and local_var_params['latest_with_content'] is not None:  # noqa: E501
+            query_params.append(('latest_with_content', local_var_params['latest_with_content']))  # noqa: E501
         if 'limit' in local_var_params and local_var_params['limit'] is not None:  # noqa: E501
             query_params.append(('limit', local_var_params['limit']))  # noqa: E501
         if 'name' in local_var_params and local_var_params['name'] is not None:  # noqa: E501
             query_params.append(('name', local_var_params['name']))  # noqa: E501
         if 'name__contains' in local_var_params and local_var_params['name__contains'] is not None:  # noqa: E501
             query_params.append(('name__contains', local_var_params['name__contains']))  # noqa: E501
         if 'name__icontains' in local_var_params and local_var_params['name__icontains'] is not None:  # noqa: E501
@@ -672,14 +686,20 @@
         if 'name__startswith' in local_var_params and local_var_params['name__startswith'] is not None:  # noqa: E501
             query_params.append(('name__startswith', local_var_params['name__startswith']))  # noqa: E501
         if 'offset' in local_var_params and local_var_params['offset'] is not None:  # noqa: E501
             query_params.append(('offset', local_var_params['offset']))  # noqa: E501
         if 'ordering' in local_var_params and local_var_params['ordering'] is not None:  # noqa: E501
             query_params.append(('ordering', local_var_params['ordering']))  # noqa: E501
             collection_formats['ordering'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
+        if 'pulp_id__in' in local_var_params and local_var_params['pulp_id__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_id__in', local_var_params['pulp_id__in']))  # noqa: E501
+            collection_formats['pulp_id__in'] = 'csv'  # noqa: E501
         if 'pulp_label_select' in local_var_params and local_var_params['pulp_label_select'] is not None:  # noqa: E501
             query_params.append(('pulp_label_select', local_var_params['pulp_label_select']))  # noqa: E501
         if 'remote' in local_var_params and local_var_params['remote'] is not None:  # noqa: E501
             query_params.append(('remote', local_var_params['remote']))  # noqa: E501
         if 'retain_repo_versions' in local_var_params and local_var_params['retain_repo_versions'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions', local_var_params['retain_repo_versions']))  # noqa: E501
         if 'retain_repo_versions__gt' in local_var_params and local_var_params['retain_repo_versions__gt'] is not None:  # noqa: E501
@@ -693,14 +713,16 @@
         if 'retain_repo_versions__lte' in local_var_params and local_var_params['retain_repo_versions__lte'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions__lte', local_var_params['retain_repo_versions__lte']))  # noqa: E501
         if 'retain_repo_versions__ne' in local_var_params and local_var_params['retain_repo_versions__ne'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions__ne', local_var_params['retain_repo_versions__ne']))  # noqa: E501
         if 'retain_repo_versions__range' in local_var_params and local_var_params['retain_repo_versions__range'] is not None:  # noqa: E501
             query_params.append(('retain_repo_versions__range', local_var_params['retain_repo_versions__range']))  # noqa: E501
             collection_formats['retain_repo_versions__range'] = 'csv'  # noqa: E501
+        if 'with_content' in local_var_params and local_var_params['with_content'] is not None:  # noqa: E501
+            query_params.append(('with_content', local_var_params['with_content']))  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
             collection_formats['exclude_fields'] = 'multi'  # noqa: E501
 
@@ -729,52 +751,52 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def modify(self, ostree_ostree_repository_href, ostree_repository_add_remove_content, **kwargs):  # noqa: E501
+    def modify(self, ostree_ostree_repository_href, repository_add_remove_content,  **kwargs):  # noqa: E501
         """Modify repository  # noqa: E501
 
         Trigger an asynchronous task to modify content.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.modify(ostree_ostree_repository_href, ostree_repository_add_remove_content, async_req=True)
+        >>> thread = api.modify(ostree_ostree_repository_href, repository_add_remove_content, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str ostree_ostree_repository_href: (required)
-        :param OstreeRepositoryAddRemoveContent ostree_repository_add_remove_content: (required)
+        :param RepositoryAddRemoveContent repository_add_remove_content: (required)
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.modify_with_http_info(ostree_ostree_repository_href, ostree_repository_add_remove_content, **kwargs)  # noqa: E501
+        return self.modify_with_http_info(ostree_ostree_repository_href, repository_add_remove_content,  **kwargs)  # noqa: E501
 
-    def modify_with_http_info(self, ostree_ostree_repository_href, ostree_repository_add_remove_content, **kwargs):  # noqa: E501
+    def modify_with_http_info(self, ostree_ostree_repository_href, repository_add_remove_content,  **kwargs):  # noqa: E501
         """Modify repository  # noqa: E501
 
         Trigger an asynchronous task to modify content.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.modify_with_http_info(ostree_ostree_repository_href, ostree_repository_add_remove_content, async_req=True)
+        >>> thread = api.modify_with_http_info(ostree_ostree_repository_href, repository_add_remove_content, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
         :param str ostree_ostree_repository_href: (required)
-        :param OstreeRepositoryAddRemoveContent ostree_repository_add_remove_content: (required)
+        :param RepositoryAddRemoveContent repository_add_remove_content: (required)
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -785,15 +807,15 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'ostree_ostree_repository_href',
-            'ostree_repository_add_remove_content'
+            'repository_add_remove_content'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -808,18 +830,18 @@
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'ostree_ostree_repository_href' is set
         if self.api_client.client_side_validation and ('ostree_ostree_repository_href' not in local_var_params or  # noqa: E501
                                                         local_var_params['ostree_ostree_repository_href'] is None):  # noqa: E501
             raise ApiValueError("Missing the required parameter `ostree_ostree_repository_href` when calling `modify`")  # noqa: E501
-        # verify the required parameter 'ostree_repository_add_remove_content' is set
-        if self.api_client.client_side_validation and ('ostree_repository_add_remove_content' not in local_var_params or  # noqa: E501
-                                                        local_var_params['ostree_repository_add_remove_content'] is None):  # noqa: E501
-            raise ApiValueError("Missing the required parameter `ostree_repository_add_remove_content` when calling `modify`")  # noqa: E501
+        # verify the required parameter 'repository_add_remove_content' is set
+        if self.api_client.client_side_validation and ('repository_add_remove_content' not in local_var_params or  # noqa: E501
+                                                        local_var_params['repository_add_remove_content'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `repository_add_remove_content` when calling `modify`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'ostree_ostree_repository_href' in local_var_params:
             path_params['ostree_ostree_repository_href'] = local_var_params['ostree_ostree_repository_href']  # noqa: E501
 
@@ -827,16 +849,16 @@
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
-        if 'ostree_repository_add_remove_content' in local_var_params:
-            body_params = local_var_params['ostree_repository_add_remove_content']
+        if 'repository_add_remove_content' in local_var_params:
+            body_params = local_var_params['repository_add_remove_content']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json', 'application/x-www-form-urlencoded', 'multipart/form-data'])  # noqa: E501
@@ -856,15 +878,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def partial_update(self, ostree_ostree_repository_href, patchedostree_ostree_repository, **kwargs):  # noqa: E501
+    def partial_update(self, ostree_ostree_repository_href, patchedostree_ostree_repository,  **kwargs):  # noqa: E501
         """Update an ostree repository  # noqa: E501
 
         Trigger an asynchronous partial update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.partial_update(ostree_ostree_repository_href, patchedostree_ostree_repository, async_req=True)
         >>> result = thread.get()
@@ -880,17 +902,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.partial_update_with_http_info(ostree_ostree_repository_href, patchedostree_ostree_repository, **kwargs)  # noqa: E501
+        return self.partial_update_with_http_info(ostree_ostree_repository_href, patchedostree_ostree_repository,  **kwargs)  # noqa: E501
 
-    def partial_update_with_http_info(self, ostree_ostree_repository_href, patchedostree_ostree_repository, **kwargs):  # noqa: E501
+    def partial_update_with_http_info(self, ostree_ostree_repository_href, patchedostree_ostree_repository,  **kwargs):  # noqa: E501
         """Update an ostree repository  # noqa: E501
 
         Trigger an asynchronous partial update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.partial_update_with_http_info(ostree_ostree_repository_href, patchedostree_ostree_repository, async_req=True)
         >>> result = thread.get()
@@ -983,15 +1005,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_repository_href, **kwargs):  # noqa: E501
+    def read(self, ostree_ostree_repository_href,  **kwargs):  # noqa: E501
         """Inspect an ostree repository  # noqa: E501
 
         A ViewSet class for OSTree repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read(ostree_ostree_repository_href, async_req=True)
         >>> result = thread.get()
@@ -1008,17 +1030,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: OstreeOstreeRepositoryResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_repository_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_repository_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_repository_href, **kwargs):  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_repository_href,  **kwargs):  # noqa: E501
         """Inspect an ostree repository  # noqa: E501
 
         A ViewSet class for OSTree repositories.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_with_http_info(ostree_ostree_repository_href, async_req=True)
         >>> result = thread.get()
@@ -1109,15 +1131,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def sync(self, ostree_ostree_repository_href, repository_sync_url, **kwargs):  # noqa: E501
+    def sync(self, ostree_ostree_repository_href, repository_sync_url,  **kwargs):  # noqa: E501
         """Sync from remote  # noqa: E501
 
         Trigger an asynchronous task to sync content.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.sync(ostree_ostree_repository_href, repository_sync_url, async_req=True)
         >>> result = thread.get()
@@ -1133,17 +1155,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.sync_with_http_info(ostree_ostree_repository_href, repository_sync_url, **kwargs)  # noqa: E501
+        return self.sync_with_http_info(ostree_ostree_repository_href, repository_sync_url,  **kwargs)  # noqa: E501
 
-    def sync_with_http_info(self, ostree_ostree_repository_href, repository_sync_url, **kwargs):  # noqa: E501
+    def sync_with_http_info(self, ostree_ostree_repository_href, repository_sync_url,  **kwargs):  # noqa: E501
         """Sync from remote  # noqa: E501
 
         Trigger an asynchronous task to sync content.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.sync_with_http_info(ostree_ostree_repository_href, repository_sync_url, async_req=True)
         >>> result = thread.get()
@@ -1236,15 +1258,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def update(self, ostree_ostree_repository_href, ostree_ostree_repository, **kwargs):  # noqa: E501
+    def update(self, ostree_ostree_repository_href, ostree_ostree_repository,  **kwargs):  # noqa: E501
         """Update an ostree repository  # noqa: E501
 
         Trigger an asynchronous update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update(ostree_ostree_repository_href, ostree_ostree_repository, async_req=True)
         >>> result = thread.get()
@@ -1260,17 +1282,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_with_http_info(ostree_ostree_repository_href, ostree_ostree_repository, **kwargs)  # noqa: E501
+        return self.update_with_http_info(ostree_ostree_repository_href, ostree_ostree_repository,  **kwargs)  # noqa: E501
 
-    def update_with_http_info(self, ostree_ostree_repository_href, ostree_ostree_repository, **kwargs):  # noqa: E501
+    def update_with_http_info(self, ostree_ostree_repository_href, ostree_ostree_repository,  **kwargs):  # noqa: E501
         """Update an ostree repository  # noqa: E501
 
         Trigger an asynchronous update task  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.update_with_http_info(ostree_ostree_repository_href, ostree_ostree_repository, async_req=True)
         >>> result = thread.get()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api/repositories_ostree_versions_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def delete(self, ostree_ostree_repository_version_href, **kwargs):  # noqa: E501
+    def delete(self, ostree_ostree_repository_version_href,  **kwargs):  # noqa: E501
         """Delete a repository version  # noqa: E501
 
         Trigger an asynchronous task to delete a repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete(ostree_ostree_repository_version_href, async_req=True)
         >>> result = thread.get()
@@ -56,17 +56,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_with_http_info(ostree_ostree_repository_version_href, **kwargs)  # noqa: E501
+        return self.delete_with_http_info(ostree_ostree_repository_version_href,  **kwargs)  # noqa: E501
 
-    def delete_with_http_info(self, ostree_ostree_repository_version_href, **kwargs):  # noqa: E501
+    def delete_with_http_info(self, ostree_ostree_repository_version_href,  **kwargs):  # noqa: E501
         """Delete a repository version  # noqa: E501
 
         Trigger an asynchronous task to delete a repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.delete_with_http_info(ostree_ostree_repository_version_href, async_req=True)
         >>> result = thread.get()
@@ -147,15 +147,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list(self, ostree_ostree_repository_href, **kwargs):  # noqa: E501
+    def list(self, ostree_ostree_repository_href,  **kwargs):  # noqa: E501
         """List repository versions  # noqa: E501
 
         A ViewSet class that represents a single OSTree repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list(ostree_ostree_repository_href, async_req=True)
         >>> result = thread.get()
@@ -168,38 +168,39 @@
         :param int number: Filter results where number matches value
         :param int number__gt: Filter results where number is greater than value
         :param int number__gte: Filter results where number is greater than or equal to value
         :param int number__lt: Filter results where number is less than value
         :param int number__lte: Filter results where number is less than or equal to value
         :param list[int] number__range: Filter results where number is between two comma separated values
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `number` - Number * `-number` - Number (descending) * `complete` - Complete * `-complete` - Complete (descending) * `info` - Info * `-info` - Info (descending) * `pk` - Pk * `-pk` - Pk (descending)
         :param datetime pulp_created: Filter results where pulp_created matches value
         :param datetime pulp_created__gt: Filter results where pulp_created is greater than value
         :param datetime pulp_created__gte: Filter results where pulp_created is greater than or equal to value
         :param datetime pulp_created__lt: Filter results where pulp_created is less than value
         :param datetime pulp_created__lte: Filter results where pulp_created is less than or equal to value
         :param list[datetime] pulp_created__range: Filter results where pulp_created is between two comma separated values
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: PaginatedRepositoryVersionResponseList
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_with_http_info(ostree_ostree_repository_href, **kwargs)  # noqa: E501
+        return self.list_with_http_info(ostree_ostree_repository_href,  **kwargs)  # noqa: E501
 
-    def list_with_http_info(self, ostree_ostree_repository_href, **kwargs):  # noqa: E501
+    def list_with_http_info(self, ostree_ostree_repository_href,  **kwargs):  # noqa: E501
         """List repository versions  # noqa: E501
 
         A ViewSet class that represents a single OSTree repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.list_with_http_info(ostree_ostree_repository_href, async_req=True)
         >>> result = thread.get()
@@ -212,21 +213,22 @@
         :param int number: Filter results where number matches value
         :param int number__gt: Filter results where number is greater than value
         :param int number__gte: Filter results where number is greater than or equal to value
         :param int number__lt: Filter results where number is less than value
         :param int number__lte: Filter results where number is less than or equal to value
         :param list[int] number__range: Filter results where number is between two comma separated values
         :param int offset: The initial index from which to return the results.
-        :param list[str] ordering: Ordering
+        :param list[str] ordering: Ordering  * `pulp_id` - Pulp id * `-pulp_id` - Pulp id (descending) * `pulp_created` - Pulp created * `-pulp_created` - Pulp created (descending) * `pulp_last_updated` - Pulp last updated * `-pulp_last_updated` - Pulp last updated (descending) * `number` - Number * `-number` - Number (descending) * `complete` - Complete * `-complete` - Complete (descending) * `info` - Info * `-info` - Info (descending) * `pk` - Pk * `-pk` - Pk (descending)
         :param datetime pulp_created: Filter results where pulp_created matches value
         :param datetime pulp_created__gt: Filter results where pulp_created is greater than value
         :param datetime pulp_created__gte: Filter results where pulp_created is greater than or equal to value
         :param datetime pulp_created__lt: Filter results where pulp_created is less than value
         :param datetime pulp_created__lte: Filter results where pulp_created is less than or equal to value
         :param list[datetime] pulp_created__range: Filter results where pulp_created is between two comma separated values
+        :param list[str] pulp_href__in: Multiple values may be separated by commas.
         :param list[str] fields: A list of fields to include in the response.
         :param list[str] exclude_fields: A list of fields to exclude from the response.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -256,14 +258,15 @@
             'ordering',
             'pulp_created',
             'pulp_created__gt',
             'pulp_created__gte',
             'pulp_created__lt',
             'pulp_created__lte',
             'pulp_created__range',
+            'pulp_href__in',
             'fields',
             'exclude_fields'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -325,14 +328,17 @@
         if 'pulp_created__lt' in local_var_params and local_var_params['pulp_created__lt'] is not None:  # noqa: E501
             query_params.append(('pulp_created__lt', local_var_params['pulp_created__lt']))  # noqa: E501
         if 'pulp_created__lte' in local_var_params and local_var_params['pulp_created__lte'] is not None:  # noqa: E501
             query_params.append(('pulp_created__lte', local_var_params['pulp_created__lte']))  # noqa: E501
         if 'pulp_created__range' in local_var_params and local_var_params['pulp_created__range'] is not None:  # noqa: E501
             query_params.append(('pulp_created__range', local_var_params['pulp_created__range']))  # noqa: E501
             collection_formats['pulp_created__range'] = 'csv'  # noqa: E501
+        if 'pulp_href__in' in local_var_params and local_var_params['pulp_href__in'] is not None:  # noqa: E501
+            query_params.append(('pulp_href__in', local_var_params['pulp_href__in']))  # noqa: E501
+            collection_formats['pulp_href__in'] = 'csv'  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'exclude_fields' in local_var_params and local_var_params['exclude_fields'] is not None:  # noqa: E501
             query_params.append(('exclude_fields', local_var_params['exclude_fields']))  # noqa: E501
             collection_formats['exclude_fields'] = 'multi'  # noqa: E501
 
@@ -361,15 +367,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def read(self, ostree_ostree_repository_version_href, **kwargs):  # noqa: E501
+    def read(self, ostree_ostree_repository_version_href,  **kwargs):  # noqa: E501
         """Inspect a repository version  # noqa: E501
 
         A ViewSet class that represents a single OSTree repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read(ostree_ostree_repository_version_href, async_req=True)
         >>> result = thread.get()
@@ -386,17 +392,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: RepositoryVersionResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_with_http_info(ostree_ostree_repository_version_href, **kwargs)  # noqa: E501
+        return self.read_with_http_info(ostree_ostree_repository_version_href,  **kwargs)  # noqa: E501
 
-    def read_with_http_info(self, ostree_ostree_repository_version_href, **kwargs):  # noqa: E501
+    def read_with_http_info(self, ostree_ostree_repository_version_href,  **kwargs):  # noqa: E501
         """Inspect a repository version  # noqa: E501
 
         A ViewSet class that represents a single OSTree repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.read_with_http_info(ostree_ostree_repository_version_href, async_req=True)
         >>> result = thread.get()
@@ -487,15 +493,15 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def repair(self, ostree_ostree_repository_version_href, repair, **kwargs):  # noqa: E501
+    def repair(self, ostree_ostree_repository_version_href, repair,  **kwargs):  # noqa: E501
         """repair  # noqa: E501
 
         Trigger an asynchronous task to repair a repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repair(ostree_ostree_repository_version_href, repair, async_req=True)
         >>> result = thread.get()
@@ -511,17 +517,17 @@
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: AsyncOperationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.repair_with_http_info(ostree_ostree_repository_version_href, repair, **kwargs)  # noqa: E501
+        return self.repair_with_http_info(ostree_ostree_repository_version_href, repair,  **kwargs)  # noqa: E501
 
-    def repair_with_http_info(self, ostree_ostree_repository_version_href, repair, **kwargs):  # noqa: E501
+    def repair_with_http_info(self, ostree_ostree_repository_version_href, repair,  **kwargs):  # noqa: E501
         """repair  # noqa: E501
 
         Trigger an asynchronous task to repair a repository version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.repair_with_http_info(ostree_ostree_repository_version_href, repair, async_req=True)
         >>> result = thread.get()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/api_client.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.0a7.dev1676776305/python'
+        self.user_agent = 'OpenAPI-Generator/2.1.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/configuration.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 2.0.0a7.dev1676776305".\
+               "SDK Package Version: 2.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/exceptions.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/__init__.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,36 @@
 # import models into model package
 from pulpcore.client.pulp_ostree.models.async_operation_response import AsyncOperationResponse
 from pulpcore.client.pulp_ostree.models.content_summary_response import ContentSummaryResponse
 from pulpcore.client.pulp_ostree.models.ostree_import_all import OstreeImportAll
 from pulpcore.client.pulp_ostree.models.ostree_import_commits_to_ref import OstreeImportCommitsToRef
 from pulpcore.client.pulp_ostree.models.ostree_ostree_commit_response import OstreeOstreeCommitResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_config_response import OstreeOstreeConfigResponse
+from pulpcore.client.pulp_ostree.models.ostree_ostree_content_response import OstreeOstreeContentResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_distribution import OstreeOstreeDistribution
 from pulpcore.client.pulp_ostree.models.ostree_ostree_distribution_response import OstreeOstreeDistributionResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_object_response import OstreeOstreeObjectResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_ref_response import OstreeOstreeRefResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_remote import OstreeOstreeRemote
 from pulpcore.client.pulp_ostree.models.ostree_ostree_remote_response import OstreeOstreeRemoteResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_remote_response_hidden_fields import OstreeOstreeRemoteResponseHiddenFields
 from pulpcore.client.pulp_ostree.models.ostree_ostree_repository import OstreeOstreeRepository
 from pulpcore.client.pulp_ostree.models.ostree_ostree_repository_response import OstreeOstreeRepositoryResponse
 from pulpcore.client.pulp_ostree.models.ostree_ostree_summary_response import OstreeOstreeSummaryResponse
-from pulpcore.client.pulp_ostree.models.ostree_repository_add_remove_content import OstreeRepositoryAddRemoveContent
 from pulpcore.client.pulp_ostree.models.paginated_repository_version_response_list import PaginatedRepositoryVersionResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_commit_response_list import PaginatedostreeOstreeCommitResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_config_response_list import PaginatedostreeOstreeConfigResponseList
+from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_content_response_list import PaginatedostreeOstreeContentResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_distribution_response_list import PaginatedostreeOstreeDistributionResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_object_response_list import PaginatedostreeOstreeObjectResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_ref_response_list import PaginatedostreeOstreeRefResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_remote_response_list import PaginatedostreeOstreeRemoteResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_repository_response_list import PaginatedostreeOstreeRepositoryResponseList
 from pulpcore.client.pulp_ostree.models.paginatedostree_ostree_summary_response_list import PaginatedostreeOstreeSummaryResponseList
 from pulpcore.client.pulp_ostree.models.patchedostree_ostree_distribution import PatchedostreeOstreeDistribution
 from pulpcore.client.pulp_ostree.models.patchedostree_ostree_remote import PatchedostreeOstreeRemote
 from pulpcore.client.pulp_ostree.models.patchedostree_ostree_repository import PatchedostreeOstreeRepository
 from pulpcore.client.pulp_ostree.models.policy_enum import PolicyEnum
 from pulpcore.client.pulp_ostree.models.repair import Repair
+from pulpcore.client.pulp_ostree.models.repository_add_remove_content import RepositoryAddRemoveContent
 from pulpcore.client.pulp_ostree.models.repository_sync_url import RepositorySyncURL
 from pulpcore.client.pulp_ostree.models.repository_version_response import RepositoryVersionResponse
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/async_operation_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/content_summary_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_import_all.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_all.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_import_commits_to_ref.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_commit_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_config_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_object_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,26 +506,26 @@
 
         self._max_retries = max_retries
 
     @property
     def policy(self):
         """Gets the policy of this OstreeOstreeRemote.  # noqa: E501
 
-                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           # noqa: E501
+                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           * `immediate` - immediate * `on_demand` - on_demand  # noqa: E501
 
         :return: The policy of this OstreeOstreeRemote.  # noqa: E501
         :rtype: PolicyEnum
         """
         return self._policy
 
     @policy.setter
     def policy(self, policy):
         """Sets the policy of this OstreeOstreeRemote.
 
-                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           # noqa: E501
+                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           * `immediate` - immediate * `on_demand` - on_demand  # noqa: E501
 
         :param policy: The policy of this OstreeOstreeRemote.  # noqa: E501
         :type: PolicyEnum
         """
 
         self._policy = policy
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,26 +428,26 @@
 
         self._max_retries = max_retries
 
     @property
     def policy(self):
         """Gets the policy of this OstreeOstreeRemoteResponse.  # noqa: E501
 
-                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           # noqa: E501
+                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           * `immediate` - immediate * `on_demand` - on_demand  # noqa: E501
 
         :return: The policy of this OstreeOstreeRemoteResponse.  # noqa: E501
         :rtype: PolicyEnum
         """
         return self._policy
 
     @policy.setter
     def policy(self, policy):
         """Sets the policy of this OstreeOstreeRemoteResponse.
 
-                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           # noqa: E501
+                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           * `immediate` - immediate * `on_demand` - on_demand  # noqa: E501
 
         :param policy: The policy of this OstreeOstreeRemoteResponse.  # noqa: E501
         :type: PolicyEnum
         """
 
         self._policy = policy
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,44 +34,49 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'pulp_labels': 'dict(str, str)',
         'name': 'str',
         'description': 'str',
         'retain_repo_versions': 'int',
-        'remote': 'str'
+        'remote': 'str',
+        'compute_delta': 'bool'
     }
 
     attribute_map = {
         'pulp_labels': 'pulp_labels',
         'name': 'name',
         'description': 'description',
         'retain_repo_versions': 'retain_repo_versions',
-        'remote': 'remote'
+        'remote': 'remote',
+        'compute_delta': 'compute_delta'
     }
 
-    def __init__(self, pulp_labels=None, name=None, description=None, retain_repo_versions=None, remote=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_labels=None, name=None, description=None, retain_repo_versions=None, remote=None, compute_delta=True, local_vars_configuration=None):  # noqa: E501
         """OstreeOstreeRepository - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_labels = None
         self._name = None
         self._description = None
         self._retain_repo_versions = None
         self._remote = None
+        self._compute_delta = None
         self.discriminator = None
 
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
         self.name = name
         self.description = description
         self.retain_repo_versions = retain_repo_versions
         self.remote = remote
+        if compute_delta is not None:
+            self.compute_delta = compute_delta
 
     @property
     def pulp_labels(self):
         """Gets the pulp_labels of this OstreeOstreeRepository.  # noqa: E501
 
 
         :return: The pulp_labels of this OstreeOstreeRepository.  # noqa: E501
@@ -144,26 +149,26 @@
 
         self._description = description
 
     @property
     def retain_repo_versions(self):
         """Gets the retain_repo_versions of this OstreeOstreeRepository.  # noqa: E501
 
-        Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
+        Retain X versions of the repository. Default is null which retains all versions.  # noqa: E501
 
         :return: The retain_repo_versions of this OstreeOstreeRepository.  # noqa: E501
         :rtype: int
         """
         return self._retain_repo_versions
 
     @retain_repo_versions.setter
     def retain_repo_versions(self, retain_repo_versions):
         """Sets the retain_repo_versions of this OstreeOstreeRepository.
 
-        Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
+        Retain X versions of the repository. Default is null which retains all versions.  # noqa: E501
 
         :param retain_repo_versions: The retain_repo_versions of this OstreeOstreeRepository.  # noqa: E501
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 retain_repo_versions is not None and retain_repo_versions < 1):  # noqa: E501
             raise ValueError("Invalid value for `retain_repo_versions`, must be a value greater than or equal to `1`")  # noqa: E501
@@ -189,14 +194,35 @@
 
         :param remote: The remote of this OstreeOstreeRepository.  # noqa: E501
         :type: str
         """
 
         self._remote = remote
 
+    @property
+    def compute_delta(self):
+        """Gets the compute_delta of this OstreeOstreeRepository.  # noqa: E501
+
+
+        :return: The compute_delta of this OstreeOstreeRepository.  # noqa: E501
+        :rtype: bool
+        """
+        return self._compute_delta
+
+    @compute_delta.setter
+    def compute_delta(self, compute_delta):
+        """Sets the compute_delta of this OstreeOstreeRepository.
+
+
+        :param compute_delta: The compute_delta of this OstreeOstreeRepository.  # noqa: E501
+        :type: bool
+        """
+
+        self._compute_delta = compute_delta
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_repository_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,44 +38,47 @@
         'pulp_created': 'datetime',
         'versions_href': 'str',
         'pulp_labels': 'dict(str, str)',
         'latest_version_href': 'str',
         'name': 'str',
         'description': 'str',
         'retain_repo_versions': 'int',
-        'remote': 'str'
+        'remote': 'str',
+        'compute_delta': 'bool'
     }
 
     attribute_map = {
         'pulp_href': 'pulp_href',
         'pulp_created': 'pulp_created',
         'versions_href': 'versions_href',
         'pulp_labels': 'pulp_labels',
         'latest_version_href': 'latest_version_href',
         'name': 'name',
         'description': 'description',
         'retain_repo_versions': 'retain_repo_versions',
-        'remote': 'remote'
+        'remote': 'remote',
+        'compute_delta': 'compute_delta'
     }
 
-    def __init__(self, pulp_href=None, pulp_created=None, versions_href=None, pulp_labels=None, latest_version_href=None, name=None, description=None, retain_repo_versions=None, remote=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_href=None, pulp_created=None, versions_href=None, pulp_labels=None, latest_version_href=None, name=None, description=None, retain_repo_versions=None, remote=None, compute_delta=True, local_vars_configuration=None):  # noqa: E501
         """OstreeOstreeRepositoryResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_href = None
         self._pulp_created = None
         self._versions_href = None
         self._pulp_labels = None
         self._latest_version_href = None
         self._name = None
         self._description = None
         self._retain_repo_versions = None
         self._remote = None
+        self._compute_delta = None
         self.discriminator = None
 
         if pulp_href is not None:
             self.pulp_href = pulp_href
         if pulp_created is not None:
             self.pulp_created = pulp_created
         if versions_href is not None:
@@ -84,14 +87,16 @@
             self.pulp_labels = pulp_labels
         if latest_version_href is not None:
             self.latest_version_href = latest_version_href
         self.name = name
         self.description = description
         self.retain_repo_versions = retain_repo_versions
         self.remote = remote
+        if compute_delta is not None:
+            self.compute_delta = compute_delta
 
     @property
     def pulp_href(self):
         """Gets the pulp_href of this OstreeOstreeRepositoryResponse.  # noqa: E501
 
 
         :return: The pulp_href of this OstreeOstreeRepositoryResponse.  # noqa: E501
@@ -244,26 +249,26 @@
 
         self._description = description
 
     @property
     def retain_repo_versions(self):
         """Gets the retain_repo_versions of this OstreeOstreeRepositoryResponse.  # noqa: E501
 
-        Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
+        Retain X versions of the repository. Default is null which retains all versions.  # noqa: E501
 
         :return: The retain_repo_versions of this OstreeOstreeRepositoryResponse.  # noqa: E501
         :rtype: int
         """
         return self._retain_repo_versions
 
     @retain_repo_versions.setter
     def retain_repo_versions(self, retain_repo_versions):
         """Sets the retain_repo_versions of this OstreeOstreeRepositoryResponse.
 
-        Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
+        Retain X versions of the repository. Default is null which retains all versions.  # noqa: E501
 
         :param retain_repo_versions: The retain_repo_versions of this OstreeOstreeRepositoryResponse.  # noqa: E501
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 retain_repo_versions is not None and retain_repo_versions < 1):  # noqa: E501
             raise ValueError("Invalid value for `retain_repo_versions`, must be a value greater than or equal to `1`")  # noqa: E501
@@ -289,14 +294,35 @@
 
         :param remote: The remote of this OstreeOstreeRepositoryResponse.  # noqa: E501
         :type: str
         """
 
         self._remote = remote
 
+    @property
+    def compute_delta(self):
+        """Gets the compute_delta of this OstreeOstreeRepositoryResponse.  # noqa: E501
+
+
+        :return: The compute_delta of this OstreeOstreeRepositoryResponse.  # noqa: E501
+        :rtype: bool
+        """
+        return self._compute_delta
+
+    @compute_delta.setter
+    def compute_delta(self, compute_delta):
+        """Sets the compute_delta of this OstreeOstreeRepositoryResponse.
+
+
+        :param compute_delta: The compute_delta of this OstreeOstreeRepositoryResponse.  # noqa: E501
+        :type: bool
+        """
+
+        self._compute_delta = compute_delta
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/ostree_ostree_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/ostree_repository_add_remove_content.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_add_remove_content.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 import re  # noqa: F401
 
 import six
 
 from pulpcore.client.pulp_ostree.configuration import Configuration
 
 
-class OstreeRepositoryAddRemoveContent(object):
+class RepositoryAddRemoveContent(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'add_content_units': 'list[object]',
-        'remove_content_units': 'list[object]',
+        'add_content_units': 'list[str]',
+        'remove_content_units': 'list[str]',
         'base_version': 'str'
     }
 
     attribute_map = {
         'add_content_units': 'add_content_units',
         'remove_content_units': 'remove_content_units',
         'base_version': 'base_version'
     }
 
     def __init__(self, add_content_units=None, remove_content_units=None, base_version=None, local_vars_configuration=None):  # noqa: E501
-        """OstreeRepositoryAddRemoveContent - a model defined in OpenAPI"""  # noqa: E501
+        """RepositoryAddRemoveContent - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._add_content_units = None
         self._remove_content_units = None
         self._base_version = None
@@ -61,76 +61,76 @@
         if remove_content_units is not None:
             self.remove_content_units = remove_content_units
         if base_version is not None:
             self.base_version = base_version
 
     @property
     def add_content_units(self):
-        """Gets the add_content_units of this OstreeRepositoryAddRemoveContent.  # noqa: E501
+        """Gets the add_content_units of this RepositoryAddRemoveContent.  # noqa: E501
 
         A list of content units to add to a new repository version. This content is added after remove_content_units are removed.  # noqa: E501
 
-        :return: The add_content_units of this OstreeRepositoryAddRemoveContent.  # noqa: E501
-        :rtype: list[object]
+        :return: The add_content_units of this RepositoryAddRemoveContent.  # noqa: E501
+        :rtype: list[str]
         """
         return self._add_content_units
 
     @add_content_units.setter
     def add_content_units(self, add_content_units):
-        """Sets the add_content_units of this OstreeRepositoryAddRemoveContent.
+        """Sets the add_content_units of this RepositoryAddRemoveContent.
 
         A list of content units to add to a new repository version. This content is added after remove_content_units are removed.  # noqa: E501
 
-        :param add_content_units: The add_content_units of this OstreeRepositoryAddRemoveContent.  # noqa: E501
-        :type: list[object]
+        :param add_content_units: The add_content_units of this RepositoryAddRemoveContent.  # noqa: E501
+        :type: list[str]
         """
 
         self._add_content_units = add_content_units
 
     @property
     def remove_content_units(self):
-        """Gets the remove_content_units of this OstreeRepositoryAddRemoveContent.  # noqa: E501
+        """Gets the remove_content_units of this RepositoryAddRemoveContent.  # noqa: E501
 
         A list of content units to remove from the latest repository version. You may also specify '*' as an entry to remove all content. This content is removed before add_content_units are added.  # noqa: E501
 
-        :return: The remove_content_units of this OstreeRepositoryAddRemoveContent.  # noqa: E501
-        :rtype: list[object]
+        :return: The remove_content_units of this RepositoryAddRemoveContent.  # noqa: E501
+        :rtype: list[str]
         """
         return self._remove_content_units
 
     @remove_content_units.setter
     def remove_content_units(self, remove_content_units):
-        """Sets the remove_content_units of this OstreeRepositoryAddRemoveContent.
+        """Sets the remove_content_units of this RepositoryAddRemoveContent.
 
         A list of content units to remove from the latest repository version. You may also specify '*' as an entry to remove all content. This content is removed before add_content_units are added.  # noqa: E501
 
-        :param remove_content_units: The remove_content_units of this OstreeRepositoryAddRemoveContent.  # noqa: E501
-        :type: list[object]
+        :param remove_content_units: The remove_content_units of this RepositoryAddRemoveContent.  # noqa: E501
+        :type: list[str]
         """
 
         self._remove_content_units = remove_content_units
 
     @property
     def base_version(self):
-        """Gets the base_version of this OstreeRepositoryAddRemoveContent.  # noqa: E501
+        """Gets the base_version of this RepositoryAddRemoveContent.  # noqa: E501
 
         A repository version whose content will be used as the initial set of content for the new repository version  # noqa: E501
 
-        :return: The base_version of this OstreeRepositoryAddRemoveContent.  # noqa: E501
+        :return: The base_version of this RepositoryAddRemoveContent.  # noqa: E501
         :rtype: str
         """
         return self._base_version
 
     @base_version.setter
     def base_version(self, base_version):
-        """Sets the base_version of this OstreeRepositoryAddRemoveContent.
+        """Sets the base_version of this RepositoryAddRemoveContent.
 
         A repository version whose content will be used as the initial set of content for the new repository version  # noqa: E501
 
-        :param base_version: The base_version of this OstreeRepositoryAddRemoveContent.  # noqa: E501
+        :param base_version: The base_version of this RepositoryAddRemoveContent.  # noqa: E501
         :type: str
         """
 
         self._base_version = base_version
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -162,18 +162,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, OstreeRepositoryAddRemoveContent):
+        if not isinstance(other, RepositoryAddRemoveContent):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, OstreeRepositoryAddRemoveContent):
+        if not isinstance(other, RepositoryAddRemoveContent):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_commit_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_config_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_object_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_ref_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/paginatedostree_ostree_summary_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,26 +504,26 @@
 
         self._max_retries = max_retries
 
     @property
     def policy(self):
         """Gets the policy of this PatchedostreeOstreeRemote.  # noqa: E501
 
-                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           # noqa: E501
+                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           * `immediate` - immediate * `on_demand` - on_demand  # noqa: E501
 
         :return: The policy of this PatchedostreeOstreeRemote.  # noqa: E501
         :rtype: PolicyEnum
         """
         return self._policy
 
     @policy.setter
     def policy(self, policy):
         """Sets the policy of this PatchedostreeOstreeRemote.
 
-                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           # noqa: E501
+                 immediate - All OSTree objects are downloaded and saved during synchronization.         on_demand - Only commits, dirtrees, and refs are downloaded. Other OSTree objects are                     not downloaded until they are requested for the first time by a client.           * `immediate` - immediate * `on_demand` - on_demand  # noqa: E501
 
         :param policy: The policy of this PatchedostreeOstreeRemote.  # noqa: E501
         :type: PolicyEnum
         """
 
         self._policy = policy
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/patchedostree_ostree_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,45 +34,50 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'pulp_labels': 'dict(str, str)',
         'name': 'str',
         'description': 'str',
         'retain_repo_versions': 'int',
-        'remote': 'str'
+        'remote': 'str',
+        'compute_delta': 'bool'
     }
 
     attribute_map = {
         'pulp_labels': 'pulp_labels',
         'name': 'name',
         'description': 'description',
         'retain_repo_versions': 'retain_repo_versions',
-        'remote': 'remote'
+        'remote': 'remote',
+        'compute_delta': 'compute_delta'
     }
 
-    def __init__(self, pulp_labels=None, name=None, description=None, retain_repo_versions=None, remote=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, pulp_labels=None, name=None, description=None, retain_repo_versions=None, remote=None, compute_delta=True, local_vars_configuration=None):  # noqa: E501
         """PatchedostreeOstreeRepository - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._pulp_labels = None
         self._name = None
         self._description = None
         self._retain_repo_versions = None
         self._remote = None
+        self._compute_delta = None
         self.discriminator = None
 
         if pulp_labels is not None:
             self.pulp_labels = pulp_labels
         if name is not None:
             self.name = name
         self.description = description
         self.retain_repo_versions = retain_repo_versions
         self.remote = remote
+        if compute_delta is not None:
+            self.compute_delta = compute_delta
 
     @property
     def pulp_labels(self):
         """Gets the pulp_labels of this PatchedostreeOstreeRepository.  # noqa: E501
 
 
         :return: The pulp_labels of this PatchedostreeOstreeRepository.  # noqa: E501
@@ -143,26 +148,26 @@
 
         self._description = description
 
     @property
     def retain_repo_versions(self):
         """Gets the retain_repo_versions of this PatchedostreeOstreeRepository.  # noqa: E501
 
-        Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
+        Retain X versions of the repository. Default is null which retains all versions.  # noqa: E501
 
         :return: The retain_repo_versions of this PatchedostreeOstreeRepository.  # noqa: E501
         :rtype: int
         """
         return self._retain_repo_versions
 
     @retain_repo_versions.setter
     def retain_repo_versions(self, retain_repo_versions):
         """Sets the retain_repo_versions of this PatchedostreeOstreeRepository.
 
-        Retain X versions of the repository. Default is null which retains all versions. This is provided as a tech preview in Pulp 3 and may change in the future.  # noqa: E501
+        Retain X versions of the repository. Default is null which retains all versions.  # noqa: E501
 
         :param retain_repo_versions: The retain_repo_versions of this PatchedostreeOstreeRepository.  # noqa: E501
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
                 retain_repo_versions is not None and retain_repo_versions < 1):  # noqa: E501
             raise ValueError("Invalid value for `retain_repo_versions`, must be a value greater than or equal to `1`")  # noqa: E501
@@ -188,14 +193,35 @@
 
         :param remote: The remote of this PatchedostreeOstreeRepository.  # noqa: E501
         :type: str
         """
 
         self._remote = remote
 
+    @property
+    def compute_delta(self):
+        """Gets the compute_delta of this PatchedostreeOstreeRepository.  # noqa: E501
+
+
+        :return: The compute_delta of this PatchedostreeOstreeRepository.  # noqa: E501
+        :rtype: bool
+        """
+        return self._compute_delta
+
+    @compute_delta.setter
+    def compute_delta(self, compute_delta):
+        """Sets the compute_delta of this PatchedostreeOstreeRepository.
+
+
+        :param compute_delta: The compute_delta of this PatchedostreeOstreeRepository.  # noqa: E501
+        :type: bool
+        """
+
+        self._compute_delta = compute_delta
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/policy_enum.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/repair.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repair.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/repository_sync_url.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/models/repository_version_response.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/pulpcore/client/pulp_ostree/rest.py` & `pulp_ostree-client-2.1.0/pulpcore/client/pulp_ostree/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/setup.py` & `pulp_ostree-client-2.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_ostree-client"
-VERSION = "2.0.0a7.dev1676776305"
+VERSION = "2.1.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_async_operation_response.py` & `pulp_ostree-client-2.1.0/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_commits_api.py` & `pulp_ostree-client-2.1.0/test/test_content_commits_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_configs_api.py` & `pulp_ostree-client-2.1.0/test/test_content_configs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_objects_api.py` & `pulp_ostree-client-2.1.0/test/test_content_objects_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_refs_api.py` & `pulp_ostree-client-2.1.0/test/test_content_refs_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_summaries_api.py` & `pulp_ostree-client-2.1.0/test/test_content_summaries_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_content_summary_response.py` & `pulp_ostree-client-2.1.0/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_distributions_ostree_api.py` & `pulp_ostree-client-2.1.0/test/test_distributions_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_import_all.py` & `pulp_ostree-client-2.1.0/test/test_ostree_import_all.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_import_commits_to_ref.py` & `pulp_ostree-client-2.1.0/test/test_ostree_import_commits_to_ref.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_commit_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_commit_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_config_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_config_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_distribution.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_distribution_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_object_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_object_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_ref_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_ref_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_remote.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_remote_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_remote_response_hidden_fields.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_repository.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,16 @@
             return OstreeOstreeRepository(
                 pulp_labels = {
                     'key' : '0'
                     }, 
                 name = '0', 
                 description = '0', 
                 retain_repo_versions = 1, 
-                remote = '0'
+                remote = '0', 
+                compute_delta = True
             )
         else :
             return OstreeOstreeRepository(
                 name = '0',
         )
 
     def testOstreeOstreeRepository(self):
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_repository_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_repository_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,16 @@
                 pulp_labels = {
                     'key' : '0'
                     }, 
                 latest_version_href = '0', 
                 name = '0', 
                 description = '0', 
                 retain_repo_versions = 1, 
-                remote = '0'
+                remote = '0', 
+                compute_delta = True
             )
         else :
             return OstreeOstreeRepositoryResponse(
                 name = '0',
         )
 
     def testOstreeOstreeRepositoryResponse(self):
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_ostree_summary_response.py` & `pulp_ostree-client-2.1.0/test/test_ostree_ostree_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_ostree_repository_add_remove_content.py` & `pulp_ostree-client-2.1.0/test/test_repository_add_remove_content.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,47 +13,47 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import pulpcore.client.pulp_ostree
-from pulpcore.client.pulp_ostree.models.ostree_repository_add_remove_content import OstreeRepositoryAddRemoveContent  # noqa: E501
+from pulpcore.client.pulp_ostree.models.repository_add_remove_content import RepositoryAddRemoveContent  # noqa: E501
 from pulpcore.client.pulp_ostree.rest import ApiException
 
-class TestOstreeRepositoryAddRemoveContent(unittest.TestCase):
-    """OstreeRepositoryAddRemoveContent unit test stubs"""
+class TestRepositoryAddRemoveContent(unittest.TestCase):
+    """RepositoryAddRemoveContent unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test OstreeRepositoryAddRemoveContent
+        """Test RepositoryAddRemoveContent
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = pulpcore.client.pulp_ostree.models.ostree_repository_add_remove_content.OstreeRepositoryAddRemoveContent()  # noqa: E501
+        # model = pulpcore.client.pulp_ostree.models.repository_add_remove_content.RepositoryAddRemoveContent()  # noqa: E501
         if include_optional :
-            return OstreeRepositoryAddRemoveContent(
+            return RepositoryAddRemoveContent(
                 add_content_units = [
-                    null
+                    '0'
                     ], 
                 remove_content_units = [
-                    null
+                    '0'
                     ], 
                 base_version = '0'
             )
         else :
-            return OstreeRepositoryAddRemoveContent(
+            return RepositoryAddRemoveContent(
         )
 
-    def testOstreeRepositoryAddRemoveContent(self):
-        """Test OstreeRepositoryAddRemoveContent"""
+    def testRepositoryAddRemoveContent(self):
+        """Test RepositoryAddRemoveContent"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginated_repository_version_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_commit_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_commit_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_config_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_config_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_distribution_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_object_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_object_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_ref_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_ref_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_remote_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_repository_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_repository_response_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,16 @@
                         pulp_labels = {
                             'key' : '0'
                             }, 
                         latest_version_href = '0', 
                         name = '0', 
                         description = '0', 
                         retain_repo_versions = 1, 
-                        remote = '0', )
+                        remote = '0', 
+                        compute_delta = True, )
                     ]
             )
         else :
             return PaginatedostreeOstreeRepositoryResponseList(
         )
 
     def testPaginatedostreeOstreeRepositoryResponseList(self):
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_paginatedostree_ostree_summary_response_list.py` & `pulp_ostree-client-2.1.0/test/test_paginatedostree_ostree_summary_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_patchedostree_ostree_distribution.py` & `pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_patchedostree_ostree_remote.py` & `pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_patchedostree_ostree_repository.py` & `pulp_ostree-client-2.1.0/test/test_patchedostree_ostree_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,16 @@
             return PatchedostreeOstreeRepository(
                 pulp_labels = {
                     'key' : '0'
                     }, 
                 name = '0', 
                 description = '0', 
                 retain_repo_versions = 1, 
-                remote = '0'
+                remote = '0', 
+                compute_delta = True
             )
         else :
             return PatchedostreeOstreeRepository(
         )
 
     def testPatchedostreeOstreeRepository(self):
         """Test PatchedostreeOstreeRepository"""
```

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_policy_enum.py` & `pulp_ostree-client-2.1.0/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_remotes_ostree_api.py` & `pulp_ostree-client-2.1.0/test/test_remotes_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repair.py` & `pulp_ostree-client-2.1.0/test/test_repair.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repositories_ostree_api.py` & `pulp_ostree-client-2.1.0/test/test_repositories_ostree_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repositories_ostree_versions_api.py` & `pulp_ostree-client-2.1.0/test/test_repositories_ostree_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repository_sync_url.py` & `pulp_ostree-client-2.1.0/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_ostree-client-2.0.0a7.dev1676776305/test/test_repository_version_response.py` & `pulp_ostree-client-2.1.0/test/test_repository_version_response.py`

 * *Files identical despite different names*

