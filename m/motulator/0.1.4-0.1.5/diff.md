# Comparing `tmp/motulator-0.1.4.tar.gz` & `tmp/motulator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motulator-0.1.4.tar", last modified: Fri Apr  7 10:01:04 2023, max compression
+gzip compressed data, was "motulator-0.1.5.tar", last modified: Sun May 28 14:12:23 2023, max compression
```

## Comparing `motulator-0.1.4.tar` & `motulator-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:01:04.301172 motulator-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-07 10:00:43.000000 motulator-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-07 10:01:04.301172 motulator-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-07 10:00:43.000000 motulator-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:01:04.297172 motulator-0.1.4/motulator/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:01:04.301172 motulator-0.1.4/motulator/control/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/im_obs_vhz.py
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/im_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/im_vhz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/sm_flux_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9447 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/sm_obs_vhz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/sm_signal_inj.py
--rw-r--r--   0 runner    (1001) docker     (123)    19488 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/sm_torque.py
--rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/control/sm_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:01:04.301172 motulator-0.1.4/motulator/model/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/im.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/im_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/mech.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/sm_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/model/sm_flux_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-07 10:00:43.000000 motulator-0.1.4/motulator/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 10:01:04.297172 motulator-0.1.4/motulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-07 10:01:04.000000 motulator-0.1.4/motulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-07 10:01:04.000000 motulator-0.1.4/motulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 10:01:04.000000 motulator-0.1.4/motulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 10:01:04.000000 motulator-0.1.4/motulator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-07 10:00:43.000000 motulator-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-07 10:01:04.301172 motulator-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.505939 motulator-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-28 14:12:07.000000 motulator-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-28 14:12:23.505939 motulator-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-05-28 14:12:07.000000 motulator-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.497939 motulator-0.1.5/motulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.497939 motulator-0.1.5/motulator/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/control/im/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/_obs_vhz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15593 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/im/_vhz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/control/sm/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_flux_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_obs_vhz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_signal_inj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19597 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16077 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/control/sm/_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.501939 motulator-0.1.5/motulator/model/im/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/im/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/im/_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.505939 motulator-0.1.5/motulator/model/sm/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/sm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/sm/_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-28 14:12:07.000000 motulator-0.1.5/motulator/model/sm/_flux_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:12:23.497939 motulator-0.1.5/motulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 14:12:23.000000 motulator-0.1.5/motulator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-28 14:12:07.000000 motulator-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-28 14:12:23.505939 motulator-0.1.5/setup.cfg
```

### Comparing `motulator-0.1.4/LICENSE` & `motulator-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `motulator-0.1.4/PKG-INFO` & `motulator-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motulator
-Version: 0.1.4
+Version: 0.1.5
 Summary: Motor Drive Simulator in Python
 Home-page: https://github.com/Aalto-Electric-Drives/motulator
 Author: Marko Hinkkanen
 Author-email: marko.hinkkanen@aalto.fi
 Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,34 +34,15 @@
 ```
 Alternatively, the repository can be cloned:
 
 https://aalto-electric-drives.github.io/motulator/installation.html
 
 Usage
 -----
-The following example shows how to create a continuous-time system model, a discrete-time controller, and a simulation object:
-```python3
-import motulator as mt
-
-# Continuous-time model for the drive system
-motor = mt.InductionMotor()     # Motor model
-mech = mt.Mechanics()           # Mechanics model
-conv = mt.Inverter() 	        # Converter model
-mdl = mt.InductionMotorDrive(motor, mech, conv)
-
-# Discrete-time controller 
-pars = mt.InductionMotorVectorCtrlPars() 	# Dataclass of control parameters
-ctrl = mt.InductionMotorVectorCtrl(pars) 	# Sensorless controller
-
-# Create a simulation object, simulate, and plot example figures
-sim = mt.Simulation(mdl, ctrl)
-sim.simulate()
-mt.plot(sim)
-```
-This example applies the default settings. The drive system, controller, reference sequences etc. are easy to configure. The example scripts and Jupyter notebooks can be downloaded here:
+The drive system, controller, reference sequences etc. are easy to configure. As a starting point, example scripts and Jupyter notebooks can be downloaded here:
 
 https://aalto-electric-drives.github.io/motulator/auto_examples/index.html
 
 New system models and controllers can be developed using the existing ones as templates.
 
 Contributing
 ------------
@@ -86,14 +67,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/angelicaiaderosa"><img src="https://avatars.githubusercontent.com/u/112799415?v=4?s=50" width="50px;" alt="angelicaiaderosa"/><br /><sub><b>angelicaiaderosa</b></sub></a><br /><a href="https://github.com/Aalto-Electric-Drives/motulator/commits?author=angelicaiaderosa" title="Code">💻</a> <a href="#example-angelicaiaderosa" title="Examples">💡</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://www.kth.se/profile/lucap"><img src="https://avatars.githubusercontent.com/u/64190518?v=4?s=50" width="50px;" alt="Luca Peretti"/><br /><sub><b>Luca Peretti</b></sub></a><br /><a href="#ideas-lucaperetti" title="Ideas, Planning, & Feedback">🤔</a> <a href="#promotion-lucaperetti" title="Promotion">📣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/GianmarioPellegrinoPolito"><img src="https://avatars.githubusercontent.com/u/70333484?v=4?s=50" width="50px;" alt="GianmarioPellegrinoPolito"/><br /><sub><b>GianmarioPellegrinoPolito</b></sub></a><br /><a href="#data-GianmarioPellegrinoPolito" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/SimFerr"><img src="https://avatars.githubusercontent.com/u/67151973?v=4?s=50" width="50px;" alt="Simone Ferrari"/><br /><sub><b>Simone Ferrari</b></sub></a><br /><a href="#data-SimFerr" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jialed0303"><img src="https://avatars.githubusercontent.com/u/118135952?v=4?s=50" width="50px;" alt="Jialed0303"/><br /><sub><b>Jialed0303</b></sub></a><br /><a href="#ideas-Jialed0303" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/murgui"><img src="https://avatars.githubusercontent.com/u/29175623?v=4?s=50" width="50px;" alt="murgui"/><br /><sub><b>murgui</b></sub></a><br /><a href="https://github.com/Aalto-Electric-Drives/motulator/issues?q=author%3Amurgui" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: motulator Version: 0.1.4 Summary: Motor Drive
+Metadata-Version: 2.1 Name: motulator Version: 0.1.5 Summary: Motor Drive
 Simulator in Python Home-page: https://github.com/Aalto-Electric-Drives/
 motulator Author: Marko Hinkkanen Author-email: marko.hinkkanen@aalto.fi
 Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # *motulator:* Motor Drive Simulator in Python [![Build Status](https:/
@@ -19,39 +19,30 @@
 motor models are simulated in the continuous-time domain while the control
 algorithms run in discrete time. The default solver is the explicit Runge-Kutta
 method of order 5(4) from scipy.integrate.solve_ivp. Simple control algorithms
 are provided as examples. The documentation is available here: https://aalto-
 electric-drives.github.io/motulator/ Installation ------------ This software
 can be installed using pip: ```bash pip install motulator ``` Alternatively,
 the repository can be cloned: https://aalto-electric-drives.github.io/
-motulator/installation.html Usage ----- The following example shows how to
-create a continuous-time system model, a discrete-time controller, and a
-simulation object: ```python3 import motulator as mt # Continuous-time model
-for the drive system motor = mt.InductionMotor() # Motor model mech =
-mt.Mechanics() # Mechanics model conv = mt.Inverter() # Converter model mdl =
-mt.InductionMotorDrive(motor, mech, conv) # Discrete-time controller pars =
-mt.InductionMotorVectorCtrlPars() # Dataclass of control parameters ctrl =
-mt.InductionMotorVectorCtrl(pars) # Sensorless controller # Create a simulation
-object, simulate, and plot example figures sim = mt.Simulation(mdl, ctrl)
-sim.simulate() mt.plot(sim) ``` This example applies the default settings. The
-drive system, controller, reference sequences etc. are easy to configure. The
-example scripts and Jupyter notebooks can be downloaded here: https://aalto-
-electric-drives.github.io/motulator/auto_examples/index.html New system models
-and controllers can be developed using the existing ones as templates.
-Contributing ------------ If you'd like to help us develop motulator, please
-have a look at these [guidelines](https://github.com/Aalto-Electric-Drives/
-motulator/blob/main/CONTRIBUTING.md) first. Contributors ------------ Thanks go
-to these wonderful people:
+motulator/installation.html Usage ----- The drive system, controller, reference
+sequences etc. are easy to configure. As a starting point, example scripts and
+Jupyter notebooks can be downloaded here: https://aalto-electric-
+drives.github.io/motulator/auto_examples/index.html New system models and
+controllers can be developed using the existing ones as templates. Contributing
+------------ If you'd like to help us develop motulator, please have a look at
+these [guidelines](https://github.com/Aalto-Electric-Drives/motulator/blob/
+main/CONTRIBUTING.md) first. Contributors ------------ Thanks go to these
+wonderful people:
                 [Lauri_Tiitinen]                          [HannuHar]              [Marko_Hinkkanen]         [silundbe]      [JoonaKukkonen]  [jarno-  [angelicaiaderosa]
                  Lauri_Tiitinen                            HannuHar                Marko_Hinkkanen           silundbe        JoonaKukkonen      k]     angelicaiaderosa
            ð» ð¤ ð¡ ð§â         ð» ð        ð» ð¤ ð�    ð» ð�    ð» ð�jarno-k      ð» ð¡
                                                                                                                                                ð¤
-                       [Luca_Peretti]             [GianmarioPellegrinoPolito]        [Simone_Ferrari]       [Jialed0303]
-                        Luca_Peretti               GianmarioPellegrinoPolito          Simone_Ferrari         Jialed0303
-                          ð¤ ð£                  ð£                      ð£             ð¤
+                       [Luca_Peretti]             [GianmarioPellegrinoPolito]        [Simone_Ferrari]       [Jialed0303]        [murgui]
+                        Luca_Peretti               GianmarioPellegrinoPolito          Simone_Ferrari         Jialed0303          murgui
+                          ð¤ ð£                  ð£                      ð£             ð¤          ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! Acknowledgement --------------- This project has been sponsored by ABB
 Oy and by the Academy of Finland *Centre of Excellence in High-Speed
 Electromechanical Energy Conversion Systems*. The example control methods
 included in this repository are based on published algorithms (available in
 textbooks and scientific articles). They do not present any proprietary control
```

### Comparing `motulator-0.1.4/README.md` & `motulator-0.1.5/motulator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: motulator
+Version: 0.1.5
+Summary: Motor Drive Simulator in Python
+Home-page: https://github.com/Aalto-Electric-Drives/motulator
+Author: Marko Hinkkanen
+Author-email: marko.hinkkanen@aalto.fi
+Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # *motulator:* Motor Drive Simulator in Python
 [![Build Status](https://github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-pages.yml/badge.svg)](https://github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-pages.yml)
 [![License](https://img.shields.io/github/license/mashape/apistatus)](https://github.com/Aalto-Electric-Drives/motulator/blob/main/LICENSE)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/motulator.svg)](https://pypi.org/project/motulator/)
 [![All Contributors](https://img.shields.io/badge/all_contributors-6-orange.svg?style=flat-square)](#contributors-)
 
 Introduction
@@ -19,34 +34,15 @@
 ```
 Alternatively, the repository can be cloned:
 
 https://aalto-electric-drives.github.io/motulator/installation.html
 
 Usage
 -----
-The following example shows how to create a continuous-time system model, a discrete-time controller, and a simulation object:
-```python3
-import motulator as mt
-
-# Continuous-time model for the drive system
-motor = mt.InductionMotor()     # Motor model
-mech = mt.Mechanics()           # Mechanics model
-conv = mt.Inverter() 	        # Converter model
-mdl = mt.InductionMotorDrive(motor, mech, conv)
-
-# Discrete-time controller 
-pars = mt.InductionMotorVectorCtrlPars() 	# Dataclass of control parameters
-ctrl = mt.InductionMotorVectorCtrl(pars) 	# Sensorless controller
-
-# Create a simulation object, simulate, and plot example figures
-sim = mt.Simulation(mdl, ctrl)
-sim.simulate()
-mt.plot(sim)
-```
-This example applies the default settings. The drive system, controller, reference sequences etc. are easy to configure. The example scripts and Jupyter notebooks can be downloaded here:
+The drive system, controller, reference sequences etc. are easy to configure. As a starting point, example scripts and Jupyter notebooks can be downloaded here:
 
 https://aalto-electric-drives.github.io/motulator/auto_examples/index.html
 
 New system models and controllers can be developed using the existing ones as templates.
 
 Contributing
 ------------
@@ -71,14 +67,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/angelicaiaderosa"><img src="https://avatars.githubusercontent.com/u/112799415?v=4?s=50" width="50px;" alt="angelicaiaderosa"/><br /><sub><b>angelicaiaderosa</b></sub></a><br /><a href="https://github.com/Aalto-Electric-Drives/motulator/commits?author=angelicaiaderosa" title="Code">💻</a> <a href="#example-angelicaiaderosa" title="Examples">💡</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://www.kth.se/profile/lucap"><img src="https://avatars.githubusercontent.com/u/64190518?v=4?s=50" width="50px;" alt="Luca Peretti"/><br /><sub><b>Luca Peretti</b></sub></a><br /><a href="#ideas-lucaperetti" title="Ideas, Planning, & Feedback">🤔</a> <a href="#promotion-lucaperetti" title="Promotion">📣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/GianmarioPellegrinoPolito"><img src="https://avatars.githubusercontent.com/u/70333484?v=4?s=50" width="50px;" alt="GianmarioPellegrinoPolito"/><br /><sub><b>GianmarioPellegrinoPolito</b></sub></a><br /><a href="#data-GianmarioPellegrinoPolito" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/SimFerr"><img src="https://avatars.githubusercontent.com/u/67151973?v=4?s=50" width="50px;" alt="Simone Ferrari"/><br /><sub><b>Simone Ferrari</b></sub></a><br /><a href="#data-SimFerr" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jialed0303"><img src="https://avatars.githubusercontent.com/u/118135952?v=4?s=50" width="50px;" alt="Jialed0303"/><br /><sub><b>Jialed0303</b></sub></a><br /><a href="#ideas-Jialed0303" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/murgui"><img src="https://avatars.githubusercontent.com/u/29175623?v=4?s=50" width="50px;" alt="murgui"/><br /><sub><b>murgui</b></sub></a><br /><a href="https://github.com/Aalto-Electric-Drives/motulator/issues?q=author%3Amurgui" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,9 +1,16 @@
-# *motulator:* Motor Drive Simulator in Python [![Build Status](https://
-github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-
+Metadata-Version: 2.1 Name: motulator Version: 0.1.5 Summary: Motor Drive
+Simulator in Python Home-page: https://github.com/Aalto-Electric-Drives/
+motulator Author: Marko Hinkkanen Author-email: marko.hinkkanen@aalto.fi
+Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # *motulator:* Motor Drive Simulator in Python [![Build Status](https:/
+/github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-
 pages.yml/badge.svg)](https://github.com/Aalto-Electric-Drives/motulator/
 actions/workflows/update_gh-pages.yml) [![License](https://img.shields.io/
 github/license/mashape/apistatus)](https://github.com/Aalto-Electric-Drives/
 motulator/blob/main/LICENSE) [![PyPI version shields.io](https://
 img.shields.io/pypi/v/motulator.svg)](https://pypi.org/project/motulator/) [!
 [All Contributors](https://img.shields.io/badge/all_contributors-6-
 orange.svg?style=flat-square)](#contributors-) Introduction ------------ This
@@ -12,39 +19,30 @@
 motor models are simulated in the continuous-time domain while the control
 algorithms run in discrete time. The default solver is the explicit Runge-Kutta
 method of order 5(4) from scipy.integrate.solve_ivp. Simple control algorithms
 are provided as examples. The documentation is available here: https://aalto-
 electric-drives.github.io/motulator/ Installation ------------ This software
 can be installed using pip: ```bash pip install motulator ``` Alternatively,
 the repository can be cloned: https://aalto-electric-drives.github.io/
-motulator/installation.html Usage ----- The following example shows how to
-create a continuous-time system model, a discrete-time controller, and a
-simulation object: ```python3 import motulator as mt # Continuous-time model
-for the drive system motor = mt.InductionMotor() # Motor model mech =
-mt.Mechanics() # Mechanics model conv = mt.Inverter() # Converter model mdl =
-mt.InductionMotorDrive(motor, mech, conv) # Discrete-time controller pars =
-mt.InductionMotorVectorCtrlPars() # Dataclass of control parameters ctrl =
-mt.InductionMotorVectorCtrl(pars) # Sensorless controller # Create a simulation
-object, simulate, and plot example figures sim = mt.Simulation(mdl, ctrl)
-sim.simulate() mt.plot(sim) ``` This example applies the default settings. The
-drive system, controller, reference sequences etc. are easy to configure. The
-example scripts and Jupyter notebooks can be downloaded here: https://aalto-
-electric-drives.github.io/motulator/auto_examples/index.html New system models
-and controllers can be developed using the existing ones as templates.
-Contributing ------------ If you'd like to help us develop motulator, please
-have a look at these [guidelines](https://github.com/Aalto-Electric-Drives/
-motulator/blob/main/CONTRIBUTING.md) first. Contributors ------------ Thanks go
-to these wonderful people:
+motulator/installation.html Usage ----- The drive system, controller, reference
+sequences etc. are easy to configure. As a starting point, example scripts and
+Jupyter notebooks can be downloaded here: https://aalto-electric-
+drives.github.io/motulator/auto_examples/index.html New system models and
+controllers can be developed using the existing ones as templates. Contributing
+------------ If you'd like to help us develop motulator, please have a look at
+these [guidelines](https://github.com/Aalto-Electric-Drives/motulator/blob/
+main/CONTRIBUTING.md) first. Contributors ------------ Thanks go to these
+wonderful people:
                 [Lauri_Tiitinen]                          [HannuHar]              [Marko_Hinkkanen]         [silundbe]      [JoonaKukkonen]  [jarno-  [angelicaiaderosa]
                  Lauri_Tiitinen                            HannuHar                Marko_Hinkkanen           silundbe        JoonaKukkonen      k]     angelicaiaderosa
            ð» ð¤ ð¡ ð§â         ð» ð        ð» ð¤ ð�    ð» ð�    ð» ð�jarno-k      ð» ð¡
                                                                                                                                                ð¤
-                       [Luca_Peretti]             [GianmarioPellegrinoPolito]        [Simone_Ferrari]       [Jialed0303]
-                        Luca_Peretti               GianmarioPellegrinoPolito          Simone_Ferrari         Jialed0303
-                          ð¤ ð£                  ð£                      ð£             ð¤
+                       [Luca_Peretti]             [GianmarioPellegrinoPolito]        [Simone_Ferrari]       [Jialed0303]        [murgui]
+                        Luca_Peretti               GianmarioPellegrinoPolito          Simone_Ferrari         Jialed0303          murgui
+                          ð¤ ð£                  ð£                      ð£             ð¤          ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! Acknowledgement --------------- This project has been sponsored by ABB
 Oy and by the Academy of Finland *Centre of Excellence in High-Speed
 Electromechanical Energy Conversion Systems*. The example control methods
 included in this repository are based on published algorithms (available in
 textbooks and scientific articles). They do not present any proprietary control
```

### Comparing `motulator-0.1.4/motulator/control/common.py` & `motulator-0.1.5/motulator/control/im/_obs_vhz.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,378 +1,295 @@
-"""Common control functions and classes."""
+"""
+Observer-based V/Hz control for induction machine drives.
 
-import numpy as np
-
-from motulator.helpers import abc2complex, complex2abc, Bunch
+This implements the observer-based V/Hz control method described in [#Tii2022]_. 
+The state-feedback control law is in the alternative form which uses an
+intermediate stator current reference.
+
+References
+----------
+.. [#Tii2022] Tiitinen, Hinkkanen, Harnefors, "Stable and passive observer-based 
+   V/Hz control for induction motors," Proc. IEEE ECCE, Detroit, MI, Oct. 2022,
+   https://doi.org/10.1109/ECCE50734.2022.9948057
 
+"""
 
 # %%
-class PWM:
-    """
-    Duty ratio references and realized voltage for three-phase PWM.
-
-    This contains the computation of the duty ratio references and the realized
-    voltage. The digital delay effects are taken into account in the realized
-    voltage.
-
-    Parameters
-    ----------
-    pars : data object
-        Control parameters.
-
-    """
-
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        try:
-            self.six_step = pars.six_step
-        except AttributeError:
-            self.six_step = False
-        self.realized_voltage = 0
-        self._u_ref_lim_old = 0
-
-    @staticmethod
-    def six_step_overmodulation(u_s_ref, u_dc):
-        """
-        Overmodulation up to six-step operation.
-
-        This method modifies the angle of the voltage reference vector in the
-        overmodulation region such that the six-step operation is reached [1]_.
-
-        Parameters
-        ----------
-        u_s_ref : complex
-            Voltage reference in stator coordinates.
-
-        Returns
-        -------
-        u_s_ref_mod : complex
-            Voltage reference in stator coordinates.
-
-        References
-        ----------
-        .. [1] Bolognani, Zigliotto, "Novel digital continuous control of SVM
-           inverters in the overmodulation range," IEEE Trans. Ind. Appl.,
-           1997, https://doi.org/10.1109/28.568019
-
-        """
-        # Limited magnitude
-        r = np.min([np.abs(u_s_ref), 2/3*u_dc])
-
-        if np.sqrt(3)*r > u_dc:
-            # Angle and sector of the reference vector
-            theta = np.angle(u_s_ref)
-            sector = np.floor(3*theta/np.pi)
-
-            # Angle reduced to the first sector (at which sector == 0)
-            theta0 = theta - sector*np.pi/3
-
-            # Intersection angle, see Eq. (9)
-            alpha_g = np.pi/6 - np.arccos(u_dc/(np.sqrt(3)*r))
-
-            # Modify the angle according to Eq. (4)
-            if alpha_g <= theta0 <= np.pi/6:
-                theta0 = alpha_g
-            elif np.pi/6 <= theta0 <= np.pi/3 - alpha_g:
-                theta0 = np.pi/3 - alpha_g
-
-            # Modified reference voltage
-            u_s_ref_mod = r*np.exp(1j*(theta0 + sector*np.pi/3))
-        else:
-            u_s_ref_mod = u_s_ref
-
-        return u_s_ref_mod
-
-    @staticmethod
-    def duty_ratios(u_s_ref, u_dc):
-        """
-        Compute the duty ratios for three-phase PWM.
-
-        This computes the duty ratios using a symmetrical suboscillation
-        method. This method is identical to the standard space-vector PWM.
-
-        Parameters
-        ----------
-        u_s_ref : complex
-            Voltage reference in stator coordinates.
-        u_dc : float
-            DC-bus voltage.
-
-        Returns
-        -------
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
-
-        """
-        # Phase voltages without the zero-sequence voltage
-        u_abc = complex2abc(u_s_ref)
-
-        # Symmetrization by adding the zero-sequence voltage
-        u_0 = .5*(np.amax(u_abc) + np.amin(u_abc))
-        u_abc -= u_0
-
-        # Preventing overmodulation by means of a minimum phase error method
-        m = (2./u_dc)*np.amax(u_abc)
-        if m > 1:
-            u_abc = u_abc/m
-
-        # Duty ratios
-        d_abc_ref = .5 + u_abc/u_dc
-
-        return d_abc_ref
-
-    def __call__(self, u_ref, u_dc, theta, w):
-        """
-        Compute the duty ratios and update the state.
-
-        Parameters
-        ----------
-        u_ref : complex
-            Voltage reference in synchronous coordinates.
-        u_dc : float
-            DC-bus voltage.
-        theta : float
-            Angle of synchronous coordinates.
-        w : float
-            Angular frequency of synchronous coordinates.
-
-        Returns
-        -------
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
-
-        """
-        d_abc_ref, u_ref_lim = self.output(u_ref, u_dc, theta, w)
-        self.update(u_ref_lim)
-
-        return d_abc_ref
-
-    def output(self, u_ref, u_dc, theta, w):
-        """Compute the duty ratio limited voltage reference."""
-        # Advance the angle due to the computational delay (T_s) and
-        # the ZOH (PWM) delay (0.5*T_s)
-        theta_comp = theta + 1.5*self.T_s*w
-
-        # Voltage reference in stator coordinates
-        u_s_ref = np.exp(1j*theta_comp)*u_ref
-
-        # Modify angle in the overmodulation region
-        if self.six_step:
-            u_s_ref = self.six_step_overmodulation(u_s_ref, u_dc)
-
-        # Duty ratios
-        d_abc_ref = self.duty_ratios(u_s_ref, u_dc)
-
-        # Realizable voltage
-        u_s_ref_lim = abc2complex(d_abc_ref)*u_dc
-        u_ref_lim = np.exp(-1j*theta_comp)*u_s_ref_lim
-
-        return d_abc_ref, u_ref_lim
-
-    def update(self, u_ref_lim):
-        """
-        Update the voltage estimate for the next sampling instant.
-
-        Parameters
-        ----------
-        u_ref_lim : complex
-            Limited voltage reference in synchronous coordinates.
-
-        """
-        self.realized_voltage = .5*(self._u_ref_lim_old + u_ref_lim)
-        self._u_ref_lim_old = u_ref_lim
+from dataclasses import dataclass
+import numpy as np
+from motulator.control._common import Ctrl, PWM, RateLimiter
+from motulator._helpers import abc2complex
+from motulator._utils import Bunch
 
 
 # %%
-class SpeedCtrl:
+# pylint: disable=too-many-instance-attributes
+@dataclass
+class ObserverBasedVHzCtrlPars:
     """
-    2DOF PI speed controller.
-
-    This controller is implemented using the disturbance-observer structure.
-    The controller is mathematically identical to the 2DOF PI speed controller.
+    Parameters for the control system.
 
     Parameters
     ----------
-    pars : data object
-        Control parameters.
+    psi_s_nom : float
+        Nominal stator flux linkage (Vs). 
+    i_s_max : float, optional
+        Maximum stator current (A). The default is inf.
+    k_tau : float, optional
+        Torque controller gain. The default is 3.
+    alpha_psi : float, optional
+        Stator flux control bandwidth (rad/s). The default is 2*pi*20.
+    alpha_f : float, optional
+        Torque high-pass filter bandwidth (rad/s). The default is 2*pi*1.
+    alpha_r : float, optional
+        Low-pass-filter bandwidth (rad/s) for slip angular frequency. The
+        default is 2*pi*1.
+    slip_compensation : bool, optional
+        Enable slip compensation. The default is False.
 
     """
-
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        try:
-            self.tau_M_max = pars.tau_M_max
-        except AttributeError:
-            # No maximum torque limit
-            self.tau_M_max = np.inf
-        try:
-            # Gains for the 2DOF PI controller
-            self.alpha = pars.alpha_s
-            self.k_t = pars.alpha_s*pars.J
-            self.k_p = 2*pars.alpha_s*pars.J
-        except AttributeError:
-            # alpha_s or J not defined, try to use k_t, k_p, k_i
-            try:
-                self.k_t = pars.k_t
-                self.k_p = pars.k_p
-                self.alpha = pars.k_i/pars.k_t
-            except AttributeError:
-                print('No speed controller gains found.')
-
-        # Integral state
-        self.tau_i = 0
-        # Load torque estimate (stored for the update method)
-        self.tau_L = 0
-
-    def output(self, w_M_ref, w_M):
-        """
-        Compute the torque reference and the load torque estimate.
-
-        Parameters
-        ----------
-        w_M_ref : float
-            Rotor speed reference (in mechanical rad/s).
-        w_M : float
-            Rotor speed (in mechanical rad/s).
-
-        Returns
-        -------
-        tau_M_ref : float
-            Torque reference.
-
-        """
-        self.tau_L = self.tau_i - (self.k_p - self.k_t)*w_M
-        tau_M_ref = self.k_t*(w_M_ref - w_M) + self.tau_L
-
-        if np.abs(tau_M_ref) > self.tau_M_max:
-            tau_M_ref = np.sign(tau_M_ref)*self.tau_M_max
-
-        return tau_M_ref
-
-    def update(self, tau_M_ref_lim):
-        """
-        Update the integral state.
-
-        Parameters
-        ----------
-        tau_M_ref_lim : float
-            Realized (limited) torque reference.
-
-        """
-        self.tau_i += self.T_s*self.alpha*(tau_M_ref_lim - self.tau_L)
+    # par: InitVar[ModelPars | None] = None
+    psi_s_nom: float = None
+    i_s_max: float = np.inf
+    k_tau: float = 3.
+    alpha_psi: float = 2*np.pi*20
+    alpha_f: float = 2*np.pi*1
+    alpha_r: float = 2*np.pi*1
+    slip_compensation: bool = False
 
 
 # %%
-class RateLimiter:
+class ObserverBasedVHzCtrl(Ctrl):
     """
-    Rate limiter.
+    Observer-based V/Hz control for induction machines.
 
     Parameters
     ----------
-    pars : data object
-        Control parameters.
+    par : ModelPars
+        Machine model parameters.
+    ctrl_par : ObserverBasedVHzCtrlPars
+        Control system parameters.
+    T_s : float, optional
+        Sampling period (s). The default is 250e-6.
+
+    Attributes
+    ----------
+    observer : SensorlessObserverExtCoord
+        Sensorless reduced-order flux observer in external coordinates.
+    rate_limiter : RateLimiter
+        Rate limiter for the speed reference.
+    pwm : PWM
+        Pulse-width modulation.
+    w_m_ref : callable
+        Speed reference (electrical rad/s) as a function of time (s).
 
     """
 
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.limit = pars.rate_limit
-        self.y_old = 0
+    # pylint: disable=too-many-instance-attributes, too-many-arguments
+    def __init__(self, par, ctrl_par, T_s=250e-6):
+        super().__init__()
+        self.T_s = T_s
+        # Model parameters
+        self.R_s, self.R_R = par.R_s, par.R_R
+        self.L_sgm = par.L_sgm
+        self.n_p = par.n_p
+        # References
+        self.w_m_ref = callable
+        self.psi_s_ref = ctrl_par.psi_s_nom
+        self.i_s_max = ctrl_par.i_s_max
+        # Control parameters
+        self.slip_compensation = ctrl_par.slip_compensation
+        self.alpha_f = ctrl_par.alpha_f
+        self.alpha_r = ctrl_par.alpha_r
+        self.alpha_psi = ctrl_par.alpha_psi
+        self.k_tau = ctrl_par.k_tau
+        # Instantiate classes
+        self.observer = FluxObserver(par, alpha_o=2*np.pi*40)
+        self.rate_limiter = RateLimiter()
+        self.pwm = PWM(six_step=False)
+        # States
+        self.theta_s, self.tau_M_ref, self.w_r_ref = 0, 0, 0
 
-    def __call__(self, u):
+    def __call__(self, mdl):
         """
-        Limit the input signal.
+        Run the main control loop.
 
         Parameters
         ----------
-        u : float
-            Input signal.
+        mdl : Drive
+            Continuous-time system model for getting the feedback signals.
 
         Returns
         -------
-        y : float
-            Rate-limited output signal.
-
-        Notes
-        -----
-        In this implementation, the falling rate limit equals the (negative)
-        rising rate limit. If needed, these limits can be separated with minor
-        modifications in the class.
-
-        """
-        rate = (u - self.y_old)/self.T_s
-
-        if rate > self.limit:
-            # Limit rising rate
-            y = self.y_old + self.T_s*self.limit
-        elif rate < -self.limit:
-            # Limit falling rate
-            y = self.y_old - self.T_s*self.limit
+        T_s : float
+            Sampling period (s).
+        d_abc : ndarray, shape (3,)
+            Duty ratios.
+
+        """
+        # Get the speed reference
+        w_m_ref = self.rate_limiter(self.T_s, self.w_m_ref(self.clock.t))
+
+        # Measure the feedback signals
+        i_s_abc = mdl.machine.meas_currents()  # Phase currents
+        u_dc = mdl.converter.meas_dc_voltage()  # DC-bus voltage
+
+        # Get the states
+        u_s = self.pwm.realized_voltage
+        psi_R = self.observer.psi_R
+        tau_M_ref = self.tau_M_ref
+        w_r_ref = self.w_r_ref
+        theta_s = self.theta_s
+
+        # Space vector and coordinate transformation
+        i_s = np.exp(-1j*theta_s)*abc2complex(i_s_abc)
+
+        # Torque estimate
+        tau_M = 1.5*self.n_p*np.imag(i_s*np.conj(psi_R))
+
+        # Slip frequency compensation (if enabled) for the low-pass filter.
+        # Note, could also be based on the low-pass filtered torque.
+        psi_R_sqr = np.abs(psi_R)**2
+        if self.slip_compensation and psi_R_sqr > 0:
+            w_r = self.R_R*tau_M/(1.5*self.n_p*psi_R_sqr)
         else:
-            y = u
+            w_r = 0
 
-        # Store the limited output
-        self.y_old = y
-
-        return y
+        # Slip compensation. Uses the low-pass filtered slip estimate w_r_ref.
+        # Note if slip compensation disabled w_r_ref == 0.
+        w_s_ref = w_m_ref + w_r_ref
+
+        # Dynamic frequency
+        w_s = w_s_ref - self.k_tau*(tau_M - tau_M_ref)
+
+        # State feedback
+        u_s_ref = self._state_feedback(i_s, psi_R, w_s)
+
+        # Data logging
+        data = Bunch(
+            i_s=i_s,
+            psi_s=psi_R + self.L_sgm*i_s,
+            psi_s_ref=self.psi_s_ref,
+            t=self.clock.t,
+            theta_s=self.theta_s,
+            u_dc=u_dc,
+            u_s=u_s,
+            w_m=self.observer.w_m,
+            w_m_ref=w_m_ref,
+            w_s=w_s,
+            tau_M=tau_M,
+        )
+        self.save(data)
+
+        # Update the states
+        self.observer.update(self.T_s, u_s, i_s, w_s)
+        self.w_r_ref += self.T_s*self.alpha_r*(w_r - self.w_r_ref)
+        self.tau_M_ref += self.T_s*self.alpha_f*(tau_M - self.tau_M_ref)
+        self.theta_s += self.T_s*w_s  # Next line: limit into [-pi, pi)
+        self.theta_s = np.mod(self.theta_s + np.pi, 2*np.pi) - np.pi
+        self.clock.update(self.T_s)
+
+        # Calculate the duty ratios and update the voltage estimate state
+        d_abc = self.pwm(self.T_s, u_s_ref, u_dc, theta_s, w_s)
+
+        return self.T_s, d_abc
+
+    def _state_feedback(self, i_s, psi_R, w_s):
+        # Internal current reference for state feedback
+        i_s_ref = (self.psi_s_ref - psi_R)/self.L_sgm
+        # Limit the reference
+        if np.abs(i_s_ref) > self.i_s_max:
+            i_s_ref = self.i_s_max*i_s_ref/np.abs(i_s_ref)
+        # State feedback
+        u_s_ref = (
+            self.R_s*i_s_ref + 1j*w_s*self.psi_s_ref +
+            self.L_sgm*self.alpha_psi*(i_s_ref - i_s))
+        return u_s_ref
 
 
 # %%
-class Ctrl:
-    """Base class for main control loops."""
+class FluxObserver:
+    """
+    Sensorless reduced-order flux observer in external coordinates.
 
-    def __init__(self):
-        self.t = 0  # Digital clock
-        self.data = Bunch()  # Data store
-        self.t_reset = 1e9  # Time at which the clock is reset
+    This is a sensorless reduced-order flux observer in synchronous coordinates
+    for an induction machine. The observer gain decouples the electrical and
+    mechanical dynamics and allows placing the poles of the linearized 
+    estimation error dynamics. This implementation operates in external 
+    coordinates (typically synchronous coordinates defined by reference signals 
+    of a control system).
 
-    def __call__(self, mdl):
-        """
-        Run the main control loop.
+    Parameters
+    ----------
+    par : ModelPars
+        Machine model parameters.
+    alpha_o : float
+        Speed-estimation bandwidth (rad/s).
+    b : callable, optional 
+        Coefficient (rad/s) of the characteristic polynomial as a function of 
+        the rotor angular speed estimate. The default is 
+        ``lambda w_m: R_R/L_M + .4*abs(w_m)``.
 
-        The main control loop is callable that returns the sampling
-        period `T_s` (float)  and the duty ratio references `d_abc_ref`
-        (ndarray, shape (3,)) for the next sampling period.
+    Attributes
+    ----------
+    psi_R : complex
+        Rotor flux estimate (Vs).
+    w_m : float
+        Rotor angular speed estimate (electrical rad/s).
+
+    Notes
+    -----
+    The characteristic polynomial of the observer in synchronous coordinates is 
+    ``s**2 + b*s + w_s**2``.  
 
-        Parameters
-        ----------
-        mdl : Model
-            System model containing methods for getting the feedback signals.
+    """
 
-        """
-        raise NotImplementedError
+    # pylint: disable=too-many-instance-attributes
+    def __init__(self, par, alpha_o, b=None):
+        self.R_s, self.R_R, self.L_sgm = par.R_s, par.R_R, par.L_sgm
+        self.alpha = par.R_R/par.L_M
+        # Design parameters
+        self.alpha_o = alpha_o
+        zeta_inf = .2  # Damping ratio at high speeds
+        self.b = lambda w_m: (
+            self.alpha + 2*zeta_inf*np.abs(w_m) if b is None else b)
+        # States
+        self.psi_R, self.w_m = 0, 0
+        # Previous current, private attribute
+        self._i_s_old = 0
 
-    def update_clock(self, T_s):
+    def update(self, T_s, u_s, i_s, w_s):
         """
-        Update the digital clock.
+        Update the states.
 
         Parameters
         ----------
         T_s : float
-            Sampling period.
-
-        """
-        self.t += T_s if self.t < self.t_reset else 0
-
-    def save(self, data):
-        """
-        Save the internal controller data.
-
-        Parameters
-        ----------
-        data : bunch or dict
-            Contains the data to be saved.
-
-        """
-        for key, value in data.items():
-            self.data.setdefault(key, []).extend([value])
-
-    def post_process(self):
-        """
-        Transform the lists to the ndarray format.
-
-        This can be run after the simulation has been completed in order to
-        simplify plotting and analysis of the stored data.
-
-        """
-        for key in self.data:
-            self.data[key] = np.asarray(self.data[key])
+            Sampling period (s).
+        u_s : complex
+            Stator voltage (V) in synchronous coordinates.
+        i_s : complex
+            Stator current (A) in synchronous coordinates.
+        w_s : float
+            Angular frequency (rad/s) of the coordinate system. 
+
+        """
+        # Observer gain with c = w_s**2 (without the orthogonal projection
+        # which is embedded into the error signal and the state update)
+        g = self.b(self.w_m)/(self.alpha - 1j*self.w_m)
+
+        # Time derivative of the stator current
+        di_s = (i_s - self._i_s_old)/T_s
+
+        # Induced voltage from the rotor quantities
+        e_r = self.R_R*i_s - (self.alpha - 1j*self.w_m)*self.psi_R
+
+        # Induced voltage from stator quantities
+        e_s = u_s - self.R_s*i_s - self.L_sgm*(di_s + 1j*w_s*i_s)
+
+        # Error signal (rad/s)
+        err = (e_s - e_r)/self.psi_R if np.abs(self.psi_R) > 0 else 0
+
+        # Update the states
+        self.psi_R += T_s*(e_s - (1j*w_s + g*err.real)*self.psi_R)
+        self.w_m += T_s*self.alpha_o*err.imag
+        self._i_s_old = i_s
```

### Comparing `motulator-0.1.4/motulator/control/im_obs_vhz.py` & `motulator-0.1.5/motulator/control/sm/_signal_inj.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,269 +1,265 @@
-"""
-Observer-based V/Hz control for induction motor drives.
+"""Sensorless control with signal injection for synchronous machine drives."""
 
-This implements the observer-based V/Hz control method described in [1]_. The
-state-feedback control law is in the alternative form which uses an
-intermediate stator current reference.
-
-References
-----------
-.. [1] Tiitinen, Hinkkanen, Harnefors, "Stable and passive observer-based V/Hz
-    control for induction motors," Proc. IEEE ECCE, Detroit, MI, Oct. 2022.
-
-"""
-
-# %%
-from typing import Callable
-from dataclasses import dataclass, field
 import numpy as np
-from motulator.control.common import Ctrl, PWM, RateLimiter
-from motulator.helpers import abc2complex, Bunch
+from motulator._helpers import abc2complex
+from motulator.control._common import Ctrl, PWM, SpeedCtrl
+from motulator.control.sm._vector import CurrentCtrl, CurrentReference
+from motulator._utils import Bunch
 
 
 # %%
-@dataclass
-class InductionMotorObsVHzCtrlPars:
-    """Control parameters."""
-
-    # pylint: disable=too-many-instance-attributes
-    # Speed reference (in electrical rad/s)
-    w_m_ref: Callable[[float], float] = field(
-        repr=False, default=lambda t: (t > .2)*(2*np.pi*50))
-
-    # Control
-    T_s: float = 250e-6
-    psi_s_nom: float = 1.04  # 1 p.u.
-    rate_limit: float = 2*np.pi*120
-    i_s_max: float = 1.5*np.sqrt(2)*5
-    alpha_f: float = 2*np.pi*1
-    alpha_psi: float = 2*np.pi*20
-    k_tau: float = 3.
-    six_step: bool = False
-
-    # Slip compensation
-    slip_compensation: bool = True
-    alpha_r: float = 2*np.pi*1
-
-    # Observer
-    alpha_o: float = 2*np.pi*40
-    zeta_inf: float = .7
-
-    # Motor parameter estimates (inverse-Γ model)
-    R_s: float = 3.7
-    R_R: float = 2.1
-    L_sgm: float = .021
-    L_M: float = .224
-    n_p: int = 2
+class SignalInjectionCtrl(Ctrl):
+    """
+    Sensorless control with signal injection for synchronous machine drives.
 
+    This class implements a square-wave signal injection for low-speed 
+    operation according to [#Kim2012]_. A phase-locked loop is used to track 
+    the rotor position. 
+    
+    Notes
+    -----
+    For a wider speed range, signal injection could be combined to a 
+    model-based observer. The effects of magnetic saturation are not
+    compensated for in this version.
 
-# %%
-class InductionMotorVHzObsCtrl(Ctrl):
-    """
-    Observer-based V/Hz control for induction motors.
+    References
+    ----------
+    .. [#Kim2012] Kim, Ha, Sul, "PWM switching frequency signal injection 
+       sensorless method in IPMSM," IEEE Trans. Ind. Appl., 2012,
+       https://doi.org/10.1109/TIA.2012.2210175
 
     Parameters
     ----------
-    pars : InductionMotorObsVHzCtrlPars
-        Control parameters.
+    T_s : float
+        Sampling period (s).
+    pars : ModelPars
+        Machine model parameters.
+    U_inj : float
+        Amplitude of the injected voltage (V).
+    w_o : float
+        PLL natural frequency (rad/s).
+
+    Attributes
+    ----------
+    current_ctrl : CurrentCtrl
+        Current controller.
+    speed_ctrl : SpeedCtrl
+        Speed controller.
+    current_ref : CurrentReference
+        Current reference generator.
+    pll : PhaseLockedLoop
+        Phase-locked loop.
+    signal_inj : SignalInjection
+        Signal injection.
+    w_m_ref : callable
+        Speed reference (electrical rad/s).
+    pwm : PWM
+        Pulse-width modulation.
 
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
+    def __init__(self, par, ref, T_s=250e-6):
         super().__init__()
-        # Instantiate classes
-        self.observer = SensorlessFluxObserver(pars)
-        self.pwm = PWM(pars)
-        self.rate_limiter = RateLimiter(pars)
-        # Reference
-        self.w_m_ref = pars.w_m_ref
-        self.psi_s_ref = pars.psi_s_nom
-        # Control Parameters
-        self.T_s = pars.T_s
-        self.alpha_f = pars.alpha_f
-        self.alpha_r = pars.alpha_r
-        self.alpha_psi = pars.alpha_psi
-        self.n_p = pars.n_p
-        self.k_tau = pars.k_tau
-        self.i_s_max = pars.i_s_max
-        self.slip_compensation = pars.slip_compensation
-        # Motor parameters
-        self.R_s = pars.R_s
-        self.R_R = pars.R_R
-        self.L_sgm = pars.L_sgm
-        # Initial states
-        self.theta_s, self.tau_M_ref, self.w_r_ref = 0, 0, 0
+        self.T_s = T_s
+        self.n_p = par.n_p
+        self.current_ref = CurrentReference(par, ref)
+        self.current_ctrl = CurrentCtrl(par, 2*np.pi*200)
+        self.pll = PhaseLockedLoop(w_o=2*np.pi*40)
+        self.signal_inj = SignalInjection(par, U_inj=250)
+        self.speed_ctrl = SpeedCtrl(par.J, 2*np.pi*4)
+        self.pwm = PWM()
+        self.w_m_ref = callable
 
     def __call__(self, mdl):
         """
         Run the main control loop.
 
         Parameters
         ----------
-        mdl : InductionMotorDrive
-            Continuous-time model of an induction motor drive for getting the
-            feedback signals.
+        mdl : Drive
+            Continuous-time system model for getting the feedback signals.
 
         Returns
         -------
         T_s : float
-            Sampling period.
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
+            Sampling period (s).
+        d_abc : ndarray, shape (3,)
+            Duty ratios.
 
         """
         # Get the speed reference
-        w_m_ref = self.rate_limiter(self.w_m_ref(self.t))
+        w_m_ref = self.w_m_ref(self.clock.t)
 
         # Measure the feedback signals
-        i_s_abc = mdl.motor.meas_currents()  # Phase currents
-        u_dc = mdl.conv.meas_dc_voltage()  # DC-bus voltage
+        i_s_abc = mdl.machine.meas_currents()  # Phase currents
+        u_dc = mdl.converter.meas_dc_voltage()  # DC-bus voltage
+        u_s = self.pwm.realized_voltage
 
-        # Space vector and coordinate transformation
-        i_s = np.exp(-1j*self.theta_s)*abc2complex(i_s_abc)
+        # Get the rotor speed and position estimates
+        w_m, theta_m = self.pll.w_m, self.pll.theta_m
 
-        # Get the states
-        u_s = self.pwm.realized_voltage
-        psi_R = self.observer.psi_R
-        tau_M_ref = self.tau_M_ref
-        w_r_ref = self.w_r_ref
-
-        # Torque estimate (11c)
-        tau_M = 1.5*self.n_p*np.imag(i_s*np.conj(psi_R))
-
-        # Slip frequency compensation (if enabled) for the low-pass filter.
-        # Note, could also be based on the low-pass filtered torque.
-        psi_R_sqr = np.abs(psi_R)**2
-        if self.slip_compensation and psi_R_sqr > 0:
-            w_r = self.R_R*tau_M/(1.5*self.n_p*psi_R_sqr)
-        else:
-            w_r = 0
-
-        # Slip compensation (9). Uses the low-pass filtered slip estimate
-        # w_r_ref. Note if slip compensation disabled w_r_ref == 0.
-        w_s_ref = w_m_ref + w_r_ref
-
-        # Dynamic frequency (7a)
-        w_s = w_s_ref - self.k_tau*(tau_M - tau_M_ref)
-
-        # State feedback
-        u_s_ref = self.state_feedback(i_s, psi_R, w_s)
-
-        # Duty ratios
-        d_abc_ref, u_s_ref_lim = self.pwm.output(
-            u_s_ref, u_dc, self.theta_s, w_s)
+        # Current vector in estimated rotor coordinates
+        i_s = np.exp(-1j*theta_m)*abc2complex(i_s_abc)
+
+        # Filter the current measurement for the current controller
+        i_s_filt = self.signal_inj.filter_current(i_s)
+
+        # Outputs
+        tau_M_ref = self.speed_ctrl.output(w_m_ref/self.n_p, w_m/self.n_p)
+        i_s_ref, tau_M_ref_lim = self.current_ref.output(tau_M_ref, w_m, u_dc)
+        err = self.signal_inj.output(self.T_s, i_s.imag)
+        # Superimpose the excitation voltage on the d-axis
+        u_s_ref = self.current_ctrl.output(
+            i_s_ref, i_s_filt) + self.signal_inj.u_sd_inj
 
         # Data logging
         data = Bunch(
-            i_s=i_s,
-            psi_s=psi_R + self.L_sgm*i_s,
-            psi_s_ref=self.psi_s_ref,
-            t=self.t,
-            theta_s=self.theta_s,
+            i_s=i_s_filt,
+            i_s_ref=i_s_ref,
+            t=self.clock.t,
+            tau_M_ref_lim=tau_M_ref_lim,
+            theta_m=theta_m,
             u_dc=u_dc,
             u_s=u_s,
-            w_m=self.observer.w_m,
+            w_m=w_m,
             w_m_ref=w_m_ref,
-            w_s=w_s,
-            tau_M=tau_M,
         )
         self.save(data)
 
-        # Update the states
-        self.pwm.update(u_s_ref_lim)
-        self.observer.update(u_s, i_s, w_s)
-        self.tau_M_ref += self.T_s*self.alpha_f*(tau_M - self.tau_M_ref)
-        self.theta_s += self.T_s*w_s  # Next line: limit into [-pi, pi)
-        self.theta_s = np.mod(self.theta_s + np.pi, 2*np.pi) - np.pi
-        self.w_r_ref += self.T_s*self.alpha_r*(w_r - self.w_r_ref)
-        self.update_clock(self.T_s)
-
-        return self.T_s, d_abc_ref
-
-    def state_feedback(self, i_s, psi_R, w_s):
-        """Compute the stator voltage reference."""
-        # Internal current reference for state feedback (6b)
-        i_s_ref = (self.psi_s_ref - psi_R)/self.L_sgm
-        # Limit the reference
-        if np.abs(i_s_ref) > self.i_s_max:
-            i_s_ref = self.i_s_max*i_s_ref/np.abs(i_s_ref)
-        # State feedback (6a)
-        u_s_ref = (
-            self.R_s*i_s_ref + 1j*w_s*self.psi_s_ref +
-            self.L_sgm*self.alpha_psi*(i_s_ref - i_s))
-        return u_s_ref
+        # Update states
+        self.speed_ctrl.update(self.T_s, tau_M_ref_lim)
+        self.current_ref.update(self.T_s, tau_M_ref_lim, u_s_ref, u_dc)
+        self.current_ctrl.update(self.T_s, u_s, w_m)
+        self.signal_inj.update(i_s)
+        self.pll.update(self.T_s, err)
+        self.clock.update(self.T_s)
+
+        # PWM output
+        d_abc = self.pwm(self.T_s, u_s_ref, u_dc, theta_m, w_m)
+
+        return self.T_s, d_abc
 
 
 # %%
-class SensorlessFluxObserver:
+class SignalInjection:
     """
-    Sensorless reduced-order flux observer.
+    Estimate the rotor position error based on signal injection.
 
-    This observer is a variant of [1]_. The observer gain decouples the
-    electrical and mechanical dynamics and allows placing the poles of the
-    corresponding linearized estimation error dynamics. This implementation
-    operates in controller coordinates.
+    This signal injection method estimates the rotor position error based on
+    the injected switching frequency signal. The estimate can be used in a 
+    phase-locked loop or in a state observer to robustify low-speed sensorless 
+    operation.
 
     Parameters
     ----------
-    pars : InductionMotorVHzObsCtrlPars
-        Control parameters.
-
-    References
-    ----------
-    .. [1] Hinkkanen, Harnefors, Luomi, "Reduced-order flux observers with
-       stator-resistance adaptation for speed-sensorless induction motor
-       drives," IEEE Trans. Power Electron., 2010,
-       https://doi.org/10.1109/TPEL.2009.2039650
+    par : ModelPars
+        Machine model parameters.
+    U_inj : float
+        Injected voltage amplitude (V).
 
     """
 
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.R_s = pars.R_s
-        self.R_R = pars.R_R
-        self.L_sgm = pars.L_sgm
-        self.alpha = pars.R_R/pars.L_M
-        self.alpha_o = pars.alpha_o
-        self.zeta_inf = pars.zeta_inf
-        # Initial states
-        self.psi_R, self.i_s_old, self.w_m = 0j, 0j, 0
+    def __init__(self, par, U_inj):
+        # Error gain
+        self.k = .5*par.L_d*par.L_q/((par.L_q - par.L_d))
+        # States
+        self._i_s_old, self._i_s_older = 0, 0
+        self.u_sd_inj = U_inj
+
+    def output(self, T_s, i_sq):
+        """
+        Compute the rotor position estimation error.
+
+        Parameters
+        ----------
+        T_s : float
+            Sampling period (s).
+        i_sq : float
+            q-axis stator current (A) in estimated rotor coordinates.
+
+        Returns
+        -------
+        err : float
+            Rotor position estimation error (electrical rad).
+
+        """
+        di_sq = i_sq - 2*self._i_s_old.imag + self._i_s_older.imag
+        err = (self.k/T_s)*di_sq/self.u_sd_inj if np.abs(
+            self.u_sd_inj) > 0 else 0
+        return err
+
+    def update(self, i_s):
+        """
+        Store the old current values for the next sampling period.
+
+        Parameters
+        ----------
+        i_s : complex
+            Stator current in estimated rotor coordinates.
+
+        """
+        # Update the integral states
+        self._i_s_older = self._i_s_old
+        self._i_s_old = i_s
+        # Reverse the d-axis square wave injection voltage
+        self.u_sd_inj = -self.u_sd_inj
 
-    def update(self, u_s, i_s, w_s):
+    def filter_current(self, i_s):
         """
-        Update the states of the observer.
+        Filter the stator current using the previously measured value.
 
         Parameters
         ----------
-        u_s : complex
-            Stator voltage.
         i_s : complex
-            Stator current.
-        w_s : float
-            Angular frequency of the reference frame.
+            Unfiltered stator current (A) in estimated rotor coordinates.
+
+        Returns
+        -------
+        i_s_filt : complex
+            Filtered stator current (A) in estimated rotor coordinates.
 
         """
-        # Decay rate
-        lambd = self.zeta_inf*np.abs(w_s) + .5*self.alpha
-        # Observer gain (without the orthogonal projection which is
-        # embedded into the state update)
-        g_o = 2*lambd/(self.alpha - 1j*self.w_m)
-
-        # Time derivative of the stator current
-        di_s = (i_s - self.i_s_old)/self.T_s
-
-        # Error voltage
-        e = (
-            self.L_sgm*(di_s + 1j*w_s*i_s) + (self.R_s + self.R_R)*i_s -
-            (self.alpha - 1j*self.w_m)*self.psi_R - u_s)
+        # Filter currents
+        i_s_filt = .5*(i_s + self._i_s_old)
+        return i_s_filt
 
-        # Error signal
-        err = e/self.psi_R if np.abs(self.psi_R) > 0 else 0
+
+# %%
+class PhaseLockedLoop:
+    """
+    Simple phase-locked loop for rotor-position estimation.
+
+    Parameters
+    ----------
+    w_o : float
+        Natural frequency (rad/s).
+
+    """
+
+    def __init__(self, w_o):
+        # Gains
+        self.k_p = w_o
+        self.k_i = w_o**2
+        # States
+        self.theta_m, self.w_m = 0, 0
+
+    def update(self, T_s, err):
+        """
+        Update the states for the next sampling period.
+
+        Parameters
+        ----------
+        T_s : float
+            Sampling period (s).
+        err : float
+            Rotor position error (rad).
+
+        """
+        # Speed estimation
+        w_m = self.k_p*err + self.w_m
 
         # Update the states
-        self.w_m -= self.T_s*self.alpha_o*err.imag
-        self.psi_R += self.T_s*(
-            u_s - self.R_s*i_s - self.L_sgm*di_s - 1j*w_s*
-            (self.psi_R + self.L_sgm*i_s) + g_o*self.psi_R*err.real)
-        self.i_s_old = i_s
+        self.w_m += T_s*self.k_i*err
+        self.theta_m += T_s*w_m  # Next line: limit into [-pi, pi)
+        self.theta_m = np.mod(self.theta_m + np.pi, 2*np.pi) - np.pi
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `motulator-0.1.4/motulator/control/im_vector.py` & `motulator-0.1.5/motulator/control/im/_vector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,218 +1,314 @@
 """
-Vector control methods for induction motor drives.
+Vector control methods for induction machine drives.
 
 The algorithms are written based on the inverse-Γ model.
 
 """
-from typing import Callable
-from dataclasses import dataclass, field
+from dataclasses import dataclass, InitVar
 import numpy as np
-
-from motulator.helpers import abc2complex, Bunch
-from motulator.control.common import Ctrl, SpeedCtrl, PWM
+from motulator._helpers import abc2complex
+from motulator.control._common import PWM, Ctrl, ComplexPICtrl, SpeedCtrl
+from motulator._utils import Bunch
 
 
 # %%
 @dataclass
-class InductionMotorVectorCtrlPars:
-    """Vector control parameters for induction motor drives."""
-
-    # pylint: disable=too-many-instance-attributes
-    # Speed reference (in electrical rad/s)
-    w_m_ref: Callable[[float], float] = field(
-        repr=False, default=lambda t: (t > .2)*(2*np.pi*50))
-    # Mode
-    sensorless: bool = True
-    # Sampling period
-    T_s: float = 250e-6
-    # Bandwidths
-    alpha_c: float = 2*np.pi*200
-    alpha_o: float = 2*np.pi*40  # Used only in the sensorless mode
-    alpha_s: float = 2*np.pi*4
-    # Sensored observer
-    g = .2  # Used only in the sensored mode
-    # Maximum values
-    tau_M_max: float = 1.5*14.6
-    i_s_max: float = 1.5*np.sqrt(2)*5
-    # Nominal values
-    psi_R_nom: float = .9
-    u_dc_nom: float = 540
-    # Motor parameter estimates (inverse-Γ model)
-    R_s: float = 3.7
-    R_R: float = 2.1
-    L_sgm: float = .021
-    L_M: float = .224
-    n_p: int = 2
-    J: float = .015
+class ModelPars:
+    """
+    Inverse-Γ model parameters of an induction machine.
+    
+    Parameters
+    ----------
+    R_s : float
+        Stator resistance (Ω).
+    R_R : float
+        Rotor resistance (Ω).
+    L_sgm : float
+        Leakage inductance (H).
+    L_M : float
+        Magnetizing inductance (H).
+    n_p : int
+        Number of pole pairs.  
+    J : float
+        Moment of inertia (kgm²).  
+    
+    """
+    R_s: float = None
+    R_R: float = None
+    L_sgm: float = None
+    L_M: float = None
+    n_p: int = None
+    J: float = None
 
 
 # %%
-class InductionMotorVectorCtrl(Ctrl):
+# pylint: disable=too-many-instance-attributes
+class VectorCtrl(Ctrl):
     """
-    Vector control for an induction motor drive.
+    Vector control for induction machine drives.
 
-    This class interconnects the subsystems of the control system and
-    provides the interface to the solver.
+    This class interconnects the subsystems of the control system and provides 
+    the interface to the solver.
 
     Parameters
     ----------
-    pars : InductionMotorVectorControlPars
-        Control parameters.
+    par : InductionMachinePars
+        Machine model parameters.
+    ref : CurrentReferencePars
+        Parameters for reference generation.
+    T_s : float, optional
+        Sampling period (s). The default is 250e-6.
+    sensorless : bool, optional
+        If True, sensorless control is used. The default is True.
+
+    Attributes
+    ----------
+    current_ref : CurrentReference
+        Current reference generator.
+    observer : Observer
+        Flux and speed observer. 
+    current_ctrl : CurrentCtrl
+        Current controller.
+    speed_ctrl : SpeedCtrl 
+        Speed controller.
+    pwm : PWM
+        Pulse-width modulation.
+    w_m_ref : callable
+        Speed reference (electrical rad/s) as a function of time (s).
 
     """
 
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
+    def __init__(self, par, ref, T_s=250e-6, sensorless=True):
         super().__init__()
-        self.T_s = pars.T_s
-        self.w_m_ref = pars.w_m_ref
-        self.sensorless = pars.sensorless
-        self.n_p = pars.n_p
-        self.speed_ctrl = SpeedCtrl(pars)
-        self.current_ref = CurrentRef(pars)
-        self.current_ctrl = CurrentCtrl(pars)
-        if self.sensorless:
-            self.observer = SensorlessObserver(pars)
-        else:
-            self.observer = Observer(pars)
-        self.pwm = PWM(pars)
+        self.w_m_ref = callable
+        self.T_s = T_s
+        self.sensorless = sensorless
+        self.n_p = par.n_p
+        self.current_ref = CurrentReference(par, ref)
+        self.current_ctrl = CurrentCtrl(par, 2*np.pi*200)
+        self.observer = Observer(par, sensorless=sensorless)
+        self.speed_ctrl = SpeedCtrl(par.J, 2*np.pi*4)
+        self.pwm = PWM()
 
+    # pylint: disable=too-many-locals
     def __call__(self, mdl):
         """
         Run the main control loop.
 
         Parameters
         ----------
-        mdl : InductionMotorDrive
-            Continuous-time model of an induction motor drive for getting the
-            feedback signals.
+        mdl : Drive
+            Continuous-time system model for getting the feedback signals.
 
         Returns
         -------
         T_s : float
-            Sampling period.
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
+            Sampling period (s).
+        d_abc : ndarray, shape (3,)
+            Duty ratios.
 
         """
         # Get the speed reference
-        w_m_ref = self.w_m_ref(self.t)
-
-        # Measure the feedback signals
-        i_s_abc = mdl.motor.meas_currents()  # Phase currents
-        u_dc = mdl.conv.meas_dc_voltage()  # DC-bus voltage
+        w_m_ref = self.w_m_ref(self.clock.t)
 
-        if not self.sensorless:
-            w_m = self.n_p*mdl.mech.meas_speed()  # Rotor speed
-        else:
-            w_m = self.observer.w_m  # Get the estimated speed
+        # Feedback signals
+        i_s_abc = mdl.machine.meas_currents()
+        u_dc = mdl.converter.meas_dc_voltage()
 
         # Get the states
+        if self.sensorless:
+            w_m = self.observer.w_m
+        else:
+            w_m = self.n_p*mdl.mechanics.meas_speed()
         u_s = self.pwm.realized_voltage
-        psi_R = self.observer.psi_R
-        theta_s = self.observer.theta_s
+        psi_R, theta_s = self.observer.psi_R, self.observer.theta_s
 
         # Space vector and coordinate transformation
         i_s = np.exp(-1j*theta_s)*abc2complex(i_s_abc)
 
-        # Outputs
+        # Controller outputs
         tau_M_ref = self.speed_ctrl.output(w_m_ref/self.n_p, w_m/self.n_p)
         i_s_ref, tau_M_ref_lim = self.current_ref.output(tau_M_ref, psi_R)
-        w_s = self.observer.output(u_s, i_s, w_m)  # w_m not used if sensorless
         u_s_ref = self.current_ctrl.output(i_s_ref, i_s)
-        d_abc_ref, u_s_ref_lim = self.pwm.output(u_s_ref, u_dc, theta_s, w_s)
 
         # Save data
         data = Bunch(
             i_s=i_s,
             i_s_ref=i_s_ref,
             psi_R=psi_R,
-            t=self.t,
+            t=self.clock.t,
             tau_M_ref_lim=tau_M_ref_lim,
             theta_s=theta_s,
             u_dc=u_dc,
             u_s=u_s,
             w_m=w_m,
             w_m_ref=w_m_ref,
-            w_s=w_s,
         )
         self.save(data)
 
-        # Update the states
-        self.pwm.update(u_s_ref_lim)
-        self.speed_ctrl.update(tau_M_ref_lim)
-        self.current_ref.update(u_s_ref, u_dc)
-        self.current_ctrl.update(u_s_ref_lim, w_s)
-        self.observer.update(i_s, w_s)
-        self.update_clock(self.T_s)
+        # Compute the flux angular frequency and update the observer states
+        # (w_m needed only in sensored mode)
+        w_s = self.observer(self.T_s, u_s, i_s, w_m)
+
+        # Update the controller states
+        self.speed_ctrl.update(self.T_s, tau_M_ref_lim)
+        self.current_ref.update(self.T_s, u_s_ref, u_dc)
+        self.current_ctrl.update(self.T_s, u_s, w_s)
+        self.clock.update(self.T_s)
 
-        return self.T_s, d_abc_ref
+        # Calculate the duty ratios and update the voltage estimate state
+        d_abc = self.pwm(self.T_s, u_s_ref, u_dc, theta_s, w_s)
+
+        return self.T_s, d_abc
 
 
 # %%
-class CurrentRef:
+class CurrentCtrl(ComplexPICtrl):
     """
-    Current reference calculation.
+    2DOF PI current controller for induction machines.
 
-    This method includes field-weakenting operation based on the unlimited
-    voltage reference feedback. The breakdown torque and current limits are
-    taken into account.
+    This class provides an interface for a current controller for induction 
+    machines. The gains are initialized based on the desired closed-loop 
+    bandwidth and the leakage inductance. 
 
     Parameters
     ----------
-    pars : InductionMotorVectorCtrlPars
-        Control parameters.
+    par : ModelPars
+        Machine parameters, contains the leakage inductance `L_sgm` (H).  
+    alpha_c : float
+        Closed-loop bandwidth (rad/s).
 
-    Notes
-    -----
-    The field-weakening method and its tuning corresponds roughly to [1]_.
+    """
+
+    def __init__(self, par, alpha_c):
+        k_t = alpha_c*par.L_sgm
+        k_i = alpha_c*k_t
+        k_p = 2*k_t
+        super().__init__(k_p, k_i, k_t)
+
+
+# %%
+# pylint: disable=too-many-instance-attributes
+@dataclass
+class CurrentReferencePars:
+    """
+    Parameters for reference generation.
+
+    This dataclass stores the nominal and limit values needed for reference 
+    generation. For calculating the rotor flux reference, the machine parameters 
+    are also required.
+
+    Parameters
+    ----------
+    par : ModelPars
+        Machine model parameters.
+    i_s_max : float
+        Maximum stator current (A). 
+    u_s_nom : float, optional
+        Nominal stator voltage (V). The default is sqrt(2/3)*400.
+    w_s_nom : float, optional
+        Nominal stator angular frequency (rad/s). The default is 2*pi*50.
+    psi_R_nom : float, optional
+        Nominal rotor flux linkage (Vs). The default is 
+        `(u_s_nom/w_s_nom)/(1 + L_sgm/L_M)`.
+    k_fw : float, optional
+        Field-weakening gain (1/H). The default is `2*R_R/(w_s_nom*L_sgm**2)`.
+    k_u : float, optional
+        Voltage utilization factor. The default is 0.95.
+    
+    """
+    par: InitVar[ModelPars] = None
+    i_s_max: float = None
+    u_s_nom: InitVar[float] = np.sqrt(2/3)*400
+    w_s_nom: InitVar[float] = 2*np.pi*50
+    psi_R_nom: float = None
+    k_fw: float = None
+    k_u: float = 0.95
+
+    def __post_init__(self, par, u_s_nom, w_s_nom):
+        psi_s_nom = u_s_nom/w_s_nom  # Nominal stator flux
+        if self.psi_R_nom is None:
+            # Nominal rotor flux (omitting the slip)
+            self.psi_R_nom = psi_s_nom/(1 + par.L_sgm/par.L_M)
+        if self.k_fw is None:
+            self.k_fw = 2*par.R_R/(w_s_nom*par.L_sgm**2)
+
+
+# %%
+class CurrentReference:
+    """
+    Current reference generation.
+
+    In the base-speed region, the current reference in rotor-flux coordinates is
+    given by::
+
+        i_s_ref = psi_R_nom/L_M + 1j*tau_M_ref/(1.5*n_p*abs(psi_R))
+
+    where `psi_R_nom` is the nominal rotor flux magnitude and `psi_R` is the 
+    estimated rotor flux. The field-weakening operation is based on adjusting 
+    the flux-producing current component::
+
+        i_s_ref.real = (k_fw/s)*(u_s_max - abs(u_s_ref))
+
+    where `1/s` refers to integration, ``u_s_max = k_u*u_dc/sqrt(3)`` is the 
+    maximum stator voltage in the linear modulation region, `u_s_ref` is the 
+    (unlimited) stator voltage reference, and `k_fw` is the field-weakening 
+    gain. The field-weakening method and its tuning corresponds roughly to
+    [#Hin2006]_. Furthermore, the torque-producing current component 
+    `i_s_ref.imag` is limited based on the maximum stator current and the 
+    breakdown slip. 
+
+    Parameters
+    ----------
+    par : ModelPars
+        Machine model parameters.
+    ref : CurrentReferencePars
+        Reference generation parameters.
 
     References
     ----------
-    .. [1] Hinkkanen, Luomi, "Braking scheme for vector-controlled induction
-       motor drives equipped with diode rectifier without braking resistor,"
-       IEEE Trans. Ind. Appl., 2006, https://doi.org/10.1109/TIA.2006.880852
+    .. [#Hin2006] Hinkkanen, Luomi, "Braking scheme for vector-controlled 
+       induction motor drives equipped with diode rectifier without braking 
+       resistor," IEEE Trans. Ind. Appl., 2006, 
+       https://doi.org/10.1109/TIA.2006.880852
 
     """
 
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.i_s_max = pars.i_s_max
-        self.L_sgm = pars.L_sgm
-        self.n_p = pars.n_p
-        # Local parameters for initializing the constants
-        psi_R_nom = pars.psi_R_nom
-        L_M = pars.L_M
-        R_R = pars.R_R
-        u_dc_nom = pars.u_dc_nom
+    def __init__(self, par, ref):
+        # Machine model parameters
+        self.L_sgm = par.L_sgm
+        self.n_p = par.n_p
+        # Other parameters
+        self.i_s_max = ref.i_s_max
+        self.k_u = ref.k_u
+        # Field-weakening gain
+        self.k_fw = ref.k_fw
         # Nominal d-axis current
-        self.i_sd_nom = psi_R_nom/L_M
-        # Field weakening
-        self.gain_fw = 3*R_R*psi_R_nom/(pars.L_sgm*u_dc_nom)**2
+        self.i_sd_nom = ref.psi_R_nom/par.L_M
         # State variable
         self.i_sd_ref = self.i_sd_nom
 
     def output(self, tau_M_ref, psi_R):
         """
         Compute the stator current reference.
 
         Parameters
         ----------
         tau_M_ref : float
-            Torque reference.
+            Torque reference (Nm).
         psi_R : float
-            Rotor flux magnitude.
+            Rotor flux magnitude (Vs).
 
         Returns
         -------
         i_s_ref : complex
-            Stator current reference.
-        tau_M : float
-            Limited torque reference.
+            Stator current reference (A).
+        tau_M_ref_lim : float
+            Limited torque reference (Nm).
 
         """
 
         def q_axis_current_limit(i_sd_ref, psi_R):
             # Priority given to the d component
             i_sq_max1 = np.sqrt(self.i_s_max**2 - i_sd_ref**2)
             # Breakdown torque limit
@@ -222,309 +318,176 @@
             return i_sq_max
 
         # q-axis current reference
         i_sq_ref = tau_M_ref/(1.5*self.n_p*psi_R) if psi_R > 0 else 0
 
         # Limit the current
         i_sq_max = q_axis_current_limit(self.i_sd_ref, psi_R)
-        if np.abs(i_sq_ref) > i_sq_max:
-            i_sq_ref = np.sign(i_sq_ref)*i_sq_max
+        i_sq_ref = np.clip(i_sq_ref, -i_sq_max, i_sq_max)
 
         # Current reference
         i_s_ref = self.i_sd_ref + 1j*i_sq_ref
 
         # Limited torque (for the speed controller)
         tau_M_ref_lim = 1.5*self.n_p*psi_R*i_sq_ref
 
         return i_s_ref, tau_M_ref_lim
 
-    def update(self, u_s_ref, u_dc):
+    def update(self, T_s, u_s_ref, u_dc):
         """
         Field-weakening based on the unlimited reference voltage.
 
         Parameters
         ----------
+        T_s : float
+            Sampling period (s)
         u_s_ref : complex
-            Unlimited stator voltage reference.
+            Unlimited stator voltage reference (V).
         u_dc : float
-            DC-bus voltage.
+            DC-bus voltage (V).
 
         """
-        u_s_max = u_dc/np.sqrt(3)
-        self.i_sd_ref += self.T_s*self.gain_fw*(
-            u_s_max**2 - np.abs(u_s_ref)**2)
-        if self.i_sd_ref > self.i_sd_nom:
-            self.i_sd_ref = self.i_sd_nom
-        elif self.i_sd_ref < -self.i_s_max:
-            self.i_sd_ref = -self.i_s_max
+        u_s_max = self.k_u*u_dc/np.sqrt(3)
+        self.i_sd_ref += T_s*self.k_fw*(u_s_max - np.abs(u_s_ref))
+        self.i_sd_ref = np.clip(self.i_sd_ref, -self.i_s_max, self.i_sd_nom)
 
 
 # %%
-class CurrentCtrl:
+class Observer:
     """
-    2DOF PI current controller.
-
-    This controller corresponds to [2]_. The continuous-time complex-vector
-    design corresponding to (13) is used here. The rotor flux linkage is
-    considered as a quasi-constant disturbance. This design could be
-    equivalently presented as a 2DOF PI controller.
+    Reduced-order flux observer for induction machines.
 
+    This class implements a reduced-order flux observer for induction machines.
+    Both sensored and sensorless operation are supported. The observer structure
+    is similar to [#Hin2010]_. Both sensored and sensorless operation are 
+    supported. The observer operates in estimated rotor flux coordinates. 
+    
     Parameters
     ----------
-    pars : InductionMotorVectorCtrlPars
-        Control parameters.
-
-    Notes
-    -----
-    This implementation does not take the magnetic saturation into account.
+    par : ModelPars
+        Machine model parameters.
+    k : callable, optional
+        Observer gain as a function of the rotor angular speed. The default is 
+        ``lambda w_m: (0.5*R_R/L_M + 0.2*abs(w_m))/(R_R/L_M - 1j*w_m)`` if
+        `sensorless` else ``lambda w_m: 1 + 0.2*abs(w_m)/(R_R/L_M - 1j*w_m)``.
+    alpha_o : float, optional
+        Observer bandwidth (rad/s). The default is 2*pi*40.
+    sensorless : bool, optional
+        If True, sensorless mode is used. The default is True.
 
-    References
+    Attributes
     ----------
-    .. [2] Awan, Saarakkala, Hinkkanen, "Flux-linkage-based current control of
-       saturated synchronous motors," IEEE Trans. Ind. Appl. 2019,
-       https://doi.org/10.1109/TIA.2019.2919258
-
-    """
-
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.L_sgm = pars.L_sgm
-        self.alpha_c = pars.alpha_c
-        # Integral state
-        self.u_i = 0
-        # Memory for the update method
-        self.e = 0
-        self.u_s_ref = 0
-
-    def output(self, i_s_ref, i_s):
-        """
-        Compute the unlimited voltage reference.
-
-        Parameters
-        ----------
-        i_s_ref : complex
-            Stator current reference.
-        i_s : complex
-            Measured stator current.
-
-        Returns
-        -------
-        u_s_ref : complex
-            Unlimited voltage reference.
-
-        """
-        psi_sgm_ref = self.L_sgm*i_s_ref
-        psi_sgm = self.L_sgm*i_s
-        k_t = self.alpha_c
-        k = 2*self.alpha_c
-        self.u_s_ref = k_t*psi_sgm_ref - k*psi_sgm + self.u_i
-        # Error (scaled, corresponds to the leakage flux linkage)
-        self.e = psi_sgm_ref - psi_sgm
-
-        return self.u_s_ref
-
-    def update(self, u_s_ref_lim, w_s):
-        """
-        Update the integral state.
-
-        Parameters
-        ----------
-        u_s_ref_lim : complex
-            Limited voltage reference.
-        w_s : float
-            Angular stator frequency.
-
-        """
-        k_i = self.alpha_c*(self.alpha_c + 1j*w_s)
-        k_t = self.alpha_c
-        self.u_i += self.T_s*k_i*(self.e + (u_s_ref_lim - self.u_s_ref)/k_t)
-
-
-# %%
-class SensorlessObserver:
-    """
-    Sensorless reduced-order flux observer.
-
-    This observer corresponds to [3]_. The observer gain decouples the
-    electrical and mechanical dynamics and allows placing the poles of the
-    corresponding linearized estimation error dynamics. This implementation
-    operates in estimated rotor flux coordinates.
-
-    Parameters
-    ----------
-    pars : InductionMotorVectorCtrlPars
-        Control parameters.
+    psi_R : float
+        Rotor flux magnitude estimate (Vs).
+    theta_s : float
+        Rotor flux angle estimate (rad).
+    w_m : float
+        Rotor angular speed estimate (electrical rad/s). In sensored mode, this
+        is the measured low-pass-filtered speed.
 
     Notes
     -----
-    This implementation corresponds to (26)-(30) in [3]_ with the choice
-    c = w_s**2 in (17). The closed-loop poles, cf. (40), can still be
-    affected via the coefficient b > 0.
+    The pure voltage model corresponds to ``k = lambda w_m: 0``, resulting in 
+    the marginally stable estimation-error dynamics. The current model is 
+    obtained by setting ``k = lambda w_m: 1``. 
 
     References
     ----------
-    .. [3] Hinkkanen, Harnefors, Luomi, "Reduced-order flux observers with
-       stator-resistance adaptation for speed-sensorless induction motor
-       drives," IEEE Trans. Power Electron., 2010,
+    .. [#Hin2010] Hinkkanen, Harnefors, Luomi, "Reduced-order flux observers 
+       with stator-resistance adaptation for speed-sensorless induction motor 
+       drives," IEEE Trans. Power Electron., 2010, 
        https://doi.org/10.1109/TPEL.2009.2039650
 
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.R_s = pars.R_s
-        self.R_R = pars.R_R
-        self.L_sgm = pars.L_sgm
-        self.L_M = pars.L_M
-        self.alpha_o = pars.alpha_o
-        self.zeta_inf = .2
-        # Initial states
-        self.theta_s, self.psi_R, self.i_s_old, self.w_m = 0, 0, 0, 0
-        # Store for the update method to avoid recalculation
-        self.dpsi_R, self.w_r = 0, 0
-
-    def output(self, u_s, i_s, *_):
-        """
-        Compute the output.
+    def __init__(self, par, k=None, alpha_o=2*np.pi*40, sensorless=True):
+        # Model parameters
+        self.R_s, self.R_R, self.L_sgm = par.R_s, par.R_R, par.L_sgm
+        self.alpha = par.R_R/par.L_M
+
+        # Other parameters
+        self.alpha_o = alpha_o
+        self.sensorless = sensorless
 
-        Parameters
-        ----------
-        u_s : complex
-            Stator voltage in estimated rotor flux coordinates.
-        i_s : complex
-            Stator current in estimated rotor flux coordinates.
-
-        Returns
-        -------
-        w_s : float
-            Angular frequency of the rotor flux.
-
-        """
-        alpha = self.R_R/self.L_M
-
-        # Observer gain (17) with c = w_s**2 (without the orthogonal projection
-        # which is embedded into the state update)
-        b = alpha + 2*self.zeta_inf*np.abs(self.w_m)
-        g = b/(alpha - 1j*self.w_m)
-
-        # Induced voltage from stator quantities, cf. (7)
-        e_s = u_s - self.R_s*i_s - self.L_sgm*(i_s - self.i_s_old)/self.T_s
-        # Induced voltage (8) from the rotor quantities
-        e_r = self.R_R*i_s - (alpha - 1j*self.w_m)*self.psi_R
-
-        # Angular frequency of the rotor flux vector
-        den = self.psi_R + self.L_sgm*(i_s.real + g.imag*i_s.imag)
-        if den > 0:
-            w_s = (e_s.imag + g.imag*(e_r - e_s).real)/den
+        # Observer gains
+        self.k1 = k
+        if self.sensorless:
+            if self.k1 is None:  # If not given, use the default gains
+                self.k1 = lambda w_m: (.5*self.alpha + .2*np.abs(w_m))/(
+                    self.alpha - 1j*w_m)
+            self.k2 = self.k1
         else:
-            w_s = self.w_m
+            if self.k1 is None:
+                self.k1 = lambda w_m: 1 + .2*np.abs(w_m)/(self.alpha - 1j*w_m)
+            self.k2 = 0*self.k1
+
+        # States
+        self.psi_R, self.theta_s, self.w_m, self._i_s_old = 0, 0, 0, 0
+
+    def _f(self, T_s, u_s, i_s, w_m):
+        # Right-hand-side of the differential equation.
+
+        # Induced voltage from stator quantities (without the w_s term that is
+        # taken into account separately to avoid an algebraic loop)
+        v_s = u_s - self.R_s*i_s - self.L_sgm*(i_s - self._i_s_old)/T_s
 
-        # Slip angular frequency (stored for the update method)
-        self.w_r = e_r.imag/self.psi_R if self.psi_R > 0 else 0
+        # Induced voltage from the rotor quantities
+        v_r = self.R_R*i_s - (self.alpha - 1j*w_m)*self.psi_R
 
-        # Increment of the flux magnitude (stored for the update method)
-        self.dpsi_R = ((1 - g.real)*(e_s.real + w_s*self.L_sgm*i_s.imag) +
-                       g.real*e_r.real)
+        # Angular frequency of the rotor flux vector
+        k1, k2 = self.k1(w_m), self.k2(w_m)
+        den = self.psi_R + self.L_sgm*np.real((1 - k1)*i_s + k2*np.conj(i_s))
+        num = np.imag(v_s + k1*(v_r - v_s) + k2*np.conj(v_r - v_s))
+        w_s = num/den if den > 0 else w_m
+
+        # Compute the derivative of the flux magnitude for the state update
+        v = v_s - 1j*w_s*self.L_sgm*i_s
+        dpsi_R = np.real(v + k1*(v_r - v) + k2*np.conj(v_r - v))
 
-        return w_s
+        return dpsi_R, w_s  # Note: w_s = dtheta_s
 
-    def update(self, i_s, w_s):
-        """Update the states for the next sampling period."""
-        self.w_m += self.T_s*self.alpha_o*(w_s - self.w_r)
-        self.psi_R += self.T_s*self.dpsi_R
-        self.theta_s += self.T_s*w_s  # Next line: limit into [-pi, pi)
+    # pylint: disable=too-many-arguments
+    def _update(self, T_s, i_s, dpsi_R, w_s, w_m):
+        # Update the states
+        self.psi_R += T_s*dpsi_R
+        self.theta_s += T_s*w_s  # Next line: limit into [-pi, pi)
         self.theta_s = np.mod(self.theta_s + np.pi, 2*np.pi) - np.pi
-        self.i_s_old = i_s
-
+        self.w_m += T_s*self.alpha_o*(w_m - self.w_m)
+        # Store the old current
+        self._i_s_old = i_s
 
-# %%
-class Observer:
-    """
-    Sensored reduced-order flux observer.
-
-    This reduced-order flux observer [4]_ uses the measured rotor speed. The
-    selected default gain allows smooth transition from the current model at
-    zero speed to the (damped) voltage model at higher speeds.
-
-    Parameters
-    ----------
-    pars : InductionMotorVectorCtrlPars
-        Control parameters.
-
-    Notes
-    -----
-    This implementation places the pole in synchronous coordinates at::
-
-        s = -R_R/L_M - g*abs(w_m) - 1j*(w_s - w_m)
-
-    References
-    ----------
-    .. [4] Verghese, Sanders, “Observers for flux estimation in induction
-       machines,” IEEE Trans. Ind. Electron., 1988,
-       https://doi.org/10.1109/41.3067
-
-    """
-
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.R_s = pars.R_s
-        self.R_R = pars.R_R
-        self.L_sgm = pars.L_sgm
-        self.alpha = pars.R_R/pars.L_M
-        # Nonnegative gain for damping
-        self.g = pars.g
-        # Initial states
-        self.theta_s, self.psi_R, self.i_s_old = 0, 0, 0
-        # Store for the update method to avoid recalculation
-        self.dpsi_R = 0
-
-    def output(self, u_s, i_s, w_m):
+    def __call__(self, T_s, u_s, i_s, w_m=None):
         """
-        Compute the output of the observer.
+        Compute the angular frequency of the flux and update the states.
 
         Parameters
         ----------
+        T_s : float
+            Sampling period (s).
         u_s : complex
-            Stator voltage in estimated rotor flux coordinates.
+            Stator voltage (V) in estimated rotor flux coordinates.
         i_s : complex
-            Stator current in estimated rotor flux coordinates.
-        w_m : float
-            Rotor angular speed (in electrical rad/s)
+            Stator current (A) in estimated rotor flux coordinates.
+        w_m : float, optional
+            Rotor angular speed (electrical rad/s). This signal is only used in
+            sensored mode. The default is None.
 
         Returns
         -------
         w_s : float
-            Angular frequency of the rotor flux.
+            Angular frequency (rad/s) of the rotor flux estimate.
 
         """
-        # The observer pole could be placed arbitrarily by means of the
-        # observer gain k. The current model would be obtained using k = 1,
-        # resulting in the pole at s = -R_R/L_M - 1j*(w_s - w_m). The pure
-        # voltage model corresponds to k = 0, resulting in the marginally
-        # stable pole at s = -1j*w_s.
-
-        # This gain leads to s = -alpha - g*abs(w_m) - 1j*(w_s - w_m)
-        k = 1 + self.g*np.abs(w_m)/(self.alpha - 1j*w_m)
-
-        # Induced voltage from the stator quantities
-        e_s = u_s - self.R_s*i_s - self.L_sgm*(i_s - self.i_s_old)/self.T_s
-        # Induced voltage from the rotor quantities
-        e_r = self.R_R*i_s - (self.alpha - 1j*w_m)*self.psi_R
-
-        # Angular frequency of the rotor flux vector
-        den = self.psi_R + self.L_sgm*((1 - k)*i_s).real
-        v = (1 - k)*e_s + k*e_r
-        w_s = v.imag/den if den > 0 else w_m
+        # Compute the time derivative of the flux estimate
+        if self.sensorless:
+            dpsi_R, w_s = self._f(T_s, u_s, i_s, self.w_m)
+            # Slip and unfiltered speed estimates
+            w_r = self.R_R*i_s.imag/self.psi_R if self.psi_R > 0 else 0
+            w_m = w_s - w_r
+        else:
+            dpsi_R, w_s = self._f(T_s, u_s, i_s, w_m)
 
-        # Increment of the flux magnitude (stored for the update method)
-        self.dpsi_R = v.real + w_s*self.L_sgm*((1 - k)*i_s).imag
+        # Update the states
+        self._update(T_s, i_s, dpsi_R, w_s, w_m)
 
         return w_s
-
-    def update(self, i_s, w_s):
-        """Update the states for the next sampling period."""
-        self.psi_R += self.T_s*self.dpsi_R
-        self.theta_s += self.T_s*w_s  # Next line: limit into [-pi, pi)
-        self.theta_s = np.mod(self.theta_s + np.pi, 2*np.pi) - np.pi
-        self.i_s_old = i_s
```

### Comparing `motulator-0.1.4/motulator/control/im_vhz.py` & `motulator-0.1.5/motulator/control/im/_vhz.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,183 +1,157 @@
 """
 V/Hz control for induction motor drives.
 
-The method is similar to [1]_. Open-loop V/Hz control can be obtained as a
-special case by choosing::
+The method is similar to [#Hin2022]_. Open-loop V/Hz control can be obtained as 
+a special case by choosing::
 
     R_s, R_R = 0, 0
     k_u, k_w = 0, 0
 
-Notes
------
-The low-pass-filtered values are marked with ref at the end of the variable
-name. These slowly varying quasi-steady-state quantities can be seen to
-represent the operating point (marked with the subscript 0 in [1]_).
-
 References
 ----------
-.. [1] Hinkkanen, Tiitinen, Mölsä, Harnefors, "On the stability of
+.. [#Hin2022] Hinkkanen, Tiitinen, Mölsä, Harnefors, "On the stability of
    volts-per-hertz control for induction motors," IEEE J. Emerg. Sel. Topics
    Power Electron., 2022, https://doi.org/10.1109/JESTPE.2021.3060583
 
 """
 # %%
-from typing import Callable
-from dataclasses import dataclass, field
 import numpy as np
-from motulator.control.common import Ctrl, PWM, RateLimiter
-from motulator.helpers import abc2complex, Bunch
-
-
-# %%
-@dataclass
-class InductionMotorVHzCtrlPars:
-    """V/Hz control parameters."""
-
-    # pylint: disable=too-many-instance-attributes
-    # Speed reference (in electrical rad/s)
-    w_m_ref: Callable[[float], float] = field(
-        repr=False, default=lambda t: (t > .2)*(2*np.pi*50))
-    T_s: float = 250e-6
-    six_step: bool = False
-    psi_s_nom: float = 1.04  # 1 p.u.
-    rate_limit: float = 2*np.pi*120
-    # Motor parameter estimates
-    R_s: float = 3.7
-    R_R: float = 2.1
-    L_sgm: float = .021
-    L_M: float = .224
-    k_u: float = 1
-    k_w: float = 4
+from motulator.control._common import Ctrl, PWM
+from motulator._helpers import abc2complex
+from motulator._utils import Bunch
 
 
 # %%
-class InductionMotorVHzCtrl(Ctrl):
+class VHzCtrl(Ctrl):
     """
     V/Hz control with the stator current feedback.
 
     Parameters
     ----------
-    pars : InductionMotorVHzCtrlPars
+    par : ModelPars
         Control parameters.
 
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
+    def __init__(self, T_s, par, psi_s_nom, k_u=1., k_w=4., six_step=False):
         super().__init__()
-        self.T_s = pars.T_s
-        self.w_m_ref = pars.w_m_ref
+        self.T_s = T_s
+        self.w_m_ref = callable
+        # Motor parameters
+        self.R_s, self.R_R = par.R_s, par.R_R
+        self.L_sgm, self.L_M = par.L_sgm, par.L_M
+        # Control parameters
+        self.k_u, self.k_w = k_w, k_u
+        self.psi_s_ref = psi_s_nom
+        w_rb = self.R_R*(self.L_M + self.L_sgm)/(self.L_sgm*self.L_M)
+        self.alpha_f = .1*w_rb
+        self.alpha_i = .1*w_rb
         # Instantiate classes
-        self.pwm = PWM(pars)
-        self.rate_limiter = RateLimiter(pars)
-        # Parameters
-        self.k_u = pars.k_u
-        self.k_w = pars.k_w
-        self.psi_s_ref = pars.psi_s_nom
-        self.R_s = pars.R_s
-        self.R_R = pars.R_R
-        self.L_sgm = pars.L_sgm
-        self.L_M = pars.L_M
-        w_rb = pars.R_R*(pars.L_M + pars.L_sgm)/(pars.L_sgm*pars.L_M)
-        self.alpha_f: float = .1*w_rb
-        self.alpha_i: float = .1*w_rb
+        self.pwm = PWM(six_step=six_step)
+        self.rate_limiter = callable
+        self.six_step = six_step
         # States
-        self.i_s_ref = 0j
-        self.theta_s = 0
-        self.w_r_ref = 0
+        self.i_s_ref, self.theta_s, self.w_r_ref = 0j, 0, 0
+        # self.T_s0 = T_s
+        # self.N = 100
 
     def __call__(self, mdl):
         """
         Run the main control loop.
 
         Parameters
         ----------
-        mdl : InductionMotorDrive
-            Continuous-time model of an induction motor drive for getting the
-            feedback signals.
+        mdl : Drive
+            Continuous-time model for getting the feedback signals.
 
         Returns
         -------
         T_s : float
-            Sampling period.
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
+            Sampling period (s).
+        d_abc : ndarray, shape (3,)
+            Duty ratios.
 
         """
         # Rate limit the frequency reference
-        w_m_ref = self.rate_limiter(self.w_m_ref(self.t))
+        w_m_ref = self.rate_limiter(self.T_s, self.w_m_ref(self.clock.t))
 
         # Measure the feedback signals
-        i_s_abc = mdl.motor.meas_currents()  # Phase currents
-        u_dc = mdl.conv.meas_dc_voltage()  # DC-bus voltage
+        i_s_abc = mdl.machine.meas_currents()  # Phase currents
+        u_dc = mdl.converter.meas_dc_voltage()  # DC-bus voltage
 
         # Space vector transformation
-        i_s = np.exp(-1j*self.theta_s)*abc2complex(i_s_abc)
+        theta_s = self.theta_s
+        i_s = np.exp(-1j*theta_s)*abc2complex(i_s_abc)
 
         # Slip compensation
         w_s_ref = w_m_ref + self.w_r_ref
 
         # Dynamic stator frequency and slip frequency
-        w_s, w_r = self.stator_freq(w_s_ref, i_s)
+        w_s, w_r = self._stator_freq(w_s_ref, i_s)
 
         # Voltage reference
-        u_s_ref = self.voltage_reference(w_s, i_s)
+        u_s_ref = self._voltage_reference(w_s, i_s)
 
-        # Compute the duty ratios
-        u_s = self.pwm.realized_voltage  # Used only for datalogging
-        d_abc_ref = self.pwm(u_s_ref, u_dc, self.theta_s, w_s)
+        # TODO: Synchronize the PWM to the stator frequency in overmodulation,
+        # a simplistic approach given below.
+        # f_s = w_s/(2*np.pi)  # Stator frequency
+        # if self.six_step and self.N*np.abs(f_s) > 1/self.T_s0:
+        #     self.T_s = 1/(self.N*f_s)
+        # else:
+        #     self.T_s = self.T_s0
 
         # Data logging
         data = Bunch(
             i_s=i_s,
             i_s_ref=self.i_s_ref,
             psi_s_ref=self.psi_s_ref,
-            t=self.t,
+            t=self.clock.t,
             theta_s=self.theta_s,
             u_dc=u_dc,
-            u_s=u_s,
+            u_s=self.pwm.realized_voltage,
             w_m_ref=w_m_ref,
             w_r=w_r,
             w_s=w_s,
         )
         self.save(data)
 
-        # Update the states
+        # Update the states. Note that the low-pass-filtered values are marked
+        # with ref at the end of the variable name.
         self.i_s_ref += self.T_s*self.alpha_i*(i_s - self.i_s_ref)
         self.w_r_ref += self.T_s*self.alpha_f*(w_r - self.w_r_ref)
         self.theta_s += self.T_s*w_s  # Next line: limit into [-pi, pi)
         self.theta_s = np.mod(self.theta_s + np.pi, 2*np.pi) - np.pi
-        self.update_clock(self.T_s)
+        self.clock.update(self.T_s)
 
-        return self.T_s, d_abc_ref
+        # Compute the duty ratios
+        d_abc = self.pwm(self.T_s, u_s_ref, u_dc, theta_s, w_s)
 
-    def stator_freq(self, w_s_ref, i_s):
-        """
-        Compute the dynamic stator frequency.
+        return self.T_s, d_abc
 
-        This computes the dynamic stator frequency reference used in the
-        coordinate transformations.
+    def _stator_freq(self, w_s_ref, i_s):
+        # Compute the stator frequency for coordinate transformations
 
-        """
         # Operating-point quantities
         psi_R_ref = self.psi_s_ref - self.L_sgm*self.i_s_ref
         psi_R_ref_sqr = np.abs(psi_R_ref)**2
         # Compute the dynamic stator frequency
         if psi_R_ref_sqr > 0:
             # Slip estimate based on the measured current
             w_r = self.R_R*np.imag(i_s*np.conj(psi_R_ref))/psi_R_ref_sqr
             # Dynamic frequency
             w_s = w_s_ref + self.k_w*(self.w_r_ref - w_r)
         else:
             w_s, w_r = 0, 0
         return w_s, w_r
 
-    def voltage_reference(self, w_s, i_s):
-        """Compute the stator voltage reference."""
+    def _voltage_reference(self, w_s, i_s):
+        # Compute the stator voltage reference
+
         # Nominal magnetizing current
         i_sd_nom = self.psi_s_ref/(self.L_M + self.L_sgm)
         # Operating-point current for RI compensation
         i_s_ref0 = i_sd_nom + 1j*self.i_s_ref.imag
         # Term -R_s omitted to avoid problems due to the voltage saturation
         # k = -R_s + k_u*L_sgm*(alpha + 1j*w_m0)
         k = self.k_u*self.L_sgm*(self.R_R/self.L_M + 1j*w_s)
```

### Comparing `motulator-0.1.4/motulator/control/sm_flux_vector.py` & `motulator-0.1.5/motulator/control/sm/_obs_vhz.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,238 +1,251 @@
-"""
-Flux-vector control for synchronous motor drives.
+"""Observer-based V/Hz control of synchronous motor drives."""
 
-This implements a version of stator-flux-vector control [1]_. Rotor coordinates 
-as well as decoupling between the stator flux and torque channels are used [2]_. 
-Here, the stator flux magnitude and the electromagnetic torque are selected as
-controllable variables. Proportional controllers are used for simplicity. The 
-magnetic saturation is not considered in this implementation.
-
-References
-----------
-.. [1] Pellegrino, Armando, Guglielmi, “Direct flux field-oriented control of
-   IPM drives with variable DC link in the field-weakening region,” IEEE Trans.
-   Ind. Appl., 2009, https://doi.org/10.1109/TIA.2009.2027167
-
-.. [2] Awan, Hinkkanen, Bojoi, Pellegrino, "Stator-flux-oriented control of
-   synchronous motors: A systematic design procedure," IEEE Trans. Ind. Appl.,
-   2019, https://doi.org/10.1109/TIA.2019.2927316
-
-"""
-from typing import Callable
-from dataclasses import dataclass, field
+from dataclasses import dataclass, InitVar
 import numpy as np
-from motulator.helpers import abc2complex, Bunch
-from motulator.control.common import Ctrl, SpeedCtrl, PWM
-from motulator.control.sm_vector import SensorlessObserver
-from motulator.control.sm_obs_vhz import FluxTorqueRef
+from motulator._helpers import abc2complex
+from motulator.control._common import Ctrl, PWM, RateLimiter
+from motulator.control.sm._flux_vector import (
+    FluxTorqueReference, FluxTorqueReferencePars)
+from motulator._utils import Bunch
 
 
 # %%
+# pylint: disable=too-many-instance-attributes
 @dataclass
-class SynchronousMotorFluxVectorCtrlPars:
-    """Control parameters: flux-vector control for synchronous motor drives."""
+class ObserverBasedVHzCtrlPars(FluxTorqueReferencePars):
+    """
+    Parameters for the control system.
 
-    # pylint: disable=too-many-instance-attributes
-    # Speed reference (in electrical rad/s)
-    w_m_ref: Callable[[float], float] = field(
-        repr=False, default=lambda t: (t > .2)*(2*np.pi*75))
-    # Mode
-    sensorless: bool = True
-    # Sampling period
-    T_s: float = 250e-6
-    # Flux reference limits
-    psi_s_min: float = None
-    psi_s_max: float = None
-    # Voltage marginal
-    k_u: float = .9
-    # Bandwidths
-    alpha_psi: float = 2*np.pi*150
-    alpha_tau: float = 2*np.pi*50
-    alpha_s: float = 2*np.pi*4
-    # Maximum values
-    tau_M_max: float = 1.5*14
-    i_s_max: float = 1.5*np.sqrt(2)*5.
-    # Motor parameter estimates
-    R_s: float = 3.6
-    L_d: float = .036
-    L_q: float = .051
-    psi_f: float = .545
-    n_p: int = 3
-    J: float = .015
-    # Sensorless observer (used only in the sensorless mode)
-    w_o: float = 2*np.pi*100
-    zeta_inf: float = .2
-    # Sensored observer (used only in the sensored mode)
-    g: float = 2*np.pi*15
+    This class extends FluxTorqueReferencePars with the parameters needed for
+    the observer-based V/Hz control.
+
+    Parameters
+    ----------
+    alpha_psi : float, optional
+        Flux control bandwidth (rad/s). The default is 2*pi*50.
+    alpha_tau : float
+        Torque control bandwidth (rad/s). The default is 2*pi*50.
+    alpha_f : float, optional
+        Bandwidth of the high-pass filter (rad/s). The default is 2*pi*1.
+
+    """
+    alpha_psi: float = 2*np.pi*50
+    alpha_tau: InitVar[float] = 2*np.pi*50
+    alpha_f: float = 2*np.pi*1
+
+    # pylint: disable=arguments-differ
+    def __post_init__(self, par, alpha_tau):
+        super().__post_init__(par)
+        # Gain k_tau
+        G = (par.L_d - par.L_q)/(par.L_d*par.L_q)
+        psi_s0 = par.psi_f if par.psi_f > 0 else self.psi_s_min
+        if par.psi_f > 0:  # PMSM or PM-SyRM
+            c_delta0 = 1.5*par.n_p*(par.psi_f*psi_s0/par.L_d - G*psi_s0**2)
+        else:  # SyRM
+            c_delta0 = 1.5*par.n_p*G*psi_s0**2
+        self.k_tau = alpha_tau/c_delta0
 
 
 # %%
-class SynchronousMotorFluxVectorCtrl(Ctrl):
+class ObserverBasedVHzCtrl(Ctrl):
     """
-    Flux-vector control for synchronous motor drives.
+    Observer-based V/Hz control for synchronous motors.
 
-    This class interconnects the subsystems of the control system and
-    provides the interface to the solver.
+    This observer-based V/Hz control control method is based on [#Tii2022]_.
 
     Parameters
     ----------
-    pars : SynchronousMotoroFluxVectorCtrlPars
-        Control parameters.
+    par : ModelPars
+        Machine model parameters.
+    ctrl_par : ObserverBasedVHzCtrlPars
+        Control system parameters.
+    T_s : float, optional
+        Sampling period (s). The default is 250e-6.
+
+    Attributes
+    ----------
+    w_m_ref : callable
+        Rotor speed reference (electrical rad/s).
+
+    References
+    ----------
+    .. [#Tii2022] Tiitinen, Hinkkanen, Kukkola, Routimo, Pellegrino, Harnefors, 
+       "Stable and passive observer-based V/Hz control for synchronous Motors," 
+       Proc. IEEE ECCE, Detroit, MI, Oct. 2022, 
+       https://doi.org/10.1109/ECCE50734.2022.9947858
 
     """
 
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
+    # pylint: disable=too-many-instance-attributes, too-many-arguments
+    def __init__(self, par, ctrl_par, T_s=250e-6):
         super().__init__()
-        self.T_s = pars.T_s
-        self.w_m_ref = pars.w_m_ref
-        self.sensorless = pars.sensorless
-        self.speed_ctrl = SpeedCtrl(pars)
-        self.pwm = PWM(pars)
-        if pars.sensorless:
-            self.observer = SensorlessObserver(pars)
-        else:
-            self.observer = Observer(pars)
-        self.flux_torque_ref = FluxTorqueRef(pars)
-        # Bandwidths
-        self.alpha_psi = pars.alpha_psi
-        self.alpha_tau = pars.alpha_tau
+        self.T_s = T_s
         # Motor parameter estimates
-        self.R_s = pars.R_s
-        self.L_d = pars.L_d
-        self.L_q = pars.L_q
-        self.n_p = pars.n_p
+        self.R_s = par.R_s
+        self.n_p = par.n_p
+        # Controller parameters
+        self.alpha_f = ctrl_par.alpha_f
+        self.alpha_psi = ctrl_par.alpha_psi
+        self.k_tau = ctrl_par.k_tau
+        # Subsystems
+        self.pwm = PWM()
+        self.flux_torque_ref = FluxTorqueReference(ctrl_par)
+        self.observer = FluxObserver(par)
+        self.rate_limiter = RateLimiter(np.inf)
+        self.w_m_ref = callable
+        # States
+        self.theta_s, self.tau_M_ref = 0, 0
 
+    # pylint: disable=too-many-locals
     def __call__(self, mdl):
         """
         Run the main control loop.
 
         Parameters
         ----------
-        mdl : SynchronousMotorDrive
-            Continuous-time model of a synchronous motor drive for getting the
-            feedback signals.
+        mdl : Drive
+            Continuous-time system model for getting the feedback signals.
 
         Returns
         -------
         T_s : float
-            Sampling period.
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
+            Sampling period (s).
+        d_abc : ndarray, shape (3,)
+            Duty ratios.
 
         """
         # Get the speed reference
-        w_m_ref = self.w_m_ref(self.t)
+        if self.rate_limiter is not None:
+            w_m_ref = self.rate_limiter(self.T_s, self.w_m_ref(self.clock.t))
+        else:
+            w_m_ref = self.w_m_ref(self.clock.t)
 
         # Feedback signals
-        i_s_abc = mdl.motor.meas_currents()  # Phase currents
-        u_dc = mdl.conv.meas_dc_voltage()  # DC-bus voltage
+        i_s_abc = mdl.machine.meas_currents()  # Phase currents
+        u_dc = mdl.converter.meas_dc_voltage()  # DC-bus voltage
         u_s = self.pwm.realized_voltage  # Realized voltage from PWM
 
-        if self.sensorless:
-            # Get the rotor speed and position estimates
-            w_m, theta_m = self.observer.w_m, self.observer.theta_m
-        else:
-            # Measure the rotor speed
-            w_m = self.n_p*mdl.mech.meas_speed()
-            # Limit the electrical rotor position into [-pi, pi)
-            theta_m = np.mod(
-                self.n_p*mdl.mech.meas_position() + np.pi, 2*np.pi) - np.pi
+        # Get the states
+        psi_s = self.observer.psi_s
+        theta_s = self.theta_s
 
-        # Current vector in estimated rotor coordinates
-        i_s = np.exp(-1j*theta_m)*abc2complex(i_s_abc)
+        # Space vector and coordinate transformation
+        i_s = np.exp(-1j*theta_s)*abc2complex(i_s_abc)
 
-        # Flux and torque estimates
-        psi_s = self.observer.psi_s
-        tau_M = 1.5*self.n_p*np.imag(i_s*np.conj(psi_s))
+        # Get the states
+        tau_M_ref = self.tau_M_ref
 
-        # Outputs
-        tau_M_ref = self.speed_ctrl.output(w_m_ref/self.n_p, w_m/self.n_p)
-        psi_s_ref, tau_M_ref_lim = self.flux_torque_ref(tau_M_ref, w_m, u_dc)
-
-        # Auxiliary current
-        i_a = psi_s.real/self.L_q + 1j*psi_s.imag/self.L_d - i_s
-
-        # Torque-production factor (c_tau = 0 corresponds to the MTPV condition)
-        c_tau = np.real(i_a*np.conj(psi_s))
-
-        # References for the flux and torque controllers
-        v_psi = self.alpha_psi*(psi_s_ref - np.abs(psi_s))
-        v_tau = self.alpha_tau*(tau_M_ref_lim - tau_M)
-        if c_tau > 0:
-            v = (np.abs(psi_s)*i_a*v_psi + 1j*psi_s*v_tau)/c_tau
-        else:
-            v = v_psi
+        # Limited flux and torque references
+        psi_s_ref, _ = self.flux_torque_ref(tau_M_ref, w_m_ref, u_dc)
 
-        # Stator voltage reference
-        u_s_ref = self.R_s*i_s + 1j*w_m*psi_s + v
+        # Electromagnetic torque
+        tau_M = 1.5*self.n_p*np.imag(i_s*np.conj(psi_s))
 
-        # PWM output
-        d_abc_ref, u_s_ref_lim = self.pwm.output(u_s_ref, u_dc, theta_m, w_m)
+        # Dynamic frequency
+        w_s = w_m_ref - self.k_tau*(tau_M - tau_M_ref)
+
+        # Voltage reference
+        err = psi_s_ref - psi_s
+        u_s_ref = self.R_s*i_s + 1j*w_s*psi_s_ref + self.alpha_psi*err
 
         # Data logging
         data = Bunch(
             i_s=i_s,
             psi_s=psi_s,
             psi_s_ref=psi_s_ref,
-            t=self.t,
-            tau_M_ref_lim=tau_M_ref_lim,
-            theta_m=theta_m,
+            t=self.clock.t,
+            theta_s=theta_s,
             u_dc=u_dc,
             u_s=u_s,
-            w_m=w_m,
             w_m_ref=w_m_ref,
+            w_s=w_s,
+            tau_M=tau_M,
         )
         self.save(data)
 
-        # Update states
-        self.observer.update(u_s, i_s, w_m)
-        self.speed_ctrl.update(tau_M_ref_lim)
-        self.pwm.update(u_s_ref_lim)
-        self.update_clock(self.T_s)
+        # Update the states
+        self.observer.update(self.T_s, u_s, i_s, w_s)
+        self.tau_M_ref += self.T_s*self.alpha_f*(tau_M - self.tau_M_ref)
+        self.theta_s += self.T_s*w_s  # Next line: limit into [-pi, pi)
+        self.theta_s = np.mod(self.theta_s + np.pi, 2*np.pi) - np.pi
+        self.clock.update(self.T_s)
+
+        # PWM output
+        d_abc = self.pwm(self.T_s, u_s_ref, u_dc, theta_s, w_s)
 
-        return self.T_s, d_abc_ref
+        return self.T_s, d_abc
 
 
 # %%
-class Observer:
+class FluxObserver:
     """
-    Sensored observer.
+    Sensorless stator flux observer.
+
+    The observer gain decouples the electrical and mechanical dynamics and 
+    allows placing the poles of the corresponding linearized estimation error 
+    dynamics. 
 
     Parameters
     ----------
-    pars : SynchronousMotoroFluxVectorCtrlPars
-        Control parameters.
+    par : ModelPars
+        Machine model parameters.
+    alpha_o : float, optional
+        Observer gain (rad/s). The default is 2*pi*20.
+    zeta_inf : float, optional
+        Damping ratio at infinite speed. The default is 0.2.
 
     """
 
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.R_s = pars.R_s
-        self.L_d = pars.L_d
-        self.L_q = pars.L_q
-        self.psi_f = pars.psi_f
-        self.g = pars.g
-        # Initial state
-        self.psi_s = pars.psi_f
+    # pylint: disable=too-many-instance-attributes
+    def __init__(self, par, alpha_o=2*np.pi*20, zeta_inf=.2):
+        self.R_s = par.R_s
+        self.L_d = par.L_d
+        self.L_q = par.L_q
+        self.psi_f = par.psi_f
+        self.alpha_o = alpha_o
+        self.b_p = .5*par.R_s*(par.L_d + par.L_q)/(par.L_d*par.L_q)
+        self.zeta_inf = zeta_inf
+        # Initial states
+        self.delta, self.psi_s = 0, par.psi_f
 
-    def update(self, u_s, i_s, w_m):
+    def update(self, T_s, u_s, i_s, w_s):
         """
         Update the states for the next sampling period.
 
         Parameters
         ----------
+        T_s : float
+            Sampling period (s).
         u_s : complex
-            Stator voltage in estimated rotor coordinates.
+            Stator voltage (V).
         i_s : complex
-            Stator current in estimated rotor coordinates.
-        w_m : float
-            Rotor speed (in electrical rad/s).
+            Stator current (A).
+        w_s : float
+            Stator angular frequency (rad/s).
 
         """
-        # Estimation error
-        e = self.L_d*i_s.real + 1j*self.L_q*i_s.imag + self.psi_f - self.psi_s
+        # Transformations to rotor coordinates. This is mathematically
+        # equivalent to the version in [Tii2022].
+        i_sr = i_s*np.exp(1j*self.delta)
+        psi_sr = self.psi_s*np.exp(1j*self.delta)
+
+        # Auxiliary flux and estimation error in rotor coordinates
+        psi_ar = self.psi_f + (self.L_d - self.L_q)*np.conj(i_sr)
+        e_r = self.L_d*i_sr.real + 1j*self.L_q*i_sr.imag + self.psi_f - psi_sr
+
+        # Auxiliary flux in controller coordinates
+        psi_a = np.exp(-1j*self.delta)*psi_ar
+
+        k = self.b_p + 2*self.zeta_inf*np.abs(w_s)
+
+        if np.abs(psi_ar) > 0:
+            # Correction voltage in controller coordinates
+            v = k*psi_a*np.real(e_r/psi_ar)
+            # Error signal
+            w_delta = self.alpha_o*np.imag(e_r/psi_ar)
+        else:
+            v, w_delta = 0, 0
 
-        # Update the state
-        self.psi_s += self.T_s*(
-            u_s - self.R_s*i_s - 1j*w_m*self.psi_s + self.g*e)
+        # Update the states
+        self.psi_s += T_s*(u_s - self.R_s*i_s - 1j*w_s*self.psi_s + v)
+        self.delta += T_s*w_delta
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `motulator-0.1.4/motulator/control/sm_obs_vhz.py` & `motulator-0.1.5/motulator/control/sm/_flux_vector.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,313 +1,294 @@
-"""
-Observer-based V/Hz control for synchronous motor drives.
+"""Flux-vector control of synchronous machine drives."""
 
-This method is based on [1]_.
-
-References
-----------
-.. [1] Tiitinen, Hinkkanen, Kukkola, Routimo, Pellegrino, Harnefors, "Stable
-    and passive observer-based V/Hz control for synchronous Motors," Proc.
-    IEEE ECCE, Detroit, MI, Oct. 2022.
-
-"""
-
-from typing import Callable
-from dataclasses import dataclass, field
+from dataclasses import dataclass, InitVar
 import numpy as np
-from motulator.helpers import abc2complex, Bunch
-from motulator.control.common import Ctrl, PWM, RateLimiter
-from motulator.control.sm_torque import TorqueCharacteristics
+from motulator._helpers import abc2complex
+from motulator.control._common import Ctrl, PWM, SpeedCtrl
+from motulator.control.sm._torque import TorqueCharacteristics
+from motulator.control.sm._vector import Observer, ModelPars
+from motulator._utils import Bunch
 
 
 # %%
-@dataclass
-class SynchronousMotorVHzObsCtrlPars:
-    """Control parameters."""
+class FluxVectorCtrl(Ctrl):
+    """
+    Flux-vector control of synchronous machine drives.
 
-    # pylint: disable=too-many-instance-attributes
-    # Speed reference (in electrical rad/s)
-    w_m_ref: Callable[[float], float] = field(
-        repr=False, default=lambda t: (t > .2)*(2*np.pi*75))
-
-    # Control
-    T_s: float = 250e-6
-    psi_s_max: float = None
-    psi_s_min: float = None
-    rate_limit: float = np.inf
-    i_s_max: float = 1.5*np.sqrt(2)*5
-    alpha_psi: float = 2*np.pi*50
-    alpha_tau: float = 2*np.pi*50
-    alpha_f: float = 2*np.pi*1
-    k_u: float = 1
-
-    # Observer
-    alpha_o: float = 2*np.pi*20
-    zeta_inf: float = .2
-
-    # Motor parameter estimates
-    R_s: float = 3.6
-    L_d: float = .036
-    L_q: float = .051
-    psi_f: float = .545
-    n_p: int = 3
+    This class implements a variant of stator-flux-vector control [#Pel2009]_. 
+    Rotor coordinates as well as decoupling between the stator flux and torque 
+    channels are used according to [#Awa2019]_. Here, the stator flux magnitude 
+    and the electromagnetic torque are selected as controllable variables. 
+
+    Notes
+    -----
+    Proportional controllers are used for simplicity. The magnetic saturation is 
+    not considered in this implementation.
 
+    Parameters
+    ----------
+    par : ModelPars
+        Machine model parameters.
+    ref : FluxTorqueReferencePars
+        Reference generation parameters.
+    alpha_psi : float, optional
+        Bandwidth of the flux controller (rad/s). The default is 2*pi*100.
+    alpha_tau : float, optional
+        Bandwidth of the torque controller (rad/s). The default is 2*pi*200.
+    T_s : float
+        Sampling period (s). The default is 250e-6.
+    sensorless : bool, optional
+        If True, sensorless control is used. The default is True.
 
-# %%
-class SynchronousMotorVHzObsCtrl(Ctrl):
-    """
-    Observer-based V/Hz control for synchronous motors.
+    Attributes
+    ----------
+    observer : Observer
+        Flux observer, having both sensorless and sensored modes.
+    flux_torque_ref : FluxTorqueReference
+        Flux and torque reference generator.
+    speed_ctrl : SpeedCtrl
+        Speed controller.
+    w_m_ref : float
+        Speed reference (electrical rad/s) as a function of time (s).
+    pwm : PWM
+        Pulse-width modulation.
 
-    Parameters
+    References
     ----------
-    pars : SynchronousMotorVHzObsCtrlPars
-        Control parameters.
+    .. [#Pel2009] Pellegrino, Armando, Guglielmi, “Direct flux field-oriented 
+       control of IPM drives with variable DC link in the field-weakening 
+       region,” IEEE Trans.Ind. Appl., 2009, 
+       https://doi.org/10.1109/TIA.2009.2027167
+
+    .. [#Awa2019] Awan, Hinkkanen, Bojoi, Pellegrino, "Stator-flux-oriented 
+       control of synchronous motors: A systematic design procedure," IEEE Trans. 
+       Ind. Appl., 2019, https://doi.org/10.1109/TIA.2019.2927316
 
     """
 
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
+    # pylint: disable=too-many-instance-attributes, too-many-arguments
+    def __init__(
+            self,
+            par,
+            ref,
+            alpha_psi=2*np.pi*100,
+            alpha_tau=2*np.pi*200,
+            T_s=250e-6,
+            sensorless=True):
         super().__init__()
-        # Instantiate classes
-        self.observer = SensorlessFluxObserver(pars)
-        self.pwm = PWM(pars)
-        self.rate_limiter = RateLimiter(pars)
-        self.flux_torque_ref = FluxTorqueRef(pars)
-        # Reference
-        self.w_m_ref = pars.w_m_ref
-        # Motor parameters
-        self.R_s = pars.R_s
-        self.n_p = pars.n_p
-        # Controller parameters
-        self.T_s = pars.T_s
-        self.alpha_f = pars.alpha_f
-        self.alpha_psi = pars.alpha_psi
-        # Gain k_tau
-        G = (pars.L_d - pars.L_q)/(pars.L_d*pars.L_q)
-        psi_s0 = pars.psi_f if pars.psi_f > 0 else pars.psi_s_min
-        if pars.psi_f > 0:  # PMSM or PM-SyRM
-            c_delta0 = 1.5*pars.n_p*(pars.psi_f*psi_s0/pars.L_d - G*psi_s0**2)
-        else:  # SyRM
-            c_delta0 = 1.5*pars.n_p*G*psi_s0**2
-        self.k_tau = pars.alpha_tau/c_delta0
-        # Initial states
-        self.theta_s, self.tau_M_ref = 0, 0
+        self.T_s = T_s
+        self.sensorless = sensorless
+        # Machine model parameters
+        self.n_p = par.n_p
+        self.R_s, self.L_d, self.L_q = par.R_s, par.L_d, par.L_q
+        # Subsystems
+        self.observer = Observer(
+            par, alpha_o=2*np.pi*100, sensorless=sensorless)
+        self.flux_torque_ref = FluxTorqueReference(ref)
+        self.pwm = PWM()
+        self.speed_ctrl = SpeedCtrl(par.J, 2*np.pi*4)
+        # Bandwidths
+        self.alpha_psi = alpha_psi
+        self.alpha_tau = alpha_tau
+        # Speed reference
+        self.w_m_ref = callable
 
+    # pylint: disable=too-many-locals
     def __call__(self, mdl):
         """
         Run the main control loop.
 
         Parameters
         ----------
-        mdl : SynchronousMotorDrive
-            Continuous-time model of a synchronous motor drive for getting the
-            feedback signals.
+        mdl : Drive
+            Continuous-time system model for getting the feedback signals.
 
         Returns
         -------
         T_s : float
-            Sampling period.
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
+            Sampling period (s).
+        d_abc : ndarray, shape (3,)
+            Duty ratios.
 
         """
         # Get the speed reference
-        w_m_ref = self.rate_limiter(self.w_m_ref(self.t))
+        w_m_ref = self.w_m_ref(self.clock.t)
 
-        # Measure the feedback signals
-        i_s_abc = mdl.motor.meas_currents()  # Phase currents
-        u_dc = mdl.conv.meas_dc_voltage()  # DC-bus voltage
+        # Feedback signals
+        i_s_abc = mdl.machine.meas_currents()  # Phase currents
+        u_dc = mdl.converter.meas_dc_voltage()  # DC-bus voltage
+        u_s = self.pwm.realized_voltage  # Realized voltage from PWM
+        #
+        if self.sensorless:
+            # Get the rotor speed and position estimates
+            w_m, theta_m = self.observer.w_m, self.observer.theta_m
+        else:
+            # Measure the rotor speed
+            w_m = self.n_p*mdl.mechanics.meas_speed()
+            # Limit the electrical rotor position into [-pi, pi)
+            theta_m = np.mod(
+                self.n_p*mdl.mechanics.meas_position() + np.pi,
+                2*np.pi) - np.pi
 
-        # Space vector and coordinate transformation
-        i_s = np.exp(-1j*self.theta_s)*abc2complex(i_s_abc)
+        # Current vector in estimated rotor coordinates
+        i_s = np.exp(-1j*theta_m)*abc2complex(i_s_abc)
 
-        # Get the states
-        u_s = self.pwm.realized_voltage
+        # Flux and torque estimates
         psi_s = self.observer.psi_s
-        tau_M_ref = self.tau_M_ref
-
-        # Limited flux and torque references
-        psi_s_ref, _ = self.flux_torque_ref(tau_M_ref, w_m_ref, u_dc)
-
-        # Electromagnetic torque (7d)
         tau_M = 1.5*self.n_p*np.imag(i_s*np.conj(psi_s))
 
-        # Dynamic frequency (5a)
-        w_s = w_m_ref - self.k_tau*(tau_M - tau_M_ref)
+        # Outputs
+        tau_M_ref = self.speed_ctrl.output(w_m_ref/self.n_p, w_m/self.n_p)
+        psi_s_ref, tau_M_ref_lim = self.flux_torque_ref(tau_M_ref, w_m, u_dc)
+
+        # Auxiliary current
+        i_a = psi_s.real/self.L_q + 1j*psi_s.imag/self.L_d - i_s
+
+        # Torque-production factor (c_tau = 0 corresponds to the MTPV condition)
+        c_tau = 1.5*self.n_p*np.real(i_a*np.conj(psi_s))
+
+        # References for the flux and torque controllers
+        v_psi = self.alpha_psi*(psi_s_ref - np.abs(psi_s))
+        v_tau = self.alpha_tau*(tau_M_ref_lim - tau_M)
+        if c_tau > 0:
+            v = (1.5*self.n_p*np.abs(psi_s)*i_a*v_psi + 1j*psi_s*v_tau)/c_tau
+        else:
+            v = v_psi
 
-        # Voltage reference (4)
-        err = psi_s_ref - psi_s
-        u_s_ref = self.R_s*i_s + 1j*w_s*psi_s_ref + self.alpha_psi*err
-
-        # Duty ratios
-        d_abc_ref, u_s_ref_lim = self.pwm.output(
-            u_s_ref, u_dc, self.theta_s, w_s)
+        # Stator voltage reference
+        u_s_ref = self.R_s*i_s + 1j*w_m*psi_s + v
 
         # Data logging
         data = Bunch(
             i_s=i_s,
             psi_s=psi_s,
             psi_s_ref=psi_s_ref,
-            t=self.t,
-            theta_s=self.theta_s,
+            t=self.clock.t,
+            tau_M_ref_lim=tau_M_ref_lim,
+            theta_m=theta_m,
             u_dc=u_dc,
             u_s=u_s,
+            w_m=w_m,
             w_m_ref=w_m_ref,
-            w_s=w_s,
-            tau_M=tau_M,
         )
         self.save(data)
 
-        # Update the states
-        self.pwm.update(u_s_ref_lim)
-        self.observer.update(u_s, i_s, w_s)
-        self.tau_M_ref += self.T_s*self.alpha_f*(tau_M - self.tau_M_ref)
-        self.theta_s += self.T_s*w_s  # Next line: limit into [-pi, pi)
-        self.theta_s = np.mod(self.theta_s + np.pi, 2*np.pi) - np.pi
-        self.update_clock(self.T_s)
+        # Update states
+        self.observer.update(self.T_s, u_s, i_s, w_m)
+        self.speed_ctrl.update(self.T_s, tau_M_ref_lim)
+        self.clock.update(self.T_s)
+
+        # PWM output
+        d_abc = self.pwm(self.T_s, u_s_ref, u_dc, theta_m, w_m)
+
+        return self.T_s, d_abc
+
+
+# %%
+@dataclass
+class FluxTorqueReferencePars:
+    """
+    Parameters for reference generation.
+
+    Parameters
+    ----------
+    par : ModelPars
+        Machine model parameters.
+    i_s_max : float
+        Maximum stator current (A). 
+    psi_s_min : float, optional
+        Minimum stator flux (Vs). The default is `psi_f`.
+    psi_s_max : float, optional
+        Maximum stator flux (Vs). The default is inf.
+    k_u : float, optional
+        Voltage utilization factor. The default is 0.95.
+
+    Attributes
+    ----------
+    psi_s_mtpa : callable
+        MTPA stator flux linkage (Vs) as a function of the torque (Nm).
+    tau_M_lim : callable
+        Torque limit (Nm) as a function of the stator flux linkage (Vs). This 
+        limit merges the MTPV and current limits. 
+
+    """
+    par: InitVar[ModelPars]
+    i_s_max: float = None
+    psi_s_min: float = None
+    psi_s_max: float = np.inf
+    k_u: float = 0.95
 
-        return self.T_s, d_abc_ref
+    def __post_init__(self, par):
+        self.psi_s_min = par.psi_f if self.psi_s_min is None else self.psi_s_min
+        # Generate LUTs
+        tq = TorqueCharacteristics(par)
+        mtpa = tq.mtpa_locus(self.i_s_max, self.psi_s_min)
+        lim = tq.mtpv_and_current_limits(self.i_s_max)
+        # MTPA locus
+        self.psi_s_mtpa = mtpa.abs_psi_s_vs_tau_M
+        # Merged MTPV and current limits
+        self.tau_M_lim = lim.tau_M_vs_abs_psi_s
 
 
 # %%
-class FluxTorqueRef:
+class FluxTorqueReference:
     """
     Flux and torque references.
 
+    The current and MTPV limits as well as the MTPA locus are implemented as
+    look-up tables, which are generated based on the constant machine model
+    parameters.
+
     Parameters
     ----------
-    pars : SynchronousMotorVHzObsCtrlPars
-        Control parameters.
+    ref : FluxTorqueReferencePars
+        Reference generation parameters.
 
     """
 
-    def __init__(self, pars):
-        self.psi_s_min = (
-            pars.psi_f if pars.psi_s_min is None else pars.psi_s_min)
-        self.psi_s_max = np.inf if pars.psi_s_max is None else pars.psi_s_max
-        self.k_u = pars.k_u
+    # pylint: disable=too-many-arguments
+    def __init__(self, ref):
+        self.psi_s_min, self.psi_s_max = ref.psi_s_min, ref.psi_s_max
+        self.k_u = ref.k_u
         # Merged MTPV and current limits
-        tq = TorqueCharacteristics(pars)
-        lims = tq.mtpv_and_current_limits(i_s_max=pars.i_s_max)
-        self.tau_M_lim = lims.tau_M_vs_abs_psi_s
+        self.tau_M_lim = ref.tau_M_lim
         # MTPA locus
-        mtpa = tq.mtpa_locus(i_s_max=pars.i_s_max)
-        self.psi_s_mtpa = mtpa.abs_psi_s_vs_tau_M
+        self.psi_s_mtpa = ref.psi_s_mtpa
 
     def __call__(self, tau_M_ref, w_m, u_dc):
         """
         Calculate the stator flux reference and limit the torque reference.
 
         Parameters
         ----------
         tau_M_ref : float
-            Unlimited torque reference.
+            Unlimited torque reference (Nm).
         w_m : float
-            Rotor speed or its reference (in electrical rad/s).
+            Rotor speed or its reference (electrical rad/s).
         u_dc : float
-            DC-bus voltage.
+            DC-bus voltage (V).
 
         Returns
         -------
         psi_s_ref : float
-            Stator flux reference.
+            Stator flux reference (Vs).
         tau_M_ref_lim : float
-            Limited torque reference.
+            Limited torque reference (Nm).
 
         """
         # Get the MTPA flux
         psi_s_mtpa = self.psi_s_mtpa(np.abs(tau_M_ref))
-        np.clip(psi_s_mtpa, self.psi_s_min, self.psi_s_max, out=psi_s_mtpa)
+        psi_s_mtpa = np.clip(psi_s_mtpa, self.psi_s_min, self.psi_s_max)
 
         # Field weakening
         u_s_max = self.k_u*u_dc/np.sqrt(3)
         psi_s_max = u_s_max/np.abs(w_m) if np.abs(w_m) > 0 else np.inf
 
         # Flux reference
         psi_s_ref = np.min([psi_s_max, psi_s_mtpa])
 
         # Limit the torque reference according to the MTPV and current limits
         tau_M_lim = self.tau_M_lim(psi_s_ref)
         tau_M_ref_lim = np.min([tau_M_lim, np.abs(tau_M_ref)
                                 ])*np.sign(tau_M_ref)
 
         return psi_s_ref, tau_M_ref_lim
-
-
-# %%
-class SensorlessFluxObserver:
-    """
-    Sensorless stator flux observer.
-
-    This observer is a variant of [1]_. The observer gain decouples the
-    electrical and mechanical dynamics and allows placing the poles of the
-    corresponding linearized estimation error dynamics. For simplicity, the
-    current model is here implemented in rotor coordinates, however this is
-    mathematically equivalent to controller coordinates implementation in [2]_.
-
-    Parameters
-    ----------
-    pars : SynchronousMotorObsVHzCtrlPars
-        Control parameters.
-
-    References
-    ----------
-    .. [1] Hinkkanen, Saarakkala, Awan, Mölsä, Tuovinen, "Observers for
-        sensorless synchronous motor drives: Framework for design and
-        analysis," IEEE Trans. Ind. Appl., 2018,
-        https://doi.org/10.1109/TIA.2018.2858753
-    .. [2] Tiitinen, Hinkkanen, Kukkola, Routimo, Pellegrino, Harnefors,
-        "Stable and passive observer-based V/Hz control for synchronous
-        Motors," Proc. IEEE ECCE, Detroit, MI, Oct. 2022.
-
-    """
-
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.R_s = pars.R_s
-        self.L_d = pars.L_d
-        self.L_q = pars.L_q
-        self.psi_f = pars.psi_f
-        self.alpha_o = pars.alpha_o
-        self.b_p = .5*pars.R_s*(pars.L_d + pars.L_q)/(pars.L_d*pars.L_q)
-        self.zeta_inf = pars.zeta_inf
-        # Initial states
-        self.delta, self.psi_s = 0, pars.psi_f
-
-    def update(self, u_s, i_s, w_s):
-        """
-        Update the states for the next sampling period.
-
-        Parameters
-        ----------
-        u_s : complex
-            Stator voltage.
-        i_s : complex
-            Stator current.
-        w_s : float
-            Stator angular frequency.
-
-        """
-        # Transformations to rotor coordinates
-        i_sr = i_s*np.exp(1j*self.delta)
-        psi_sr = self.psi_s*np.exp(1j*self.delta)
-
-        # Auxiliary flux and estimation error in rotor coordinates
-        psi_ar = self.psi_f + (self.L_d - self.L_q)*np.conj(i_sr)
-        e_r = self.L_d*i_sr.real + 1j*self.L_q*i_sr.imag + self.psi_f - psi_sr
-
-        # Auxiliary flux in controller coordinates
-        psi_a = np.exp(-1j*self.delta)*psi_ar
-
-        g_o = self.b_p + 2*self.zeta_inf*np.abs(w_s)
-
-        if np.abs(psi_ar) > 0:
-            # Correction voltage in controller coordinates
-            v = g_o*psi_a*np.real(e_r/psi_ar)
-            # Error signal
-            w_delta = self.alpha_o*np.imag(e_r/psi_ar)
-        else:
-            v, w_delta = 0, 0
-
-        # Update the states
-        self.psi_s += self.T_s*(u_s - self.R_s*i_s - 1j*w_s*self.psi_s + v)
-        self.delta += self.T_s*w_delta
```

### Comparing `motulator-0.1.4/motulator/control/sm_torque.py` & `motulator-0.1.5/motulator/control/sm/_torque.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,134 +1,127 @@
 """
 Torque characteristics for synchronous machines.
 
-This contains computation and plotting of torque characteristics for
-synchronous machines, including the MTPA and MTPV loci [1]_. The methods can be
-used to define look-up tables for control and to analyze the characteristics.
-In this version, the magnetic saturation is omitted.
+This contains computation and plotting of torque characteristics for synchronous 
+machines, including the MTPA and MTPV loci [#Mor1990]_. The methods can be used 
+to define look-up tables for control and to analyze the characteristics. This 
+version omits the magnetic saturation.
 
 References
 ----------
-.. [1] Morimoto, Takeda, Hirasa, Taniguchi, "Expansion of operating limits for
-   permanent magnet motor by current vector control considering inverter
-   capacity," IEEE Trans. Ind. Appl., 1990,
+.. [#Mor1990] Morimoto, Takeda, Hirasa, Taniguchi, "Expansion of operating 
+   limits for permanent magnet motor by current vector control considering 
+   inverter capacity," IEEE Trans. Ind. Appl., 1990,
    https://doi.org/10.1109/28.60058
 
 """
+
 from sys import float_info
 import numpy as np
 from scipy.interpolate import interp1d
 import matplotlib.pyplot as plt
 from cycler import cycler
-from motulator.helpers import Bunch
+from motulator._utils import Bunch
 
 plt.rcParams['axes.prop_cycle'] = cycler(color='brgcmyk')
 plt.rcParams['lines.linewidth'] = 1.
 plt.rcParams.update({"text.usetex": False})  # Disable LaTeX in plots
 
 
 # %%
 class TorqueCharacteristics:
     """
-    Compute MTPA and MTPV loci based on the motor parameters.
+    Compute MTPA and MTPV loci based on the machine parameters.
 
     The magnetic saturation is omitted.
 
     Parameters
     ----------
-    pars : data object
-        Motor parameters.
+    par : ModelPars
+        Machine model parameters.
 
     """
 
-    def __init__(self, pars):
-        self.n_p = pars.n_p
-        self.L_d = pars.L_d
-        self.L_q = pars.L_q
-        self.psi_f = pars.psi_f
-        try:
-            self.psi_s_min = pars.psi_s_min
-        except AttributeError:
-            self.psi_s_min = None
-        try:
-            self.psi_s_max = pars.psi_s_max
-        except AttributeError:
-            self.psi_s_max = None
+    def __init__(self, par):
+        self.n_p = par.n_p
+        self.L_d = par.L_d
+        self.L_q = par.L_q
+        self.psi_f = par.psi_f
 
     def torque(self, psi_s):
         """
         Compute the torque as a function of the stator flux linkage.
 
         Parameters
         ----------
         psi_s : complex
-            Stator flux.
+            Stator flux (Vs).
 
         Returns
         -------
         tau_M : float
-            Electromagnetic torque.
+            Electromagnetic torque (Nm).
 
         """
         i_s = self.current(psi_s)
         tau_M = 1.5*self.n_p*np.imag(i_s*np.conj(psi_s))
 
         return tau_M
 
     def current(self, psi_s):
         """
         Compute the stator current as a function of the stator flux linkage.
 
         Parameters
         ----------
         psi_s : complex
-            Stator flux linkage.
+            Stator flux linkage (Vs).
 
         Returns
         -------
         i_s : complex
-            Stator current.
+            Stator current (A).
 
         """
         i_s = (psi_s.real - self.psi_f)/self.L_d + 1j*psi_s.imag/self.L_q
 
         return i_s
 
     def flux(self, i_s):
         """
         Compute the stator flux linkage as a function of the current.
 
         Parameters
         ----------
         i_s : complex
-            Stator current.
+            Stator current (A).
 
         Returns
         -------
         psi_s : complex
-            Stator flux linkage.
+            Stator flux linkage (Vs).
 
         """
         psi_s = self.L_d*i_s.real + self.psi_f + 1j*self.L_q*i_s.imag
 
         return psi_s
 
     def mtpa(self, abs_i_s):
         """
         Compute the MTPA stator current angle.
 
         Parameters
         ----------
         abs_i_s : float
-            Stator current magnitude.
+            Stator current magnitude (A).
 
         Returns
         -------
         beta : float
-            MTPA angle of the stator current vector.
+            MTPA angle of the stator current vector (electrical rad).
 
         """
         # Replace zeros with epsilon
         abs_i_s = (abs_i_s > 0)*abs_i_s + (abs_i_s <= 0)*float_info.epsilon
 
         if self.psi_f == 0:
             # SyRM (d-axis aligned with the maximum inductance)
@@ -150,20 +143,20 @@
     def mtpv(self, abs_psi_s):
         """
         Compute the MTPV stator flux angle.
 
         Parameters
         ----------
         abs_psi_s : float
-            Stator flux magnitude.
+            Stator flux magnitude (Vs).
 
         Returns
         -------
         delta : float
-            MTPV angle of the stator flux vector.
+            MTPV angle of the stator flux vector (electrical rad).
 
         """
         # Replace zeros with epsilon
         abs_psi_s = ((abs_psi_s > 0)*abs_psi_s +
                      (abs_psi_s <= 0)*float_info.epsilon)
 
         if self.psi_f == 0:
@@ -193,20 +186,20 @@
         It is used here to "cut" the MTPV characteristics at the desired
         current. Alternatively just a large enough maximum flux magnitude could
         be used.
 
         Parameters
         ----------
         abs_i_s : float
-            Stator current magnitude.
+            Stator current magnitude (A).
 
         Returns
         -------
         i_s : complex
-            MTPV stator current.
+            MTPV stator current (A).
 
         """
         if self.psi_f == 0:
             # SyRM
             i_s = abs_i_s*np.exp(1j*(np.arctan(self.L_d/self.L_q)))
         elif self.psi_f/self.L_d < abs_i_s:
             if self.L_d == self.L_q:
@@ -228,101 +221,103 @@
                 i_s = i_sd + 1j*i_sq
         else:
             # No MTPV for the given current magnitude
             i_s = np.nan
 
         return i_s
 
-    def mtpa_locus(self, i_s_max=1, N=20):
+    def mtpa_locus(self, i_s_max, psi_s_min=None, N=20):
         """
         Compute the MTPA locus.
 
         Parameters
         ----------
-        i_s_max : float, optional
-            Maximum stator current magnitude at which the locus is computed.
-            The default is 1.
+        i_s_max : float
+            Maximum stator current magnitude (A) at which the locus is computed.
+        psi_s_min : float, optional
+            Minimum stator flux magnitude (Vs) at which the locus is computed.
         N : int, optional
             Amount of points. The default is 20.
 
         Returns
         -------
         Bunch object with the following fields defined:
         psi_s : complex
-            Stator flux.
+            Stator flux (Vs).
         i_s : complex
-            Stator current.
+            Stator current (A).
         tau_M : float
-            Electromagnetic torque.
-        abs_psi_s_vs_tau_M : interp1d object
-            Stator flux magnitude as a function of the torque.
-        i_sd_vs_tau_M : interp1d object
-            d-axis current as a function of the torque.
+            Electromagnetic torque (Nm).
+        abs_psi_s_vs_tau_M : callable
+            Stator flux magnitude (Vs) as a function of the torque (Nm).
+        i_sd_vs_tau_M : callable
+            d-axis current (A) as a function of the torque (Nm).
 
         """
         # Current  magnitudes
         abs_i_s = np.linspace(0, i_s_max, N)
 
         # MTPA locus expressed with different quantities
         beta = self.mtpa(abs_i_s)
         i_s = abs_i_s*np.exp(1j*beta)
 
-        if (self.psi_s_min is not None) and (self.psi_f == 0):
+        if (psi_s_min is not None) and (self.psi_f == 0):
             # Minimum d-axis current for sensorless SyRM drives
-            i_sd_min = self.psi_s_min/self.L_d
+            i_sd_min = psi_s_min/self.L_d
             i_s.real = ((i_s.real < i_sd_min)*i_sd_min +
                         (i_s.real >= i_sd_min)*i_s.real)
 
         psi_s = self.flux(i_s)
+        abs_psi_s = np.abs(psi_s)
         tau_M = self.torque(psi_s)
 
         # Create an interpolant that can be used as a look-up table. If needed,
         # more interpolants can be easily added.
         abs_psi_s_vs_tau_M = interp1d(
-            tau_M, np.abs(psi_s), fill_value='extrapolate')
-        i_sd_vs_tau_M = interp1d(tau_M, i_s.real, fill_value='extrapolate')
+            tau_M, abs_psi_s, fill_value=abs_psi_s[-1], bounds_error=False)
+        i_sd_vs_tau_M = interp1d(
+            tau_M, i_s.real, fill_value=i_s.real[-1], bounds_error=False)
 
         # Return the result as a bunch object
         return Bunch(
             psi_s=psi_s,
             i_s=i_s,
             tau_M=tau_M,
             abs_psi_s_vs_tau_M=abs_psi_s_vs_tau_M,
             i_sd_vs_tau_M=i_sd_vs_tau_M)
 
-    def mtpv_locus(self, psi_s_max=1, i_s_max=None, N=20):
+    def mtpv_locus(self, psi_s_max=None, i_s_max=None, N=20):
         """
         Compute the MTPV locus.
 
         Parameters
         ----------
         psi_s_max : float, optional
-            Maximum stator flux magnitude at which the locus is computed. The
-            default is 1.
+            Maximum stator flux magnitude (Vs) at which the locus is computed. 
+            Either `psi_s_max` or `i_s_max` must be given.
         i_s_max : float, optional
-            Maximum stator current magnitude at which the locus is computed.
-            The default is None.
+            Maximum stator current magnitude (A) at which the locus is computed.
         N : int, optional
             Amount of points. The default is 20.
 
         Returns
         -------
         Bunch object with the following fields defined:
         psi_s : complex
-            Stator flux.
+            Stator flux (Vs).
         i_s : complex
-            Stator current.
+            Stator current (A).
         tau_M : float
-            Electromagnetic torque.
+            Electromagnetic torque (Nm).
         tau_M_vs_abs_psi_s : interp1d object
-            Torque as a function of the flux magnitude.
+            Torque (Nm) as a function of the flux magnitude (Vs).
 
         """
         # If i_s_max is given, compute the corresponding MTPV stator flux
-        if i_s_max:
+        if i_s_max is not None:
             i_s_mtpv = self.mtpv_current(i_s_max)
             psi_s_max = np.abs(self.flux(i_s_mtpv))
 
         # Flux magnitudes
         abs_psi_s = np.linspace(0, psi_s_max, N)
 
         # MTPV locus expressed with different quantities
@@ -338,40 +333,40 @@
         # Return the result as a bunch object
         return Bunch(
             psi_s=psi_s,
             i_s=i_s,
             tau_M=tau_M,
             tau_M_vs_abs_psi_s=tau_M_vs_abs_psi_s)
 
-    def current_limit(self, i_s_max=1, gamma1=np.pi, gamma2=0, N=20):
+    def current_limit(self, i_s_max, gamma1=np.pi, gamma2=0, N=20):
         """
         Compute the current limit.
 
         Parameters
         ----------
-        i_s_max : float, optional
-            Current limit. The default is 1.
+        i_s_max : float
+            Current limit (A). 
         gamma1 : float, optional
-            Starting angle in radians. The default is 0.
+            Starting angle (electrical rad). The default is 0.
         gamma2 : float, optional
-            End angle in radians. The defauls in np.pi.
+            End angle (electrical rad). The defauls in pi.
         N : int, optional
             Amount of points. The default is 20.
 
         Returns
         -------
         Bunch object with the following fields defined:
         psi_s : complex
-            Stator flux.
+            Stator flux (Vs).
         i_s : complex
-            Stator current.
+            Stator current (A).
         tau_M : float
-            Electromagnetic torque.
+            Electromagnetic torque (Nm).
         tau_M_vs_abs_psi_s : interp1d object
-            Torque as a function of the flux magnitude.
+            Torque (Nm) as a function of the flux magnitude (Vs).
 
         """
         if np.isnan(gamma1):
             # No MTPV
             gamma1 = np.pi
 
         gamma = np.linspace(gamma1, gamma2, N)
@@ -392,32 +387,32 @@
         # Return the result as a bunch object
         return Bunch(
             psi_s=psi_s,
             i_s=i_s,
             tau_M=tau_M,
             tau_M_vs_abs_psi_s=tau_M_vs_abs_psi_s)
 
-    def mtpv_and_current_limits(self, i_s_max=1, N=20):
+    def mtpv_and_current_limits(self, i_s_max, N=20):
         """
         Merge the MTPV and current limits into a single interpolant.
 
         Parameters
         ----------
-        i_s_max : float, optional
-            Current limit. The default is 1.
+        i_s_max : float
+            Current limit (A).
         N : int, optional
             Amount of points. The default is 20.
 
         Returns
         -------
         Bunch object with the following fields defined:
         tau_M_vs_abs_psi_s : interp1d object
-            Torque as a function of the flux magnitude.
+            Torque (Nm) as a function of the flux magnitude (Vs).
         i_sd_vs_tau_M : interp1d object
-            d-axis current as a function of the torque.
+            d-axis current (A) as a function of the torque (Nm).
 
         """
         mtpa = self.mtpa_locus(i_s_max=i_s_max, N=N)
         mtpv = self.mtpv_locus(i_s_max=i_s_max, N=N)
         clim = self.current_limit(
             i_s_max=i_s_max,
             N=N,
@@ -452,16 +447,16 @@
         Plot the stator flux linkage loci.
 
         Per-unit quantities are used.
 
         Parameters
         ----------
         i_s_max : float
-            Maximum current at which the loci are evaluated.
-        base : object
+            Maximum current (A) at which the loci are evaluated.
+        base : BaseValues
             Base values.
         N : int, optional
             Amount of points to be evaluated. The default is 20.
 
         """
         # Compute the characteristics
         mtpa = self.mtpa_locus(i_s_max=i_s_max, N=N)
@@ -499,16 +494,16 @@
         Plot the current loci.
 
         Per-unit quantities are used.
 
         Parameters
         ----------
         i_s_max : float
-            Maximum current at which the loci are evaluated.
-        base : object
+            Maximum current (A) at which the loci are evaluated.
+        base : BaseValues
             Base values.
         N : int, optional
             Amount of points to be evaluated. The default is 20.
 
         """
         # Compute the characteristics
         mtpa = self.mtpa_locus(i_s_max=i_s_max, N=N)
@@ -545,16 +540,16 @@
         Plot torque vs. current characteristics.
 
         Per-unit quantities are used.
 
         Parameters
         ----------
         i_s_max : float
-            Maximum current at which the loci are evaluated.
-        base : object
+            Maximum current (A) at which the loci are evaluated.
+        base : BaseValues
             Base values.
         N : int, optional
             Amount of points to be evaluated. The default is 20.
 
         """
         # Compute the characteristics
         mtpa = self.mtpa_locus(i_s_max=i_s_max, N=N)
@@ -601,16 +596,16 @@
         Plot torque vs. flux magnitude characteristics.
 
         Per-unit quantities are used.
 
         Parameters
         ----------
         i_s_max : float
-            Maximum current at which the loci are evaluated.
-        base : object
+            Maximum current (A) at which the loci are evaluated.
+        base : BaseValues
             Base values.
         N : int, optional
             Amount of points to be evaluated. The default is 20.
 
         """
         # Compute the characteristics
         mtpa = self.mtpa_locus(i_s_max=i_s_max, N=N)
```

### Comparing `motulator-0.1.4/motulator/control/sm_vector.py` & `motulator-0.1.5/motulator/control/sm/_vector.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,315 +1,337 @@
-"""Current vector control for synchronous motor drives."""
+"""Current vector control methods for synchronous machine drives."""
 
-from typing import Callable
-from dataclasses import dataclass, field
+from dataclasses import dataclass, InitVar
 import numpy as np
-from motulator.helpers import abc2complex, Bunch
-from motulator.control.common import Ctrl, SpeedCtrl, PWM
-from motulator.control.sm_torque import TorqueCharacteristics
+from motulator._helpers import abc2complex
+from motulator.control._common import Ctrl, ComplexPICtrl, PWM, SpeedCtrl
+from motulator.control.sm._torque import TorqueCharacteristics
+from motulator._utils import Bunch
 
 
 # %%
 @dataclass
-class SynchronousMotorVectorCtrlPars:
-    """Vector control parameters for synchronous motors."""
+class ModelPars:
+    """
+    Model parameters of a synchronous machine.
+    
+    Parameters
+    ----------
+    R_s : float
+        Stator resistance (Ω).
+    L_d : float
+        d-axis inductance (H).
+    L_q : float
+        q-axis inductance (H).
+    psi_f : float
+        PM flux linkage (Vs).
+    n_p : int
+        Number of pole pairs.
+    J : float
+        Moment of inertia (kgm²).
 
-    # pylint: disable=too-many-instance-attributes
-    # Speed reference (in electrical rad/s)
-    w_m_ref: Callable[[float], float] = field(
-        repr=False, default=lambda t: (t > .2)*(2*np.pi*75))
-    # Mode
-    sensorless: bool = True
-    # Sampling period
-    T_s: float = 250e-6
-    # Bandwidths
-    alpha_c: float = 2*np.pi*200
-    alpha_fw: float = 2*np.pi*20
-    alpha_s: float = 2*np.pi*4
-    # Maximum values
-    tau_M_max: float = 2*14
-    i_s_max: float = 1.5*np.sqrt(2)*5
-    psi_s_min: float = None
-    # Voltage margin
-    k_u: float = .95
-    # Nominal values
-    w_nom: float = 2*np.pi*75
-    # Motor parameter estimates
-    R_s: float = 3.6
-    L_d: float = .036
-    L_q: float = .051
-    psi_f: float = .545
-    n_p: int = 3
-    J: float = .015
-    # Sensorless observer
-    w_o: float = 2*np.pi*40  # Used only in the sensorless mode
-    zeta_inf: float = .2
+    """
+    R_s: float = None
+    L_d: float = None
+    L_q: float = None
+    psi_f: float = None
+    n_p: int = None
+    J: float = None
 
 
 # %%
-class SynchronousMotorVectorCtrl(Ctrl):
+class VectorCtrl(Ctrl):
     """
-    Vector control for a synchronous motor drive.
+    Vector control for synchronous machine drives.
 
     This class interconnects the subsystems of the control system and
     provides the interface to the solver.
 
     Parameters
     ----------
-    pars : SynchronousMotorVectorCtrlPars
-        Control parameters.
+    par : ModelPars
+        Machine model parameters.
+    ref : ReferencePars
+        Reference generation parameters.
+    T_s : float, optional
+        Sampling period (s). The default is 250e-6.
+    sensorless : bool, optional
+        If True, sensorless control is used. The default is True.
 
+    Attributes
+    ----------
+    current_ref : CurrentReference
+        Current reference generator.
+    observer : Observer
+        Flux and rotor position observer, used in the sensorless mode only.
+    current_ctrl : CurrentCtrl
+        Current controller.
+    speed_ctrl : SpeedCtrl 
+        Speed controller.
+    pwm : PWM
+        Pulse-width modulation.
+    w_m_ref : callable
+        Speed reference (electrical rad/s) as a function of time (s).
+        
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
+    def __init__(self, par, ref, T_s=250e-6, sensorless=True):
         super().__init__()
-        self.T_s = pars.T_s
-        self.w_m_ref = pars.w_m_ref
-        self.n_p = pars.n_p
-        self.sensorless = pars.sensorless
-        self.current_ctrl = CurrentCtrl(pars)
-        self.speed_ctrl = SpeedCtrl(pars)
-        self.current_ref = CurrentRef(pars)
-        self.pwm = PWM(pars)
-        if pars.sensorless:
-            self.observer = SensorlessObserver(pars)
+        self.T_s = T_s
+        self.sensorless = sensorless
+        self.n_p = par.n_p
+        self.current_ref = CurrentReference(par, ref)
+        self.current_ctrl = CurrentCtrl(par, 2*np.pi*200)
+        if sensorless:
+            self.observer = Observer(par, alpha_o=2*np.pi*100, sensorless=True)
         else:
             self.observer = None
+        self.speed_ctrl = SpeedCtrl(par.J, 2*np.pi*4)
+        self.pwm = PWM()
+        self.w_m_ref = callable
 
+    # pylint: disable=too-many-locals
     def __call__(self, mdl):
         """
         Run the main control loop.
 
         Parameters
         ----------
-        mdl : SynchronousMotorDrive
-            Continuous-time model of a synchronous motor drive for getting the
-            feedback signals.
+        mdl : Drive
+            Continuous-time system model for getting the feedback signals.
 
         Returns
         -------
         T_s : float
-            Sampling period.
-        d_abc_ref : ndarray, shape (3,)
-            Duty ratio references.
+            Sampling period (s).
+        d_abc : ndarray, shape (3,)
+            Duty ratios.
 
         """
         # Get the speed reference
-        w_m_ref = self.w_m_ref(self.t)
+        w_m_ref = self.w_m_ref(self.clock.t)
 
         # Measure the feedback signals
-        i_s_abc = mdl.motor.meas_currents()  # Phase currents
-        u_dc = mdl.conv.meas_dc_voltage()  # DC-bus voltage
+        i_s_abc = mdl.machine.meas_currents()
+        u_dc = mdl.converter.meas_dc_voltage()
+        u_s = self.pwm.realized_voltage
 
-        if not self.sensorless:
-            # Measure the rotor speed
-            w_m = self.n_p*mdl.mech.meas_speed()
-            # Limit the electrical rotor position into [-pi, pi)
-            theta_m = np.mod(
-                self.n_p*mdl.mech.meas_position() + np.pi, 2*np.pi) - np.pi
-        else:
-            # Get the rotor speed and position estimates
+        # Get the states
+        if self.sensorless:
             w_m, theta_m = self.observer.w_m, self.observer.theta_m
-
-        # Get the realized voltage from the PWM method
-        u_s = self.pwm.realized_voltage
+        else:
+            w_m = self.n_p*mdl.mechanics.meas_speed()
+            theta_m = self.n_p*mdl.mechanics.meas_position()
+            theta_m = np.mod(theta_m + np.pi, 2*np.pi) - np.pi
 
         # Current vector in estimated rotor coordinates
         i_s = np.exp(-1j*theta_m)*abc2complex(i_s_abc)
 
         # Outputs
         tau_M_ref = self.speed_ctrl.output(w_m_ref/self.n_p, w_m/self.n_p)
         i_s_ref, tau_M_ref_lim = self.current_ref.output(tau_M_ref, w_m, u_dc)
         u_s_ref = self.current_ctrl.output(i_s_ref, i_s)
-        d_abc_ref, u_s_ref_lim = self.pwm.output(u_s_ref, u_dc, theta_m, w_m)
 
         # Data logging
         data = Bunch(
             i_s=i_s,
             i_s_ref=i_s_ref,
-            t=self.t,
+            t=self.clock.t,
             tau_M_ref_lim=tau_M_ref_lim,
             theta_m=theta_m,
             u_dc=u_dc,
             u_s=u_s,
             w_m=w_m,
             w_m_ref=w_m_ref,
         )
         self.save(data)
 
         # Update states
         if self.sensorless:
-            self.observer.update(u_s, i_s)
-        self.speed_ctrl.update(tau_M_ref_lim)
-        self.current_ref.update(tau_M_ref_lim, u_s_ref, u_dc)
-        self.current_ctrl.update(u_s_ref_lim, w_m)
-        self.pwm.update(u_s_ref_lim)
-        self.update_clock(self.T_s)
+            self.observer.update(self.T_s, u_s, i_s)
+        self.speed_ctrl.update(self.T_s, tau_M_ref_lim)
+        self.current_ref.update(self.T_s, tau_M_ref_lim, u_s_ref, u_dc)
+        self.current_ctrl.update(self.T_s, u_s, w_m)
+        self.clock.update(self.T_s)
+
+        d_abc = self.pwm(self.T_s, u_s_ref, u_dc, theta_m, w_m)
 
-        return self.T_s, d_abc_ref
+        return self.T_s, d_abc
 
 
 # %%
-class CurrentCtrl:
+class CurrentCtrl(ComplexPICtrl):
     """
-    2DOF PI current controller.
+    Current controller for synchronous machines.
 
-    This controller corresponds to [1]_. The continuous-time complex-vector
-    design corresponding to (13) is used here. This design could be
-    equivalently presented as a 2DOF PI controller.
+    This provides an interface of a current controller for synchronous machines
+    [#Awa2019]_. The gains are initialized based on the desired closed-loop 
+    bandwidth and the inductances. 
 
     Parameters
     ----------
-    pars : SynchronousMotorVectorCtrlPars (or its subset)
-        Control parameters.
-
-    Notes
-    -----
-    For better performance at high speeds with low sampling frequencies, the
-    discrete-time design in (18) is recommended. This implementation does not
-    take the magnetic saturation into account.
+    par : ModelPars
+        Synchronous machine parameters, should contain `L_d` and `L_q` (H). 
+    alpha_c : float
+        Closed-loop bandwidth (rad/s).
 
     References
     ----------
-    .. [1] Awan, Saarakkala, Hinkkanen, "Flux-linkage-based current control of
-       saturated synchronous motors," IEEE Trans. Ind. Appl. 2019,
+    .. [#Awa2019] Awan, Saarakkala, Hinkkanen, "Flux-linkage-based current 
+       control of saturated synchronous motors," IEEE Trans. Ind. Appl. 2019,
        https://doi.org/10.1109/TIA.2019.2919258
 
     """
 
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.L_d = pars.L_d
-        self.L_q = pars.L_q
-        self.alpha_c = pars.alpha_c
-        # Integral state
-        self.u_i = 0
-        # Memory for the update method
-        self.e = 0
-        self.u_s_ref = 0
-
-    def output(self, i_s_ref, i_s):
-        """
-        Compute the unlimited voltage reference.
-
-        Parameters
-        ----------
-        i_s_ref : complex
-            Current reference.
-        i_s : complex
-            Measured current.
-
-        Returns
-        -------
-        u_s_ref : complex
-            Unlimited voltage reference.
-
-        """
-        # Gains
-        k_t = self.alpha_c
-        k = 2*self.alpha_c
-        # PM-flux linkage cancels out
-        psi_s_ref = self.L_d*i_s_ref.real + 1j*self.L_q*i_s_ref.imag
-        psi_s = self.L_d*i_s.real + 1j*self.L_q*i_s.imag
-        self.u_s_ref = k_t*psi_s_ref - k*psi_s + self.u_i
-        # Error signal (scaled, corresponds to the stator flux linkage).
-        self.e = psi_s_ref - psi_s
+    def __init__(self, par, alpha_c):
+        k_p, k_i, k_t = 2*alpha_c, alpha_c**2, alpha_c
+        super().__init__(k_p, k_i, k_t)
+        self.L_d = par.L_d
+        self.L_q = par.L_q
+
+    def output(self, i_ref, i):
+        # Extends the base class method by transforming the currents to the
+        # flux linkages, which is a simple way to take the saliency into account
+        psi_ref = self.L_d*i_ref.real + 1j*self.L_q*i_ref.imag
+        psi = self.L_d*i.real + 1j*self.L_q*i.imag
+        return super().output(psi_ref, psi)
 
-        return self.u_s_ref
 
-    def update(self, u_s_ref_lim, w_m):
-        """
-        Update the integral state.
+# %%
+# pylint: disable=too-many-instance-attributes
+@dataclass
+class CurrentReferencePars:
+    """
+    Parameters for reference generation.
 
-        Parameters
-        ----------
-        u_s_ref_lim : complex
-            Limited voltage reference.
-        w_m : float
-            Angular rotor speed.
+    Parameters
+    ----------
+    par : ModelPars
+        Machine model parameters.
+    i_s_max : float
+        Maximum stator current (A). 
+    psi_s_min : float, optional
+        Minimum stator flux (Vs). The default is `psi_f`.
+    w_m_nom : float, optional
+        Nominal rotor angular speed (electrical rad/s). Needed if `k_fw` is not
+        directly provided.
+    alpha_fw : float, optional
+        Field-weakening bandwidth (rad/s). The default is 2*pi*20.
+    k_fw : float, optional
+        Field-weakening gain. The default is `alpha_fw/(w_m_nom*par.L_d)`.
+    k_u : float, optional
+        Voltage utilization factor. The default is 0.95.
 
-        """
-        k_t = self.alpha_c
-        k_i = self.alpha_c*(self.alpha_c + 1j*w_m)
-        self.u_i += self.T_s*k_i*(self.e + (u_s_ref_lim - self.u_s_ref)/k_t)
+    Attributes
+    ----------
+    i_sd_mtpa : callable
+        MTPA d-axis current (A) as a funtion of the torque (Nm).
+    tau_M_lim : callable
+        Torque limite (Nm) as a function of the stator flux linkage (Vs). This
+        limit merges the MTPV and current limits.
+    i_sd_lim : callable
+        d-axis current limit (A) as a function of the stator flux linkage (Vs).
+        This limit merges the MTPV and current limits.
+    
+    """
+    par: InitVar[ModelPars]
+    i_s_max: float
+    psi_s_min: float = None
+    w_m_nom: InitVar[float] = None
+    alpha_fw: InitVar[float] = 2*np.pi*20
+    k_fw: float = None
+    k_u: float = 0.95
+
+    def __post_init__(self, par, w_m_nom, alpha_fw):
+        # Minimum stator flux
+        if self.psi_s_min is None:
+            self.psi_s_min = par.psi_f
+        # Field-weakening gain
+        if self.k_fw is None:
+            self.k_fw = alpha_fw/(w_m_nom*par.L_d)
+        # Generate LUTs
+        tq = TorqueCharacteristics(par)
+        mtpa = tq.mtpa_locus(self.i_s_max, self.psi_s_min)
+        lim = tq.mtpv_and_current_limits(self.i_s_max)
+        # MTPA locus
+        self.i_sd_mtpa = mtpa.i_sd_vs_tau_M
+        # Merged MTPV and current limits
+        self.tau_M_lim = lim.tau_M_vs_abs_psi_s
+        self.i_sd_lim = lim.i_sd_vs_tau_M
 
 
 # %%
-class CurrentRef:
+class CurrentReference:
     """
     Current reference calculation.
 
-    This method includes the MTPA locus and field-weakenting operation based on
+    This method includes the MTPA locus and field-weakening operation based on
     the unlimited voltage reference feedback. The MTPV and current limits are
-    taken into account. This resembles the method presented [2]_.
+    taken into account. This resembles the method presented [#Bed2020]_.
 
     Parameters
     ----------
-    pars : SynchronousMotorVectorCtrlPars (or its subset)
-        Control parameters.
+    par : ModelPars
+        Machine model parameters.
+    ref : CurrentReferencePars
+        Reference generation parameters.
 
     Notes
     -----
-    Instead of the PI controller used in [2]_, we use a simpler integral
+    Instead of the PI controller used in [#Bed2020]_, we use a simpler integral
     controller with a constant gain. The resulting operating-point-dependent
-    closed-loop pole could be derived using (12) of the paper. Unlike in [2]_,
-    the MTPV limit is also included here by means of limiting the reference
-    torque and the d-axis current reference.
+    closed-loop pole could be derived using (12) of the paper. Unlike in 
+    [#Bed2020]_, the MTPV limit is also included here by means of limiting the 
+    reference torque and the d-axis current reference.
 
     References
     ----------
-    .. [2] Bedetti, Calligaro, Petrella, "Analytical design and autotuning of
-       adaptive flux-weakening voltage regulation loop in IPMSM drives with
-       accurate torque regulation," IEEE Trans. Ind. Appl., 2020,
+    .. [#Bed2020] Bedetti, Calligaro, Petrella, "Analytical design and 
+       autotuning of adaptive flux-weakening voltage regulation loop in IPMSM 
+       drives with accurate torque regulation," IEEE Trans. Ind. Appl., 2020,
        https://doi.org/10.1109/TIA.2019.2942807
 
     """
 
-    # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.i_s_max = pars.i_s_max
-        self.n_p = pars.n_p
-        self.L_d = pars.L_d
-        self.L_q = pars.L_q
-        self.psi_f = pars.psi_f
-        self.k = pars.alpha_fw/(pars.w_nom*self.L_d)
-        self.k_u = pars.k_u
-        # Generate LUTs
-        tq = TorqueCharacteristics(pars)
-        mtpa = tq.mtpa_locus(i_s_max=pars.i_s_max)
-        lims = tq.mtpv_and_current_limits(i_s_max=pars.i_s_max)
-        # MTPA locus
-        self.i_sd_mtpa = mtpa.i_sd_vs_tau_M
-        # Merged MTPV and current limits
-        self.tau_M_lim = lims.tau_M_vs_abs_psi_s
-        self.i_sd_lim = lims.i_sd_vs_tau_M
-        # Initial value
+    # pylint: disable=too-many-instance-attributes, too-many-arguments
+    def __init__(self, par, ref):
+        # Machine model parameters
+        self.n_p = par.n_p
+        self.L_d, self.L_q, self.psi_f = par.L_d, par.L_q, par.psi_f
+        # Reference generation parameters
+        self.i_sd_mtpa = ref.i_sd_mtpa  # MTPA locus
+        self.tau_M_lim = ref.tau_M_lim  # Merged MTPV and current limits
+        self.i_sd_lim = ref.i_sd_lim  # Merged MTPV and current limits
+        self.psi_s_min = ref.psi_s_min  # Minimum flux linkage
+        self.i_s_max = ref.i_s_max  # Maximum current
+        self.k_fw = ref.k_fw  # Field-weakening gain
+        self.k_u = ref.k_u  # Voltage utilization factor
+        # State
         self.i_sd_ref = 0
 
     def output(self, tau_M_ref, w_m, u_dc):
         """
         Compute the stator current reference.
 
         Parameters
         ----------
         tau_M_ref : float
-            Torque reference.
+            Torque reference (Nm).
         w_m : float
-            Rotor speed (in electrical rad/s)
+            Rotor speed (electrical rad/s)
         u_dc : float
-            DC-bus voltage.
+            DC-bus voltage (V).
 
         Returns
         -------
         i_s_ref : complex
-            Stator current reference.
+            Stator current reference (A).
         tau_M_ref_lim : float
-            Limited torque reference.
+            Limited torque reference (Nm).
 
         """
 
         def limit_torque(tau_M_ref, w_m, u_dc):
             if np.abs(w_m) > 0:
                 psi_s_max = self.k_u*u_dc/np.sqrt(3)/np.abs(w_m)
                 tau_M_max = self.tau_M_lim(psi_s_max)
@@ -341,108 +363,135 @@
         i_s_ref = self.i_sd_ref + 1j*i_sq_ref
 
         # Limited torque (for the speed controller)
         tau_M_ref_lim = 1.5*self.n_p*psi_t*i_sq_ref
 
         return i_s_ref, tau_M_ref_lim
 
-    def update(self, tau_M_ref_lim, u_s_ref, u_dc):
+    def update(self, T_s, tau_M_ref_lim, u_s_ref, u_dc):
         """
         Field-weakening based on the unlimited reference voltage.
 
         Parameters
         ----------
+        T_s : float
+            Sampling period (s).
         tau_M_ref_lim : float
-            Limited torque reference.
+            Limited torque reference (Nm).
         u_s_ref : complex
-            Unlimited stator voltage reference.
-        u_dc : DC-bus voltage.
-            float.
+            Unlimited stator voltage reference (V).
+        u_dc : float 
+            DC-bus voltage (V).
 
         """
         u_s_max = self.k_u*u_dc/np.sqrt(3)
-        self.i_sd_ref += self.T_s*self.k*(u_s_max - np.abs(u_s_ref))
+        self.i_sd_ref += T_s*self.k_fw*(u_s_max - np.abs(u_s_ref))
 
         # Limit the current
         i_sd_mtpa = self.i_sd_mtpa(np.abs(tau_M_ref_lim))
         i_sd_lim = self.i_sd_lim(np.abs(tau_M_ref_lim))
-
-        if self.i_sd_ref > i_sd_mtpa:
-            self.i_sd_ref = i_sd_mtpa
-        elif self.i_sd_ref < i_sd_lim:
-            self.i_sd_ref = i_sd_lim
+        self.i_sd_ref = np.clip(self.i_sd_ref, i_sd_lim, i_sd_mtpa)
 
 
 # %%
-class SensorlessObserver:
+class Observer:
     """
-    Sensorless observer.
+    Observer for synchronous machines.
 
-    This observer corresponds to [3]_. The observer gain decouples the
-    electrical and mechanical dynamics and allows placing the poles of the
-    corresponding linearized estimation error dynamics. This implementation
-    operates in estimated rotor coordinates.
+    This observer estimates the rotor angle, the rotor speed, and the stator 
+    flux linkage. The design is based on [#Hin2018]_. The observer gain 
+    decouples the electrical and mechanical dynamics and allows placing the 
+    poles of the corresponding linearized estimation error dynamics. This 
+    implementation operates in estimated rotor coordinates. The observer can 
+    also be used in the sensored mode by providing the measured rotor speed as 
+    an input.
 
     Parameters
     ----------
-    pars : SynchronousMotorVectorCtrlPars (or its subset)
-        Control parameters.
+    par : ModelPars
+        Machine model parameters.
+    alpha_o : float, optional
+        Observer bandwidth (electrical rad/s). The default is 2*pi*40.
+    k : callable, optional
+        Observer gain as a function of the rotor angular speed. The default is 
+        ``lambda w_m: 0.25*(R_s*(L_d + L_q)/(L_d*L_q) + 0.2*abs(w_m))`` if
+        `sensorless` else ``lambda w_m: 2*pi*15``.
+
+    Attributes
+    ----------
+    theta_m : float
+        Rotor angle estimate (electrical rad).
+    w_m : float
+        Rotor speed estimate (electrical rad/s).
+    psi_s : complex
+        Stator flux estimate (Vs).
 
     References
     ----------
-    .. [3] Hinkkanen, Saarakkala, Awan, Mölsä, Tuovinen, "Observers for
+    .. [#Hin2018] Hinkkanen, Saarakkala, Awan, Mölsä, Tuovinen, "Observers for
        sensorless synchronous motor drives: Framework for design and analysis,"
        IEEE Trans. Ind. Appl., 2018, https://doi.org/10.1109/TIA.2018.2858753
 
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(self, pars):
-        self.T_s = pars.T_s
-        self.R_s = pars.R_s
-        self.L_d = pars.L_d
-        self.L_q = pars.L_q
-        self.psi_f = pars.psi_f
-        self.k_p = 2*pars.w_o
-        self.k_i = pars.w_o**2
-        self.b_p = .5*pars.R_s*(pars.L_d + pars.L_q)/(pars.L_d*pars.L_q)
-        self.zeta_inf = pars.zeta_inf
+    def __init__(self, par, alpha_o=2*np.pi*40, k=None, sensorless=True):
+        self.R_s = par.R_s
+        self.L_d, self.L_q, self.psi_f = par.L_d, par.L_q, par.psi_f
+        self.psi_f = par.psi_f
+        self.alpha_o = alpha_o
+        self.sensorless = sensorless
+        self.k1 = k
+        if self.sensorless:
+            if self.k1 is None:  # If not given, use the default gains
+                sigma0 = .25*par.R_s*(par.L_d + par.L_q)/(par.L_d*par.L_q)
+                self.k1 = lambda w_m: (sigma0 + .2*np.abs(w_m))
+            self.k2 = self.k1
+        else:
+            if self.k1 is None:
+                self.k1 = lambda w_m: 2*np.pi*15
+            self.k2 = 0*self.k1
         # Initial states
-        self.theta_m, self.w_m, self.psi_s = 0, 0, pars.psi_f
+        self.theta_m, self.w_m, self.psi_s = 0, 0, par.psi_f
 
-    def update(self, u_s, i_s, *_):
+    def update(self, T_s, u_s, i_s, w_m=None):
         """
         Update the states for the next sampling period.
 
         Parameters
         ----------
+        T_s : float
+            Sampling period (s).
         u_s : complex
-            Stator voltage in estimated rotor coordinates.
+            Stator voltage (V) in estimated rotor coordinates.
         i_s : complex
-            Stator current in estimated rotor coordinates.
+            Stator current (A) in estimated rotor coordinates.
+        w_m : float, optional
+            Rotor angular speed (electrical rad/s). Needed only in the sensored
+            mode. The default is None. 
 
         """
-        # Auxiliary flux (12)
-        psi_a = self.psi_f + (self.L_d - self.L_q)*np.conj(i_s)
-
-        # Estimation error (6)
+        # Estimation error
         e = self.L_d*i_s.real + 1j*self.L_q*i_s.imag + self.psi_f - self.psi_s
 
-        # Pole locations are chosen according to (36), with c = w_m**2
-        # and w_inf = inf, and the gain corresponding to (30) is used
-        k = self.b_p + 2*self.zeta_inf*np.abs(self.w_m)
-        if np.abs(psi_a) > 0:
-            # Correction voltage
-            v = k*psi_a*np.real(e/psi_a)
-            # Error signal (10)
-            eps = -np.imag(e/psi_a)
-        else:
-            v, eps = 0, 0
+        if self.sensorless:
+            # Auxiliary flux
+            psi_a = self.psi_f + (self.L_d - self.L_q)*np.conj(i_s)
 
-        # Speed estimation (9)
-        w_m = self.k_p*eps + self.w_m
+            # Observer gains
+            k1 = self.k1(self.w_m)
+            k2 = k1*psi_a/np.conj(psi_a) if np.abs(psi_a) > 0 else k1
+
+            # Speed estimation
+            eps = -np.imag(e/psi_a) if np.abs(psi_a) > 0 else 0
+            w_s = 2*self.alpha_o*eps + self.w_m
+        else:
+            k1, k2 = self.k1, 0
+            w_s = w_m
+            eps = 0
 
         # Update the states
-        self.psi_s += self.T_s*(u_s - self.R_s*i_s - 1j*w_m*self.psi_s + v)
-        self.w_m += self.T_s*self.k_i*eps
-        self.theta_m += self.T_s*w_m  # Next line: limit into [-pi, pi)
+        self.psi_s += T_s*(
+            u_s - self.R_s*i_s - 1j*w_s*self.psi_s + k1*e + k2*np.conj(e))
+        self.w_m += T_s*self.alpha_o**2*eps
+        self.theta_m += T_s*w_s  # Next line: limit into [-pi, pi)
         self.theta_m = np.mod(self.theta_m + np.pi, 2*np.pi) - np.pi
```

### Comparing `motulator-0.1.4/motulator/model/converter.py` & `motulator-0.1.5/motulator/model/_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 """
 Power converter models.
 
 An inverter with constant DC-bus voltage and a frequency converter with a diode
 front-end rectifier are modeled. Complex space vectors are used also for duty
 ratios and switching states, wherever applicable. In this module, all space
-vectors are in stationary coordinates. The default values correspond to a
-2.2-kW 400-V motor drive.
+vectors are in stationary coordinates. 
 
 """
 import numpy as np
 
 
 # %%
 class Inverter:
     """
     Inverter with constant DC-bus voltage and switching-cycle averaging.
 
     Parameters
     ----------
     u_dc : float
-        DC-bus voltage.
+        DC-bus voltage (V).
 
     """
 
-    def __init__(self, u_dc=540):
+    def __init__(self, u_dc):
         self.u_dc0 = u_dc
         self.q = 0j  # Switching state vector
 
     @staticmethod
     def ac_voltage(q, u_dc):
         """
         Compute the AC-side voltage of a lossless inverter.
 
         Parameters
         ----------
         q : complex
             Switching state vector.
         u_dc : float
-            DC-bus voltage.
+            DC-bus voltage (V).
 
         Returns
         -------
         u_ac : complex
-            AC-side voltage.
+            AC-side voltage (V).
 
         """
         u_ac = q*u_dc
         return u_ac
 
     @staticmethod
     def dc_current(q, i_ac):
@@ -54,33 +53,33 @@
         Compute the DC-side current of a lossless inverter.
 
         Parameters
         ----------
         q : complex
             Switching state vector.
         i_ac : complex
-            AC-side current.
+            AC-side current (A).
 
         Returns
         -------
         i_dc : float
-            DC-side current.
+            DC-side current (A).
 
         """
         i_dc = 1.5*np.real(q*np.conj(i_ac))
         return i_dc
 
     def meas_dc_voltage(self):
         """
         Measure the DC-bus voltage.
 
         Returns
         -------
         float
-            DC-bus voltage.
+            DC-bus voltage (V).
 
         """
         return self.u_dc0
 
 
 # %%
 class FrequencyConverter(Inverter):
@@ -90,25 +89,25 @@
     This extends the Inverter class with models for a strong grid, a
     three-phase diode-bridge rectifier, an LC filter, and a three-phase
     inverter.
 
     Parameters
     ----------
     L : float
-        DC-bus inductance.
+        DC-bus inductance (H).
     C : float
-        DC-bus capacitance.
+        DC-bus capacitance (F).
     U_g : float
-        Grid voltage (line-line, rms).
+        Grid voltage (V, line-line, rms).
     f_g : float
-        Grid frequency.
+        Grid frequency (Hz).
 
     """
 
-    def __init__(self, L=2e-3, C=235e-6, U_g=400, f_g=50):
+    def __init__(self, L, C, U_g, f_g):
         # pylint: disable=super-init-not-called
         self.L, self.C = L, C
         # Initial value of the DC-bus inductor current
         self.i_L0 = 0
         # Initial value of the DC-bus voltage
         self.u_dc0 = np.sqrt(2)*U_g
         # Peak-valued line-neutral grid voltage
@@ -121,20 +120,20 @@
     def grid_voltages(self, t):
         """
         Compute three-phase grid voltages.
 
         Parameters
         ----------
         t : float
-            Time.
+            Time (s).
 
         Returns
         -------
         u_g_abc : ndarray of floats, shape (3,)
-            The phase voltages.
+            Phase voltages (V).
 
         """
         theta_g = self.w_g*t
         u_g_abc = self.u_g*np.array([
             np.cos(theta_g),
             np.cos(theta_g - 2*np.pi/3),
             np.cos(theta_g - 4*np.pi/3)
@@ -144,26 +143,26 @@
     def f(self, t, u_dc, i_L, i_dc):
         """
         Compute the state derivatives.
 
         Parameters
         ----------
         t : float
-            Time.
+            Time (s).
         u_dc : float
-            DC-bus voltage over the capacitor.
+            DC-bus voltage (V) over the capacitor.
         i_L : float
-            DC-bus inductor current.
+            DC-bus inductor current (A).
         i_dc : float
-            Current to the inverter.
+            Current to the inverter (A).
 
         Returns
         -------
         list, length 2
-            Time derivative of the state vector, [du_dc, d_iL]
+            Time derivative of the state vector, [du_dc, di_L]
 
         """
         # Grid phase voltages
         u_g_abc = self.grid_voltages(t)
         # Output voltage of the diode bridge
         u_di = np.amax(u_g_abc, axis=0) - np.amin(u_g_abc, axis=0)
         # State derivatives
```

### Comparing `motulator-0.1.4/motulator/model/im_drive.py` & `motulator-0.1.5/motulator/model/sm/_drive.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,284 +1,366 @@
 """
-Continuous-time models for induction motor drives.
+Continuous-time models for synchronous motor drives.
 
-Peak-valued complex space vectors are used. The space vector models are
-implemented in stator coordinates. The default values correspond to a 2.2-kW
-induction motor.
+Peak-valued complex space vectors are used.
 
 """
 import numpy as np
+from motulator._helpers import complex2abc
+from motulator._utils import Bunch
 
-from motulator.helpers import abc2complex, Bunch
+
+# %%
+class SynchronousMachine:
+    """
+    Synchronous machine model.
+
+    This models a synchronous machine in rotor coordinates. The stator flux 
+    linkage and the electrical angle of the rotor are the state variables. 
+
+    Parameters
+    ----------
+    n_p : int
+        Number of pole pairs.
+    R_s : float
+        Stator resistance (Ω).
+    L_d : float
+        d-axis inductance (H).
+    L_q : float
+        q-axis inductance (H).
+    psi_f : float
+        PM-flux linkage (Vs).
+
+    """
+
+    def __init__(self, n_p, R_s, L_d, L_q, psi_f):
+        # pylint: disable=too-many-arguments
+        self.n_p, self.R_s = n_p, R_s
+        self.L_d, self.L_q, self.psi_f = L_d, L_q, psi_f
+        # Initial values
+        self.psi_s0 = complex(psi_f)
+        self.theta_m0 = 0
+
+    def current(self, psi_s):
+        """
+        Compute the stator current.
+
+        Parameters
+        ----------
+        psi_s : complex
+            Stator flux linkage (Vs).
+
+        Returns
+        -------
+        i_s : complex
+            Stator current (A).
+
+        """
+        i_s = (psi_s.real - self.psi_f)/self.L_d + 1j*psi_s.imag/self.L_q
+        return i_s
+
+    def magnetic(self, psi_s):
+        """
+        Magnetic model.
+
+        Parameters
+        ----------
+        psi_s : complex
+            Stator flux linkage (Vs).
+
+        Returns
+        -------
+        i_s : complex
+            Stator current (A).
+        tau_M : float
+            Electromagnetic torque (Nm).
+
+        """
+        i_s = self.current(psi_s)
+        tau_M = 1.5*self.n_p*np.imag(i_s*np.conj(psi_s))
+        return i_s, tau_M
+
+    def f(self, psi_s, u_s, w_M):
+        """
+        Compute the state derivative.
+
+        Parameters
+        ----------
+        psi_s : complex
+            Stator flux linkage (Vs).
+        u_s : complex
+            Stator voltage (V).
+        w_M : float
+            Rotor angular speed (mechanical rad/s).
+
+        Returns
+        -------
+        complex list, length 2
+            Time derivative of the state vector, [dpsi_s, dtheta_m0]
+        i_s : complex
+            Stator current (A).
+        tau_M : float
+            Electromagnetic torque (Nm).
+
+        Notes
+        -----
+        In addition to the state derivative, this method also returns the 
+        output signals (stator current `i_ss` and torque `tau_M`) needed for 
+        interconnection with other subsystems. This avoids overlapping 
+        computation in simulation.
+
+        """
+        i_s, tau_M = self.magnetic(psi_s)
+        dpsi_s = u_s - self.R_s*i_s - 1j*self.n_p*w_M*psi_s
+        dtheta_m = self.n_p*w_M
+        return [dpsi_s, dtheta_m], i_s, tau_M
+
+    def meas_currents(self):
+        """
+        Measure the phase currents at the end of the sampling period.
+
+        Returns
+        -------
+        i_s_abc : 3-tuple of floats
+            Phase currents (A).
+
+        """
+        i_s0 = self.current(self.psi_s0)
+        i_s_abc = complex2abc(np.exp(1j*self.theta_m0)*i_s0)
+        return i_s_abc
+
+
+# %%
+class SynchronousMachineSaturated(SynchronousMachine):
+    """
+    Model of a saturated synchronous machine.
+
+    This overrides the linear magnetics model of the SynchronousMachine class
+    with a generic saturation model::
+
+        i_s = i_s(psi_s)
+        
+    The saturation model could be an analytical function or a look-up table. 
+
+    Parameters
+    ----------
+    n_p : int
+        Number of pole pairs.
+    R_s : float
+        Stator resistance (Ω).
+    current : callable
+        Function that computes the stator current `i_s` as a function of the 
+        stator flux linkage `psi_s`. 
+    psi_s0 : complex, optional
+        Initial value of the stator flux linkage (Vs). For PM machines, this 
+        should be solved from the the saturation model. The default is 0j. 
+
+    """
+
+    def __init__(self, n_p, R_s, current, psi_s0=0j):
+        # pylint: disable=super-init-not-called
+        self.n_p, self.R_s = n_p, R_s
+        self.current = current
+        # Initial values
+        self.psi_s0 = complex(psi_s0)
+        self.theta_m0 = 0
 
 
 # %%
-class InductionMotorDrive:
+class Drive:
     """
-    Continuous-time model for an induction motor drive.
+    Continuous-time model for a synchronous machine drive.
 
-    This interconnects the subsystems of an induction motor drive and provides
-    an interface to the solver. More complicated systems could be modeled using
-    a similar template.
+    This interconnects the subsystems of a synchronous machine drive and 
+    provides an interface to the solver. More complicated systems could be 
+    modeled using a similar template.
 
     Parameters
     ----------
-    motor : InductionMotor | InductionMotorSaturated
-        Induction motor model.
-    mech : Mechanics
+    machine : SynchronousMachine
+        Synchronous machine model.
+    mechanics : Mechanics
         Mechanics model.
-    conv : Inverter
+    converter : Inverter
         Inverter model.
 
     """
 
-    def __init__(self, motor=None, mech=None, conv=None):
-        self.motor = motor
-        self.mech = mech
-        self.conv = conv
-        self.t0 = 0  # Initial time
+    def __init__(self, machine=None, mechanics=None, converter=None):
+        self.machine = machine
+        self.mechanics = mechanics
+        self.converter = converter
+
+        # Initial time
+        self.t0 = 0
+
         # Store the solution in these lists
-        self.data = Bunch()  # Stores the solution data
+        self.data = Bunch()
         self.data.t, self.data.q = [], []
-        self.data.psi_ss, self.data.psi_rs = [], []
-        self.data.theta_M, self.data.w_M = [], []
+        self.data.psi_s, self.data.theta_m = [], []
+        self.data.w_M, self.data.theta_M = [], []
 
     def get_initial_values(self):
         """
         Get the initial values.
 
         Returns
         -------
         x0 : complex list, length 4
             Initial values of the state variables.
 
         """
         x0 = [
-            self.motor.psi_ss0,
-            self.motor.psi_rs0,
-            self.mech.w_M0,
-            self.mech.theta_M0,
+            self.machine.psi_s0,
+            self.machine.theta_m0,
+            self.mechanics.w_M0,
+            self.mechanics.theta_M0,
         ]
         return x0
 
     def set_initial_values(self, t0, x0):
         """
         Set the initial values.
 
         Parameters
         ----------
+        t0 : float
+            Initial time (s).
         x0 : complex ndarray
             Initial values of the state variables.
 
         """
         self.t0 = t0
-        self.motor.psi_ss0 = x0[0]
-        self.motor.psi_rs0 = x0[1]
-        # x0[2].imag and x0[3].imag are always zero
-        self.mech.w_M0 = x0[2].real
-        # Limit theta_M0 = x0[3].real into [-pi, pi)
-        self.mech.theta_M0 = np.mod(x0[3].real + np.pi, 2*np.pi) - np.pi
+        self.machine.psi_s0 = x0[0]
+        # x0[1:3].imag are always zero
+        self.machine.theta_m0 = x0[1].real
+        self.mechanics.w_M0 = x0[2].real
+        # Limit the angles into [-pi, pi)
+        self.mechanics.theta_m0 = np.mod(x0[1].real + np.pi, 2*np.pi) - np.pi
+        self.mechanics.theta_M0 = np.mod(x0[3].real + np.pi, 2*np.pi) - np.pi
 
     def f(self, t, x):
         """
         Compute the complete state derivative list for the solver.
 
         Parameters
         ----------
         t : float
-            Time.
+            Time (s).
         x : complex ndarray
             State vector.
 
         Returns
         -------
         complex list
             State derivatives.
 
         """
         # Unpack the states
-        psi_ss, psi_rs, w_M, _ = x
+        psi_s, theta_m, w_M, _ = x
+
         # Interconnections: outputs for computing the state derivatives
-        u_ss = self.conv.ac_voltage(self.conv.q, self.conv.u_dc0)
-        # State derivatives plus the outputs for interconnections
-        motor_f, _, tau_M = self.motor.f(psi_ss, psi_rs, u_ss, w_M)
-        mech_f = self.mech.f(t, w_M, tau_M)
+        u_ss = self.converter.ac_voltage(
+            self.converter.q, self.converter.u_dc0)
+        u_s = np.exp(-1j*theta_m)*u_ss  # Stator voltage in rotor coordinates
+
+        # State derivatives
+        machine_f, _, tau_M = self.machine.f(psi_s, u_s, w_M)
+        mechanics_f = self.mechanics.f(t, w_M, tau_M)
+
         # List of state derivatives
-        return motor_f + mech_f
+        return machine_f + mechanics_f
 
     def save(self, sol):
         """
         Save the solution.
 
         Parameters
         ----------
-        sol : Bunch object
+        sol : Bunch
             Solution from the solver.
 
         """
         self.data.t.extend(sol.t)
         self.data.q.extend(sol.q)
-        self.data.psi_ss.extend(sol.y[0])
-        self.data.psi_rs.extend(sol.y[1])
+        self.data.psi_s.extend(sol.y[0])
+        self.data.theta_m.extend(sol.y[1].real)
         self.data.w_M.extend(sol.y[2].real)
         self.data.theta_M.extend(sol.y[3].real)
 
     def post_process(self):
         """Transform the lists to the ndarray format and post-process them."""
         # From lists to the ndarray
         for key in self.data:
             self.data[key] = np.asarray(self.data[key])
 
-        # Some useful variables
-        self.data.i_ss, _, self.data.tau_M = self.motor.magnetic(
-            self.data.psi_ss, self.data.psi_rs)
+        # Compute some useful quantities
+        self.data.i_s, self.data.tau_M = self.machine.magnetic(self.data.psi_s)
+        self.data.w_m = self.machine.n_p*self.data.w_M
+        self.data.tau_L = (
+            self.mechanics.tau_L_t(self.data.t) +
+            self.mechanics.tau_L_w(self.data.w_M))
+        self.data.u_ss = self.converter.ac_voltage(
+            self.data.q, self.converter.u_dc0)
+        self.data.theta_m = np.mod(  # Limit into [-pi, pi)
+            self.data.theta_m + np.pi, 2*np.pi) - np.pi
         self.data.theta_M = np.mod(  # Limit into [-pi, pi)
             self.data.theta_M + np.pi, 2*np.pi) - np.pi
-        self.data.theta_m = np.mod(  # Limit into [-pi, pi)
-            self.motor.n_p*self.data.theta_M + np.pi, 2*np.pi) - np.pi
-        self.data.w_m = self.motor.n_p*self.data.w_M
-        self.data.tau_L = (
-            self.mech.tau_L_t(self.data.t) + self.mech.tau_L_w(self.data.w_M))
-        self.data.u_ss = self.conv.ac_voltage(self.data.q, self.conv.u_dc0)
-
-        # Compute the inverse-Γ rotor flux
-        try:
-            # Saturable stator inductance
-            L_s = self.motor.L_s(np.abs(self.data.psi_ss))
-        except TypeError:
-            # Constant stator inductance
-            L_s = self.motor.L_s
-        gamma = L_s/(L_s + self.motor.L_ell)  # Magnetic coupling factor
-        self.data.psi_Rs = gamma*self.data.psi_rs
-
-
-# %%
-class InductionMotorDriveDiode(InductionMotorDrive):
-    """
-    Induction motor drive equipped with a diode bridge.
-
-    This model extends the InductionMotorDrive class with a model for a
-    three-phase diode bridge fed from stiff supply voltages. The DC bus is
-    modeled as an inductor and a capacitor.
-
-    Parameters
-    ----------
-    motor : InductionMotor | InductionMotorSaturated
-        Induction motor model.
-    mech : Mechanics
-        Mechanics model.
-    conv : FrequencyConverter
-        Frequency converter model.
-
-    """
-
-    def __init__(self, motor=None, mech=None, conv=None):
-        super().__init__(motor=motor, mech=mech)
-        self.conv = conv
-        self.data.u_dc, self.data.i_L = [], []
-
-    def get_initial_values(self):
-        """Extend the base class."""
-        x0 = super().get_initial_values() + [self.conv.u_dc0, self.conv.i_L0]
-        return x0
-
-    def set_initial_values(self, t0, x0):
-        """Extend the base class."""
-        super().set_initial_values(t0, x0[0:4])
-        self.conv.u_dc0 = x0[4].real
-        self.conv.i_L0 = x0[5].real
-
-    def f(self, t, x):
-        """Override the base class."""
-        # Unpack the states for better readability
-        psi_ss, psi_rs, w_M, _, u_dc, i_L = x
-
-        # Interconnections: outputs for computing the state derivatives
-        u_ss = self.conv.ac_voltage(self.conv.q, u_dc)
-        motor_f, i_ss, tau_M = self.motor.f(psi_ss, psi_rs, u_ss, w_M)
-        i_dc = self.conv.dc_current(self.conv.q, i_ss)
-
-        # Return the list of state derivatives
-        return (
-            motor_f + self.mech.f(t, w_M, tau_M) +
-            self.conv.f(t, u_dc, i_L, i_dc))
-
-    def save(self, sol):
-        """Extend the base class."""
-        super().save(sol)
-        self.data.u_dc.extend(sol.y[4].real)
-        self.data.i_L.extend(sol.y[5].real)
-
-    def post_process(self):
-        """Extend the base class."""
-        super().post_process()
-        # From lists to the ndarray
-        self.data.u_dc = np.asarray(self.data.u_dc)
-        self.data.i_L = np.asarray(self.data.i_L)
-        # Some useful variables
-        self.data.u_ss = self.conv.ac_voltage(self.data.q, self.data.u_dc)
-        self.data.i_dc = self.conv.dc_current(self.data.q, self.data.i_ss)
-        u_g_abc = self.conv.grid_voltages(self.data.t)
-        self.data.u_g = abc2complex(u_g_abc)
-        # Voltage at the output of the diode bridge
-        self.data.u_di = np.amax(u_g_abc, axis=0) - np.amin(u_g_abc, axis=0)
-        # Diode briddge switching states (-1, 0, 1)
-        q_g_abc = ((np.amax(u_g_abc, axis=0) == u_g_abc).astype(int) -
-                   (np.amin(u_g_abc, axis=0) == u_g_abc).astype(int))
-        # Grid current space vector
-        self.data.i_g = abc2complex(q_g_abc)*self.data.i_L
+        self.data.i_ss = self.data.i_s*np.exp(1j*self.data.theta_m)
 
 
 # %%
-class InductionMotorDriveTwoMass(InductionMotorDrive):
+class DriveTwoMassMechanics(Drive):
     """
-    Induction motor drive with two-mass mechanics.
+    Synchronous machine drive with two-mass mechanics.
 
-    This interconnects the subsystems of an induction motor drive and provides
-    an interface to the solver.
+    This interconnects the subsystems of a synchronous machine drive and
+    provides an interface to the solver.
 
     Parameters
     ----------
-    motor : InductionMotor | InductionMotorSaturated
-        Induction motor model.
-    mech : MechanicsTwoMass
+    machine : SynchronousMachine
+        Synchronous machine model.
+    mechanics : MechanicsTwoMass
         Mechanics model.
-    conv : Inverter
+    converter : Inverter
         Inverter model.
 
     """
 
-    def __init__(self, motor=None, mech=None, conv=None):
-        super().__init__(motor=motor, mech=mech, conv=conv)
+    def __init__(self, machine=None, mechanics=None, converter=None):
+        super().__init__(machine, mechanics, converter)
         self.data.w_L, self.data.theta_ML = [], []
 
     def get_initial_values(self):
         """Extend the base class."""
         x0 = super().get_initial_values() + [
-            self.mech.w_L0, self.mech.theta_ML0
+            self.mechanics.w_L0, self.mechanics.theta_ML0
         ]
         return x0
 
     def set_initial_values(self, t0, x0):
         """Extend the base class."""
         super().set_initial_values(t0, x0[0:4])
-        self.mech.w_L0 = x0[4].real
-        self.mech.theta_ML0 = np.mod(x0[5].real + np.pi, 2*np.pi) - np.pi
+        self.mechanics.w_L0 = x0[4].real
+        self.mechanics.theta_ML0 = np.mod(x0[5].real + np.pi, 2*np.pi) - np.pi
 
     def f(self, t, x):
         """Override the base class."""
         # Unpack the states
-        psi_ss, psi_rs, w_M, _, w_L, theta_ML = x
+        psi_s, theta_m, w_M, _, w_L, theta_ML = x
         # Interconnections: outputs for computing the state derivatives
-        u_ss = self.conv.ac_voltage(self.conv.q, self.conv.u_dc0)
+        u_ss = self.converter.ac_voltage(
+            self.converter.q, self.converter.u_dc0)
+        u_s = np.exp(-1j*theta_m)*u_ss  # Stator voltage in rotor coordinates
         # State derivatives plus the outputs for interconnections
-        motor_f, _, tau_M = self.motor.f(psi_ss, psi_rs, u_ss, w_M)
-        mech_f = self.mech.f(t, w_M, w_L, theta_ML, tau_M)
+        machine_f, _, tau_M = self.machine.f(psi_s, u_s, w_M)
+        mechanics_f = self.mechanics.f(t, w_M, w_L, theta_ML, tau_M)
         # List of state derivatives
-        return motor_f + mech_f
+        return machine_f + mechanics_f
 
     def save(self, sol):
         """Extend the base class."""
         super().save(sol)
         self.data.w_L.extend(sol.y[4].real)
         self.data.theta_ML.extend(sol.y[5].real)
```

### Comparing `motulator-0.1.4/motulator/model/mech.py` & `motulator-0.1.5/motulator/model/_mechanics.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,43 +7,43 @@
     Mechanics subsystem.
 
     This models an equation of motion for stiff mechanics.
 
     Parameters
     ----------
     J : float
-        Total moment of inertia.
-    tau_L_w : function
-        Load torque as function of speed, `tau_L_w(w_M)`. For example,
-        tau_L_w = b*w_M, where b is the viscous friction coefficient.
-    tau_L_t : function
-        Load torque as a function of time, `tau_L_t(t)`.
+        Total moment of inertia (kgm²).
+    tau_L_w : callable
+        Load torque (Nm) as a function of speed, `tau_L_w(w_M)`. For example,
+        ``tau_L_w = b*w_M``, where `b` is the viscous friction coefficient. The
+        default is zero, ``lambda w_M: 0*w_M``.
+    tau_L_t : callable
+        Load torque (Nm) as a function of time, `tau_L_t(t)`. The default is 
+        zero, ``lambda t: 0*t``.
 
     """
 
-    def __init__(
-            self, J=.015, tau_L_w=lambda w_M: 0*w_M, tau_L_t=lambda t: 0*t):
+    def __init__(self, J, tau_L_w=lambda w_M: 0*w_M, tau_L_t=lambda t: 0*t):
         self.J = J
-        self.tau_L_t = tau_L_t
-        self.tau_L_w = tau_L_w
+        self.tau_L_t, self.tau_L_w = tau_L_t, tau_L_w
         # Initial values
         self.w_M0, self.theta_M0 = 0, 0
 
     def f(self, t, w_M, tau_M):
         """
         Compute the state derivatives.
 
         Parameters
         ----------
         t : float
-            Time.
+            Time (s).
         w_M : float
-            Rotor angular speed (in mechanical rad/s).
+            Rotor angular speed (mechanical rad/s).
         tau_M : float
-            Electromagnetic torque.
+            Electromagnetic torque (Nm).
 
         Returns
         -------
         list, length 2
             Time derivatives of the state vector.
 
         """
@@ -59,15 +59,15 @@
         Measure the rotor speed.
 
         This returns the rotor speed at the end of the sampling period.
 
         Returns
         -------
         w_M0 : float
-            Rotor angular speed (in mechanical rad/s).
+            Rotor angular speed (mechanical rad/s).
 
         """
         # The quantization noise of an incremental encoder could be modeled
         # by means of the rotor angle, to be done later.
         return self.w_M0
 
     def meas_position(self):
@@ -75,15 +75,15 @@
         Measure the rotor angle.
 
         This returns the rotor angle at the end of the sampling period.
 
         Returns
         -------
         theta_M0 : float
-            Rotor angle (in mechanical rad).
+            Rotor angle (mechanical rad).
 
         """
         return self.theta_M0
 
 
 # %%
 class MechanicsTwoMass(Mechanics):
@@ -91,67 +91,59 @@
     Two-mass mechanics subsystem.
 
     This models an equation of motion for two-mass mechanics.
 
     Parameters
     ----------
     J_M : float
-        Moment of inertia of the motor.
+        Motor moment of inertia (kgm²).
     J_L : float
-        Moment of inertia of the load.
+        Load moment of inertia (kgm²).
     K_S : float
-        Torsional stiffness of the shaft.
+        Shaft torsional stiffness (Nm).
     C_S : float
-        Torsional damping of the shaft.
-    tau_L_w : function
-        Load torque as function of the load speed, `tau_L_w(w_L)`. For example,
-        tau_L_w = b*w_L, where b is the viscous friction coefficient.
-    tau_L_t : function
-        Load torque as a function of time, `tau_L_t(t)`.
+        Shaft torsional damping (Nms).
+    tau_L_w : callable
+        Load torque (Nm) as a function of the load speed, `tau_L_w(w_L)`, e.g., 
+        ``tau_L_w = B*w_L``, where `B` is the viscous friction coefficient. The
+        default is zero, ``lambda w_L: 0*w_L``.
+    tau_L_t : callable
+        Load torque (Nm) as a function of time, `tau_L_t(t)`. The default is
+        zero, ``lambda t: 0*t``.
 
     """
 
     # pylint: disable=too-many-instance-attributes
-    def __init__(
-            self,
-            J_M=.005,
-            J_L=.005,
-            K_S=700.,
-            C_S=.13,
-            tau_L_w=lambda w_M: 0*w_M,
-            tau_L_t=lambda t: 0*t):
+    def __init__(self, J_M, J_L, K_S, C_S, tau_L_w=None, tau_L_t=None):
         # pylint: disable=too-many-arguments
         # pylint: disable=super-init-not-called
-        self.J_M = J_M
-        self.J_L = J_L
-        self.K_S = K_S
-        self.C_S = C_S
-        self.tau_L_t = tau_L_t
-        self.tau_L_w = tau_L_w
+        self.J_M, self.J_L, self.K_S, self.C_S = J_M, J_L, K_S, C_S
+        self.tau_L_w = tau_L_w if tau_L_w is not None else lambda w_L: 0*w_L
+        self.tau_L_t = tau_L_t if tau_L_t is not None else lambda t: 0*t
         # Initial values
         self.w_M0, self.theta_M0, self.w_L0, self.theta_ML0 = 0, 0, 0, 0
 
     def f(self, t, w_M, w_L, theta_ML, tau_M):
         # pylint: disable=too-many-arguments
         # pylint: disable=arguments-differ
         """
         Compute the state derivatives.
 
         Parameters
         ----------
         t : float
-            Time.
+            Time (s).
         w_M : float
-            Rotor angular speed (in mechanical rad/s).
+            Rotor angular speed (mechanical rad/s).
         w_L : float
-            Load angular speed (in mechanical rad/s).
+            Load angular speed (mechanical rad/s).
         theta_ML : float
-            Twist angle, theta_M - theta_L (in mechanical rad).
+            Twist angle, theta_M - theta_L (mechanical rad).
         tau_M : float
-            Electromagnetic torque.
+            Electromagnetic torque (Nm).
 
         Returns
         -------
         list, length 4
             Time derivatives of the state vector.
 
         """
@@ -172,26 +164,26 @@
         Measure the load speed.
 
         This returns the load speed at the end of the sampling period.
 
         Returns
         -------
         w_L0 : float
-            Load angular speed (in mechanical rad/s).
+            Load angular speed (mechanical rad/s).
 
         """
         return self.w_L0
 
     def meas_load_position(self):
         """
         Measure the load angle.
 
         This returns the load angle at the end of the sampling period.
 
         Returns
         -------
         theta_L0 : float
-            Rotor angle (in mechanical rad).
+            Rotor angle (mechanical rad).
 
         """
         theta_L0 = self.theta_M0 - self.theta_ML0
         return theta_L0
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `motulator-0.1.4/motulator/model/sm_flux_maps.py` & `motulator-0.1.5/motulator/model/sm/_flux_maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # %%
 import numpy as np
 import matplotlib.pyplot as plt
 from cycler import cycler
 from scipy.io import loadmat
 from scipy.interpolate import griddata
-from motulator.helpers import Bunch
+from motulator._utils import Bunch
 
 # Plotting parameters
 plt.rcParams['axes.prop_cycle'] = cycler(color='brgcmyk')
 plt.rcParams['lines.linewidth'] = 1.
 plt.rcParams['axes.grid'] = True
 plt.rcParams.update({'text.usetex': False})
 
@@ -35,18 +35,19 @@
     add_negative_q_axis : bool, optional
         Adds the negative q-axis data based on the symmetry.
 
     Returns
     -------
     Bunch object with the following fields defined:
     i_s : complex ndarray
-        Stator current data.
+        Stator current data (A).
     psi_s : complex ndarray
-        Stator flux linkage data.
+        Stator flux linkage data (Vs).
     tau_M : ndarray
+        Torque data (Nm).
 
     Notes
     -----
     Some example data files (including THOR.mat) are available in the SyR-e
     repository, licensed under the Apache License, Version 2.0.
 
     """
@@ -193,18 +194,19 @@
     N_q : int, optional
         Number of interpolated samples in the q axis. The default is 32.
 
     Returns
     -------
     Bunch object with the following fields defined:
     i_s : complex ndarray, shape (N_d, N_q)
-        Stator current data.
+        Stator current data (A).
     psi_s : complex ndarray, shape (N_d, N_q)
-        Stator flux linkage data.
+        Stator flux linkage data (Vs).
     tau_M : ndarray, shape (N_d, N_q)
+        Torque data (Nm).
 
     """
     # Points at which to interpolate data
     i_d = np.linspace(np.min(data.i_s.real), np.max(data.i_s.real), N_d)
     i_q = np.linspace(np.min(data.i_s.imag), np.max(data.i_s.imag), N_q)
     i_d, i_q = np.meshgrid(i_d, i_q)
 
@@ -231,18 +233,19 @@
     N_q : int, optional
         Number of interpolated samples in the q axis. The default is 32.
 
     Returns
     -------
     Bunch object with the following fields defined:
     psi_s : complex ndarray, shape (N_d, N_q)
-        Stator flux linkage data.
+        Stator flux linkage data (Vs).
     i_s : complex ndarray, shape (N_d, N_q)
-        Stator current data.
+        Stator current data (A).
     tau_M : ndarray, shape (N_d, N_q)
+        Torque data (Nm).
 
     """
     # Get the range
     psi_d_max = np.min(np.max(data.psi_s.real, axis=0))
     psi_d_min = np.max(np.min(data.psi_s.real, axis=0))
     psi_q_max = np.min(np.max(data.psi_s.imag, axis=1))
     psi_q_min = np.max(np.min(data.psi_s.imag, axis=1))
```

### Comparing `motulator-0.1.4/motulator/plots.py` & `motulator-0.1.5/motulator/_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Example plotting scripts."""
 
 # %%
 import numpy as np
 import matplotlib.pyplot as plt
 from cycler import cycler
-from motulator.helpers import Bunch, complex2abc
+from motulator._helpers import complex2abc
+from motulator._utils import Bunch
 
 # Plotting parameters
 plt.rcParams['axes.prop_cycle'] = cycler(color='brgcmyk')
 plt.rcParams['lines.linewidth'] = 1.
 plt.rcParams['axes.grid'] = True
 plt.rcParams.update({"text.usetex": False})
 
 
 # %%
-def plot(sim, t_span=None, base=None):
+# pylint: disable=too-many-branches
+def plot(sim, base=None, t_span=None):
     """
     Plot example figures.
 
     Plots figures in per-unit values, if the base values are given. Otherwise
     SI units are used.
 
     Parameters
     ----------
-    sim : Simulation object
+    sim : Simulation
         Should contain the simulated data.
-    t_span : 2-tuple, optional
-        Time span. The default is (0, sim.ctrl.t[-1]).
     base : BaseValues, optional
         Base values for scaling the waveforms.
+    t_span : 2-tuple, optional
+        Time span. The default is (0, sim.ctrl.t[-1]).
 
     """
     # pylint: disable=too-many-statements
     mdl = sim.mdl.data  # Continuous-time data
     ctrl = sim.ctrl.data  # Discrete-time data
 
     # Check if the time span was given
@@ -148,31 +150,36 @@
     fig.align_ylabels()
 
     plt.tight_layout()
     plt.show()
 
 
 # %%
-def plot_extra(sim, t_span=(1.1, 1.125), base=None):
+# pylint: disable=too-many-statements
+def plot_extra(sim, base=None, t_span=None):
     """
     Plot extra waveforms for a motor drive with a diode bridge.
 
     Parameters
     ----------
-    sim : Simulation object
+    sim : Simulation
         Should contain the simulated data.
-    t_span : 2-tuple, optional
-        Time span. The default is (1.1, 1.125).
     base : BaseValues, optional
         Base values for scaling the waveforms.
+    t_span : 2-tuple, optional
+        Time span. The default is (0, sim.ctrl.t[-1]).
 
     """
     mdl = sim.mdl.data  # Continuous-time data
     ctrl = sim.ctrl.data  # Discrete-time data
 
+    # Check if the time span was given
+    if t_span is None:
+        t_span = (0, ctrl.t[-1])
+
     # Check if the base values were iven
     if base is not None:
         pu_vals = True
     else:
         pu_vals = False
         base = Bunch(w=1, u=1, i=1, psi=1, tau=1)  # Unity base values
 
@@ -251,18 +258,16 @@
 
 # %%
 def save_plot(name):
     """
     Save figures.
 
     This saves figures in a folder "figures" in the current directory. If the
-    folder doesn't exist, it is created.
+    folder does not exist, it is created.
 
     Parameters
     ----------
     name : string
         Name for the figure
-    plt : object
-        Handle for the figure to be saved
 
     """
     plt.savefig(name + '.pdf')
```

### Comparing `motulator-0.1.4/motulator/simulation.py` & `motulator-0.1.5/motulator/model/_simulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Simulation environment."""
 
 import numpy as np
 from scipy.integrate import solve_ivp
 from scipy.io import savemat
-from motulator.helpers import abc2complex
+from motulator._helpers import abc2complex
 
 
 # %%
 class Delay:
     """
     Computational delay.
 
@@ -41,15 +41,15 @@
         # Add the latest value to the end of the list
         self.data.append(u)
         # Pop the first element and return it
         return self.data.pop(0)
 
 
 # %%
-class CarrierCmp:
+class CarrierComparison:
     """
     Carrier comparison.
 
     This computes the the switching states and their durations based on the
     duty ratios. Instead of searching for zero crossings, the switching
     instants are explicitly computed in the beginning of each sampling period,
     allowing faster simulations.
@@ -60,16 +60,16 @@
         Amount of the counter quantization levels. The default is 2**12.
     return_complex : bool, optional
         Complex switching state space vectors are returned if True. Otherwise
         phase switching states are returned. The default is True.
 
     Examples
     --------
-    >>> from motulator.simulation import CarrierCmp
-    >>> carrier_cmp = CarrierCmp(return_complex=False)
+    >>> from motulator.model import CarrierComparison
+    >>> carrier_cmp = CarrierComparison(return_complex=False)
     >>> # First call gives rising edges
     >>> t_steps, q_abc = carrier_cmp(1e-3, [.4, .2, .8])
     >>> # Durations of the switching states
     >>> t_steps
     array([0.00019995, 0.00040015, 0.00019995, 0.00019995])
     >>> # Switching states
     >>> q_abc
@@ -100,31 +100,31 @@
            [1, 1, 1]])
 
     """
 
     def __init__(self, N=2**12, return_complex=True):
         self.N = N
         self.return_complex = return_complex
-        self.rising_edge = True  # Stores the carrier direction
+        self._rising_edge = True  # Stores the carrier direction
 
     def __call__(self, T_s, d_abc):
         """
         Compute the switching state durations and vectors.
 
         Parameters
         ----------
         T_s : float
-            Half carrier period.
+            Half carrier period (s).
         d_abc : array_like of floats, shape (3,)
             Duty ratios in the range [0, 1].
 
         Returns
         -------
         t_steps : ndarray, shape (4,)
-            Switching state durations, `[t0, t1, t2, t3]`.
+            Switching state durations (s), `[t0, t1, t2, t3]`.
         q : complex ndarray, shape (4,)
             Switching state vectors, `[q0, q1, q2, q3]`, where `q1` and `q2`
             are active vectors.
 
         Notes
         -----
         No switching (e.g. `d_a == 0` or `d_a == 1`) or simultaneous switchings
@@ -139,27 +139,27 @@
         # Compute the correponding switching states:
         q_abc = (t_n[:, np.newaxis] < d_abc).astype(int)
 
         # Durations of switching states
         t_steps = T_s*np.diff(t_n, append=1)
 
         # Flip the sequence if rising edge
-        if self.rising_edge:
+        if self._rising_edge:
             t_steps = np.flip(t_steps)
             q_abc = np.flipud(q_abc)
 
         # Change the carrier direction for the next call
-        self.rising_edge = not self.rising_edge
+        self._rising_edge = not self._rising_edge
 
         return ((t_steps, abc2complex(q_abc.T)) if self.return_complex else
                 (t_steps, q_abc))
 
 
 # %%
-def zoh(T_s, d_abc):
+def _zoh(T_s, d_abc):
     """
     Zero-order hold of the duty ratios over the sampling period.
 
     Parameters
     ----------
     T_s : float
         Sampling period.
@@ -185,93 +185,93 @@
     """
     Simulation environment.
 
     Each simulation object has a system model object and a controller object.
 
     Parameters
     ----------
-    mdl : InductionMotorDrive | SynchronousMotorDrive
+    mdl : Drive 
         Continuous-time system model.
     ctrl : Ctrl
         Discrete-time controller.
     delay : int, optional
         Amount of computational delays. The default is 1.
     pwm : bool, optional
         Enable carrier comparison. The default is False.
 
     """
 
     def __init__(self, mdl=None, ctrl=None, delay=1, pwm=False):
         self.mdl = mdl
         self.ctrl = ctrl
-        self.delay = Delay(delay)
+        self._delay = Delay(delay)
         if pwm:
-            self.pwm = CarrierCmp()
+            self._pwm = CarrierComparison()
         else:
-            self.pwm = zoh
+            self._pwm = _zoh
 
     def simulate(self, t_stop=1, max_step=np.inf):
         """
         Solve the continuous-time model and call the discrete-time controller.
 
         Parameters
         ----------
         t_stop : float, optional
             Simulation stop time. The default is 1.
         max_step : float, optional
-            Max step size of the solver. The default is inf.
+            Max step size of the solver. The default is `inf`.
 
         Notes
         -----
-        Other options of solve_ivp could be easily changed if needed, but, for
-        simplicity, only max_step is included as an option of this method.
+        Other options of `solve_ivp` could be easily changed if needed, but, for
+        simplicity, only `max_step` is included as an option of this method.
 
         """
         try:
-            self.simulation_loop(t_stop, max_step)
+            self._simulation_loop(t_stop, max_step)
         except FloatingPointError:
             print(f'Invalid value encountered at {self.mdl.t0:.2f} seconds.')
         # Call the post-processing functions
         self.mdl.post_process()
         self.ctrl.post_process()
 
     @np.errstate(invalid='raise')
-    def simulation_loop(self, t_stop, max_step):
+    def _simulation_loop(self, t_stop, max_step):
         """Run the main simulation loop."""
         while self.mdl.t0 <= t_stop:
 
             # Run the digital controller
             T_s, d_abc_ref = self.ctrl(self.mdl)
 
             # Computational delay model
-            d_abc = self.delay(d_abc_ref)
+            d_abc = self._delay(d_abc_ref)
 
             # Carrier comparison
-            t_steps, q = self.pwm(T_s, d_abc)
+            t_steps, q = self._pwm(T_s, d_abc)
 
             # Loop over the sampling period T_s
             for i, t_step in enumerate(t_steps):
 
                 if t_step > 0:
                     # Update the switching state
-                    self.mdl.conv.q = q[i]
+                    self.mdl.converter.q = q[i]
 
                     # Get initial values
                     x0 = self.mdl.get_initial_values()
 
                     # Integrate over t_span
                     t_span = (self.mdl.t0, self.mdl.t0 + t_step)
                     sol = solve_ivp(self.mdl.f, t_span, x0, max_step=max_step)
 
                     # Set the new initial values (last points of the solution)
                     t0_new, x0_new = t_span[-1], sol.y[:, -1]
                     self.mdl.set_initial_values(t0_new, x0_new)
 
                     # Save the solution
-                    sol.q = len(sol.t)*[self.mdl.conv.q]
+                    sol.q = len(sol.t)*[self.mdl.converter.q]
                     self.mdl.save(sol)
 
     def save_mat(self, name='sim'):
         """
         Save the simulation data into MATLAB .mat files.
 
         Parameters
```

### Comparing `motulator-0.1.4/motulator.egg-info/PKG-INFO` & `motulator-0.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: motulator
-Version: 0.1.4
-Summary: Motor Drive Simulator in Python
-Home-page: https://github.com/Aalto-Electric-Drives/motulator
-Author: Marko Hinkkanen
-Author-email: marko.hinkkanen@aalto.fi
-Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # *motulator:* Motor Drive Simulator in Python
 [![Build Status](https://github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-pages.yml/badge.svg)](https://github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-pages.yml)
 [![License](https://img.shields.io/github/license/mashape/apistatus)](https://github.com/Aalto-Electric-Drives/motulator/blob/main/LICENSE)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/motulator.svg)](https://pypi.org/project/motulator/)
 [![All Contributors](https://img.shields.io/badge/all_contributors-6-orange.svg?style=flat-square)](#contributors-)
 
 Introduction
@@ -34,34 +19,15 @@
 ```
 Alternatively, the repository can be cloned:
 
 https://aalto-electric-drives.github.io/motulator/installation.html
 
 Usage
 -----
-The following example shows how to create a continuous-time system model, a discrete-time controller, and a simulation object:
-```python3
-import motulator as mt
-
-# Continuous-time model for the drive system
-motor = mt.InductionMotor()     # Motor model
-mech = mt.Mechanics()           # Mechanics model
-conv = mt.Inverter() 	        # Converter model
-mdl = mt.InductionMotorDrive(motor, mech, conv)
-
-# Discrete-time controller 
-pars = mt.InductionMotorVectorCtrlPars() 	# Dataclass of control parameters
-ctrl = mt.InductionMotorVectorCtrl(pars) 	# Sensorless controller
-
-# Create a simulation object, simulate, and plot example figures
-sim = mt.Simulation(mdl, ctrl)
-sim.simulate()
-mt.plot(sim)
-```
-This example applies the default settings. The drive system, controller, reference sequences etc. are easy to configure. The example scripts and Jupyter notebooks can be downloaded here:
+The drive system, controller, reference sequences etc. are easy to configure. As a starting point, example scripts and Jupyter notebooks can be downloaded here:
 
 https://aalto-electric-drives.github.io/motulator/auto_examples/index.html
 
 New system models and controllers can be developed using the existing ones as templates.
 
 Contributing
 ------------
@@ -86,14 +52,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/angelicaiaderosa"><img src="https://avatars.githubusercontent.com/u/112799415?v=4?s=50" width="50px;" alt="angelicaiaderosa"/><br /><sub><b>angelicaiaderosa</b></sub></a><br /><a href="https://github.com/Aalto-Electric-Drives/motulator/commits?author=angelicaiaderosa" title="Code">💻</a> <a href="#example-angelicaiaderosa" title="Examples">💡</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://www.kth.se/profile/lucap"><img src="https://avatars.githubusercontent.com/u/64190518?v=4?s=50" width="50px;" alt="Luca Peretti"/><br /><sub><b>Luca Peretti</b></sub></a><br /><a href="#ideas-lucaperetti" title="Ideas, Planning, & Feedback">🤔</a> <a href="#promotion-lucaperetti" title="Promotion">📣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/GianmarioPellegrinoPolito"><img src="https://avatars.githubusercontent.com/u/70333484?v=4?s=50" width="50px;" alt="GianmarioPellegrinoPolito"/><br /><sub><b>GianmarioPellegrinoPolito</b></sub></a><br /><a href="#data-GianmarioPellegrinoPolito" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/SimFerr"><img src="https://avatars.githubusercontent.com/u/67151973?v=4?s=50" width="50px;" alt="Simone Ferrari"/><br /><sub><b>Simone Ferrari</b></sub></a><br /><a href="#data-SimFerr" title="Data">🔣</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Jialed0303"><img src="https://avatars.githubusercontent.com/u/118135952?v=4?s=50" width="50px;" alt="Jialed0303"/><br /><sub><b>Jialed0303</b></sub></a><br /><a href="#ideas-Jialed0303" title="Ideas, Planning, & Feedback">🤔</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/murgui"><img src="https://avatars.githubusercontent.com/u/29175623?v=4?s=50" width="50px;" alt="murgui"/><br /><sub><b>murgui</b></sub></a><br /><a href="https://github.com/Aalto-Electric-Drives/motulator/issues?q=author%3Amurgui" title="Bug reports">🐛</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: motulator Version: 0.1.4 Summary: Motor Drive
-Simulator in Python Home-page: https://github.com/Aalto-Electric-Drives/
-motulator Author: Marko Hinkkanen Author-email: marko.hinkkanen@aalto.fi
-Project-URL: Bug Tracker, https://github.com/Aalto-Electric-Drives/motulator/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
-LICENSE # *motulator:* Motor Drive Simulator in Python [![Build Status](https:/
-/github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-
+# *motulator:* Motor Drive Simulator in Python [![Build Status](https://
+github.com/Aalto-Electric-Drives/motulator/actions/workflows/update_gh-
 pages.yml/badge.svg)](https://github.com/Aalto-Electric-Drives/motulator/
 actions/workflows/update_gh-pages.yml) [![License](https://img.shields.io/
 github/license/mashape/apistatus)](https://github.com/Aalto-Electric-Drives/
 motulator/blob/main/LICENSE) [![PyPI version shields.io](https://
 img.shields.io/pypi/v/motulator.svg)](https://pypi.org/project/motulator/) [!
 [All Contributors](https://img.shields.io/badge/all_contributors-6-
 orange.svg?style=flat-square)](#contributors-) Introduction ------------ This
@@ -19,39 +12,30 @@
 motor models are simulated in the continuous-time domain while the control
 algorithms run in discrete time. The default solver is the explicit Runge-Kutta
 method of order 5(4) from scipy.integrate.solve_ivp. Simple control algorithms
 are provided as examples. The documentation is available here: https://aalto-
 electric-drives.github.io/motulator/ Installation ------------ This software
 can be installed using pip: ```bash pip install motulator ``` Alternatively,
 the repository can be cloned: https://aalto-electric-drives.github.io/
-motulator/installation.html Usage ----- The following example shows how to
-create a continuous-time system model, a discrete-time controller, and a
-simulation object: ```python3 import motulator as mt # Continuous-time model
-for the drive system motor = mt.InductionMotor() # Motor model mech =
-mt.Mechanics() # Mechanics model conv = mt.Inverter() # Converter model mdl =
-mt.InductionMotorDrive(motor, mech, conv) # Discrete-time controller pars =
-mt.InductionMotorVectorCtrlPars() # Dataclass of control parameters ctrl =
-mt.InductionMotorVectorCtrl(pars) # Sensorless controller # Create a simulation
-object, simulate, and plot example figures sim = mt.Simulation(mdl, ctrl)
-sim.simulate() mt.plot(sim) ``` This example applies the default settings. The
-drive system, controller, reference sequences etc. are easy to configure. The
-example scripts and Jupyter notebooks can be downloaded here: https://aalto-
-electric-drives.github.io/motulator/auto_examples/index.html New system models
-and controllers can be developed using the existing ones as templates.
-Contributing ------------ If you'd like to help us develop motulator, please
-have a look at these [guidelines](https://github.com/Aalto-Electric-Drives/
-motulator/blob/main/CONTRIBUTING.md) first. Contributors ------------ Thanks go
-to these wonderful people:
+motulator/installation.html Usage ----- The drive system, controller, reference
+sequences etc. are easy to configure. As a starting point, example scripts and
+Jupyter notebooks can be downloaded here: https://aalto-electric-
+drives.github.io/motulator/auto_examples/index.html New system models and
+controllers can be developed using the existing ones as templates. Contributing
+------------ If you'd like to help us develop motulator, please have a look at
+these [guidelines](https://github.com/Aalto-Electric-Drives/motulator/blob/
+main/CONTRIBUTING.md) first. Contributors ------------ Thanks go to these
+wonderful people:
                 [Lauri_Tiitinen]                          [HannuHar]              [Marko_Hinkkanen]         [silundbe]      [JoonaKukkonen]  [jarno-  [angelicaiaderosa]
                  Lauri_Tiitinen                            HannuHar                Marko_Hinkkanen           silundbe        JoonaKukkonen      k]     angelicaiaderosa
            ð» ð¤ ð¡ ð§â         ð» ð        ð» ð¤ ð�    ð» ð�    ð» ð�jarno-k      ð» ð¡
                                                                                                                                                ð¤
-                       [Luca_Peretti]             [GianmarioPellegrinoPolito]        [Simone_Ferrari]       [Jialed0303]
-                        Luca_Peretti               GianmarioPellegrinoPolito          Simone_Ferrari         Jialed0303
-                          ð¤ ð£                  ð£                      ð£             ð¤
+                       [Luca_Peretti]             [GianmarioPellegrinoPolito]        [Simone_Ferrari]       [Jialed0303]        [murgui]
+                        Luca_Peretti               GianmarioPellegrinoPolito          Simone_Ferrari         Jialed0303          murgui
+                          ð¤ ð£                  ð£                      ð£             ð¤          ð
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! Acknowledgement --------------- This project has been sponsored by ABB
 Oy and by the Academy of Finland *Centre of Excellence in High-Speed
 Electromechanical Energy Conversion Systems*. The example control methods
 included in this repository are based on published algorithms (available in
 textbooks and scientific articles). They do not present any proprietary control
```

### Comparing `motulator-0.1.4/motulator.egg-info/SOURCES.txt` & `motulator-0.1.5/motulator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 motulator/__init__.py
-motulator/helpers.py
-motulator/plots.py
-motulator/simulation.py
+motulator/_helpers.py
+motulator/_plots.py
+motulator/_utils.py
 motulator.egg-info/PKG-INFO
 motulator.egg-info/SOURCES.txt
 motulator.egg-info/dependency_links.txt
 motulator.egg-info/top_level.txt
 motulator/control/__init__.py
-motulator/control/common.py
-motulator/control/im_obs_vhz.py
-motulator/control/im_vector.py
-motulator/control/im_vhz.py
-motulator/control/sm_flux_vector.py
-motulator/control/sm_obs_vhz.py
-motulator/control/sm_signal_inj.py
-motulator/control/sm_torque.py
-motulator/control/sm_vector.py
+motulator/control/_common.py
+motulator/control/im/__init__.py
+motulator/control/im/_obs_vhz.py
+motulator/control/im/_vector.py
+motulator/control/im/_vhz.py
+motulator/control/sm/__init__.py
+motulator/control/sm/_flux_vector.py
+motulator/control/sm/_obs_vhz.py
+motulator/control/sm/_signal_inj.py
+motulator/control/sm/_torque.py
+motulator/control/sm/_vector.py
 motulator/model/__init__.py
-motulator/model/converter.py
-motulator/model/im.py
-motulator/model/im_drive.py
-motulator/model/mech.py
-motulator/model/sm.py
-motulator/model/sm_drive.py
-motulator/model/sm_flux_maps.py
+motulator/model/_converter.py
+motulator/model/_mechanics.py
+motulator/model/_simulation.py
+motulator/model/im/__init__.py
+motulator/model/im/_drive.py
+motulator/model/sm/__init__.py
+motulator/model/sm/_drive.py
+motulator/model/sm/_flux_maps.py
```

### Comparing `motulator-0.1.4/setup.cfg` & `motulator-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = motulator
-version = 0.1.4
+version = 0.1.5
 author = Marko Hinkkanen
 author_email = marko.hinkkanen@aalto.fi
 description = Motor Drive Simulator in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Aalto-Electric-Drives/motulator
 project_urls =
```

