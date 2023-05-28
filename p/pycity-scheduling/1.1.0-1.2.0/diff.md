# Comparing `tmp/pycity_scheduling-1.1.0.tar.gz` & `tmp/pycity_scheduling-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycity_scheduling-1.1.0.tar", last modified: Wed Jan  5 14:30:08 2022, max compression
+gzip compressed data, was "pycity_scheduling-1.2.0.tar", last modified: Sun May 28 13:22:11 2023, max compression
```

## Comparing `pycity_scheduling-1.1.0.tar` & `pycity_scheduling-1.2.0.tar`

### file list

```diff
@@ -1,110 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.369569 pycity_scheduling-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    14115 2022-01-05 14:30:08.369569 pycity_scheduling-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    13062 2021-12-13 09:03:46.000000 pycity_scheduling-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-05 14:30:08.369569 pycity_scheduling-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2944 2022-01-05 13:52:38.000000 pycity_scheduling-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.314567 pycity_scheduling-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.317568 pycity_scheduling-1.1.0/src/pycity_scheduling/
--rw-rw-rw-   0 root         (0) root         (0)     1502 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.323568 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/
--rw-rw-rw-   0 root         (0) root         (0)     1865 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17641 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     3749 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/central_optimization_algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     7232 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     8933 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     4267 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/local_optimization_algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.337568 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/
--rw-rw-rw-   0 root         (0) root         (0)     6760 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3290 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/apartment.py
--rw-rw-rw-   0 root         (0) root         (0)     8208 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/battery.py
--rw-rw-rw-   0 root         (0) root         (0)     4584 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/boiler.py
--rw-rw-rw-   0 root         (0) root         (0)    10826 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/building.py
--rw-rw-rw-   0 root         (0) root         (0)     5673 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/building_energy_system.py
--rw-rw-rw-   0 root         (0) root         (0)     6643 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/chiller.py
--rw-rw-rw-   0 root         (0) root         (0)     4909 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/city_district.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/combined_heat_power.py
--rw-rw-rw-   0 root         (0) root         (0)    10897 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/curtailable_load.py
--rw-rw-rw-   0 root         (0) root         (0)    10613 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/deferrable_load.py
--rw-rw-rw-   0 root         (0) root         (0)     6282 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/electrical_entity.py
--rw-rw-rw-   0 root         (0) root         (0)     4571 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/electrical_heater.py
--rw-rw-rw-   0 root         (0) root         (0)    10977 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/electrical_vehicle.py
--rw-rw-rw-   0 root         (0) root         (0)     5435 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/entity_container.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     7916 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/fixed_load.py
--rw-rw-rw-   0 root         (0) root         (0)     6412 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/heat_pump.py
--rw-rw-rw-   0 root         (0) root         (0)    13587 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/optimization_entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6317 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/photovoltaic.py
--rw-rw-rw-   0 root         (0) root         (0)     9540 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/prices.py
--rw-rw-rw-   0 root         (0) root         (0)     4250 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/space_cooling.py
--rw-rw-rw-   0 root         (0) root         (0)     5768 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/space_heating.py
--rw-rw-rw-   0 root         (0) root         (0)     5670 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_cooling_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_entity_cooling.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_entity_heating.py
--rw-rw-rw-   0 root         (0) root         (0)     5668 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_heating_storage.py
--rw-rw-rw-   0 root         (0) root         (0)    11526 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/timer.py
--rw-rw-rw-   0 root         (0) root         (0)     1389 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/weather.py
--rw-rw-rw-   0 root         (0) root         (0)     4468 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/classes/wind_energy_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.344569 pycity_scheduling-1.1.0/src/pycity_scheduling/data/
--rw-rw-rw-   0 root         (0) root         (0)     1206 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   245151 2021-06-17 07:06:09.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt
--rw-rw-rw-   0 root         (0) root         (0)      157 2021-06-17 07:06:09.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/data/consumer_prices_yearly.txt
--rw-rw-rw-   0 root         (0) root         (0)   209814 2021-06-17 07:06:09.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt
--rw-rw-rw-   0 root         (0) root         (0)     5367 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/data/ev_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10134 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/data/tabula_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.361569 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1206 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9237 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_00_fundamentals.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_01_algorithm_central.py
--rw-rw-rw-   0 root         (0) root         (0)     4742 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_02_algorithm_local.py
--rw-rw-rw-   0 root         (0) root         (0)     4784 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py
--rw-rw-rw-   0 root         (0) root         (0)     5146 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)     5090 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py
--rw-rw-rw-   0 root         (0) root         (0)     7324 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_06_algorithm_warmstart.py
--rw-rw-rw-   0 root         (0) root         (0)     3976 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_07_objective_peak-shaving.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_08_objective_max-consumption.py
--rw-rw-rw-   0 root         (0) root         (0)     4014 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_09_objective_self-consumption.py
--rw-rw-rw-   0 root         (0) root         (0)     4559 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_10_objective_price.py
--rw-rw-rw-   0 root         (0) root         (0)     4662 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_11_objective_co2.py
--rw-rw-rw-   0 root         (0) root         (0)     5155 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_12_objective_valley-filling.py
--rw-rw-rw-   0 root         (0) root         (0)     4946 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_13_district_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     6333 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_14_district_flexibility_quantification.py
--rw-rw-rw-   0 root         (0) root         (0)     6480 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_15_scheduling_complex_city_district.py
--rw-rw-rw-   0 root         (0) root         (0)     7109 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_16_scheduling_convex_vs._integer_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     4985 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_17_scheduling_pv+battery_system.py
--rw-rw-rw-   0 root         (0) root         (0)     6817 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_18_scheduling_heating_and_cooling_loads.py
--rw-rw-rw-   0 root         (0) root         (0)     4556 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_19_scheduling_robust_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_20_post-processing_schedule_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_21_post-processing_metrics_evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)    12963 2021-12-21 16:52:15.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/illustrative_code_example_cost_minimization_use_case_interactive.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1540 2021-12-21 16:52:15.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/illustrative_code_example_listing1.py
--rw-rw-rw-   0 root         (0) root         (0)     2032 2021-12-21 16:52:15.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/illustrative_code_example_listing2.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2021-12-21 16:52:15.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/examples/illustrative_code_example_listing3.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2636 2022-01-05 14:26:50.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/solvers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.361569 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/
--rw-rw-rw-   0 root         (0) root         (0)     1206 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.365569 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/
--rw-rw-rw-   0 root         (0) root         (0)     1206 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8307 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_algorithms.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_all_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    71923 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_classes.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_examples.py
--rw-rw-rw-   0 root         (0) root         (0)    19315 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.368569 pycity_scheduling-1.1.0/src/pycity_scheduling/util/
--rw-rw-rw-   0 root         (0) root         (0)     9172 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4325 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/util/debug.py
--rw-rw-rw-   0 root         (0) root         (0)    17520 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/util/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5813 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/util/generic_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)    13889 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/util/metric.py
--rw-rw-rw-   0 root         (0) root         (0)    10387 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/util/plot_schedules.py
--rw-rw-rw-   0 root         (0) root         (0)     5488 2022-01-05 08:39:54.000000 pycity_scheduling-1.1.0/src/pycity_scheduling/util/write_schedules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-05 14:30:08.318568 pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14115 2022-01-05 14:30:08.000000 pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5166 2022-01-05 14:30:08.000000 pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-05 14:30:08.000000 pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-05 14:30:08.000000 pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      100 2022-01-05 14:30:08.000000 pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-01-05 14:30:08.000000 pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/top_level.txt
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.267594 pycity_scheduling-1.2.0/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1181 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/LICENSE.txt
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    14130 2023-05-28 13:22:11.267016 pycity_scheduling-1.2.0/PKG-INFO
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    13079 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/README.md
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)       38 2023-05-28 13:22:11.267760 pycity_scheduling-1.2.0/setup.cfg
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2997 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/setup.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.136260 pycity_scheduling-1.2.0/src/
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.145586 pycity_scheduling-1.2.0/src/pycity_scheduling/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1502 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/__init__.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.165029 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2407 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/__init__.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    18247 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/algorithm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     3790 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/central_optimization_algorithm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     7560 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    13129 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm_mpi.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     9471 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    15116 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm_mpi.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    38707 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    46132 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm_mpi.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4292 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/local_optimization_algorithm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2048 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.197266 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6740 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/__init__.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     3290 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/apartment.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     8281 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/battery.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4607 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/boiler.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    11100 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5741 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building_energy_system.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6643 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/chiller.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5335 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/city_district.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5130 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/combined_heat_power.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    10897 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/curtailable_load.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    10906 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/deferrable_load.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4564 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_heater.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    11739 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_vehicle.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6922 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electrical_entity.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5658 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/entity_container.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1406 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/environment.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     7916 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/fixed_load.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6414 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/heat_pump.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    13587 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/optimization_entity.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6350 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/photovoltaic.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     9540 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/prices.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4250 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_cooling.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5768 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_heating.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5680 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_cooling_storage.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2598 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_cooling.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2598 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_heating.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5736 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_heating_storage.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    11526 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/timer.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1389 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/weather.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4501 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/classes/wind_energy_converter.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1587 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/constants.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.219453 pycity_scheduling-1.2.0/src/pycity_scheduling/data/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)   878254 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/TRY_2018.dat
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/__init__.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)   245151 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)      157 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/consumer_prices_yearly.txt
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)   209814 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     3384 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/ev_data.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    10134 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/data/tabula_data.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.246022 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/__init__.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.247363 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/case_studies/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    14406 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/case_studies/illustrative_code_example_cost_minimization_use_case_interactive.ipynb
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     9230 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_00_fundamentals.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4939 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_01_algorithm_central.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4813 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_02_algorithm_local.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4855 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5299 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5161 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     7873 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_06_algorithm_exchange-miqp-admm.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     7440 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_07_algorithm_warmstart.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     9238 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_08_algorithm_parallel_mpi.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     3982 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_09_objective_peak-shaving.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     3993 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_10_objective_self-consumption.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4153 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_11_objective_max-consumption.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4565 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_12_objective_price.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4668 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_13_objective_co2.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5161 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_14_objective_valley-filling.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4942 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_15_district_generator.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6531 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_16_scheduling_complex_city_district.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6328 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_17_district_flexibility_quantification.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4987 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_18_scheduling_pv+battery_system.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     6816 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_19_scheduling_heating_and_cooling_loads.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     7198 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_20_scheduling_convex_vs._integer_mode.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4546 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_21_scheduling_robust_optimization.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     7526 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_22_post-processing_schedule_evaluation.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4739 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_23_post-processing_metrics_evaluation.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1605 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/exceptions.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2448 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/solvers.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.248615 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/__init__.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.255606 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     1206 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/__init__.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     9236 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_algorithms.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2627 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_all_classes.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    71186 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_classes.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     2064 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_examples.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    19729 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_util.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.265858 pycity_scheduling-1.2.0/src/pycity_scheduling/util/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     9168 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/__init__.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4325 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/debug.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    28659 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/district_analyzer.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    19720 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/factory.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5813 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/generic_constraints.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    13889 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/metric.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     4488 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/mpi_interface.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    10383 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/plot_schedules.py
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5488 2023-05-28 13:19:58.000000 pycity_scheduling-1.2.0/src/pycity_scheduling/util/write_schedules.py
+drwxr-xr-x   0 schwarz  (1000067) users    (1000001)        0 2023-05-28 13:22:11.151627 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)    14130 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/PKG-INFO
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)     5509 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/SOURCES.txt
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)        1 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/dependency_links.txt
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)        1 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/not-zip-safe
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)      114 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/requires.txt
+-rw-r--r--   0 schwarz  (1000067) users    (1000001)       18 2023-05-28 13:22:11.000000 pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/top_level.txt
```

### Comparing `pycity_scheduling-1.1.0/LICENSE.txt` & `pycity_scheduling-1.2.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 The MIT License
 
-Copyright (C) 2022, Institute for Automation of Complex Power Systems (ACS), E.ON Energy Research Center (E.ON ERC), RWTH Aachen University
+Copyright (C) 2023, Institute for Automation of Complex Power Systems (ACS), E.ON Energy Research Center (E.ON ERC), RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pycity_scheduling-1.1.0/PKG-INFO` & `pycity_scheduling-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycity_scheduling
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python framework for the development, testing, and assessment of optimization-basedpower scheduling algorithms for multi-energy systems in city districts
 Home-page: https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling
 Author: Institute for Automation of Complex Power Systems (ACS),E.ON Energy Research Center (E.ON ERC),RWTH Aachen University
 Author-email: post_acs@eonerc.rwth-aachen.de
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -62,15 +62,15 @@
 - [bonmin](https://github.com/coin-or/Bonmin)
 - [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
 - [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
 
 
 ### Installation of pycity_scheduling
 
-The latest version of pycity_scheduling is v1.1.0.
+The latest version of pycity_scheduling is v1.2.0.
 
 If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
 
 `pip install pycity_scheduling`
 
 or to install in editable mode:
 
@@ -119,15 +119,14 @@
 
 
 def main(do_plot=False):
     print("\n\n------ Example 00: Fundamentals ------\n\n")
 
     # 1) Environment objects:
 
-
     # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
     # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
     # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
 
     # Generate a timer object for the environment:
     timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
 
@@ -136,15 +135,14 @@
 
     # Generate a price object for the environment:
     price = Prices(timer=timer)
 
     # Generate the environment object:
     environment = Environment(timer=timer, weather=weather, prices=price)
 
-
     # Now there is a distinct environment object with timer, weather and price data.
     # We can use it to access different data of interest.
 
     # For example, print the current weekday:
     print('Weekday:')
     print(environment.timer.weekday)
 
@@ -152,15 +150,14 @@
     print('\nOutdoor temperature forecast:')
     print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
 
     # For example, print the energy spot market day-ahead prices:
     print('\nDay-ahead spot market prices on 2015/01/01:')
     print(environment.prices.da_prices)
 
-
     # 2) Buildings objects:
 
     # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
     # represent the different customers of the local energy system / city district under investigation.
     # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
     # necessarily represent a building structure, as it would be the case for a wind energy converter.
 
@@ -170,15 +167,14 @@
     # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
     # In general, every building object can, however, hold up to N different apartments (=multi-family house).
     apartment = Apartment(environment=environment)
     bes = BuildingEnergySystem(environment=environment)
 
     building.addMultipleEntities([apartment, bes])
 
-
     # Every apartment usually possesses both electrical and thermal loads:
     # The electrical load is added to the apartment as follows:
     load = FixedLoad(environment=environment, method=1, annual_demand=3000)
 
     # Print and show the electrical power curve in Watt:
     print('\nElectrical load in Watt:')
     print(load.get_power(currentValues=False))
@@ -201,15 +197,14 @@
     plt.ylabel('Thermal power in Watt (space heating)')
     plt.title('Space heating power curve')
     if do_plot:
         plt.show()
 
     apartment.addMultipleEntities([load, space_heating])
 
-
     # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
     # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
     # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
     # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
     # several optimization constraints.
     eh = HeatPump(environment=environment, p_th_nom=16.0)
     ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
@@ -218,15 +213,14 @@
     bes.addMultipleDevices([eh, ths, pv])
 
     # Verify if the assets were added successfully (method getHasDevice):
     print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
     print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
     print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
 
-
     # 3) CityDistrict objects:
 
     # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
     # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
     # their local assets and it hence includes all the optimization problem information and data.
 
     # Create a city district object:
@@ -260,15 +254,14 @@
 
     # Print the city district information:
     print('\nTotal number of buildings in city district:')
     print(cd.get_nb_of_building_entities())
     print("\nDetailed city district information:")
     debug.print_district(cd, 3)
 
-
     # 4) Power scheduling:
 
     # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
     # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
     # the city district object to a certain power scheduling algorithm.
     # Here, the central optimization algorithm is used.
 
@@ -298,15 +291,15 @@
 if __name__ == '__main__':
     # Run example:
     main(do_plot=True)
 ```
 
 ## Tutorial
 
-The pycity_scheduling package comes with several example/tutorial scripts in folder ./src/examples.
+The pycity_scheduling package comes with several example, tutorial, and simple case study scripts in folder ./src/examples.
 
 The unit tests can be found in folder ./src/testing.
 
 
 Moreover, also check the pycity_base package's tutorials for the basic usage of the framework's core functionalities. 
 
 
@@ -323,9 +316,7 @@
 
 [Institute for Automation of Complex Power Systems (ACS)](http://www.acs.eonerc.rwth-aachen.de) \
 [E.ON Energy Research Center (E.ON ERC)](http://www.eonerc.rwth-aachen.de) \
 [RWTH Aachen University, Germany](http://www.rwth-aachen.de)
 
 
 <img src="https://fein-aachen.org/img/logos/eonerc.png"/>
-
-
```

### Comparing `pycity_scheduling-1.1.0/README.md` & `pycity_scheduling-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 - [bonmin](https://github.com/coin-or/Bonmin)
 - [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
 - [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
 
 
 ### Installation of pycity_scheduling
 
-The latest version of pycity_scheduling is v1.1.0.
+The latest version of pycity_scheduling is v1.2.0.
 
 If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
 
 `pip install pycity_scheduling`
 
 or to install in editable mode:
 
@@ -96,15 +96,14 @@
 
 
 def main(do_plot=False):
     print("\n\n------ Example 00: Fundamentals ------\n\n")
 
     # 1) Environment objects:
 
-
     # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
     # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
     # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
 
     # Generate a timer object for the environment:
     timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
 
@@ -113,15 +112,14 @@
 
     # Generate a price object for the environment:
     price = Prices(timer=timer)
 
     # Generate the environment object:
     environment = Environment(timer=timer, weather=weather, prices=price)
 
-
     # Now there is a distinct environment object with timer, weather and price data.
     # We can use it to access different data of interest.
 
     # For example, print the current weekday:
     print('Weekday:')
     print(environment.timer.weekday)
 
@@ -129,15 +127,14 @@
     print('\nOutdoor temperature forecast:')
     print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
 
     # For example, print the energy spot market day-ahead prices:
     print('\nDay-ahead spot market prices on 2015/01/01:')
     print(environment.prices.da_prices)
 
-
     # 2) Buildings objects:
 
     # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
     # represent the different customers of the local energy system / city district under investigation.
     # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
     # necessarily represent a building structure, as it would be the case for a wind energy converter.
 
@@ -147,15 +144,14 @@
     # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
     # In general, every building object can, however, hold up to N different apartments (=multi-family house).
     apartment = Apartment(environment=environment)
     bes = BuildingEnergySystem(environment=environment)
 
     building.addMultipleEntities([apartment, bes])
 
-
     # Every apartment usually possesses both electrical and thermal loads:
     # The electrical load is added to the apartment as follows:
     load = FixedLoad(environment=environment, method=1, annual_demand=3000)
 
     # Print and show the electrical power curve in Watt:
     print('\nElectrical load in Watt:')
     print(load.get_power(currentValues=False))
@@ -178,15 +174,14 @@
     plt.ylabel('Thermal power in Watt (space heating)')
     plt.title('Space heating power curve')
     if do_plot:
         plt.show()
 
     apartment.addMultipleEntities([load, space_heating])
 
-
     # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
     # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
     # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
     # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
     # several optimization constraints.
     eh = HeatPump(environment=environment, p_th_nom=16.0)
     ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
@@ -195,15 +190,14 @@
     bes.addMultipleDevices([eh, ths, pv])
 
     # Verify if the assets were added successfully (method getHasDevice):
     print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
     print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
     print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
 
-
     # 3) CityDistrict objects:
 
     # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
     # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
     # their local assets and it hence includes all the optimization problem information and data.
 
     # Create a city district object:
@@ -237,15 +231,14 @@
 
     # Print the city district information:
     print('\nTotal number of buildings in city district:')
     print(cd.get_nb_of_building_entities())
     print("\nDetailed city district information:")
     debug.print_district(cd, 3)
 
-
     # 4) Power scheduling:
 
     # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
     # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
     # the city district object to a certain power scheduling algorithm.
     # Here, the central optimization algorithm is used.
 
@@ -275,15 +268,15 @@
 if __name__ == '__main__':
     # Run example:
     main(do_plot=True)
 ```
 
 ## Tutorial
 
-The pycity_scheduling package comes with several example/tutorial scripts in folder ./src/examples.
+The pycity_scheduling package comes with several example, tutorial, and simple case study scripts in folder ./src/examples.
 
 The unit tests can be found in folder ./src/testing.
 
 
 Moreover, also check the pycity_base package's tutorials for the basic usage of the framework's core functionalities.
```

### Comparing `pycity_scheduling-1.1.0/setup.py` & `pycity_scheduling-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2020,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -17,40 +17,42 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
+
 import setuptools
 from pathlib import Path
 
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setuptools.setup(
     name="pycity_scheduling",
     description="A Python framework for the development, testing, and assessment of optimization-based"
                 "power scheduling algorithms for multi-energy systems in city districts",
-    version="1.1.0",
+    version="1.2.0",
     author="Institute for Automation of Complex Power Systems (ACS),"
            "E.ON Energy Research Center (E.ON ERC),"
            "RWTH Aachen University",
     author_email="post_acs@eonerc.rwth-aachen.de",
     url="https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling",
     license="MIT",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
-    package_data={"pycity_scheduling": ["data/*.txt", "examples/*.ipynb"]},
+    package_data={"pycity_scheduling": ["data/*.txt", "data/*.dat", "examples/case_studies/*.ipynb"]},
     data_files=[(".", ["LICENSE.txt", "README.md"])],
     install_requires=[
         "numpy==1.19.5",
         "pandas==1.1.5",
         "matplotlib==3.3.4",
         "pyomo==5.7.3",
+        "mpi4py==3.1.3",
         "pycity_base==0.3.2"
     ],
     extras_require={
         "test": ["pytest==6.2.4"]
     },
     platforms="any",
     long_description=long_description,
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -21,29 +21,43 @@
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
 from .stand_alone_optimization_algorithm import StandAlone
 from .local_optimization_algorithm import LocalOptimization
 from .exchange_admm_algorithm import ExchangeADMM
+from .exchange_admm_algorithm_mpi import ExchangeADMMMPI
 from .central_optimization_algorithm import CentralOptimization
 from .dual_decomposition_algorithm import DualDecomposition
+from .dual_decomposition_algorithm_mpi import DualDecompositionMPI
+from .exchange_miqp_admm_algorithm import ExchangeMIQPADMM
+from .exchange_miqp_admm_algorithm_mpi import ExchangeMIQPADMMMPI
+
 
 
 __all__ = [
     'StandAlone',
     'LocalOptimization',
     'ExchangeADMM',
+    'ExchangeADMMMPI',
     'CentralOptimization',
     'DualDecomposition',
+    'DualDecompositionMPI',
+    'ExchangeMIQPADMM',
+    'ExchangeMIQPADMMMPI',
     'algorithm',
     'algorithms',
+
 ]
 
 
 algorithms = {
     'stand-alone': StandAlone,
     'local': LocalOptimization,
     'exchange-admm': ExchangeADMM,
+    'exchange-admm-mpi': ExchangeADMMMPI,
     'central': CentralOptimization,
     'dual-decomposition': DualDecomposition,
+    'dual-decomposition-mpi': DualDecompositionMPI,
+    'exchange-miqp-admm': ExchangeMIQPADMM,
+    'exchange-miqp-admm-mpi': ExchangeMIQPADMMMPI,
 }
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/algorithm.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/algorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -20,20 +20,21 @@
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
 import numpy as np
 import time
+import warnings
 import pyomo.environ as pyomo
 from pyomo.solvers.plugins.solvers.persistent_solver import PersistentSolver
 from pyomo.opt import SolverStatus, TerminationCondition
 
 from pycity_scheduling.classes import CityDistrict, Building
-from pycity_scheduling.exceptions import NonoptimalError, MaxIterationError
+from pycity_scheduling.exceptions import NonoptimalError
 from pycity_scheduling.solvers import DEFAULT_SOLVER, DEFAULT_SOLVER_OPTIONS
 
 
 class OptimizationAlgorithm:
     """
     Base class for all optimization algorithms.
 
@@ -206,49 +207,55 @@
             results["iterations"] = []
         iterations = results["iterations"]
         is_last_iteration = False
         while not is_last_iteration:
             iterations.append((iterations[-1] + 1) if len(iterations) > 0 else 1)
             self._iteration(results, params, debug=debug)
             self._save_time(results, params)
-            is_last_iteration = self._is_last_iteration(results, params)
+            is_last_iteration = self._is_last_iteration(results, params, debug)
         return
 
     def _iteration(self, results, params, debug):
         """Execute a single iteration of the algorithm.
 
         Parameters
         ----------
         results : dict
             Dictionary in which performance values of the algorithm are stored.
         params : dict
             Dictionary in which intermediate results are stored.
+        """
+        return
+
+    def _is_last_iteration(self, results, params, debug):
+        """Returns True if the current iteration is the last one.
+            It checks if the iteration limit is exceeded.
+            Overwrite this function to apply additional, individual stopping criteria other than the iteration limit.
+            Anyway, this parent method must be called in a child method, so that the check of an exceeded iteration
+            limit below is executed.
+
+        Parameters
+        ----------
         debug : bool, optional
             Specify whether detailed debug information shall be printed.
         Raises
         ------
-        MaxIterationError
+        Warning
             If the stopping criteria can not be reached in max_iterations.
         NonoptimalError
             If no feasible solution for the city district is found or a solver
             problem is encountered.
         """
-        if results["iterations"][-1] > self.max_iterations:
+        if results["iterations"][-1] >= self.max_iterations:
             if debug:
-                print(
-                    "Exceeded iteration limit of {0} iterations. "
-                    "Norms are ||r|| =  {1}, ||s|| = {2}."
-                        .format(self.max_iterations, results["r_norms"][-1], results["s_norms"][-1])
-                )
-            raise MaxIterationError("Iteration Limit exceeded.")
-        return
-
-    def _is_last_iteration(self, results, params):
-        """Returns True if the current iteration is the last one."""
-        raise NotImplementedError("This method should be implemented by subclass.")
+                warnings.warn("User defined iteration limit exceeded")
+            print("Exceeded the user defined iteration limit of {0} iterations. "
+                  "Terminating the iterative algorithm.".format(self.max_iterations))
+            return True
+        return False
 
 
 class DistributedAlgorithm(OptimizationAlgorithm):
     """Base class for all distributed optimization algorithms.
 
     These algorithms can divide the optimization problem into sub-problems.
     """
@@ -327,20 +334,21 @@
         - `convex`  : Use linear constraints
         - `integer`  : May use non-linear constraints
     robustness : tuple, optional
         Tuple of two floats. First entry defines how many time steps are
         protected from deviations. Second entry defines the magnitude of
         deviations which are considered.
     """
-    def __init__(self, solver, solver_options, entities, mode="convex", robustness=None):
+    def __init__(self, solver, solver_options, entities, mode="convex", robustness=None, write_ilp_file=False):
         self.solver = pyomo.SolverFactory(solver, node_ids=[entity.id for entity in entities],
                                           **solver_options.get("__call__", {}))
         self.solver_options = solver_options
         self.is_persistent = isinstance(self.solver, PersistentSolver)
         self.robustness = robustness
+        self.write_ilp_file = write_ilp_file
         self.entities = entities
         self.mode = mode
         self.model = None
         self._prepare()
 
     def _prepare(self):
         """Create the pyomo model for the entities and populate it."""
@@ -373,14 +381,22 @@
                 entity.update_model(mode=self.mode, robustness=robustness)
             else:
                 entity.update_model(mode=self.mode)
         if self.is_persistent:
             self.solver.set_instance(self.model, **self.solver_options.get("set_instance", {}))
         return
 
+    def constr_update(self):
+        """Only propagate the constraints update of the model."""
+        if self.is_persistent:
+            self.solver.set_instance(self.model, **self.solver_options.get("set_instance", {}))
+        else:
+            pass
+        return
+
     def obj_update(self):
         """Only propagate the objective value update of the model."""
         if self.is_persistent:
             self.solver.set_objective(self.model.o)
         else:
             pass
         return
@@ -408,15 +424,15 @@
                     solve_options["save_results"] = False
                     solve_options["load_solutions"] = False
                 result = self.solver.solve(**solve_options)
         else:
             result = self.solver.solve(self.model, **solve_options)
         if result.solver.termination_condition != TerminationCondition.optimal or \
                 result.solver.status != SolverStatus.ok:
-            if debug:
+            if debug and self.write_ilp_file:
                 import pycity_scheduling.util.debug as debug
                 debug.analyze_model(self.model, self.solver, result)
             raise NonoptimalError("Could not retrieve schedule from model.")
         if self.is_persistent and variables is not None:
             self.solver.load_vars(variables)
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/central_optimization_algorithm.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/central_optimization_algorithm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -26,18 +26,18 @@
 import pyomo.environ as pyomo
 
 from pycity_scheduling.algorithms.algorithm import OptimizationAlgorithm, SolverNode
 from pycity_scheduling.solvers import DEFAULT_SOLVER, DEFAULT_SOLVER_OPTIONS
 
 
 class CentralOptimization(OptimizationAlgorithm):
-    """ Implementation of a central Algorithm.
+    """
+    Implementation of the reference Central Optimization algorithm.
 
-        Only creates one model and calls the solver only once. Combines the
-        objectives of all entities.
+    Only creates one model and calls the solver once. Combines the objectives of all entities.
     """
     def __init__(self, city_district, solver=DEFAULT_SOLVER, solver_options=DEFAULT_SOLVER_OPTIONS, mode="convex",
                  robustness=None):
         super(CentralOptimization, self).__init__(city_district, solver, solver_options, mode)
         # create single solver node for all entities
         self.node = SolverNode(solver, solver_options, self.entities, mode, robustness=robustness)
         # add coupling between all entities in the single model
@@ -55,21 +55,21 @@
         Parameters
         ----------
         model : pyomo.ConcreteModel
             Model to add the constraint to.
         """
         def p_el_couple_rule(model, t):
             return self.city_district.model.p_el_vars[t] == \
-                   pyomo.quicksum(entity.model.p_el_vars[t] for entity in self.entities[1:])
+                   sum(entity.model.p_el_vars[t] for entity in self.entities[1:])
         model.couple = pyomo.Constraint(self.city_district.model.t, rule=p_el_couple_rule)
         return
 
     def _add_objective(self):
-        self.node.model.o = pyomo.Objective(expr=pyomo.quicksum(entity.model.beta * entity.get_objective()
-                                                                for entity in self.entities))
+        self.node.model.o = pyomo.Objective(expr=sum(entity.model.beta * entity.get_objective()
+                                                     for entity in self.entities))
         return
 
     def _presolve(self, full_update, beta, robustness, debug):
         results, params = super()._presolve(full_update, beta, robustness, debug)
         for entity in self.entities:
             entity.model.beta = self._get_beta(params, beta)
         if full_update:
@@ -77,8 +77,9 @@
         else:
             self.node.obj_update()
         return results, params
 
     def _solve(self, results, params, debug):
         self.node.solve(variables=None, debug=debug)
         self._save_time(results, params)
+        results["obj_value"] = pyomo.value(self.node.model.o)
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -28,128 +28,130 @@
 from pycity_scheduling.classes import (CityDistrict, Building, Photovoltaic, WindEnergyConverter)
 from pycity_scheduling.util import extract_pyomo_values
 from pycity_scheduling.algorithms.algorithm import IterationAlgorithm, DistributedAlgorithm, SolverNode
 from pycity_scheduling.solvers import DEFAULT_SOLVER, DEFAULT_SOLVER_OPTIONS
 
 
 class DualDecomposition(IterationAlgorithm, DistributedAlgorithm):
-    """Implementation of the Dual Decomposition Algorithm.
+    """
+    Implementation of the distributed Dual Decomposition algorithm.
 
+    Parameters
+    ----------
+    city_district : CityDistrict
+    solver : str, optional
+        Solver to use for solving (sub)problems.
+    solver_options : dict, optional
+        Options to pass to calls to the solver. Keys are the name of
+        the functions being called and are one of `__call__`, `set_instance_`,
+        `solve`.
+        `__call__` is the function being called when generating an instance
+        with the pyomo SolverFactory.  Additionally to the options provided,
+        `node_ids` is passed to this call containing the IDs of the entities
+        being optimized.
+        `set_instance` is called when a pyomo Model is set as an instance of
+        a persistent solver. `solve` is called to perform an optimization. If
+        not set, `save_results` and `load_solutions` may be set to false to
+        provide a speedup.
+    mode : str, optional
+        Specifies which set of constraints to use.
+        - `convex`  : Use linear constraints
+        - `integer`  : May use non-linear constraints
+    eps_primal : float, optional
+        Primal stopping criterion for the dual decomposition algorithm.
+    rho : float, optional
+        Step size for the dual decomposition algorithm.
+    max_iterations : int, optional
+        Maximum number of ADMM iterations.
+    robustness : tuple, optional
+        Tuple of two floats. First entry defines how many time steps are
+        protected from deviations. Second entry defines the magnitude of
+        deviations which are considered.
     """
     def __init__(self, city_district, solver=DEFAULT_SOLVER, solver_options=DEFAULT_SOLVER_OPTIONS, mode="convex",
                  eps_primal=0.1, rho=2.0, max_iterations=10000, robustness=None):
-        """
-        Set up the Dual Decomposition Algorithm for optimizing a specific city district.
-
-        Parameters
-        ----------
-        city_district : CityDistrict
-        solver : str, optional
-            Solver to use for solving (sub)problems.
-        solver_options : dict, optional
-            Options to pass to calls to the solver. Keys are the name of
-            the functions being called and are one of `__call__`, `set_instance_`,
-            `solve`.
-            `__call__` is the function being called when generating an instance
-            with the pyomo SolverFactory.  Additionally to the options provided,
-            `node_ids` is passed to this call containing the IDs of the entities
-            being optimized.
-            `set_instance` is called when a pyomo Model is set as an instance of
-            a persistent solver. `solve` is called to perform an optimization. If
-            not set, `save_results` and `load_solutions` may be set to false to
-            provide a speedup.
-        mode : str, optional
-            Specifies which set of constraints to use.
-            - `convex`  : Use linear constraints
-            - `integer`  : May use non-linear constraints
-        eps_primal : float, optional
-            Primal stopping criterion for the dual decomposition algorithm.
-        rho : float, optional
-            Stepsize for the dual decomposition algorithm.
-        max_iterations : int, optional
-            Maximum number of ADMM iterations.
-        robustness : tuple, optional
-            Tuple of two floats. First entry defines how many time steps are
-            protected from deviations. Second entry defines the magnitude of
-            deviations which are considered.
-        """
         super(DualDecomposition, self).__init__(city_district, solver, solver_options, mode)
         self.eps_primal = eps_primal
         self.rho = rho
         self.max_iterations = max_iterations
-        # create solver nodes for each entity
-        self.nodes = [
-            SolverNode(solver, solver_options, [entity], mode, robustness=robustness)
-            for entity in self.entities
-        ]
-        # create pyomo parameters for each entity
-        for node, entity in zip(self.nodes, self.entities):
+        self.op_horizon = self.city_district.op_horizon
+
+        # Only consider entities of type CityDistrict, Building, Photovoltaic, WindEnergyConverter
+        self._entities = [entity for entity in self.entities if
+                          isinstance(entity, (CityDistrict, Building, Photovoltaic, WindEnergyConverter))]
+
+        # Create a solver node for each entity
+        self.nodes = [SolverNode(solver, solver_options, [entity], mode, robustness=robustness)
+                      for entity in self._entities]
+
+        # Create pyomo parameters for each entity
+        for node, entity in zip(self.nodes, self._entities):
             node.model.beta = pyomo.Param(mutable=True, initialize=1)
             node.model.lambdas = pyomo.Param(entity.model.t, mutable=True, initialize=0)
         self._add_objective()
 
     def _add_objective(self):
-        for i, node, entity in zip(range(len(self.entities)), self.nodes, self.entities):
+        for i, node, entity in zip(range(len(self._entities)), self.nodes, self._entities):
             obj = node.model.beta * entity.get_objective()
             if i == 0:
                 # penalty term is expanded and constant is omitted
-                # invert sign of p_el_schedule and p_el_vars (omitted for quadratic
-                # term)
-                obj -= pyomo.sum_product(node.model.lambdas, entity.model.p_el_vars)
+                # invert sign of p_el_schedule and p_el_vars (omitted for quadratic term)
+                for t in range(self.op_horizon):
+                    obj -= node.model.lambdas[t] * entity.model.p_el_vars[t]
             else:
-                obj += pyomo.sum_product(node.model.lambdas, entity.model.p_el_vars)
+                for t in range(self.op_horizon):
+                    obj += node.model.lambdas[t] * entity.model.p_el_vars[t]
             node.model.o = pyomo.Objective(expr=obj)
         return
 
     def _presolve(self, full_update, beta, robustness, debug):
         results, params = super()._presolve(full_update, beta, robustness, debug)
-
-        for node, entity in zip(self.nodes, self.entities):
+        for node, entity in zip(self.nodes, self._entities):
             node.model.beta = self._get_beta(params, entity)
             if full_update:
                 node.full_update(robustness)
         results["r_norms"] = []
         results["lambdas"] = []
         return results, params
 
-    def _is_last_iteration(self, results, params):
+    def _is_last_iteration(self, results, params, debug):
+        if super(DualDecomposition, self)._is_last_iteration(results, params, debug):
+            return True
         return results["r_norms"][-1] <= self.eps_primal
 
     def _iteration(self, results, params, debug):
         super(DualDecomposition, self)._iteration(results, params, debug)
-        op_horizon = self.entities[0].op_horizon
         if "lambdas" not in params:
-            params["lambdas"] = np.zeros(op_horizon)
+            params["lambdas"] = np.zeros(self.op_horizon)
         lambdas = params["lambdas"]
 
-        # -----------------
-        # 1) optimize all entities
-        # -----------------
-        for i, node, entity in zip(range(len(self.nodes)), self.nodes, self.entities):
-            if not isinstance(
-                    entity,
-                    (CityDistrict, Building, Photovoltaic, WindEnergyConverter)
-            ):
-                continue
-            for t in range(op_horizon):
+        # ------------------------------------------
+        # 1) Optimize all entities
+        # ------------------------------------------
+        for i, node, entity in zip(range(len(self._entities)), self.nodes, self._entities):
+            for t in range(self.op_horizon):
                 node.model.lambdas[t] = lambdas[t]
             node.obj_update()
-            node.solve(variables=[entity.model.p_el_vars[t] for t in range(op_horizon)], debug=debug)
+            node.solve(variables=[entity.model.p_el_vars[t] for t in range(self.op_horizon)], debug=debug)
 
-        # --------------------------
-        # 2) incentive signal update
-        # --------------------------
-        p_el_schedules = np.array([extract_pyomo_values(entity.model.p_el_vars, float) for entity in self.entities])
+        # ------------------------------------------
+        # 2) Calculate incentive signal update
+        # ------------------------------------------
+        p_el_schedules = np.array([extract_pyomo_values(entity.model.p_el_vars, float) for entity in self._entities])
         lambdas -= self.rho * p_el_schedules[0]
         lambdas += self.rho * np.sum(p_el_schedules[1:], axis=0)
 
         # ------------------------------------------
         # 3) Calculate parameters for stopping criteria
         # ------------------------------------------
-        r = np.zeros(op_horizon)
+        r = np.zeros(self.op_horizon)
         r -= p_el_schedules[0]
         r += np.sum(p_el_schedules[1:], axis=0)
-
-        # save parameters for another iteration
         results["r_norms"].append(np.linalg.norm(r, np.inf))
         results["lambdas"].append(np.copy(lambdas))
+
+        # ------------------------------------------
+        # 4) Save required parameters for another iteration
+        # ------------------------------------------
+        params["lambdas"] = lambdas
+
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/exchange_admm_algorithm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -28,17 +28,17 @@
 from pycity_scheduling.classes import (CityDistrict, Building, Photovoltaic, WindEnergyConverter)
 from pycity_scheduling.util import extract_pyomo_values
 from pycity_scheduling.algorithms.algorithm import IterationAlgorithm, DistributedAlgorithm, SolverNode
 from pycity_scheduling.solvers import DEFAULT_SOLVER, DEFAULT_SOLVER_OPTIONS
 
 
 class ExchangeADMM(IterationAlgorithm, DistributedAlgorithm):
-    """Implementation of the Exchange ADMM Algorithm.
-
-    Uses the Exchange ADMM algorithm described in [1].
+    """
+    Implementation of the distributed ADMM algorithm.
+    This class implements the Exchange ADMM as described in [1].
 
     Parameters
     ----------
     city_district : CityDistrict
     solver : str, optional
         Solver to use for solving (sub)problems.
     solver_options : dict, optional
@@ -58,136 +58,136 @@
         - `convex`  : Use linear constraints
         - `integer`  : May use non-linear constraints
     eps_primal : float, optional
         Primal stopping criterion for the ADMM algorithm.
     eps_dual : float, optional
         Dual stopping criterion for the ADMM algorithm.
     rho : float, optional
-        Stepsize for the ADMM algorithm.
+        Step size for the ADMM algorithm.
     max_iterations : int, optional
         Maximum number of ADMM iterations.
     robustness : tuple, optional
         Tuple of two floats. First entry defines how many time steps are
         protected from deviations. Second entry defines the magnitude of
         deviations which are considered.
 
     References
     ----------
-    .. [1] "Alternating Direction Method of Multipliers for Decentralized
-       Electric Vehicle Charging Control" by Jose Rivera, Philipp Wolfrum,
-       Sandra Hirche, Christoph Goebel, and Hans-Arno Jacobsen
-       Online: https://mediatum.ub.tum.de/doc/1187583/1187583.pdf (accessed on 2020/09/28)
+    [1] "Alternating Direction Method of Multipliers for Decentralized
+    Electric Vehicle Charging Control" by Jose Rivera, Philipp Wolfrum,
+    Sandra Hirche, Christoph Goebel, and Hans-Arno Jacobsen
+    Online: https://mediatum.ub.tum.de/doc/1187583/1187583.pdf (accessed on 2020/09/28)
     """
     def __init__(self, city_district, solver=DEFAULT_SOLVER, solver_options=DEFAULT_SOLVER_OPTIONS, mode="convex",
                  eps_primal=0.1, eps_dual=1.0, rho=2.0, max_iterations=10000, robustness=None):
         super(ExchangeADMM, self).__init__(city_district, solver, solver_options, mode)
         self.eps_primal = eps_primal
         self.eps_dual = eps_dual
         self.rho = rho
         self.max_iterations = max_iterations
-        # create solver nodes for each entity
-        self.nodes = [
-            SolverNode(solver, solver_options, [entity], mode, robustness=robustness)
-            for entity in self.entities
-        ]
-        # create pyomo parameters for each entity
-        for node, entity in zip(self.nodes, self.entities):
+        self.op_horizon = self.city_district.op_horizon
+
+        # Only consider entities of type CityDistrict, Building, Photovoltaic, WindEnergyConverter
+        self._entities = [entity for entity in self.entities if
+                          isinstance(entity, (CityDistrict, Building, Photovoltaic, WindEnergyConverter))]
+
+        # Create a solver node for each entity
+        self.nodes = [SolverNode(solver, solver_options, [entity], mode, robustness=robustness)
+                      for entity in self._entities]
+
+        # Create pyomo parameters for each entity
+        for node, entity in zip(self.nodes, self._entities):
             node.model.beta = pyomo.Param(mutable=True, initialize=1)
             node.model.xs_ = pyomo.Param(entity.model.t, mutable=True, initialize=0)
             node.model.us = pyomo.Param(entity.model.t, mutable=True, initialize=0)
             node.model.last_p_el_schedules = pyomo.Param(entity.model.t, mutable=True, initialize=0)
         self._add_objective()
 
     def _add_objective(self):
-        for i, node, entity in zip(range(len(self.entities)), self.nodes, self.entities):
+        for i, node, entity in zip(range(len(self._entities)), self.nodes, self._entities):
             obj = node.model.beta * entity.get_objective()
-            obj += self.rho / 2 * pyomo.sum_product(entity.model.p_el_vars, entity.model.p_el_vars)
+            for t in range(self.op_horizon):
+                obj += self.rho / 2 * entity.model.p_el_vars[t] * entity.model.p_el_vars[t]
             # penalty term is expanded and constant is omitted
             if i == 0:
-                # invert sign of p_el_schedule and p_el_vars (omitted for quadratic
-                # term)
-                obj += self.rho * pyomo.sum_product(
-                    [(-node.model.last_p_el_schedules[t] - node.model.xs_[t] - node.model.us[t])
-                     for t in range(entity.op_horizon)],
-                     entity.model.p_el_vars
-                )
+                # invert sign of p_el_schedule and p_el_vars (omitted for quadratic term)
+                penalty = [(-node.model.last_p_el_schedules[t] - node.model.xs_[t] - node.model.us[t])
+                           for t in range(self.op_horizon)]
+                for t in range(self.op_horizon):
+                    obj += self.rho * penalty[t] * entity.model.p_el_vars[t]
             else:
-                obj += self.rho * pyomo.sum_product(
-                    [(-node.model.last_p_el_schedules[t] + node.model.xs_[t] + node.model.us[t])
-                     for t in range(entity.op_horizon)],
-                    entity.model.p_el_vars
-                )
+                penalty = [(-node.model.last_p_el_schedules[t] + node.model.xs_[t] + node.model.us[t])
+                           for t in range(self.op_horizon)]
+                for t in range(self.op_horizon):
+                    obj += self.rho * penalty[t] * entity.model.p_el_vars[t]
             node.model.o = pyomo.Objective(expr=obj)
         return
 
     def _presolve(self, full_update, beta, robustness, debug):
         results, params = super()._presolve(full_update, beta, robustness, debug)
-
-        for node, entity in zip(self.nodes, self.entities):
+        for node, entity in zip(self.nodes, self._entities):
             node.model.beta = self._get_beta(params, entity)
             if full_update:
                 node.full_update(robustness)
         results["r_norms"] = []
         results["s_norms"] = []
         return results, params
 
-    def _is_last_iteration(self, results, params):
+    def _is_last_iteration(self, results, params, debug):
+        if super(ExchangeADMM, self)._is_last_iteration(results, params, debug):
+            return True
         return results["r_norms"][-1] <= self.eps_primal and results["s_norms"][-1] <= self.eps_dual
 
     def _iteration(self, results, params, debug):
         super(ExchangeADMM, self)._iteration(results, params, debug)
-        op_horizon = self.entities[0].op_horizon
 
         # fill parameters if not already present
         if "p_el" not in params:
-            params["p_el"] = np.zeros((len(self.entities), op_horizon))
+            params["p_el"] = np.zeros((len(self._entities), self.op_horizon))
         if "x_" not in params:
-            params["x_"] = np.zeros(op_horizon)
+            params["x_"] = np.zeros(self.op_horizon)
         if "u" not in params:
-            params["u"] = np.zeros(op_horizon)
-        u = params["u"]
+            params["u"] = np.zeros(self.op_horizon)
+        last_u = params["u"]
+        last_p_el = params["p_el"]
+        last_x_ = params["x_"]
 
-        # -----------------
-        # 1) optimize all entities
-        # -----------------
+        # ------------------------------------------
+        # 1) Optimize all entities
+        # ------------------------------------------
         to_solve_nodes = []
         variables = []
-        for i, node, entity in zip(range(len(self.nodes)), self.nodes, self.entities):
-            if not isinstance(
-                    entity,
-                    (CityDistrict, Building, Photovoltaic, WindEnergyConverter)
-            ):
-                continue
-
-            for t in range(op_horizon):
-                node.model.last_p_el_schedules[t] = params["p_el"][i][t]
-                node.model.xs_[t] = params["x_"][t]
-                node.model.us[t] = params["u"][t]
+        for i, node, entity in zip(range(len(self._entities)), self.nodes, self._entities):
+            for t in range(self.op_horizon):
+                node.model.last_p_el_schedules[t] = last_p_el[i][t]
+                node.model.xs_[t] = last_x_[t]
+                node.model.us[t] = last_u[t]
             node.obj_update()
             to_solve_nodes.append(node)
-            variables.append([entity.model.p_el_vars[t] for t in range(op_horizon)])
+            variables.append([entity.model.p_el_vars[t] for t in range(self.op_horizon)])
         self._solve_nodes(results, params, to_solve_nodes, variables=variables, debug=debug)
 
-        # --------------------------
-        # 2) incentive signal update
-        # --------------------------
-        p_el_schedules = np.array([extract_pyomo_values(entity.model.p_el_vars, float) for entity in self.entities])
-        x_ = (-p_el_schedules[0] + sum(p_el_schedules[1:])) / len(self.entities)
-
-        u += x_
+        # ------------------------------------------
+        # 2) Calculate incentive signal update
+        # ------------------------------------------
+        p_el_schedules = np.array([extract_pyomo_values(entity.model.p_el_vars, float) for entity in self._entities])
+        x_ = (-p_el_schedules[0] + sum(p_el_schedules[1:])) / len(self._entities)
 
         # ------------------------------------------
         # 3) Calculate parameters for stopping criteria
         # ------------------------------------------
-        results["r_norms"].append(np.math.sqrt(len(self.entities)) * np.linalg.norm(x_))
+        results["r_norms"].append(np.math.sqrt(len(self._entities)) * np.linalg.norm(x_))
 
         s = np.zeros_like(p_el_schedules)
-        s[0] = - self.rho * (-p_el_schedules[0] + params["p_el"][0] + params["x_"] - x_)
-        for i in range(1, len(self.entities)):
-            s[i] = - self.rho * (p_el_schedules[i] - params["p_el"][i] + params["x_"] - x_)
+        s[0] = - self.rho * (-p_el_schedules[0] + last_p_el[0] + last_x_ - x_)
+        for i in range(1, len(self._entities)):
+            s[i] = - self.rho * (p_el_schedules[i] - last_p_el[i] + last_x_ - x_)
         results["s_norms"].append(np.linalg.norm(s.flatten()))
 
-        # save parameters for another iteration
+        # ------------------------------------------
+        # 4) Save required parameters for another iteration
+        # ------------------------------------------
         params["p_el"] = p_el_schedules
         params["x_"] = x_
-        params["u"] = u
+        params["u"] += x_
+
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/local_optimization_algorithm.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/local_optimization_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -26,17 +26,18 @@
 import pyomo.environ as pyomo
 
 from pycity_scheduling.algorithms.algorithm import DistributedAlgorithm, SolverNode
 from pycity_scheduling.solvers import DEFAULT_SOLVER, DEFAULT_SOLVER_OPTIONS
 
 
 class LocalOptimization(DistributedAlgorithm):
-    """Implementation of the reference optimization algorithm.
+    """
+    Implementation of the reference Local Optimization algorithm.
 
-        Schedule all nodes in `city_district` on their own.
+    Schedule all nodes (i.e., buildings) in `city_district` on their own.
     """
     def __init__(self, city_district, solver=DEFAULT_SOLVER, solver_options=DEFAULT_SOLVER_OPTIONS, mode="convex",
                  robustness=None):
         super(LocalOptimization, self).__init__(city_district, solver, solver_options, mode)
         # create solver nodes for each entity
         self.nodes = [
             SolverNode(solver, solver_options, [entity], mode, robustness=robustness)
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -26,20 +26,20 @@
 import pyomo.environ as pyomo
 
 from pycity_scheduling.classes.city_district import CityDistrict
 from pycity_scheduling.algorithms.local_optimization_algorithm import LocalOptimization
 
 
 class StandAlone(LocalOptimization):
-    """Implementation of the reference optimization algorithm.
-
-    Schedule all entities in `city_district` on their own.
+    """
+    Implementation of the reference Stand-alone Optimization algorithm.
 
+    Schedule all entities (i.e., devices) in `city_district` on their own.
     """
     def _add_objective(self):
         for node, entity in zip(self.nodes, self.entities):
             if not isinstance(entity, CityDistrict):
-                node.model.o = pyomo.Objective(expr=node.model.beta * pyomo.quicksum(ent.get_objective()
-                                                                                     for ent in entity.get_entities()))
+                node.model.o = pyomo.Objective(expr=node.model.beta * sum(ent.get_objective()
+                                                                          for ent in entity.get_entities()))
             else:
                 node.model.o = pyomo.Objective(expr=0)
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -36,16 +36,16 @@
 from pycity_scheduling.classes.apartment import Apartment
 from pycity_scheduling.classes.battery import Battery
 from pycity_scheduling.classes.boiler import Boiler
 from pycity_scheduling.classes.chiller import Chiller
 from pycity_scheduling.classes.combined_heat_power import CombinedHeatPower
 from pycity_scheduling.classes.curtailable_load import CurtailableLoad
 from pycity_scheduling.classes.deferrable_load import DeferrableLoad
-from pycity_scheduling.classes.electrical_heater import ElectricalHeater
-from pycity_scheduling.classes.electrical_vehicle import ElectricalVehicle
+from pycity_scheduling.classes.electric_heater import ElectricHeater
+from pycity_scheduling.classes.electric_vehicle import ElectricVehicle
 from pycity_scheduling.classes.fixed_load import FixedLoad
 from pycity_scheduling.classes.heat_pump import HeatPump
 from pycity_scheduling.classes.photovoltaic import Photovoltaic
 from pycity_scheduling.classes.space_cooling import SpaceCooling
 from pycity_scheduling.classes.space_heating import SpaceHeating
 from pycity_scheduling.classes.thermal_heating_storage import ThermalHeatingStorage
 from pycity_scheduling.classes.thermal_cooling_storage import ThermalCoolingStorage
@@ -67,16 +67,16 @@
     'Apartment',
     'Battery',
     'Boiler',
     'Chiller',
     'CombinedHeatPower',
     'CurtailableLoad',
     'DeferrableLoad',
-    'ElectricalHeater',
-    'ElectricalVehicle',
+    'ElectricHeater',
+    'ElectricVehicle',
     'FixedLoad',
     'HeatPump',
     'Photovoltaic',
     'SpaceCooling',
     'SpaceHeating',
     'ThermalHeatingStorage',
     'ThermalCoolingStorage',
@@ -101,41 +101,41 @@
     'AP': Apartment,
     'BAT': Battery,
     'BL': Boiler,
     'CH': Chiller,
     'CHP': CombinedHeatPower,
     'CL': CurtailableLoad,
     'DL': DeferrableLoad,
-    'EH': ElectricalHeater,
-    'EV': ElectricalVehicle,
+    'EH': ElectricHeater,
+    'EV': ElectricVehicle,
     'FL': FixedLoad,
     'HP': HeatPump,
     'PV': Photovoltaic,
     'SC': SpaceCooling,
     'SH': SpaceHeating,
     'THS': ThermalHeatingStorage,
     'TCS': ThermalCoolingStorage,
     'WEC': WindEnergyConverter,
 }
 
 heating_devices = {
     'HP': HeatPump,
     'BL': Boiler,
     'CHP': CombinedHeatPower,
-    'EH': ElectricalHeater,
+    'EH': ElectricHeater,
 }
 
 cooling_devices = {
     'CH': Chiller,
 }
 
 consumption_devices = {
     'CL': CurtailableLoad,
     'DL': DeferrableLoad,
-    'EV': ElectricalVehicle,
+    'EV': ElectricVehicle,
     'FL': FixedLoad,
 }
 
 generation_devices = {
     'CHP': CombinedHeatPower,
     'PV': Photovoltaic,
     'WEC': WindEnergyConverter,
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/apartment.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/apartment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/battery.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/battery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -44,16 +44,16 @@
     p_el_max_charge : float
         Maximum charging power [kW].
     p_el_max_discharge : float, optional
         Maximum discharging power [kW]. Defaults to zero.
     soc_init : float, optional
         Initial state of charge. Defaults to 50%.
     eta : float, optional
-        Charging and discharging efficiency. Must be in (0,1]. Defaults
-        to one.
+        Charging and discharging efficiency. Must be in (0,1].
+        Defaults to one.
     storage_end_equality : bool, optional
         `True` if the soc at the end of the scheduling has to be equal to
         the initial soc.
         `False` if it has to be greater or equal than the initial soc.
         Defaults to `False`.
 
     Notes
@@ -83,15 +83,15 @@
 
     .. math::
 
         p_{el\\_demand} &\\leq& p_{state} * p_{el\\_max\\_discharge} \\\\
         p_{el\\_supply} &\\leq& (1-p_{state}) * p_{el\\_max\\_charge}
     """
 
-    def __init__(self, environment, e_el_max, p_el_max_charge, p_el_max_discharge=None, soc_init=0.5, eta=1,
+    def __init__(self, environment, e_el_max, p_el_max_charge, p_el_max_discharge=None, soc_init=0.5, eta=0.95,
                  storage_end_equality=False):
 
         capacity = e_el_max * 3600 * 1000
         soc_abs = soc_init * capacity  # absolute SOC
         super().__init__(environment, soc_abs, capacity, 0.0, eta, eta)
         self._long_id = "BAT_" + self._id_string
 
@@ -137,37 +137,38 @@
             m.p_el_vars.setlb(None)
             m.p_el_demand_vars = pyomo.Var(m.t, domain=pyomo.Reals,
                                            bounds=(0.0, np.inf if mode == "integer" else self.p_el_max_charge),
                                            initialize=0)
             m.p_el_supply_vars = pyomo.Var(m.t, domain=pyomo.Reals,
                                            bounds=(0.0, np.inf if mode == "integer" else self.p_el_max_discharge),
                                            initialize=0)
-            m.e_el_vars = pyomo.Var(m.t, domain=pyomo.Reals, bounds=(0, self.e_el_max), initialize=0)
+            m.e_el_vars = pyomo.Var(m.t, domain=pyomo.Reals, bounds=(0, self.e_el_max),
+                                    initialize=self.e_el_max*self.soc_init)
 
             def p_rule(model, t):
                 return model.p_el_vars[t] == model.p_el_demand_vars[t] - model.p_el_supply_vars[t]
             m.p_constr = pyomo.Constraint(m.t, rule=p_rule)
             m.e_el_init = pyomo.Param(default=self.soc_init * self.e_el_max, mutable=True)
 
             def e_rule(model, t):
                 delta = (
                         (self.eta_charge * model.p_el_demand_vars[t]
                          - (1.0 / self.eta_discharge) * model.p_el_supply_vars[t])
                         * self.time_slot
                 )
-                e_el_last = model.e_el_vars[t - 1] if t >= 1 else model.e_el_init
+                e_el_last = model.e_el_vars[t-1] if t >= 1 else model.e_el_init
                 return model.e_el_vars[t] == e_el_last + delta
             m.e_constr = pyomo.Constraint(m.t, rule=e_rule)
 
-            def e_end_rule(model):
-                if self.storage_end_equality:
-                    return model.e_el_vars[self.op_horizon-1] == self.e_el_max * self.soc_init
-                else:
-                    return model.e_el_vars[self.op_horizon-1] >= self.e_el_max * self.soc_init
-            m.e_end_constr = pyomo.Constraint(rule=e_end_rule)
+            # Set bounds for the final storage capacity
+            if self.storage_end_equality:
+                m.e_el_vars[self.op_horizon-1].setlb(self.e_el_max * self.soc_init)
+                m.e_el_vars[self.op_horizon-1].setub(self.e_el_max * self.soc_init)
+            else:
+                m.e_el_vars[self.op_horizon-1].setlb(self.e_el_max * self.soc_init)
 
             if mode == "integer":
                 m.p_state_vars = pyomo.Var(m.t, domain=pyomo.Binary)
 
                 def c_rule(model, t):
                     return model.p_el_demand_vars[t] <= model.p_state_vars[t] * self.p_el_max_charge
                 m.p_charge_integer_constr = pyomo.Constraint(m.t, rule=c_rule)
@@ -185,9 +186,9 @@
     def update_model(self, mode=""):
         m = self.model
         timestep = self.timestep
 
         if timestep == 0:
             m.e_el_init = self.soc_init * self.e_el_max
         else:
-            m.e_el_init = self.e_el_schedule[timestep - 1]
+            m.e_el_init = self.e_el_schedule[timestep-1]
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/boiler.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/boiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -60,15 +60,15 @@
         0 \\geq p_{th\\_heat} \\geq -p_{th\\_nom}
 
     - See also:
         - pycity_scheduling.util.generic_constraints.LowerActivationLimit:
           Generates additional constraints for the `lower_activation_limit` in `integer` mode.
     """
 
-    def __init__(self, environment, p_th_nom, eta=1, lower_activation_limit=0):
+    def __init__(self, environment, p_th_nom, eta=1, lower_activation_limit=0.0):
         # Flow temperature of 55 C
         super().__init__(environment, 1000*p_th_nom, eta, 55, lower_activation_limit)
         self._long_id = "BL_" + self._id_string
         self.p_th_nom = p_th_nom
 
         self.activation_constr = LowerActivationLimit(self, "p_th_heat", lower_activation_limit, -p_th_nom)
 
@@ -115,8 +115,8 @@
             Coefficient for the objective function.
 
         Returns
         -------
         ExpressionBase :
             Objective function.
         """
-        return coeff * pyomo.sum_product(self.model.p_th_heat_vars)
+        return coeff * sum(self.model.p_th_heat_vars[t] for t in range(self.op_horizon))
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/building.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -42,14 +42,15 @@
         Objective for the scheduling. The default is 'price'.
 
         - 'price' : Optimize for the prices given by `prices.tou_prices`.
         - 'co2' : Optimize for the CO2 emissions given by `prices.co2_prices`.
         - 'peak-shaving' : Try to flatten the schedule as much as possible.
         - 'max-consumption' : Try to reduce the maximum of the absolute values of the schedule as much as possible.
         - 'self-consumption' : Try to maximize the self-consumption of the local power generation.
+        - 'least-squares': Try to `follow` a given reference power profile.
         - 'none' : No objective (leave all flexibility to other participants).
     name : str, optional
         Name for the building.
         If name is None, set it to self._long_id.
     profile_type : str, optional
         Thermal SLP profile name
         Requires `method=1`
@@ -71,14 +72,16 @@
     building_type : str, optional
         Build year profile name, the detailed list is implemented in
         `tabula_data.py`.
     storage_end_equality : bool, optional
         `True` if the soc at the end of the scheduling has to be equal to
         the initial soc.
         `False` if it has to be greater or equal than the initial soc.
+    least_squares_profile : numpy.ndarray, optional
+        Profile to be used by the least-squares objective.
 
     Notes
     -----
     - The exchange of thermal energy between different buildings is currently not supported.
       As a result, the building adds the following set of constrains additionally to the
       ones of the EntityContainer:
 
@@ -94,27 +97,28 @@
     - The :math:`E_{u\\_bound}` and :math:`E_{l\\_bound}` are determined by the
       robustness parameter, the available capacity of thermal heating storage, the magnitude of heating
       required by SpaceHeating and the magnitude of heating that can be produced by the building's heating units.
     """
 
     def __init__(self, environment, objective='price', name=None,
                  profile_type=None, building_type=None,
-                 storage_end_equality=False):
+                 storage_end_equality=False, least_squares_profile=None):
         super().__init__(environment)
 
         self._long_id = "BD_" + self._id_string
         if name is None:
             self.name = self._long_id
         else:
             self.name = name
 
         self.objective = objective
         self.profile_type = profile_type
         self.building_type = building_type
         self.storage_end_equality = storage_end_equality
+        self.least_squares_profile = least_squares_profile
 
     def populate_model(self, model, mode="convex", robustness=None):
         """
         Add building block to pyomo ConcreteModel.
 
         Call parent's `populate_model` method and set variables lower
         bounds to `None`. Then call `populate_model` method of the BES
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/building_energy_system.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/building_energy_system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -95,35 +95,35 @@
 
         Parameters
         ----------
         all_devices : boolean, optional
             If true: Return all installed devices
             If false: Only return the specified devices
         battery : boolean, optional
-            Return information on the battery
+            Return information about the battery unit
         boiler : boolean, optional
-            Return information on the boiler
+            Return information about the boiler unit
         chp : boolean, optional
-            Return information on the chp unit
+            Return information about the chp unit
         chiller : boolean, optional
-            Return information on the chiller unit
+            Return information about the chiller unit
         electrical_heater : boolean, optional
-            Return information on the electrical heater
+            Return information about the electric heater unit
         heatpump : boolean, optional
-            Return information on the heat pump
+            Return information about the heat pump unit
         inverter_acdc : boolean, optional
-            Return information on the AC-DC inverter
+            Return information about the AC-DC inverter unit
         inverter_dcac : boolean, optional
-            Return information on the DC-AC inverter
+            Return information about the DC-AC inverter unit
         pv : boolean, optional
-            Return information on the PV modules
+            Return information about the PV unit
         ths : boolean, optional
-            Return information on the thermal heating storage
+            Return information about the thermal heating storage unit
         tcs : boolean, optional
-            Return information on the thermal cooling storage
+            Return information about the thermal cooling storage unit
         """
         result = super().getHasDevices(all_devices=all_devices,
                                        battery=battery,
                                        boiler=boiler,
                                        chp=chp,
                                        compression_chiller=chiller,
                                        electrical_heater=electrical_heater,
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/chiller.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/chiller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/city_district.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/city_district.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -38,32 +38,36 @@
     environment : Environment
     objective : str, optional
         Objective for the district operator. Default is 'price'.
 
         - 'price' : Optimize for the minimum total cost given by `prices.da_prices`.
         - 'peak-shaving' : Try to 'flatten' the schedule as much as possible.
         - 'co2' : Optimize for the minimum total co2 emissions given by `prices.co2_prices`.
-        - 'valley-filling' : Try to fill the 'valleys' given by a reference power profile.
+        - 'valley-filling' : Try to fill the 'valleys' given by `self.valley_profile`.
         - 'max-consumption' : Try to minimize the maximum power subscription.
         - 'self-consumption' : Try to maximize the self-consumption of the local power generation.
+        - 'least-squares': Try to `follow` a given reference power profile.
         - 'flexibility-quantification' : To be used to quantify the flexibility potential of the city district only.
         - 'none' : No objective.
     valley_profile : numpy.ndarray, optional
         Profile to be filled by applying the valley filling objective.
+    least_squares_profile : numpy.ndarray, optional
+        Profile to be used by the least-squares objective.
 
     Notes
     -----
     - The constraints generated by a CD are the same as the ones created by an EntityContainer.
     """
 
-    def __init__(self, environment, objective='price', valley_profile=None):
+    def __init__(self, environment, objective='price', valley_profile=None, least_squares_profile=None):
         super().__init__(environment)
         self._long_id = "CD_" + self._id_string
         self.objective = objective
         self.valley_profile = valley_profile
+        self.least_squares_profile = least_squares_profile
 
     def populate_model(self, model, mode="convex"):
         """
         Add city district block to pyomo ConcreteModel.
 
         Call parent's `populate_model` methods and set variables lower
         bounds to `None`.
@@ -75,35 +79,40 @@
             Specifies which set of constraints to use.
 
             - `convex`  : Use linear constraints
             - `integer`  : Use same constraints as convex mode
         """
         super().populate_model(model, mode)
         m = self.model
-
+        
         if mode in ["convex", "integer"]:
             m.p_el_vars.setlb(None)
         else:
             raise ValueError(
                 "Mode %s is not implemented by city district." % str(mode)
             )
         return
 
     def get_objective(self, coeff=1):
         if self.objective == 'valley-filling':
-            e = coeff * pyomo.sum_product(self.model.p_el_vars, self.model.p_el_vars)
+            obj = 0
             valley = self.valley_profile[self.op_slice]
-            e += 2 * coeff * pyomo.sum_product(valley, self.model.p_el_vars)
-            return e
+            for t in range(self.op_horizon):
+                obj += coeff * self.model.p_el_vars[t] * self.model.p_el_vars[t]
+                obj += 2 * coeff * valley[t] * self.model.p_el_vars[t]
+            return obj
         elif self.objective == 'price':
             prices = self.environment.prices.da_prices[self.op_slice]
             s = sum(abs(prices))
             if s > 0:
+                obj = 0
                 prices = prices * self.op_horizon / s
-                return pyomo.sum_product(prices, self.model.p_el_vars)
+                for t in range(self.op_horizon):
+                    obj += prices[t] * self.model.p_el_vars[t]
+                return obj
             else:
                 return 0
         else:
             return super().get_objective(coeff)
 
     def get_lower_entities(self):
         for node in self.nodes.values():
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/combined_heat_power.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/combined_heat_power.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -65,15 +65,15 @@
         \\frac{p_{el}}{p_{el\\_nom}} &=& \\frac{p_{th\\_heat}}{p_{th\\_nom}}
 
     - See also:
         - pycity_scheduling.util.generic_constraints.LowerActivationLimit:
           Generates additional constraints for the `lower_activation_limit` in `integer` mode.
     """
 
-    def __init__(self, environment, p_th_nom, p_el_nom=None, eta=1, lower_activation_limit=0):
+    def __init__(self, environment, p_th_nom, p_el_nom=None, eta=1, lower_activation_limit=0.6):
         q_nominal = p_th_nom * 1000
         if p_el_nom is None:
             p_nominal = q_nominal
             self.p_el_nom = p_th_nom
         else:
             p_nominal = p_el_nom * 1000
             self.p_el_nom = p_el_nom
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/curtailable_load.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/curtailable_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/deferrable_load.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/deferrable_load.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -150,15 +150,16 @@
                     ("DeferrableLoad {} is not able to consume enough power in the given op_horizon," +
                      "which will render the model infeasible")
                     .format(self._long_id)
                 )
 
             # consume e_consumption the op_horizon
             def p_consumption_rule(model):
-                return pyomo.sum_product(model.p_el_vars) * self.time_slot == self.e_consumption
+                return sum(model.p_el_vars[t] for t in range(len(model.p_el_vars))) * self.time_slot == \
+                       self.e_consumption
             m.P_consumption_constr = pyomo.Constraint(rule=p_consumption_rule)
 
         elif mode == "integer":
             self.runtime = self.e_consumption / (self.p_el_nom * self.time_slot)
             rounded_runtime = int(round(self.runtime))
             if not np.isclose(self.runtime, rounded_runtime):
                 warn("Consumption of DLs is in integer mode always a multiple of " +
@@ -175,22 +176,25 @@
             # create binary variables representing if operation begins in timeslot t
             # Since the DL has to finish operation when the op_horizon ends, binary variables representing a too late
             # start can be omitted.
             m.p_start_vars = pyomo.Var(pyomo.RangeSet(0, self.op_horizon-self.runtime), domain=pyomo.Binary)
 
             # coupling the start variable to the electrical variables following
             def state_coupl_rule(model, t):
-                return model.p_el_vars[t] == self.p_el_nom * pyomo.quicksum(
-                       (model.p_start_vars[t] for t in range(max(0, t+1-self.runtime),
-                                                             min(self.op_horizon-self.runtime+1, t+1))))
+                return model.p_el_vars[t] == self.p_el_nom * sum(
+                       (model.p_start_vars[tau] for tau in range(max(0, t+1-self.runtime),
+                                                                 min(self.op_horizon-self.runtime+1, t+1))))
             m.state_coupl_integer_constr = pyomo.Constraint(m.t, rule=state_coupl_rule)
 
             # run once in the op_horizon
             def state_once_rule(model):
-                return pyomo.sum_product(model.p_start_vars) == 1.0
+                if len(model.p_start_vars) > 0:
+                    return sum(model.p_start_vars[t] for t in range(len(model.p_start_vars))) == 1.0
+                else:
+                    return pyomo.sum_product(model.p_start_vars) == 1.0
             m.state_once_integer_constr = pyomo.Constraint(rule=state_once_rule)
 
         else:
             raise ValueError(
                 "Mode %s is not implemented by class DeferrableLoad." % str(mode)
             )
         return
@@ -247,10 +251,12 @@
         -------
         ExpressionBase :
             Objective function.
         """
         m = self.model
         max_loading_time = sum(self.load_time) * self.time_slot
         optimal_p_el = self.e_consumption / max_loading_time
-        obj = coeff * pyomo.sum_product(m.p_el_vars, m.p_el_vars)
-        obj += -2 * coeff * optimal_p_el * pyomo.sum_product(m.p_el_vars)
+        obj = 0
+        for t in range(self.op_horizon):
+            obj += coeff * m.p_el_vars[t] * m.p_el_vars[t]
+        obj -= 2 * coeff * optimal_p_el * sum(m.p_el_vars[t] for t in range(self.op_horizon))
         return obj
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/electrical_entity.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electrical_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -97,39 +97,57 @@
                 m.max_p_flex_gen_constr = pyomo.Constraint(m.t, rule=max_p_flex_generation_rule)
         else:
             raise ValueError("Mode %s is not implemented by electrical entity." % str(mode))
         return
 
     def get_objective(self, coeff=1):
         if self.objective == 'peak-shaving':
-            return coeff * pyomo.sum_product(self.model.p_el_vars, self.model.p_el_vars)
+            obj = 0
+            for t in range(self.op_horizon):
+                obj += self.model.p_el_vars[t] * self.model.p_el_vars[t]
+            return coeff * obj
         if self.objective in ['price', 'co2']:
             if self.objective == 'price':
                 prices = self.environment.prices.tou_prices
             else:
                 prices = self.environment.prices.co2_prices
             prices = prices[self.op_slice]
             s = sum(abs(prices))
             if s > 0:
                 prices = prices * self.op_horizon / s
-                return coeff * pyomo.sum_product(prices, self.model.p_el_vars)
+                obj = 0
+                for t in range(self.op_horizon):
+                    obj += prices[t] * self.model.p_el_vars[t]
+                return coeff * obj
             else:
                 return 0
         if self.objective == "max-consumption":
             if not hasattr(self.model, "max_consumption_var"):
                 raise ValueError("Objective 'max-consumption' needs to be selected during populate_model call.")
             if coeff < 0:
                 raise ValueError("Setting a coefficient below zero is not supported for the max-consumption objective.")
             return coeff * self.model.max_consumption_var
         if self.objective == "self-consumption":
             if not hasattr(self.model, "p_export_var"):
                 raise ValueError("'Objective self-consumption' needs to be selected during populate_model call.")
             if coeff < 0:
                 raise ValueError("Setting a coefficient below zero is not supported for the self-consumption "
                                  "objective.")
-            return coeff * pyomo.sum_product(self.model.p_export_var, self.model.p_export_var)
+            obj = 0
+            for t in range(self.op_horizon):
+                obj += self.model.p_export_var[t] * self.model.p_export_var[t]
+            return coeff * obj
+        if self.objective == 'least-squares':
+            obj = 0
+            for t in range(self.op_horizon):
+                obj += (self.model.p_el_vars[t] - self.least_squares_profile[t]) * \
+                       (self.model.p_el_vars[t] - self.least_squares_profile[t])
+            return coeff * obj
         if self.objective == 'flexibility-quantification':
             if not hasattr(self.model, "max_p_flex_var"):
                 raise ValueError("Objective 'flexibility-quantification' needs to be selected during populate_model "
                                  "call.")
-            return coeff * pyomo.sum_product(self.model.max_p_flex_var, self.model.max_p_flex_var)
+            obj = 0
+            for t in range(self.op_horizon):
+                obj += self.model.max_p_flex_var[t] * self.model.max_p_flex_var[t]
+            return coeff * obj
         return super().get_objective(coeff)
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/electrical_heater.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_heater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -27,29 +27,29 @@
 import pycity_base.classes.supply.electrical_heater as eh
 
 from pycity_scheduling.util.generic_constraints import LowerActivationLimit
 from pycity_scheduling.classes.thermal_entity_heating import ThermalEntityHeating
 from pycity_scheduling.classes.electrical_entity import ElectricalEntity
 
 
-class ElectricalHeater(ThermalEntityHeating, ElectricalEntity, eh.ElectricalHeater):
+class ElectricHeater(ThermalEntityHeating, ElectricalEntity, eh.ElectricalHeater):
     """
     Extension of pyCity_base class ElectricalHeater for scheduling purposes.
 
     Parameters
     ----------
     environment : pycity_scheduling.classes.Environment
         Common to all other objects. Includes time and weather instances.
     p_th_nom : float
         Nominal thermal power output in [kW].
     eta : float, optional
-        Efficiency of the electrical heater. Defaults to one.
+        Efficiency of the electric heater. Defaults to one.
     lower_activation_limit : float, optional (only adhered to in integer mode)
-        Must be in [0, 1]. Lower activation limit of the electrical heater
-        as a percentage of the rated power. When the electrical heater is
+        Must be in [0, 1]. Lower activation limit of the electric heater
+        as a percentage of the rated power. When the electric heater is
         in operation, its power must be zero or between the lower activation
         limit and its rated power.
 
         - `lower_activation_limit = 0`: Linear behavior
         - `lower_activation_limit = 1`: Two-point controlled
 
     Notes
@@ -62,15 +62,15 @@
         \\eta * p_{el} &=& - p_{th\\_heat}
 
     - See also:
         - pycity_scheduling.util.generic_constraints.LowerActivationLimit: Generates additional constraints for the
           `lower_activation_limit` in `integer` mode.
     """
 
-    def __init__(self, environment, p_th_nom, eta=1, lower_activation_limit=0):
+    def __init__(self, environment, p_th_nom, eta=1, lower_activation_limit=0.25):
         # Flow temperature of 55 C
         super().__init__(environment, p_th_nom*1000, eta, 85, lower_activation_limit)
         self._long_id = "EH_" + self._id_string
         self.p_th_nom = p_th_nom
         self.activation_constr = LowerActivationLimit(self, "p_th_heat", lower_activation_limit, -p_th_nom)
 
     def populate_model(self, model, mode="convex"):
@@ -101,10 +101,10 @@
                 return - model.p_th_heat_vars[t] == self.eta * model.p_el_vars[t]
             m.p_coupl_constr = pyomo.Constraint(m.t, rule=p_coupl_rule)
 
             self.activation_constr.apply(m, mode)
 
         else:
             raise ValueError(
-                "Mode %s is not implemented by class ElectricalHeater." % str(mode)
+                "Mode %s is not implemented by class ElectricHeater." % str(mode)
             )
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/electrical_vehicle.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/electric_vehicle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -26,45 +26,56 @@
 import pyomo.environ as pyomo
 from warnings import warn
 
 from pycity_scheduling.classes.battery import Battery
 from pycity_scheduling import util
 
 
-class ElectricalVehicle(Battery):
+class ElectricVehicle(Battery):
     """
-    Class representing an electrical vehicle for scheduling purposes.
+    Class representing an electric vehicle for scheduling purposes.
 
     Parameters
     ----------
     environment : Environment
         Common Environment instance.
     e_el_max : float
         Electric capacity of the battery in [kWh].
     p_el_max_charge : float
         Maximum charging power in [kW].
     p_el_max_discharge : float, optional
         Maximum discharging power in [kW]. Defaults to zero.
     soc_init : float, optional
         Initial state of charge. Defaults to 50%.
     charging_time : array of binaries, optional
-        Indicator when electrical vehicle can be charged.
+        Indicator when electric vehicle can be charged.
 
         - `charging_time[t] == 0`: EV cannot be charged in t
         - `charging_time[t] == 1`: EV can be charged in t
 
         It must contain at least one `0` otherwise the model will become
         infeasible. Its length has to be consistent with `ct_pattern`.
         Defaults to only charge during night.
     ct_pattern : str, optional
         Define how the `charging_time` profile is to be used.
 
         - `None` : Profile matches simulation horizon (default).
         - 'daily' : Profile matches one day.
         - 'weekly' : Profile matches one week.
+    simulate_driving : bool, optional
+        Simulate driving.
+
+        - `True`: EV may drive and lose energy during the trip
+        - `False`: EV cannot drive and lose energy during the trip
+    minimum_soc_end : float, optional
+        Set the minimum state of charge for an EV at the end of the optimization horizon. Must be in (0,1].
+        Defaults to 80%.
+    eta : float, optional
+        Charging and discharging efficiency of the EV. Must be in (0,1].
+        Defaults to 100%.
 
     Notes
     -----
     - EVs offer sets of constraints for operation. The :math:`e_{el}` equivalence
       constraint is replaced by the following constraint:
 
     .. math::
@@ -84,22 +95,24 @@
 
     - The constraint for the parameter `storage_end_equality` is removed. Instead,
       the EV needs to be fully charged at the end of the `simu_horizon` if parameter `ct_pattern`
       is one at the end of the simulation horizon.
     """
 
     def __init__(self, environment, e_el_max, p_el_max_charge, p_el_max_discharge=0.0,
-                 soc_init=0.5, charging_time=None, ct_pattern=None):
-        super().__init__(environment, e_el_max, p_el_max_charge, p_el_max_discharge, soc_init, eta=1,
+                 soc_init=0.5, charging_time=None, ct_pattern=None, simulate_driving=False, minimum_soc_end=0.8,
+                 eta=1.0):
+        super().__init__(environment, e_el_max, p_el_max_charge, p_el_max_discharge, soc_init, eta,
                          storage_end_equality=False)
-        self._kind = "electricalvehicle"
+        self._kind = "electricvehicle"
         self._long_id = "EV_" + self._id_string
-
         self.charging_time_initial = charging_time
         self.ct_pattern = ct_pattern
+        self.simulate_driving = simulate_driving
+        self.minimum_soc_end = minimum_soc_end
 
         if charging_time is None:
             # load at night, drive during day
             ts_per_day = int(24 / self.time_slot)
             a = int(ts_per_day / 4)
             b = int(ts_per_day / 2)
             c = ts_per_day - a - b
@@ -115,29 +128,31 @@
         self.charging_durations = self.stopping_timesteps - self.starting_timesteps
         # Links charging periods to indices in previous arrays.
         self.charging_indices = np.zeros_like(charging_time, dtype=np.int)
         for i, start in enumerate(self.starting_timesteps):
             self.charging_indices[start:start + self.charging_durations[i]] = np.full(self.charging_durations[i], i)
 
         # Contains the amount of energy to charge in charging periods.
-        self.required_charges = np.full_like(self.charging_durations, 0.8 * e_el_max, dtype=np.float)
+        self.required_charges = np.full_like(self.charging_durations, self.minimum_soc_end * e_el_max, dtype=np.float)
 
         if len(self.charging_time) > 0:
-            # In first charging cycle the required charge is determined by soc_init and is not necessarily 80%.
-            self.required_charges[0] = (1 - soc_init) * e_el_max
+            # In first charging cycle the required charge is determined by the difference between soc_init and
+            # minimum_soc_end.
+            self.required_charges[0] = (1 - (minimum_soc_end - soc_init)) * e_el_max
 
             if self.charging_time[-1]:
-                # Limit charge at end of simu horizon to not become infeasible.
+                # Limit charge at end of simulation horizon to not become infeasible.
                 self.required_charges[-1] = min(self.required_charges[-1], self.charging_durations[-1] *
                                                 self.time_slot * p_el_max_charge * self.eta_charge)
 
-        if any(self.required_charges > self.charging_durations * self.time_slot * p_el_max_charge * self.eta_charge):
+        if any(self.required_charges > self.charging_durations * self.time_slot * p_el_max_charge *
+               self.eta_charge):
             warn("Charging pattern results in infeasible constraints.")
-
-        self.new_var("p_el_drive")
+        if self.simulate_driving:
+            self.new_var("p_el_drive")
 
     def populate_model(self, model, mode="convex"):
         """
         Add device block to pyomo ConcreteModel
 
         Call parent's `populate_model` method. Replace coupling
         constraints from Battery class with coupling constraints
@@ -152,86 +167,85 @@
             - `convex`  : Use linear constraints
             - `integer`  : Use integer variables representing discrete control decisions
         """
         super().populate_model(model, mode)
         m = self.model
 
         if mode == "convex" or "integer":
-            # Simulate power consumption while driving
-            m.p_el_drive_vars = pyomo.Var(m.t, domain=pyomo.Reals, bounds=(0, None), initialize=0)
-
             # Replace coupling constraints from Battery class
             m.del_component("e_constr")
-            m.del_component("e_end_constr")
+
+            # Simulate power consumption while driving
+            if self.simulate_driving:
+                m.p_el_drive_vars = pyomo.Var(m.t, domain=pyomo.Reals, bounds=(0, None), initialize=0)
+
+            # Reset e_el bounds
+            for t in self.op_time_vec:
+                m.e_el_vars[t].setub(self.e_el_max)
+                m.e_el_vars[t].setlb(self.soc_init * self.e_el_max)
+            m.e_el_vars[self.op_horizon-1].setlb(self.minimum_soc_end * self.e_el_max)
 
             def e_rule(model, t):
-                delta = (
-                    (self.eta_charge * model.p_el_demand_vars[t]
-                     - (1.0 / self.eta_discharge) * model.p_el_supply_vars[t]
-                     - model.p_el_drive_vars[t])
-                    * self.time_slot
-                )
-                e_el_last = model.e_el_vars[t - 1] if t >= 1 else model.e_el_init
+                if self.simulate_driving:
+                    delta = (
+                        (self.eta_charge * model.p_el_demand_vars[t]
+                         - (1.0 / self.eta_discharge) * model.p_el_supply_vars[t]
+                         - model.p_el_drive_vars[t])
+                        * self.time_slot
+                    )
+                else:
+                    delta = (
+                        (self.eta_charge * model.p_el_demand_vars[t]
+                         - (1.0 / self.eta_discharge) * model.p_el_supply_vars[t])
+                        * self.time_slot
+                    )
+                e_el_last = model.e_el_vars[t-1] if t >= 1 else model.e_el_init
                 return model.e_el_vars[t] == e_el_last + delta
             m.e_constr = pyomo.Constraint(m.t, rule=e_rule)
         else:
             raise ValueError(
-                "Mode %s is not implemented by class ElectricalVehicle." % str(mode)
+                "Mode %s is not implemented by class ElectricVehicle." % str(mode)
             )
         return
 
     def update_model(self, mode=""):
         m = self.model
 
         super().update_model(mode)
 
         timestep = self.timestep
         charging_time = self.charging_time[self.op_slice]
         # Is true if t is before the initial charging period.
         is_initial = not any(self.charging_time[:timestep])
 
-        # Reset e_el bounds
-        for t in self.op_time_vec:
-            m.e_el_vars[t].setub(self.e_el_max)
-            m.e_el_vars[t].setlb(0.0)
-
         for t in self.op_time_vec:
             if charging_time[t]:
                 m.p_el_demand_vars[t].setub(self.p_el_max_charge)
-                m.p_el_supply_vars[t].setub(self.p_el_max_discharge)
-                m.p_el_drive_vars[t].setub(0.0)
+                if self.simulate_driving:
+                    m.p_el_supply_vars[t].setub(self.p_el_max_discharge)
+                    m.p_el_drive_vars[t].setub(0.0)
+                else:
+                    m.p_el_supply_vars[t].setub(0.0)
                 is_initial = False
             else:
                 m.p_el_demand_vars[t].setub(0.0)
                 m.p_el_supply_vars[t].setub(0.0)
-                m.p_el_drive_vars[t].setub(None)
+                if self.simulate_driving:
+                    m.p_el_drive_vars[t].setub(None)
 
                 if is_initial:
                     # Remain at soc_init before the first charging period is reached.
                     m.e_el_vars[t].setub(self.soc_init * self.e_el_max)
                     m.e_el_vars[t].setlb(self.soc_init * self.e_el_max)
-                else:
-                    m.e_el_vars[t].setub(0.2 * self.e_el_max)
-                    m.e_el_vars[t].setlb(0.2 * self.e_el_max)
 
             if t + 1 < self.op_horizon:
                 if charging_time[t] and not charging_time[t+1]:
-                    # Full battery at end of charging period
+                    # SOC at the end of the optimization horizon:
                     m.e_el_vars[t].setub(self.e_el_max)
-                    m.e_el_vars[t].setlb(self.e_el_max)
-
-        if charging_time[-1]:
-            current_ts = (timestep + self.op_horizon - 1) % int(24 / self.time_slot)
-            i = self.charging_indices[current_ts]
-
-            first_ts = self.starting_timesteps[i]
-            portion_charge = (current_ts - first_ts + 1) * self.required_charges[i] / self.charging_durations[i]
-            starting_charge = 0.2 * self.e_el_max if i != 0 else self.soc_init * self.e_el_max
-            m.e_el_vars[self.op_horizon-1].setub(starting_charge + portion_charge)
-            m.e_el_vars[self.op_horizon-1].setlb(starting_charge + portion_charge)
+                    m.e_el_vars[t].setlb(self.minimum_soc_end * self.e_el_max)
         return
 
     def get_objective(self, coeff=1):
         """
         Objective function for entity level scheduling.
 
         Return the objective function of the electric vehicle weighted with
@@ -247,8 +261,11 @@
         -------
         ExpressionBase :
             Objective function.
         """
         m = self.model
         c = np.array(list(map(lambda x: x+1, range(self.op_horizon))))
         c = c * (coeff * self.op_horizon / sum(c))
-        return pyomo.sum_product(c, m.p_el_vars, m.p_el_vars)
+        obj = 0
+        for t in range(self.op_horizon):
+            obj += c[t] * m.p_el_vars[t] * m.p_el_vars[t]
+        return obj
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/entity_container.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/entity_container.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -87,25 +87,32 @@
                     p_el_var_list.append(entity.model.p_el_vars)
 
             m.p_th_cool_vars.setlb(None)
             m.p_th_heat_vars.setlb(None)
             m.p_el_vars.setlb(None)
 
             def p_th_cool_sum_rule(model, t):
-                return model.p_th_cool_vars[t] == pyomo.quicksum(p_th_Cool_var[t] for
-                                                                 p_th_Cool_var in p_th_cool_var_list)
+                if len(p_th_cool_var_list) > 0:
+                    return model.p_th_cool_vars[t] == sum(p_th_Cool_var[t] for p_th_Cool_var in p_th_cool_var_list)
+                else:
+                    return model.p_th_cool_vars[t] == 0.0
             m.p_th_cool_constr = pyomo.Constraint(m.t, rule=p_th_cool_sum_rule)
 
             def p_th_heat_sum_rule(model, t):
-                return model.p_th_heat_vars[t] == pyomo.quicksum(p_th_Heat_var[t] for
-                                                                 p_th_Heat_var in p_th_heat_var_list)
+                if len(p_th_heat_var_list) > 0:
+                    return model.p_th_heat_vars[t] == sum(p_th_Heat_var[t] for p_th_Heat_var in p_th_heat_var_list)
+                else:
+                    return model.p_th_heat_vars[t] == 0.0
             m.p_th_heat_constr = pyomo.Constraint(m.t, rule=p_th_heat_sum_rule)
 
             def p_el_sum_rule(model, t):
-                return model.p_el_vars[t] == pyomo.quicksum(p_el_var[t] for p_el_var in p_el_var_list)
+                if len(p_el_var_list) > 0:
+                    return model.p_el_vars[t] == sum(p_el_var[t] for p_el_var in p_el_var_list)
+                else:
+                    return model.p_el_vars[t] == 0.0
             m.p_el_constr = pyomo.Constraint(m.t, rule=p_el_sum_rule)
         else:
             raise ValueError(
                 "Mode %s is not implemented by class EntityContainer." % str(mode)
             )
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/environment.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/fixed_load.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/fixed_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/heat_pump.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/heat_pump.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -78,15 +78,15 @@
 
     - See also:
         - pycity_scheduling.util.generic_constraints.LowerActivationLimit:
           Generates additional constraints for the `lower_activation_limit` in `integer` mode.
     """
 
     def __init__(self, environment, p_th_nom, cop=None, eta=0.36, t_max=55.0,
-                 lower_activation_limit=0, t_flow=55.0):
+                 lower_activation_limit=0.4, t_flow=55.0):
         simu_horizon = environment.timer.simu_horizon
 
         (t_ambient,) = environment.weather.getWeatherForecast(getTAmbient=True)
         ts = environment.timer.time_in_year()
         t_ambient = t_ambient[ts:ts + simu_horizon]
         if cop is None:
             cop = eta * np.true_divide((t_flow + 273.15), (t_flow - t_ambient))
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/optimization_entity.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/optimization_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/photovoltaic.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/photovoltaic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -135,10 +135,12 @@
         Returns
         -------
         ExpressionBase :
             Objective function.
         """
         m = self.model
 
-        s = pyomo.sum_product(m.p_el_vars, m.p_el_vars)
-        s += -2 * pyomo.sum_product(self.p_el_supply[self.op_slice], m.p_el_vars)
+        s = 0
+        for t in self.op_time_vec:
+            s += m.p_el_vars[t] * m.p_el_vars[t]
+            s -= 2 * self.p_el_supply[self.op_slice][t] * m.p_el_vars[t]
         return coeff * s
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/prices.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/space_cooling.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_cooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/space_heating.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/space_heating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_cooling_storage.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_cooling_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -104,30 +104,29 @@
         m = self.model
 
         if mode == "convex" or "integer":
             m.p_th_cool_vars.setlb(None)
 
             m.e_th_cool_vars = pyomo.Var(m.t, domain=pyomo.Reals, bounds=(0, self.e_th_max), initialize=0)
 
-            m.e_th_ini = pyomo.Param(default=self.soc_init * self.e_th_max, mutable=True)
+            m.e_th_init = pyomo.Param(default=self.soc_init * self.e_th_max, mutable=True)
 
             def e_rule(model, t):
-                e_th_last = model.e_th_cool_vars[t - 1] if t >= 1 else model.e_th_ini
+                e_th_last = model.e_th_cool_vars[t - 1] if t >= 1 else model.e_th_init
                 return model.e_th_cool_vars[t] == e_th_last * (1 - self.th_loss_coeff) + \
                        m.p_th_cool_vars[t] * self.time_slot
             m.e_constr = pyomo.Constraint(m.t, rule=e_rule)
 
-            def e_end_rule(model):
-                if self.storage_end_equality:
-                    return model.e_th_cool_vars[self.op_horizon-1] == self.e_th_max * self.soc_init
-                else:
-                    return model.e_th_cool_vars[self.op_horizon-1] >= self.e_th_max * self.soc_init
-            m.e_end_constr = pyomo.Constraint(rule=e_end_rule)
+            # Set bounds for the final storage capacity
+            if self.storage_end_equality:
+                model.e_th_cool_vars[self.op_horizon-1].setlb(self.e_th_max * self.soc_init)
+                model.e_th_cool_vars[self.op_horizon-1].setub(self.e_th_max * self.soc_init)
+            else:
+                m.e_th_cool_vars[self.op_horizon - 1].setlb(self.e_th_max * self.soc_init)
 
-            return
         else:
             raise ValueError(
                 "Mode %s is not implemented by class ThermalCoolingStorage." % str(mode)
             )
 
     def update_model(self, mode=""):
         m = self.model
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_entity_cooling.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_cooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_entity_heating.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_entity_heating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/thermal_heating_storage.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/thermal_heating_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -101,22 +101,22 @@
             - `integer` : Use same constraints as convex mode
         """
         super().populate_model(model, mode)
         m = self.model
 
         if mode == "convex" or "integer":
             m.p_th_heat_vars.setlb(None)
+            m.e_th_heat_vars = pyomo.Var(m.t, domain=pyomo.Reals, bounds=(0, self.e_th_max),
+                                         initialize=self.e_th_max*self.soc_init)
 
-            m.e_th_heat_vars = pyomo.Var(m.t, domain=pyomo.Reals, bounds=(0, self.e_th_max), initialize=0)
-
-            m.e_th_ini = pyomo.Param(default=self.soc_init * self.e_th_max, mutable=True)
+            m.e_th_init = pyomo.Param(default=self.soc_init * self.e_th_max, mutable=True)
 
             def e_rule(model, t):
-                e_th_last = model.e_th_heat_vars[t - 1] if t >= 1 else model.e_th_ini
-                return model.e_th_heat_vars[t] == e_th_last * (1 - self.th_loss_coeff) + \
+                e_th_last = model.e_th_heat_vars[t-1] if t >= 1 else model.e_th_init
+                return model.e_th_heat_vars[t] == e_th_last * (1.0 - self.th_loss_coeff) + \
                        m.p_th_heat_vars[t] * self.time_slot
             m.e_constr = pyomo.Constraint(m.t, rule=e_rule)
 
             def e_end_rule(model):
                 if self.storage_end_equality:
                     return model.e_th_heat_vars[self.op_horizon-1] == self.e_th_max * self.soc_init
                 else:
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/timer.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/weather.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/weather.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/classes/wind_energy_converter.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/classes/wind_energy_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -108,10 +108,12 @@
         Returns
         -------
         ExpressionBase :
             Objective function.
         """
         m = self.model
 
-        s = pyomo.sum_product(m.p_el_vars, m.p_el_vars)
-        s += -2 * pyomo.sum_product(self.p_el_supply[self.op_slice], m.p_el_vars)
+        s = 0
+        for t in self.op_time_vec:
+            s += m.p_el_vars[t] * m.p_el_vars[t]
+            s -= 2 * self.p_el_supply[self.op_slice][t] * m.p_el_vars[t]
         return coeff * s
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/constants.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/data/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt` & `pycity_scheduling-1.2.0/src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt` & `pycity_scheduling-1.2.0/src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt`

 * *Files identical despite different names*

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/data/tabula_data.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/data/tabula_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_00_fundamentals.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_00_fundamentals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -34,15 +34,14 @@
 
 
 def main(do_plot=False):
     print("\n\n------ Example 00: Fundamentals ------\n\n")
 
     # 1) Environment objects:
 
-
     # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
     # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
     # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
 
     # Generate a timer object for the environment:
     timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
 
@@ -51,15 +50,14 @@
 
     # Generate a price object for the environment:
     price = Prices(timer=timer)
 
     # Generate the environment object:
     environment = Environment(timer=timer, weather=weather, prices=price)
 
-
     # Now there is a distinct environment object with timer, weather and price data.
     # We can use it to access different data of interest.
 
     # For example, print the current weekday:
     print('Weekday:')
     print(environment.timer.weekday)
 
@@ -67,15 +65,14 @@
     print('\nOutdoor temperature forecast:')
     print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
 
     # For example, print the energy spot market day-ahead prices:
     print('\nDay-ahead spot market prices on 2015/01/01:')
     print(environment.prices.da_prices)
 
-
     # 2) Buildings objects:
 
     # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
     # represent the different customers of the local energy system / city district under investigation.
     # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
     # necessarily represent a building structure, as it would be the case for a wind energy converter.
 
@@ -85,15 +82,14 @@
     # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
     # In general, every building object can, however, hold up to N different apartments (=multi-family house).
     apartment = Apartment(environment=environment)
     bes = BuildingEnergySystem(environment=environment)
 
     building.addMultipleEntities([apartment, bes])
 
-
     # Every apartment usually possesses both electrical and thermal loads:
     # The electrical load is added to the apartment as follows:
     load = FixedLoad(environment=environment, method=1, annual_demand=3000)
 
     # Print and show the electrical power curve in Watt:
     print('\nElectrical load in Watt:')
     print(load.get_power(currentValues=False))
@@ -116,15 +112,14 @@
     plt.ylabel('Thermal power in Watt (space heating)')
     plt.title('Space heating power curve')
     if do_plot:
         plt.show()
 
     apartment.addMultipleEntities([load, space_heating])
 
-
     # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
     # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
     # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
     # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
     # several optimization constraints.
     eh = HeatPump(environment=environment, p_th_nom=16.0)
     ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
@@ -133,15 +128,14 @@
     bes.addMultipleDevices([eh, ths, pv])
 
     # Verify if the assets were added successfully (method getHasDevice):
     print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
     print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
     print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
 
-
     # 3) CityDistrict objects:
 
     # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
     # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
     # their local assets and it hence includes all the optimization problem information and data.
 
     # Create a city district object:
@@ -175,15 +169,14 @@
 
     # Print the city district information:
     print('\nTotal number of buildings in city district:')
     print(cd.get_nb_of_building_entities())
     print("\nDetailed city district information:")
     debug.print_district(cd, 3)
 
-
     # 4) Power scheduling:
 
     # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
     # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
     # the city district object to a certain power scheduling algorithm.
     # Here, the central optimization algorithm is used.
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_01_algorithm_central.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_01_algorithm_central.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -41,40 +41,40 @@
     e = Environment(timer=t, weather=w, prices=p)
 
     # City district with district operator objective "peak-shaving":
     cd = CityDistrict(environment=e, objective='peak-shaving')
 
     # Schedule two sample buildings. The buildings' objectives are defined as "price".
 
-    # Building no. one comes with fixed load, space heating, electrical heater, pv unit, thermal energy storage, and
+    # Building no. one comes with fixed load, space heating, electric heater, pv unit, thermal energy storage, and
     # electrical energy storage:
     bd1 = Building(environment=e, objective='price')
     cd.addEntity(entity=bd1, position=[0, 0])
     bes = BuildingEnergySystem(environment=e)
     bd1.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
     bes.addDevice(ths)
-    eh = ElectricalHeater(environment=e, p_th_nom=10)
+    eh = ElectricHeater(environment=e, p_th_nom=10)
     bes.addDevice(eh)
     ap = Apartment(environment=e)
     bd1.addEntity(ap)
     load = np.array([10.0, 10.0])
     fi = FixedLoad(e, method=0, demand=load)
     ap.addEntity(fi)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
     pv = Photovoltaic(environment=e, method=1, peak_power=4.6)
     bes.addDevice(pv)
-    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6)
+    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)
     bes.addDevice(bat)
 
-    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage
-    # and an electrical vehicle:
+    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage,
+    # and an electric vehicle:
     bd2 = Building(environment=e, objective='price')
-    cd.addEntity(entity=bd2, position=[0, 0])
+    cd.addEntity(entity=bd2, position=[0, 1])
     bes = BuildingEnergySystem(environment=e)
     bd2.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=35, soc_init=0.5)
     bes.addDevice(ths)
     chp = CombinedHeatPower(environment=e, p_th_nom=20.0)
     bes.addDevice(chp)
     ap = Apartment(environment=e)
@@ -82,15 +82,16 @@
     load = np.array([20.0, 20.0])
     dl = DeferrableLoad(environment=e, p_el_nom=2.0, e_consumption=2.0, load_time=[1, 1])
     ap.addEntity(dl)
     cl = CurtailableLoad(environment=e, p_el_nom=1.6, max_curtailment=0.8)
     ap.addEntity(cl)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
-    ev = ElectricalVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65, charging_time=[0, 1])
+    ev = ElectricVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.1, charging_time=[1, 1],
+                         simulate_driving=False, minimum_soc_end=0.9)
     ap.addEntity(ev)
 
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     results = opt.solve()
     cd.copy_schedule("central")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_02_algorithm_local.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_02_algorithm_local.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -41,40 +41,40 @@
     e = Environment(timer=t, weather=w, prices=p)
 
     # City district with district operator objective "peak-shaving":
     cd = CityDistrict(environment=e, objective='peak-shaving')
 
     # Schedule two sample buildings. The buildings' objectives are defined as "price".
 
-    # Building no. one comes with fixed load, space heating, electrical heater, pv unit, thermal energy storage, and
+    # Building no. one comes with fixed load, space heating, electric heater, pv unit, thermal energy storage, and
     # electrical energy storage:
     bd1 = Building(environment=e, objective='price')
     cd.addEntity(entity=bd1, position=[0, 0])
     bes = BuildingEnergySystem(environment=e)
     bd1.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
     bes.addDevice(ths)
-    eh = ElectricalHeater(environment=e, p_th_nom=10)
+    eh = ElectricHeater(environment=e, p_th_nom=10)
     bes.addDevice(eh)
     ap = Apartment(environment=e)
     bd1.addEntity(ap)
     load = np.array([10.0, 10.0])
     fi = FixedLoad(e, method=0, demand=load)
     ap.addEntity(fi)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
     pv = Photovoltaic(environment=e, method=1, peak_power=4.6)
     bes.addDevice(pv)
-    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6)
+    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)
     bes.addDevice(bat)
 
-    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage and
-    # an electrical vehicle:
+    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage,
+    # and an electric vehicle:
     bd2 = Building(environment=e, objective='price')
-    cd.addEntity(entity=bd2, position=[0, 0])
+    cd.addEntity(entity=bd2, position=[0, 1])
     bes = BuildingEnergySystem(environment=e)
     bd2.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=35, soc_init=0.5)
     bes.addDevice(ths)
     chp = CombinedHeatPower(environment=e, p_th_nom=20.0)
     bes.addDevice(chp)
     ap = Apartment(environment=e)
@@ -82,15 +82,16 @@
     load = np.array([20.0, 20.0])
     dl = DeferrableLoad(environment=e, p_el_nom=2.0, e_consumption=2.0, load_time=[1, 1])
     ap.addEntity(dl)
     cl = CurtailableLoad(environment=e, p_el_nom=1.6, max_curtailment=0.8)
     ap.addEntity(cl)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
-    ev = ElectricalVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65, charging_time=[0, 1])
+    ev = ElectricVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.1, charging_time=[1, 1],
+                         simulate_driving=False, minimum_soc_end=0.9)
     ap.addEntity(ev)
 
     # Perform the scheduling:
     opt = LocalOptimization(city_district=cd)
     results = opt.solve()
     cd.copy_schedule("local")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -41,40 +41,40 @@
     e = Environment(timer=t, weather=w, prices=p)
 
     # City district with district operator objective "peak-shaving":
     cd = CityDistrict(environment=e, objective='peak-shaving')
 
     # Schedule two sample buildings. The buildings' objectives are defined as "price".
 
-    # Building no. one comes with fixed load, space heating, electrical heater, pv unit, thermal energy storage, and
+    # Building no. one comes with fixed load, space heating, electric heater, pv unit, thermal energy storage, and
     # electrical energy storage:
     bd1 = Building(environment=e, objective='price')
     cd.addEntity(entity=bd1, position=[0, 0])
     bes = BuildingEnergySystem(environment=e)
     bd1.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
     bes.addDevice(ths)
-    eh = ElectricalHeater(environment=e, p_th_nom=10)
+    eh = ElectricHeater(environment=e, p_th_nom=10)
     bes.addDevice(eh)
     ap = Apartment(environment=e)
     bd1.addEntity(ap)
     load = np.array([10.0, 10.0])
     fi = FixedLoad(e, method=0, demand=load)
     ap.addEntity(fi)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
     pv = Photovoltaic(environment=e, method=1, peak_power=4.6)
     bes.addDevice(pv)
-    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6)
+    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)
     bes.addDevice(bat)
 
-    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage and
-    # an electrical vehicle:
+    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage,
+    # and an electric vehicle:
     bd2 = Building(environment=e, objective='price')
-    cd.addEntity(entity=bd2, position=[0, 0])
+    cd.addEntity(entity=bd2, position=[0, 1])
     bes = BuildingEnergySystem(environment=e)
     bd2.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=35, soc_init=0.5)
     bes.addDevice(ths)
     chp = CombinedHeatPower(environment=e, p_th_nom=20.0)
     bes.addDevice(chp)
     ap = Apartment(environment=e)
@@ -82,15 +82,16 @@
     load = np.array([20.0, 20.0])
     dl = DeferrableLoad(environment=e, p_el_nom=2.0, e_consumption=2.0, load_time=[1, 1])
     ap.addEntity(dl)
     cl = CurtailableLoad(environment=e, p_el_nom=1.6, max_curtailment=0.8)
     ap.addEntity(cl)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
-    ev = ElectricalVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65, charging_time=[0, 1])
+    ev = ElectricVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.1, charging_time=[1, 1],
+                         simulate_driving=False, minimum_soc_end=0.9)
     ap.addEntity(ev)
 
     # Perform the scheduling:
     opt = StandAlone(city_district=cd)
     results = opt.solve()
     cd.copy_schedule("stand-alone")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -40,40 +40,40 @@
     e = Environment(timer=t, weather=w, prices=p)
 
     # City district with district operator objective "peak-shaving":
     cd = CityDistrict(environment=e, objective='peak-shaving')
 
     # Schedule two sample buildings. The buildings' objectives are defined as "price".
 
-    # Building no. one comes with fixed load, space heating, electrical heater, pv unit, thermal energy storage, and
+    # Building no. one comes with fixed load, space heating, electric heater, pv unit, thermal energy storage, and
     # electrical energy storage:
     bd1 = Building(environment=e, objective='price')
     cd.addEntity(entity=bd1, position=[0, 0])
     bes = BuildingEnergySystem(environment=e)
     bd1.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
     bes.addDevice(ths)
-    eh = ElectricalHeater(environment=e, p_th_nom=10)
+    eh = ElectricHeater(environment=e, p_th_nom=10)
     bes.addDevice(eh)
     ap = Apartment(environment=e)
     bd1.addEntity(ap)
     load = np.array([10.0, 10.0])
     fi = FixedLoad(e, method=0, demand=load)
     ap.addEntity(fi)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
     pv = Photovoltaic(environment=e, method=1, peak_power=4.6)
     bes.addDevice(pv)
-    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6)
+    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)
     bes.addDevice(bat)
 
-    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage and
-    # an electrical vehicle:
+    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage,
+    # and an electric vehicle:
     bd2 = Building(environment=e, objective='price')
-    cd.addEntity(entity=bd2, position=[0, 0])
+    cd.addEntity(entity=bd2, position=[0, 1])
     bes = BuildingEnergySystem(environment=e)
     bd2.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=35, soc_init=0.5)
     bes.addDevice(ths)
     chp = CombinedHeatPower(environment=e, p_th_nom=20.0)
     bes.addDevice(chp)
     ap = Apartment(environment=e)
@@ -81,19 +81,20 @@
     load = np.array([20.0, 20.0])
     dl = DeferrableLoad(environment=e, p_el_nom=2.0, e_consumption=2.0, load_time=[1, 1])
     ap.addEntity(dl)
     cl = CurtailableLoad(environment=e, p_el_nom=1.6, max_curtailment=0.8)
     ap.addEntity(cl)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
-    ev = ElectricalVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65, charging_time=[0, 1])
+    ev = ElectricVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.1, charging_time=[1, 1],
+                         simulate_driving=False, minimum_soc_end=0.9)
     ap.addEntity(ev)
 
     # Perform the scheduling:
-    opt = DualDecomposition(city_district=cd, rho=0.1, eps_primal=1.0)
+    opt = DualDecomposition(city_district=cd, rho=0.1, eps_primal=1.0, max_iterations=1000)
     results = opt.solve()
     cd.copy_schedule("dual_decomposition")
 
     # Print some ADMM results:
     print("Dual Decomposition - Number of iterations:")
     print(results["iterations"][-1])
     print("Dual Decomposition - Norm vector 'r' over iterations:")
@@ -112,13 +113,13 @@
     return
 
 
 # Conclusions:
 # If the distributed dual decomposition optimization algorithm is applied, the two buildings are scheduled in a way
 # so that both the local and system level objectives are satisfied. Local flexibility is used to achieve the system
 # level objective. The scheduling results are close to the ones of the central algorithm, which demonstrates the
-# correctness of the distributed algorithm.
+# correctness of the distributed algorithm. Nevertheless, Dual Decomposition can be slow in convergence!
 
 
 if __name__ == '__main__':
     # Run example:
     main(do_plot=True)
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -41,40 +41,40 @@
     e = Environment(timer=t, weather=w, prices=p)
 
     # City district with district operator objective "peak-shaving":
     cd = CityDistrict(environment=e, objective='peak-shaving')
 
     # Schedule two sample buildings. The buildings' objectives are defined as "price".
 
-    # Building no. one comes with fixed load, space heating, electrical heater, pv unit, thermal energy storage, and
+    # Building no. one comes with fixed load, space heating, electric heater, pv unit, thermal energy storage, and
     # electrical energy storage:
     bd1 = Building(environment=e, objective='price')
     cd.addEntity(entity=bd1, position=[0, 0])
     bes = BuildingEnergySystem(environment=e)
     bd1.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
     bes.addDevice(ths)
-    eh = ElectricalHeater(environment=e, p_th_nom=10)
+    eh = ElectricHeater(environment=e, p_th_nom=10)
     bes.addDevice(eh)
     ap = Apartment(environment=e)
     bd1.addEntity(ap)
     load = np.array([10.0, 10.0])
     fi = FixedLoad(e, method=0, demand=load)
     ap.addEntity(fi)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
     pv = Photovoltaic(environment=e, method=1, peak_power=4.6)
     bes.addDevice(pv)
-    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6)
+    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)
     bes.addDevice(bat)
 
-    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage and
-    # an electrical vehicle:
+    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage,
+    # and an electric vehicle:
     bd2 = Building(environment=e, objective='price')
-    cd.addEntity(entity=bd2, position=[0, 0])
+    cd.addEntity(entity=bd2, position=[0, 1])
     bes = BuildingEnergySystem(environment=e)
     bd2.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=35, soc_init=0.5)
     bes.addDevice(ths)
     chp = CombinedHeatPower(environment=e, p_th_nom=20.0)
     bes.addDevice(chp)
     ap = Apartment(environment=e)
@@ -82,15 +82,16 @@
     load = np.array([20.0, 20.0])
     dl = DeferrableLoad(environment=e, p_el_nom=2.0, e_consumption=2.0, load_time=[1, 1])
     ap.addEntity(dl)
     cl = CurtailableLoad(environment=e, p_el_nom=1.6, max_curtailment=0.8)
     ap.addEntity(cl)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
-    ev = ElectricalVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65, charging_time=[0, 1])
+    ev = ElectricVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.1, charging_time=[1, 1],
+                         simulate_driving=False, minimum_soc_end=0.9)
     ap.addEntity(ev)
 
     # Perform the scheduling:
     opt = ExchangeADMM(city_district=cd, rho=2.0, eps_primal=0.001, eps_dual=0.01)
     results = opt.solve()
     cd.copy_schedule("admm")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_06_algorithm_warmstart.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_07_algorithm_warmstart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -30,15 +30,15 @@
 from pycity_scheduling.solvers import *
 
 
 # This examples demonstrates the warmstart capability for algorithms implemented in pycity_scheduling.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 06: Algorithm Warmstart ------\n\n")
+    print("\n\n------ Example 07: Algorithm Warmstart ------\n\n")
 
     # Unfortunately, algorithm warmstart capabilities are supported by the Gurobi/CPLEX solvers only:
     if not (DEFAULT_SOLVER is "gurobi_direct" or
             DEFAULT_SOLVER is "gurobi_persistent" or
             DEFAULT_SOLVER is "cplex"):
         print("Algorithm warmstart capability supported by the Gurobi/CPLEX solvers only! Example is not executed.")
         return
@@ -50,60 +50,61 @@
     e = Environment(timer=t, weather=w, prices=p)
 
     # City district with district operator objective "peak-shaving":
     cd = CityDistrict(environment=e, objective='peak-shaving')
 
     # Schedule two sample buildings. The buildings' objectives are defined as "peak-shaving".
 
-    # Building no. one comes with fixed load, space heating, electrical heater, pv unit, thermal energy storage, and
+    # Building no. one comes with fixed load, space heating, electric heater, pv unit, thermal energy storage, and
     # electrical battery energy storage:
     bd1 = Building(environment=e, objective='peak-shaving')
     cd.addEntity(entity=bd1, position=[0, 0])
     bes = BuildingEnergySystem(environment=e)
     bd1.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
     bes.addDevice(ths)
-    eh = ElectricalHeater(environment=e, p_th_nom=10, lower_activation_limit=0.25)
+    eh = ElectricHeater(environment=e, p_th_nom=10, lower_activation_limit=0.25)
     bes.addDevice(eh)
     ap = Apartment(environment=e)
     bd1.addEntity(ap)
     load = np.array(-np.sin(np.linspace(0, 2.1*np.pi, 96)+1))
     fi = FixedLoad(e, method=0, demand=load)
     ap.addEntity(fi)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
     pv = Photovoltaic(environment=e, method=1, peak_power=4.6)
     bes.addDevice(pv)
-    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6)
+    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)
     bes.addDevice(bat)
 
-    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage and
-    # an electrical vehicle:
+    # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage,
+    # and an electric vehicle:
     bd2 = Building(environment=e, objective='peak-shaving')
-    cd.addEntity(entity=bd2, position=[0, 0])
+    cd.addEntity(entity=bd2, position=[0, 1])
     bes = BuildingEnergySystem(environment=e)
     bd2.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=35, soc_init=0.5)
     bes.addDevice(ths)
-    chp = CombinedHeatPower(environment=e, p_th_nom=20.0, lower_activation_limit=0.1)
+    chp = CombinedHeatPower(environment=e, p_th_nom=20.0, lower_activation_limit=0.0)
     bes.addDevice(chp)
     ap = Apartment(environment=e)
     bd2.addEntity(ap)
     load = np.array(-2*np.sin(np.linspace(0, 1.9*np.pi, 96)+3))
     dl = DeferrableLoad(environment=e, p_el_nom=2.0, e_consumption=2.0)
     ap.addEntity(dl)
     cl = CurtailableLoad(environment=e, p_el_nom=1.6, max_curtailment=0.8)
     ap.addEntity(cl)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
-    ev = ElectricalVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65)
+    ev = ElectricVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.5, simulate_driving=False,
+                         minimum_soc_end=0.8, charging_time=np.ones(t.simu_horizon))
     ap.addEntity(ev)
 
     # Perform the scheduling with the Exchange ADMM algorithm to obtain an algorithm warmstart point:
-    opt = ExchangeADMM(city_district=cd, rho=2.0, eps_primal=1, eps_dual=1, mode="integer")
+    opt = ExchangeADMM(city_district=cd, rho=2.0, eps_primal=0.01, eps_dual=0.01, mode="integer")
     r1 = opt.solve()
     imbalance = sum(np.abs(cd.schedule["p_el"] - bd1.schedule["p_el"] - bd2.schedule["p_el"]))
 
     # Let the city district account for power imbalances in order to achieve a feasible schedule.
     cd.account_imbalance()
     admm_obj_imbalance = pyomo.value(cd.get_objective() + bd1.get_objective() + bd2.get_objective())
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_07_objective_peak-shaving.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_09_objective_peak-shaving.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -30,15 +30,15 @@
 
 
 # This is a very simple power scheduling example using the central optimization algorithm to demonstrate the impact
 # of system level objective "peak-shaving".
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 07: Objective Peak-Shaving ------\n\n")
+    print("\n\n------ Example 09: Objective Peak-Shaving ------\n\n")
 
     # Define timer, price, weather, and environment objects:
     t = Timer(op_horizon=96, step_size=900, initial_date=(2015, 4, 1))
     p = Prices(timer=t)
     w = Weather(timer=t)
     e = Environment(timer=t, weather=w, prices=p)
 
@@ -50,28 +50,27 @@
     for i in range(n):
         bd = Building(environment=e, objective='none')
         cd.addEntity(entity=bd, position=[0, i])
         bes = BuildingEnergySystem(environment=e)
         bd.addEntity(bes)
         ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(environment=e, p_th_nom=10)
+        eh = ElectricHeater(environment=e, p_th_nom=10)
         bes.addDevice(eh)
         ap = Apartment(environment=e)
         bd.addEntity(ap)
         fi = FixedLoad(e, method=1, annual_demand=3000.0, profile_type='H0')
         ap.addEntity(fi)
         sh = SpaceHeating(environment=e, method=1, living_area=120, specific_demand=90, profile_type='HEF')
         ap.addEntity(sh)
         pv = Photovoltaic(environment=e, method=1, peak_power=8.2)
         bes.addDevice(pv)
-        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6)
+        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6, eta=1.0)
         bes.addDevice(bat)
 
-
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     opt.solve()
     cd.copy_schedule("peak-shaving")
 
     # Print and show the city district's schedule:
     print("Schedule of the city district:")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_08_objective_max-consumption.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_11_objective_max-consumption.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -30,15 +30,15 @@
 
 
 # This is a very simple power scheduling example using the central optimization algorithm to demonstrate the impact
 # of system level objective "max-consumption".
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 08: Objective Max-Consumption ------\n\n")
+    print("\n\n------ Example 11: Objective Max-Consumption ------\n\n")
 
     # Define timer, price, weather, and environment objects:
     t = Timer(op_horizon=96, step_size=900, initial_date=(2015, 4, 1))
     p = Prices(timer=t)
     w = Weather(timer=t)
     e = Environment(timer=t, weather=w, prices=p)
 
@@ -50,28 +50,27 @@
     for i in range(n):
         bd = Building(environment=e, objective='none')
         cd.addEntity(entity=bd, position=[0, i])
         bes = BuildingEnergySystem(environment=e)
         bd.addEntity(bes)
         ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(environment=e, p_th_nom=10)
+        eh = ElectricHeater(environment=e, p_th_nom=10)
         bes.addDevice(eh)
         ap = Apartment(environment=e)
         bd.addEntity(ap)
         fi = FixedLoad(e, method=1, annual_demand=3000.0, profile_type='H0')
         ap.addEntity(fi)
         sh = SpaceHeating(environment=e, method=1, living_area=120, specific_demand=90, profile_type='HEF')
         ap.addEntity(sh)
         pv = Photovoltaic(environment=e, method=1, peak_power=8.2)
         bes.addDevice(pv)
-        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6)
+        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6, eta=1.0)
         bes.addDevice(bat)
 
-
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     results = opt.solve()
     cd.copy_schedule("max-consumption")
 
     # Print and show the city district's schedule:
     print("Schedule of the city district:")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_09_objective_self-consumption.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_10_objective_self-consumption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -30,15 +30,15 @@
 
 
 # This is a very simple power scheduling example using the central optimization algorithm to demonstrate the impact
 # of system level objective "self-consumption".
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 09: Objective Self-Consumption ------\n\n")
+    print("\n\n------ Example 10: Objective Self-Consumption ------\n\n")
 
     # Define timer, price, weather, and environment objects:
     t = Timer(op_horizon=96, step_size=900, initial_date=(2015, 4, 1))
     p = Prices(timer=t)
     w = Weather(timer=t)
     e = Environment(timer=t, weather=w, prices=p)
 
@@ -50,38 +50,36 @@
     for i in range(n):
         bd = Building(environment=e, objective='none')
         cd.addEntity(entity=bd, position=[0, i])
         bes = BuildingEnergySystem(environment=e)
         bd.addEntity(bes)
         ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(environment=e, p_th_nom=10)
+        eh = ElectricHeater(environment=e, p_th_nom=10)
         bes.addDevice(eh)
         ap = Apartment(environment=e)
         bd.addEntity(ap)
         fi = FixedLoad(e, method=1, annual_demand=3000.0, profile_type='H0')
         ap.addEntity(fi)
         sh = SpaceHeating(environment=e, method=1, living_area=120, specific_demand=90, profile_type='HEF')
         ap.addEntity(sh)
         pv = Photovoltaic(environment=e, method=1, peak_power=8.2)
         bes.addDevice(pv)
-        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6)
+        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6, eta=1.0)
         bes.addDevice(bat)
 
-
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     results = opt.solve()
     cd.copy_schedule("self-consumption")
 
     # Print and show the city district's schedule:
     print("Schedule of the city district:")
     print(list(cd.p_el_schedule))
     plt.plot(cd.p_el_schedule)
-    #plt.ylim([-2.0, 5.0])
     plt.xlabel('Time in hours')
     plt.ylabel('Electrical power in kW')
     plt.title('City district scheduling result')
     plt.grid()
     if do_plot:
         plt.show()
     return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_10_objective_price.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_12_objective_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -31,15 +31,15 @@
 
 
 # This is a very simple power scheduling example using the central optimization algorithm to demonstrate the impact
 # of system level objective "price".
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 10: Objective Price ------\n\n")
+    print("\n\n------ Example 12: Objective Price ------\n\n")
 
     # Define timer, price, weather, and environment objects:
     t = Timer(op_horizon=96, step_size=900, initial_date=(2015, 4, 1))
     p = Prices(timer=t)
     w = Weather(timer=t)
     e = Environment(timer=t, weather=w, prices=p)
 
@@ -51,28 +51,27 @@
     for i in range(n):
         bd = Building(environment=e, objective='none')
         cd.addEntity(entity=bd, position=[0, i])
         bes = BuildingEnergySystem(environment=e)
         bd.addEntity(bes)
         ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(environment=e, p_th_nom=10)
+        eh = ElectricHeater(environment=e, p_th_nom=10)
         bes.addDevice(eh)
         ap = Apartment(environment=e)
         bd.addEntity(ap)
         fi = FixedLoad(e, method=1, annual_demand=3000.0, profile_type='H0')
         ap.addEntity(fi)
         sh = SpaceHeating(environment=e, method=1, living_area=120, specific_demand=90, profile_type='HEF')
         ap.addEntity(sh)
         pv = Photovoltaic(environment=e, method=1, peak_power=8.2)
         bes.addDevice(pv)
-        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6)
+        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6, eta=1.0)
         bes.addDevice(bat)
 
-
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     opt.solve()
     cd.copy_schedule("price")
 
     # Print and show the city district's schedule:
     print("Schedule of the city district:")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_11_objective_co2.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_13_objective_co2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -31,15 +31,15 @@
 
 
 # This is a very simple power scheduling example using the central optimization algorithm to demonstrate the impact
 # of system level objective "co2".
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 11: Objective CO2------\n\n")
+    print("\n\n------ Example 13: Objective CO2------\n\n")
 
     # Define timer, price, weather, and environment objects:
     t = Timer(op_horizon=96, step_size=900, initial_date=(2015, 4, 1))
     p = Prices(timer=t)
     w = Weather(timer=t)
     e = Environment(timer=t, weather=w, prices=p)
 
@@ -51,28 +51,27 @@
     for i in range(n):
         bd = Building(environment=e, objective='none')
         cd.addEntity(entity=bd, position=[0, i])
         bes = BuildingEnergySystem(environment=e)
         bd.addEntity(bes)
         ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(environment=e, p_th_nom=10)
+        eh = ElectricHeater(environment=e, p_th_nom=10)
         bes.addDevice(eh)
         ap = Apartment(environment=e)
         bd.addEntity(ap)
         fi = FixedLoad(e, method=1, annual_demand=3000.0, profile_type='H0')
         ap.addEntity(fi)
         sh = SpaceHeating(environment=e, method=1, living_area=120, specific_demand=90, profile_type='HEF')
         ap.addEntity(sh)
         pv = Photovoltaic(environment=e, method=1, peak_power=8.2)
         bes.addDevice(pv)
-        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6)
+        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6, eta=1.0)
         bes.addDevice(bat)
 
-
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     opt.solve()
     cd.copy_schedule("co2")
 
     # Print and show the city district's schedule:
     print("Schedule of the city district:")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_12_objective_valley-filling.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_14_objective_valley-filling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -31,15 +31,15 @@
 
 
 # This is a very simple power scheduling example using the central optimization algorithm to demonstrate the impact
 # of system level objective "valley-filling".
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 12: Objective Valley-Filling ------\n\n")
+    print("\n\n------ Example 14: Objective Valley-Filling ------\n\n")
 
     # Define timer, price, weather, and environment objects:
     t = Timer(op_horizon=96, step_size=900, initial_date=(2015, 4, 1))
     p = Prices(timer=t)
     w = Weather(timer=t)
     e = Environment(timer=t, weather=w, prices=p)
 
@@ -52,28 +52,27 @@
     for i in range(n):
         bd = Building(environment=e, objective='none')
         cd.addEntity(entity=bd, position=[0, i])
         bes = BuildingEnergySystem(environment=e)
         bd.addEntity(bes)
         ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(environment=e, p_th_nom=10)
+        eh = ElectricHeater(environment=e, p_th_nom=10)
         bes.addDevice(eh)
         ap = Apartment(environment=e)
         bd.addEntity(ap)
         fi = FixedLoad(e, method=1, annual_demand=3000.0, profile_type='H0')
         ap.addEntity(fi)
         sh = SpaceHeating(environment=e, method=1, living_area=120, specific_demand=90, profile_type='HEF')
         ap.addEntity(sh)
         pv = Photovoltaic(environment=e, method=1, peak_power=8.2)
         bes.addDevice(pv)
-        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6)
+        bat = Battery(environment=e, e_el_max=12.0, p_el_max_charge=4.6, p_el_max_discharge=4.6, eta=1.0)
         bes.addDevice(bat)
 
-
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     results = opt.solve()
     cd.copy_schedule("valley-filling")
 
     # Print and show the city district's schedule:
     print("Schedule of the city district:")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_13_district_generator.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_15_district_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -31,15 +31,15 @@
 # This examples shows the creation of a (complex) city district setup using the pycity_scheduling district generator.
 # The obtained district setup is based on building stock information data provided by the EU project TABULA/EPISCOPE
 # (https://episcope.eu/welcome/). The functions required for the city district setup can be found in the
 # pycity_scheduling factory file.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 13: District Generator ------\n\n")
+    print("\n\n------ Example 15: District Generator ------\n\n")
 
     # First, create an environment using the factory's "generate_standard_environment" method. The environment
     # automatically encapsulates time, weather, and price data/information.
     env = factory.generate_standard_environment(initial_date=(2018, 12, 6), step_size=900, op_horizon=96)
 
     # Create 20 single-family houses:
     num_sfh = 20
@@ -47,15 +47,15 @@
     # 50% SFH.2002, 30% SFH.2010, 20% SFH.2016 (based on TABULA):
     sfh_distribution = {
         'SFH.2002': 0.5,
         'SFH.2010': 0.3,
         'SFH.2016': 0.2,
     }
 
-    # 50% of the single-family houses are equipped with heat pump, 10% with boiler, and 40% with electrical heater:
+    # 50% of the single-family houses are equipped with heat pump, 10% with boiler, and 40% with electric heater:
     sfh_heating_distribution = {
         'HP': 0.5,
         'BL': 0.1,
         'EH': 0.4,
     }
 
     # All single-family houses are equipped with a fixed load, 20% have a deferrable load, and 30% have an electric
@@ -76,15 +76,15 @@
     # 60% MFH.2002, 20% SFH.2010, 20% SFH.2016 (based on TABULA):
     mfh_distribution = {
         'MFH.2002': 0.6,
         'MFH.2010': 0.2,
         'MFH.2016': 0.2,
     }
 
-    # 40% of the multi-family houses are equipped with heat pump, 20% with boiler, and 40% with electrical heater:
+    # 40% of the multi-family houses are equipped with heat pump, 20% with boiler, and 40% with electric heater:
     mfh_heating_distribution = {
         'HP': 0.4,
         'BL': 0.2,
         'EH': 0.4,
     }
 
     # All apartments inside a multi-family houses are equipped with a fixed load, 20% have a deferrable load, and 20%
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_14_district_flexibility_quantification.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_17_district_flexibility_quantification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -25,19 +25,19 @@
 import numpy as np
 
 import pycity_scheduling.util.factory as factory
 from pycity_scheduling.util import calculate_flexibility_potential
 
 
 # This example shows how to quantify the operational flexibility potential for a given city district using
-# pycity_scheduling. It is built upon the same district setup as defined in example 'example_12_district_generator.py'.
+# pycity_scheduling. It is built upon the same district setup as defined in example 'example_15_district_generator.py'.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 14: District Flexibility Quantification ------\n\n")
+    print("\n\n------ Example 17: District Flexibility Quantification ------\n\n")
 
     # First, create an environment using the factory's "generate_standard_environment" method. The environment
     # automatically encapsulates time, weather, and price data/information.
     env = factory.generate_standard_environment(initial_date=(2018, 12, 6), step_size=900, op_horizon=96)
 
     # Create 12 single-family houses:
     num_sfh = 12
@@ -45,15 +45,15 @@
     # 50% SFH.2002, 30% SFH.2010, 20% SFH.2016 (based on TABULA):
     sfh_distribution = {
         'SFH.2002': 0.5,
         'SFH.2010': 0.3,
         'SFH.2016': 0.2,
     }
 
-    # 50% of the single-family houses are equipped with heat pump, 10% with boiler, and 40% with electrical heater:
+    # 50% of the single-family houses are equipped with heat pump, 10% with boiler, and 40% with electric heater:
     sfh_heating_distribution = {
         'HP': 0.5,
         'BL': 0.1,
         'EH': 0.4,
     }
 
     # All single-family houses are equipped with a fixed load, 20% have a deferrable load, and 30% have an electric
@@ -74,15 +74,15 @@
     # 60% MFH.2002, 20% SFH.2010, 20% SFH.2016 (based on TABULA):
     mfh_distribution = {
         'MFH.2002': 0.6,
         'MFH.2010': 0.2,
         'MFH.2016': 0.2,
     }
 
-    # 40% of the multi-family houses are equipped with heat pump, 20% with boiler, and 40% with electrical heater:
+    # 40% of the multi-family houses are equipped with heat pump, 20% with boiler, and 40% with electric heater:
     mfh_heating_distribution = {
         'HP': 0.4,
         'BL': 0.2,
         'EH': 0.4,
     }
 
     # All apartments inside a multi-family houses are equipped with a fixed load, 20% have a deferrable load, and 20%
@@ -104,15 +104,14 @@
                                                 sfh_building_distribution=sfh_distribution,
                                                 sfh_heating_distribution=sfh_heating_distribution,
                                                 sfh_device_probabilities=sfh_device_probs,
                                                 mfh_building_distribution=mfh_distribution,
                                                 mfh_heating_distribution=mfh_heating_distribution,
                                                 mfh_device_probabilities=mfh_device_probs)
 
-
     # The city district's maximum operational flexibility potential in terms of the absolute flexibility gain metric can
     # be quantified very easily using the pycity_scheduling's "calculate_flexibility_potential" function. The absolute
     # flexibility gain is a measure for the energy shifted between a coordinated and an uncoordinated scheduling
     # scenario. Here, the coordinated case is represented through the central optimization algorithm, whereas the
     # uncoordinated case is represented through the stand-alone optimization algorithm.
     flex = calculate_flexibility_potential(city_district=district,
                                            algorithm="central",
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_15_scheduling_complex_city_district.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_16_scheduling_complex_city_district.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -28,19 +28,19 @@
 import pycity_scheduling.util.factory as factory
 import pycity_scheduling.util.debug as debug
 from pycity_scheduling.algorithms import *
 from pycity_scheduling.classes import *
 
 
 # In this example, the power schedule for a complex city district scenario is determined. The scenario is built upon the
-# district setup as defined in example 'example_12_district_generator.py', but it contains more than 100 buildings and
+# district setup as defined in example 'example_15_district_generator.py', but it contains more than 100 buildings and
 # is hence considered more complex.
 
 def main(do_plot=False):
-    print("\n\n------ Example 15: Scheduling Complex City District ------\n\n")
+    print("\n\n------ Example 16: Scheduling Complex City District ------\n\n")
 
     # First, create an environment using the factory's "generate_standard_environment" method. The environment
     # automatically encapsulates time, weather, and price data/information.
     env = factory.generate_standard_environment(initial_date=(2018, 12, 6), step_size=900, op_horizon=96)
 
     # Create 75 single-family houses:
     num_sfh = 75
@@ -48,15 +48,15 @@
     # 50% SFH.2002, 30% SFH.2010, 20% SFH.2016 (based on TABULA):
     sfh_distribution = {
         'SFH.2002': 0.5,
         'SFH.2010': 0.3,
         'SFH.2016': 0.2,
     }
 
-    # 50% of the single-family houses are equipped with heat pump, 10% with boiler, and 40% with electrical heater:
+    # 50% of the single-family houses are equipped with heat pump, 10% with boiler, and 40% with electric heater:
     sfh_heating_distribution = {
         'HP': 0.5,
         'BL': 0.1,
         'EH': 0.4,
     }
 
     # All single-family houses are equipped with a fixed load, 20% have a deferrable load, and 30% have an electric
@@ -77,15 +77,15 @@
     # 60% MFH.2002, 20% SFH.2010, 20% SFH.2016 (based on TABULA):
     mfh_distribution = {
         'MFH.2002': 0.6,
         'MFH.2010': 0.2,
         'MFH.2016': 0.2,
     }
 
-    # 40% of the multi-family houses are equipped with heat pump, 20% with boiler, and 40% with electrical heater:
+    # 40% of the multi-family houses are equipped with heat pump, 20% with boiler, and 40% with electric heater:
     mfh_heating_distribution = {
         'HP': 0.4,
         'BL': 0.2,
         'EH': 0.4,
     }
 
     # All apartments inside a multi-family houses are equipped with a fixed load, 20% have a deferrable load, and 20%
@@ -96,16 +96,17 @@
         'FL': 1,
         'DL': 0.2,
         'EV': 0.2,
         'BAT': 0.4,
         'PV': 0.8,
     }
 
-    # Finally, create the desired city district using the factory's "generate_tabula_district" method. The district's/
-    # district operator's objective is defined as "peak-shaving" and the buildings' objectives are defined as "price".
+    # Finally, create the desired city district using the factory's "generate_tabula_district" method. The district's
+    # district operator's objective is defined as "price" (i.e., day-ahead prices) and the buildings' objectives are
+    # also defined as "price" (i.e., time-of-use prices).
     district = factory.generate_tabula_district(env, num_sfh, num_mfh,
                                                 sfh_distribution,
                                                 sfh_heating_distribution,
                                                 sfh_device_probs,
                                                 mfh_distribution,
                                                 mfh_heating_distribution,
                                                 mfh_device_probs,
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_16_scheduling_convex_vs._integer_mode.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_20_scheduling_convex_vs._integer_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -28,47 +28,46 @@
 
 import pycity_scheduling.util.factory as factory
 from pycity_scheduling.classes import *
 from pycity_scheduling.algorithms import *
 
 
 # This is a simple power scheduling example to demonstrate the difference between the pycity_scheduling's convex and
-# integer (MIP) optimization models using the distributed Exchange ADMM algorithm.
+# integer (MIP) optimization models using the distributed Exchange MIQP ADMM algorithm.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 16: Scheduling Convex vs. Integer Mode ------\n\n")
+    print("\n\n------ Example 20: Scheduling Convex vs. Integer Mode ------\n\n")
 
     # Scheduling will be performed for a typical winter day within the annual heating period:
     env = factory.generate_standard_environment(step_size=3600, op_horizon=24, mpc_horizon=None, mpc_step_width=None,
                                                 initial_date=(2010, 2, 10), initial_time=(0, 0, 0))
 
     # City district / district operator objective is peak-shaving:
     cd = CityDistrict(environment=env, objective='peak-shaving')
 
-    # Building equipped with space heating, electrical heater, thermal energy storage, and photovoltaic unit.
-    # Objective is peak-shaving:
-    bd1 = Building(environment=env, objective='peak-shaving')
+    # Building equipped with space heating, electric heater, thermal energy storage, and photovoltaic unit.
+    # Objective is self-consumption:
+    bd1 = Building(environment=env, objective='self-consumption')
     cd.addEntity(entity=bd1, position=[0, 0])
     ap1 = Apartment(environment=env)
     bd1.addEntity(ap1)
     sh1 = SpaceHeating(environment=env, method=1, living_area=120.0, specific_demand=85.9, profile_type='HEF')
     ap1.addEntity(sh1)
     bes1 = BuildingEnergySystem(environment=env)
     bd1.addEntity(bes1)
-    eh1 = ElectricalHeater(environment=env, p_th_nom=12.0, lower_activation_limit=0.5)
+    eh1 = ElectricHeater(environment=env, p_th_nom=12.0, lower_activation_limit=0.25)
     bes1.addDevice(eh1)
     ths1 = ThermalHeatingStorage(environment=env, e_th_max=24.0)
     bes1.addDevice(ths1)
     pv1 = Photovoltaic(environment=env, method=1, peak_power=25.0)
     bes1.addDevice(pv1)
 
-
     # First, perform the power scheduling using convex models for the electrical appliances:
-    opt = ExchangeADMM(cd, mode='convex')
+    opt = ExchangeMIQPADMM(cd, mode='convex', rho=0.5, eps_primal=1.0, eps_dual=0.1)
     opt.solve()
     cd.copy_schedule("convex_schedule")
 
     # Plot the convex schedules:
     plot_time = list(range(env.timer.timesteps_used_horizon))
 
     gs = gridspec.GridSpec(5, 1)
@@ -111,15 +110,15 @@
         if hasattr(figManager, "window"):
             figManagerWindow = figManager.window
             if hasattr(figManagerWindow, "state"):
                 figManager.window.state("zoomed")
         plt.show()
 
     # Second, perform the power scheduling using integer models for the electrical appliances:
-    opt = ExchangeADMM(cd, mode='integer')
+    opt = ExchangeMIQPADMM(cd, mode='integer', rho=0.5, eps_primal=1.0, eps_dual=0.1)
     opt.solve()
     cd.copy_schedule("integer_schedule")
 
     # Plot the integer schedules:
     gs = gridspec.GridSpec(5, 1)
     ax0 = plt.subplot(gs[0])
     ax0.plot(plot_time, cd.p_el_schedule)
@@ -165,16 +164,16 @@
     return
 
 
 # Conclusions:
 # In the convex case, the peak-shaving objective can be fully satisfied, which becomes evident from the "flat" power
 # profile of the obtained city district power curve. To perfectly balance the power demand and supply in the district,
 # the flexibility from the thermal heating storage unit is exploited together with the capability to operate the
-# electrical heater at any operation point between 0% and 100% of its nominal power. Instead, in the integer case, the
-# electrical heater can only operate at either 0% or in-between 50% and 100% of its nominal power. For this reason, the
+# electric heater at any operation point between 0% and 100% of its nominal power. Instead, in the integer case, the
+# electric heater can only operate at either 0% or in-between 25% and 100% of its nominal power. For this reason, the
 # final power profile on the city district level is not as "flat" as in the convex case. However, the integer case
-# might better reflect the actual operation conditions of a real electrical heater unit.
+# might better reflect the actual operation conditions of a real electric heater unit.
 
 
 if __name__ == '__main__':
     # Run example:
     main(do_plot=True)
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_17_scheduling_pv+battery_system.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_18_scheduling_pv+battery_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -32,15 +32,15 @@
 
 
 # This is a simple power scheduling example to demonstrate the integration and interaction of PV and battery storage
 # systems using the central optimization algorithm.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 17: Scheduling PV+Battery System ------\n\n")
+    print("\n\n------ Example 18: Scheduling PV+Battery System ------\n\n")
 
     # Scheduling will be performed for one month:
     env = factory.generate_standard_environment(step_size=3600, op_horizon=24*31, mpc_horizon=None,
                                                 mpc_step_width=None, initial_date=(2018, 3, 1), initial_time=(0, 0, 0))
 
     # City district / district operator objective is peak-shaving:
     cd = CityDistrict(environment=env, objective='peak-shaving')
@@ -52,15 +52,15 @@
     bd.addEntity(ap)
     fl = FixedLoad(environment=env, method=1, annual_demand=3500.0, profile_type="H0")
     ap.addEntity(fl)
     bes = BuildingEnergySystem(environment=env)
     bd.addEntity(bes)
     pv = Photovoltaic(environment=env, method=0, area=25.0, beta=30.0, eta_noct=0.15)
     bes.addDevice(pv)
-    bat = Battery(environment=env, e_el_max=13.6, p_el_max_charge=24.0, p_el_max_discharge=3.6, soc_init=0.5, eta=1,
+    bat = Battery(environment=env, e_el_max=13.6, p_el_max_charge=24.0, p_el_max_discharge=3.6, soc_init=0.5, eta=1.0,
                   storage_end_equality=True)
     bes.addDevice(bat)
 
     # Perform the scheduling:
     opt = CentralOptimization(city_district=cd)
     results = opt.solve()
     cd.copy_schedule("central")
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_18_scheduling_heating_and_cooling_loads.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_19_scheduling_heating_and_cooling_loads.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -32,15 +32,15 @@
 
 
 # This is a simple power scheduling example to demonstrate the integration and impact of building cooling and
 # heating loads using the central optimization algorithm.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 18: Scheduling Heating and Cooling Loads ------\n\n")
+    print("\n\n------ Example 19: Scheduling Heating and Cooling Loads ------\n\n")
 
     # Scheduling will be performed for a full year:
     env = factory.generate_standard_environment(step_size=3600, op_horizon=24*365, mpc_horizon=None,
                                                 mpc_step_width=None, initial_date=(2018, 1, 1), initial_time=(0, 0, 0))
 
     # Use a standardized thermal load profile for space heating and then 'convert' it into a cooling load
     # (inverted load assumption according to pycity_base):
@@ -71,15 +71,14 @@
         figManager = plt.get_current_fig_manager()
         if hasattr(figManager, "window"):
             figManagerWindow = figManager.window
             if hasattr(figManagerWindow, "state"):
                 figManager.window.state("zoomed")
         plt.show()
 
-
     # Now perform the scheduling of two buildings, where the first building is equipped with the heating load and
     # a thermal heating system and the second building is equipped with the cooling load and a thermal cooling system.
 
     # City district with district operator objective "price":
     cd = CityDistrict(environment=env, objective='max-consumption')
 
     # Building no. one with building objective price:
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_19_scheduling_robust_optimization.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_21_scheduling_robust_optimization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -30,21 +30,21 @@
 from pycity_scheduling.util.metric import calculate_costs
 
 
 # This is a simple power scheduling example combined with a Robust Optimization (RO) application.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 19: Scheduling Robust Optimization ------\n\n")
+    print("\n\n------ Example 21: Scheduling Robust Optimization ------\n\n")
 
     # Use a simple environment of 6 hours with quarter-hourly resolution (=15min=900sec):
     env = factory.generate_standard_environment(step_size=900, op_horizon=6)
 
     # Make it "attractive" for the customer to shift demand into the first half of the scheduling period
-    # (compare example_20_post-processing_metrics_evaluation.py):
+    # (compare example_23_post-processing_metrics_evaluation.py):
     env.prices.tou_prices = np.array([5]*3 + [10]*3)
 
     district = classes.CityDistrict(env)
     # The sample building in this example comes with a constant space heating load of 10kW, thermal storage of capacity
     # 20kWh and an electric heater of thermal nominal power 20kW:
     bd = factory.generate_simple_building(env, sh=10, ths=20, eh=20)
 
@@ -56,15 +56,15 @@
     bd.copy_schedule("ref")
 
     # Protect 6 time steps and assume a maximum deviation of 50% in each time step.
     # Such a high deviation is usually unrealistic, but makes it a good example here.
     opt.solve(robustness=(6, 0.5))
 
     # Print schedules/results:
-    # **Note:** We compare the schedules from the two performed schedulings (with/without RO) with each other.
+    # We compare the schedules from the two performed schedulings (with/without RO) with each other.
     np.set_printoptions(formatter={'float': '{: >8.3f}'.format})
     print('Building p_el:')
     print(bd.p_el_ref_schedule)
     print(bd.p_el_schedule)
     print('ThermalEnergyStorage e_th_heat:')
     print(bd.bes.tes_units[0].e_th_heat_ref_schedule)
     print(bd.bes.tes_units[0].e_th_heat_schedule)
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_20_post-processing_schedule_evaluation.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_22_post-processing_schedule_evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -31,53 +31,53 @@
 from pycity_scheduling.util.write_schedules import schedule_to_json, schedule_to_csv
 
 
 # This examples demonstrates some post-processing capabilities of the pycity_scheduling framework.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 20: Post-Processing Schedule Evaluation ------\n\n")
+    print("\n\n------ Example 22: Post-Processing Schedule Evaluation ------\n\n")
 
     # Define timer, price, weather, and environment objects:
     t = Timer()
     p = Prices(timer=t)
     w = Weather(timer=t)
     e = Environment(timer=t, weather=w, prices=p)
 
     # City district with district operator objective "peak-shaving":
     cd = CityDistrict(environment=e, objective='peak-shaving')
 
     # Schedule two sample buildings. The buildings' objectives are defined as "peak-shaving".
 
-    # Building no. one comes with fixed load, space heating, electrical heater, pv unit, thermal energy storage, and
+    # Building no. one comes with fixed load, space heating, electric heater, pv unit, thermal energy storage, and
     # electrical battery energy storage:
     bd1 = Building(environment=e, objective='peak-shaving')
     cd.addEntity(entity=bd1, position=[0, 0])
     bes = BuildingEnergySystem(environment=e)
     bd1.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=40, soc_init=0.5)
     bes.addDevice(ths)
-    eh = ElectricalHeater(environment=e, p_th_nom=10)
+    eh = ElectricHeater(environment=e, p_th_nom=10)
     bes.addDevice(eh)
     ap = Apartment(environment=e)
     bd1.addEntity(ap)
     load = np.array(-np.sin(np.linspace(0, 2.1*np.pi, 96)+1))
     fi = FixedLoad(e, method=0, demand=load)
     ap.addEntity(fi)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
     pv = Photovoltaic(environment=e, method=1, peak_power=4.6)
     bes.addDevice(pv)
-    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6)
+    bat = Battery(environment=e, e_el_max=4.8, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)
     bes.addDevice(bat)
 
     # Building no. two comes with deferrable load, curtailable load, space heating, chp unit, thermal energy storage and
-    # an electrical vehicle:
+    # an electric vehicle:
     bd2 = Building(environment=e, objective='peak-shaving')
-    cd.addEntity(entity=bd2, position=[0, 0])
+    cd.addEntity(entity=bd2, position=[0, 1])
     bes = BuildingEnergySystem(environment=e)
     bd2.addEntity(bes)
     ths = ThermalHeatingStorage(environment=e, e_th_max=35, soc_init=0.5)
     bes.addDevice(ths)
     chp = CombinedHeatPower(environment=e, p_th_nom=20.0)
     bes.addDevice(chp)
     ap = Apartment(environment=e)
@@ -85,15 +85,16 @@
     load = np.array(-2*np.sin(np.linspace(0, 1.9*np.pi, 96)+3))
     dl = DeferrableLoad(environment=e, p_el_nom=2.0, e_consumption=2.0)
     ap.addEntity(dl)
     cl = CurtailableLoad(environment=e, p_el_nom=1.6, max_curtailment=0.8)
     ap.addEntity(cl)
     sh = SpaceHeating(environment=e, method=0, loadcurve=load)
     ap.addEntity(sh)
-    ev = ElectricalVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65)
+    ev = ElectricVehicle(environment=e, e_el_max=37.0, p_el_max_charge=22.0, soc_init=0.65, simulate_driving=True,
+                         minimum_soc_end=0.8)
     ap.addEntity(ev)
 
     # Perform the local scheduling:
     opt = LocalOptimization(city_district=cd)
     opt.solve()
     cd.copy_schedule("ref")
 
@@ -104,15 +105,14 @@
 
     if not do_plot:
         fig, ax = plt.subplots()
         kwargs = {'ax': ax}
     else:
         kwargs = {}
 
-
     # As the power generation of a PV unit cannot be altered by the algorithms when force_renewables is not set to True,
     # the schedule is the same for 'ref' and 'default'.
     if do_plot:
         plot_entity(pv, schedule=["ref", "default"], **kwargs)
 
     # When the city district objective is not considered in the scheduling (= uncoordinated reference case), the
     # electricity schedule of the city district is usually not balanced. This is not the case for the coordinated case
@@ -128,37 +128,36 @@
 
     # The CHP unit has the optional integer variable p_th_Heat_state. Even when the integer mode is not used as in this
     # example, the schedule for this variable is still provided. For this variable, the value is always rounded to zero
     # if it is close enough to zero.
     if do_plot:
         plot_entity(chp, schedule=["ref", "default"], **kwargs)
 
-    # The electrical vehicle and battery objects also have an integer variable. This variable indicates if the battery
+    # The electric vehicle and battery objects also have an integer variable. This variable indicates if the battery
     # is either charging or discharging/not charging.
     if do_plot:
         plot_entity(ev, schedule=["ref", "default"], **kwargs)
 
     # The imbalance for the city district schedule in respect to the two buildings' schedules is rather large for the
     # default schedule. This is because of the relatively large eps_primal value for the ADMM algorithm in this example.
     if do_plot:
         plot_imbalance(cd, schedule=["ref", "default"], **kwargs)
 
     # Since a building is always solved in one solver instance for the ADMM algorithm, its individual imbalance is
     # small, though. A solver with a large primal feasibility tolerance could, however, yield larger imbalances.
     if do_plot:
         plot_imbalance(bd1, schedule=["ref", "default"], **kwargs)
 
-
     # If required, the schedules can also be saved as .json or .csv files:
     save_schedule = do_plot
 
     if save_schedule:
         entities = list(cd.get_all_entities())
-        schedule_to_csv(entities, file_name="example_19", schedule=["ref", "default"])
-        schedule_to_json(entities, file_name="example_19", schedule=["ref", "default"])
+        schedule_to_csv(entities, file_name="example_22", schedule=["ref", "default"])
+        schedule_to_json(entities, file_name="example_22", schedule=["ref", "default"])
 
         # Plot the city district hierarchy and its lower-level devices into the current directory:
         plot_entity_directory(cd, ["ref", "default"], levels=2)
     return
 
 
 # Conclusions:
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/example_21_post-processing_metrics_evaluation.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/example_23_post-processing_metrics_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -33,15 +33,15 @@
 
 # This is a simple power scheduling example using the central optimization algorithm in order to demonstrate the
 # capabilities of the pycity_scheduling framework when it comes to the evaluation of metrics. The evaluation of metrics
 # is usually an important post-processing step.
 
 
 def main(do_plot=False):
-    print("\n\n------ Example 21: Post-Processing Metrics Evaluation ------\n\n")
+    print("\n\n------ Example 23: Post-Processing Metrics Evaluation ------\n\n")
 
     # Use a standard environment of 24 hours with hourly resolution (=60min=3600sec):
     env = factory.generate_standard_environment(step_size=3600, op_horizon=24)
 
     # Make it "attractive" for the consumers to shift demand into the second half of the scheduling period:
     env.prices.tou_prices = np.array([20]*12 + [10]*12)
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/examples/illustrative_code_example_cost_minimization_use_case_interactive.ipynb` & `pycity_scheduling-1.2.0/src/pycity_scheduling/examples/case_studies/illustrative_code_example_cost_minimization_use_case_interactive.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991319444444444%*

 * *Differences: {"'cells'": '{4: {\'source\': {insert: [(0, \'"""\\n\'), (1, \'The pycity_scheduling '*

 * *            "framework\\n'), (2, '\\n'), (3, '\\n'), (4, 'Copyright (C) 2023,\\n'), (5, 'Institute "*

 * *            "for Automation of Complex Power Systems (ACS),\\n'), (6, 'E.ON Energy Research Center "*

 * *            "(E.ON ERC),\\n'), (7, 'RWTH Aachen University\\n'), (8, '\\n'), (9, 'Permission is "*

 * *            'hereby granted, free of charge, to any person obtaining a copy of this software and '*

 * *            'associated\\n […]*

```diff
@@ -34,14 +34,38 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "\"\"\"\n",
+                "The pycity_scheduling framework\n",
+                "\n",
+                "\n",
+                "Copyright (C) 2023,\n",
+                "Institute for Automation of Complex Power Systems (ACS),\n",
+                "E.ON Energy Research Center (E.ON ERC),\n",
+                "RWTH Aachen University\n",
+                "\n",
+                "Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated\n",
+                "documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the\n",
+                "rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit\n",
+                "persons to whom the Software is furnished to do so, subject to the following conditions:\n",
+                "\n",
+                "The above copyright notice and this permission notice shall be included in all copies or substantial portions of the\n",
+                "Software.\n",
+                "\n",
+                "THE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE\n",
+                "WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\n",
+                "COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR\n",
+                "OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+                "\"\"\"\n",
+                "\n",
+                "\n",
                 "import matplotlib.pyplot as plt\n",
                 "from pycity_scheduling.classes import *\n",
                 "from pycity_scheduling.algorithms import *"
             ]
         },
         {
             "cell_type": "code",
@@ -59,15 +83,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "fi = FixedLoad(environment=e, method=1, annual_demand=3000.0, profile_type=\"H0\")\n",
                 "pv = Photovoltaic(environment=e, method=1, peak_power=6.0)\n",
-                "ba = Battery(environment=e, e_el_max=8.4, p_el_max_charge=3.6, p_el_max_discharge=3.6)"
+                "ba = Battery(environment=e, e_el_max=8.4, p_el_max_charge=3.6, p_el_max_discharge=3.6, eta=1.0)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/exceptions.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/solvers.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/solvers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -20,37 +20,35 @@
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
 # Specify different third-party mathematical programming solvers and solver options:
 
-BONMIN_SOLVER = "bonmin"
-BONMIN_SOLVER_OPTIONS = {'solve': {'options': {'bonmin.algorithm': 'b-hyb',
-                                               'bonmin.allowable_gap': 1e-10,
-                                               'bonmin.allowable_fraction_gap': 1e-4}}}
-
-CPLEX_SOLVER = "cplex"
-CPLEX_SOLVER_OPTIONS = {'solve': {'options': {}}}
-
-GLPK_SOLVER = "glpk"
-GLPK_SOLVER_OPTIONS = {'solve': {'options': {}}}
-
 GUROBI_DIRECT_SOLVER = "gurobi_direct"
 GUROBI_DIRECT_SOLVER_OPTIONS = {'solve': {'options': {'OutputFlag': 0,
                                                       'LogToConsole': 0,
                                                       'Logfile': "",
-                                                      "Method": 1}}}
+                                                      "Method": -1}}}
 
 GUROBI_PERSISTENT_SOLVER = "gurobi_persistent"
 GUROBI_PERSISTENT_SOLVER_OPTIONS = {'solve': {'options': {'OutputFlag': 0,
                                                           'LogToConsole': 0,
                                                           'Logfile': "",
-                                                          "Method": 1}}}
+                                                          "Method": -1}}}
 
 SCIP_SOLVER = "scip"
 SCIP_SOLVER_OPTIONS = {'solve': {'options': {}}}
 
+BONMIN_SOLVER = "couenne"
+BONMIN_SOLVER_OPTIONS = {'solve': {'options': {}}}
+
+CPLEX_SOLVER = "cplex"
+CPLEX_SOLVER_OPTIONS = {'solve': {'options': {}}}
+
+GLPK_SOLVER = "glpk"
+GLPK_SOLVER_OPTIONS = {'solve': {'options': {}}}
+
 
 # Set the default mathematical programming solver to be used by the pycity_scheduling framework:
 DEFAULT_SOLVER = GUROBI_DIRECT_SOLVER
 DEFAULT_SOLVER_OPTIONS = GUROBI_DIRECT_SOLVER_OPTIONS
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/testing/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_algorithms.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -41,15 +41,15 @@
 
         bd1 = Building(e, objective='peak-shaving')
         cd.addEntity(bd1, [0, 0])
         bes = BuildingEnergySystem(e)
         bd1.addEntity(bes)
         ths = ThermalHeatingStorage(e, 40, 0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(e, 10)
+        eh = ElectricHeater(e, 10)
         bes.addDevice(eh)
         ap = Apartment(e)
         bd1.addEntity(ap)
         load = np.array([10, 10])
         fi = FixedLoad(e, method=0, demand=load)
         ap.addEntity(fi)
         sh = SpaceHeating(e, method=0, loadcurve=load)
@@ -57,25 +57,25 @@
 
         bd2 = Building(e, objective='peak-shaving')
         cd.addEntity(bd2, [0, 0])
         bes = BuildingEnergySystem(e)
         bd2.addEntity(bes)
         ths = ThermalHeatingStorage(e, 40, 0.5)
         bes.addDevice(ths)
-        eh = ElectricalHeater(e, 20)
+        eh = ElectricHeater(e, 20)
         bes.addDevice(eh)
         ap = Apartment(e)
         bd2.addEntity(ap)
         load = np.array([20, 20])
         fi = FixedLoad(e, method=0, demand=load)
         ap.addEntity(fi)
         sh = SpaceHeating(e, method=0, loadcurve=load)
         ap.addEntity(sh)
 
-        wec = WindEnergyConverter(e, [50, 50], [0, 0], force_renewables=False)
+        wec = WindEnergyConverter(e, np.array([50, 50]), np.array([0, 0]), force_renewables=False)
         cd.addEntity(wec, [0, 0])
 
         pv = Photovoltaic(e, method=1, peak_power=4.6, force_renewables=False)
         cd.addEntity(pv, [0, 0])
 
         self.timer = t
         self.cd = cd
@@ -98,18 +98,14 @@
         self.assertGreater(1, r["s_norms"][-1])
 
         # Test infeasible model:
         self.bd1.model.new_constr = pyomo.Constraint(expr=self.bd1.model.p_el_vars[0] == 0)
         self.bd1.model.p_el_vars[0].setub(15.0)
         with self.assertRaises(NonoptimalError):
             f.solve(full_update=True, debug=False)
-
-        f2 = algorithms['exchange-admm'](self.cd, rho=2, eps_primal=0.001, max_iterations=2)
-        with self.assertRaises(MaxIterationError):
-            f2.solve()
         return
 
     def test_exchange_admm_beta(self):
         t = Timer(op_horizon=2)
         p = Prices(t)
         w = Weather(t)
         e = Environment(t, w, p)
@@ -125,15 +121,15 @@
         fi = FixedLoad(e, method=0, demand=load)
         ap.addEntity(fi)
 
         bd2 = Building(e, objective='peak-shaving')
         cd.addEntity(bd2, [0, 0])
         bes = BuildingEnergySystem(e)
         bd2.addEntity(bes)
-        bat = Battery(e, 100, 100, storage_end_equality=True)
+        bat = Battery(e, 100, 100, eta=1.0, storage_end_equality=True)
         bes.addDevice(bat)
 
         f = algorithms['exchange-admm'](cd, rho=2, eps_primal=0.001, eps_dual=0.01)
         r = f.solve()
         self.assertAlmostEqual(10, bd1.p_el_schedule[0], 4)
         self.assertAlmostEqual(-10, bd1.p_el_schedule[1], 4)
         self.assertAlmostEqual(-5, bd2.p_el_schedule[0], 2)
@@ -154,14 +150,37 @@
         self.assertAlmostEqual(-10, bd1.p_el_schedule[1], 4)
         self.assertAlmostEqual(0, bd2.p_el_schedule[0], 2)
         self.assertAlmostEqual(0, bd2.p_el_schedule[1], 2)
         self.assertAlmostEqual(10, cd.p_el_schedule[0], 2)
         self.assertAlmostEqual(-10, cd.p_el_schedule[1], 2)
         return
 
+    def test_exchange_miqp_admm(self):
+        # Exchange MIQP ADMM constrained:
+        f = algorithms['exchange-miqp-admm'](self.cd, rho=2.0, eps_primal=0.001, eps_dual=0.01,
+                                             x_update_mode='constrained', mode="integer")
+        r = f.solve()
+
+        self.assertAlmostEqual(20, self.bd1.p_el_schedule[0], 4)
+        self.assertAlmostEqual(20, self.bd1.p_el_schedule[1], 4)
+        self.assertAlmostEqual(40, self.bd2.p_el_schedule[0], 4)
+        self.assertAlmostEqual(40, self.bd2.p_el_schedule[1], 4)
+        self.assertAlmostEqual(60, self.cd.p_el_schedule[0], 2)
+        self.assertAlmostEqual(60, self.cd.p_el_schedule[1], 2)
+
+        self.assertGreater(0.001, r["r_norms"][-1])
+        self.assertGreater(0.01, r["s_norms"][-1])
+
+        # Test infeasible model:
+        self.bd1.model.new_constr = pyomo.Constraint(expr=self.bd1.model.p_el_vars[0] == 0)
+        self.bd1.model.p_el_vars[0].setub(15.0)
+        with self.assertRaises(NonoptimalError):
+            f.solve(full_update=True, debug=False)
+        return
+
     def test_dual_decomposition(self):
         f = algorithms['dual-decomposition'](self.cd, eps_primal=0.001)
         f.solve()
 
         self.assertAlmostEqual(20, self.bd1.p_el_schedule[0], 4)
         self.assertAlmostEqual(20, self.bd1.p_el_schedule[1], 4)
         self.assertAlmostEqual(40, self.bd2.p_el_schedule[0], 4)
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_all_classes.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_all_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -42,24 +42,24 @@
         ths = ThermalHeatingStorage(e, 1000, 0.5)
         bes.addDevice(ths)
         tcs = ThermalCoolingStorage(e, 500, 0.75)
         bes.addDevice(tcs)
         bat = Battery(e, 10, 10)
         bes.addDevice(bat)
         bl = Boiler(e, 10, 1)
-        eh = ElectricalHeater(e, 10)
+        eh = ElectricHeater(e, 10)
         hp = HeatPump(e, 10)
         chp = CombinedHeatPower(e, 10, 10, 0.5)
         ch = Chiller(e, 12)
         bes.addMultipleDevices([bl, eh, hp, chp, ch])
         ap = Apartment(e)
         bd.addEntity(ap)
         fl = FixedLoad(e, method=1, annual_demand=6000, profile_type='H0')
         sh = SpaceHeating(e, method=1, living_area=100, specific_demand=50, profile_type='HEF')
         sc = SpaceCooling(e, method=0, loadcurve=sh.loadcurve)
         ap.addMultipleEntities([fl, sh, sc])
-        ev = ElectricalVehicle(e, 10, 10, soc_init=1, charging_time=[1]*48+[0]*48)
+        ev = ElectricVehicle(e, 10, 10, soc_init=1, charging_time=[1]*48+[0]*48)
         ap.addEntity(ev)
         cl = CurtailableLoad(e, 0.1, 0.5)
         dl = DeferrableLoad(e, 10, 10, [1]*96)
         ap.addMultipleEntities([cl, dl])
         return
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_classes.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -71,54 +71,60 @@
         return
 
     def test_populate_model(self):
         model = pyomo.ConcreteModel()
         self.bat.populate_model(model)
         model.c1 = pyomo.Constraint(expr=self.bat.model.e_el_vars[2] == 10)
         model.c2 = pyomo.Constraint(expr=self.bat.model.e_el_vars[0] == 5)
-        obj = pyomo.sum_product(self.bat.model.p_el_demand_vars, self.bat.model.p_el_demand_vars)
+        obj = 0
+        for t in range(len(self.bat.model.p_el_demand_vars)):
+            obj += self.bat.model.p_el_demand_vars[t] * self.bat.model.p_el_demand_vars[t]
         model.o = pyomo.Objective(expr=obj)
         result = solve_model(model)
 
         # TODO stats are currently not correct due to a pyomo bug
         # use result as a workaround
         #model.compute_statistics()
         #stats = model.statistics
         #self.assertEqual(12, stats.number_of_variables)
         self.assertEqual(13, result.Problem[0].number_of_variables)
-        var_sum = pyomo.value(pyomo.quicksum(self.bat.model.p_el_vars[t] for t in range(1, 3)))
+        var_sum = pyomo.value(sum(self.bat.model.p_el_vars[t] for t in range(1, 3)))
         self.assertAlmostEqual(40, var_sum, places=5)
-        var_sum = pyomo.value(pyomo.quicksum(
+        var_sum = pyomo.value(sum(
             self.bat.model.p_el_supply_vars[t] + self.bat.model.p_el_demand_vars[t] for t in range(1, 3)
         ))
         self.assertAlmostEqual(40, var_sum, places=5)
         return
 
     def test_update_model(self):
         model = pyomo.ConcreteModel()
         self.bat.populate_model(model)
         demand_var = self.bat.model.p_el_vars
         self.bat.update_model()
         model.c1 = pyomo.Constraint(expr=self.bat.model.e_el_vars[0] == 10)
-        obj = pyomo.sum_product(demand_var, demand_var)
+        obj = 0
+        for t in range(len(demand_var)):
+            obj += demand_var[t] * demand_var[t]
         model.o = pyomo.Objective(expr=obj)
         solve_model(model)
 
         self.assertAlmostEqual(10, pyomo.value(demand_var[0]), places=5)
         return
 
     def test_update_schedule(self):
         model = pyomo.ConcreteModel()
         self.bat.populate_model(model)
         self.bat.update_model()
         self.bat.model.p_el_demand_vars.setlb(3.0)
         self.bat.model.p_el_demand_vars.setub(3.0)
         self.bat.model.p_el_supply_vars.setlb(0.0)
         self.bat.model.p_el_supply_vars.setub(0.0)
-        obj = pyomo.sum_product(self.bat.model.p_el_demand_vars, self.bat.model.p_el_demand_vars)
+        obj = 0
+        for t in range(len(self.bat.model.p_el_demand_vars)):
+            obj += self.bat.model.p_el_demand_vars[t] * self.bat.model.p_el_demand_vars[t]
         model.o = pyomo.Objective(expr=obj)
         solve_model(model)
         self.bat.update_schedule()
         assert_equal_array(self.bat.p_el_schedule, [3] * 3)
         assert_equal_array(self.bat.e_el_schedule, 0.875 * 10 + np.arange(1, 4)*3*0.25*0.5)
         return
 
@@ -159,15 +165,15 @@
 
     def test_no_discharge(self):
         e = get_env(9, 9)
         model = pyomo.ConcreteModel()
         bat = Battery(e, 30, 10, p_el_max_discharge=0, soc_init=0.5, eta=1)
         bat.populate_model(model)
         bat.update_model()
-        model.o = pyomo.Objective(expr=pyomo.sum_product(bat.model.p_el_vars))
+        model.o = pyomo.Objective(expr=sum(bat.model.p_el_vars[t] for t in range(len(bat.model.p_el_vars))))
         solve_model(model)
         bat.update_schedule()
         assert_equal_array(bat.e_el_schedule, [15] * 9)
         assert_equal_array(bat.p_el_schedule, [0] * 9)
         assert_equal_array(bat.p_el_demand_schedule, [0] * 9)
         assert_equal_array(bat.p_el_supply_schedule, [0] * 9)
         return
@@ -310,15 +316,15 @@
 
         ap = Apartment(env)
         self.bd.addEntity(ap)
         loadcurve = np.array([15, 15, 10, 10])
         sh = SpaceHeating(env, loadcurve=loadcurve)
         ap.addEntity(sh)
 
-        eh = ElectricalHeater(env, 20)
+        eh = ElectricHeater(env, 20)
         bes.addDevice(eh)
 
         self.bd.populate_model(model, robustness=(3, 0.5))
         self.bd.update_model(robustness=(3, 0.5))
         assert_equal_array(np.array([self.bd.model.lower_robustness_bounds[i].value for i in range(3)]),
                            np.cumsum(loadcurve[:3])*0.5/4)
         assert_equal_array(np.array([self.bd.model.upper_robustness_bounds[i].value for i in range(3)]),
@@ -332,15 +338,15 @@
         env = self.bd.environment
         bes = BuildingEnergySystem(env)
         self.bd.addEntity(bes)
         schedules = list(self.bd.schedules.keys())
         model = pyomo.ConcreteModel()
         self.bd.populate_model(model)
         self.bd.update_model()
-        model.o = pyomo.Objective(expr=pyomo.sum_product(self.bd.model.p_el_vars))
+        model.o = pyomo.Objective(expr=sum(self.bd.model.p_el_vars[t] for t in range(len(self.bd.model.p_el_vars))))
         solve_model(model)
         self.assertEqual(schedules, list(self.bd.schedules.keys()))
         self.bd.update_schedule()
         self.assertEqual(schedules, list(self.bd.schedules.keys()))
         self.bd.schedules["ref"]["p_el"] = np.arange(8)
         self.bd.copy_schedule("new", "ref")
         schedules.append("new")
@@ -389,16 +395,18 @@
 
     def test_lower_activation(self):
         e = get_env(4, 8)
         ch = Chiller(e, 10, cop=np.full(8, 11), lower_activation_limit=0.5)
         m = pyomo.ConcreteModel()
         ch.populate_model(m, "integer")
         ch.update_model("integer")
-        obj = pyomo.sum_product(ch.model.p_th_cool_vars, ch.model.p_th_cool_vars)
-        obj += 2 * 3 * pyomo.sum_product(ch.model.p_th_cool_vars)
+        obj = 0
+        for t in range(len(ch.model.p_th_cool_vars)):
+            obj += ch.model.p_th_cool_vars[t] * ch.model.p_th_cool_vars[t]
+        obj += 2 * 3 * sum(ch.model.p_th_cool_vars[t] for t in range(len(ch.model.p_th_cool_vars)))
         m.o = pyomo.Objective(expr=obj)
         solve_model(m)
         ch.update_schedule()
         assert_equal_array(ch.p_th_cool_schedule[:4], [-5] * 4)
         return
 
 
@@ -412,27 +420,27 @@
         self.e = get_env(5, 20)
         return
 
     def test_populate_model(self):
         model = pyomo.ConcreteModel()
         cl = CurtailableLoad(self.e, 2, 0.5)
         cl.populate_model(model)
-        obj = pyomo.sum_product(cl.model.p_el_vars)
+        obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
         model.o = pyomo.Objective(expr=obj)
         solve_model(model)
         cl.update_schedule()
         self.assertAlmostEqual(5, pyomo.value(obj))
         self.assertTrue(5, sum(cl.p_el_schedule[:5]))
         return
 
     def test_populate_model_on_off(self):
         model = pyomo.ConcreteModel()
         cl = CurtailableLoad(self.e, 2, 0.5, 2, 2)
         cl.populate_model(model)
-        obj = pyomo.sum_product(cl.model.p_el_vars)
+        obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
         model.o = pyomo.Objective(expr=obj)
         solve_model(model)
         cl.update_schedule()
         self.assertAlmostEqual(7, pyomo.value(obj))
         self.assertAlmostEqual(7, sum(cl.p_el_schedule[:5]))
         return
 
@@ -440,15 +448,15 @@
         for low, full in self.combinations:
             min_states = sum(np.tile([False]*low + [True]*full, 5)[:5])
             for nom in [0.5, 1, 2]:
                 with self.subTest(msg="max_low={} min_full={} nom={}".format(low, full, nom)):
                     model = pyomo.ConcreteModel()
                     cl = CurtailableLoad(self.e, nom, 0.75, low, full)
                     cl.populate_model(model, mode="integer")
-                    obj = pyomo.sum_product(cl.model.p_el_vars)
+                    obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
                     model.o = pyomo.Objective(expr=obj)
                     results = solve_model(model)
                     cl.update_schedule()
                     schedule_states = np.isclose(cl.p_el_schedule[:5], [nom]*5)
                     assert_equal_array(cl.p_state_schedule[:5], schedule_states)
                     self.assertEqual(min_states, sum(schedule_states))
                     self.assertAlmostEqual(min_states*nom+(5-min_states)*nom*0.75, pyomo.value(obj))
@@ -456,15 +464,15 @@
 
     def test_update_model(self):
         for width in [1, 2, 4, 5]:
             with self.subTest(msg="step width={}".format(width)):
                 model = pyomo.ConcreteModel()
                 cl = CurtailableLoad(self.e, 2, 0.5)
                 cl.populate_model(model)
-                obj = pyomo.sum_product(cl.model.p_el_vars)
+                obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
                 model.o = pyomo.Objective(expr=obj)
                 solve_model(model)
                 for t in range(0, 20-5+1, width):
                     self.e.timer.current_timestep = t
                     cl.update_model()
                     solve_model(model)
                     cl.update_schedule()
@@ -475,15 +483,15 @@
     def test_update_model_on_off(self):
         for low, full in self.combinations:
             for width in [1, 2, 4, 5]:
                 with self.subTest(msg="max_low={} min_full={} step width={}".format(low, full, width)):
                     model = pyomo.ConcreteModel()
                     cl = CurtailableLoad(self.e, 2, 0.5, low, full)
                     cl.populate_model(model)
-                    obj = pyomo.sum_product(cl.model.p_el_vars)
+                    obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
                     model.o = pyomo.Objective(expr=obj)
                     solve_model(model)
                     for t in range(0, 20-5+1, width):
                         self.e.timer.current_timestep = t
                         cl.update_model()
                         solve_model(model)
                         cl.update_schedule()
@@ -500,26 +508,30 @@
         for low, full in self.combinations:
             states = np.tile([False] * low + [True] * full, 20)[:20]
             for width in [1, 2, 4, 5]:
                 with self.subTest(msg="max_low={} min_full={} step width={}".format(low, full, width)):
                     model = pyomo.ConcreteModel()
                     cl = CurtailableLoad(self.e, 2, 0.5, low, full)
                     cl.populate_model(model, mode="integer")
-                    obj = pyomo.sum_product(cl.model.p_el_vars)
+                    obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
                     for t in range(0, 20-5+1, width):
                         self.e.timer.current_timestep = t
                         cl.update_model(mode="integer")
                         model.o = pyomo.Objective(expr=obj)
                         results = solve_model(model)
                         self.assertEqual(results.solver.termination_condition, TerminationCondition.optimal)
                         best_obj = pyomo.value(obj)
                         model.o_constr = pyomo.Constraint(expr=best_obj == obj)
                         model.del_component("o")
-                        model.o = pyomo.Objective(expr=pyomo.sum_product(range(0, -cl.op_horizon, -1),
-                                                                         cl.model.p_el_vars))
+                        objective = 0
+                        count = 0
+                        for i in range(0, -cl.op_horizon, -1):
+                            objective += i * cl.model.p_el_vars[count]
+                            count += 1
+                        model.o = pyomo.Objective(expr=objective)
                         results = solve_model(model)
                         model.del_component("o")
                         model.del_component("o_constr")
                         self.assertEqual(results.solver.termination_condition, TerminationCondition.optimal)
                         cl.update_schedule()
                         schedule_states_el = np.isclose(cl.p_el_schedule[t:t+5], [2] * 5)
                         schedule_states_b = np.isclose(cl.p_state_schedule[t:t+5], [1] * 5)
@@ -566,15 +578,15 @@
             for horizon in [1, 2, 4]:
                 if horizon >= width:
                     with self.subTest(msg="width={} horizon={}".format(width, horizon)):
                         e = get_env(horizon, 20)
                         model = pyomo.ConcreteModel()
                         cl = CurtailableLoad(e, 2, 0.5)
                         cl.populate_model(model)
-                        obj = pyomo.sum_product(cl.model.p_el_vars)
+                        obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
                         model.o = pyomo.Objective(expr=obj)
                         for t in range(0, 21 - horizon, width):
                             e.timer.current_timestep = t
                             cl.update_model()
                             solve_model(model)
                             self.assertEqual(1, pyomo.value(cl.model.p_el_vars[0]))
                             cl.update_schedule()
@@ -589,15 +601,15 @@
                     for low, full in self.combinations:
                         with self.subTest(msg="width={} horizon={} max_low={} min_full={}"
                                               .format(width, horizon, low, full)):
 
                             model = pyomo.ConcreteModel()
                             cl = CurtailableLoad(e, 2, 0.5, low, full)
                             cl.populate_model(model)
-                            obj = pyomo.sum_product(cl.model.p_el_vars)
+                            obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
                             model.c = pyomo.Objective(expr=obj)
                             for t in range(0, 21 - horizon, width):
                                 e.timer.current_timestep = t
                                 cl.update_model()
                                 solve_model(model)
                                 cl.update_schedule()
 
@@ -614,26 +626,30 @@
                 if horizon >= width:
                     for low, full in self.combinations:
                         with self.subTest(msg="width={} horizon={} max_low={} min_full={}".format(width, horizon, low, full)):
                             states = np.tile([1] * low + [2] * full, 20)[:20]
                             model = pyomo.ConcreteModel()
                             cl = CurtailableLoad(e, 2, 0.5, low, full)
                             cl.populate_model(model, mode="integer")
-                            obj = pyomo.sum_product(cl.model.p_el_vars)
+                            obj = sum(cl.model.p_el_vars[t] for t in range(len(cl.model.p_el_vars)))
                             for t in range(0, 21 - horizon, width):
                                 e.timer.current_timestep = t
                                 cl.update_model(mode="integer")
                                 model.o = pyomo.Objective(expr=obj)
                                 results = solve_model(model)
                                 self.assertEqual(results.solver.termination_condition, TerminationCondition.optimal)
                                 best_obj = pyomo.value(obj)
                                 model.o_constr = pyomo.Constraint(expr=best_obj == obj)
                                 model.del_component("o")
-                                model.o = pyomo.Objective(expr=pyomo.sum_product(range(-1, -cl.op_horizon-1, -1),
-                                                                                 cl.model.p_el_vars))
+                                objective = 0
+                                count = 0
+                                for i in range(-1, -cl.op_horizon-1, -1):
+                                    objective += i * cl.model.p_el_vars[count]
+                                    count += 1
+                                model.o = pyomo.Objective(expr=objective)
                                 results = solve_model(model)
                                 model.del_component("o")
                                 model.del_component("o_constr")
                                 self.assertEqual(results.solver.termination_condition, TerminationCondition.optimal)
                                 cl.update_schedule()
 
                             assert_equal_array(cl.p_el_schedule, states)
@@ -778,16 +794,18 @@
 
     def test_lower_activation(self):
         e = get_env(4, 8)
         chp = CombinedHeatPower(e, 10, 10, 0.8, 0.5)
         m = pyomo.ConcreteModel()
         chp.populate_model(m, "integer")
         chp.update_model("integer")
-        obj = pyomo.sum_product(chp.model.p_el_vars, chp.model.p_el_vars)
-        obj += 2*3 * pyomo.sum_product(chp.model.p_el_vars)
+        obj = 0
+        for t in range(len(chp.model.p_el_vars)):
+            obj += chp.model.p_el_vars[t] * chp.model.p_el_vars[t]
+        obj += 2*3 * sum(chp.model.p_el_vars[t] for t in range(len(chp.model.p_el_vars)))
         m.o = pyomo.Objective(expr=obj)
         solve_model(m)
         chp.update_schedule()
         assert_equal_array(chp.p_el_schedule[:4], [-5]*4)
         return
 
     def test_bounds(self):
@@ -821,20 +839,23 @@
         return
 
     def test_update_model(self):
         with self.assertWarns(UserWarning):
             dl = DeferrableLoad(self.e, 19, 10, load_time=self.lt)
         model = pyomo.ConcreteModel()
         dl.populate_model(model)
-        obj = pyomo.sum_product(dl.model.p_el_vars, dl.model.p_el_vars)
+        obj = 0
+        for t in range(len(dl.model.p_el_vars)):
+            obj += dl.model.p_el_vars[t] * dl.model.p_el_vars[t]
         model.o = pyomo.Objective(expr=obj)
         dl.update_model()
         solve_model(model)
 
-        self.assertAlmostEqual(10, pyomo.value(pyomo.sum_product(dl.model.p_el_vars)) * dl.time_slot, places=5)
+        self.assertAlmostEqual(10, pyomo.value(sum(dl.model.p_el_vars[t] for t in range(len(dl.model.p_el_vars))))
+                               * dl.time_slot, places=5)
 
         dl.timer.mpc_update()
         dl.update_model()
         solve_model(model)
 
         for t, c in enumerate(self.lt[1:7]):
             if c == 1:
@@ -848,25 +869,25 @@
 
     def test_infeasible_consumption(self):
         with self.assertWarns(UserWarning):
             feasible = DeferrableLoad(self.e, 10, 10, load_time=self.lt)
         m = pyomo.ConcreteModel()
         feasible.populate_model(m)
         feasible.update_model()
-        obj = pyomo.sum_product(feasible.model.p_el_vars)
+        obj = sum(feasible.model.p_el_vars[t] for t in range(len(feasible.model.p_el_vars)))
         m.o = pyomo.Objective(expr=obj)
         results = solve_model(m)
         self.assertEqual(results.solver.termination_condition, TerminationCondition.optimal)
 
         m = pyomo.ConcreteModel()
         with self.assertWarns(UserWarning):
             infeasible = DeferrableLoad(self.e, 10, 10.6, load_time=self.lt)
         infeasible.populate_model(m)
         infeasible.update_model()
-        obj = pyomo.sum_product(infeasible.model.p_el_vars)
+        obj = sum(infeasible.model.p_el_vars[t] for t in range(len(infeasible.model.p_el_vars)))
         m.o = pyomo.Objective(expr=obj)
         logger = logging.getLogger("pyomo.core")
         oldlevel = logger.level
         logger.setLevel(logging.ERROR)
         results = solve_model(m)
         logger.setLevel(oldlevel)
         self.assertEqual(results.solver.termination_condition, TerminationCondition.infeasible)
@@ -874,15 +895,18 @@
 
     def test_update_model_integer(self):
         with self.assertWarns(UserWarning):
             dl = DeferrableLoad(self.e, 19, 9.5, load_time=self.lt)
         m = pyomo.ConcreteModel()
         dl.populate_model(m, mode="integer")
 
-        obj = pyomo.sum_product([0] * 2 + [1] * 2 + [0] * 2, dl.model.p_el_vars, dl.model.p_el_vars)
+        coeff = [0] * 2 + [1] * 2 + [0] * 2
+        obj = 0
+        for t in range(len(dl.model.p_el_vars)):
+            obj += coeff[t] * dl.model.p_el_vars[t] * dl.model.p_el_vars[t]
         m.o = pyomo.Objective(expr=obj)
         with self.assertWarns(UserWarning):
             dl.update_model(mode="integer")
         results = solve_model(m)
         self.assertEqual(results.solver.termination_condition, TerminationCondition.optimal)
         dl.update_schedule()
 
@@ -904,43 +928,43 @@
     def test_infeasible_integer(self):
         e = get_env(1, 9)
         model = pyomo.ConcreteModel()
         with self.assertWarns(UserWarning):
             dl = DeferrableLoad(e, 19, 9.5, load_time=self.lt)
             dl.populate_model(model, mode="integer")
             dl.update_model(mode="integer")
-        obj = pyomo.sum_product(dl.model.p_el_vars)
+        obj = sum(dl.model.p_el_vars[t] for t in range(len(dl.model.p_el_vars)))
         model.o = pyomo.Objective(expr=obj)
         logger = logging.getLogger("pyomo.core")
         oldlevel = logger.level
         logger.setLevel(logging.ERROR)
         results = solve_model(model)
         logger.setLevel(oldlevel)
         self.assertEqual(results.solver.termination_condition, TerminationCondition.infeasible)
 
         model = pyomo.ConcreteModel()
         with self.assertWarns(UserWarning):
             dl = DeferrableLoad(self.e, 19, 19, load_time=self.lt)
             dl.populate_model(model, mode="integer")
             dl.update_model(mode="integer")
-        obj = pyomo.sum_product(dl.model.p_el_vars)
+        obj = sum(dl.model.p_el_vars[t] for t in range(len(dl.model.p_el_vars)))
         model.o = pyomo.Objective(expr=obj)
         logger = logging.getLogger("pyomo.core")
         oldlevel = logger.level
         logger.setLevel(logging.ERROR)
         results = solve_model(model)
         logger.setLevel(oldlevel)
         self.assertEqual(results.solver.termination_condition, TerminationCondition.infeasible)
 
         model = pyomo.ConcreteModel()
         with self.assertWarns(UserWarning):
             dl = DeferrableLoad(self.e, 19, 19*3/4, load_time=self.lt)
             dl.populate_model(model, mode="integer")
             dl.update_model(mode="integer")
-        obj = pyomo.sum_product(dl.model.p_el_vars)
+        obj = sum(dl.model.p_el_vars[t] for t in range(len(dl.model.p_el_vars)))
         model.o = pyomo.Objective(expr=obj)
         results = solve_model(model)
         self.assertEqual(results.solver.termination_condition, TerminationCondition.optimal)
         dl.update_schedule()
         assert_equal_array(dl.p_el_schedule[:6], [0, 19, 19, 19, 0, 0])
         return
 
@@ -968,15 +992,15 @@
     def test_populate_model(self):
         e = get_env(2, 4)
         load = np.arange(1, 5)
         model = pyomo.ConcreteModel()
         self.fl = FixedLoad(e, method=0, demand=load)
         self.fl.populate_model(model)
         self.fl.update_model()
-        model.o = pyomo.Objective(expr=pyomo.sum_product(self.fl.model.p_el_vars))
+        model.o = pyomo.Objective(expr=sum(self.fl.model.p_el_vars[t] for t in range(len(self.fl.model.p_el_vars))))
         solve_model(model)
         for t in range(2):
             self.assertEqual(self.fl.model.p_el_vars[t].value, load[t])
         return
 
     def test_unit_conversion(self):
         ti = Timer(step_size=1800,
@@ -1160,37 +1184,39 @@
         model.o = pyomo.Objective(expr=obj)
         solve_model(model)
 
         self.assertAlmostEqual(3, pyomo.value(obj), 4)
         return
 
 
-class TestElectricalHeater(unittest.TestCase):
+class TestElectricHeater(unittest.TestCase):
     def setUp(self):
         e = get_env(4, 8)
-        self.eh = ElectricalHeater(e, 10, 10, 0.8)
+        self.eh = ElectricHeater(e, 10, 10, 0.8)
         return
 
     def test_lower_activation(self):
         e = get_env(4, 8)
-        eh = ElectricalHeater(e, 10, lower_activation_limit=0.5)
+        eh = ElectricHeater(e, 10, lower_activation_limit=0.5)
         m = pyomo.ConcreteModel()
         eh.populate_model(m, "integer")
         eh.update_model("integer")
-        obj = pyomo.sum_product(eh.model.p_el_vars, eh.model.p_el_vars)
-        obj += -2 * 3 * pyomo.sum_product(eh.model.p_el_vars)
+        obj = 0
+        for t in range(len(eh.model.p_el_vars)):
+            obj += eh.model.p_el_vars[t] * eh.model.p_el_vars[t]
+        obj += -2 * 3 * sum(eh.model.p_el_vars[t] for t in range(len(eh.model.p_el_vars)))
         m.o = pyomo.Objective(expr=obj)
         solve_model(m)
         eh.update_schedule()
         assert_equal_array(eh.p_el_schedule[:4], [5] * 4)
         return
 
     def test_update_schedule(self):
         e = get_env(2, 2)
-        eh = ElectricalHeater(e, 10, lower_activation_limit=0.5)
+        eh = ElectricHeater(e, 10, lower_activation_limit=0.5)
         m = pyomo.ConcreteModel()
         eh.populate_model(m)
         eh.update_model()
         obj = eh.model.p_el_vars[0] - eh.model.p_el_vars[1]
         eh.model.p_el_vars[0].setlb(5.0)
         eh.model.p_el_vars[1].setub(0.05)
         m.o = pyomo.Objective(expr=obj)
@@ -1202,43 +1228,46 @@
         return
 
 
 class TestElectricVehicle(unittest.TestCase):
     def setUp(self):
         e = get_env(6, 9)
         self.ct = [1, 1, 1, 0, 0, 0, 1, 1, 1]
-        self.ev = ElectricalVehicle(e, 10, 20, p_el_max_discharge=20, soc_init=0.5, charging_time=self.ct)
+        self.ev = ElectricVehicle(e, 10, 20, p_el_max_discharge=20, soc_init=0.5, charging_time=self.ct,
+                                  simulate_driving=True, minimum_soc_end=1.0, eta=1.0)
         return
 
     def test_populate_model(self):
         model = pyomo.ConcreteModel()
         self.ev.populate_model(model)
         model.c1 = pyomo.Constraint(expr=self.ev.model.e_el_vars[2] == 10)
         model.c2 = pyomo.Constraint(expr=self.ev.model.e_el_vars[0] == 5)
-        obj = pyomo.sum_product(self.ev.model.p_el_demand_vars, self.ev.model.p_el_demand_vars)
+        obj = 0
+        for t in range(len(self.ev.model.p_el_demand_vars)):
+            obj += self.ev.model.p_el_demand_vars[t] * self.ev.model.p_el_demand_vars[t]
         model.o = pyomo.Objective(expr=obj)
         result = solve_model(model)
 
         self.assertEqual(31, result.Problem[0].number_of_variables)
-        var_sum = pyomo.value(pyomo.quicksum(self.ev.model.p_el_vars[t] for t in range(1, 6)))
+        var_sum = pyomo.value(sum(self.ev.model.p_el_vars[t] for t in range(1, 6)))
         self.assertAlmostEqual(20, var_sum, places=2)
-        var_sum = pyomo.value(pyomo.quicksum(
+        var_sum = pyomo.value(sum(
             self.ev.model.p_el_supply_vars[t] + self.ev.model.p_el_demand_vars[t] for t in range(1, 6)))
         self.assertAlmostEqual(20, var_sum, places=2)
         return
 
     def test_update_model(self):
         model = pyomo.ConcreteModel()
         self.ev.populate_model(model)
         self.ev.update_model()
         model.o = pyomo.Objective(expr=self.ev.get_objective())
         solve_model(model)
 
         self.assertAlmostEqual(10, self.ev.model.e_el_vars[2].value, places=5)
-        self.assertAlmostEqual(2, self.ev.model.e_el_vars[3].value, places=5)
+        self.assertAlmostEqual(10, self.ev.model.e_el_vars[3].value, places=5)
 
         self.ev.timer.mpc_update()
         self.ev.update_model()
         solve_model(model)
 
         for t, c in enumerate(self.ct[1:7]):
             if c:
@@ -1246,24 +1275,16 @@
                 self.assertEqual(20, self.ev.model.p_el_supply_vars[t].ub)
                 self.assertEqual(0, self.ev.model.p_el_drive_vars[t].ub)
             else:
                 self.assertEqual(0, self.ev.model.p_el_demand_vars[t].ub)
                 self.assertEqual(0, self.ev.model.p_el_supply_vars[t].ub)
                 self.assertIsNone(self.ev.model.p_el_drive_vars[t].ub)
         self.assertAlmostEqual(10, self.ev.model.e_el_vars[1].value, places=5)
-        self.assertAlmostEqual(2, self.ev.model.e_el_vars[2].value, places=5)
-        self.assertLessEqual(1.6, self.ev.model.e_el_vars[5].value)
-
-        self.ev.update_schedule()
-        self.ev.timer.mpc_update()
-        self.ev.timer.mpc_update()
-        self.ev.update_model()
-        solve_model(model)
-
-        self.assertAlmostEqual(10, self.ev.model.e_el_vars[5].value, places=5)
+        self.assertAlmostEqual(10, self.ev.model.e_el_vars[2].value, places=5)
+        self.assertLessEqual(3, self.ev.model.e_el_vars[5].value)
         return
 
     def test_get_objective(self):
         model = pyomo.ConcreteModel()
         self.ev.populate_model(model)
         self.ev.update_model()
 
@@ -1272,116 +1293,63 @@
             ref = (i + 1) / 21 * 6 * 11
             coeff = obj.args[i].args[0].args[0]
             self.assertAlmostEqual(ref, coeff, places=5)
         return
 
     def test_no_charge_time(self):
         e = get_env(6, 9)
-        ev = ElectricalVehicle(e, 37.0, 11.0)
+        ev = ElectricVehicle(e, 37.0, 11.0)
         assert_equal_array(ev.charging_time, [1]*9)
         e = get_env(28, 96*24-12)
-        ev = ElectricalVehicle(e, 37.0, 11.0)
+        ev = ElectricVehicle(e, 37.0, 11.0)
         assert_equal_array(ev.charging_time, np.tile([1] * 24 + [0] * 48 + [1] * 24, 24)[:-12])
         return
 
     def test_no_discharge(self):
         model = pyomo.ConcreteModel()
         e = get_env(6, 9)
-        ev = ElectricalVehicle(e, 10.0, 40.0, charging_time=self.ct)
+        ev = ElectricVehicle(e, 10.0, 40.0, charging_time=self.ct, simulate_driving=True, minimum_soc_end=1.0, eta=1.0)
         ev.populate_model(model)
         ev.update_model()
         model.o = pyomo.Objective(expr=ev.model.p_el_vars[0] + ev.model.p_el_vars[1])
         solve_model(model)
         ev.update_schedule()
         assert_equal_array(ev.p_el_schedule[:4], [0, 0, 5*4, 0])
         assert_equal_array(ev.p_el_demand_schedule[:4], [0, 0, 5 * 4, 0])
         assert_equal_array(ev.p_el_supply_schedule[:4], [0, 0, 0, 0])
-        assert_equal_array(ev.e_el_schedule[:4], [5, 5, 10, 2])
+        assert_equal_array(ev.e_el_schedule[:4], [5, 5, 10, 10])
 
         model = pyomo.ConcreteModel()
         e = get_env(6, 9)
-        ev = ElectricalVehicle(e, 10.0, 40.0, p_el_max_discharge=8, charging_time=self.ct)
+        ev = ElectricVehicle(e, 10.0, 40.0, p_el_max_discharge=8, charging_time=self.ct, simulate_driving=True,
+                             minimum_soc_end=1.0, eta=1.0)
         ev.populate_model(model)
         ev.update_model()
         model.o = pyomo.Objective(expr=ev.model.p_el_vars[0] + ev.model.p_el_vars[1])
         solve_model(model)
         ev.update_schedule()
-        assert_equal_array(ev.p_el_schedule[:4], [-8, -8, 9 * 4, 0])
-        assert_equal_array(ev.p_el_demand_schedule[:4], [0, 0, 9 * 4, 0])
-        assert_equal_array(ev.p_el_supply_schedule[:4], [8, 8, 0, 0])
-        assert_equal_array(ev.e_el_schedule[:4], [3, 1, 10, 2])
-        return
-
-    def test_partial_charge(self):
-        for step_size in [1, 2, 3, 6, 12]:
-            with self.subTest("step_size: {}".format(step_size)):
-                e = get_env(step_size, 12, step_size)
-                self.ct = [1, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0, 0]
-                self.ev = ElectricalVehicle(e, 10, 20, 0.5, charging_time=self.ct)
-                m = pyomo.ConcreteModel()
-                self.ev.populate_model(m)
-                m.o = pyomo.Objective(expr=pyomo.sum_product(
-                    self.ev.model.p_el_vars,
-                    self.ev.model.p_el_vars
-                ))
-                for i in range(0, 12, step_size):
-                    self.ev.update_model(m)
-                    solve_model(m)
-                    self.ev.update_schedule()
-                    e.timer.mpc_update()
-                assert_equal_array(self.ev.p_el_schedule, [5 / 3 * 4] * 3 + [0] * 3 + [8 / 3 * 4] * 3 + [0] * 3)
-
-        step_size = 12
-        e = get_env(step_size, 12, step_size)
-        self.ev = ElectricalVehicle(e, 10, 20, 20, soc_init=0.5, charging_time=self.ct)
-        m = pyomo.ConcreteModel()
-        self.ev.populate_model(m)
-        self.ev.update_model(m)
-        m.o = pyomo.Objective(expr=self.ev.model.p_el_vars[2] + self.ev.model.p_el_vars[7])
-        solve_model(m)
-        self.ev.update_schedule()
-        self.assertAlmostEqual(0, self.ev.p_el_schedule[2], 4)
-        self.assertAlmostEqual(-2 * 4, self.ev.p_el_schedule[7], 4)
+        assert_equal_array(ev.p_el_schedule[:4], [0, 0, 20, 0])
+        assert_equal_array(ev.p_el_demand_schedule[:4], [0, 8, 20, 0])
+        assert_equal_array(ev.p_el_supply_schedule[:4], [0, 8, 0, 0])
+        assert_equal_array(ev.e_el_schedule[:4], [5, 5, 10, 10])
         return
 
     def test_bad_charging_times(self):
         e = get_env(3, 12)
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always", UserWarning)
-            self.ev = ElectricalVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 1, 0, 0, 0, 1, 1, 1, 1, 0, 0])
-            self.assertEqual(0, len(w))
+        self.ev = ElectricVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 1, 0, 0, 0, 1, 1, 1, 1, 0, 0],
+                                  simulate_driving=True, minimum_soc_end=1.0, eta=1.0)
         with self.assertWarns(UserWarning):
-            self.ev = ElectricalVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0])
+            self.ev = ElectricVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0],
+                                      simulate_driving=True, minimum_soc_end=1.0, eta=1.0)
         with self.assertWarns(UserWarning):
-            self.ev = ElectricalVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 0, 0])
+            self.ev = ElectricVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 1, 0, 0, 0, 0, 1, 1, 1, 0, 0],
+                                      simulate_driving=True, minimum_soc_end=1.0, eta=1.0)
         with self.assertWarns(UserWarning):
-            self.ev = ElectricalVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 1, 0, 0, 1, 1, 1, 0, 1, 1, 1])
-        return
-
-    def test_inital_charging_times(self):
-        for step_size in [1, 2, 3, 6, 12]:
-            with self.subTest("step_size: {}".format(step_size)):
-                e = get_env(step_size, 12, step_size)
-                with warnings.catch_warnings(record=True) as w:
-                    warnings.simplefilter("always", UserWarning)
-                    self.ev = ElectricalVehicle(e, 10, 8, soc_init=0.8,
-                                                charging_time=[0, 1, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0])
-                    self.assertEqual(0, len(w))
-                m = pyomo.ConcreteModel()
-                self.ev.populate_model(m)
-                m.o = pyomo.Objective(expr=pyomo.sum_product(self.ev.model.p_el_vars, self.ev.model.p_el_vars))
-                for i in range(0, 12, step_size):
-                    self.ev.update_model(m)
-                    solve_model(m)
-                    self.ev.update_schedule()
-                    e.timer.mpc_update()
-                assert_equal_array(self.ev.p_el_schedule, [0, 8] + [0] * 4 + [8] * 4 + [0] * 2)
-                assert_equal_array(self.ev.p_el_demand_schedule, [0, 8] + [0] * 4 + [8] * 4 + [0] * 2)
-                assert_equal_array(self.ev.p_el_supply_schedule, [0] * 12)
-                assert_equal_array(self.ev.e_el_schedule, [8, 10] + [2] * 4 + [4, 6, 8, 10] + [2] * 2)
+            self.ev = ElectricVehicle(e, 10, 8, soc_init=0.5, charging_time=[1, 1, 1, 0, 0, 1, 1, 1, 0, 1, 1, 1],
+                                      simulate_driving=True, minimum_soc_end=1.0, eta=1.0)
         return
 
 
 class TestHeatPump(unittest.TestCase):
     def setUp(self):
         e = get_env(4, 8)
         self.hp = HeatPump(e, 10, cop=np.full(8, 11))
@@ -1406,16 +1374,18 @@
 
     def test_lower_activation(self):
         e = get_env(4, 8)
         hp = HeatPump(e, 10, lower_activation_limit=0.5)
         m = pyomo.ConcreteModel()
         hp.populate_model(m, "integer")
         hp.update_model("integer")
-        obj = pyomo.sum_product(hp.model.p_th_heat_vars, hp.model.p_th_heat_vars)
-        obj += 2 * 3 * pyomo.sum_product(hp.model.p_th_heat_vars)
+        obj = 0
+        for t in range(len(hp.model.p_th_heat_vars)):
+            obj += hp.model.p_th_heat_vars[t] * hp.model.p_th_heat_vars[t]
+        obj += 2 * 3 * sum(hp.model.p_th_heat_vars[t] for t in range(len(hp.model.p_th_heat_vars)))
         m.o = pyomo.Objective(expr=obj)
         solve_model(m)
         hp.update_schedule()
         assert_equal_array(hp.p_th_heat_schedule[:4], [-5] * 4)
         return
 
 
@@ -1486,15 +1456,16 @@
     def test_update_schedule(self):
         m = pyomo.ConcreteModel()
         self.tcs.populate_model(m)
         self.tcs.update_model()
         for t in range(3):
             self.tcs.model.p_th_cool_vars[t].setub(t)
             self.tcs.model.p_th_cool_vars[t].setlb(t)
-        m.o = pyomo.Objective(expr=pyomo.sum_product(self.tcs.model.p_th_cool_vars))
+        m.o = pyomo.Objective(expr=sum(self.tcs.model.p_th_cool_vars[t]
+                                       for t in range(len(self.tcs.model.p_th_cool_vars))))
         solve_model(m)
         a = np.arange(3)
 
         self.tcs.update_schedule()
         assert_equal_array(self.tcs.p_th_cool_schedule, a)
         assert_equal_array(self.tcs.e_th_cool_schedule, [20, 20.25, 20.75])
         return
@@ -1509,15 +1480,16 @@
     def test_update_schedule(self):
         m = pyomo.ConcreteModel()
         self.ths.populate_model(m)
         self.ths.update_model()
         for t in range(3):
             self.ths.model.p_th_heat_vars[t].setub(t)
             self.ths.model.p_th_heat_vars[t].setlb(t)
-        m.o = pyomo.Objective(expr=pyomo.sum_product(self.ths.model.p_th_heat_vars))
+        m.o = pyomo.Objective(expr=sum(self.ths.model.p_th_heat_vars[t]
+                                       for t in range(len(self.ths.model.p_th_heat_vars))))
         solve_model(m)
         a = np.arange(3)
 
         self.ths.update_schedule()
         assert_equal_array(self.ths.p_th_heat_schedule, a)
         assert_equal_array(self.ths.e_th_heat_schedule, [20, 20.25, 20.75])
         return
@@ -1533,15 +1505,16 @@
     def test_update_schedule(self):
         m = pyomo.ConcreteModel()
         self.tc.populate_model(m)
         self.tc.update_model()
         for t in range(4):
             self.tc.model.p_th_cool_vars[t].setub(t)
             self.tc.model.p_th_cool_vars[t].setlb(t)
-        m.o = pyomo.Objective(expr=pyomo.sum_product(self.tc.model.p_th_cool_vars))
+        m.o = pyomo.Objective(expr=sum(self.tc.model.p_th_cool_vars[t]
+                                       for t in range(len(self.tc.model.p_th_cool_vars))))
         solve_model(m)
         a = np.arange(4)
 
         self.tc.update_schedule()
         assert_equal_array(self.tc.p_th_cool_schedule[:4], a)
         self.tc.timer.mpc_update()
         self.tc.update_schedule()
@@ -1559,15 +1532,16 @@
     def test_update_schedule(self):
         m = pyomo.ConcreteModel()
         self.th.populate_model(m)
         self.th.update_model()
         for t in range(4):
             self.th.model.p_th_heat_vars[t].setub(t)
             self.th.model.p_th_heat_vars[t].setlb(t)
-        m.o = pyomo.Objective(expr=pyomo.sum_product(self.th.model.p_th_heat_vars))
+        m.o = pyomo.Objective(expr=sum(self.th.model.p_th_heat_vars[t]
+                                       for t in range(len(self.th.model.p_th_heat_vars))))
         solve_model(m)
         a = np.arange(4)
 
         self.th.update_schedule()
         assert_equal_array(self.th.p_th_heat_schedule[:4], a)
         self.th.timer.mpc_update()
         self.th.update_schedule()
@@ -1708,20 +1682,20 @@
                mpc_step_width=mpc_step_width)
     we = Weather(ti)
     pr = Prices(ti)
     return Environment(ti, we, pr)
 
 
 def assert_equal_array(a: np.ndarray, expected):
-    if not np.allclose(a, expected):
+    if not np.allclose(a, expected, rtol=1e-3, atol=1e-6):
         expected = np.array(expected)
         msg = "Array {} does not equal expected array {}".format(np.array2string(a), np.array2string(expected))
         raise AssertionError(msg)
 
 
 def solve_model(model):
     # hack to suppress pyomo no constraint warning
     if not hasattr(model, "simple_var"):
         model.simple_var = pyomo.Var(domain=pyomo.Reals, bounds=(None, None), initialize=0)
         model.simple_constr = pyomo.Constraint(expr=model.simple_var == 1)
     opt = pyomo.SolverFactory(solvers.DEFAULT_SOLVER)
-    return opt.solve(model)
+    return opt.solve(model, **solvers.DEFAULT_SOLVER_OPTIONS.get("solve", {}))
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_examples.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/testing/unit_tests/test_util.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/testing/unit_tests/test_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -54,37 +54,38 @@
         self.env = Environment(t, w, p)
         return
 
     def test_lower_activation_limit(self):
         ee = ElectricalEntity(self.env)
         m = pyomo.ConcreteModel()
         ee.populate_model(m, "integer")
-        o = pyomo.sum_product(ee.model.p_el_vars, ee.model.p_el_vars)
-        o -= 2 * 0.3 * pyomo.sum_product(ee.model.p_el_vars)
+        o = 0
+        for t in range(len(ee.model.p_el_vars)):
+            o += ee.model.p_el_vars[t] * ee.model.p_el_vars[t]
+        o -= 2 * 0.3 * sum(ee.model.p_el_vars[t] for t in range(len(ee.model.p_el_vars)))
         m.o = pyomo.Objective(expr=o)
         self.assertEqual(_get_constr_count(ee.model), 0)
         lal_constr = gen_constrs.LowerActivationLimit(ee, "p_el", 0.5, 1)
 
         lal_constr.apply(ee.model, "convex")
         self.assertEqual(_get_constr_count(ee.model), 0)
-        opt = pyomo.SolverFactory(solvers.DEFAULT_SOLVER)
-        opt.solve(m)
+        solve_model(m)
         ee.update_schedule()
         for i in ee.op_time_vec:
-            self.assertAlmostEqual(ee.p_el_schedule[i], 0.3, 4)
-            self.assertAlmostEqual(ee.p_el_state_schedule[i], 1.0, 4)
+            self.assertAlmostEqual(ee.p_el_schedule[i], 0.3, 3)
+            self.assertAlmostEqual(ee.p_el_state_schedule[i], 1.0, 3)
 
         lal_constr.apply(ee.model, "integer")
         self.assertEqual(_get_constr_count(ee.model), 12*2)
 
-        opt.solve(m)
+        solve_model(m)
         ee.update_schedule()
         for i in ee.op_time_vec:
-            self.assertAlmostEqual(ee.p_el_schedule[i], 0.5, 4)
-            self.assertAlmostEqual(ee.p_el_state_schedule[i], 1.0, 4)
+            self.assertAlmostEqual(ee.p_el_schedule[i], 0.5, 3)
+            self.assertAlmostEqual(ee.p_el_state_schedule[i], 1.0, 3)
         return
 
 
 class TestFactory(unittest.TestCase):
     def setUp(self):
         t = Timer()
         p = Prices(t)
@@ -313,120 +314,119 @@
 
     def test_value_extraction(self):
         v = pyomo.Var(domain=pyomo.Reals)
         with self.assertRaises(ValueError):
             util.extract_pyomo_values(v)
 
         m = pyomo.ConcreteModel()
-        opt = pyomo.SolverFactory(solvers.DEFAULT_SOLVER)
 
         m.v = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.v == 1.0)
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(1, e)
         self.assertIs(float, type(e))
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(pyomo.RangeSet(1, 2), domain=pyomo.Reals)
-        opt.solve(m)
+        solve_model(m)
 
         m.v[1].value = 1
         m.v[2].value = 2
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(0, e[0])
         self.assertEqual(0, e[1])
         self.assertEqual('f', e.dtype.kind)
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(domain=pyomo.Integers, bounds=(4, 5))
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(4, e)
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(domain=pyomo.Integers, bounds=(4.1, 4.3))
-        opt.solve(m)
+        solve_model(m)
         with self.assertRaises(SchedulingError):
             util.extract_pyomo_values(m.v)
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(pyomo.RangeSet(1, 2), domain=pyomo.Binary, bounds=(0.1, 0.9))
-        opt.solve(m)
+        solve_model(m)
         with self.assertRaises(SchedulingError):
             util.extract_pyomo_values(m.v)
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(domain=pyomo.Integers, bounds=(3.9, 4.3))
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(4, e)
         self.assertIs(int, type(e))
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(domain=pyomo.Integers)
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(0, e)
         self.assertIs(int, type(e))
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(domain=pyomo.Integers, bounds=(None, -5))
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(-5, e)
         self.assertIs(int, type(e))
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(domain=pyomo.Integers, bounds=(-10, -2))
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(-2, e)
         self.assertIs(int, type(e))
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(domain=pyomo.Integers, bounds=(2, 10))
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(2, e)
         self.assertIs(int, type(e))
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(pyomo.RangeSet(1, 2), domain=pyomo.Binary)
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(0, e[0])
         self.assertEqual(0, e[1])
         self.assertEqual('b', e.dtype.kind)
 
         m = pyomo.ConcreteModel()
         m.a = pyomo.Var(domain=pyomo.Reals)
         m.c = pyomo.Constraint(expr=m.a == 1.0)
         m.v = pyomo.Var(pyomo.RangeSet(1, 2), domain=pyomo.Binary, bounds=(1, None))
-        opt.solve(m)
+        solve_model(m)
         e = util.extract_pyomo_values(m.v)
         self.assertEqual(1, e[0])
         self.assertEqual(1, e[1])
         self.assertEqual('b', e.dtype.kind)
         return
 
 
@@ -442,7 +442,16 @@
         return 36
 
     @staticmethod
     def time_in_day(from_init):
         if not from_init:
             raise ValueError
         return 12
+
+
+def solve_model(model):
+    # hack to suppress pyomo no constraint warning
+    if not hasattr(model, "simple_var"):
+        model.simple_var = pyomo.Var(domain=pyomo.Reals, bounds=(None, None), initialize=0)
+        model.simple_constr = pyomo.Constraint(expr=model.simple_var == 1)
+    opt = pyomo.SolverFactory(solvers.DEFAULT_SOLVER)
+    return opt.solve(model, **solvers.DEFAULT_SOLVER_OPTIONS.get("solve", {}))
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/util/__init__.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/util/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -35,21 +35,21 @@
     'extract_pyomo_value',
     'extract_pyomo_values',
 ]
 
 
 def compute_profile(timer, profile, pattern=None):
     """
-    Compute a load series profile for an electrical vehicle.
+    Compute a load series profile for an electric vehicle.
 
     Parameters
     ----------
     timer : pycity_scheduling.classes.Timer
     profile : array of binaries
-        Indicator when electrical vehicle can be charged.
+        Indicator when electric vehicle can be charged.
 
         - `profile[t] == 0`: EV cannot be charged in t
         - `profile[t] == 1`: EV can be charged in t
         It must contain at least one `0` otherwise the model will become
         infeasible. Its length has to be consistent with `pattern`.
     pattern : str, optional
         Define how the `profile` is to be used.
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/util/debug.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/util/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/util/factory.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/util/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -20,15 +20,15 @@
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 
 import numpy as np
 import random
-from shapely.geometry import Point
+import os
 
 from pycity_scheduling.classes import *
 from pycity_scheduling.data.tabula_data import tabula_building_data as tbd
 from pycity_scheduling.data.ev_data import ev_data as evd
 
 
 def generate_standard_environment(**timer_args):
@@ -36,21 +36,30 @@
     Generate a standard environment object.
 
     Returns
     -------
     pycity_scheduling.classes.Environment
     """
     timer = Timer(**timer_args)
-    weather = Weather(timer)
+
+    weather_file_name = "TRY_2018.dat"
+    root_path = os.path.dirname(os.path.dirname(__file__))
+    weather_file_path = os.path.join(root_path, "data", weather_file_name)
+    weather = Weather(timer, path_TRY=weather_file_path, location=(51.53, 7.21), altitude=10.0)
+
     prices = Prices(timer)
+
     environment = Environment(timer, weather, prices)
     return environment
 
 
 def _calculate_ev_times(timer):
+    """
+    Supporting function to calculate electric vehicle charging time slots.
+    """
     length = int(3600/timer.time_discretization)
     ev_time_ranges = [
         [0] * (8 * length) + [1] * (12 * length) + [0] * (4 * length),
         [1] * (12 * length) + [0] * (12 * length),
         [0] * (12 * length) + [1] * (12 * length),
         [1] * (10 * length) + [0] * (12 * length) + [1] * (2 * length),
         [1] * (9 * length) + [0] * (12 * length) + [1] * (3 * length),
@@ -59,14 +68,17 @@
         [1] * (6 * length) + [0] * (12 * length) + [1] * (6 * length),
         [1] * (5 * length) + [0] * (12 * length) + [1] * (7 * length),
     ]
     return ev_time_ranges
 
 
 def _calculate_dl_times(timer):
+    """
+    Supporting function to calculate deferrable load consumption time slots.
+    """
     length = int(3600/timer.time_discretization)
     dl_time_ranges = [
         [1] * (8 * length) + [0] * (16 * length),
         [0] * (8 * length) + [1] * (4 * length) + [0] * (12 * length),
         [0] * (12 * length) + [1] * (4 * length) + [0] * (8 * length),
         [0] * (16 * length) + [1] * (4 * length) + [0] * (4 * length),
         [0] * (20 * length) + [1] * (4 * length),
@@ -116,15 +128,16 @@
 
 def generate_tabula_buildings(environment,
                               number,
                               building_distribution=None,
                               heating_distribution=None,
                               device_probabilities=None,
                               objective='price',
-                              seed=None):
+                              seed=None,
+                              mpi_interface=None):
     """
     Generate buildings based on the TABULA data.
 
     Generate buildings based on the TABULA data from: http://www.episcope.eu/ (accessed on 2020/09/28)
     Heating units are automatically dimensioned and added to each building. A
     THS always covers the thermal energy demand of a building for at least two
     hours.
@@ -155,18 +168,21 @@
         Values : float
             Number between 0 and 1.
     objective : str, optional
         The objective for all buildings.
     seed: int, optional
         Specify a seed for the randomization. If omitted, a non-deterministic
         city district will be generated.
-
+    mpi_interface : MPIInterface, optional
+        In the case of MPI, create a more "lightweight" city district per MPI process only containing the particular
+        buildings and assets that are required for the computations using MPI. Rank zero always has a list with all
+        buildings.
     Returns
     ----------
-    list of pycity_scheduling.classes.Building :
+    list of pycity_scheduling.classes.Building : list
         List of generated buildings.
     """
     if building_distribution is None:
         share = 1/len(tbd)
         building_distribution = {b: share for b in tbd}
     if heating_distribution is None:
         share = 1/len(heating_devices)
@@ -199,31 +215,40 @@
 
     # building entities
     a = round(device_probabilities.get('PV', 0) * number)
     pv_list = [True] * a + [False] * (number - a)
     a = round(device_probabilities.get('BAT', 0) * number)
     bat_list = [True] * a + [False] * (number - a)
 
-    ev_time_ranges = _calculate_ev_times(environment.timer)
     dl_time_ranges = _calculate_dl_times(environment.timer)
 
     if seed is not None:
         random.seed(seed)
     random.shuffle(heating_list)
     random.shuffle(fl_list)
     random.shuffle(dl_list)
     random.shuffle(pv_list)
     random.shuffle(ev_list)
     random.shuffle(bat_list)
 
     buildings = []
     ap_counter = 0
 
+    mpi_process_range = np.array([])
+    if mpi_interface is not None:
+        mpi_process_range = mpi_interface.get_mpi_process_range(number+1)
+
     # Generate buildings:
     for i, b in enumerate(building_dicts):
+        dummy_building = False
+        if mpi_interface is not None:
+            if mpi_interface.get_rank() != 0:
+                if mpi_interface.get_rank() != mpi_process_range[i+1]:
+                    dummy_building = True
+
         building_type = b['building_type']
         name = 'BD{:03}_{}'.format(i + 1, building_type)
 
         bd = Building(environment, objective=objective, name=name,
                       profile_type=b['th_profile_type'],
                       building_type=building_type)
 
@@ -233,88 +258,100 @@
         ap_area = b['net_floor_area']/b['apartments']
 
         for n in range(b['apartments']):
             ap = Apartment(environment, ap_area)
             sh = SpaceHeating(environment, method=1, living_area=ap_area,
                               specific_demand=b['th_demand'],
                               profile_type=b['th_profile_type'])
-            ap.addEntity(sh)
+            if not dummy_building:
+                ap.addEntity(sh)
 
             if fl_list[ap_counter]:
                 fl = FixedLoad(environment, method=1,
                                annual_demand=b['el_demand'],
                                profile_type=b['el_profile_type'])
-                ap.addEntity(fl)
+                if not dummy_building:
+                    ap.addEntity(fl)
 
             if dl_list[ap_counter]:
                 e_el = random.uniform(0.8, 4.5)
                 p_el = random.uniform(1.125, 2.5)
                 time = random.choice(dl_time_ranges)
                 dl = DeferrableLoad(environment, p_el_nom=p_el,
                                     e_consumption=e_el, load_time=time,
                                     lt_pattern='daily')
-                ap.addEntity(dl)
+                if not dummy_building:
+                    ap.addEntity(dl)
 
             if ev_list[ap_counter]:
                 ev_data = random.choice(list(evd.values()))
-                ev_charging_time = random.choice(ev_time_ranges)
-                soc = 0.5 if ev_data['charging_method'] == 'fast' else 0.75
-                ev = ElectricalVehicle(environment,
-                                       e_el_max=ev_data['e_el_storage_max'],
-                                       p_el_max_charge=ev_data['p_el_nom'],
-                                       soc_init=soc,
-                                       charging_time=ev_charging_time,
-                                       ct_pattern='daily')
-                ap.addEntity(ev)
+                ev_charging_time = np.ones(environment.timer.simu_horizon)
+                soc = random.uniform(0.2, 0.4)
+                ev = ElectricVehicle(environment,
+                                     e_el_max=ev_data['e_el_storage_max'],
+                                     p_el_max_charge=11.0,
+                                     soc_init=soc,
+                                     charging_time=ev_charging_time,
+                                     simulate_driving=False,
+                                     minimum_soc_end=0.8,
+                                     eta=0.95)
+                if not dummy_building:
+                    ap.addEntity(ev)
 
-            bd.addEntity(ap)
+            if not dummy_building:
+                bd.addEntity(ap)
             ap_counter += 1
 
-        p_th_heat = max(sum(e.p_th_heat_schedule for e in filter_entities(bd, 'SH'))) + 1
+        if not dummy_building:
+            p_th_heat = max(sum(e.p_th_heat_schedule for e in filter_entities(bd, 'SH'))) + 1
+        else:
+            p_th_heat = 100.0
         heating_device = heating_list[i](environment, p_th_nom=p_th_heat)
-        ths = ThermalHeatingStorage(environment, e_th_max=2.0*p_th_heat, soc_init=0.5)
-        bes.addDevice(heating_device)
-        bes.addDevice(ths)
+        ths = ThermalHeatingStorage(environment, e_th_max=2.0*p_th_heat, soc_init=0.5, loss_factor=10)
+
+        if not dummy_building:
+            bes.addDevice(heating_device)
+            bes.addDevice(ths)
 
         if pv_list[i]:
             if b['roof_angle'] == 0.0:
                 angle = 35.0
             else:
                 angle = b['roof_angle']
             area = b['roof_area']/2.0
             # Solar world 290 standard values
             pv = Photovoltaic(environment, method=0, area=area, eta_noct=0.161853,
                               t_cell_noct=46, alpha_noct=-0.0041, beta=angle)
-            bes.addDevice(pv)
+            if not dummy_building:
+                bes.addDevice(pv)
 
         if bat_list[i]:
             p_el = 13.5 * b['apartments']
             bat = Battery(environment, e_el_max=p_el, p_el_max_charge=4.6,
-                          p_el_max_discharge=4.6, soc_init=0.5)
-            bes.addDevice(bat)
+                          p_el_max_discharge=4.6, soc_init=0.5, eta=0.95)
+            if not dummy_building:
+                bes.addDevice(bat)
 
         buildings.append(bd)
-
-    assert ap_counter == number_ap
-
     return buildings
 
 
 def generate_tabula_district(environment,
                              number_sfh,
                              number_mfh,
                              sfh_building_distribution=None,
                              sfh_heating_distribution=None,
                              sfh_device_probabilities=None,
                              mfh_building_distribution=None,
                              mfh_heating_distribution=None,
                              mfh_device_probabilities=None,
                              district_objective='price',
                              building_objective='price',
-                             seed=1):
+                             seed=1,
+                             mpi_interface=None):
     """
     Generate a TABULA-based city district.
 
     Parameters
     ----------
     environment : pycity_scheduling.classes.Environment
     number_sfh : int
@@ -364,46 +401,53 @@
     district_objective : str, optional
         Objective function for the city district (district operator). Default is 'price'.
     building_objective : str, optional
         Objective function for the buildings. Default is 'price'.
     seed: int, optional
         Specify a seed for the randomization. If omitted, a non-deterministic
         city district will be generated.
-
+    mpi_interface : MPIInterface, optional
+        In the case of MPI, create a more "lightweight" city district per MPI process only containing the particular
+        buildings and assets that are required for the computations using MPI. Rank zero always has the city district
+        with all buildings.
     Returns
-    -------
+    ----------
+    list of pycity_scheduling.classes.CityDistrict : CityDistrict
+        CityDistrict object containing the generated buildings.
 
     """
     cd = CityDistrict(environment, district_objective)
     # noinspection PyListCreation
     building_list = []
     building_list.extend(generate_tabula_buildings(environment,
                                                    number_sfh,
                                                    sfh_building_distribution,
                                                    sfh_heating_distribution,
                                                    sfh_device_probabilities,
                                                    building_objective,
-                                                   seed
+                                                   seed,
+                                                   mpi_interface
                                                    ))
     building_list.extend(generate_tabula_buildings(environment,
                                                    number_mfh,
                                                    mfh_building_distribution,
                                                    mfh_heating_distribution,
                                                    mfh_device_probabilities,
                                                    building_objective,
                                                    seed+1,
+                                                   mpi_interface
                                                    ))
-    positions = [Point(0, i+1) for i in range(len(building_list))]
+    positions = [[0, i+1] for i in range(len(building_list))]
     cd.addMultipleEntities(building_list, positions)
     return cd
 
 
 def generate_simple_building(env, fl=0, sh=0, eh=0, ths=0, bat=0):
     """
-    Generate a simple building with loads and storages.
+    Generate a simple building with load and storage units.
 
     Parameters
     ----------
     env : pycity_scheduling.classes.Environment
     fl : float, optional
         Demand of the FixedLoad in [kW].
     sh : float, optional
@@ -413,27 +457,28 @@
     ths : float, optional
         Capacity of the ThermalHeatingStorage in [kWh].
     bat : float, optional
         Capacity of the Battery in [kWh].
 
     Returns
     -------
-    pycity_scheduling.classes.Building
+    pycity_scheduling.classes.Building: Building
+        Simple building with load and storage units.
     """
     ti = env.timer
 
     bd = Building(env)
     ap = Apartment(env)
     bd.addEntity(ap)
     bes = BuildingEnergySystem(env)
     bd.addEntity(bes)
     if fl:
         ap.addEntity(FixedLoad(env, demand=np.full(ti.simu_horizon, fl)))
     if sh:
         ap.addEntity(SpaceHeating(env, loadcurve=np.full(ti.simu_horizon, sh)))
     if eh:
-        bes.addDevice(ElectricalHeater(env, p_th_nom=eh))
+        bes.addDevice(ElectricHeater(env, p_th_nom=eh))
     if ths:
         bes.addDevice(ThermalHeatingStorage(env, e_th_max=ths, soc_init=0.5))
     if bat:
         bes.addDevice(Battery(env, e_el_max=bat, p_el_max_charge=bat/ti.time_slot))
     return bd
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/util/generic_constraints.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/util/generic_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/util/metric.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/util/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/util/plot_schedules.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/util/plot_schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -23,15 +23,15 @@
 
 
 import numpy as np
 import os
 import os.path as op
 import matplotlib.pyplot as plt
 
-from pycity_scheduling.classes import Battery, ElectricalVehicle, CombinedHeatPower
+from pycity_scheduling.classes import Battery, ElectricVehicle, CombinedHeatPower
 
 
 _known_varnames = {
     "p_el": plt.get_cmap("tab20").colors[:2],
     "e_el": plt.get_cmap("tab20").colors[8:10],
     "p_th": plt.get_cmap("tab20").colors[2:4],
     "e_th": plt.get_cmap("tab20").colors[6:8]
@@ -89,15 +89,15 @@
 
     var_colors = _known_varnames.copy()
     unknown_vars = entity.schedule.keys() - _known_varnames.keys()
     if isinstance(entity, Battery):
         unknown_vars.discard("p_el_demand")
         unknown_vars.discard("p_el_supply")
         unknown_vars.discard("p_state")
-    if isinstance(entity, ElectricalVehicle):
+    if isinstance(entity, ElectricVehicle):
         unknown_vars.discard("p_el_drive")
         unknown_vars.discard("p_state")
     if isinstance(entity, CombinedHeatPower):
         unknown_vars.discard("total_device")
         unknown_vars.discard("current_device")
     for i, uv in enumerate(unknown_vars):
         if i >= len(_other_colors):
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling/util/write_schedules.py` & `pycity_scheduling-1.2.0/src/pycity_scheduling/util/write_schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The pycity_scheduling framework
 
 
-Copyright (C) 2022,
+Copyright (C) 2023,
 Institute for Automation of Complex Power Systems (ACS),
 E.ON Energy Research Center (E.ON ERC),
 RWTH Aachen University
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
 documentation files (the "Software"), to deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/PKG-INFO` & `pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycity-scheduling
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python framework for the development, testing, and assessment of optimization-basedpower scheduling algorithms for multi-energy systems in city districts
 Home-page: https://git.rwth-aachen.de/acs/public/simulation/pycity_scheduling
 Author: Institute for Automation of Complex Power Systems (ACS),E.ON Energy Research Center (E.ON ERC),RWTH Aachen University
 Author-email: post_acs@eonerc.rwth-aachen.de
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -62,15 +62,15 @@
 - [bonmin](https://github.com/coin-or/Bonmin)
 - [Gurobi (gurobipy)](https://www.gurobi.com/products/gurobi-optimizer/) (default)
 - [IBM ILOG CPLEX](https://www.ibm.com/products/ilog-cplex-optimization-studio)
 
 
 ### Installation of pycity_scheduling
 
-The latest version of pycity_scheduling is v1.1.0.
+The latest version of pycity_scheduling is v1.2.0.
 
 If all the abovementioned dependencies are installed, you should be able to install package pycity_scheduling via [PyPI](https://pypi.org/) (using Python version >= 3.7) as follows:
 
 `pip install pycity_scheduling`
 
 or to install in editable mode:
 
@@ -119,15 +119,14 @@
 
 
 def main(do_plot=False):
     print("\n\n------ Example 00: Fundamentals ------\n\n")
 
     # 1) Environment objects:
 
-
     # (Almost) every object within pycity_scheduling requires an environment. The environment object holds general data,
     # which is valid for all objects within pycity_scheduling, such as time data, weather data or energy market prices.
     # Therefore, all objects point to an environment. The first step is usually to generate such an environment.
 
     # Generate a timer object for the environment:
     timer = Timer(step_size=3600, op_horizon=24, initial_date=(2015, 1, 1), initial_time=(0, 0, 0))
 
@@ -136,15 +135,14 @@
 
     # Generate a price object for the environment:
     price = Prices(timer=timer)
 
     # Generate the environment object:
     environment = Environment(timer=timer, weather=weather, prices=price)
 
-
     # Now there is a distinct environment object with timer, weather and price data.
     # We can use it to access different data of interest.
 
     # For example, print the current weekday:
     print('Weekday:')
     print(environment.timer.weekday)
 
@@ -152,15 +150,14 @@
     print('\nOutdoor temperature forecast:')
     print(environment.weather.getWeatherForecast(getTAmbient=True)[0][:10])
 
     # For example, print the energy spot market day-ahead prices:
     print('\nDay-ahead spot market prices on 2015/01/01:')
     print(environment.prices.da_prices)
 
-
     # 2) Buildings objects:
 
     # After defining the environment, different building objects should be created. In pycity_scheduling, buildings
     # represent the different customers of the local energy system / city district under investigation.
     # In general, buildings should also be understood in a more abstract way. For instance, a building object must not
     # necessarily represent a building structure, as it would be the case for a wind energy converter.
 
@@ -170,15 +167,14 @@
     # This building is assumed to be equipped with a building energy system and one apartment (=single-family house).
     # In general, every building object can, however, hold up to N different apartments (=multi-family house).
     apartment = Apartment(environment=environment)
     bes = BuildingEnergySystem(environment=environment)
 
     building.addMultipleEntities([apartment, bes])
 
-
     # Every apartment usually possesses both electrical and thermal loads:
     # The electrical load is added to the apartment as follows:
     load = FixedLoad(environment=environment, method=1, annual_demand=3000)
 
     # Print and show the electrical power curve in Watt:
     print('\nElectrical load in Watt:')
     print(load.get_power(currentValues=False))
@@ -201,15 +197,14 @@
     plt.ylabel('Thermal power in Watt (space heating)')
     plt.title('Space heating power curve')
     if do_plot:
         plt.show()
 
     apartment.addMultipleEntities([load, space_heating])
 
-
     # The BuildingEnergySystem (BES) class is a 'container' for all kind of building energy systems (i.e., electrical
     # and/or thermal assets). For example, we can add an electro-thermal heating system (such as a heatpump plus thermal
     # energy storage) and a photovoltaic unit to a building's BES as done below. In pycity_scheduling all BES devices
     # automatically come with basic scheduling models, which include the required Pyomo optimization variables and
     # several optimization constraints.
     eh = HeatPump(environment=environment, p_th_nom=16.0)
     ths = ThermalHeatingStorage(environment=environment, e_th_max=20.0, soc_init=0.5, loss_factor=0)
@@ -218,15 +213,14 @@
     bes.addMultipleDevices([eh, ths, pv])
 
     # Verify if the assets were added successfully (method getHasDevice):
     print('\nBES has heatpump? : ', bes.getHasDevices(all_devices=False, heatpump=True)[0])
     print('BES has thermal heating storage? : ', bes.getHasDevices(all_devices=False, ths=True)[0])
     print('BES has photovoltaic? : ', bes.getHasDevices(all_devices=False, pv=True)[0])
 
-
     # 3) CityDistrict objects:
 
     # In pycity_scheduling, a group of buildings form a CityDistrict object. The CityDistrict is the object to be
     # "provided" to a power scheduling algorithm later on. In other word, it encapsulates all buildings together with
     # their local assets and it hence includes all the optimization problem information and data.
 
     # Create a city district object:
@@ -260,15 +254,14 @@
 
     # Print the city district information:
     print('\nTotal number of buildings in city district:')
     print(cd.get_nb_of_building_entities())
     print("\nDetailed city district information:")
     debug.print_district(cd, 3)
 
-
     # 4) Power scheduling:
 
     # The final step is to schedule the buildings/assets inside the city district subject to a certain optimization
     # objective, which can be, for example, peak-shaving. The scheduling is then performed by the user by "passing"
     # the city district object to a certain power scheduling algorithm.
     # Here, the central optimization algorithm is used.
 
@@ -298,15 +291,15 @@
 if __name__ == '__main__':
     # Run example:
     main(do_plot=True)
 ```
 
 ## Tutorial
 
-The pycity_scheduling package comes with several example/tutorial scripts in folder ./src/examples.
+The pycity_scheduling package comes with several example, tutorial, and simple case study scripts in folder ./src/examples.
 
 The unit tests can be found in folder ./src/testing.
 
 
 Moreover, also check the pycity_base package's tutorials for the basic usage of the framework's core functionalities. 
 
 
@@ -323,9 +316,7 @@
 
 [Institute for Automation of Complex Power Systems (ACS)](http://www.acs.eonerc.rwth-aachen.de) \
 [E.ON Energy Research Center (E.ON ERC)](http://www.eonerc.rwth-aachen.de) \
 [RWTH Aachen University, Germany](http://www.rwth-aachen.de)
 
 
 <img src="https://fein-aachen.org/img/logos/eonerc.png"/>
-
-
```

### Comparing `pycity_scheduling-1.1.0/src/pycity_scheduling.egg-info/SOURCES.txt` & `pycity_scheduling-1.2.0/src/pycity_scheduling.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,31 +11,35 @@
 src/pycity_scheduling.egg-info/not-zip-safe
 src/pycity_scheduling.egg-info/requires.txt
 src/pycity_scheduling.egg-info/top_level.txt
 src/pycity_scheduling/algorithms/__init__.py
 src/pycity_scheduling/algorithms/algorithm.py
 src/pycity_scheduling/algorithms/central_optimization_algorithm.py
 src/pycity_scheduling/algorithms/dual_decomposition_algorithm.py
+src/pycity_scheduling/algorithms/dual_decomposition_algorithm_mpi.py
 src/pycity_scheduling/algorithms/exchange_admm_algorithm.py
+src/pycity_scheduling/algorithms/exchange_admm_algorithm_mpi.py
+src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm.py
+src/pycity_scheduling/algorithms/exchange_miqp_admm_algorithm_mpi.py
 src/pycity_scheduling/algorithms/local_optimization_algorithm.py
 src/pycity_scheduling/algorithms/stand_alone_optimization_algorithm.py
 src/pycity_scheduling/classes/__init__.py
 src/pycity_scheduling/classes/apartment.py
 src/pycity_scheduling/classes/battery.py
 src/pycity_scheduling/classes/boiler.py
 src/pycity_scheduling/classes/building.py
 src/pycity_scheduling/classes/building_energy_system.py
 src/pycity_scheduling/classes/chiller.py
 src/pycity_scheduling/classes/city_district.py
 src/pycity_scheduling/classes/combined_heat_power.py
 src/pycity_scheduling/classes/curtailable_load.py
 src/pycity_scheduling/classes/deferrable_load.py
+src/pycity_scheduling/classes/electric_heater.py
+src/pycity_scheduling/classes/electric_vehicle.py
 src/pycity_scheduling/classes/electrical_entity.py
-src/pycity_scheduling/classes/electrical_heater.py
-src/pycity_scheduling/classes/electrical_vehicle.py
 src/pycity_scheduling/classes/entity_container.py
 src/pycity_scheduling/classes/environment.py
 src/pycity_scheduling/classes/fixed_load.py
 src/pycity_scheduling/classes/heat_pump.py
 src/pycity_scheduling/classes/optimization_entity.py
 src/pycity_scheduling/classes/photovoltaic.py
 src/pycity_scheduling/classes/prices.py
@@ -44,54 +48,56 @@
 src/pycity_scheduling/classes/thermal_cooling_storage.py
 src/pycity_scheduling/classes/thermal_entity_cooling.py
 src/pycity_scheduling/classes/thermal_entity_heating.py
 src/pycity_scheduling/classes/thermal_heating_storage.py
 src/pycity_scheduling/classes/timer.py
 src/pycity_scheduling/classes/weather.py
 src/pycity_scheduling/classes/wind_energy_converter.py
+src/pycity_scheduling/data/TRY_2018.dat
 src/pycity_scheduling/data/__init__.py
 src/pycity_scheduling/data/co2_emissions_quarter-hour_2015.txt
 src/pycity_scheduling/data/consumer_prices_yearly.txt
 src/pycity_scheduling/data/da_prices_quarter-hour_2015.txt
 src/pycity_scheduling/data/ev_data.py
 src/pycity_scheduling/data/tabula_data.py
 src/pycity_scheduling/examples/__init__.py
 src/pycity_scheduling/examples/example_00_fundamentals.py
 src/pycity_scheduling/examples/example_01_algorithm_central.py
 src/pycity_scheduling/examples/example_02_algorithm_local.py
 src/pycity_scheduling/examples/example_03_algorithm_stand-alone.py
 src/pycity_scheduling/examples/example_04_algorithm_dual-decomposition.py
 src/pycity_scheduling/examples/example_05_algorithm_exchange-admm.py
-src/pycity_scheduling/examples/example_06_algorithm_warmstart.py
-src/pycity_scheduling/examples/example_07_objective_peak-shaving.py
-src/pycity_scheduling/examples/example_08_objective_max-consumption.py
-src/pycity_scheduling/examples/example_09_objective_self-consumption.py
-src/pycity_scheduling/examples/example_10_objective_price.py
-src/pycity_scheduling/examples/example_11_objective_co2.py
-src/pycity_scheduling/examples/example_12_objective_valley-filling.py
-src/pycity_scheduling/examples/example_13_district_generator.py
-src/pycity_scheduling/examples/example_14_district_flexibility_quantification.py
-src/pycity_scheduling/examples/example_15_scheduling_complex_city_district.py
-src/pycity_scheduling/examples/example_16_scheduling_convex_vs._integer_mode.py
-src/pycity_scheduling/examples/example_17_scheduling_pv+battery_system.py
-src/pycity_scheduling/examples/example_18_scheduling_heating_and_cooling_loads.py
-src/pycity_scheduling/examples/example_19_scheduling_robust_optimization.py
-src/pycity_scheduling/examples/example_20_post-processing_schedule_evaluation.py
-src/pycity_scheduling/examples/example_21_post-processing_metrics_evaluation.py
-src/pycity_scheduling/examples/illustrative_code_example_cost_minimization_use_case_interactive.ipynb
-src/pycity_scheduling/examples/illustrative_code_example_listing1.py
-src/pycity_scheduling/examples/illustrative_code_example_listing2.py
-src/pycity_scheduling/examples/illustrative_code_example_listing3.py
+src/pycity_scheduling/examples/example_06_algorithm_exchange-miqp-admm.py
+src/pycity_scheduling/examples/example_07_algorithm_warmstart.py
+src/pycity_scheduling/examples/example_08_algorithm_parallel_mpi.py
+src/pycity_scheduling/examples/example_09_objective_peak-shaving.py
+src/pycity_scheduling/examples/example_10_objective_self-consumption.py
+src/pycity_scheduling/examples/example_11_objective_max-consumption.py
+src/pycity_scheduling/examples/example_12_objective_price.py
+src/pycity_scheduling/examples/example_13_objective_co2.py
+src/pycity_scheduling/examples/example_14_objective_valley-filling.py
+src/pycity_scheduling/examples/example_15_district_generator.py
+src/pycity_scheduling/examples/example_16_scheduling_complex_city_district.py
+src/pycity_scheduling/examples/example_17_district_flexibility_quantification.py
+src/pycity_scheduling/examples/example_18_scheduling_pv+battery_system.py
+src/pycity_scheduling/examples/example_19_scheduling_heating_and_cooling_loads.py
+src/pycity_scheduling/examples/example_20_scheduling_convex_vs._integer_mode.py
+src/pycity_scheduling/examples/example_21_scheduling_robust_optimization.py
+src/pycity_scheduling/examples/example_22_post-processing_schedule_evaluation.py
+src/pycity_scheduling/examples/example_23_post-processing_metrics_evaluation.py
+src/pycity_scheduling/examples/case_studies/illustrative_code_example_cost_minimization_use_case_interactive.ipynb
 src/pycity_scheduling/testing/__init__.py
 src/pycity_scheduling/testing/unit_tests/__init__.py
 src/pycity_scheduling/testing/unit_tests/test_algorithms.py
 src/pycity_scheduling/testing/unit_tests/test_all_classes.py
 src/pycity_scheduling/testing/unit_tests/test_classes.py
 src/pycity_scheduling/testing/unit_tests/test_examples.py
 src/pycity_scheduling/testing/unit_tests/test_util.py
 src/pycity_scheduling/util/__init__.py
 src/pycity_scheduling/util/debug.py
+src/pycity_scheduling/util/district_analyzer.py
 src/pycity_scheduling/util/factory.py
 src/pycity_scheduling/util/generic_constraints.py
 src/pycity_scheduling/util/metric.py
+src/pycity_scheduling/util/mpi_interface.py
 src/pycity_scheduling/util/plot_schedules.py
 src/pycity_scheduling/util/write_schedules.py
```

