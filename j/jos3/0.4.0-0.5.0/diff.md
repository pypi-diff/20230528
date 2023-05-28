# Comparing `tmp/jos3-0.4.0.tar.gz` & `tmp/jos3-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jos3-0.4.0.tar", last modified: Wed Aug 17 03:00:51 2022, max compression
+gzip compressed data, was "jos3-0.5.0.tar", last modified: Sun May 28 03:00:38 2023, max compression
```

## Comparing `jos3-0.4.0.tar` & `jos3-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-08-17 03:00:51.695567 jos3-0.4.0/
--rw-rw-rw-   0        0        0     1095 2022-01-10 05:19:36.000000 jos3-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     3069 2022-08-17 03:00:51.694563 jos3-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     2229 2022-02-20 05:55:30.000000 jos3-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2022-08-17 03:00:51.695567 jos3-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1726 2022-01-10 05:19:36.000000 jos3-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-17 03:00:51.601290 jos3-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-17 03:00:51.672944 jos3-0.4.0/src/jos3/
--rw-rw-rw-   0        0        0       71 2022-08-17 02:45:39.000000 jos3-0.4.0/src/jos3/__init__.py
--rw-rw-rw-   0        0        0     3500 2022-02-20 05:15:46.000000 jos3-0.4.0/src/jos3/comfmod.py
--rw-rw-rw-   0        0        0    14496 2022-04-24 09:40:08.000000 jos3-0.4.0/src/jos3/construction.py
--rw-rw-rw-   0        0        0    36283 2022-02-20 05:39:05.000000 jos3-0.4.0/src/jos3/jos3.py
--rw-rw-rw-   0        0        0    11779 2022-02-20 05:15:46.000000 jos3-0.4.0/src/jos3/matrix.py
--rw-rw-rw-   0        0        0    11430 2022-01-10 05:19:36.000000 jos3-0.4.0/src/jos3/params.py
--rw-rw-rw-   0        0        0    27804 2022-02-20 05:15:46.000000 jos3-0.4.0/src/jos3/thermoregulation.py
-drwxrwxrwx   0        0        0        0 2022-08-17 03:00:51.692266 jos3-0.4.0/src/jos3.egg-info/
--rw-rw-rw-   0        0        0     3069 2022-08-17 03:00:50.000000 jos3-0.4.0/src/jos3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2022-08-17 03:00:51.000000 jos3-0.4.0/src/jos3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-17 03:00:50.000000 jos3-0.4.0/src/jos3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-08-17 03:00:51.000000 jos3-0.4.0/src/jos3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 03:00:38.105621 jos3-0.5.0/
+-rw-rw-rw-   0        0        0     1095 2022-01-10 05:19:36.000000 jos3-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    15560 2023-05-28 03:00:38.104615 jos3-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14720 2023-05-28 02:48:29.000000 jos3-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 03:00:38.106619 jos3-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1726 2022-01-10 05:19:36.000000 jos3-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 03:00:38.025383 jos3-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 03:00:38.058922 jos3-0.5.0/src/jos3/
+-rw-rw-rw-   0        0        0       71 2023-05-28 02:48:29.000000 jos3-0.5.0/src/jos3/__init__.py
+-rw-rw-rw-   0        0        0     3500 2022-02-20 05:15:46.000000 jos3-0.5.0/src/jos3/comfmod.py
+-rw-rw-rw-   0        0        0    14496 2023-05-20 00:25:13.000000 jos3-0.5.0/src/jos3/construction.py
+-rw-rw-rw-   0        0        0    36650 2023-05-28 02:54:53.000000 jos3-0.5.0/src/jos3/jos3.py
+-rw-rw-rw-   0        0        0    11779 2022-02-20 05:15:46.000000 jos3-0.5.0/src/jos3/matrix.py
+-rw-rw-rw-   0        0        0    11420 2023-05-28 02:55:35.000000 jos3-0.5.0/src/jos3/params.py
+-rw-rw-rw-   0        0        0    28207 2023-05-28 02:54:02.000000 jos3-0.5.0/src/jos3/thermoregulation.py
+drwxrwxrwx   0        0        0        0 2023-05-28 03:00:38.101593 jos3-0.5.0/src/jos3.egg-info/
+-rw-rw-rw-   0        0        0    15560 2023-05-28 03:00:37.000000 jos3-0.5.0/src/jos3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-05-28 03:00:37.000000 jos3-0.5.0/src/jos3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 03:00:37.000000 jos3-0.5.0/src/jos3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-28 03:00:37.000000 jos3-0.5.0/src/jos3.egg-info/top_level.txt
```

### Comparing `jos3-0.4.0/LICENSE` & `jos3-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jos3-0.4.0/setup.py` & `jos3-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `jos3-0.4.0/src/jos3/comfmod.py` & `jos3-0.5.0/src/jos3/comfmod.py`

 * *Files identical despite different names*

### Comparing `jos3-0.4.0/src/jos3/construction.py` & `jos3-0.5.0/src/jos3/construction.py`

 * *Files identical despite different names*

### Comparing `jos3-0.4.0/src/jos3/jos3.py` & `jos3-0.5.0/src/jos3/jos3.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,31 +38,32 @@
     Parameters
     -------
     height : float, optional
         Body height [m]. The default is 1.72.
     weight : float, optional
         Body weight [kg]. The default is 74.43.
     fat : float, optional
-        Fat rte [%]. The default is 15.
+        Fat percentage [%]. The default is 15.
     age : int, optional
         Age [years]. The default is 20.
     sex : str, optional
         Sex ("male" or "female"). The default is "male".
     ci : float, optional
         Cardiac index [L/min/m2]. The default is 2.6432.
     bmr_equation : str, optional
         Choose a BMR equation. The default is "harris-benedict".
+        To use the equation for Japanese, enter "japanese".
     bsa_equation : str, optional
         Choose a BSA equation.
-        You can choose
+        You can choose "dubois", "fujimoto", "kruazumi", "takahira".
         The default is "dubois".
     ex_output : None, list or "all", optional
-        If you want to get extra output parameters, set the parameters as the list format.
+        If you want to get extra output parameters, set the parameters as the list format like ["BFsk", "BFcr", "Tar"].
         If ex_output is "all", all parameters are output.
-        The default is None.
+        The default is None, which outputs only important parameters such as local skin temperatures.
 
 
     Setter & Getter
     -------
     Input parameters of environmental conditions are set as the Setter format.
     If you set the different conditons in each body parts, set the list.
     List input must be 17 lengths and means the input of "Head", "Neck", "Chest",
@@ -141,15 +142,15 @@
     >>> model.Va = 0.2  # Air velocity [m/s]
     >>> model.PAR = 1.2  # Physical activity ratio [-]
     >>> model.posture = "sitting"  # Set the posture
     >>> model.simulate(60)  # Exposre time = 60 [min]
 
     Set the next phase:
 
-    >>> model.To = 20  # Chang only operative temperature
+    >>> model.To = 20  # Change only operative temperature
     >>> model.simulate(60)  # Additional exposre time = 60 [min]
 
 
     Show the results:
 
     >>> import pandas as pd
     >>> df = pd.DataFrame(model.dict_results())  # Make pandas.DataFrame
@@ -233,14 +234,15 @@
                 "bat_positive": False,
                 "ava_zero": False,
                 "shivering": False,}
         threg.PRE_SHIV = 0 # reset
         self._history = []
         self._t = dt.timedelta(0) # Elapsed time
         self._cycle = 0 # Cycle time
+        self._atmospheric_pressure = 101.33  # kPa. Used to fix the hc, he values
 
         # Reset setpoint temperature
         dictout = self._reset_setpt()
         self._history.append(dictout)  # Save the last model parameters
 
 
     def _reset_setpt(self):
@@ -330,18 +332,19 @@
         hr = threg.fixed_hr(threg.rad_coef(self._posture,))
         # Manual setting
         if self._hc is not None:
             hc = self._hc
         if self._hr is not None:
             hr = self._hr
 
+
         # Operarive temp. [oC], heat and evaporative heat resistance [m2.K/W], [m2.kPa/W]
         to = threg.operative_temp(self._ta, self._tr, hc, hr,)
-        r_t = threg.dry_r(hc, hr, self._clo)
-        r_et = threg.wet_r(hc, self._clo, self._iclo)
+        r_t = threg.dry_r(hc, hr, self._clo, pt=self._atmospheric_pressure)
+        r_et = threg.wet_r(hc, self._clo, iclo=self._iclo, pt=self._atmospheric_pressure)
 
         #------------------------------------------------------------------
         # Thermoregulation
         #------------------------------------------------------------------
         # Setpoint temperature of thermoregulation
         if passive:
             setpt_cr = tcr.copy()
@@ -1136,9 +1139,9 @@
         else:
             first_item = inp[0]
             array = np.ones(17)*first_item
     except:
         array = np.ones(17)*inp
     return array.copy()
 
-if __name__ is "__main__":
-    import jos3
+if __name__ == "__main__":
+    import jos3
```

### Comparing `jos3-0.4.0/src/jos3/matrix.py` & `jos3-0.5.0/src/jos3/matrix.py`

 * *Files identical despite different names*

### Comparing `jos3-0.4.0/src/jos3/params.py` & `jos3-0.5.0/src/jos3/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,13 +351,9 @@
             outparams += line + "\n"
 
     docs = outparams + "\n" + exoutparams
     docs = textwrap.indent(docs.strip(), "    ")
 
     return docs
 
-if __name__ is "__main__":
-    show_outparam_docs()
-
-
-
-
+if __name__ == "__main__":
+    show_outparam_docs()
```

### Comparing `jos3-0.4.0/src/jos3/thermoregulation.py` & `jos3-0.5.0/src/jos3/thermoregulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         0.096, 0.063, 0.050, 0.096, 0.063, 0.050,
         0.209, 0.112, 0.056, 0.209, 0.112, 0.056,])
 
 
 def conv_coef(posture="standing", va=0.1, ta=28.8, tsk=34.0,):
     """
     Calculate convective heat transfer coefficient (hc) [W/K.m2]
-    
+
     Parameters
     ----------
     posture : str, optional
         Select posture from standing, sitting or lying.
         The default is "standing".
     va : float or iter, optional
         Air velocity [m/s]. If iter is input, its length should be 17.
@@ -89,29 +89,29 @@
 
     return hc
 
 
 def rad_coef(posture="standing"):
     """
     Calculate radiative heat transfer coefficient (hr) [W/K.m2]
-    
+
     Parameters
     ----------
     posture : str, optional
         Select posture from standing, sitting or lying.
         The default is "standing".
 
     Returns
     -------
     hc : numpy.ndarray
         Radiative heat transfer coefficient (hr) [W/K.m2].
 
     """
-    
-    
+
+
     if posture.lower() == "standing":
         # Ichihara et al., 1997, https://doi.org/10.3130/aija.62.45_5
         hr = np.array([
                 4.89, 4.89, 4.32, 4.09, 4.32,
                 4.55, 4.43, 4.21, 4.55, 4.43, 4.21,
                 4.77, 5.34, 6.14, 4.77, 5.34, 6.14,])
     elif posture.lower() in ["sitting", "sedentary"]:
@@ -154,63 +154,74 @@
 
 
 def clo_area_factor(clo):
     fcl = np.where(clo<0.5, clo*0.2+1, clo*0.1+1.05)
     return fcl
 
 
-def dry_r(hc, hr, clo):
+def dry_r(hc, hr, clo, pt=101.33):
     """
     Calculate total sensible thermal resistance.
 
     Parameters
     ----------
     hc : float or array
         Convective heat transfer coefficient (hc) [W/K.m2].
     hr : float or array
         Radiative heat transfer coefficient (hr) [W/K.m2].
     clo : float or array
         Clothing insulation [clo].
+    pt : float
+        Local atmospheric pressure [kPa].
+        Corrected hc (hcc) is calculated as follows:
+            hcc = hc * ((pt / 101.33) ** 0.55)
 
     Returns
     -------
     rt : float or array
         Total sensible thermal resistance between skin and ambient.
     """
     fcl = clo_area_factor(clo)
-    r_a = 1/(hc+hr)
+    hcc = hc * ((pt / 101.33) ** 0.55)
+    r_a = 1/(hcc+hr)
     r_cl = 0.155*clo
     r_t = r_a/fcl + r_cl
     return r_t
 
 
-def wet_r(hc, clo, iclo=0.45, lewis_rate=16.5):
+def wet_r(hc, clo, iclo=0.45, lewis_rate=16.5, pt=101.33):
     """
     Calculate total evaporative thermal resistance.
 
     Parameters
     ----------
     hc : float or array
         Convective heat transfer coefficient (hc) [W/K.m2].
     clo : float or array
         Clothing insulation [clo].
     iclo : float, or array, optional
         Clothin vapor permeation efficiency [-]. The default is 0.45.
     lewis_rate : float, optional
         Lewis rate [K/kPa]. The default is 16.5.
+    pt : float
+        Local atmospheric pressure [kPa].
+        Corrected he (hec) is calculated as follows:
+            hec = he * ((101.33 / pt) ** 0.45)
 
     Returns
     -------
     ret : float or array
         Total evaporative thermal resistance.
 
     """
     fcl = clo_area_factor(clo)
     r_cl = 0.155 * clo
-    r_ea = 1 / (lewis_rate * hc)
+    he = hc * lewis_rate
+    hec = he * ((101.33 / pt) ** 0.45)
+    r_ea = 1 / hec
     r_ecl = r_cl / (lewis_rate * iclo)
     r_et = r_ea / fcl + r_ecl
     return r_et
 
 
 def heat_resistances(
         ta=np.ones(17)*28.8,
@@ -251,32 +262,32 @@
     # SKINR
     receptor = np.array([
             0.0549, 0.0146, 0.1492, 0.1321, 0.2122,
             0.0227, 0.0117, 0.0923, 0.0227, 0.0117, 0.0923,
             0.0501, 0.0251, 0.0167, 0.0501, 0.0251, 0.0167,])
 
     # wrms signal
-    wrm = np.maximum(err_sk, 0) 
+    wrm = np.maximum(err_sk, 0)
     wrm *= receptor
-    wrms = wrm.sum() 
+    wrms = wrm.sum()
     # clds signal
-    cld = np.minimum(err_sk, 0) 
+    cld = np.minimum(err_sk, 0)
     cld *= -receptor
     clds = cld.sum()
 
     return wrms, clds
 
 
 # Antoine equation [kPa]
 antoine = lambda x: math.e**(16.6536-(4030.183/(x+235)))
 # Tetens equation [kPa]
 tetens = lambda x: 0.61078*10**(7.5*x/(x+237.3))
 
 
-def evaporation(err_cr, err_sk, tsk, ta, rh, ret, 
+def evaporation(err_cr, err_sk, tsk, ta, rh, ret,
                 height=1.72, weight=74.43, equation="dubois", age=20):
     """
     Calculate evaporative heat loss.
 
     Parameters
     ----------
     err_cr, err_sk : array
@@ -343,15 +354,15 @@
     wet = 0.06 + 0.94*(e_sweat/e_max)
     wet = np.minimum(wet, 1)  # Wettedness' upper limit
     e_sk = wet * e_max
     e_sweat = (wet - 0.06) / 0.94 * e_max  # Effective sweating
     return wet, e_sk, e_max, e_sweat
 
 
-def skin_bloodflow(err_cr, err_sk, 
+def skin_bloodflow(err_cr, err_sk,
         height=1.72, weight=74.43, equation="dubois", age=20, ci=2.59,):
     """
     Calculate skin blood flow rate (BFsk) [L/h].
 
     Parameters
     ----------
     err_cr, err_sk : array
@@ -409,24 +420,24 @@
                 0.31, 0.31, 0.31, 0.31, 0.31, 0.31,
                 ])
         sd_stric = np.ones(17)
 
     #皮膚血流量 [L/h]
     bf_sk = (1 + skin_dilat * sd_dilat * sig_dilat) / \
             (1 + skin_stric * sd_stric * sig_stric) * bfb_sk * 2**(err_sk/6)
-    
+
     bfbr = cons.bfb_rate(height, weight, equation, age, ci,)
     bf_sk *= bfbr
     return bf_sk
 
 
-def ava_bloodflow(err_cr, err_sk, 
+def ava_bloodflow(err_cr, err_sk,
         height=1.72, weight=74.43, equation="dubois", age=20, ci=2.59,):
     """
-    Calculate areteriovenous anastmoses (AVA) blood flow rate [L/h] based on 
+    Calculate areteriovenous anastmoses (AVA) blood flow rate [L/h] based on
     Takemori's model, 1995.
 
     Parameters
     ----------
     err_cr, err_sk : array
         Difference between setpoint and body temperatures [oC].
     height : float, optional
@@ -452,16 +463,16 @@
     err_bcr = np.average(err_cr[2:5], weights=cap_bcr)
 
     # Cal. mean error skin temp.
     bsa = _BSAst
     err_msk = np.average(err_sk, weights=bsa)
 
     # Openbess of AVA [-]
-    sig_ava_hand = 0.265 * (err_bcr + 0.43) + 0.953 * (err_msk + 0.1905) + 0.9126
-    sig_ava_foot = 0.265 * (err_bcr - 0.97) + 0.953 * (err_msk - 0.0095) + 0.9126
+    sig_ava_hand = 0.265 * (err_msk + 0.43) + 0.953 * (err_bcr + 0.1905) + 0.9126
+    sig_ava_foot = 0.265 * (err_msk - 0.997) + 0.953 * (err_bcr + 0.0095) + 0.9126
 
     sig_ava_hand = min(sig_ava_hand, 1)
     sig_ava_hand = max(sig_ava_hand, 0)
     sig_ava_foot = min(sig_ava_foot, 1)
     sig_ava_foot = max(sig_ava_foot, 0)
 
     bfbr = bfbr = cons.bfb_rate(height, weight, equation, age, ci,)
@@ -600,15 +611,15 @@
 
 PRE_SHIV = 0
 def shivering(err_cr, err_sk, tcr, tsk,
               height=1.72, weight=74.43, equation="dubois", age=20, sex="male", dtime=60,
               options={}):
     """
     Calculate local metabolic rate by shivering [W].
-    
+
     Parameters
     ----------
     err_cr, err_sk : array
         Difference between setpoint and body temperatures [oC].
     tcr, tsk : array
         Core and skin temperatures [oC].
     height : float, optional
@@ -626,15 +637,15 @@
         Interval of analysis time. The default is 60.
 
     Returns
     -------
     Mshiv : array
         Local metabolic rate by shivering [W].
 
-    """    
+    """
     wrms, clds = error_signals(err_cr, err_sk,)
     shivf = np.array([
             0.0339, 0.0436, 0.27394, 0.24102, 0.38754,
             0.00243, 0.00137, 0.0002, 0.00243, 0.00137, 0.0002,
             0.0039, 0.00175, 0.00035, 0.0039, 0.00175, 0.00035,])
     sig_shiv = 24.36 * clds * (-err_cr[0])
     sig_shiv = max(sig_shiv, 0)
```

