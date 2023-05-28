# Comparing `tmp/pyhalo-0.2.1.tar.gz` & `tmp/pyhalo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhalo-0.2.1.tar", last modified: Wed May 24 16:06:12 2023, max compression
+gzip compressed data, was "pyhalo-0.2.2.tar", last modified: Sun May 28 04:58:19 2023, max compression
```

## Comparing `pyhalo-0.2.1.tar` & `pyhalo-0.2.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.597891 pyhalo-0.2.1/
--rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.1/AUTHORS.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.1/HISTORY.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.1/LICENSE
--rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.1/MANIFEST.in
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-24 16:06:12.596954 pyhalo-0.2.1/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     1998 2023-05-18 15:44:57.000000 pyhalo-0.2.1/README.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.485276 pyhalo-0.2.1/docs/
--rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/Makefile
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/authors.rst
--rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.1/docs/conf.py
--rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/contributing.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/history.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/index.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/installation.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/make.bat
--rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/readme.rst
--rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.1/docs/usage.rst
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.495010 pyhalo-0.2.1/pyHalo/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.501973 pyhalo-0.2.1/pyHalo/Cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.1/pyHalo/Cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Cosmology/cosmology.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Cosmology/geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.506981 pyhalo-0.2.1/pyHalo/Halos/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.516430 pyhalo-0.2.1/pyHalo/Halos/HaloModels/
--rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/NFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/PTMass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/PsuedoJaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3967 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/TNFW.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/TNFWemulator.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/ULDM.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/generalized_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.1/pyHalo/Halos/HaloModels/powerlaw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.1/pyHalo/Halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8643 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/concentration.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5373 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/halo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/lens_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10172 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/tidal_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Halos/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.525528 pyhalo-0.2.1/pyHalo/Rendering/
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.531565 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/density_peaks.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/mass_function_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/util.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.537964 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3156 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4384 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.1/pyHalo/Rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/correlated_structure.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/halo_population.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4621 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/line_of_sight.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/rendering_class_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5972 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/Rendering/two_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.1/pyHalo/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/concentration_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/defaults.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    46842 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/pyhalo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/realization_extensions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    36187 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1176 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/truncation_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    13604 2023-05-18 15:44:57.000000 pyhalo-0.2.1/pyHalo/utilities.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.499773 pyhalo-0.2.1/pyHalo.egg-info/
--rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/PKG-INFO
--rw-r--r--   0 danielgilman   (501) staff       (20)     3893 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/SOURCES.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/dependency_links.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/entry_points.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.1/pyHalo.egg-info/not-zip-safe
--rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/requires.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-05-24 16:06:12.000000 pyhalo-0.2.1/pyHalo.egg-info/top_level.txt
--rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-24 16:05:34.000000 pyhalo-0.2.1/pyproject.toml
--rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-05-24 16:06:12.598186 pyhalo-0.2.1/setup.cfg
--rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.1/setup.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.557114 pyhalo-0.2.1/tests/
--rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.1/tests/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_concentration_models.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.560510 pyhalo-0.2.1/tests/test_cosmology/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.1/tests/test_cosmology/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_cosmology/test_cone_geometry.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_cosmology/test_cosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_cosmology/test_cylinder_geometry.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.587367 pyhalo-0.2.1/tests/test_halos/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.1/tests/test_halos/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3025 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_adiabatic_tides.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_concentrations.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_gaussian.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.1/tests/test_halos/test_general_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_lenscosmo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_nfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_pjaffe.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_point_mass.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.1/tests/test_halos/test_powerlaw_profile.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_tnfw_halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2401 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_truncation.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_uldm.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_halos/test_util.py
--rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_mass_function_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_preset_models.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_pyhalo_base.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_realization_extensions.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.590775 pyhalo-0.2.1/tests/test_rendering/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.1/tests/test_rendering/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_2halo.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_los.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.593581 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_base_functions.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_delta_function.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_population.py
-drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-24 16:06:12.596062 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/
--rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/__init__.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_correlated.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2191 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_nfw.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_uniform.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_rendering/test_subhalos.py
--rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_single_realization.py
--rw-r--r--   0 danielgilman   (501) staff       (20)     3373 2023-05-18 15:44:57.000000 pyhalo-0.2.1/tests/test_utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.142624 pyhalo-0.2.2/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      156 2018-08-15 00:45:59.000000 pyhalo-0.2.2/AUTHORS.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3515 2018-08-15 00:45:59.000000 pyhalo-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       89 2018-08-15 00:45:59.000000 pyhalo-0.2.2/HISTORY.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1072 2018-08-15 00:45:59.000000 pyhalo-0.2.2/LICENSE
+-rw-r--r--   0 danielgilman   (501) staff       (20)      262 2018-08-15 00:45:59.000000 pyhalo-0.2.2/MANIFEST.in
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-28 04:58:19.141428 pyhalo-0.2.2/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2041 2023-05-26 19:45:13.000000 pyhalo-0.2.2/README.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.020447 pyhalo-0.2.2/docs/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      607 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/Makefile
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/authors.rst
+-rwxr-xr-x   0 danielgilman   (501) staff       (20)     4799 2018-10-06 19:25:46.000000 pyhalo-0.2.2/docs/conf.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)       33 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/contributing.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       28 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/history.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      303 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/index.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1110 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/installation.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)      768 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/make.bat
+-rw-r--r--   0 danielgilman   (501) staff       (20)       27 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/readme.rst
+-rw-r--r--   0 danielgilman   (501) staff       (20)       67 2018-08-15 00:45:59.000000 pyhalo-0.2.2/docs/usage.rst
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.034268 pyhalo-0.2.2/pyHalo/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.042832 pyhalo-0.2.2/pyHalo/Cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-08-15 00:50:13.000000 pyhalo-0.2.2/pyHalo/Cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4768 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Cosmology/cosmology.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9394 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Cosmology/geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.048176 pyhalo-0.2.2/pyHalo/Halos/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.065927 pyhalo-0.2.2/pyHalo/Halos/HaloModels/
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2920 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/NFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1515 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/PTMass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4967 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/PsuedoJaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3967 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/TNFW.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5544 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/TNFWemulator.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     9969 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/ULDM.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-11-11 08:37:06.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1575 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4561 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/generalized_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5615 2023-05-18 16:09:33.000000 pyhalo-0.2.2/pyHalo/Halos/HaloModels/powerlaw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-02-20 20:53:15.000000 pyhalo-0.2.2/pyHalo/Halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8628 2023-05-26 19:44:32.000000 pyhalo-0.2.2/pyHalo/Halos/concentration.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5423 2023-05-28 04:22:20.000000 pyhalo-0.2.2/pyHalo/Halos/halo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16076 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/lens_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8469 2023-05-28 04:43:27.000000 pyhalo-0.2.2/pyHalo/Halos/tidal_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2142 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Halos/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.077091 pyhalo-0.2.2/pyHalo/Rendering/
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.088717 pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1873 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     7019 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/density_peaks.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    10149 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/mass_function_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      883 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/util.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.094323 pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:19.000000 pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      361 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2440 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3156 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4384 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.2/pyHalo/Rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8837 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/correlated_structure.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5268 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/halo_population.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4621 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/line_of_sight.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3205 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/rendering_class_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5972 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3487 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/Rendering/two_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      149 2018-08-15 00:45:59.000000 pyhalo-0.2.2/pyHalo/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2570 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/concentration_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3846 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/defaults.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2447 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    46841 2023-05-26 19:51:20.000000 pyhalo-0.2.2/pyHalo/preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5617 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/pyhalo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    26366 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/realization_extensions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    36187 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1176 2023-05-18 15:44:57.000000 pyhalo-0.2.2/pyHalo/truncation_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    14271 2023-05-28 04:22:20.000000 pyhalo-0.2.2/pyHalo/utilities.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.040495 pyhalo-0.2.2/pyHalo.egg-info/
+-rw-r--r--   0 danielgilman   (501) staff       (20)      672 2023-05-28 04:58:18.000000 pyhalo-0.2.2/pyHalo.egg-info/PKG-INFO
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3893 2023-05-28 04:58:18.000000 pyhalo-0.2.2/pyHalo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2023-05-28 04:58:18.000000 pyhalo-0.2.2/pyHalo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       43 2023-05-28 04:58:18.000000 pyhalo-0.2.2/pyHalo.egg-info/entry_points.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)        1 2018-08-23 21:07:23.000000 pyhalo-0.2.2/pyHalo.egg-info/not-zip-safe
+-rw-r--r--   0 danielgilman   (501) staff       (20)       11 2023-05-28 04:58:18.000000 pyhalo-0.2.2/pyHalo.egg-info/requires.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)       13 2023-05-28 04:58:18.000000 pyhalo-0.2.2/pyHalo.egg-info/top_level.txt
+-rw-r--r--   0 danielgilman   (501) staff       (20)      526 2023-05-28 04:58:02.000000 pyhalo-0.2.2/pyproject.toml
+-rw-r--r--   0 danielgilman   (501) staff       (20)       38 2023-05-28 04:58:19.142909 pyhalo-0.2.2/setup.cfg
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1639 2023-05-24 16:05:34.000000 pyhalo-0.2.2/setup.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.105529 pyhalo-0.2.2/tests/
+-rw-r--r--   0 danielgilman   (501) staff       (20)       61 2018-10-06 19:25:46.000000 pyhalo-0.2.2/tests/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1688 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_concentration_models.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.109672 pyhalo-0.2.2/tests/test_cosmology/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2018-10-18 06:20:01.000000 pyhalo-0.2.2/tests/test_cosmology/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5023 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_cosmology/test_cone_geometry.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3841 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_cosmology/test_cosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3969 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_cosmology/test_cylinder_geometry.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.129610 pyhalo-0.2.2/tests/test_halos/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2019-12-04 22:13:12.000000 pyhalo-0.2.2/tests/test_halos/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2832 2023-05-28 04:43:27.000000 pyhalo-0.2.2/tests/test_halos/test_adiabatic_tides.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4220 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_concentrations.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1334 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_gaussian.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     6011 2023-05-18 16:13:37.000000 pyhalo-0.2.2/tests/test_halos/test_general_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3407 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_lenscosmo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2682 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_nfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3343 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_pjaffe.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1665 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_point_mass.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     4304 2023-05-18 16:13:19.000000 pyhalo-0.2.2/tests/test_halos/test_powerlaw_profile.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2719 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_tnfw_halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2401 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_truncation.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5002 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_uldm.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     1068 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_halos/test_util.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)      874 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_mass_function_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3224 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_preset_models.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     8793 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_pyhalo_base.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    16257 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_realization_extensions.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.134052 pyhalo-0.2.2/tests/test_rendering/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2022-04-26 14:26:20.000000 pyhalo-0.2.2/tests/test_rendering/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2584 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_2halo.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3422 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_los.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.136958 pyhalo-0.2.2/tests/test_rendering/test_mass_functions/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_mass_functions/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     5915 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_mass_functions/test_base_functions.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2173 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_mass_functions/test_delta_function.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    11175 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_mass_functions/test_sheth_tormen.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2936 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_population.py
+drwxr-xr-x   0 danielgilman   (501) staff       (20)        0 2023-05-28 04:58:19.139814 pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/
+-rw-r--r--   0 danielgilman   (501) staff       (20)        0 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/__init__.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2096 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/test_correlated.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2191 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/test_nfw.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     2153 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/test_uniform.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3491 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_rendering/test_subhalos.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)    23809 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_single_realization.py
+-rw-r--r--   0 danielgilman   (501) staff       (20)     3373 2023-05-18 15:44:57.000000 pyhalo-0.2.2/tests/test_utilities.py
```

### Comparing `pyhalo-0.2.1/CONTRIBUTING.rst` & `pyhalo-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/LICENSE` & `pyhalo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/PKG-INFO` & `pyhalo-0.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.1/README.rst` & `pyhalo-0.2.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 pyHalo renders full mass distributions for substructure lensing simulations with the open source gravitational lensing software package lenstronomy (https://github.com/sibirrer/lenstronomy). The example notebooks illustrate the core functionality of this package. 
 
 If you would like to use this package and have questions, please get in touch with me at daniel.gilman@utoronto.ca - I am happy to help! 
 
 Installation
 ------------
-Clone the repository, navigate into the directory that contains the setup.py file and run "python setup.py install"
+"python3 -m pip install pyhalo==0.2.1"
+
+Or clone the repository, navigate into the directory that contains the setup.py file and run "python setup.py install"
 
 The first code release, before majoring refactoring, is 8302393. 
 
 In order to use this package when not installing via pip, you'll need to install colossus http://www.benediktdiemer.com/code/colossus/ 
 
 Features
 --------
```

### Comparing `pyhalo-0.2.1/docs/Makefile` & `pyhalo-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/docs/conf.py` & `pyhalo-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/docs/installation.rst` & `pyhalo-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/docs/make.bat` & `pyhalo-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Cosmology/cosmology.py` & `pyhalo-0.2.2/pyHalo/Cosmology/cosmology.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Cosmology/geometry.py` & `pyhalo-0.2.2/pyHalo/Cosmology/geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/NFW.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/NFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/PTMass.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/PTMass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/PsuedoJaffe.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/PsuedoJaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/TNFW.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/TNFW.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/TNFWemulator.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/TNFWemulator.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/ULDM.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/ULDM.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/gaussian.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/generalized_nfw.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/generalized_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/HaloModels/powerlaw.py` & `pyhalo-0.2.2/pyHalo/Halos/HaloModels/powerlaw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/concentration.py` & `pyhalo-0.2.2/pyHalo/Halos/concentration.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,27 +188,27 @@
         rescale = redshift_factor * rescale_factor
         return rescale
 
 class ConcentrationWDMHyperbolic(_ConcentrationTurnover):
 
     name = 'WDM_HYPERBOLIC'
 
-    def __init__(self, lens_cosmo, concentration_cdm_class, log_mc, a,  b, scatter=True,
+    def __init__(self, cosmo, concentration_cdm_class, log_mc, a,  b, scatter=True,
                  scatter_dex=0.2, kwargs_cdm={}):
         """
 
-        :param lens_cosmo:
+        :param cosmo:
         :param concentration_cdm_class:
         :param kwargs_cdm:
         """
         if 'scatter' not in kwargs_cdm.keys():
             kwargs_cdm['scatter'] = scatter
         if 'scatter_dex' not in kwargs_cdm.keys():
             kwargs_cdm['scatter_dex'] = scatter_dex
-        cdm_concentration = concentration_cdm_class(lens_cosmo, **kwargs_cdm)
+        cdm_concentration = concentration_cdm_class(cosmo, **kwargs_cdm)
         self._a = a
         self._b = b
         self._log_mc = log_mc
         super(ConcentrationWDMHyperbolic, self).__init__(cdm_concentration)
 
     def suppression(self, m, z):
         """
```

### Comparing `pyhalo-0.2.1/pyHalo/Halos/halo_base.py` & `pyhalo-0.2.2/pyHalo/Halos/halo_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABC, abstractmethod
 import numpy as np
-import inspect
 from pyHalo.utilities import ITSampling
-_path_galacticus_data_testing = inspect.getfile(inspect.currentframe())[0:-13]+'/adiabatic_tides_data/galacticus_data.txt'
-_path_galacticus_data_run = inspect.getfile(inspect.currentframe())[0:-8]+'/adiabatic_tides_data/galacticus_data.txt'
-try:
-    _rperi_sampling = ITSampling(np.loadtxt(_path_galacticus_data_run)[:,0])
-except:
-    _rperi_sampling = ITSampling(np.loadtxt(_path_galacticus_data_testing)[:,0])
+
+_log10_rperi_bins = np.array([-2.   , -1.885, -1.77 , -1.655, -1.54 , -1.425, -1.31 , -1.195,
+       -1.08 , -0.965, -0.85 , -0.735, -0.62 , -0.505, -0.39 , -0.275,
+       -0.16 , -0.045,  0.07 ,  0.185])
+_log10_prob = np.array([  18,   23,   37,   33,   42,   78,  139,  181,  321,  538,  749,
+       1018, 1268, 1501, 1577, 1232,  569,  207,   23,    7])
+_cdf = np.cumsum(_log10_prob)
+_log10_rpericenter_sampling = ITSampling(_log10_rperi_bins, _cdf)
 
 class Halo(ABC):
 
     def __init__(self, mass=None, x=None, y=None, r3d=None, mdef=None, z=None,
                  sub_flag=None, lens_cosmo_instance=None, args={}, unique_tag=None, fixed_position=False):
 
         """
@@ -135,14 +136,14 @@
         :return:
         """
         if not self.is_subhalo:
             print("Orbital pericenter is a meaningless concept for field halos. It is possible you assigned a tidal "
                   "truncation model that requires this information to field halos.")
             return None
         if not hasattr(self, '_rperi_units_r200'):
-            self._rperi_units_r200 = _rperi_sampling(n_samples=1.0)
+            self._rperi_units_r200 = 10**float(_log10_rpericenter_sampling(n_samples=1.0))
         return self._rperi_units_r200
```

### Comparing `pyhalo-0.2.1/pyHalo/Halos/lens_cosmo.py` & `pyhalo-0.2.2/pyHalo/Halos/lens_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Halos/tidal_truncation.py` & `pyhalo-0.2.2/pyHalo/Halos/tidal_truncation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import numpy as np
-import inspect
 import pickle
-import inspect
 from pyHalo.Halos.concentration import ConcentrationDiemerJoyce
 from scipy.interpolate import RegularGridInterpolator
 from pyHalo.Halos.util import tau_mf_interpolation
 from colossus.lss import peaks
 from colossus.halo import splashback
-_path_testing = inspect.getfile(inspect.currentframe())[0:-29]+'/adiabatic_tides_data/'
-_path_run = inspect.getfile(inspect.currentframe())[0:-20]+'/adiabatic_tides_data/'
+
 
 class TruncationSplashBack(object):
 
     def __init__(self, lens_cosmo):
         """
         This computes the splashback radius of a halo as the truncation radius (appropriate for field halos)
         See Diemer (2020)
@@ -118,55 +115,37 @@
         return np.round(rtrunc_kpc, 3)
 
 class AdiabaticTidesTruncation(object):
     """
     An example of the type of class we want to create and implement in pyHalo
     """
 
-    def __init__(self, lens_cosmo, log_m_host, z_host, log10_galaxy_rs=np.log10(0.5),
-                 log10_galaxy_m=np.log10(0.1), mass_loss_interp=None, pyhalo_home_directory=''):
+    def __init__(self, lens_cosmo, log_m_host, z_host, mass_loss_interp):
         """
 
-        :param lens_cosmo:
-        :param log_m_host:
-        :param z_host:
-        :param log10_galaxy_rs:
-        :param log10_galaxy_m:
-        :param mass_loss_interp:
-        :param pyhalo_home_directory:
-        """
-
-        if mass_loss_interp is None:
-            m_host_list = np.array([13.0])
-            z_host_list = np.array([0.5])
-            fnames = ['13.0_z0.5']
-            fname_base = pyhalo_home_directory + '/pyHalo/Halos/adiabatic_tides_data/subhalo_mass_loss_interp_mhost'
-            dmhost = abs(m_host_list - log_m_host) / 0.1
-            d_zhost = abs(z_host_list - z_host) / 0.2
-            penalty = dmhost + d_zhost
-            idx_min = np.argsort(penalty)[0]
-            fname = fname_base + fnames[idx_min]
-            f = open(fname, 'rb')
-            self._mass_loss_interp = pickle.load(f)
-            f.close()
-        else:
-            self._mass_loss_interp = mass_loss_interp
-
+        :param lens_cosmo: an instacee of the LensCosmo class
+        :param log_m_host: the host halo mass
+        :param z_host: the redshift of the host halo
+        :param mass_loss_interp: an instance of RegularGridInterpolator
+        The interpolator should take as input a point
+        (log10(concentration), log10(r_pericenter), c_host) and return the
+        asymptotic final bound mass divided by the infall mass
+        """
+        self._mass_loss_interp = mass_loss_interp
         min_max_c = [1.0, 10 ** 2.7]
-        min_max_rperi = [10 ** -2.5, 1.0]
+        min_max_rperi = [10 ** -2.0, 10 ** 0.2]
         self._lens_cosmo = lens_cosmo
         cmodel = ConcentrationDiemerJoyce(self._lens_cosmo.cosmo.astropy, scatter=False)
         c_host = cmodel.nfw_concentration(10**log_m_host, z_host)
+        self._chost = c_host
         self._host_dynamical_time = self._lens_cosmo.halo_dynamical_time(10**log_m_host, z_host, c_host)
         self._min_c = min_max_c[0]
         self._max_c = min_max_c[1]
         self._min_rperi = min_max_rperi[0]
         self._max_rperi = min_max_rperi[1]
-        self._log10_galaxy_rs = log10_galaxy_rs
-        self._log10_galaxy_m = log10_galaxy_m
         self._tau_mf_interpolation = tau_mf_interpolation()
 
     def truncation_radius_halo(self, halo):
         """
         This function solves for the truncation radius divided by the halo scale radius (tau) given an instance of
         Halo (see pyhalo.HaloModels.TNFW) and other arguments for the interpolation function
 
@@ -175,21 +154,19 @@
         :return tau: the truncation radius divided by the halo's scale radius
         """
 
         # compute the halo parameeters
         c = halo.c
         # now make sure that the points are inside the region where we computed the interpolation
         r_pericenter_over_r200 = np.absolute(halo.rperi_units_r200)
-        if r_pericenter_over_r200 > self._max_rperi:
-            r_pericenter_over_r200 = self._max_rperi
-        if r_pericenter_over_r200 < self._min_rperi:
-            r_pericenter_over_r200 = self._min_rperi
-        point = (np.log10(c), np.log10(r_pericenter_over_r200), self._log10_galaxy_rs, self._log10_galaxy_m)
-        point = self._make_params_in_bounds(point)
-
+        r_pericenter_over_r200 = max(self._min_rperi, r_pericenter_over_r200)
+        r_pericenter_over_r200 = min(self._max_rperi, r_pericenter_over_r200)
+        c = max(self._min_c, c)
+        c = min(self._max_c, c)
+        point = (np.log10(c), np.log10(r_pericenter_over_r200), self._chost)
         # evaluate the mass loss
         log10mass_loss_fraction_asymptotic = float(self._mass_loss_interp(point))
 
         time_since_infall = halo.time_since_infall
         n_orbits = time_since_infall / self._host_dynamical_time
         mass_loss_fraction = self._temporal_mass_loss(10 ** log10mass_loss_fraction_asymptotic, n_orbits)
         log10mass_loss_fraction = np.log10(mass_loss_fraction)
@@ -218,23 +195,7 @@
         """
         (log10c, log10mass_loss_fraction) = point
         log10c = max(self._min_c, log10c)
         log10c = min(self._max_c, log10c)
         log10mass_loss_fraction = max(-1.5, log10mass_loss_fraction)
         log10mass_loss_fraction = min(-0.01, log10mass_loss_fraction)
         return (log10c, log10mass_loss_fraction)
-
-    def _make_params_in_bounds(self, point):
-        """
-        This routine makes sure the arguments for the initerpolation are inside the domain of the function.
-        """
-        (log10c, log10r_pericenter_over_r200, log10_galaxy_rs, log10_galaxy_m) = point
-        log10c = max(self._min_c, log10c)
-        log10c = min(self._max_c, log10c)
-        log10r_pericenter_over_r200 = max(-2.5, log10r_pericenter_over_r200)
-        log10r_pericenter_over_r200 = min(0.0, log10r_pericenter_over_r200)
-        log10_galaxy_rs = max(-2.0, log10_galaxy_rs)
-        log10_galaxy_rs = min(0.3, log10_galaxy_rs)
-        log10_galaxy_m = max(-2.5, log10_galaxy_m)
-        log10_galaxy_m = min(-0.25, log10_galaxy_m)
-        new_point = (log10c, log10r_pericenter_over_r200, log10_galaxy_rs, log10_galaxy_m)
-        return new_point
```

### Comparing `pyhalo-0.2.1/pyHalo/Halos/util.py` & `pyhalo-0.2.2/pyHalo/Halos/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/delta_function.py` & `pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/density_peaks.py` & `pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/density_peaks.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/mass_function_base.py` & `pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/mass_function_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/MassFunctions/util.py` & `pyhalo-0.2.2/pyHalo/Rendering/MassFunctions/util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/correlated.py` & `pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/nfw.py` & `pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/SpatialDistributions/uniform.py` & `pyhalo-0.2.2/pyHalo/Rendering/SpatialDistributions/uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/correlated_structure.py` & `pyhalo-0.2.2/pyHalo/Rendering/correlated_structure.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/halo_population.py` & `pyhalo-0.2.2/pyHalo/Rendering/halo_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/line_of_sight.py` & `pyhalo-0.2.2/pyHalo/Rendering/line_of_sight.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/rendering_class_base.py` & `pyhalo-0.2.2/pyHalo/Rendering/rendering_class_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/subhalos.py` & `pyhalo-0.2.2/pyHalo/Rendering/subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/Rendering/two_halo.py` & `pyhalo-0.2.2/pyHalo/Rendering/two_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/concentration_models.py` & `pyhalo-0.2.2/pyHalo/concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/defaults.py` & `pyhalo-0.2.2/pyHalo/defaults.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/mass_function_models.py` & `pyhalo-0.2.2/pyHalo/mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/preset_models.py` & `pyhalo-0.2.2/pyHalo/preset_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,14 @@
                          'kwargs_density_profile': {}}
 
     realization_list = pyhalo.render(population_model_list, mass_function_class_list, kwargs_mass_function_list,
                                           spatial_distribution_class_list, kwargs_spatial_distribution_list,
                                           geometry, mdef_subhalos, mdef_field_halos, kwargs_halo_model, nrealizations=1)
     return realization_list[0]
 
-
 def WDM(z_lens, z_source, log_mc, sigma_sub=0.025, log_mlow=6., log_mhigh=10.,
         mass_function_model_subhalos='LOVELL2020', kwargs_mass_function_subhalos={},
         mass_function_model_fieldhalos='LOVELL2020', kwargs_mass_function_fieldhalos={},
         concentration_model_subhalos='BOSE2016', kwargs_concentration_model_subhalos={},
         concentration_model_fieldhalos='BOSE2016', kwargs_concentration_model_fieldhalos={},
         truncation_model_subhalos='TRUNCATION_ROCHE_GILMAN2020', kwargs_trunction_model_subhalos={},
         truncation_model_fieldhalos='TRUNCATION_RN', kwargs_truncation_model_fieldhalos={},
```

### Comparing `pyhalo-0.2.1/pyHalo/pyhalo.py` & `pyhalo-0.2.2/pyHalo/pyhalo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/realization_extensions.py` & `pyhalo-0.2.2/pyHalo/realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/single_realization.py` & `pyhalo-0.2.2/pyHalo/single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/truncation_models.py` & `pyhalo-0.2.2/pyHalo/truncation_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyHalo/utilities.py` & `pyhalo-0.2.2/pyHalo/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,38 @@
 from scipy.integrate import quad
 from pyHalo.Halos.lens_cosmo import LensCosmo
 from scipy.integrate import simps
 from pyHalo.concentration_models import preset_concentration_models
 
 class ITSampling(object):
 
-    def __init__(self, samples):
+    def __init__(self, x, cdf):
         """
         This class performs inverse transform sampling of a distribution given samples from the distribution
         :param samples: samples from the distribution
         """
-        ran = (np.min(samples), np.max(samples))
-        h, x = np.histogram(samples, range=ran, bins=150)
-        x = x[0:-1] + (x[1] - x[0])/2
-        cdf = np.cumsum(h)
         cdf = cdf / float(np.max(cdf))
         self._cdf_inverse = interp1d(cdf, x)
         self._umin = cdf[0]
         self._umax = cdf[-1]
 
+    @classmethod
+    def from_samples(cls, samples):
+        """
+        samples from the target distribution
+        :param samples:
+        :return:
+        """
+        ran = (np.min(samples), np.max(samples))
+        h, x = np.histogram(samples, range=ran, bins=150)
+        x = x[0:-1] + (x[1] - x[0]) / 2
+        cdf = np.cumsum(h)
+        cdf = cdf / float(np.max(cdf))
+        return ITSampling(x, cdf)
+
     def __call__(self, n_samples):
         """
         Generates samples from the distribution
         :param n_samples: number of samples to draw
         :return: the samples
         """
         u = np.random.uniform(self._umin, self._umax, int(n_samples))
@@ -43,15 +53,25 @@
     :param function: the function or probability density you want to sample from
     :param args: arguments passed to function after x
     :param n_samples: number of samples to draw
     :return: samples from the probability density described by function
     """
     y = function(x, *args)
     cdf = np.cumsum(y)
-    cdf /= np.max(cdf)
+    return inverse_transform_sampling_from_cdf(x, cdf, n_samples)
+
+def inverse_transform_sampling_from_cdf(x, cdf, n_samples):
+    """
+
+    :param x: the domain of the function across which you want to obtain samples
+    :param cdf: the cumulative distribution function of the pdf
+    :param n_samples: number of samples to draw
+    :return: samples from the probability density that corresponds to cdf
+    """
+    cdf = cdf * float(np.max(cdf)) ** -1
     cdf_inverse = interp1d(cdf, x)
     u = np.random.uniform(cdf[0], cdf[-1], n_samples)
     return cdf_inverse(u)
 
 def generate_lens_plane_redshifts(zlens, zsource):
     """
     This routine sets up the redshift planes along the line of sight in the lens system
```

### Comparing `pyhalo-0.2.1/pyHalo.egg-info/PKG-INFO` & `pyhalo-0.2.2/pyHalo.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhalo
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package for generating populations of dark matter halos
 Home-page: https://github.com/dangilman/pyHalo
 Author: Daniel Gilman
 Author-email: Daniel Gilman <daniel.gilman@utoronto.ca>
 License: MIT license
 Project-URL: Homepage, https://github.com/dangilman/pyHalo
 Project-URL: Bug Tracker, https://github.com/dangilman/pyHalo/issues
```

### Comparing `pyhalo-0.2.1/pyHalo.egg-info/SOURCES.txt` & `pyhalo-0.2.2/pyHalo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/pyproject.toml` & `pyhalo-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyhalo"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Daniel Gilman", email="daniel.gilman@utoronto.ca" },
 ]
 description = "A python package for generating populations of dark matter halos"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyhalo-0.2.1/setup.py` & `pyhalo-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_concentration_models.py` & `pyhalo-0.2.2/tests/test_concentration_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_cosmology/test_cone_geometry.py` & `pyhalo-0.2.2/tests/test_cosmology/test_cone_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_cosmology/test_cosmo.py` & `pyhalo-0.2.2/tests/test_cosmology/test_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_cosmology/test_cylinder_geometry.py` & `pyhalo-0.2.2/tests/test_cosmology/test_cylinder_geometry.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_adiabatic_tides.py` & `pyhalo-0.2.2/tests/test_halos/test_adiabatic_tides.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,25 @@
 from pyHalo.Halos.lens_cosmo import LensCosmo
 import numpy as np
 
 class DummyInterp(object):
 
     def __call__(self, x):
         #np.log10(c), np.log10(r_pericenter_over_r200), self._log10_galaxy_rs, self._log10_galaxy_m
-        (log10c, log10_rperi_r200, log10_galrs, log10_galm) = x
+        (log10c, log10_rperi_r200, chost) = x
         rperi_term = (10**log10_rperi_r200 / 1.0) ** 2
         c_term = (10**log10c / 500) **0.5
         return np.log10(c_term * rperi_term)
 
 class TestAdiabaticTides(object):
 
     def setup_method(self):
         self.lens_cosmo_instance = LensCosmo(0.5, 1.5)
-        log10_galaxy_rs, log10_galaxy_m, host_dynamical_time = np.log10(0.5), np.log10(0.25), 1.0
         self.att = AdiabaticTidesTruncation(self.lens_cosmo_instance,
-                                            13.3, 0.5, log10_galaxy_rs, log10_galaxy_m,
-                                            mass_loss_interp=DummyInterp())
+                                            13.3, 0.5, mass_loss_interp=DummyInterp())
 
 
     def test_rt(self):
 
         mass = 10 ** 8.0
         x = 0.1
         y = 0.5
```

### Comparing `pyhalo-0.2.1/tests/test_halos/test_concentrations.py` & `pyhalo-0.2.2/tests/test_halos/test_concentrations.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_gaussian.py` & `pyhalo-0.2.2/tests/test_halos/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_general_nfw.py` & `pyhalo-0.2.2/tests/test_halos/test_general_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_lenscosmo.py` & `pyhalo-0.2.2/tests/test_halos/test_lenscosmo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_nfw_halo.py` & `pyhalo-0.2.2/tests/test_halos/test_nfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_pjaffe.py` & `pyhalo-0.2.2/tests/test_halos/test_pjaffe.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_point_mass.py` & `pyhalo-0.2.2/tests/test_halos/test_point_mass.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_powerlaw_profile.py` & `pyhalo-0.2.2/tests/test_halos/test_powerlaw_profile.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_tnfw_halo.py` & `pyhalo-0.2.2/tests/test_halos/test_tnfw_halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_truncation.py` & `pyhalo-0.2.2/tests/test_halos/test_truncation.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_uldm.py` & `pyhalo-0.2.2/tests/test_halos/test_uldm.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_halos/test_util.py` & `pyhalo-0.2.2/tests/test_halos/test_util.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_mass_function_models.py` & `pyhalo-0.2.2/tests/test_mass_function_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_preset_models.py` & `pyhalo-0.2.2/tests/test_preset_models.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_pyhalo_base.py` & `pyhalo-0.2.2/tests/test_pyhalo_base.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_realization_extensions.py` & `pyhalo-0.2.2/tests/test_realization_extensions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_2halo.py` & `pyhalo-0.2.2/tests/test_rendering/test_2halo.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_los.py` & `pyhalo-0.2.2/tests/test_rendering/test_los.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_base_functions.py` & `pyhalo-0.2.2/tests/test_rendering/test_mass_functions/test_base_functions.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_delta_function.py` & `pyhalo-0.2.2/tests/test_rendering/test_mass_functions/test_delta_function.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_mass_functions/test_sheth_tormen.py` & `pyhalo-0.2.2/tests/test_rendering/test_mass_functions/test_sheth_tormen.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_population.py` & `pyhalo-0.2.2/tests/test_rendering/test_population.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_correlated.py` & `pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/test_correlated.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_nfw.py` & `pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/test_nfw.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_spatial_distribution/test_uniform.py` & `pyhalo-0.2.2/tests/test_rendering/test_spatial_distribution/test_uniform.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_rendering/test_subhalos.py` & `pyhalo-0.2.2/tests/test_rendering/test_subhalos.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_single_realization.py` & `pyhalo-0.2.2/tests/test_single_realization.py`

 * *Files identical despite different names*

### Comparing `pyhalo-0.2.1/tests/test_utilities.py` & `pyhalo-0.2.2/tests/test_utilities.py`

 * *Files identical despite different names*

