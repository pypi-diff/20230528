# Comparing `tmp/pyasd-0.0.7.tar.gz` & `tmp/pyasd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyasd-0.0.7.tar", last modified: Tue May  9 10:31:47 2023, max compression
+gzip compressed data, was "pyasd-0.0.8.tar", last modified: Sun May 28 17:01:00 2023, max compression
```

## Comparing `pyasd-0.0.7.tar` & `pyasd-0.0.8.tar`

### file list

```diff
@@ -1,158 +1,159 @@
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.671012 pyasd-0.0.7/
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.7/LICENSE
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      488 2023-01-06 02:20:47.000000 pyasd-0.0.7/MANIFEST.in
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-09 10:31:47.671012 pyasd-0.0.7/PKG-INFO
--rw-r--r--   0 zsh       (1000) zsh       (1000)     1350 2023-04-26 14:54:49.000000 pyasd-0.0.7/README.md
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.651012 pyasd-0.0.7/asd/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      344 2023-05-09 10:31:47.000000 pyasd-0.0.7/asd/__init__.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.651012 pyasd-0.0.7/asd/core/
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/constants.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/dipolar_interactions.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/geometry.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/gneb.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28461 2023-05-09 09:34:19.000000 pyasd-0.0.7/asd/core/hamiltonian.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/llg_advanced.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    34609 2023-05-09 01:11:38.000000 pyasd-0.0.7/asd/core/llg_simple.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/log_general.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    35175 2023-05-09 09:27:46.000000 pyasd-0.0.7/asd/core/monte_carlo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7332 2023-05-09 10:27:02.000000 pyasd-0.0.7/asd/core/random_vectors.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    28028 2023-05-03 15:39:15.000000 pyasd-0.0.7/asd/core/shell_exchange.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    20217 2023-05-09 09:29:35.000000 pyasd-0.0.7/asd/core/spin_configurations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.7/asd/core/spin_correlations.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4455 2023-05-07 01:15:42.000000 pyasd-0.0.7/asd/core/topological_charge.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.655012 pyasd-0.0.7/asd/data_base/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.7/asd/data_base/exchange_for_Cr2I3X3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.7/asd/data_base/exchange_for_CrI3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.7/asd/data_base/exchange_for_CrMnI6_U2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.7/asd/data_base/exchange_for_CrMnI6_U4.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.7/asd/data_base/exchange_for_CrMnI6_rect.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.7/asd/data_base/exchange_for_Gd2C.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.7/asd/data_base/exchange_for_MnI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.7/asd/data_base/exchange_for_NiI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.7/asd/data_base/exchange_for_RuCl3.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.7/asd/data_base/exchange_for_VOI2.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.7/asd/data_base/exchange_for_kagome.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.7/asd/data_base/exchange_for_skx.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.655012 pyasd-0.0.7/asd/mpi/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2556 2023-05-09 02:04:47.000000 pyasd-0.0.7/asd/mpi/mpi_tools.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.659012 pyasd-0.0.7/asd/utility/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.7/asd/utility/Swq.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.7/asd/utility/__init__.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     8709 2023-05-07 06:58:07.000000 pyasd-0.0.7/asd/utility/analyze_Spirit_results.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     9134 2023-05-07 06:52:31.000000 pyasd-0.0.7/asd/utility/asd_arguments.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.7/asd/utility/auxiliary_colormaps.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.7/asd/utility/curve_fit.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.7/asd/utility/four_state_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.7/asd/utility/head_figlet.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.7/asd/utility/mag_thermal.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     7619 2023-05-09 02:11:15.000000 pyasd-0.0.7/asd/utility/ovf_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.7/asd/utility/plot_tools_3d.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    13553 2023-05-07 06:40:57.000000 pyasd-0.0.7/asd/utility/post_llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5470 2023-05-07 06:40:40.000000 pyasd-0.0.7/asd/utility/post_mc.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)    19392 2023-05-09 02:10:46.000000 pyasd-0.0.7/asd/utility/spin_visualize_tools.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2442 2023-05-09 02:10:36.000000 pyasd-0.0.7/asd/utility/spirit_tool.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.659012 pyasd-0.0.7/examples/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.7/examples/README
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.659012 pyasd-0.0.7/examples/example1/
--rw-r--r--   0 zsh       (1000) zsh       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.7/examples/example1/.coverage
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.7/examples/example1/single_spin_LLG.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.659012 pyasd-0.0.7/examples/example2/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.7/examples/example2/README.md
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.7/examples/example2/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.659012 pyasd-0.0.7/examples/example3/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.7/examples/example3/README.md
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.7/examples/example3/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.659012 pyasd-0.0.7/examples/example4/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.7/examples/example4/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.7/examples/example4/llg.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.647012 pyasd-0.0.7/misc/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.659012 pyasd-0.0.7/misc/archives/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.7/misc/archives/ovf-0.4.3.tar.gz
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.7/misc/archives/pyfiglet-0.7.tar.gz
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/pyasd.egg-info/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      425 2023-05-09 10:31:47.000000 pyasd-0.0.7/pyasd.egg-info/PKG-INFO
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     4686 2023-05-09 10:31:47.000000 pyasd-0.0.7/pyasd.egg-info/SOURCES.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)        1 2023-05-09 10:31:47.000000 pyasd-0.0.7/pyasd.egg-info/dependency_links.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       43 2023-05-09 10:31:47.000000 pyasd-0.0.7/pyasd.egg-info/requires.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)     1083 2023-05-09 10:31:47.000000 pyasd-0.0.7/pyasd.egg-info/top_level.txt
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       38 2023-05-09 10:31:47.671012 pyasd-0.0.7/setup.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4975 2023-05-09 10:31:17.000000 pyasd-0.0.7/setup.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.647012 pyasd-0.0.7/tests_basic/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/tests_basic/B_eff/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.7/tests_basic/B_eff/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.7/tests_basic/B_eff/test_B_eff.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/tests_basic/OVF/
--rw-rw-r--   0 zsh       (1000) zsh       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.7/tests_basic/OVF/README
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.7/tests_basic/OVF/pyasd_ovf_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.7/tests_basic/OVF/test_ovf.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/tests_basic/mag_confs/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/tests_basic/mag_confs/Potts/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.7/tests_basic/mag_confs/Potts/Potts_test.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/tests_basic/mag_confs/domain_walls/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/domain_walls/dw_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/interpolate_images.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/tests_basic/mag_confs/meron/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/meron/bimeron.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/meron/meron.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.663012 pyasd-0.0.7/tests_basic/mag_confs/misc/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/misc/interpolate_images.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/misc/mpi_topo.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1067 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/misc/regular_order_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/misc/struct_factor.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/misc/test_pbc_shell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/Skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/a2sk.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/mpi_firework.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/skyrmionium.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/mag_confs/spirals/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
--rw-r--r--   0 zsh       (1000) zsh       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.7/tests_basic/mag_confs/spirals/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/spirals/spiral_test.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/mag_confs/test_regular_orders_honeycomb.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/mpi/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.7/tests_basic/mpi/test_group_rank.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.651012 pyasd-0.0.7/tests_basic/total_energy/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.647012 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
--rw-rw-r--   0 zsh       (1000) zsh       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/simple/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.667012 pyasd-0.0.7/tests_basic/total_energy/chiral_confs/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.7/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.671012 pyasd-0.0.7/tests_basic/total_energy/large_test/
--rw-r--r--   0 zsh       (1000) zsh       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.7/tests_basic/total_energy/large_test/README
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/large_test/large_cell.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.671012 pyasd-0.0.7/tests_basic/total_energy/large_test/test_loop_methods/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.671012 pyasd-0.0.7/tests_basic/total_energy/local_energy/
--rwxrwxr-x   0 zsh       (1000) zsh       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/local_energy/CrMnI6_test.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/local_energy/test_local_en.py
-drwxrwxr-x   0 zsh       (1000) zsh       (1000)        0 2023-05-09 10:31:47.671012 pyasd-0.0.7/tests_basic/total_energy/regular_orders/
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     7050 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     1851 2023-01-05 07:16:05.000000 pyasd-0.0.7/tests_basic/total_energy/regular_orders/llg.py
--rwxr-xr-x   0 zsh       (1000) zsh       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.7/tests_basic/total_energy/regular_orders/phase_diagram_tri.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/
+-rw-r--r--   0 shz       (1000) shz       (1000)     1468 2023-01-05 06:57:53.000000 pyasd-0.0.8/LICENSE
+-rw-r--r--   0 shz       (1000) shz       (1000)      488 2023-05-09 10:17:42.000000 pyasd-0.0.8/MANIFEST.in
+-rw-r--r--   0 shz       (1000) shz       (1000)      425 2023-05-28 17:01:00.724262 pyasd-0.0.8/PKG-INFO
+-rw-r--r--   0 shz       (1000) shz       (1000)     1350 2023-04-26 14:54:49.000000 pyasd-0.0.8/README.md
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/
+-rw-r--r--   0 shz       (1000) shz       (1000)      344 2023-05-28 17:01:00.000000 pyasd-0.0.8/asd/__init__.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/core/
+-rw-r--r--   0 shz       (1000) shz       (1000)        0 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/__init__.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      537 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/constants.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      902 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/dipolar_interactions.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    14970 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/geometry.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    34800 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/gneb.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    28461 2023-05-09 09:34:19.000000 pyasd-0.0.8/asd/core/hamiltonian.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    13407 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/llg_advanced.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    34609 2023-05-09 01:11:38.000000 pyasd-0.0.8/asd/core/llg_simple.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     6394 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/log_general.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    35175 2023-05-09 09:27:46.000000 pyasd-0.0.8/asd/core/monte_carlo.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     7332 2023-05-09 09:32:21.000000 pyasd-0.0.8/asd/core/random_vectors.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    28028 2023-05-03 15:39:15.000000 pyasd-0.0.8/asd/core/shell_exchange.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    21553 2023-05-12 03:07:14.000000 pyasd-0.0.8/asd/core/spin_configurations.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    13692 2023-05-01 09:00:05.000000 pyasd-0.0.8/asd/core/spin_correlations.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     4507 2023-05-10 06:53:02.000000 pyasd-0.0.8/asd/core/topological_charge.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/data_base/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     4160 2022-11-27 16:42:32.000000 pyasd-0.0.8/asd/data_base/exchange_for_Cr2I3X3.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1657 2022-11-03 04:08:41.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrI3.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3216 2022-10-04 07:38:22.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U2.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     6933 2022-11-17 08:49:56.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U4.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3873 2023-01-05 11:41:58.000000 pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_rect.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1295 2022-11-14 15:25:58.000000 pyasd-0.0.8/asd/data_base/exchange_for_Gd2C.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     4390 2022-12-24 03:07:21.000000 pyasd-0.0.8/asd/data_base/exchange_for_MnI2.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2594 2022-12-24 03:07:20.000000 pyasd-0.0.8/asd/data_base/exchange_for_NiI2.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     5909 2022-11-14 15:08:43.000000 pyasd-0.0.8/asd/data_base/exchange_for_RuCl3.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2188 2022-02-21 08:35:16.000000 pyasd-0.0.8/asd/data_base/exchange_for_VOI2.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1468 2022-11-27 16:26:00.000000 pyasd-0.0.8/asd/data_base/exchange_for_kagome.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1066 2022-02-21 07:00:49.000000 pyasd-0.0.8/asd/data_base/exchange_for_skx.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/mpi/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2556 2023-05-09 02:04:47.000000 pyasd-0.0.8/asd/mpi/mpi_tools.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/asd/utility/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    12245 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/Swq.py
+-rw-r--r--   0 shz       (1000) shz       (1000)        0 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/__init__.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     8709 2023-05-07 06:58:07.000000 pyasd-0.0.8/asd/utility/analyze_Spirit_results.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     9134 2023-05-07 06:52:31.000000 pyasd-0.0.8/asd/utility/asd_arguments.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    55462 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/auxiliary_colormaps.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2143 2023-02-03 13:19:28.000000 pyasd-0.0.8/asd/utility/curve_fit.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     5328 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/four_state_tools.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1880 2023-04-17 02:00:31.000000 pyasd-0.0.8/asd/utility/head_figlet.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     6688 2023-02-07 02:54:27.000000 pyasd-0.0.8/asd/utility/mag_thermal.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     7619 2023-05-09 02:11:15.000000 pyasd-0.0.8/asd/utility/ovf_tools.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     7753 2023-02-03 13:19:13.000000 pyasd-0.0.8/asd/utility/plot_tools_3d.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    13553 2023-05-07 06:40:57.000000 pyasd-0.0.8/asd/utility/post_llg.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     5470 2023-05-07 06:40:40.000000 pyasd-0.0.8/asd/utility/post_mc.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    19392 2023-05-10 14:31:13.000000 pyasd-0.0.8/asd/utility/spin_visualize_tools.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2442 2023-05-09 02:10:36.000000 pyasd-0.0.8/asd/utility/spirit_tool.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/
+-rw-r--r--   0 shz       (1000) shz       (1000)      266 2023-01-11 07:09:44.000000 pyasd-0.0.8/examples/README
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example1/
+-rw-r--r--   0 shz       (1000) shz       (1000)    53248 2022-11-27 08:16:32.000000 pyasd-0.0.8/examples/example1/.coverage
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2626 2023-01-05 02:33:47.000000 pyasd-0.0.8/examples/example1/single_spin_LLG.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example2/
+-rw-r--r--   0 shz       (1000) shz       (1000)      392 2023-01-11 07:10:07.000000 pyasd-0.0.8/examples/example2/README.md
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1305 2023-01-05 02:34:09.000000 pyasd-0.0.8/examples/example2/llg.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example3/
+-rw-r--r--   0 shz       (1000) shz       (1000)      385 2023-01-11 07:09:55.000000 pyasd-0.0.8/examples/example3/README.md
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1306 2022-11-27 08:14:55.000000 pyasd-0.0.8/examples/example3/llg.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/examples/example4/
+-rw-r--r--   0 shz       (1000) shz       (1000)       59 2022-10-28 23:58:00.000000 pyasd-0.0.8/examples/example4/README
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1319 2022-11-27 08:14:55.000000 pyasd-0.0.8/examples/example4/llg.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/misc/
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/misc/archives/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)   492671 2022-11-26 13:27:45.000000 pyasd-0.0.8/misc/archives/ovf-0.4.3.tar.gz
+-rwxr-xr-x   0 shz       (1000) shz       (1000)   691395 2021-09-12 03:38:59.000000 pyasd-0.0.8/misc/archives/pyfiglet-0.7.tar.gz
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/pyasd.egg-info/
+-rw-r--r--   0 shz       (1000) shz       (1000)      425 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/PKG-INFO
+-rw-r--r--   0 shz       (1000) shz       (1000)     4701 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/SOURCES.txt
+-rw-r--r--   0 shz       (1000) shz       (1000)        1 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/dependency_links.txt
+-rw-r--r--   0 shz       (1000) shz       (1000)       43 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/requires.txt
+-rw-r--r--   0 shz       (1000) shz       (1000)     1083 2023-05-28 17:01:00.000000 pyasd-0.0.8/pyasd.egg-info/top_level.txt
+-rw-r--r--   0 shz       (1000) shz       (1000)       38 2023-05-28 17:01:00.724262 pyasd-0.0.8/setup.cfg
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3490 2023-05-28 17:00:15.000000 pyasd-0.0.8/setup.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/tests_basic/
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/B_eff/
+-rw-r--r--   0 shz       (1000) shz       (1000)      219 2023-01-05 07:15:01.000000 pyasd-0.0.8/tests_basic/B_eff/README
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1238 2023-01-05 07:14:20.000000 pyasd-0.0.8/tests_basic/B_eff/test_B_eff.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/OVF/
+-rw-r--r--   0 shz       (1000) shz       (1000)       64 2023-02-08 03:42:29.000000 pyasd-0.0.8/tests_basic/OVF/README
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3532 2023-02-08 03:43:05.000000 pyasd-0.0.8/tests_basic/OVF/pyasd_ovf_test.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2777 2023-02-08 03:42:25.000000 pyasd-0.0.8/tests_basic/OVF/test_ovf.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/Potts/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      880 2022-12-11 16:02:18.000000 pyasd-0.0.8/tests_basic/mag_confs/Potts/Potts_test.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/domain_walls/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      916 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/domain_walls/analytical_single_domain.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1983 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/domain_walls/dw_test.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1558 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/interpolate_images.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/meron/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1229 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3213 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/bimeron.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2055 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1475 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/meron/meron.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/misc/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1359 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/interpolate_images.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1055 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/mpi_topo.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1680 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/struct_factor.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      768 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/misc/test_pbc_shell.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/regular_magnetic_orders/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1732 2023-05-23 07:46:00.000000 pyasd-0.0.8/tests_basic/mag_confs/regular_magnetic_orders/regular_order_test.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1289 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Skyrmion.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3902 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1935 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/a2sk.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1809 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/afm_skyrmion.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     5572 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/firework.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     4145 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
+-rw-r--r--   0 shz       (1000) shz       (1000)      266 2021-07-10 08:59:53.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/input.cfg
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2196 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/mpi_firework.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1241 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/skyrmionium.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      831 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/skyrmion/view_3d_skyr.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mag_confs/spirals/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1511 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/spirals/CrMnI6_spiral.py
+-rw-r--r--   0 shz       (1000) shz       (1000)      266 2021-09-21 08:17:22.000000 pyasd-0.0.8/tests_basic/mag_confs/spirals/input.cfg
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     4060 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/spirals/spiral_test.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1337 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/mag_confs/test_regular_orders_honeycomb.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/mpi/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      460 2023-01-05 15:02:33.000000 pyasd-0.0.8/tests_basic/mpi/test_group_rank.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/tests_basic/total_energy/
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.714262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      443 2022-11-20 00:54:15.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/input.cfg
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      120 2022-11-19 15:36:27.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/post
+-rw-r--r--   0 shz       (1000) shz       (1000)      462 2022-11-20 00:54:36.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/quadruplet
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3625 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     5188 2023-05-01 09:01:00.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      363 2022-11-20 00:26:00.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/input.cfg
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1765 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      120 2022-11-19 15:38:35.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/post
+-rw-r--r--   0 shz       (1000) shz       (1000)      449 2022-11-20 00:22:35.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/quadruplet
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      751 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     7818 2022-11-19 12:09:07.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/input.cfg
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     3923 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/chiral_confs/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1972 2023-01-05 11:42:50.000000 pyasd-0.0.8/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/large_test/
+-rw-r--r--   0 shz       (1000) shz       (1000)      136 2023-01-05 15:00:27.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/README
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1854 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/large_cell.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1506 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1998 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/local_energy/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)      413 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/local_energy/CrMnI6_test.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     4098 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/local_energy/test_local_en.py
+drwxr-xr-x   0 shz       (1000) shz       (1000)        0 2023-05-28 17:01:00.724262 pyasd-0.0.8/tests_basic/total_energy/regular_orders/
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     1851 2023-05-11 13:40:16.000000 pyasd-0.0.8/tests_basic/total_energy/regular_orders/llg.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)    13977 2023-05-19 07:49:42.000000 pyasd-0.0.8/tests_basic/total_energy/regular_orders/phase_diagram_honeycomb.py
+-rwxr-xr-x   0 shz       (1000) shz       (1000)     2685 2022-11-28 02:21:11.000000 pyasd-0.0.8/tests_basic/total_energy/regular_orders/phase_diagram_triangular.py
```

### Comparing `pyasd-0.0.7/LICENSE` & `pyasd-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/README.md` & `pyasd-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/constants.py` & `pyasd-0.0.8/asd/core/constants.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/dipolar_interactions.py` & `pyasd-0.0.8/asd/core/dipolar_interactions.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/geometry.py` & `pyasd-0.0.8/asd/core/geometry.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/gneb.py` & `pyasd-0.0.8/asd/core/gneb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/hamiltonian.py` & `pyasd-0.0.8/asd/core/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/llg_advanced.py` & `pyasd-0.0.8/asd/core/llg_advanced.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/llg_simple.py` & `pyasd-0.0.8/asd/core/llg_simple.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/log_general.py` & `pyasd-0.0.8/asd/core/log_general.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/monte_carlo.py` & `pyasd-0.0.8/asd/core/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/random_vectors.py` & `pyasd-0.0.8/asd/core/random_vectors.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/shell_exchange.py` & `pyasd-0.0.8/asd/core/shell_exchange.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/spin_configurations.py` & `pyasd-0.0.8/asd/core/spin_configurations.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,58 +37,93 @@
     Did you forget to initialize the spin configuration?
     max deviation of norm = {:10.5f}\n'''.format(np.max(abs(norm-1)))
 
 
 
 # create "regular magnetic order" as elaborated in 
 # Phys. Rev. B 83, 184401 (2011)
-def regular_order(lat_type='triangular',order_name='tetrahedra'):
+def regular_order_on_triangular_lattice(conf_name='Tetrahedra'):
     from asd.core.geometry import build_latt
-    if lat_type=='triangular':
-        if order_name=='tetrahedra':
-            latt,sites = build_latt(lat_type,2,2,1,return_neigh=False)
-            sp_lat = np.zeros((2,2,1,3),float)
-            sp_lat[0,0,0] = np.array([1,1,1])
-            sp_lat[1,0,0] = np.array([-1,-1,1])
-            sp_lat[0,1,0] = np.array([1,-1,-1])
-            sp_lat[1,1,0] = np.array([-1,1,-1])
-            sp_lat /= np.sqrt(3)
-
-            # rotate so that one of the four spins points to [0,0,1]
-            vec = np.array([1,-1,0])*np.arccos(1/np.sqrt(3))/np.sqrt(2)
-            mat = RT.from_rotvec(vec).as_matrix()
-            sp_lat = np.dot(sp_lat,mat.T)
+    if order_name=='Tetrahedra':
+        latt,sites = build_latt(lat_type,2,2,1,return_neigh=False)
+        sp_lat = np.zeros((2,2,1,3),float)
+        sp_lat[0,0,0] = np.array([1,1,1])
+        sp_lat[1,0,0] = np.array([-1,-1,1])
+        sp_lat[0,1,0] = np.array([1,-1,-1])
+        sp_lat[1,1,0] = np.array([-1,1,-1])
+        sp_lat /= np.sqrt(3)
+
+        # rotate so that one of the four spins points to [0,0,1]
+        vec = np.array([1,-1,0])*np.arccos(1/np.sqrt(3))/np.sqrt(2)
+        mat = RT.from_rotvec(vec).as_matrix()
+        sp_lat = np.dot(sp_lat,mat.T)
     return sp_lat
 
 
-def gen_regular_order_on_honeycomb_lattice(conf_name='FM'):
-    magmom = np.zeros((2,2,2),float)
-    if conf_name=='FM': 
-        magmom[:,:,:] = 1.
-    elif conf_name=='Neel-AFM':
-        magmom[:,:,0]=1.
-        magmom[:,:,1]=-1.
-    elif conf_name=='zigzag-AFM':
-        magmom[:,0] = 1.
-        magmom[:,1] = -1.
-    elif conf_name=='stripy-AFM':
-        magmom[:,0,0] = 1.
-        magmom[:,0,1] = -1.
-        magmom[:,1,0] = -1.
-        magmom[:,1,1] = 1.
-    elif conf_name=='super-Neel-AFM':
-        magmom[0,0,0] = 1.
-        magmom[0,0,1] = -1.
-        magmom[0,1,:] = 1.
-        magmom[1,0,:] = -1.
-        magmom[1,1,0] = 1.
-        magmom[1,1,1] = -1.
+def gen_regular_order_on_honeycomb_lattice(conf_name='FM',Neel_vec=np.array([0,0,1])):
+    sp_lat = np.zeros((2,2,2,3),float)
+
+    if conf_name in ['FM','Neel','Zigzag','Stripy','super-Neel']:
+        # some colinear orders
+        magmom = np.zeros((2,2,2),float)
+        if conf_name=='FM': 
+            magmom[:,:,:] = 1.
+        elif conf_name=='Neel':
+            magmom[:,:,0]=1.
+            magmom[:,:,1]=-1.
+        elif conf_name=='Zigzag':
+            magmom[:,0] = 1.
+            magmom[:,1] = -1.
+        elif conf_name=='Stripy':
+            magmom[:,0,0] = 1.
+            magmom[:,0,1] = -1.
+            magmom[:,1,0] = -1.
+            magmom[:,1,1] = 1.
+        elif conf_name=='super-Neel':
+            magmom[0,0,0] = 1.
+            magmom[0,0,1] = -1.
+            magmom[0,1,:] = 1.
+            magmom[1,0,:] = -1.
+            magmom[1,1,0] = 1.
+            magmom[1,1,1] = -1.
+        sp_lat = np.einsum('...,d->...d',magmom,Neel_vec)
+
     else:
-        exit('magmom still under test')
-    return magmom
+        # some noncollinear orders
+        if conf_name=='Cubic':
+            vv = np.mgrid[-1:2:2,-1:2:2,-1:2:2]
+            vv = np.array(vv,float)/np.sqrt(3)
+            sp_lat = np.transpose(vv,(1,2,3,0))
+        elif conf_name=='Tetrahedra':
+            vv = np.array([
+            [-1,-1,-1],
+            [ 1, 1,-1],
+            [-1, 1, 1],
+            [ 1,-1, 1],
+            ])/np.sqrt(3)
+            sp_lat[0,0,0] = vv[0]
+            sp_lat[1,1,1] = vv[0]
+            sp_lat[0,0,1] = vv[1]
+            sp_lat[1,1,0] = vv[1]
+            sp_lat[1,0,0] = vv[2]
+            sp_lat[0,1,1] = vv[2]
+            sp_lat[1,0,1] = vv[3]
+            sp_lat[0,1,0] = vv[3]
+        elif conf_name=='V-shape':
+            exit('V-shaped AFM order is currently not available') 
+        else:
+            exit('conf {} not yet available'.format(conf_name))
+
+    return sp_lat
+
+
+def regular_order(lat_type='triangular',order_name='Tetrahedra',Neel_vec=np.array([0,0,1])):
+    if lat_type=='triangular': sp_lat = gen_regular_order_on_triangular_lattice(order_name)
+    if lat_type=='honeycomb':  sp_lat = gen_regular_order_on_honeycomb_lattice(order_name,Neel_vec=Neel_vec)
+    return sp_lat 
 
 
 def visualize_spin_conf(latt,sites,sp_lat,title='initial spin'):
     from asd.utility.spin_visualize_tools import plot_spin_2d,quiver_kws
     sites_cart = np.dot(sites,latt)
     nx,ny=sp_lat.shape[:2]
     superlatt=np.dot([[nx,0],[0,ny]],latt)
```

### Comparing `pyasd-0.0.7/asd/core/spin_correlations.py` & `pyasd-0.0.8/asd/core/spin_correlations.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/core/topological_charge.py` & `pyasd-0.0.8/asd/core/topological_charge.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,17 @@
     return tri_simplices
 
 
 def calc_topo_chg(spins,sites=None,tri_simplices=None,pbc=[0,0,0],spatial_resolved=False,solid_angle_method=2):
     check_sp_lat_norm(spins)
     all_spins=spins.reshape(-1,3)
     if tri_simplices is None and sites is not None: 
-        assert np.prod(spins.shape[:-1])==np.prod(sites.shape[:-1]),'No. of spins and sites inconsistent!'
+        n1 = np.prod(spins.shape[:-1])
+        n2 = np.prod(sites.shape[:-1])
+        assert n1==n2,'No. of spins {} and sites {} inconsistent!'.format(n1,n2)
         tri_simplices = get_tri_simplices(sites)
     assert solid_angle_method in [1,2], 'valid value for solid_angle_method: 1 or 2'
     if solid_angle_method==1:   Q_distri = np.array([calc_solid_angle_1(*tuple(all_spins[idx])) for idx in tri_simplices])
     if solid_angle_method==2:   Q_distri = np.array([calc_solid_angle_2(*tuple(all_spins[idx])) for idx in tri_simplices])
     Q = np.sum(Q_distri)/4/np.pi
     if spatial_resolved: return tri_simplices,Q_distri,Q
     else: return Q
```

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_Cr2I3X3.py` & `pyasd-0.0.8/asd/data_base/exchange_for_Cr2I3X3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_CrI3.py` & `pyasd-0.0.8/asd/data_base/exchange_for_CrI3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_CrMnI6_U2.py` & `pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_CrMnI6_U4.py` & `pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_U4.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_CrMnI6_rect.py` & `pyasd-0.0.8/asd/data_base/exchange_for_CrMnI6_rect.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_Gd2C.py` & `pyasd-0.0.8/asd/data_base/exchange_for_Gd2C.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_MnI2.py` & `pyasd-0.0.8/asd/data_base/exchange_for_MnI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_NiI2.py` & `pyasd-0.0.8/asd/data_base/exchange_for_NiI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_RuCl3.py` & `pyasd-0.0.8/asd/data_base/exchange_for_RuCl3.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_VOI2.py` & `pyasd-0.0.8/asd/data_base/exchange_for_VOI2.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_kagome.py` & `pyasd-0.0.8/asd/data_base/exchange_for_kagome.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/data_base/exchange_for_skx.py` & `pyasd-0.0.8/asd/data_base/exchange_for_skx.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/mpi/mpi_tools.py` & `pyasd-0.0.8/asd/mpi/mpi_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/Swq.py` & `pyasd-0.0.8/asd/utility/Swq.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/analyze_Spirit_results.py` & `pyasd-0.0.8/asd/utility/analyze_Spirit_results.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/asd_arguments.py` & `pyasd-0.0.8/asd/utility/asd_arguments.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/auxiliary_colormaps.py` & `pyasd-0.0.8/asd/utility/auxiliary_colormaps.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/curve_fit.py` & `pyasd-0.0.8/asd/utility/curve_fit.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/four_state_tools.py` & `pyasd-0.0.8/asd/utility/four_state_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/head_figlet.py` & `pyasd-0.0.8/asd/utility/head_figlet.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/mag_thermal.py` & `pyasd-0.0.8/asd/utility/mag_thermal.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/ovf_tools.py` & `pyasd-0.0.8/asd/utility/ovf_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/plot_tools_3d.py` & `pyasd-0.0.8/asd/utility/plot_tools_3d.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/post_llg.py` & `pyasd-0.0.8/asd/utility/post_llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/post_mc.py` & `pyasd-0.0.8/asd/utility/post_mc.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/spin_visualize_tools.py` & `pyasd-0.0.8/asd/utility/spin_visualize_tools.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/asd/utility/spirit_tool.py` & `pyasd-0.0.8/asd/utility/spirit_tool.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/examples/example1/.coverage` & `pyasd-0.0.8/examples/example1/.coverage`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/examples/example1/single_spin_LLG.py` & `pyasd-0.0.8/examples/example1/single_spin_LLG.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/examples/example2/llg.py` & `pyasd-0.0.8/examples/example2/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/examples/example3/llg.py` & `pyasd-0.0.8/examples/example3/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/examples/example4/llg.py` & `pyasd-0.0.8/examples/example4/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/misc/archives/ovf-0.4.3.tar.gz` & `pyasd-0.0.8/misc/archives/ovf-0.4.3.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/misc/archives/pyfiglet-0.7.tar.gz` & `pyasd-0.0.8/misc/archives/pyfiglet-0.7.tar.gz`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/pyasd.egg-info/SOURCES.txt` & `pyasd-0.0.8/pyasd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 tests_basic/mag_confs/domain_walls/dw_test.py
 tests_basic/mag_confs/meron/Meron-anti-meron-latt.py
 tests_basic/mag_confs/meron/bimeron.py
 tests_basic/mag_confs/meron/contrast_vorticity_helicity.py
 tests_basic/mag_confs/meron/meron.py
 tests_basic/mag_confs/misc/interpolate_images.py
 tests_basic/mag_confs/misc/mpi_topo.py
-tests_basic/mag_confs/misc/regular_order_test.py
 tests_basic/mag_confs/misc/struct_factor.py
 tests_basic/mag_confs/misc/test_pbc_shell.py
+tests_basic/mag_confs/regular_magnetic_orders/regular_order_test.py
 tests_basic/mag_confs/skyrmion/Skyrmion.py
 tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py
 tests_basic/mag_confs/skyrmion/a2sk.py
 tests_basic/mag_confs/skyrmion/afm_skyrmion.py
 tests_basic/mag_confs/skyrmion/firework.py
 tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py
 tests_basic/mag_confs/skyrmion/input.cfg
@@ -111,10 +111,10 @@
 tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py
 tests_basic/total_energy/large_test/README
 tests_basic/total_energy/large_test/large_cell.py
 tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py
 tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py
 tests_basic/total_energy/local_energy/CrMnI6_test.py
 tests_basic/total_energy/local_energy/test_local_en.py
-tests_basic/total_energy/regular_orders/honeycomb_Heisenberg_phase_diagram.py
 tests_basic/total_energy/regular_orders/llg.py
-tests_basic/total_energy/regular_orders/phase_diagram_tri.py
+tests_basic/total_energy/regular_orders/phase_diagram_honeycomb.py
+tests_basic/total_energy/regular_orders/phase_diagram_triangular.py
```

### Comparing `pyasd-0.0.7/pyasd.egg-info/top_level.txt` & `pyasd-0.0.8/pyasd.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/setup.py` & `pyasd-0.0.8/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,56 +9,20 @@
 #===========================================================================#
 
 
 from __future__ import print_function
 import sys
 import os
 import glob
+from utility_setup import *
 import time
 #from distutils.core import setup  # deprecated soon
 import setuptools
 
 
-def set_path(bin_dirs):
-    current_path = os.environ['PATH'].split(os.pathsep)
-    for bin_dir in bin_dirs:
-        binpath="export PATH=\$PATH:{0}".format(bin_dir)
-        print ('\nThe directory containing executive files is:\n{}'.format(bin_dir))
-        if sys.platform=='linux':
-            print ('Linux/Unix operating system')
-            add_binpath = 'echo "{0}"|cat >>~/.bashrc'.format(binpath)
-            if bin_dir not in current_path:  os.system(add_binpath)
-            else:  print ('The utility directory already in the path\n')
-        elif sys.platform=='win32':
-            print ('Windows operating system')
-            print ('Please add the path to enviroment variable manually')
-
-
-
-def test_modules(module_list,desc,pkg='asd'):
-    import importlib
-    cwd=os.getcwd()
-    os.chdir(os.path.expanduser('~'))
-    print ( '\n{0}\nTEST: {1}\n{0}'.format('='*50,desc))
-    print ( '{:40s} {:10s}\n{}'.format('MODULE','STATUS','-'*50))
-    for mod in module_list:
-        try:
-            if sys.platform=='linux': mod = mod.replace('/','.')
-            elif sys.platform=='win32': mod = mod.replace('\\','.').replace('/','.')
-            importlib.import_module(mod)
-            print('{0:40s} success'.format(mod))
-        except:
-            print('{0:40s} failed!'.format(mod))
-    print('{0}\n'.format('='*50))
-    for item in glob.glob('*pyc'): os.remove(item)
-    if os.path.isdir('__pycache__'): shutil.rmtree('__pycache__')
-    os.chdir(cwd)
-
-
-
 core_modules = [
 'constants',
 'random_vectors',
 'shell_exchange',
 'geometry',
 'spin_configurations',
 'spin_correlations',
@@ -95,27 +59,28 @@
 core_modules  = ['asd/core/{}'.format(item) for item in core_modules]
 utility_modules  = ['asd/utility/{}'.format(item) for item in utility_modules]
 mpi_modules = ['asd/mpi/mpi_tools']
 
 
 kwargs_setup = dict(
 name='pyasd',
-version='0.0.7',
+version='0.0.8',
 author='Shunhong Zhang',
 author_email='zhangshunhong.pku@gmail.com',
+platform=sys.platform,
 url='https://to_be_posted',
 download_url='https://on_request',
 keywords='spin dynamics simulation',
 py_modules = utility_modules + core_modules + database_modules + mpi_modules + init_files,
 packages = setuptools.find_packages(),
 license='LICENSE',
 license_file='LICENSE',
 description='A python-based spin dynamics simulator',
 long_description='LLG/Monte Carlo/GNEB simulators for classical spin systems',
-platforms=sys.platform,
+platforms=[sys.platform],
 install_requires=[
 'numpy',
 'scipy',
 'matplotlib',
 'mpi4py',
 'pyfiglet',
 'ovf'],
@@ -127,22 +92,20 @@
 bindirs = ['{}/asd/utility'.format(os.getcwd())]
 
 
 def set_build_time_stamp(kwargs_setup):
     import locale
     with open('asd/__init__.py','r') as fw: lines = fw.readlines()
     __doc__ = '{:<20s}  =  "built at {}'.format('__built_time__',time.ctime())
-    try:  loc0 = locale.getlocale()[0]
-    except:  loc0 = locale.getdefaultlocale()[0]
-    if loc0=='en_US': __doc__ += '_{}"\n'.format(time.tzname[1])
+    if locale.getdefaultlocale()[0]=='en_US': __doc__ += '_{}"\n'.format(time.tzname[1])
     else: __doc__ += '"\n'
     lines = [__doc__] + [line for line in lines if '__built_time__' not in line]
     with open('asd/__init__.py','w') as fw: 
         fw.write(__doc__)
-        for key in ['__name__','__version__','__author__','__author_email__','__url__','__license__','__platforms__']:
+        for key in ['__name__','__version__','__author__','__author_email__','__url__','__license__','__platform__']:
             print ('{:<20s}  =  "{}"'.format(key,kwargs_setup[key.strip('__')]),file=fw)
  
  
  
 if __name__=='__main__':
     set_build_time_stamp(kwargs_setup)
     print('\n{0}\nINSTALL\n{0}'.format('='*50))
```

### Comparing `pyasd-0.0.7/tests_basic/B_eff/test_B_eff.py` & `pyasd-0.0.8/tests_basic/B_eff/test_B_eff.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/OVF/pyasd_ovf_test.py` & `pyasd-0.0.8/tests_basic/OVF/pyasd_ovf_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/OVF/test_ovf.py` & `pyasd-0.0.8/tests_basic/OVF/test_ovf.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/Potts/Potts_test.py` & `pyasd-0.0.8/tests_basic/mag_confs/Potts/Potts_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/domain_walls/analytical_single_domain.py` & `pyasd-0.0.8/tests_basic/mag_confs/domain_walls/analytical_single_domain.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/domain_walls/dw_test.py` & `pyasd-0.0.8/tests_basic/mag_confs/domain_walls/dw_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/interpolate_images.py` & `pyasd-0.0.8/tests_basic/mag_confs/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py` & `pyasd-0.0.8/tests_basic/mag_confs/meron/Meron-anti-meron-latt.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/meron/bimeron.py` & `pyasd-0.0.8/tests_basic/mag_confs/meron/bimeron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py` & `pyasd-0.0.8/tests_basic/mag_confs/meron/contrast_vorticity_helicity.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/meron/meron.py` & `pyasd-0.0.8/tests_basic/mag_confs/meron/meron.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/misc/interpolate_images.py` & `pyasd-0.0.8/tests_basic/mag_confs/misc/interpolate_images.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/misc/mpi_topo.py` & `pyasd-0.0.8/tests_basic/mag_confs/misc/mpi_topo.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/misc/struct_factor.py` & `pyasd-0.0.8/tests_basic/mag_confs/misc/struct_factor.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/misc/test_pbc_shell.py` & `pyasd-0.0.8/tests_basic/mag_confs/misc/test_pbc_shell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/Skyrmion.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/Spirit_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/a2sk.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/a2sk.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/afm_skyrmion.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/afm_skyrmion.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/firework.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/gen_skyr_Mz.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/mpi_firework.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/mpi_firework.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/skyrmionium.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/skyrmionium.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/skyrmion/view_3d_skyr.py` & `pyasd-0.0.8/tests_basic/mag_confs/skyrmion/view_3d_skyr.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/spirals/CrMnI6_spiral.py` & `pyasd-0.0.8/tests_basic/mag_confs/spirals/CrMnI6_spiral.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/spirals/spiral_test.py` & `pyasd-0.0.8/tests_basic/mag_confs/spirals/spiral_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/mag_confs/test_regular_orders_honeycomb.py` & `pyasd-0.0.8/tests_basic/mag_confs/test_regular_orders_honeycomb.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py` & `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/honeycomb/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py` & `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py` & `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py` & `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/triangular/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py` & `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/complex_ham/vis_plaquttes.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/simple/input.cfg` & `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/input.cfg`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py` & `pyasd-0.0.8/tests_basic/total_energy/benchmark_spirit/simple/test_tot_E.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py` & `pyasd-0.0.8/tests_basic/total_energy/chiral_confs/test_chiral_magnet_energy.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/large_test/large_cell.py` & `pyasd-0.0.8/tests_basic/total_energy/large_test/large_cell.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py` & `pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/rect_CrMnI6_test.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py` & `pyasd-0.0.8/tests_basic/total_energy/large_test/test_loop_methods/square_2NN.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/local_energy/test_local_en.py` & `pyasd-0.0.8/tests_basic/total_energy/local_energy/test_local_en.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/regular_orders/llg.py` & `pyasd-0.0.8/tests_basic/total_energy/regular_orders/llg.py`

 * *Files identical despite different names*

### Comparing `pyasd-0.0.7/tests_basic/total_energy/regular_orders/phase_diagram_tri.py` & `pyasd-0.0.8/tests_basic/total_energy/regular_orders/phase_diagram_triangular.py`

 * *Files identical despite different names*

