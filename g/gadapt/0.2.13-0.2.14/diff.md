# Comparing `tmp/gadapt-0.2.13.tar.gz` & `tmp/gadapt-0.2.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gadapt-0.2.13.tar", last modified: Thu May 25 20:01:16 2023, max compression
+gzip compressed data, was "dist\gadapt-0.2.14.tar", last modified: Sun May 28 17:26:21 2023, max compression
```

## Comparing `gadapt-0.2.13.tar` & `gadapt-0.2.14.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.872894 gadapt-0.2.13/
--rw-rw-rw-   0        0        0      320 2023-05-25 20:01:16.873893 gadapt-0.2.13/PKG-INFO
--rw-rw-rw-   0        0        0     3623 2023-05-25 15:08:36.000000 gadapt-0.2.13/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.658891 gadapt-0.2.13/gadapt/
--rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.13/gadapt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.683891 gadapt-0.2.13/gadapt/cost_finding/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.13/gadapt/cost_finding/__init__.py
--rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/cost_finding/base_cost_finder.py
--rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/cost_finding/common_cost_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.696392 gadapt-0.2.13/gadapt/crossover/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.13/gadapt/crossover/__init__.py
--rw-rw-rw-   0        0        0     7036 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/crossover/base_crossover.py
--rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.13/gadapt/crossover/uniform_crossover.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.698892 gadapt-0.2.13/gadapt/execution/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.13/gadapt/execution/__init__.py
--rw-rw-rw-   0        0        0     3101 2023-05-25 16:03:23.000000 gadapt-0.2.13/gadapt/execution/ga_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.705893 gadapt-0.2.13/gadapt/exit_check/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.13/gadapt/exit_check/__init__.py
--rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.13/gadapt/exit_check/avg_cost_exit_checker.py
--rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/exit_check/base_exit_checker.py
--rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.13/gadapt/exit_check/min_cost_exit_checker.py
--rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.13/gadapt/exit_check/requested_cost_exit_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.709391 gadapt-0.2.13/gadapt/factory/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.13/gadapt/factory/__init__.py
--rw-rw-rw-   0        0        0     9957 2023-05-25 16:26:07.000000 gadapt-0.2.13/gadapt/factory/ga_factory.py
--rw-rw-rw-   0        0        0     8842 2023-05-25 16:17:40.000000 gadapt-0.2.13/gadapt/ga.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.712393 gadapt-0.2.13/gadapt/ga_logging/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.13/gadapt/ga_logging/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.13/gadapt/ga_logging/logging_settings.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.742393 gadapt-0.2.13/gadapt/ga_model/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.13/gadapt/ga_model/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-05-24 06:43:20.000000 gadapt-0.2.13/gadapt/ga_model/chromosome.py
--rw-rw-rw-   0        0        0      683 2023-05-21 10:44:03.000000 gadapt-0.2.13/gadapt/ga_model/definitions.py
--rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.13/gadapt/ga_model/ga_options.py
--rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.13/gadapt/ga_model/ga_results.py
--rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/ga_model/gene.py
--rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/ga_model/genetic_variable.py
--rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.13/gadapt/ga_model/message_levels.py
--rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.13/gadapt/ga_model/population.py
--rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/ga_model/ranking_model.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.754891 gadapt-0.2.13/gadapt/gene_combination/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.13/gadapt/gene_combination/__init__.py
--rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/gene_combination/base_gene_combination.py
--rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.13/gadapt/gene_combination/blending_gene_combination.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.756391 gadapt-0.2.13/gadapt/immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.13/gadapt/immigration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.765894 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/__init__.py
--rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
--rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.13/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.775392 gadapt-0.2.13/gadapt/immigration/population_immigration/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.13/gadapt/immigration/population_immigration/__init__.py
--rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/immigration/population_immigration/base_population_immigrator.py
--rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.13/gadapt/immigration/population_immigration/common_population_immigrator.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.777393 gadapt-0.2.13/gadapt/mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.13/gadapt/mutation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.789893 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/__init__.py
--rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
--rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
--rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.13/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.797892 gadapt-0.2.13/gadapt/mutation/population_mutation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/__init__.py
--rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/base_population_mutator.py
--rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/composed_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.800393 gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0     1982 2023-05-23 23:45:44.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/parents_diversity_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.803894 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
--rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
--rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
--rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.13/gadapt/mutation/population_mutation/random_population_mutator.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.807392 gadapt-0.2.13/gadapt/parent_selection/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.13/gadapt/parent_selection/__init__.py
--rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/parent_selection/base_parent_selector.py
--rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.13/gadapt/parent_selection/sampling_parent_selector.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.826392 gadapt-0.2.13/gadapt/sampling/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.13/gadapt/sampling/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.13/gadapt/sampling/base_sampling.py
--rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.13/gadapt/sampling/from_top_to_bottom_sampling.py
--rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.13/gadapt/sampling/random_sampling.py
--rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.13/gadapt/sampling/roulette_wheel_sampling.py
--rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.13/gadapt/sampling/tournament_sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.828393 gadapt-0.2.13/gadapt/string_operation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.13/gadapt/string_operation/__init__.py
--rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.13/gadapt/string_operation/ga_strings.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.831893 gadapt-0.2.13/gadapt/utils/
--rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.13/gadapt/utils/TimeStampFormatter.py
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.13/gadapt/utils/__init__.py
--rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.13/gadapt/utils/ga_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.835892 gadapt-0.2.13/gadapt/validation/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.13/gadapt/validation/__init__.py
--rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.13/gadapt/validation/base_options_validator.py
--rw-rw-rw-   0        0        0    17426 2023-05-25 15:43:59.000000 gadapt-0.2.13/gadapt/validation/common_options_validator.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.869892 gadapt-0.2.13/gadapt/variable_update/
--rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.13/gadapt/variable_update/__init__.py
--rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.13/gadapt/variable_update/base_variable_updater.py
--rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.13/gadapt/variable_update/common_variable_updater.py
-drwxrwxrwx   0        0        0        0 2023-05-25 20:01:16.679391 gadapt-0.2.13/gadapt.egg-info/
--rw-rw-rw-   0        0        0      320 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3461 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 20:01:03.000000 gadapt-0.2.13/gadapt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-25 20:01:16.877393 gadapt-0.2.13/setup.cfg
--rw-rw-rw-   0        0        0      389 2023-05-25 20:00:39.000000 gadapt-0.2.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.202414 gadapt-0.2.14/
+-rw-rw-rw-   0        0        0      320 2023-05-28 17:26:21.202914 gadapt-0.2.14/PKG-INFO
+-rw-rw-rw-   0        0        0    19350 2023-05-28 15:29:08.000000 gadapt-0.2.14/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.018915 gadapt-0.2.14/gadapt/
+-rw-rw-rw-   0        0        0        2 2023-05-24 06:11:19.000000 gadapt-0.2.14/gadapt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.045914 gadapt-0.2.14/gadapt/cost_finding/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:46.000000 gadapt-0.2.14/gadapt/cost_finding/__init__.py
+-rw-rw-rw-   0        0        0      728 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/cost_finding/base_cost_finder.py
+-rw-rw-rw-   0        0        0     2112 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/cost_finding/common_cost_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.050913 gadapt-0.2.14/gadapt/crossover/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:39.000000 gadapt-0.2.14/gadapt/crossover/__init__.py
+-rw-rw-rw-   0        0        0     7034 2023-05-28 13:24:31.000000 gadapt-0.2.14/gadapt/crossover/base_crossover.py
+-rw-rw-rw-   0        0        0     1257 2023-05-23 23:45:14.000000 gadapt-0.2.14/gadapt/crossover/uniform_crossover.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.052914 gadapt-0.2.14/gadapt/execution/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:34.000000 gadapt-0.2.14/gadapt/execution/__init__.py
+-rw-rw-rw-   0        0        0     3233 2023-05-27 11:13:47.000000 gadapt-0.2.14/gadapt/execution/ga_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.059915 gadapt-0.2.14/gadapt/exit_check/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:29.000000 gadapt-0.2.14/gadapt/exit_check/__init__.py
+-rw-rw-rw-   0        0        0      315 2023-05-23 23:28:45.000000 gadapt-0.2.14/gadapt/exit_check/avg_cost_exit_checker.py
+-rw-rw-rw-   0        0        0     1060 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/exit_check/base_exit_checker.py
+-rw-rw-rw-   0        0        0      305 2023-05-23 23:28:54.000000 gadapt-0.2.14/gadapt/exit_check/min_cost_exit_checker.py
+-rw-rw-rw-   0        0        0      387 2023-05-23 23:29:00.000000 gadapt-0.2.14/gadapt/exit_check/requested_cost_exit_checker.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.061914 gadapt-0.2.14/gadapt/factory/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:24.000000 gadapt-0.2.14/gadapt/factory/__init__.py
+-rw-rw-rw-   0        0        0     9949 2023-05-28 13:25:45.000000 gadapt-0.2.14/gadapt/factory/ga_factory.py
+-rw-rw-rw-   0        0        0     8920 2023-05-28 13:38:36.000000 gadapt-0.2.14/gadapt/ga.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.072413 gadapt-0.2.14/gadapt/ga_logging/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:17.000000 gadapt-0.2.14/gadapt/ga_logging/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-05-24 07:42:21.000000 gadapt-0.2.14/gadapt/ga_logging/logging_settings.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.085914 gadapt-0.2.14/gadapt/ga_model/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:07.000000 gadapt-0.2.14/gadapt/ga_model/__init__.py
+-rw-rw-rw-   0        0        0     6671 2023-05-28 13:24:31.000000 gadapt-0.2.14/gadapt/ga_model/chromosome.py
+-rw-rw-rw-   0        0        0      680 2023-05-28 13:25:45.000000 gadapt-0.2.14/gadapt/ga_model/definitions.py
+-rw-rw-rw-   0        0        0     5248 2023-05-25 16:08:26.000000 gadapt-0.2.14/gadapt/ga_model/ga_options.py
+-rw-rw-rw-   0        0        0     1398 2023-05-24 16:01:11.000000 gadapt-0.2.14/gadapt/ga_model/ga_results.py
+-rw-rw-rw-   0        0        0     1339 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/ga_model/gene.py
+-rw-rw-rw-   0        0        0     2546 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/ga_model/genetic_variable.py
+-rw-rw-rw-   0        0        0       53 2023-05-17 16:44:58.000000 gadapt-0.2.14/gadapt/ga_model/message_levels.py
+-rw-rw-rw-   0        0        0    10169 2023-05-24 16:00:25.000000 gadapt-0.2.14/gadapt/ga_model/population.py
+-rw-rw-rw-   0        0        0      785 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/ga_model/ranking_model.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.089414 gadapt-0.2.14/gadapt/gene_combination/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:14:01.000000 gadapt-0.2.14/gadapt/gene_combination/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/gene_combination/base_gene_combination.py
+-rw-rw-rw-   0        0        0      837 2023-05-23 23:22:44.000000 gadapt-0.2.14/gadapt/gene_combination/blending_gene_combination.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.097914 gadapt-0.2.14/gadapt/immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:24.000000 gadapt-0.2.14/gadapt/immigration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.103914 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:55.000000 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/__init__.py
+-rw-rw-rw-   0        0        0      611 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py
+-rw-rw-rw-   0        0        0      336 2023-05-23 23:22:33.000000 gadapt-0.2.14/gadapt/immigration/chromosome_immigration/random_chromosome_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.108415 gadapt-0.2.14/gadapt/immigration/population_immigration/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:43.000000 gadapt-0.2.14/gadapt/immigration/population_immigration/__init__.py
+-rw-rw-rw-   0        0        0      174 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/immigration/population_immigration/base_population_immigrator.py
+-rw-rw-rw-   0        0        0      831 2023-05-23 23:22:20.000000 gadapt-0.2.14/gadapt/immigration/population_immigration/common_population_immigrator.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.113415 gadapt-0.2.14/gadapt/mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 00:04:04.000000 gadapt-0.2.14/gadapt/mutation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.122414 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:32.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/__init__.py
+-rw-rw-rw-   0        0        0      841 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
+-rw-rw-rw-   0        0        0     2938 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
+-rw-rw-rw-   0        0        0      936 2023-05-23 23:45:26.000000 gadapt-0.2.14/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.152413 gadapt-0.2.14/gadapt/mutation/population_mutation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:12.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/__init__.py
+-rw-rw-rw-   0        0        0     1402 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/base_population_mutator.py
+-rw-rw-rw-   0        0        0     1269 2023-05-23 23:43:50.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/composed_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.154915 gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:26.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     2899 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0     1976 2023-05-28 15:09:04.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.158914 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:13:19.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
+-rw-rw-rw-   0        0        0     3769 2023-05-24 06:54:24.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
+-rw-rw-rw-   0        0        0      469 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
+-rw-rw-rw-   0        0        0     1069 2023-05-23 23:46:12.000000 gadapt-0.2.14/gadapt/mutation/population_mutation/random_population_mutator.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.162414 gadapt-0.2.14/gadapt/parent_selection/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:56.000000 gadapt-0.2.14/gadapt/parent_selection/__init__.py
+-rw-rw-rw-   0        0        0      299 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/parent_selection/base_parent_selector.py
+-rw-rw-rw-   0        0        0      883 2023-05-23 23:20:13.000000 gadapt-0.2.14/gadapt/parent_selection/sampling_parent_selector.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.185414 gadapt-0.2.14/gadapt/sampling/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:48.000000 gadapt-0.2.14/gadapt/sampling/__init__.py
+-rw-rw-rw-   0        0        0      707 2023-05-24 06:38:53.000000 gadapt-0.2.14/gadapt/sampling/base_sampling.py
+-rw-rw-rw-   0        0        0      433 2023-05-23 23:19:58.000000 gadapt-0.2.14/gadapt/sampling/from_top_to_bottom_sampling.py
+-rw-rw-rw-   0        0        0      425 2023-05-23 23:46:22.000000 gadapt-0.2.14/gadapt/sampling/random_sampling.py
+-rw-rw-rw-   0        0        0     1812 2023-05-23 23:46:32.000000 gadapt-0.2.14/gadapt/sampling/roulette_wheel_sampling.py
+-rw-rw-rw-   0        0        0     2622 2023-05-23 23:46:42.000000 gadapt-0.2.14/gadapt/sampling/tournament_sampling.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.187914 gadapt-0.2.14/gadapt/string_operation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:11:28.000000 gadapt-0.2.14/gadapt/string_operation/__init__.py
+-rw-rw-rw-   0        0        0     3219 2023-05-24 06:41:20.000000 gadapt-0.2.14/gadapt/string_operation/ga_strings.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.192916 gadapt-0.2.14/gadapt/utils/
+-rw-rw-rw-   0        0        0      229 2023-05-04 17:34:59.000000 gadapt-0.2.14/gadapt/utils/TimeStampFormatter.py
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:32.000000 gadapt-0.2.14/gadapt/utils/__init__.py
+-rw-rw-rw-   0        0        0     1272 2023-05-25 15:37:31.000000 gadapt-0.2.14/gadapt/utils/ga_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.197914 gadapt-0.2.14/gadapt/validation/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:26.000000 gadapt-0.2.14/gadapt/validation/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-05-24 06:45:03.000000 gadapt-0.2.14/gadapt/validation/base_options_validator.py
+-rw-rw-rw-   0        0        0    17413 2023-05-28 13:25:45.000000 gadapt-0.2.14/gadapt/validation/common_options_validator.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.201415 gadapt-0.2.14/gadapt/variable_update/
+-rw-rw-rw-   0        0        0        0 2023-05-24 06:12:11.000000 gadapt-0.2.14/gadapt/variable_update/__init__.py
+-rw-rw-rw-   0        0        0      176 2023-05-24 06:38:52.000000 gadapt-0.2.14/gadapt/variable_update/base_variable_updater.py
+-rw-rw-rw-   0        0        0     2001 2023-05-24 06:54:25.000000 gadapt-0.2.14/gadapt/variable_update/common_variable_updater.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:26:21.039413 gadapt-0.2.14/gadapt.egg-info/
+-rw-rw-rw-   0        0        0      320 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3460 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 17:26:20.000000 gadapt-0.2.14/gadapt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-28 17:26:21.208913 gadapt-0.2.14/setup.cfg
+-rw-rw-rw-   0        0        0      389 2023-05-28 17:26:01.000000 gadapt-0.2.14/setup.py
```

### Comparing `gadapt-0.2.13/gadapt/cost_finding/base_cost_finder.py` & `gadapt-0.2.14/gadapt/cost_finding/base_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/cost_finding/common_cost_finder.py` & `gadapt-0.2.14/gadapt/cost_finding/common_cost_finder.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/crossover/base_crossover.py` & `gadapt-0.2.14/gadapt/crossover/base_crossover.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,16 @@
             if (genetic_variable_mother is None):
                 raise Exception("chromosomes in crossover do not have the same structure!")
             genetic_diversity.append(get_genetic_diversity(mother_gene, father_gene))
             var1, var2 = self.combine(mother_gene, father_gene)
             offspring1.add_gene(self.genetic_variable_father, var1)
             offspring2.add_gene(self.genetic_variable_father, var2)
         parrents_diversity = round(ga_utils.average(genetic_diversity), 2)
-        offspring1.parents_diversity = parrents_diversity
-        offspring2.parents_diversity = parrents_diversity
+        offspring1.parent_diversity = parrents_diversity
+        offspring2.parent_diversity = parrents_diversity
         offspring1.mutation_on_both_sides = self.mutation_on_both_sides
         offspring2.mutation_on_both_sides = self.mutation_on_both_sides
         offspring1.mother_id = mother.chromosome_id
         offspring2.mother_id = mother.chromosome_id
         offspring1.father_id = father.chromosome_id
         offspring2.father_id = father.chromosome_id
         self.increase_generation(offspring1, offspring2, mother, father)
```

### Comparing `gadapt-0.2.13/gadapt/crossover/uniform_crossover.py` & `gadapt-0.2.14/gadapt/crossover/uniform_crossover.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/execution/ga_executor.py` & `gadapt-0.2.14/gadapt/execution/ga_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,47 +15,47 @@
     def execute(self) -> GAResults:
         results = GAResults()
         try: 
             init_logging(self.ga_options.logging)                           
         except Exception as ex:
             results.messages.append((message_levels.WARNING, "Logging failed. Error message: {exc}".format(exc=str(ex))))
             self.ga_options.logging = False        
-        #try:
-        chromosome_mutator = self.factory.get_chromosome_mutator()
-        population_mutator = self.factory.get_population_mutator()
-        exit_checker = self.factory.get_exit_checker()
-        cost_finder = self.factory.get_cost_finder()
-        population_immigrator = self.factory.get_population_immigrator()
-        chromosome_immigrator = self.factory.get_chromosome_immigrator()
-        selector = self.factory.get_parent_selector()
-        gene_combination = self.factory.get_gene_combination()
-        crossover = self.factory.get_crossover(
-            gene_combination, chromosome_mutator, chromosome_immigrator)
-        variable_updater = variable_updater=self.factory.get_variable_updater()
-        population = Population(self.ga_options,
-                                chromosome_mutator=chromosome_mutator,
-                                population_mutator=population_mutator,
-                                exit_checker=exit_checker,
-                                cost_finder=cost_finder,
-                                population_immigrator=population_immigrator,
-                                chromosome_immigrator=chromosome_immigrator,
-                                selector=selector,
-                                crossover=crossover,
-                                variable_updater=variable_updater)
-        population.find_costs()
-        while not population.exit():
-            population.immigrate()
-            population.mate()
-            population.mutate()
-            population.find_costs()            
-        if population.timeout_expired:
-            results.messages.append((message_levels.WARNING, "Timeout expired!"))
-        best_individual = population.best_individual
-        results.min_cost = population.min_cost
-        results.number_of_iterations = population.population_generation
-        for g in best_individual:
-            results.result_values[g.genetic_variable.variable_id] = g.variable_value
-        #except Exception as ex:
-        #    results.success = False
-        #    results.messages.append((message_levels.ERROR, str(ex)))
+        try:
+            chromosome_mutator = self.factory.get_chromosome_mutator()
+            population_mutator = self.factory.get_population_mutator()
+            exit_checker = self.factory.get_exit_checker()
+            cost_finder = self.factory.get_cost_finder()
+            population_immigrator = self.factory.get_population_immigrator()
+            chromosome_immigrator = self.factory.get_chromosome_immigrator()
+            selector = self.factory.get_parent_selector()
+            gene_combination = self.factory.get_gene_combination()
+            crossover = self.factory.get_crossover(
+                gene_combination, chromosome_mutator, chromosome_immigrator)
+            variable_updater = variable_updater=self.factory.get_variable_updater()
+            population = Population(self.ga_options,
+                                    chromosome_mutator=chromosome_mutator,
+                                    population_mutator=population_mutator,
+                                    exit_checker=exit_checker,
+                                    cost_finder=cost_finder,
+                                    population_immigrator=population_immigrator,
+                                    chromosome_immigrator=chromosome_immigrator,
+                                    selector=selector,
+                                    crossover=crossover,
+                                    variable_updater=variable_updater)
+            population.find_costs()
+            while not population.exit():
+                population.immigrate()
+                population.mate()
+                population.mutate()
+                population.find_costs()            
+            if population.timeout_expired:
+                results.messages.append((message_levels.WARNING, "Timeout expired!"))
+            best_individual = population.best_individual
+            results.min_cost = population.min_cost
+            results.number_of_iterations = population.population_generation
+            for g in best_individual:
+                results.result_values[g.genetic_variable.variable_id] = g.variable_value
+        except Exception as ex:
+            results.success = False
+            results.messages.append((message_levels.ERROR, str(ex)))
         return results
```

### Comparing `gadapt-0.2.13/gadapt/exit_check/base_exit_checker.py` & `gadapt-0.2.14/gadapt/exit_check/base_exit_checker.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/factory/ga_factory.py` & `gadapt-0.2.14/gadapt/factory/ga_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from gadapt.immigration.population_immigration.common_population_immigrator import CommonPopulationImmigrator
 from gadapt.mutation.chromosome_mutation.base_chromosome_mutator import BaseChromosomeMutator
 from gadapt.mutation.chromosome_mutation.cross_diversity_chromosome_mutator import CrossDiversityChromosomeMutator
 from gadapt.mutation.chromosome_mutation.random_chromosome_mutator import RandomChromosomeMutator
 from gadapt.mutation.population_mutation.base_population_mutator import BasePopulationMutator
 from gadapt.mutation.population_mutation.composed_population_mutator import ComposedPopulationMutator
 from gadapt.mutation.population_mutation.cost_diversity.cost_diversity_population_mutator import CostDiversityPopulationMutator
-from gadapt.mutation.population_mutation.parents_diversity_population_mutator import ParentsDiversityPopulationMutator
+from gadapt.mutation.population_mutation.parent_diversity_population_mutator import ParentsDiversityPopulationMutator
 from gadapt.mutation.population_mutation.previous_cost_diversity.previous_cost_diversity_population_mutator import PreviousCostDiversityPopulationMutator
 from gadapt.mutation.population_mutation.previous_cost_diversity.previous_cost_diversity_property_taker import AvgPreviousCostCostDiversityPropertyTaker, BasePreviousCostDiversityPropertyTaker, MinPreviousCostCostDiversityPropertyTaker
 from gadapt.mutation.population_mutation.random_population_mutator import RandomPopulationMutator
 from gadapt.parent_selection.base_parent_selector import BaseParentSelector
 from gadapt.parent_selection.sampling_parent_selector import SamplingParentSelector
 from gadapt.sampling.base_sampling import BaseSampling
 from gadapt.sampling.from_top_to_bottom_sampling import FromTopToBottomSampling
@@ -84,31 +84,31 @@
         self.population_mutator_options_validation()
         if population_mutator_string is None:
             population_mutator_string = self.ga.population_mutation.strip()
         if population_mutator_string.find(definitions.PARAM_SEPARATOR) > -1:
             return self.get_population_mutator_combined()
         elif population_mutator_string == definitions.COST_DIVERSITY:
             return CostDiversityPopulationMutator(self.options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
-        elif population_mutator_string == definitions.PARENTS_DIVERSITY:
+        elif population_mutator_string == definitions.PARENT_DIVERSITY:
             return ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options)
         elif population_mutator_string == definitions.RANDOM:
             return RandomPopulationMutator(self.options)
         else:
             raise Exception("unknown population mutation")
 
     def get_previous_cost_diversity_property_taker(self) -> BasePreviousCostDiversityPropertyTaker:
         return AvgPreviousCostCostDiversityPropertyTaker()
 
     def get_population_mutator_combined(self) -> ComposedPopulationMutator:
         mutator_strings = [ms.strip() for ms in self.ga.population_mutation.split(definitions.PARAM_SEPARATOR)]
         if (self.is_cost_diversity_random(mutator_strings)):
             return CostDiversityPopulationMutator(self.options, RandomPopulationMutator(self.options))
-        if (self.is_cost_diversity_parents_diversity(mutator_strings)):
+        if (self.is_cost_diversity_parent_diversity(mutator_strings)):
             return CostDiversityPopulationMutator(self.options, ParentsDiversityPopulationMutator(self.get_sampling_method(self.ga.parent_diversity_mutation_chromosome_selection), self.options))
-        if self.is_cost_diversity_parents_diversity_random(mutator_strings):
+        if self.is_cost_diversity_parent_diversity_random(mutator_strings):
             composedPopulationMutator = ComposedPopulationMutator(self.options)
             composedPopulationMutator.append(ParentsDiversityPopulationMutator(self.get_sampling_method(
                 self.ga.parent_diversity_mutation_chromosome_selection), self.options))
             composedPopulationMutator.append(
                 RandomPopulationMutator(self.options))
             return PreviousCostDiversityPopulationMutator(self.options, composedPopulationMutator)
         composedPopulationMutator = ComposedPopulationMutator(self.options)
@@ -117,21 +117,21 @@
         return composedPopulationMutator
 
     def is_cost_diversity_random(self, mutator_strings: list):
         if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
         return False
 
-    def is_cost_diversity_parents_diversity(self, mutator_strings: list):
-        if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENTS_DIVERSITY in mutator_strings:
+    def is_cost_diversity_parent_diversity(self, mutator_strings: list):
+        if len(mutator_strings) == 2 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENT_DIVERSITY in mutator_strings:
             return True
         return False
 
-    def is_cost_diversity_parents_diversity_random(self, mutator_strings: list):
-        if len(mutator_strings) == 3 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENTS_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
+    def is_cost_diversity_parent_diversity_random(self, mutator_strings: list):
+        if len(mutator_strings) == 3 and definitions.COST_DIVERSITY in mutator_strings and definitions.PARENT_DIVERSITY in mutator_strings and definitions.RANDOM in mutator_strings:
             return True
         return False
 
     def get_parent_selector(self) -> BaseParentSelector:
         return SamplingParentSelector(self.get_sampling_method(self.ga.parent_selection))
 
     def get_sampling_method(self, str) -> BaseSampling:
```

### Comparing `gadapt-0.2.13/gadapt/ga.py` & `gadapt-0.2.14/gadapt/ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self,
                  cost_function = None,
                  population_size = 64, 
                  exit_check = definitions.AVG_COST,
                  requested_cost = sys.float_info.max,
                  max_attempt_no = 10,
                  parent_selection = definitions.ROULETTE_WHEEL,
-                 population_mutation = definitions.COST_DIVERSITY, 
+                 population_mutation = "{0}{1}{2}".format(definitions.COST_DIVERSITY, definitions.PARAM_SEPARATOR, definitions.PARENT_DIVERSITY),
                  number_of_mutation_chromosomes = -1,    
                  percentage_of_mutation_chromosomes = 10.0,
                  parent_diversity_mutation_chromosome_selection = definitions.ROULETTE_WHEEL, 
                  must_mutate_for_same_parents = True,
                  chromosome_mutation = definitions.CROSS_DIVERSITY,                                        
                  number_of_mutation_genes = -1,   
                  percentage_of_mutations_genes = 10.0,
```

### Comparing `gadapt-0.2.13/gadapt/ga_logging/logging_settings.py` & `gadapt-0.2.14/gadapt/ga_logging/logging_settings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/ga_model/chromosome.py` & `gadapt-0.2.14/gadapt/ga_model/chromosome.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,20 +134,20 @@
         self._father_id = value
 
     def add_gene(self, gen_var: GeneticVariable, gen_var_value: float = definitions.FLOAT_NAN):
         g = Gene(gen_var, gen_var_value)
         self.append(g)
 
     @property
-    def parents_diversity(self) -> float:
-        return self._parents_diversity
+    def parent_diversity(self) -> float:
+        return self._parent_diversity
     
-    @parents_diversity.setter
-    def parents_diversity(self, value: float):
-        self._parents_diversity = value
+    @parent_diversity.setter
+    def parent_diversity(self, value: float):
+        self._parent_diversity = value
 
     @property
     def population_generation(self) -> int:
         return self._population_generation
     
     @population_generation.setter
     def population_generation(self, value: int):
```

### Comparing `gadapt-0.2.13/gadapt/ga_model/definitions.py` & `gadapt-0.2.14/gadapt/ga_model/definitions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 RANDOM = "random"
 COST_DIVERSITY = "cost_diversity"
-PARENTS_DIVERSITY = "parents_diversity"
+PARENT_DIVERSITY = "parent_diversity"
 CROSS_DIVERSITY = "cross_diversity"
 TOURNAMENT = "tournament"
 FROM_TOP_TO_BOTTOM = "from_top_to_bottom"
 ROULETTE_WHEEL = "roulette_wheel"
 AVG_COST = "avg_cost"
 MIN_COST = "min_cost"
 REQUESTED = "requested"
 AVG = "avg"
 MIN = "min"
 PARAM_SEPARATOR = ","
 FLOAT_NAN = float("NaN")
 NOT_IMPLEMENTED = "not implemented"
-POPULATION_MUTATOR_STRINGS = [COST_DIVERSITY, PARENTS_DIVERSITY, RANDOM]
+POPULATION_MUTATOR_STRINGS = [COST_DIVERSITY, PARENT_DIVERSITY, RANDOM]
 CHROMOSOME_MUTATOR_STRINGS = [RANDOM, CROSS_DIVERSITY]
 SELECTION_STRINGS = [RANDOM, FROM_TOP_TO_BOTTOM, ROULETTE_WHEEL, TOURNAMENT]
 EXIT_CRITERIA_STRINGS = [AVG_COST, MIN_COST, REQUESTED]
```

### Comparing `gadapt-0.2.13/gadapt/ga_model/ga_options.py` & `gadapt-0.2.14/gadapt/ga_model/ga_options.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/ga_model/ga_results.py` & `gadapt-0.2.14/gadapt/ga_model/ga_results.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/ga_model/gene.py` & `gadapt-0.2.14/gadapt/ga_model/gene.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/ga_model/genetic_variable.py` & `gadapt-0.2.14/gadapt/ga_model/genetic_variable.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/ga_model/population.py` & `gadapt-0.2.14/gadapt/ga_model/population.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/ga_model/ranking_model.py` & `gadapt-0.2.14/gadapt/ga_model/ranking_model.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/gene_combination/blending_gene_combination.py` & `gadapt-0.2.14/gadapt/gene_combination/blending_gene_combination.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py` & `gadapt-0.2.14/gadapt/immigration/chromosome_immigration/base_chromosome_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/immigration/population_immigration/common_population_immigrator.py` & `gadapt-0.2.14/gadapt/immigration/population_immigration/common_population_immigrator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py` & `gadapt-0.2.14/gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py` & `gadapt-0.2.14/gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py` & `gadapt-0.2.14/gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/population_mutation/base_population_mutator.py` & `gadapt-0.2.14/gadapt/mutation/population_mutation/base_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/population_mutation/composed_population_mutator.py` & `gadapt-0.2.14/gadapt/mutation/population_mutation/composed_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py` & `gadapt-0.2.14/gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/population_mutation/parents_diversity_population_mutator.py` & `gadapt-0.2.14/gadapt/mutation/population_mutation/parent_diversity_population_mutator.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 
 class ParentsDiversityPopulationMutator(BasePopulationMutator):
         
     def __init__(self, sampling: BaseSampling, options: GAOptions) -> None:
         super().__init__(options)
         self.sampling = sampling
             
-    def sort_key_parents_diversity_random(self, c: Chromosome):
-        return (c.parents_diversity, random.random())      
+    def sort_key_parent_diversity_random(self, c: Chromosome):
+        return (c.parent_diversity, random.random())      
     
     def mutate_population(self, population, number_of_mutation_chromosomes):
         if population is None:
             raise Exception("Population must not be null")
         unallocated_chromosomes: List[Chromosome] = self.get_unallocated_chromosomes(
-            population, self.sort_key_parents_diversity_random)
+            population, self.sort_key_parent_diversity_random)
         chromosomes_for_mutation: List[Chromosome] = []
         if self.options.must_mutate_for_same_parents:
             chromosomes_for_mutation = [
-                c for c in unallocated_chromosomes if c.parents_diversity == 0]              
+                c for c in unallocated_chromosomes if c.parent_diversity == 0]              
         chromosomes_for_mutation_count = len(chromosomes_for_mutation)
         rest_number = number_of_mutation_chromosomes - chromosomes_for_mutation_count
         if rest_number > 0:
             if self.options.must_mutate_for_same_parents:
-                chromosomes_for_mutation = [c for c in unallocated_chromosomes if (not c.parents_diversity == 0)]
+                chromosomes_for_mutation = [c for c in unallocated_chromosomes if (not c.parent_diversity == 0)]
             else:
                 chromosomes_for_mutation = [c for c in unallocated_chromosomes]
-            chromosomes_for_mutation = self.sampling.get_sample(chromosomes_for_mutation, rest_number, lambda c: c.parents_diversity)       
+            chromosomes_for_mutation = self.sampling.get_sample(chromosomes_for_mutation, rest_number, lambda c: c.parent_diversity)       
         for c in chromosomes_for_mutation:
             c.mutate(self.options.number_of_mutation_genes)
         return len(chromosomes_for_mutation)
```

### Comparing `gadapt-0.2.13/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py` & `gadapt-0.2.14/gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/mutation/population_mutation/random_population_mutator.py` & `gadapt-0.2.14/gadapt/mutation/population_mutation/random_population_mutator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/parent_selection/sampling_parent_selector.py` & `gadapt-0.2.14/gadapt/parent_selection/sampling_parent_selector.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/sampling/base_sampling.py` & `gadapt-0.2.14/gadapt/sampling/base_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/sampling/roulette_wheel_sampling.py` & `gadapt-0.2.14/gadapt/sampling/roulette_wheel_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/sampling/tournament_sampling.py` & `gadapt-0.2.14/gadapt/sampling/tournament_sampling.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/string_operation/ga_strings.py` & `gadapt-0.2.14/gadapt/string_operation/ga_strings.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/utils/ga_utils.py` & `gadapt-0.2.14/gadapt/utils/ga_utils.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/validation/base_options_validator.py` & `gadapt-0.2.14/gadapt/validation/base_options_validator.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt/validation/common_options_validator.py` & `gadapt-0.2.14/gadapt/validation/common_options_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,22 @@
     def check_cost_function(self):
         if self.options.cost_function is None:
             self.add_message("Cost Function must not be None!")
             return False
         elif not callable(self.options.cost_function):
             self.add_message("Cost Function must be callable!")
             return False
-        kwargsmin = {}
-        kwargsmax = {}
+        argsmin = {}
+        argsmax = {}
         for v in self.options._genetic_variables:
-            kwargsmin[v.variable_id] = v.min_value
-            kwargsmax[v.variable_id] = v.max_value
+            argsmin[v.variable_id] = v.min_value
+            argsmax[v.variable_id] = v.max_value
         try:
-            func_result_min = self.options.cost_function(kwargsmin)
-            func_result_max = self.options.cost_function(kwargsmin)
+            func_result_min = self.options.cost_function(argsmin)
+            func_result_max = self.options.cost_function(argsmax)
             if not isinstance(func_result_min, float) or not isinstance(func_result_max, float):
                 self.add_message("The function must return float value!")
                 return False
         except KeyError:
             self.add_message("Inadequate number of parameters for the passed function!")
             return False
         except Exception as ex:
@@ -178,15 +178,15 @@
             rslt &= False        
         if self.options.must_mutate_for_same_parents is None:
             self.add_message("Must Mutate For Same Parents must not be None!")
             rslt &= False
         elif not isinstance(self.options.must_mutate_for_same_parents, bool):
             self.add_message("Must Mutate For Same Parents must be type bool!")
             rslt &= False 
-        if self.options.population_mutation == definitions.COST_DIVERSITY or definitions.PARENTS_DIVERSITY in self.options.population_mutation:
+        if self.options.population_mutation == definitions.COST_DIVERSITY or definitions.PARENT_DIVERSITY in self.options.population_mutation:
             if self.options.parent_diversity_mutation_chromosome_selection is None:
                 self.add_message("Parent Diversity Mutation Chromosome Selection must not be None!")
                 rslt &= False
             elif not isinstance(self.options.parent_diversity_mutation_chromosome_selection, str):
                 self.add_message("Parent Diversity Mutation Chromosome Selection must be type str!")
                 rslt &= False
             elif not self.validate_selection(self.options.parent_diversity_mutation_chromosome_selection, "Parents Diversity Mutation Chromosome Selection", (population_size // 2) - self.options.immigration_number, "Group Size for Parents Diversity Mutation Chromosome Selection cannot have the value below half population!"):
```

### Comparing `gadapt-0.2.13/gadapt/variable_update/common_variable_updater.py` & `gadapt-0.2.14/gadapt/variable_update/common_variable_updater.py`

 * *Files identical despite different names*

### Comparing `gadapt-0.2.13/gadapt.egg-info/SOURCES.txt` & `gadapt-0.2.14/gadapt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 gadapt/mutation/chromosome_mutation/__init__.py
 gadapt/mutation/chromosome_mutation/base_chromosome_mutator.py
 gadapt/mutation/chromosome_mutation/cross_diversity_chromosome_mutator.py
 gadapt/mutation/chromosome_mutation/random_chromosome_mutator.py
 gadapt/mutation/population_mutation/__init__.py
 gadapt/mutation/population_mutation/base_population_mutator.py
 gadapt/mutation/population_mutation/composed_population_mutator.py
-gadapt/mutation/population_mutation/parents_diversity_population_mutator.py
+gadapt/mutation/population_mutation/parent_diversity_population_mutator.py
 gadapt/mutation/population_mutation/random_population_mutator.py
 gadapt/mutation/population_mutation/cost_diversity/__init__.py
 gadapt/mutation/population_mutation/cost_diversity/cost_diversity_population_mutator.py
 gadapt/mutation/population_mutation/previous_cost_diversity/__init__.py
 gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_population_mutator.py
 gadapt/mutation/population_mutation/previous_cost_diversity/previous_cost_diversity_property_taker.py
 gadapt/parent_selection/__init__.py
```

