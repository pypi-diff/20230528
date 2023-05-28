# Comparing `tmp/gitlabform-ytt-3.7.0a4.tar.gz` & `tmp/gitlabform-ytt-3.7.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabform-ytt-3.7.0a4.tar", last modified: Sun May 28 09:24:20 2023, max compression
+gzip compressed data, was "gitlabform-ytt-3.7.0a5.tar", last modified: Sun May 28 09:28:49 2023, max compression
```

## Comparing `gitlabform-ytt-3.7.0a4.tar` & `gitlabform-ytt-3.7.0a5.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.049507 gitlabform-ytt-3.7.0a4/
--rw-r--r--   0 pattu      (502) staff       (20)     1091 2023-05-25 15:51:39.000000 gitlabform-ytt-3.7.0a4/LICENSE
--rw-r--r--   0 pattu      (502) staff       (20)     2388 2023-05-28 09:24:20.049732 gitlabform-ytt-3.7.0a4/PKG-INFO
--rw-r--r--   0 pattu      (502) staff       (20)     1196 2023-05-27 14:38:16.000000 gitlabform-ytt-3.7.0a4/README.md
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:19.947425 gitlabform-ytt-3.7.0a4/gitlabform/
--rw-r--r--   0 pattu      (502) staff       (20)    23874 2023-05-28 09:23:33.000000 gitlabform-ytt-3.7.0a4/gitlabform/__init__.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:19.951900 gitlabform-ytt-3.7.0a4/gitlabform/configuration/
--rw-r--r--   0 pattu      (502) staff       (20)      391 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/configuration/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)      589 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/configuration/common.py
--rw-r--r--   0 pattu      (502) staff       (20)    12541 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/configuration/core.py
--rw-r--r--   0 pattu      (502) staff       (20)     4705 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/configuration/groups.py
--rw-r--r--   0 pattu      (502) staff       (20)     2760 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/configuration/projects.py
--rw-r--r--   0 pattu      (502) staff       (20)    15180 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/configuration/transform.py
--rw-r--r--   0 pattu      (502) staff       (20)      277 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/constants.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:19.969521 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/
--rw-r--r--   0 pattu      (502) staff       (20)     2594 2023-05-25 16:27:36.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)     3624 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/branches.py
--rw-r--r--   0 pattu      (502) staff       (20)     1700 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/commits.py
--rw-r--r--   0 pattu      (502) staff       (20)    11524 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/core.py
--rw-r--r--   0 pattu      (502) staff       (20)     1354 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_badges.py
--rw-r--r--   0 pattu      (502) staff       (20)     1588 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_ldap_links.py
--rw-r--r--   0 pattu      (502) staff       (20)     1835 2023-05-25 19:38:39.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_saml_links.py
--rw-r--r--   0 pattu      (502) staff       (20)     1928 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_variables.py
--rw-r--r--   0 pattu      (502) staff       (20)     5919 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/groups.py
--rw-r--r--   0 pattu      (502) staff       (20)     1099 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/integrations.py
--rw-r--r--   0 pattu      (502) staff       (20)     3982 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/members.py
--rw-r--r--   0 pattu      (502) staff       (20)     1899 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/merge_requests.py
--rw-r--r--   0 pattu      (502) staff       (20)      855 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/pipelines.py
--rw-r--r--   0 pattu      (502) staff       (20)     1594 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_badges.py
--rw-r--r--   0 pattu      (502) staff       (20)     4539 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_deploy_keys.py
--rw-r--r--   0 pattu      (502) staff       (20)     4119 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_merge_requests_approvals.py
--rw-r--r--   0 pattu      (502) staff       (20)     1706 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_protected_environments.py
--rw-r--r--   0 pattu      (502) staff       (20)     9736 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/projects.py
--rw-r--r--   0 pattu      (502) staff       (20)     2254 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/repositories.py
--rw-r--r--   0 pattu      (502) staff       (20)      766 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/resource_groups.py
--rw-r--r--   0 pattu      (502) staff       (20)     3971 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/schedules.py
--rw-r--r--   0 pattu      (502) staff       (20)     1418 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/tags.py
--rw-r--r--   0 pattu      (502) staff       (20)      613 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/users.py
--rw-r--r--   0 pattu      (502) staff       (20)     1825 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/gitlab/variables.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:19.972892 gitlabform-ytt-3.7.0a4/gitlabform/lists/
--rw-r--r--   0 pattu      (502) staff       (20)     1689 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/lists/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)     3881 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/lists/filter.py
--rw-r--r--   0 pattu      (502) staff       (20)     2571 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/lists/groups.py
--rw-r--r--   0 pattu      (502) staff       (20)     5532 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/lists/projects.py
--rw-r--r--   0 pattu      (502) staff       (20)     1949 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/output.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:19.977377 gitlabform-ytt-3.7.0a4/gitlabform/processors/
--rw-r--r--   0 pattu      (502) staff       (20)     1256 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)     7790 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/abstract_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     3958 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/defining_keys.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:19.983607 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/
--rw-r--r--   0 pattu      (502) staff       (20)     1310 2023-05-25 16:46:34.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)      719 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_badges_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      737 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_ldap_links_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     9695 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_members_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      636 2023-05-25 16:48:36.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_saml_links_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      399 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_settings_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      684 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_variables_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     8955 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/multiple_entities_processor.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:19.998722 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/
--rw-r--r--   0 pattu      (502) staff       (20)     2744 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)      716 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/badges_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      678 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/branches_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      814 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/deploy_keys_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)    11944 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/files_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     1348 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/hooks_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      934 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/integrations_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     6738 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/members_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      712 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/merge_requests_approval_rules.py
--rw-r--r--   0 pattu      (502) staff       (20)      966 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/merge_requests_approvals.py
--rw-r--r--   0 pattu      (502) staff       (20)      618 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/project_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      469 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/project_push_rules_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      407 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/project_settings_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     1979 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/resource_groups_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     5026 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/schedules_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     1812 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/tags_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     2323 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/project/variables_processor.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.000311 gitlabform-ytt-3.7.0a4/gitlabform/processors/shared/
--rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/shared/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)      915 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/shared/protected_environments_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)     2201 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/single_entity_processor.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.003548 gitlabform-ytt-3.7.0a4/gitlabform/processors/util/
--rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/util/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)    14003 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/util/branch_protector.py
--rw-r--r--   0 pattu      (502) staff       (20)     1277 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/util/decorators.py
--rw-r--r--   0 pattu      (502) staff       (20)     2014 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/processors/util/difference_logger.py
--rw-r--r--   0 pattu      (502) staff       (20)      109 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/run.py
--rw-r--r--   0 pattu      (502) staff       (20)      189 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/gitlabform/util.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.009703 gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/
--rw-r--r--   0 pattu      (502) staff       (20)     2388 2023-05-28 09:24:19.000000 gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/PKG-INFO
--rw-r--r--   0 pattu      (502) staff       (20)     5425 2023-05-28 09:24:19.000000 gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/SOURCES.txt
--rw-r--r--   0 pattu      (502) staff       (20)        1 2023-05-28 09:24:19.000000 gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/dependency_links.txt
--rw-r--r--   0 pattu      (502) staff       (20)       54 2023-05-28 09:24:19.000000 gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/entry_points.txt
--rw-r--r--   0 pattu      (502) staff       (20)      445 2023-05-28 09:24:19.000000 gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/requires.txt
--rw-r--r--   0 pattu      (502) staff       (20)       17 2023-05-28 09:24:19.000000 gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/top_level.txt
--rw-r--r--   0 pattu      (502) staff       (20)      104 2023-05-28 09:24:20.051777 gitlabform-ytt-3.7.0a4/setup.cfg
--rw-r--r--   0 pattu      (502) staff       (20)     2818 2023-05-28 09:24:11.000000 gitlabform-ytt-3.7.0a4/setup.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.010522 gitlabform-ytt-3.7.0a4/tests/
--rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/__init__.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.012035 gitlabform-ytt-3.7.0a4/tests/acceptance/
--rw-r--r--   0 pattu      (502) staff       (20)     6996 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)     9214 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/conftest.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.034444 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/
--rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/__init__.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     2738 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_archive_project.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     5971 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_badges.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     3293 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_branches.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     8047 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_deploy_keys.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     1224 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_deploy_keys_all_projects.py
--rwxr-xr-x   0 pattu      (502) staff       (20)    10859 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     1434 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files_all.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     1951 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files_protected.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     3059 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files_templates.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     4136 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_badges.py
--rw-r--r--   0 pattu      (502) staff       (20)     7715 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_members_groups.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     9639 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_members_users.py
--rwxr-xr-x   0 pattu      (502) staff       (20)      882 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_settings.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     5622 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_variables.py
--rw-r--r--   0 pattu      (502) staff       (20)     1721 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_inheritance_break.py
--rwxr-xr-x   0 pattu      (502) staff       (20)    10353 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_integrations.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     2324 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_members.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     2071 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_members_add_group.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     2231 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_members_enforce.py
--rwxr-xr-x   0 pattu      (502) staff       (20)      544 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_project_settings.py
--rw-r--r--   0 pattu      (502) staff       (20)     1300 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_resource_groups.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     1664 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_running.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     7264 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_schedules.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     5045 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_tags.py
--rwxr-xr-x   0 pattu      (502) staff       (20)      871 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_token_from_config.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     5559 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_variables.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.037148 gitlabform-ytt-3.7.0a4/tests/unit/
--rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/__init__.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.045156 gitlabform-ytt-3.7.0a4/tests/unit/configuration/
--rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/__init__.py
--rwxr-xr-x   0 pattu      (502) staff       (20)     3042 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_case_sensitivity.py
--rw-r--r--   0 pattu      (502) staff       (20)     4914 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
--rw-r--r--   0 pattu      (502) staff       (20)     4306 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_inheritance_break_subgroups.py
--rw-r--r--   0 pattu      (502) staff       (20)     4291 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_inheritance_break_validation.py
--rw-r--r--   0 pattu      (502) staff       (20)     3902 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_projects_and_groups.py
--rw-r--r--   0 pattu      (502) staff       (20)     2575 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_skip_groups_skip_projects.py
--rw-r--r--   0 pattu      (502) staff       (20)     3614 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_subgroups.py
--rw-r--r--   0 pattu      (502) staff       (20)      589 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_yaml_version.py
-drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:24:20.048679 gitlabform-ytt-3.7.0a4/tests/unit/processors/
--rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/processors/__init__.py
--rw-r--r--   0 pattu      (502) staff       (20)     1092 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/processors/test_abstract_processor.py
--rw-r--r--   0 pattu      (502) staff       (20)      875 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/processors/test_branch_protector.py
--rw-r--r--   0 pattu      (502) staff       (20)     1042 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/processors/test_difference_logger.py
--rw-r--r--   0 pattu      (502) staff       (20)      687 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/test_access_levels.py
--rw-r--r--   0 pattu      (502) staff       (20)      760 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a4/tests/unit/test_non_empty_configs_provider.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.201297 gitlabform-ytt-3.7.0a5/
+-rw-r--r--   0 pattu      (502) staff       (20)     1091 2023-05-25 15:51:39.000000 gitlabform-ytt-3.7.0a5/LICENSE
+-rw-r--r--   0 pattu      (502) staff       (20)     2388 2023-05-28 09:28:49.201515 gitlabform-ytt-3.7.0a5/PKG-INFO
+-rw-r--r--   0 pattu      (502) staff       (20)     1196 2023-05-27 14:38:16.000000 gitlabform-ytt-3.7.0a5/README.md
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.094054 gitlabform-ytt-3.7.0a5/gitlabform/
+-rw-r--r--   0 pattu      (502) staff       (20)    23874 2023-05-28 09:23:33.000000 gitlabform-ytt-3.7.0a5/gitlabform/__init__.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.098629 gitlabform-ytt-3.7.0a5/gitlabform/configuration/
+-rw-r--r--   0 pattu      (502) staff       (20)      391 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/configuration/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)      589 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/configuration/common.py
+-rw-r--r--   0 pattu      (502) staff       (20)    12541 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/configuration/core.py
+-rw-r--r--   0 pattu      (502) staff       (20)     4705 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/configuration/groups.py
+-rw-r--r--   0 pattu      (502) staff       (20)     2760 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/configuration/projects.py
+-rw-r--r--   0 pattu      (502) staff       (20)    15180 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/configuration/transform.py
+-rw-r--r--   0 pattu      (502) staff       (20)      277 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/constants.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.118014 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/
+-rw-r--r--   0 pattu      (502) staff       (20)     2594 2023-05-25 16:27:36.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)     3624 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/branches.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1700 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/commits.py
+-rw-r--r--   0 pattu      (502) staff       (20)    11528 2023-05-28 09:28:21.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/core.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1354 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_badges.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1588 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_ldap_links.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1835 2023-05-25 19:38:39.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_saml_links.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1928 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_variables.py
+-rw-r--r--   0 pattu      (502) staff       (20)     5919 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/groups.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1099 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/integrations.py
+-rw-r--r--   0 pattu      (502) staff       (20)     3982 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/members.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1899 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/merge_requests.py
+-rw-r--r--   0 pattu      (502) staff       (20)      855 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/pipelines.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1594 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_badges.py
+-rw-r--r--   0 pattu      (502) staff       (20)     4539 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_deploy_keys.py
+-rw-r--r--   0 pattu      (502) staff       (20)     4119 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_merge_requests_approvals.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1706 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_protected_environments.py
+-rw-r--r--   0 pattu      (502) staff       (20)     9736 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/projects.py
+-rw-r--r--   0 pattu      (502) staff       (20)     2254 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/repositories.py
+-rw-r--r--   0 pattu      (502) staff       (20)      766 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/resource_groups.py
+-rw-r--r--   0 pattu      (502) staff       (20)     3971 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/schedules.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1418 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/tags.py
+-rw-r--r--   0 pattu      (502) staff       (20)      613 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/users.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1825 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/gitlab/variables.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.121622 gitlabform-ytt-3.7.0a5/gitlabform/lists/
+-rw-r--r--   0 pattu      (502) staff       (20)     1689 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/lists/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)     3881 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/lists/filter.py
+-rw-r--r--   0 pattu      (502) staff       (20)     2571 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/lists/groups.py
+-rw-r--r--   0 pattu      (502) staff       (20)     5532 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/lists/projects.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1949 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/output.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.126166 gitlabform-ytt-3.7.0a5/gitlabform/processors/
+-rw-r--r--   0 pattu      (502) staff       (20)     1256 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)     7790 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/abstract_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     3958 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/defining_keys.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.132469 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/
+-rw-r--r--   0 pattu      (502) staff       (20)     1310 2023-05-25 16:46:34.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)      719 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_badges_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      737 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_ldap_links_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     9695 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_members_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      636 2023-05-25 16:48:36.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_saml_links_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      399 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_settings_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      684 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_variables_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     8955 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/multiple_entities_processor.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.147559 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/
+-rw-r--r--   0 pattu      (502) staff       (20)     2744 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)      716 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/badges_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      678 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/branches_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      814 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/deploy_keys_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)    11944 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/files_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1348 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/hooks_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      934 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/integrations_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     6738 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/members_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      712 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/merge_requests_approval_rules.py
+-rw-r--r--   0 pattu      (502) staff       (20)      966 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/merge_requests_approvals.py
+-rw-r--r--   0 pattu      (502) staff       (20)      618 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/project_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      469 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/project_push_rules_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      407 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/project_settings_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1979 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/resource_groups_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     5026 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/schedules_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1812 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/tags_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     2323 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/project/variables_processor.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.149162 gitlabform-ytt-3.7.0a5/gitlabform/processors/shared/
+-rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/shared/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)      915 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/shared/protected_environments_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)     2201 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/single_entity_processor.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.152367 gitlabform-ytt-3.7.0a5/gitlabform/processors/util/
+-rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/util/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)    14003 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/util/branch_protector.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1277 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/util/decorators.py
+-rw-r--r--   0 pattu      (502) staff       (20)     2014 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/processors/util/difference_logger.py
+-rw-r--r--   0 pattu      (502) staff       (20)      109 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/run.py
+-rw-r--r--   0 pattu      (502) staff       (20)      189 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/gitlabform/util.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.159410 gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/
+-rw-r--r--   0 pattu      (502) staff       (20)     2388 2023-05-28 09:28:49.000000 gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/PKG-INFO
+-rw-r--r--   0 pattu      (502) staff       (20)     5425 2023-05-28 09:28:49.000000 gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/SOURCES.txt
+-rw-r--r--   0 pattu      (502) staff       (20)        1 2023-05-28 09:28:49.000000 gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/dependency_links.txt
+-rw-r--r--   0 pattu      (502) staff       (20)       54 2023-05-28 09:28:49.000000 gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/entry_points.txt
+-rw-r--r--   0 pattu      (502) staff       (20)      445 2023-05-28 09:28:49.000000 gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/requires.txt
+-rw-r--r--   0 pattu      (502) staff       (20)       17 2023-05-28 09:28:49.000000 gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/top_level.txt
+-rw-r--r--   0 pattu      (502) staff       (20)      104 2023-05-28 09:28:49.203714 gitlabform-ytt-3.7.0a5/setup.cfg
+-rw-r--r--   0 pattu      (502) staff       (20)     2818 2023-05-28 09:28:42.000000 gitlabform-ytt-3.7.0a5/setup.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.160340 gitlabform-ytt-3.7.0a5/tests/
+-rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/__init__.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.162083 gitlabform-ytt-3.7.0a5/tests/acceptance/
+-rw-r--r--   0 pattu      (502) staff       (20)     6996 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)     9214 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/conftest.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.185720 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/
+-rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/__init__.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     2738 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_archive_project.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     5971 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_badges.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     3293 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_branches.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     8047 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_deploy_keys.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     1224 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_deploy_keys_all_projects.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)    10859 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     1434 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files_all.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     1951 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files_protected.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     3059 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files_templates.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     4136 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_badges.py
+-rw-r--r--   0 pattu      (502) staff       (20)     7715 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_members_groups.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     9639 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_members_users.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)      882 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_settings.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     5622 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_variables.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1721 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_inheritance_break.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)    10353 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_integrations.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     2324 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_members.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     2071 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_members_add_group.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     2231 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_members_enforce.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)      544 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_project_settings.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1300 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_resource_groups.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     1664 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_running.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     7264 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_schedules.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     5045 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_tags.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)      871 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_token_from_config.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     5559 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_variables.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.188369 gitlabform-ytt-3.7.0a5/tests/unit/
+-rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/__init__.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.196875 gitlabform-ytt-3.7.0a5/tests/unit/configuration/
+-rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/__init__.py
+-rwxr-xr-x   0 pattu      (502) staff       (20)     3042 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_case_sensitivity.py
+-rw-r--r--   0 pattu      (502) staff       (20)     4914 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
+-rw-r--r--   0 pattu      (502) staff       (20)     4306 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_inheritance_break_subgroups.py
+-rw-r--r--   0 pattu      (502) staff       (20)     4291 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_inheritance_break_validation.py
+-rw-r--r--   0 pattu      (502) staff       (20)     3902 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_projects_and_groups.py
+-rw-r--r--   0 pattu      (502) staff       (20)     2575 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_skip_groups_skip_projects.py
+-rw-r--r--   0 pattu      (502) staff       (20)     3614 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_subgroups.py
+-rw-r--r--   0 pattu      (502) staff       (20)      589 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_yaml_version.py
+drwxr-xr-x   0 pattu      (502) staff       (20)        0 2023-05-28 09:28:49.200482 gitlabform-ytt-3.7.0a5/tests/unit/processors/
+-rw-r--r--   0 pattu      (502) staff       (20)        0 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/processors/__init__.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1092 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/processors/test_abstract_processor.py
+-rw-r--r--   0 pattu      (502) staff       (20)      875 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/processors/test_branch_protector.py
+-rw-r--r--   0 pattu      (502) staff       (20)     1042 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/processors/test_difference_logger.py
+-rw-r--r--   0 pattu      (502) staff       (20)      687 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/test_access_levels.py
+-rw-r--r--   0 pattu      (502) staff       (20)      760 2023-05-25 15:51:40.000000 gitlabform-ytt-3.7.0a5/tests/unit/test_non_empty_configs_provider.py
```

### Comparing `gitlabform-ytt-3.7.0a4/LICENSE` & `gitlabform-ytt-3.7.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/PKG-INFO` & `gitlabform-ytt-3.7.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform-ytt
-Version: 3.7.0a4
+Version: 3.7.0a5
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML. Forked changes pending inclusion in Gitlabform
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform-ytt Version: 3.7.0a4 Summary: ð
+Metadata-Version: 2.1 Name: gitlabform-ytt Version: 3.7.0a5 Summary: ð
 Specialized configuration as a code tool for GitLab projects, groups and more
 using hierarchical configuration written in YAML. Forked changes pending
 inclusion in Gitlabform Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors Keywords: cli,yaml,gitlab,configuration-
 as-code Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `gitlabform-ytt-3.7.0a4/README.md` & `gitlabform-ytt-3.7.0a5/README.md`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/__init__.py` & `gitlabform-ytt-3.7.0a5/gitlabform/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/configuration/common.py` & `gitlabform-ytt-3.7.0a5/gitlabform/configuration/common.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/configuration/core.py` & `gitlabform-ytt-3.7.0a5/gitlabform/configuration/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/configuration/groups.py` & `gitlabform-ytt-3.7.0a5/gitlabform/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/configuration/projects.py` & `gitlabform-ytt-3.7.0a5/gitlabform/configuration/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/configuration/transform.py` & `gitlabform-ytt-3.7.0a5/gitlabform/configuration/transform.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/__init__.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/branches.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/commits.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/commits.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/core.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.session.mount("http://", HTTPAdapter(max_retries=retries))
         self.session.mount("https://", HTTPAdapter(max_retries=retries))
 
         self.session.verify = self.ssl_verify
         if not self.ssl_verify:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-        self.gitlabform_version = pkg_resources.get_distribution("gitlabform").version
+        self.gitlabform_version = pkg_resources.get_distribution("gitlabform_ytt").version
         self.requests_version = pkg_resources.get_distribution("requests").version
         self.session.headers.update(
             {
                 "private-token": self.token,
                 "authorization": f"Bearer {self.token}",
                 "user-agent": f"GitLabForm/{self.gitlabform_version} (python-requests/{self.requests_version})",
             }
```

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_badges.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_ldap_links.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_ldap_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_saml_links.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_saml_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/group_variables.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/groups.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/integrations.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/members.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/merge_requests.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/merge_requests.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/pipelines.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/pipelines.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_badges.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_deploy_keys.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_merge_requests_approvals.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/project_protected_environments.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/project_protected_environments.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/projects.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/repositories.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/resource_groups.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/schedules.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/tags.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/users.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/gitlab/variables.py` & `gitlabform-ytt-3.7.0a5/gitlabform/gitlab/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/lists/__init__.py` & `gitlabform-ytt-3.7.0a5/gitlabform/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/lists/filter.py` & `gitlabform-ytt-3.7.0a5/gitlabform/lists/filter.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/lists/groups.py` & `gitlabform-ytt-3.7.0a5/gitlabform/lists/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/lists/projects.py` & `gitlabform-ytt-3.7.0a5/gitlabform/lists/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/output.py` & `gitlabform-ytt-3.7.0a5/gitlabform/output.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/__init__.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/abstract_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/defining_keys.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/defining_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/group/__init__.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/group/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_badges_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_ldap_links_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_ldap_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_members_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_saml_links_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_saml_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/group/group_variables_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/group/group_variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/multiple_entities_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/multiple_entities_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/__init__.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/badges_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/branches_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/branches_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/deploy_keys_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/deploy_keys_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/files_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/files_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/hooks_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/hooks_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/integrations_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/integrations_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/members_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/merge_requests_approval_rules.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/merge_requests_approval_rules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/merge_requests_approvals.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/project_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/project_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/resource_groups_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/resource_groups_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/schedules_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/schedules_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/tags_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/tags_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/project/variables_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/project/variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/shared/protected_environments_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/shared/protected_environments_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/single_entity_processor.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/single_entity_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/util/branch_protector.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/util/branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/util/decorators.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/util/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform/processors/util/difference_logger.py` & `gitlabform-ytt-3.7.0a5/gitlabform/processors/util/difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/PKG-INFO` & `gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform-ytt
-Version: 3.7.0a4
+Version: 3.7.0a5
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML. Forked changes pending inclusion in Gitlabform
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform-ytt Version: 3.7.0a4 Summary: ð
+Metadata-Version: 2.1 Name: gitlabform-ytt Version: 3.7.0a5 Summary: ð
 Specialized configuration as a code tool for GitLab projects, groups and more
 using hierarchical configuration written in YAML. Forked changes pending
 inclusion in Gitlabform Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors Keywords: cli,yaml,gitlab,configuration-
 as-code Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `gitlabform-ytt-3.7.0a4/gitlabform_ytt.egg-info/SOURCES.txt` & `gitlabform-ytt-3.7.0a5/gitlabform_ytt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/setup.py` & `gitlabform-ytt-3.7.0a5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         return github_actions_path + "/version"
     else:
         return "version"
 
 
 setup(
     name="gitlabform-ytt",
-    version="3.7.0a4",
+    version="3.7.0a5",
     description="🏗 Specialized configuration as a code tool for GitLab projects, groups and more"
     " using hierarchical configuration written in YAML. Forked changes pending inclusion in Gitlabform",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://gitlabform.github.io/gitlabform",
     author="Greg Dubicki and Contributors",
     keywords=["cli", "yaml", "gitlab", "configuration-as-code"],
```

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/__init__.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/conftest.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/conftest.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_archive_project.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_archive_project.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_badges.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_branches.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_deploy_keys.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_deploy_keys_all_projects.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_deploy_keys_all_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files_all.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files_all.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files_protected.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files_protected.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_files_templates.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_files_templates.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_badges.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_members_groups.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_members_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_members_users.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_members_users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_settings.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_group_variables.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_inheritance_break.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_inheritance_break.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_integrations.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_members.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_members_add_group.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_members_add_group.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_members_enforce.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_members_enforce.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_project_settings.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_project_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_resource_groups.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_running.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_running.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_schedules.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_tags.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_token_from_config.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_token_from_config.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/acceptance/standard/test_variables.py` & `gitlabform-ytt-3.7.0a5/tests/acceptance/standard/test_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_case_sensitivity.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_case_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_inheritance_break_projects_and_groups.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_inheritance_break_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_inheritance_break_subgroups.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_inheritance_break_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_inheritance_break_validation.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_inheritance_break_validation.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_projects_and_groups.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_skip_groups_skip_projects.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_skip_groups_skip_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_subgroups.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/configuration/test_yaml_version.py` & `gitlabform-ytt-3.7.0a5/tests/unit/configuration/test_yaml_version.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/processors/test_abstract_processor.py` & `gitlabform-ytt-3.7.0a5/tests/unit/processors/test_abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/processors/test_branch_protector.py` & `gitlabform-ytt-3.7.0a5/tests/unit/processors/test_branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/processors/test_difference_logger.py` & `gitlabform-ytt-3.7.0a5/tests/unit/processors/test_difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/test_access_levels.py` & `gitlabform-ytt-3.7.0a5/tests/unit/test_access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabform-ytt-3.7.0a4/tests/unit/test_non_empty_configs_provider.py` & `gitlabform-ytt-3.7.0a5/tests/unit/test_non_empty_configs_provider.py`

 * *Files identical despite different names*

