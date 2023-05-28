# Comparing `tmp/adbkit-0.17.tar.gz` & `tmp/adbkit-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbkit-0.17.tar", last modified: Fri Mar 10 16:26:40 2023, max compression
+gzip compressed data, was "adbkit-0.18.tar", last modified: Sun May 28 07:49:29 2023, max compression
```

## Comparing `adbkit-0.17.tar` & `adbkit-0.18.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-10 16:26:40.122275 adbkit-0.17/
--rw-rw-rw-   0        0        0     1148 2023-03-10 16:25:34.000000 adbkit-0.17/LICENSE.rst
--rw-rw-rw-   0        0        0      113 2023-03-10 16:25:33.000000 adbkit-0.17/MANIFEST.in
--rw-rw-rw-   0        0        0   161917 2023-03-10 16:26:40.122275 adbkit-0.17/PKG-INFO
--rw-rw-rw-   0        0        0   160032 2023-03-10 16:23:20.000000 adbkit-0.17/README.md
-drwxrwxrwx   0        0        0        0 2023-03-10 16:26:40.117276 adbkit-0.17/adbkit/
--rw-rw-rw-   0        0        0     1090 2022-10-05 20:27:47.000000 adbkit-0.17/adbkit/LICENSE
--rw-rw-rw-   0        0        0   160032 2023-03-10 16:23:20.000000 adbkit-0.17/adbkit/README.MD
--rw-rw-rw-   0        0        0   123316 2023-03-10 16:17:36.000000 adbkit-0.17/adbkit/__init__.py
--rw-rw-rw-   0        0        0      648 2023-03-10 16:26:38.000000 adbkit-0.17/adbkit/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-03-10 16:26:38.000000 adbkit-0.17/adbkit/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-03-10 16:26:40.121275 adbkit-0.17/adbkit.egg-info/
--rw-rw-rw-   0        0        0   161917 2023-03-10 16:26:39.000000 adbkit-0.17/adbkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-03-10 16:26:40.000000 adbkit-0.17/adbkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-10 16:26:39.000000 adbkit-0.17/adbkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      616 2023-03-10 16:26:39.000000 adbkit-0.17/adbkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-10 16:26:39.000000 adbkit-0.17/adbkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-03-10 16:26:40.123300 adbkit-0.17/setup.cfg
--rw-rw-rw-   0        0        0     2791 2023-03-10 16:26:38.000000 adbkit-0.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 07:49:29.310506 adbkit-0.18/
+-rw-rw-rw-   0        0        0     1148 2023-05-28 07:48:50.000000 adbkit-0.18/LICENSE.rst
+-rw-rw-rw-   0        0        0       89 2023-05-28 07:48:49.000000 adbkit-0.18/MANIFEST.in
+-rw-rw-rw-   0        0        0   161921 2023-05-28 07:49:29.311455 adbkit-0.18/PKG-INFO
+-rw-rw-rw-   0        0        0   160268 2023-05-28 07:38:39.000000 adbkit-0.18/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 07:49:29.306602 adbkit-0.18/adbkit/
+-rw-rw-rw-   0        0        0   160268 2023-05-28 07:38:39.000000 adbkit-0.18/adbkit/README.MD
+-rw-rw-rw-   0        0        0   129534 2023-05-28 07:33:33.000000 adbkit-0.18/adbkit/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-28 07:49:28.000000 adbkit-0.18/adbkit/requirements.txt
+-rw-rw-rw-   0        0        0   340479 2023-05-28 07:49:28.000000 adbkit-0.18/adbkit/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-28 07:49:29.309502 adbkit-0.18/adbkit.egg-info/
+-rw-rw-rw-   0        0        0   161921 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      651 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 07:49:29.000000 adbkit-0.18/adbkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-28 07:49:29.312430 adbkit-0.18/setup.cfg
+-rw-rw-rw-   0        0        0     2785 2023-05-28 07:49:28.000000 adbkit-0.18/setup.py
```

### Comparing `adbkit-0.17/LICENSE.rst` & `adbkit-0.18/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adbkit-0.17/PKG-INFO` & `adbkit-0.18/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,1031 +1,1041 @@
-Metadata-Version: 2.1
-Name: adbkit
-Version: 0.17
-Summary: Big automation package for ADB
-Home-page: https://github.com/hansalemaos/adbkit
-Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
-License: MIT
-Keywords: adb,android,automation,shell,root
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
-# Easier ADB automation 
-
-## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
-
-### pip install adbkit
-
-**Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
-
-**10/03/2023: Tesseract with multiprocessing / Bluestacks Hyper-V connect** 
-
-```python
-# Connects to all Bluestacks Hyper-V devices (dynamic ADB ports)  and returns a DataFrame 
-from adbkit import ADBTools
-ald=ADBTools.connect_to_all_bluestacks_hyperv_devices(    adb_path="C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
-timeout=10,
-bluestacks_config=r"C:\ProgramData\BlueStacks_nxt\bluestacks.conf",)
-
-# Tesseract OCR on all found elements - multiprocessing 
-adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
-deviceserial = "localhost:52249"
-self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
-self.aa_connect_to_device()
-self.aa_activate_tesseract(
-    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
-)
-self.aa_update_screenshot()
-df=self.aa_get_all_displayed_items_from_uiautomator(
-	screenshotfolder="f:\\compare_android2",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
-
-
-      bb_area  bb_bounds  bb_center_x  bb_center_x_cropped  bb_center_y  bb_center_y_cropped  bb_checkable  bb_checked   bb_class  bb_clickable bb_content_desc  bb_cropped_x_end  bb_cropped_x_start  bb_cropped_y_end  bb_cropped_y_start  bb_enabled  bb_focusable  bb_focused  bb_height  bb_height_cropped  bb_index bb_keys_hierarchy  bb_long_clickable  bb_old_index bb_package  bb_password bb_pure_id bb_resource_id bb_screenshot  bb_scrollable  bb_selected bb_shapely    bb_text  bb_valid_square  bb_width  bb_width_cropped  bb_x_end  bb_x_start  bb_y_end  bb_y_start ee_bb_longtouch ee_bb_longtouch_bs ee_bb_longtouch_offset ee_bb_longtouch_offset_bs ee_bb_touch ee_bb_touch_bs ee_bb_touch_offset ee_bb_touch_offset_bs ff_bb_downswipe ff_bb_save_screenshot ff_bb_show_screenshot ff_bb_tap_center_offset ff_bb_tap_center_offset_long ff_bb_tap_center_variation ff_bb_tap_center_variation_long ff_bb_tap_exact_center ff_bb_tap_exact_center_long ff_bb_upswipe bb_scanned_text
-0   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0    (node,)             False                  0     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-1   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  1     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-2   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  2     com.bl...      False    id/con...  androi...      [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-3   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  3     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-4   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  4     com.bl...      False    id/dra...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-5   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  5     com.bl...      False    id/ite...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-6   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  6     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-7   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 1  (node,...             False                  7     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-8    771120.0  (44, 8...        800          800                  335          335                False         False     a.q.a.b      False                          1556                44                 590                80                True        True         False         510        510                 0  (node,...             False                  8     com.bl...      False    id/des...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
-9    281464.0  (196, ...        800          800                  783          783                False         False   androi...      False                          1404               196                 900               667                True       False         False         233        233                 3  (node,...             False                  9     com.bl...      False      id/dock  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        667          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
-10   771120.0  (44, 8...        800          800                  335          335                False         False   androi...      False                          1556                44                 590                80                True       False         False         510        510                 0  (node,...             False                 10     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
-11    21744.0  (196, ...        800          800                  685          685                False         False   androi...      False                          1404               196                 694               676                True       False         False          18         18                 0  (node,...             False                 11     com.bl...      False    id/pop...  com.bl...      [[[35,...         False          False    POLYGO...  JOGOS ...       True            1208       1208             1404        196        694        676          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     JOGOS ...     
-12   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 1  (node,...             False                 12     com.bl...      False    id/fra...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
-13    42840.0  (44, 8...        170          170                  165          165                False         False   androi...       True                           296                44                 250                80                True        True         False         170        170                 0  (node,...              True                 13     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              296         44        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Play S...     
-14    42840.0  (296, ...        422          422                  165          165                False         False   androi...       True                           548               296                 250                80                True        True         False         170        170                 1  (node,...              True                 14     com.bl...      False         <NA>                 [[[36,...         False          False    POLYGO...                  True             252        252              548        296        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Centra...     
-15    42840.0  (548, ...        674          674                  165          165                False         False   androi...       True                           800               548                 250                80                True        True         False         170        170                 2  (node,...              True                 15     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              800        548        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Ga ...     
-16    42840.0  (800, ...        926          926                  165          165                False         False   androi...       True                          1052               800                 250                80                True        True         False         170        170                 3  (node,...              True                 16     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1052        800        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Jogue ...     
-17    42840.0  (1052,...       1178         1178                  165          165                False         False   androi...       True                          1304              1052                 250                80                True        True         False         170        170                 4  (node,...              True                 17     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1304       1052        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     IMEI/P...     
-18    42840.0  (1304,...       1430         1430                  165          165                False         False   androi...       True                          1556              1304                 250                80                True        True         False         170        170                 5  (node,...              True                 18     com.bl...      False         <NA>                 [[[38,...         False          False    POLYGO...                  True             252        252             1556       1304        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     SocksD...     
-19   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 0  (node,...             False                 19     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
-20   140128.0  (196, ...        800          800                  842          842                False         False   androi...      False                          1404               196                 900               784                True       False         False         116        116                 1  (node,...             False                 20     com.bl...      False    id/vie...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        784          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-21   197288.0  (258, ...        800          800                  785          785                False         False   androi...      False                          1342               258                 876               694                True       False         False         182        182                 0  (node,...             False                 21     com.bl...      False    id/all...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1084       1084             1342        258        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     a 2e4 ...     
-22    28938.0  (324, ...        403          403                  785          785                False         False   androi...       True                           483               324                 876               694                True        True         False         182        182                 0  (node,...             False                 22     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              483        324        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
-23    28938.0  (483, ...        562          562                  785          785                False         False   androi...       True                           642               483                 876               694                True        True         False         182        182                 1  (node,...             False                 23     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              642        483        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Ly m V...     
-24    28938.0  (642, ...        721          721                  785          785                False         False   androi...       True                           801               642                 876               694                True        True         False         182        182                 2  (node,...             False                 24     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              801        642        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-25    28938.0  (801, ...        880          880                  785          785                False         False   androi...       True                           960               801                 876               694                True        True         False         182        182                 3  (node,...             False                 25     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              960        801        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
-26    28756.0  (960, ...       1039         1039                  785          785                False         False   androi...       True                          1118               960                 876               694                True        True         False         182        182                 4  (node,...             False                 26     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1118        960        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
-27    28756.0  (1118,...       1197         1197                  785          785                False         False   androi...       True                          1276              1118                 876               694                True        True         False         182        182                 5  (node,...             False                 27     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1276       1118        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
-28    10000.0  (353, ...        403          403                  770          770                False         False   androi...      False                           453               353                 820               720                True       False         False         100        100                 0  (node,...             False                 28     com.bl...      False    id/app...  com.bl...      [[[44,...         False          False    POLYGO...                  True             100        100              453        353        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-29     7632.0  (324, ...        403          403                  852          852                False         False   androi...      False                           483               324                 876               828                True       False         False          48         48                 1  (node,...             False                 29     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Street...       True             159        159              483        324        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
-30    10000.0  (512, ...        562          562                  770          770                False         False   androi...      False                           612               512                 820               720                True       False         False         100        100                 0  (node,...             False                 30     com.bl...      False    id/app...  com.bl...      [[[46,...         False          False    POLYGO...                  True             100        100              612        512        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()       a wings     
-31     7632.0  (483, ...        562          562                  852          852                False         False   androi...      False                           642               483                 876               828                True       False         False          48         48                 1  (node,...             False                 31     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Viking...       True             159        159              642        483        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Viking...     
-32    10000.0  (671, ...        721          721                  770          770                False         False   androi...      False                           771               671                 820               720                True       False         False         100        100                 0  (node,...             False                 32     com.bl...      False    id/app...  com.bl...      [[[182...         False          False    POLYGO...                  True             100        100              771        671        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-33     7632.0  (642, ...        721          721                  852          852                False         False   androi...      False                           801               642                 876               828                True       False         False          48         48                 1  (node,...             False                 33     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Draken...       True             159        159              801        642        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Draken...     
-34    10000.0  (830, ...        880          880                  770          770                False         False   androi...      False                           930               830                 820               720                True       False         False         100        100                 0  (node,...             False                 34     com.bl...      False    id/app...  com.bl...      [[[184...         False          False    POLYGO...                  True             100        100              930        830        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-35     7632.0  (801, ...        880          880                  852          852                False         False   androi...      False                           960               801                 876               828                True       False         False          48         48                 1  (node,...             False                 35     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  War Ro...       True             159        159              960        801        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
-36    10000.0  (989, ...       1039         1039                  770          770                False         False   androi...      False                          1089               989                 820               720                True       False         False         100        100                 0  (node,...             False                 36     com.bl...      False    id/app...  com.bl...      [[[243...         False          False    POLYGO...                  True             100        100             1089        989        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-37     7584.0  (960, ...       1039         1039                  852          852                False         False   androi...      False                          1118               960                 876               828                True       False         False          48         48                 1  (node,...             False                 37     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Warspe...       True             158        158             1118        960        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
-38    10000.0  (1147,...       1197         1197                  770          770                False         False   androi...      False                          1247              1147                 820               720                True       False         False         100        100                 0  (node,...             False                 38     com.bl...      False    id/app...  com.bl...      [[[59,...         False          False    POLYGO...                  True             100        100             1247       1147        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-39     7584.0  (1118,...       1197         1197                  852          852                False         False   androi...      False                          1276              1118                 876               828                True       False         False          48         48                 1  (node,...             False                 39     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Dark O...       True             158        158             1276       1118        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
-40      529.0  (745, ...        756          756                  734          734                False         False   androi...      False                           768               745                 746               723                True       False         False          23         23                 0  (node,...             False                 40     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23              768        745        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-41      529.0  (1221,...       1232         1232                  734          734                False         False   androi...      False                          1244              1221                 746               723                True       False         False          23         23                 0  (node,...             False                 41     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23             1244       1221        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-
-
-
-
-
-self.aa_update_screenshot()
-df = self.aa_get_all_displayed_items_from_activities(
-	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-dftesser=self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
-
-
-      aa_area  aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text
-0       529.0  (427, ...        438          438                  734          734            androi...         False          ...            False                  450               427                 746               723                12     True       True      False         True            c741e85       208936581              23         23          app:id...              True        False          7f08011e  213123...         29        False               True               False            False             True                False                      False               False         id/pop...  [[[103...         False                    False              POLYGO...       True                I           23         23              450         97               427          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              28          27          26          24          22          20           6           5           4           3           2           0                 
-1       529.0  (586, ...        597          597                  734          734            androi...         False          ...            False                  609               586                 746               723                12     True       True      False         True            e9bb4da       245085402              23         23          app:id...              True        False          7f080121  213123...         33        False               True               False            False             True                False                      False               False         id/pop...  [[[187...         False                    False              POLYGO...       True                I           23         23              609         97               586          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              32          31          26          24          22          20           6           5           4           3           2           0                 
-2       529.0  (745, ...        756          756                  734          734            androi...         False          ...            False                  768               745                 746               723                12     True       True      False         True            5a48615        94668309              23         23          app:id...              True        False          7f080120  213123...         37        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23              768         97               745          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              36          35          26          24          22          20           6           5           4           3           2           0                 
-3       529.0  (904, ...        915          915                  734          734            androi...         False          ...            False                  927               904                 746               723                12     True       True      False         True            4029d0b        67280139              23         23          app:id...              True        False          7f08011d  213123...         41        False               True               False            False             True                False                      False               False         id/pop...  [[[255...         False                    False              POLYGO...       True                I           23         23              927         97               904          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              40          39          26          24          22          20           6           5           4           3           2           0                 
-4       529.0  (1063,...       1074         1074                  734          734            androi...         False          ...            False                 1086              1063                 746               723                12     True       True      False         True            27867e8        41445352              23         23          app:id...              True        False          7f08011c  213123...         45        False               True               False            False             True                False                      False               False         id/pop...  [[[65,...         False                    False              POLYGO...       True                I           23         23             1086         97              1063          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              44          43          26          24          22          20           6           5           4           3           2           0                 
-5       529.0  (1221,...       1232         1232                  734          734            androi...         False          ...            False                 1244              1221                 746               723                12     True       True      False         True            125ad2a        19246378              23         23          app:id...              True        False          7f08011f  213123...         49        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23             1244         97              1221          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              48          47          26          24          22          20           6           5           4           3           2           0                 
-6     10000.0  (353, ...        403          403                  770          770            androi...         False          ...            False                  453               353                 820               720                11    False       True      False         True            29caf0f        43822863             100        100          app:id...              True        False          7f080058  213123...         28        False              False               False            False            False                False                      False               False         id/app...  [[[44,...         False                    False              POLYGO...       True                V          100        100              453        129               353          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>                 
-7      7632.0  (324, ...        403          403                  852          852            androi...         False          ...            False                  483               324                 876               828                11     True       True      False         True            ea74b9c       245844892              48         48          app:id...              True        False          7f080060  213123...         30        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              483        159               324           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>   Street...     
-8     10000.0  (512, ...        562          562                  770          770            androi...         False          ...            False                  612               512                 820               720                11    False       True      False         True            cece9a5       216852901             100        100          app:id...              True        False          7f08005b  213123...         32        False              False               False            False            False                False                      False               False         id/app...  [[[46,...         False                    False              POLYGO...       True                V          100        100              612        129               512          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>     a wings     
-9      7632.0  (483, ...        562          562                  852          852            androi...         False          ...            False                  642               483                 876               828                11     True       True      False         True            aadf17a       179171706              48         48          app:id...              True        False          7f080063  213123...         34        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              642        159               483           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>   Viking...     
-10    10000.0  (671, ...        721          721                  770          770            androi...         False          ...            False                  771               671                 820               720                11    False       True      False         True            9ff2d2b       167718187             100        100          app:id...              True        False          7f08005a  213123...         36        False              False               False            False            False                False                      False               False         id/app...  [[[182...         False                    False              POLYGO...       True                V          100        100              771        129               671          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>                 
-11     7632.0  (642, ...        721          721                  852          852            androi...         False          ...            False                  801               642                 876               828                11     True       True      False         True            bab8588       195790216              48         48          app:id...              True        False          7f080062  213123...         38        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              801        159               642           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>   Draken...     
-12    10000.0  (830, ...        880          880                  770          770            androi...         False          ...            False                  930               830                 820               720                11    False       True      False         True            9e77b21       166165281             100        100          app:id...              True        False          7f080057  213123...         40        False              False               False            False            False                False                      False               False         id/app...  [[[184...         False                    False              POLYGO...       True                V          100        100              930        129               830          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>                 
-13     7632.0  (801, ...        880          880                  852          852            androi...         False          ...            False                  960               801                 876               828                11     True       True      False         True            b99ab46       194620230              48         48          app:id...              True        False          7f08005f  213123...         42        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              960        159               801           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>   War Ro...     
-14    10000.0  (989, ...       1039         1039                  770          770            androi...         False          ...            False                 1089               989                 820               720                11    False       True      False         True             c17107        12677383             100        100          app:id...              True        False          7f080056  213123...         44        False              False               False            False            False                False                      False               False         id/app...  [[[243...         False                    False              POLYGO...       True                V          100        100             1089        129               989          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>                 
-15     7584.0  (960, ...       1039         1039                  852          852            androi...         False          ...            False                 1118               960                 876               828                11     True       True      False         True            5377234        87519796              48         48          app:id...              True        False          7f08005e  213123...         46        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1118        158               960           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>   Warspe...     
-16    10000.0  (1147,...       1197         1197                  770          770            androi...         False          ...            False                 1247              1147                 820               720                11    False       True      False         True            59fa85d        94349405             100        100          app:id...              True        False          7f080059  213123...         48        False              False               False            False            False                False                      False               False         id/app...  [[[59,...         False                    False              POLYGO...       True                V          100        100             1247        129              1147          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>                 
-17     7584.0  (1118,...       1197         1197                  852          852            androi...         False          ...            False                 1276              1118                 876               828                11     True       True      False         True            f3535d2       255145426              48         48          app:id...              True        False          7f080061  213123...         50        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1276        158              1118           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>   Dark O...     
-18    30210.0  (324, ...        403          403                  781          781            androi...          True          ...            False                  483               324                 876               686                10    False       True       True         True            18369ed        25389549             190        190          app:id...              True        False          7f080050  213123...         27        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              483        225               324          66                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Street...     
-19    30210.0  (483, ...        562          562                  781          781            androi...          True          ...            False                  642               483                 876               686                10    False       True       True         True            9888022       159940642             190        190          app:id...              True        False          7f080053  213123...         31        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              642        384               483         225                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Ly m V...     
-20    30210.0  (642, ...        721          721                  781          781            androi...          True          ...            False                  801               642                 876               686                10    False       True       True         True            2751ab3        41228979             190        190          app:id...              True        False          7f080052  213123...         35        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              801        543               642         384                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   i Drak...     
-21    30210.0  (801, ...        880          880                  781          781            androi...          True          ...            False                  960               801                 876               686                10    False       True       True         True            3711870        57743472             190        190          app:id...              True        False          7f08004f  213123...         39        False              False               False            False            False                False                      False               False         id/app...  [[[87,...         False                    False              POLYGO...       True                V          159        159              960        702               801         543                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   War Ro...     
-22    30020.0  (960, ...       1039         1039                  781          781            androi...          True          ...            False                 1118               960                 876               686                10    False       True       True         True            339b7e9        54114281             190        190          app:id...              True        False          7f08004e  213123...         43        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1118        860               960         702                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Warspe...     
-23    30020.0  (1118,...       1197         1197                  781          781            androi...          True          ...            False                 1276              1118                 876               686                10    False       True       True         True            cd27c6e       215121006             190        190          app:id...              True        False          7f080051  213123...         47        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1276       1018              1118         860                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Dark O...     
-24      900.0  (785, ...        800          800                  797          797            androi...         False          ...            False                  815               785                 812               782                 9     True       True      False         True            268c7fc        40421372              30         30          app:id...              True        False          7f0800a8  213123...         25        False              False               False            False             True                False                      False               False         id/doc...  [[[35,...         False                    False              POLYGO...       True                G           30         30              815        619               785         589                812        118               782          88                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
-25   205960.0  (258, ...        800          800                  781          781            androi...         False          ...            False                 1342               258                 876               686                 9    False       True      False         True            8a2d3cc       144888780             190        190          app:id...              True        False          7f080048  213123...         26        False              False               False            False            False                False                      False               False         id/all...  [[[35,...         False                    False              POLYGO...       True                V         1084       1084             1342       1146               258          62                876        182               686          -8                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>   Street...     
-26    51579.0  (31, 6...        812          812                   78           78            androi...          True          ...            False                 1594                31                  95                62                 9     True       True       True         True            b601a94       190847636              33         33          app:id...              True        False          7f0800c6  213123...         54        False               True               False            False             True                False                      False               False         id/gro...  [[[35,...         False                    False              POLYGO...       True                V         1563       1563             1594       1588                31          25                 95         53                62          20                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
-27  1179406.0  (43, 9...        800          800                  484          484            com.bl...         False          ...            False                 1557                43                 874                95                 9     True       True      False         True            27c993d        41720125             779        779          app:id...              True        False          7f0800c3  213123...         55        False               True               False            False             True                False                      False               False          id/group  [[[35,...         False                    False              POLYGO...       True                V         1514       1514             1557       1551                43          37                874        832                95          53                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>   Ga u i...     
-28    42840.0  (296, ...        422          422                  165          165            com.bl...          True          ...            False                  548               296                 250                80                 8     True       True       True         True              d801f          884767             170        170               <NA>              True         True              <NA>       <NA>         10        False              False               False            False            False                False                      False               False              <NA>  [[[36,...         False                    False              POLYGO...       True                V          252        252              548        504               296         252                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Centra...     
-29    42840.0  (44, 8...        170          170                  165          165            com.bl...          True          ...            False                  296                44                 250                80                 8     True       True       True         True            9c32f6c       163786604             170        170               <NA>              True         True              <NA>       <NA>         11        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              296        252                44           0                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Play S...     
-30    42840.0  (800, ...        926          926                  165          165            com.bl...          True          ...            False                 1052               800                 250                80                 8     True       True       True         True            a164935       169232693             170        170               <NA>              True         True              <NA>       <NA>         12        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1052       1008               800         756                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Jogue ...     
-31    42840.0  (1052,...       1178         1178                  165          165            com.bl...          True          ...            False                 1304              1052                 250                80                 8     True       True       True         True            9c981ca       164200906             170        170               <NA>              True         True              <NA>       <NA>         13        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1304       1260              1052        1008                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   IMEI/P...     
-32    42840.0  (548, ...        674          674                  165          165            com.bl...          True          ...            False                  800               548                 250                80                 8     True       True       True         True            c93ff3b       211025723             170        170               <NA>              True         True              <NA>       <NA>         14        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              800        756               548         504                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   as Ga ...     
-33    42840.0  (1304,...       1430         1430                  165          165            com.bl...          True          ...            False                 1556              1304                 250                80                 8     True       True       True         True            569d658        90822232             170        170               <NA>              True         True              <NA>       <NA>         15        False              False               False            False            False                False                      False               False              <NA>  [[[38,...         False                    False              POLYGO...       True                V          252        252             1556       1512              1304        1260                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   SocksD...     
-34   140128.0  (196, ...        800          800                  842          842            androi...         False          ...            False                 1404               196                 900               784                 8     True       True      False         True            d395417       221860887             116        116          app:id...              True        False          7f08017f  213123...         23        False              False               False            False            False                False                      False               False         id/vie...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               784          90                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>                 
-35   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 8    False       True      False         True            9d20004       164757508             206        206               <NA>              True        False              <NA>       <NA>         24        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               694           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
-36  1352976.0  (6, 42...        800          800                  468          468            androi...         False          ...            False                 1594                 6                 894                42                 8    False       True      False         True            ebbfee7       247201511             852        852               <NA>              True        False              <NA>       <NA>         53        False               True               False            False             True                False                      False               False              <NA>  [[[39,...         False                    False              POLYGO...       True                V         1588       1588             1594       1594                 6           6                894        858                42           6                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   a | | ...     
-37   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 7     True       True      False         True             49b71b         4831003             510        510               <NA>              True        False              <NA>       <NA>          9        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1512                44           0                590        510                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
-38      225.0  (726, ...        733          733                  620          620            androi...         False          ...            False                  741               726                 628               613                 7     True       True      False         True            1b8c9ce        28887502              15         15          app:id...              True        False          7f0800ef  213123...         18        False               True               False            False             True                False                      False               False         id/loa...  [[[35,...         False                    False              POLYGO...       True                V           15         15              741         25               726          10                628         22               613           7                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
-39     2604.0  (751, ...        813          813                  620          620            androi...         False          ...            False                  875               751                 631               610                 7     True       True      False         True            c7ee0ef       209641711              21         21          app:id...              True        False          7f0800dc  213123...         19        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                V          124        124              875        159               751          35                631         25               610           4                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
-40    21744.0  (196, ...        800          800                  685          685            androi...         False          ...            False                 1404               196                 694               676                 7     True       True      False         True            d6f43b1       225395633              18         18          app:id...              True        False          7f08011b  213123...         21        False              False               False            False            False                False                      False               False         id/pop...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                694         27               676           9                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   JOGOS ...     
-41   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 7    False       True      False         True            ae5f096       182841494             206        206          app:id...              True        False          7f0800bd  213123...         22        False              False               False            False            False                False                      False               False         id/fra...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        233               694          27                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
-42  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 7    False       True      False         True            69044a6       110118054             864        864               <NA>              True        False              <NA>       <NA>         52        False               True               False            False             True                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-43  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 6    False       True      False         True            46dee93        74313363             864        864          app:id...              True        False          7f08006c  213123...          7        False              False               False            False             True                False                      False               False         id/bac...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-44   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 6     True       True       True         True            6affac3       112196291             510        510          app:id...              True        False          7f08009e  213123...          8        False              False               False            False            False                False                      False               False         id/des...  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1556                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
-45    25600.0  (0, 59...        800          800                  598          598            com.bl...         False          ...            False                 1600                 0                 606               590                 6     True       True      False         True            a318ed0       171019984              16         16          app:id...              True        False          7f08009f  213123...         16        False               True               False            False             True                False                      False               False         id/des...  [[[28,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                606        570               590         554                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-46     5070.0  (716, ...        800          800                  621          621            androi...         False          ...            False                  885               716                 636               606                 6    False       True      False         True            57d5ec9        92102345              30         30          app:id...              True        False          7f0800db  213123...         17        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                I          169        169              885        885               716         716                636        600               606         570                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-47   281464.0  (196, ...        800          800                  783          783            androi...         False          ...            False                 1404               196                 900               667                 6    False       True      False         True            d275f40       220684096             233        233          app:id...              True        False          7f0800a7  213123...         20        False              False               False            False            False                False                      False               False           id/dock  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1404               196         196                900        864               667         631                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Street...     
-48  1382400.0  (0, 36...        800          800                  468          468            com.bl...          True          ...            False                 1600                 0                 900                36                 6    False       True       True         True            25d1e01        39656961             864        864          app:id...              True        False          7f0800c4  213123...         51        False               True               False            False             True                False                      False               False         id/gro...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-49    19380.0  (44, 8...         63           63                  335          335            androi...         False          ...            False                   82                44                 590                80                 6     True       True      False         True            4493e79        71908985             510        510          app:id...              True        False          7f0800e5  213123...         56        False              False               False            False            False                False                      False               False         id/lef...  [[[35,...         False                    False              POLYGO...       True                V           38         38               82         82                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-50    19380.0  (1518,...       1537         1537                  335          335            androi...         False          ...            False                 1556              1518                 590                80                 6     True       True      False         True            ecea7be       248424382             510        510          app:id...              True        False          7f08012e  213123...         57        False              False               False            False            False                False                      False               False         id/rig...  [[[37,...         False                    False              POLYGO...       True                V           38         38             1556       1556              1518        1518                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-51  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 5    False       True      False         True            294a77d        43296637             864        864               <NA>              True        False              <NA>       <NA>          6        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-52  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 5     True       True      False         True            c019672       201430642             864        864               <NA>              True        False              <NA>       <NA>         58        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-53  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 4     True       True      False         True            38d79ff        59603455             864        864          app:id...              True        False          7f0800df  213123...          5        False              False               False            False            False                False                      False               False         id/ite...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-54  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 3    False       True       True         True            d8cdd1e       227335454             864        864          app:id...              True        False          7f0800b1  213123...          4        False              False                True            False            False                False                      False               False         id/dra...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                36          36                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-55  1440000.0  (0, 0,...        800          800                  450          450            androi...         False        an...            False                 1600                 0                 900                 0                 2    False       True      False         True            2b36d59        45313369             900        900               <NA>              True        False              <NA>       <NA>          3        False              False               False            False            False                False                      False               False              <NA>  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
-56        0.0  (0, 0,...          0            0                    0            0            androi...         False      andr...            False                    0                 0                   0                 0                 1    False       True      False        False            812b782       135444354               0          0          androi...              True        False           102018a   16908682          1        False              False               False            False             True                False                      False               False         id/act...        NaN         False                    False              POLYGO...      False                G            0          0                0          0                 0           0                  0          0                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()            <NA>                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-57  1440000.0  (0, 0,...        800          800                  450          450            androi...         False      andr...            False                 1600                 0                 900                 0                 1    False       True      False         True            5f37da0        99843488             900        900          androi...              True        False           1020002   16908290          2        False              False               False            False            False                False                      False               False         id/con...  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
-
-```
-
-**01/03/2023: Added adbdevicechanger** 
-```python
-# https://github.com/hansalemaos/adbdevicechanger
-# tested with bluestacks - root access
-self.aa_activate_adbdevicechanger()
-self.bb_adbdevicechanger.change_android_id()
-
-b'Row: 0 _id=227, name=device_name, value=OnePlus 5T\r\n'
-Out[7]: ('f7a32086dc724a4a', 'OnePlus 5T')
-
-
-self.bb_adbdevicechanger.change_device_name(
-    modelregex=".*",
-    developerregex=".*",
-    androidfullnameregex=".*",
-    year=">1",
-    month=">0",
-    versionnumberaround=7.05,
-)
-b'Row: 0 _id=2340, name=android_id, value=f7a32086dc724a4a\r\n'
-b'Row: 0 _id=228, name=device_name, value=HTC U11\r\n'
-Out[8]: ('f7a32086dc724a4a', 'HTC U11')
-
-self.bb_adbdevicechanger.change_android_id_and_device_name(
-    modelregex=".*",
-    developerregex=".*",
-    androidfullnameregex=".*",
-    year=">1",
-    month=">0",
-    versionnumberaround=7.05,
-)
-b'Row: 0 _id=2341, name=android_id, value=fb9afc93197942d8\r\n'
-b'Row: 0 _id=229, name=device_name, value=Nokia 8\r\n'
-Out[9]: ('fb9afc93197942d8', 'Nokia 8')
-
-
-self.bb_adbdevicechanger.get_random_android_cellphones(    modelregex="Samsung.*",
-    developerregex=".*",
-    androidfullnameregex=".*",
-    year=">2010",
-    month=">0",
-    versionnumberaround=9.05,
-    howmany=10,
-    return_list=False,)
-Out[13]: 
-                       aa_model  ...              uuid
-0  Samsung Galaxy Note 20/Ultra  ...  36f8a604180b4d7f
-1            Samsung Galaxy A70  ...  cb7f374cd85d4330
-2      Samsung Galaxy A30s/A50s  ...  9380749deb5942f6
-3      Samsung Galaxy Note 10/+  ...  c36816b1906542dc
-4    Samsung Galaxy S20/+/Ultra  ...  33dc12217b404a62
-5         Samsung Galaxy A90 5G  ...  cf0084fa8261465d
-6      Samsung Galaxy A51 5G UW  ...  3177aa09b1fc40d9
-7            Samsung Galaxy A01  ...  44db6d59366143cd
-8         Samsung Galaxy A42 5G  ...  a5b6fb2d08ac4475
-9           Samsung Galaxy A20e  ...  806b4ae287ec4d34
-[10 rows x 10 columns]
-
-```
-
-
-**23/02/2023: New methods**
-```python
-from adbkit import ADBTools
-adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
-deviceserial = "localhost:5555"
-self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
-self.aa_connect_to_device()
-self.aa_activate_tesseract(
-    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
-)
-
-#####################################################################################
-# This method uses Tesseract! You can download it here: https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
-self.aa_update_screenshot() # Update the screenshot before 
-df=self.aa_ocr_elements_from_activities(['Play Store'], # pass all strings as a list 
-minpercentage=85, # fuzzy match
-maxtolerance=10,
-screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-
-    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
-32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
-
-
-
-#####################################################################################
-# Another example (Play Store written wrong)
-
-df2=self.aa_ocr_elements_from_uiautomator(['blai Store'],minpercentage=70, maxtolerance=10, )
-
-    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
-32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
-
-#####################################################################################
-# Pass a list of tuples:
-((x,y),time in seconds)
-
-self.aa_multi_input_tap_with_delay([((100,100),2), ((200,200),3)])
-#####################################################################################
-
-self.aa_input_tap(x=100,y=100)
-
-#####################################################################################
-# https://github.com/hansalemaos/adbescapes
-# Converts Unicode string to ASCII and escapes all characters that need to be escaped. 
-# You have to activate it, before using it. The first start takes some time because numba needs to compile the code 
-self.aa_activate_input_text_formated()
-
-# input 
-text="""
-"'ąćęłń'\tóśźż\nĄĆĘŁŃÓŚŹŻ\n\"Junto à Estação de \nCarcavelos;\"" "äöüÄÖÜß"
-"""
-self.aa_input_text_formated_with_delay(text,delay=(0.01, 0.2),respect_german_letters=False, exit_keys="ctrl+x")
-
-
-# output
-"'aceln'    oszz
-ACELNOSZZ
-"Junto a Estacao de 
-Carcavelos;"" "aouAOUb"
-
-# If you want it the German way :)
-self.aa_input_text_formated(text,respect_german_letters=True, exit_keys="ctrl+x")
-
-"'aceln'    oszz
-ACELNOSZZ
-"Junto a Estacao de 
-Carcavelos;"" "aeoeueAeOeUess"
-#####################################################################################
-self.aa_install_apk_from_hdd(r"C:\Users\Gamer\anaconda3\envs\instcont\instagram.apk")
-#####################################################################################
-self.aa_uninstall_package('com.instagram.lite')
-#####################################################################################
-# First argument is a regex 
-self.aa_copy_apk_to_hdd('com.insta.*', 'c:\\instaapkdownload')
-#####################################################################################
-```
-
-
-
-**17/01/2023: Screenshot fix**
-
-
-```python
-$pip install adbkit
-from adbkit import ADBTools
-adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
-deviceserial = "localhost:5875"
-
-# Create an instance
-# Don't get confused about the instance name "self". I did it because it is faster copying methods from the class 
-self = ADBTools(adb_path, deviceserial, sdcard="/sdcard/")
-self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
-
-# connect to the device 
-self.aa_connect_to_device()
-```
-
-
-
-```python
-# If you are using BlueStacks and want to have root access, call:
-self.aa_root_bluestacks_instances() 
-# This method will basically do this steps: https://appuals.com/root-bluestacks/ to root BlueStacks
-# You can run the script every time you use this module. It won't hurt. 
-# The first time, you might have to restart BlueStacks to enable the root access 
-```
-
-
-
-```python
-# If your device/BlueStacks is rooted, enable root so that all commands will be sent as root 
-self.aa_enable_root() 
-# can be disabled by calling :
-self.aa_disable_root()
-```
-
-
-
-```python
-# Activates self.bb_adbkeyboard 
-# Read more about it: https://github.com/hansalemaos/adb_unicode_keyboard
-self.aa_activate_adb_keyboard(exit_keys="ctrl+x") 
-```
-
-
-
-```python
-# Activates self.bb_sendevent_keyboard (needs root access)
-# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
-
-self.aa_activate_sendevent_keyboard(
-    sdcard="/storage/emulated/0/",
-    tmp_folder_on_sd_card="AUTOMAT",
-    exit_keys="ctrl+x",
-)  # needs root access
-
-# Here is one example: 
-self.bb_adbkeyboard.press_7_keycode_0()
-```
-
-
-
-```python
-# Activates self.self.bb_getevent_sendevent
-# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
-
-self.aa_activate_getevent_sendevent(
-    sdcard="/storage/emulated/0/",
-    tmp_folder_on_sd_card="AUTOMAT",
-    bluestacks_divider=32767,
-    exit_keys="ctrl+x",
-)  # needs root access
-```
-
-
-
-```python
-# Activates self.bb_sendevent_touch
-# Read more about it: https://github.com/hansalemaos/sendevent_touch
-
-self.aa_activate_sendevent_touch(
-    sdcard="/storage/emulated/0/",
-    tmp_folder_on_sd_card="AUTOMAT",
-    bluestacks_divider=32767,
-    use_bluestacks_coordinates=True,
-)  # needs root access
-
-# Here is one example:
-self.bb_sendevent_touch.touch(10,10)
-```
-
-
-
-```python
-# Activates https://github.com/hansalemaos/a_pandas_ex_tesseract_multirow_regex_fuzz
-# You can download the 64 bit version of tesseract here: 
-# https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
-
-self.aa_activate_tesseract(
-        tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
-    )
-
-# Once activated, you can call:
-# self.aa_ocr_with_tesseract()
-
-    left  top  width  height       conf        text  middle_x  middle_y  end_x  end_y
-8    382   42    499      49  37.512093         RH,       631        66    881     91
-9    728   34     98      61  30.925949          2.       777        64    826     95
-13   370  101     37      11   84.72541     'system       388       106    407    112
-14   411  101     24      10  79.929901        Apps       423       106    435    111
-15   536   90     36      28  85.425911      Roblox       554       104    572    118
-16   676  100     55       9  88.744247  BlueStacks       703       104    731    109
-17   735  101      7       8  80.470955           X       738       105    742    109
-18   814  101     31      10  90.271423      Spiele       829       106    845    111
-19   848  101     18       8  93.303749         und       857       105    866    109
-20   869  103     41       9  87.963295     gewinne       889       107    910    112
-28    72  100     20      12  96.004517        Play        82       106     92    112
-29    95  101     27       8  86.986359       Store       108       105    122    109
-33   225  211     49      12  76.804665   Globoplay       249       217    274    223
-37   326  489     25      28  91.894142       Tibia       338       503    351    517
-38   401  500     50       8  91.477989   Guardians       426       504    451    508
-39   455  499     10       9  72.064316          of       460       503    465    508
-41   415  512     37       9  75.078018     Cloudia       433       516    452    521
-
-# and even perform a multiline fuzzy search:
-xxx = self.aa_ocr_with_tesseract(search_for='Kontakte verwalten')
-```
-```python
-# Use this method to update the screenshot 
-# The updated screenshot can be found here: self.screenshot
-self.aa_update_screenshot()
-
-```
-
-
-
-```python
-# get 5 screenshot within 5 seconds
-xx=self.aa_get_screenshots(
-        sleeptime=1,
-        number=5)
-
-```
-
-
-
-```python
-# Now you can use self.df to do operations on the screenshot 
-# More information about a_pandas_ex_image_tools:
-# https://github.com/hansalemaos/a_pandas_ex_image_tools
-self.aa_update_imagedf()
-```
-
-
-```python
-# If you want to capture the logcat output and analyze it in a DataFrame,
-use: 
-logcatcap = self.aa_capture_logcat(
-        exit_keys="ctrl+x",
-        timeout=None,
-    )  
-
-# When you exit using "ctrl+x", the method will return a DataFrame
-# By the way: almost all methods can be interrupted using a key command 
-```
-
-
-
-```python
-# Those 2 methods will help you to identify and interact with views:
-# Read more about it: https://github.com/hansalemaos/androdf
-df1 = self.aa_get_all_displayed_items_from_uiautomator(
-	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-
-df3 = self.aa_get_all_displayed_items_from_activities(
-	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-```
-
-
-
-```python
-# Uses: https://github.com/hansalemaos/a_pandas_ex_adb_to_df
-# lists all files in DataFrame and adds useful functions
-# self.aa_list_all_files_on_device()
-
-dffiles = self.aa_list_folder_content(folder_to_search="data/")  
-print(dffiles)
-                  aa_date  ... ff_pull_file_cat
-0     2022-12-11 06:48:00  ...               ()
-1     2022-12-26 22:16:00  ...               ()
-2     2022-12-06 19:10:00  ...               ()
-3     2022-12-06 13:38:00  ...               ()
-4     2022-12-26 22:16:00  ...               ()
-                   ...  ...              ...
-26120 2021-09-16 04:21:00  ...               ()
-26121 2021-09-16 03:53:00  ...               ()
-26122 2021-09-16 03:53:00  ...               ()
-26123 2021-09-16 04:35:00  ...               ()
-26124 2021-09-16 04:31:00  ...               ()
-[26125 rows x 16 columns]
-```
-
-
-
-```python
-# Search with grep 
-# Uses https://github.com/hansalemaos/adb_grep_search
-dfgrep = self.aa_grep_search(
-        folder_to_search="data/data",
-        filetype="*.db",
-        regular_expression=r"CREATE.TABLE",
-        exit_keys="ctrl+x",
-        timeout=None,
-        remove_control_characters=True,
-    )
-
-dfgrep
-Out[19]: 
-                                               aa_file  ...      aa_regex
-0    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-1    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-2    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-3    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-4    data/data/com.globo.globotv/databases/mcsdk_bf...  ...  CREATE.TABLE
-..                                                 ...  ...           ...
-103  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-104  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-105  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-106  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-107  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-[108 rows x 5 columns]
-```
-
-
-
-```python
-# Uses https://github.com/hansalemaos/a_pandas_ex_adb_settings_to_df
-self.aa_parse_settings_from_all_packages(
-        tempfolder="f:\\tmpfolder", datafolder="data/"
-    )
-
-        index          aa_all_keys  ... level_22 level_23
-0         0.0         (long, name)  ...      NaN      NaN
-1         1.0        (long, value)  ...      NaN      NaN
-2         0.0   (boolean, 0, name)  ...      NaN      NaN
-3         1.0  (boolean, 0, value)  ...      NaN      NaN
-4         2.0   (boolean, 1, name)  ...      NaN      NaN
-       ...                  ...  ...      ...      ...
-110795    NaN            (6, desc)  ...      NaN      NaN
-110796    NaN           (6, label)  ...      NaN      NaN
-110797    NaN             (6, pkg)  ...      NaN      NaN
-110798    NaN          (6, source)  ...      NaN      NaN
-110799    NaN             (6, url)  ...      NaN      NaN
-[110800 rows x 31 columns]
-
-You might see this error messages several times:
-
-"Go to: https://www.sqlite.org/download.html ,
-download the dll and put it in the DLLs folder of your env!"
-
-You can ignore it.
-```
-
-
-
-```python
-#This method helps you find all executable activities from a package 
-# More about it: https://github.com/hansalemaos/a_pandas_ex_adb_execute_activities
-
-self.aa_get_activity_execution_df_from_one_package(
-        packagename="com.roblox.client"
-    ) 
-```
-
-
-
-```python
-# adds new contact, can be saved straight away
-addcon = self.aa_add_new_contact(
-	"hans", "+55119897827552", "hans@something.com", "my address", save=False
-)
-```
-
-
-
-```python
-# If you play Roblox, you can enable/disable some textures to get higher fps
-self.aa_enable_roblox_textures(
-	exit_keys="ctrl+x",
-	print_output=True,
-	timeout=None,
-)
-
-self.aa_disable_roblox_textures(
-	exit_keys="ctrl+x",
-	print_output=True,
-	timeout=None,
-)
-```
-
-
-
-```python
-# goes to the home screen, doesn't close anything
-self.aa_go_to_home_screen()
-```
-
-
-
-```python
-# repeat=5 usually deletes more than 5 characters!!
-self.aa_press_delete_key_repeated_times(repeat=5)
-```
-
-
-
-```python
-# starts the android file manager, pass the file type you want to see
-self.aa_get_content(type_="text/plain")
-```
-
-
-
-```python
-# Here are some methods to get useful information. 
-# Returns DataFrames 
-print(self.aa_whole_dumpsys_to_df())
-print(self.aa_list_all_packages())
-print(self.aa_list_broadcast_stats())
-print(self.aa_list_pending_intents())
-print(self.aa_list_all_activities_from_device())
-print(self.aa_list_all_services())
-print(self.aa_list_all_receivers())
-print(self.aa_list_all_activities())
-print(self.aa_get_procstats())
-print(self.aa_list_all_devices()) # devices on the device (dev ...)
-print(self.aa_list_devices()) # all adb devices (localhost:5555 ...)
-print(self.aa_list_pids_basic())
-print(self.aa_list_pids_complete())
-print(self.aa_list_memory())
-print(self.aa_getprop())
-print(self.aa_list_all_broadcasts())
-print(self.aa_list_all_broadcasts_history())
-print(self.aa_list_users())
-print(self.aa_list_permission_groups())
-print(self.aa_list_disabled_packages())
-print(self.aa_list_apps_in_use())
-print(self.aa_list_3rd_party_packages())
-print(self.aa_list_features())
-```
-
-
-
-```python
-# Smile! :)
-self.aa_open_camera_photo_mode()
-```
-
-
-
-```python
-# works with and without http://
-print(self.aa_open_website("google.com"))
-```
-
-
-
-```python
-# switches to gallery
-self.aa_start_gallery()
-```
-
-
-
-```python
-# cheeeese
-self.aa_take_a_picture()
-```
-
-
-
-```python
-# useful for some apps 
-self.aa_adb_turn_screen_compatibility_off()
-self.aa_adb_turn_screen_compatibility_on()
-```
-
-
-
-```python
-# Be careful! 
-self.aa_remove_file('/sdcard/9.png')
-```
-
-
-
-```python
-# Essential when you use your cell phone (with Whatsapp, Facebook ...) to automize things.
-self.aa_enable_notifications()
-self.aa_disable_notifications()
-```
-
-
-
-```python
-# More useful stuff for notifications
-self.aa_expand_settings() 
-self.aa_expand_notifications()
-```
-
-
-
-```python
-# Changes the screen orientation
-# You can pass:
-# horizontal_upside_down or 2
-# vertical or 1
-# horizontal or 0
-# vertical_upside_down or 3
-self.aa_change_screen_orientation("horizontal")
-```
-
-
-
-```python
-self.aa_get_display_orientation()
-#Out[4]: 0 
-# 0 means horizontal
-```
-
-
-
-```python
-# Sometimes you upload new media files, but you can't see the thumbnails immediately
-# This method updates all thumbnails
-self.aa_rescan_media()
-```
-
-
-
-```python
-# If you are in the middle of a text and want to go to the end of the line
-self.aa_move_to_end_of_line()
-```
-
-
-
-```python
-# Useful keyboard stuff 
-self.aa_hide_keyboard()
-self.aa_is_keyboard_shown()
-```
-
-
-
-```python
-# Doesn't work on BlueStacks, but on my pixel 6 there are no problems
-# (Actually it is not necessary when using BlueStacks hahaha)
-self.aa_is_screen_unlocked()
-```
-
-
-
-```python
-# Don't use this command on BlueStacks, you will have to reboot the device
-self.aa_lock_screen()
-```
-
-
-
-```python
-# Useful commands 
-self.aa_press_home() #back to home screen
-self.aa_press_app_switch()
-```
-
-
-
-```python
-# Configured for my Pixel 6, but should work on any device with a 
-# newer android version. 
-self.aa_swipe_up_to_unlock_screen('3333')
-```
-
-
-
-```python
-# doesn't work with BlueStacks, because of the app switch design, 
-# but it does on my pixel and should work with any device that 
-# has a recent Android version
-self.aa_close_all_apps_with_swipe()
-```
-
-
-
-```python
-# uninstalls a package
-self.aa_uninstall_package('com.google.android.youtube')
-```
-
-
-
-```python
-# Returns the activity needed to open the package 
-self.aa_resolve_activity('com.roblox.client')
-b'priority=0 preferredOrder=0 match=0x108000 specificIndex=-1 isDefault=true\r\n'
-b'com.roblox.client/.startup.ActivitySplash\r\n'
-```
-
-
-
-```python
-# But you can also open any package using:
-self.aa_open_app('com.roblox.client')
-```
-
-
-
-```python
-# This method makes swiping easy
-# x (start), y (start), x (end) y (end), last number in seconds
-self.aa_swipe(500, 400, 500, 100, 1.1) 
-```
-
-
-
-```python
-#opens a separate shell window using cmd.exe 
-self.aa_open_shell() 
-```
-
-
-
-```python
-# It changes the dictionary that you are in
-# and executes a command 
-self.aa_change_cwd_and_execute_adb_shell('ls', 'data/')
-b'5.3.10.1001\r\n'
-b'5.9.300.1014\r\n'
-b'adb\r\n'
-b'anr\r\n'
-b'app\r\n'
-b'app-asec\r\n'
-b'app-ephemeral\r\n'
-b'app-lib\r\n'
-b'app-private\r\n'
-b'arm\r\n'
-....
-```
-
-
-
-```python
-# This can also be accomplished by sending multiple commands: 
-self.aa_execute_multiple_adb_shell_commands(['cd data/', 'ls|grep system'])
-Out[28]: [b'system\r\n', b'system_ce\r\n', b'system_de\r\n']
-```
-
-
-
-```python
-# You can also send non-shell commands: 
-self.aa_execute_non_shell_adb_command('devices')
-```
-
-
-
-```python
-# This method pushes a file to your sdcard:
-self.aa_push_to_sdcard(r'F:\donedone.png')
-```
-
-
-
-```python
-# This method pulls a file to your hdd
-self.aa_pull('/sdcard/donedone.png', 'f:\\dfdffasd')
-```
-
-
-
-```python
-# A fast way of scanning all connected devices:
-# start/end means the ports you want to start/end with
-# After 10 seconds, all processes that have not completed the search
-# will be killed 
-self.aa_connect_do_all_devices(start=4999, end=6000, timeout=10)
-    '''self.aa_list_devices()
-b'List of devices attached\r\n'
-b'localhost:5037\toffline\r\n'
-b'localhost:5040\toffline\r\n'
-b'localhost:5357\toffline\r\n'
-b'localhost:5725\tdevice\r\n'
-b'localhost:5800\toffline\r\n'
-b'localhost:5875\tdevice\r\n'
-b'localhost:5900\toffline\r\n'
-b'localhost:5955\tdevice\r\n'
-b'\r\n'''
-
-    '''
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process'''
-```
-
-
-
-```python
-# Uses https://github.com/hansalemaos/a_cv2_shape_finder 
-# to detect shapes in the screenshot 
-self.get_shapes_from_screenshot_THRESH_OTSU()
-self.get_shapes_from_screenshot_ADAPTIVE_THRESH_MEAN_C()
-self.get_shapes_from_screenshot_ADAPTIVE_THRESH_GAUSSIAN_C()
-```
-
-
-
-```python
-#Some self-explaining stuff  
-
-self.aa_isfolder('/sdcard/donedone.png')
-False
-self.aa_isfolder('/sdcard/')
-True
-next(self.aa_get_screenshots())
-
-self.aa_path_exists('/sdcard/')
-True
-self.aa_path_exists('/sdcard2/')
-False
-
-self.aa_get_screen_resolution()
-(960, 540)
-
-self.aa_restart_server()
-self.aa_reboot_and_listen_to_usb()
-self.aa_start_server()
-self.aa_stop_server()
-self.aa_kill_server()
-self.aa_force_stop('com.roblox.client') #root
-self.aa_show_screenshot_in_browser()
-```
-
+# Easier ADB automation 
+
+## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
+
+### pip install adbkit
+
+**Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
+
+**28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
+
+```python
+from adbkit import ADBTools
+from kthread_sleep import sleep
+
+adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
+deviceserial = "localhost:5555"
+ADBTools.aa_kill_all_running_adb_instances()
+
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_start_server() # creates a new process which is not a child process
+sleep(3)
+self.aa_connect_to_device()
+self.aa_activate_scrcpy_screenshots_tcp(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+# for a usb connection:
+# self.aa_activate_scrcpy_screenshots_usb(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+
+# each killkey combination can only be used once!
+self.aa_show_screenshot( sleeptime=1, killkeys="ctrl+alt+h")
+
+# How to stop showing screenshots
+# press the killkeys combination "ctrl+alt+h" and call the method aa_kill_show_screenshot to kill all threads
+self.aa_kill_show_screenshot()
+
+# once your done with everything, make sure to close the scrcpy connection:
+self.aa_kill_scrcpy_connection()
+
+```
+
+**10/03/2023: Tesseract with multiprocessing / Bluestacks Hyper-V connect** 
+
+```python
+# Connects to all Bluestacks Hyper-V devices (dynamic ADB ports)  and returns a DataFrame 
+from adbkit import ADBTools
+ald=ADBTools.connect_to_all_bluestacks_hyperv_devices(    adb_path="C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
+timeout=10,
+bluestacks_config=r"C:\ProgramData\BlueStacks_nxt\bluestacks.conf",)
+
+# Tesseract OCR on all found elements - multiprocessing 
+adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
+deviceserial = "localhost:52249"
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_connect_to_device()
+self.aa_activate_tesseract(
+    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
+)
+self.aa_update_screenshot()
+df=self.aa_get_all_displayed_items_from_uiautomator(
+	screenshotfolder="f:\\compare_android2",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
+
+
+      bb_area  bb_bounds  bb_center_x  bb_center_x_cropped  bb_center_y  bb_center_y_cropped  bb_checkable  bb_checked   bb_class  bb_clickable bb_content_desc  bb_cropped_x_end  bb_cropped_x_start  bb_cropped_y_end  bb_cropped_y_start  bb_enabled  bb_focusable  bb_focused  bb_height  bb_height_cropped  bb_index bb_keys_hierarchy  bb_long_clickable  bb_old_index bb_package  bb_password bb_pure_id bb_resource_id bb_screenshot  bb_scrollable  bb_selected bb_shapely    bb_text  bb_valid_square  bb_width  bb_width_cropped  bb_x_end  bb_x_start  bb_y_end  bb_y_start ee_bb_longtouch ee_bb_longtouch_bs ee_bb_longtouch_offset ee_bb_longtouch_offset_bs ee_bb_touch ee_bb_touch_bs ee_bb_touch_offset ee_bb_touch_offset_bs ff_bb_downswipe ff_bb_save_screenshot ff_bb_show_screenshot ff_bb_tap_center_offset ff_bb_tap_center_offset_long ff_bb_tap_center_variation ff_bb_tap_center_variation_long ff_bb_tap_exact_center ff_bb_tap_exact_center_long ff_bb_upswipe bb_scanned_text
+0   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0    (node,)             False                  0     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+1   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  1     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+2   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  2     com.bl...      False    id/con...  androi...      [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+3   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  3     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+4   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  4     com.bl...      False    id/dra...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+5   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  5     com.bl...      False    id/ite...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+6   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  6     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+7   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 1  (node,...             False                  7     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+8    771120.0  (44, 8...        800          800                  335          335                False         False     a.q.a.b      False                          1556                44                 590                80                True        True         False         510        510                 0  (node,...             False                  8     com.bl...      False    id/des...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
+9    281464.0  (196, ...        800          800                  783          783                False         False   androi...      False                          1404               196                 900               667                True       False         False         233        233                 3  (node,...             False                  9     com.bl...      False      id/dock  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        667          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
+10   771120.0  (44, 8...        800          800                  335          335                False         False   androi...      False                          1556                44                 590                80                True       False         False         510        510                 0  (node,...             False                 10     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
+11    21744.0  (196, ...        800          800                  685          685                False         False   androi...      False                          1404               196                 694               676                True       False         False          18         18                 0  (node,...             False                 11     com.bl...      False    id/pop...  com.bl...      [[[35,...         False          False    POLYGO...  JOGOS ...       True            1208       1208             1404        196        694        676          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     JOGOS ...     
+12   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 1  (node,...             False                 12     com.bl...      False    id/fra...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
+13    42840.0  (44, 8...        170          170                  165          165                False         False   androi...       True                           296                44                 250                80                True        True         False         170        170                 0  (node,...              True                 13     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              296         44        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Play S...     
+14    42840.0  (296, ...        422          422                  165          165                False         False   androi...       True                           548               296                 250                80                True        True         False         170        170                 1  (node,...              True                 14     com.bl...      False         <NA>                 [[[36,...         False          False    POLYGO...                  True             252        252              548        296        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Centra...     
+15    42840.0  (548, ...        674          674                  165          165                False         False   androi...       True                           800               548                 250                80                True        True         False         170        170                 2  (node,...              True                 15     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              800        548        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Ga ...     
+16    42840.0  (800, ...        926          926                  165          165                False         False   androi...       True                          1052               800                 250                80                True        True         False         170        170                 3  (node,...              True                 16     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1052        800        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Jogue ...     
+17    42840.0  (1052,...       1178         1178                  165          165                False         False   androi...       True                          1304              1052                 250                80                True        True         False         170        170                 4  (node,...              True                 17     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1304       1052        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     IMEI/P...     
+18    42840.0  (1304,...       1430         1430                  165          165                False         False   androi...       True                          1556              1304                 250                80                True        True         False         170        170                 5  (node,...              True                 18     com.bl...      False         <NA>                 [[[38,...         False          False    POLYGO...                  True             252        252             1556       1304        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     SocksD...     
+19   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 0  (node,...             False                 19     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
+20   140128.0  (196, ...        800          800                  842          842                False         False   androi...      False                          1404               196                 900               784                True       False         False         116        116                 1  (node,...             False                 20     com.bl...      False    id/vie...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        784          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+21   197288.0  (258, ...        800          800                  785          785                False         False   androi...      False                          1342               258                 876               694                True       False         False         182        182                 0  (node,...             False                 21     com.bl...      False    id/all...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1084       1084             1342        258        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     a 2e4 ...     
+22    28938.0  (324, ...        403          403                  785          785                False         False   androi...       True                           483               324                 876               694                True        True         False         182        182                 0  (node,...             False                 22     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              483        324        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
+23    28938.0  (483, ...        562          562                  785          785                False         False   androi...       True                           642               483                 876               694                True        True         False         182        182                 1  (node,...             False                 23     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              642        483        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Ly m V...     
+24    28938.0  (642, ...        721          721                  785          785                False         False   androi...       True                           801               642                 876               694                True        True         False         182        182                 2  (node,...             False                 24     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              801        642        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+25    28938.0  (801, ...        880          880                  785          785                False         False   androi...       True                           960               801                 876               694                True        True         False         182        182                 3  (node,...             False                 25     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              960        801        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
+26    28756.0  (960, ...       1039         1039                  785          785                False         False   androi...       True                          1118               960                 876               694                True        True         False         182        182                 4  (node,...             False                 26     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1118        960        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
+27    28756.0  (1118,...       1197         1197                  785          785                False         False   androi...       True                          1276              1118                 876               694                True        True         False         182        182                 5  (node,...             False                 27     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1276       1118        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
+28    10000.0  (353, ...        403          403                  770          770                False         False   androi...      False                           453               353                 820               720                True       False         False         100        100                 0  (node,...             False                 28     com.bl...      False    id/app...  com.bl...      [[[44,...         False          False    POLYGO...                  True             100        100              453        353        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+29     7632.0  (324, ...        403          403                  852          852                False         False   androi...      False                           483               324                 876               828                True       False         False          48         48                 1  (node,...             False                 29     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Street...       True             159        159              483        324        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
+30    10000.0  (512, ...        562          562                  770          770                False         False   androi...      False                           612               512                 820               720                True       False         False         100        100                 0  (node,...             False                 30     com.bl...      False    id/app...  com.bl...      [[[46,...         False          False    POLYGO...                  True             100        100              612        512        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()       a wings     
+31     7632.0  (483, ...        562          562                  852          852                False         False   androi...      False                           642               483                 876               828                True       False         False          48         48                 1  (node,...             False                 31     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Viking...       True             159        159              642        483        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Viking...     
+32    10000.0  (671, ...        721          721                  770          770                False         False   androi...      False                           771               671                 820               720                True       False         False         100        100                 0  (node,...             False                 32     com.bl...      False    id/app...  com.bl...      [[[182...         False          False    POLYGO...                  True             100        100              771        671        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+33     7632.0  (642, ...        721          721                  852          852                False         False   androi...      False                           801               642                 876               828                True       False         False          48         48                 1  (node,...             False                 33     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Draken...       True             159        159              801        642        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Draken...     
+34    10000.0  (830, ...        880          880                  770          770                False         False   androi...      False                           930               830                 820               720                True       False         False         100        100                 0  (node,...             False                 34     com.bl...      False    id/app...  com.bl...      [[[184...         False          False    POLYGO...                  True             100        100              930        830        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+35     7632.0  (801, ...        880          880                  852          852                False         False   androi...      False                           960               801                 876               828                True       False         False          48         48                 1  (node,...             False                 35     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  War Ro...       True             159        159              960        801        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
+36    10000.0  (989, ...       1039         1039                  770          770                False         False   androi...      False                          1089               989                 820               720                True       False         False         100        100                 0  (node,...             False                 36     com.bl...      False    id/app...  com.bl...      [[[243...         False          False    POLYGO...                  True             100        100             1089        989        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+37     7584.0  (960, ...       1039         1039                  852          852                False         False   androi...      False                          1118               960                 876               828                True       False         False          48         48                 1  (node,...             False                 37     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Warspe...       True             158        158             1118        960        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
+38    10000.0  (1147,...       1197         1197                  770          770                False         False   androi...      False                          1247              1147                 820               720                True       False         False         100        100                 0  (node,...             False                 38     com.bl...      False    id/app...  com.bl...      [[[59,...         False          False    POLYGO...                  True             100        100             1247       1147        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+39     7584.0  (1118,...       1197         1197                  852          852                False         False   androi...      False                          1276              1118                 876               828                True       False         False          48         48                 1  (node,...             False                 39     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Dark O...       True             158        158             1276       1118        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
+40      529.0  (745, ...        756          756                  734          734                False         False   androi...      False                           768               745                 746               723                True       False         False          23         23                 0  (node,...             False                 40     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23              768        745        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+41      529.0  (1221,...       1232         1232                  734          734                False         False   androi...      False                          1244              1221                 746               723                True       False         False          23         23                 0  (node,...             False                 41     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23             1244       1221        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+
+
+
+
+
+self.aa_update_screenshot()
+df = self.aa_get_all_displayed_items_from_activities(
+	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+dftesser=self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
+
+
+      aa_area  aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text
+0       529.0  (427, ...        438          438                  734          734            androi...         False          ...            False                  450               427                 746               723                12     True       True      False         True            c741e85       208936581              23         23          app:id...              True        False          7f08011e  213123...         29        False               True               False            False             True                False                      False               False         id/pop...  [[[103...         False                    False              POLYGO...       True                I           23         23              450         97               427          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              28          27          26          24          22          20           6           5           4           3           2           0                 
+1       529.0  (586, ...        597          597                  734          734            androi...         False          ...            False                  609               586                 746               723                12     True       True      False         True            e9bb4da       245085402              23         23          app:id...              True        False          7f080121  213123...         33        False               True               False            False             True                False                      False               False         id/pop...  [[[187...         False                    False              POLYGO...       True                I           23         23              609         97               586          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              32          31          26          24          22          20           6           5           4           3           2           0                 
+2       529.0  (745, ...        756          756                  734          734            androi...         False          ...            False                  768               745                 746               723                12     True       True      False         True            5a48615        94668309              23         23          app:id...              True        False          7f080120  213123...         37        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23              768         97               745          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              36          35          26          24          22          20           6           5           4           3           2           0                 
+3       529.0  (904, ...        915          915                  734          734            androi...         False          ...            False                  927               904                 746               723                12     True       True      False         True            4029d0b        67280139              23         23          app:id...              True        False          7f08011d  213123...         41        False               True               False            False             True                False                      False               False         id/pop...  [[[255...         False                    False              POLYGO...       True                I           23         23              927         97               904          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              40          39          26          24          22          20           6           5           4           3           2           0                 
+4       529.0  (1063,...       1074         1074                  734          734            androi...         False          ...            False                 1086              1063                 746               723                12     True       True      False         True            27867e8        41445352              23         23          app:id...              True        False          7f08011c  213123...         45        False               True               False            False             True                False                      False               False         id/pop...  [[[65,...         False                    False              POLYGO...       True                I           23         23             1086         97              1063          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              44          43          26          24          22          20           6           5           4           3           2           0                 
+5       529.0  (1221,...       1232         1232                  734          734            androi...         False          ...            False                 1244              1221                 746               723                12     True       True      False         True            125ad2a        19246378              23         23          app:id...              True        False          7f08011f  213123...         49        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23             1244         97              1221          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              48          47          26          24          22          20           6           5           4           3           2           0                 
+6     10000.0  (353, ...        403          403                  770          770            androi...         False          ...            False                  453               353                 820               720                11    False       True      False         True            29caf0f        43822863             100        100          app:id...              True        False          7f080058  213123...         28        False              False               False            False            False                False                      False               False         id/app...  [[[44,...         False                    False              POLYGO...       True                V          100        100              453        129               353          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>                 
+7      7632.0  (324, ...        403          403                  852          852            androi...         False          ...            False                  483               324                 876               828                11     True       True      False         True            ea74b9c       245844892              48         48          app:id...              True        False          7f080060  213123...         30        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              483        159               324           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>   Street...     
+8     10000.0  (512, ...        562          562                  770          770            androi...         False          ...            False                  612               512                 820               720                11    False       True      False         True            cece9a5       216852901             100        100          app:id...              True        False          7f08005b  213123...         32        False              False               False            False            False                False                      False               False         id/app...  [[[46,...         False                    False              POLYGO...       True                V          100        100              612        129               512          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>     a wings     
+9      7632.0  (483, ...        562          562                  852          852            androi...         False          ...            False                  642               483                 876               828                11     True       True      False         True            aadf17a       179171706              48         48          app:id...              True        False          7f080063  213123...         34        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              642        159               483           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>   Viking...     
+10    10000.0  (671, ...        721          721                  770          770            androi...         False          ...            False                  771               671                 820               720                11    False       True      False         True            9ff2d2b       167718187             100        100          app:id...              True        False          7f08005a  213123...         36        False              False               False            False            False                False                      False               False         id/app...  [[[182...         False                    False              POLYGO...       True                V          100        100              771        129               671          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>                 
+11     7632.0  (642, ...        721          721                  852          852            androi...         False          ...            False                  801               642                 876               828                11     True       True      False         True            bab8588       195790216              48         48          app:id...              True        False          7f080062  213123...         38        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              801        159               642           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>   Draken...     
+12    10000.0  (830, ...        880          880                  770          770            androi...         False          ...            False                  930               830                 820               720                11    False       True      False         True            9e77b21       166165281             100        100          app:id...              True        False          7f080057  213123...         40        False              False               False            False            False                False                      False               False         id/app...  [[[184...         False                    False              POLYGO...       True                V          100        100              930        129               830          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>                 
+13     7632.0  (801, ...        880          880                  852          852            androi...         False          ...            False                  960               801                 876               828                11     True       True      False         True            b99ab46       194620230              48         48          app:id...              True        False          7f08005f  213123...         42        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              960        159               801           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>   War Ro...     
+14    10000.0  (989, ...       1039         1039                  770          770            androi...         False          ...            False                 1089               989                 820               720                11    False       True      False         True             c17107        12677383             100        100          app:id...              True        False          7f080056  213123...         44        False              False               False            False            False                False                      False               False         id/app...  [[[243...         False                    False              POLYGO...       True                V          100        100             1089        129               989          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>                 
+15     7584.0  (960, ...       1039         1039                  852          852            androi...         False          ...            False                 1118               960                 876               828                11     True       True      False         True            5377234        87519796              48         48          app:id...              True        False          7f08005e  213123...         46        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1118        158               960           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>   Warspe...     
+16    10000.0  (1147,...       1197         1197                  770          770            androi...         False          ...            False                 1247              1147                 820               720                11    False       True      False         True            59fa85d        94349405             100        100          app:id...              True        False          7f080059  213123...         48        False              False               False            False            False                False                      False               False         id/app...  [[[59,...         False                    False              POLYGO...       True                V          100        100             1247        129              1147          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>                 
+17     7584.0  (1118,...       1197         1197                  852          852            androi...         False          ...            False                 1276              1118                 876               828                11     True       True      False         True            f3535d2       255145426              48         48          app:id...              True        False          7f080061  213123...         50        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1276        158              1118           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>   Dark O...     
+18    30210.0  (324, ...        403          403                  781          781            androi...          True          ...            False                  483               324                 876               686                10    False       True       True         True            18369ed        25389549             190        190          app:id...              True        False          7f080050  213123...         27        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              483        225               324          66                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Street...     
+19    30210.0  (483, ...        562          562                  781          781            androi...          True          ...            False                  642               483                 876               686                10    False       True       True         True            9888022       159940642             190        190          app:id...              True        False          7f080053  213123...         31        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              642        384               483         225                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Ly m V...     
+20    30210.0  (642, ...        721          721                  781          781            androi...          True          ...            False                  801               642                 876               686                10    False       True       True         True            2751ab3        41228979             190        190          app:id...              True        False          7f080052  213123...         35        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              801        543               642         384                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   i Drak...     
+21    30210.0  (801, ...        880          880                  781          781            androi...          True          ...            False                  960               801                 876               686                10    False       True       True         True            3711870        57743472             190        190          app:id...              True        False          7f08004f  213123...         39        False              False               False            False            False                False                      False               False         id/app...  [[[87,...         False                    False              POLYGO...       True                V          159        159              960        702               801         543                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   War Ro...     
+22    30020.0  (960, ...       1039         1039                  781          781            androi...          True          ...            False                 1118               960                 876               686                10    False       True       True         True            339b7e9        54114281             190        190          app:id...              True        False          7f08004e  213123...         43        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1118        860               960         702                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Warspe...     
+23    30020.0  (1118,...       1197         1197                  781          781            androi...          True          ...            False                 1276              1118                 876               686                10    False       True       True         True            cd27c6e       215121006             190        190          app:id...              True        False          7f080051  213123...         47        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1276       1018              1118         860                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Dark O...     
+24      900.0  (785, ...        800          800                  797          797            androi...         False          ...            False                  815               785                 812               782                 9     True       True      False         True            268c7fc        40421372              30         30          app:id...              True        False          7f0800a8  213123...         25        False              False               False            False             True                False                      False               False         id/doc...  [[[35,...         False                    False              POLYGO...       True                G           30         30              815        619               785         589                812        118               782          88                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
+25   205960.0  (258, ...        800          800                  781          781            androi...         False          ...            False                 1342               258                 876               686                 9    False       True      False         True            8a2d3cc       144888780             190        190          app:id...              True        False          7f080048  213123...         26        False              False               False            False            False                False                      False               False         id/all...  [[[35,...         False                    False              POLYGO...       True                V         1084       1084             1342       1146               258          62                876        182               686          -8                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>   Street...     
+26    51579.0  (31, 6...        812          812                   78           78            androi...          True          ...            False                 1594                31                  95                62                 9     True       True       True         True            b601a94       190847636              33         33          app:id...              True        False          7f0800c6  213123...         54        False               True               False            False             True                False                      False               False         id/gro...  [[[35,...         False                    False              POLYGO...       True                V         1563       1563             1594       1588                31          25                 95         53                62          20                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
+27  1179406.0  (43, 9...        800          800                  484          484            com.bl...         False          ...            False                 1557                43                 874                95                 9     True       True      False         True            27c993d        41720125             779        779          app:id...              True        False          7f0800c3  213123...         55        False               True               False            False             True                False                      False               False          id/group  [[[35,...         False                    False              POLYGO...       True                V         1514       1514             1557       1551                43          37                874        832                95          53                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>   Ga u i...     
+28    42840.0  (296, ...        422          422                  165          165            com.bl...          True          ...            False                  548               296                 250                80                 8     True       True       True         True              d801f          884767             170        170               <NA>              True         True              <NA>       <NA>         10        False              False               False            False            False                False                      False               False              <NA>  [[[36,...         False                    False              POLYGO...       True                V          252        252              548        504               296         252                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Centra...     
+29    42840.0  (44, 8...        170          170                  165          165            com.bl...          True          ...            False                  296                44                 250                80                 8     True       True       True         True            9c32f6c       163786604             170        170               <NA>              True         True              <NA>       <NA>         11        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              296        252                44           0                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Play S...     
+30    42840.0  (800, ...        926          926                  165          165            com.bl...          True          ...            False                 1052               800                 250                80                 8     True       True       True         True            a164935       169232693             170        170               <NA>              True         True              <NA>       <NA>         12        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1052       1008               800         756                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Jogue ...     
+31    42840.0  (1052,...       1178         1178                  165          165            com.bl...          True          ...            False                 1304              1052                 250                80                 8     True       True       True         True            9c981ca       164200906             170        170               <NA>              True         True              <NA>       <NA>         13        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1304       1260              1052        1008                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   IMEI/P...     
+32    42840.0  (548, ...        674          674                  165          165            com.bl...          True          ...            False                  800               548                 250                80                 8     True       True       True         True            c93ff3b       211025723             170        170               <NA>              True         True              <NA>       <NA>         14        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              800        756               548         504                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   as Ga ...     
+33    42840.0  (1304,...       1430         1430                  165          165            com.bl...          True          ...            False                 1556              1304                 250                80                 8     True       True       True         True            569d658        90822232             170        170               <NA>              True         True              <NA>       <NA>         15        False              False               False            False            False                False                      False               False              <NA>  [[[38,...         False                    False              POLYGO...       True                V          252        252             1556       1512              1304        1260                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   SocksD...     
+34   140128.0  (196, ...        800          800                  842          842            androi...         False          ...            False                 1404               196                 900               784                 8     True       True      False         True            d395417       221860887             116        116          app:id...              True        False          7f08017f  213123...         23        False              False               False            False            False                False                      False               False         id/vie...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               784          90                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>                 
+35   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 8    False       True      False         True            9d20004       164757508             206        206               <NA>              True        False              <NA>       <NA>         24        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               694           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
+36  1352976.0  (6, 42...        800          800                  468          468            androi...         False          ...            False                 1594                 6                 894                42                 8    False       True      False         True            ebbfee7       247201511             852        852               <NA>              True        False              <NA>       <NA>         53        False               True               False            False             True                False                      False               False              <NA>  [[[39,...         False                    False              POLYGO...       True                V         1588       1588             1594       1594                 6           6                894        858                42           6                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   a | | ...     
+37   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 7     True       True      False         True             49b71b         4831003             510        510               <NA>              True        False              <NA>       <NA>          9        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1512                44           0                590        510                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
+38      225.0  (726, ...        733          733                  620          620            androi...         False          ...            False                  741               726                 628               613                 7     True       True      False         True            1b8c9ce        28887502              15         15          app:id...              True        False          7f0800ef  213123...         18        False               True               False            False             True                False                      False               False         id/loa...  [[[35,...         False                    False              POLYGO...       True                V           15         15              741         25               726          10                628         22               613           7                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
+39     2604.0  (751, ...        813          813                  620          620            androi...         False          ...            False                  875               751                 631               610                 7     True       True      False         True            c7ee0ef       209641711              21         21          app:id...              True        False          7f0800dc  213123...         19        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                V          124        124              875        159               751          35                631         25               610           4                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
+40    21744.0  (196, ...        800          800                  685          685            androi...         False          ...            False                 1404               196                 694               676                 7     True       True      False         True            d6f43b1       225395633              18         18          app:id...              True        False          7f08011b  213123...         21        False              False               False            False            False                False                      False               False         id/pop...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                694         27               676           9                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   JOGOS ...     
+41   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 7    False       True      False         True            ae5f096       182841494             206        206          app:id...              True        False          7f0800bd  213123...         22        False              False               False            False            False                False                      False               False         id/fra...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        233               694          27                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
+42  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 7    False       True      False         True            69044a6       110118054             864        864               <NA>              True        False              <NA>       <NA>         52        False               True               False            False             True                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+43  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 6    False       True      False         True            46dee93        74313363             864        864          app:id...              True        False          7f08006c  213123...          7        False              False               False            False             True                False                      False               False         id/bac...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+44   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 6     True       True       True         True            6affac3       112196291             510        510          app:id...              True        False          7f08009e  213123...          8        False              False               False            False            False                False                      False               False         id/des...  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1556                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
+45    25600.0  (0, 59...        800          800                  598          598            com.bl...         False          ...            False                 1600                 0                 606               590                 6     True       True      False         True            a318ed0       171019984              16         16          app:id...              True        False          7f08009f  213123...         16        False               True               False            False             True                False                      False               False         id/des...  [[[28,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                606        570               590         554                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+46     5070.0  (716, ...        800          800                  621          621            androi...         False          ...            False                  885               716                 636               606                 6    False       True      False         True            57d5ec9        92102345              30         30          app:id...              True        False          7f0800db  213123...         17        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                I          169        169              885        885               716         716                636        600               606         570                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+47   281464.0  (196, ...        800          800                  783          783            androi...         False          ...            False                 1404               196                 900               667                 6    False       True      False         True            d275f40       220684096             233        233          app:id...              True        False          7f0800a7  213123...         20        False              False               False            False            False                False                      False               False           id/dock  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1404               196         196                900        864               667         631                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Street...     
+48  1382400.0  (0, 36...        800          800                  468          468            com.bl...          True          ...            False                 1600                 0                 900                36                 6    False       True       True         True            25d1e01        39656961             864        864          app:id...              True        False          7f0800c4  213123...         51        False               True               False            False             True                False                      False               False         id/gro...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+49    19380.0  (44, 8...         63           63                  335          335            androi...         False          ...            False                   82                44                 590                80                 6     True       True      False         True            4493e79        71908985             510        510          app:id...              True        False          7f0800e5  213123...         56        False              False               False            False            False                False                      False               False         id/lef...  [[[35,...         False                    False              POLYGO...       True                V           38         38               82         82                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+50    19380.0  (1518,...       1537         1537                  335          335            androi...         False          ...            False                 1556              1518                 590                80                 6     True       True      False         True            ecea7be       248424382             510        510          app:id...              True        False          7f08012e  213123...         57        False              False               False            False            False                False                      False               False         id/rig...  [[[37,...         False                    False              POLYGO...       True                V           38         38             1556       1556              1518        1518                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+51  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 5    False       True      False         True            294a77d        43296637             864        864               <NA>              True        False              <NA>       <NA>          6        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+52  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 5     True       True      False         True            c019672       201430642             864        864               <NA>              True        False              <NA>       <NA>         58        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+53  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 4     True       True      False         True            38d79ff        59603455             864        864          app:id...              True        False          7f0800df  213123...          5        False              False               False            False            False                False                      False               False         id/ite...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+54  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 3    False       True       True         True            d8cdd1e       227335454             864        864          app:id...              True        False          7f0800b1  213123...          4        False              False                True            False            False                False                      False               False         id/dra...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                36          36                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+55  1440000.0  (0, 0,...        800          800                  450          450            androi...         False        an...            False                 1600                 0                 900                 0                 2    False       True      False         True            2b36d59        45313369             900        900               <NA>              True        False              <NA>       <NA>          3        False              False               False            False            False                False                      False               False              <NA>  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
+56        0.0  (0, 0,...          0            0                    0            0            androi...         False      andr...            False                    0                 0                   0                 0                 1    False       True      False        False            812b782       135444354               0          0          androi...              True        False           102018a   16908682          1        False              False               False            False             True                False                      False               False         id/act...        NaN         False                    False              POLYGO...      False                G            0          0                0          0                 0           0                  0          0                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()            <NA>                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+57  1440000.0  (0, 0,...        800          800                  450          450            androi...         False      andr...            False                 1600                 0                 900                 0                 1    False       True      False         True            5f37da0        99843488             900        900          androi...              True        False           1020002   16908290          2        False              False               False            False            False                False                      False               False         id/con...  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
+
+```
+
+**01/03/2023: Added adbdevicechanger** 
+```python
+# https://github.com/hansalemaos/adbdevicechanger
+# tested with bluestacks - root access
+self.aa_activate_adbdevicechanger()
+self.bb_adbdevicechanger.change_android_id()
+
+b'Row: 0 _id=227, name=device_name, value=OnePlus 5T\r\n'
+Out[7]: ('f7a32086dc724a4a', 'OnePlus 5T')
+
+
+self.bb_adbdevicechanger.change_device_name(
+    modelregex=".*",
+    developerregex=".*",
+    androidfullnameregex=".*",
+    year=">1",
+    month=">0",
+    versionnumberaround=7.05,
+)
+b'Row: 0 _id=2340, name=android_id, value=f7a32086dc724a4a\r\n'
+b'Row: 0 _id=228, name=device_name, value=HTC U11\r\n'
+Out[8]: ('f7a32086dc724a4a', 'HTC U11')
+
+self.bb_adbdevicechanger.change_android_id_and_device_name(
+    modelregex=".*",
+    developerregex=".*",
+    androidfullnameregex=".*",
+    year=">1",
+    month=">0",
+    versionnumberaround=7.05,
+)
+b'Row: 0 _id=2341, name=android_id, value=fb9afc93197942d8\r\n'
+b'Row: 0 _id=229, name=device_name, value=Nokia 8\r\n'
+Out[9]: ('fb9afc93197942d8', 'Nokia 8')
+
+
+self.bb_adbdevicechanger.get_random_android_cellphones(    modelregex="Samsung.*",
+    developerregex=".*",
+    androidfullnameregex=".*",
+    year=">2010",
+    month=">0",
+    versionnumberaround=9.05,
+    howmany=10,
+    return_list=False,)
+Out[13]: 
+                       aa_model  ...              uuid
+0  Samsung Galaxy Note 20/Ultra  ...  36f8a604180b4d7f
+1            Samsung Galaxy A70  ...  cb7f374cd85d4330
+2      Samsung Galaxy A30s/A50s  ...  9380749deb5942f6
+3      Samsung Galaxy Note 10/+  ...  c36816b1906542dc
+4    Samsung Galaxy S20/+/Ultra  ...  33dc12217b404a62
+5         Samsung Galaxy A90 5G  ...  cf0084fa8261465d
+6      Samsung Galaxy A51 5G UW  ...  3177aa09b1fc40d9
+7            Samsung Galaxy A01  ...  44db6d59366143cd
+8         Samsung Galaxy A42 5G  ...  a5b6fb2d08ac4475
+9           Samsung Galaxy A20e  ...  806b4ae287ec4d34
+[10 rows x 10 columns]
+
+```
+
+
+**23/02/2023: New methods**
+```python
+from adbkit import ADBTools
+adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
+deviceserial = "localhost:5555"
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_connect_to_device()
+self.aa_activate_tesseract(
+    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
+)
+
+#####################################################################################
+# This method uses Tesseract! You can download it here: https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
+self.aa_update_screenshot() # Update the screenshot before 
+df=self.aa_ocr_elements_from_activities(['Play Store'], # pass all strings as a list 
+minpercentage=85, # fuzzy match
+maxtolerance=10,
+screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+
+    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
+32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
+
+
+
+#####################################################################################
+# Another example (Play Store written wrong)
+
+df2=self.aa_ocr_elements_from_uiautomator(['blai Store'],minpercentage=70, maxtolerance=10, )
+
+    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
+32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
+
+#####################################################################################
+# Pass a list of tuples:
+((x,y),time in seconds)
+
+self.aa_multi_input_tap_with_delay([((100,100),2), ((200,200),3)])
+#####################################################################################
+
+self.aa_input_tap(x=100,y=100)
+
+#####################################################################################
+# https://github.com/hansalemaos/adbescapes
+# Converts Unicode string to ASCII and escapes all characters that need to be escaped. 
+# You have to activate it, before using it. The first start takes some time because numba needs to compile the code 
+self.aa_activate_input_text_formated()
+
+# input 
+text="""
+"'ąćęłń'\tóśźż\nĄĆĘŁŃÓŚŹŻ\n\"Junto à Estação de \nCarcavelos;\"" "äöüÄÖÜß"
+"""
+self.aa_input_text_formated_with_delay(text,delay=(0.01, 0.2),respect_german_letters=False, exit_keys="ctrl+x")
+
+
+# output
+"'aceln'    oszz
+ACELNOSZZ
+"Junto a Estacao de 
+Carcavelos;"" "aouAOUb"
+
+# If you want it the German way :)
+self.aa_input_text_formated(text,respect_german_letters=True, exit_keys="ctrl+x")
+
+"'aceln'    oszz
+ACELNOSZZ
+"Junto a Estacao de 
+Carcavelos;"" "aeoeueAeOeUess"
+#####################################################################################
+self.aa_install_apk_from_hdd(r"C:\Users\Gamer\anaconda3\envs\instcont\instagram.apk")
+#####################################################################################
+self.aa_uninstall_package('com.instagram.lite')
+#####################################################################################
+# First argument is a regex 
+self.aa_copy_apk_to_hdd('com.insta.*', 'c:\\instaapkdownload')
+#####################################################################################
+```
+
+
+
+**17/01/2023: Screenshot fix**
+
+
+```python
+$pip install adbkit
+from adbkit import ADBTools
+adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
+deviceserial = "localhost:5875"
+
+# Create an instance
+# Don't get confused about the instance name "self". I did it because it is faster copying methods from the class 
+self = ADBTools(adb_path, deviceserial, sdcard="/sdcard/")
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+
+# connect to the device 
+self.aa_connect_to_device()
+```
+
+
+
+```python
+# If you are using BlueStacks and want to have root access, call:
+self.aa_root_bluestacks_instances() 
+# This method will basically do this steps: https://appuals.com/root-bluestacks/ to root BlueStacks
+# You can run the script every time you use this module. It won't hurt. 
+# The first time, you might have to restart BlueStacks to enable the root access 
+```
+
+
+
+```python
+# If your device/BlueStacks is rooted, enable root so that all commands will be sent as root 
+self.aa_enable_root() 
+# can be disabled by calling :
+self.aa_disable_root()
+```
+
+
+
+```python
+# Activates self.bb_adbkeyboard 
+# Read more about it: https://github.com/hansalemaos/adb_unicode_keyboard
+self.aa_activate_adb_keyboard(exit_keys="ctrl+x") 
+```
+
+
+
+```python
+# Activates self.bb_sendevent_keyboard (needs root access)
+# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
+
+self.aa_activate_sendevent_keyboard(
+    sdcard="/storage/emulated/0/",
+    tmp_folder_on_sd_card="AUTOMAT",
+    exit_keys="ctrl+x",
+)  # needs root access
+
+# Here is one example: 
+self.bb_adbkeyboard.press_7_keycode_0()
+```
+
+
+
+```python
+# Activates self.self.bb_getevent_sendevent
+# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
+
+self.aa_activate_getevent_sendevent(
+    sdcard="/storage/emulated/0/",
+    tmp_folder_on_sd_card="AUTOMAT",
+    bluestacks_divider=32767,
+    exit_keys="ctrl+x",
+)  # needs root access
+```
+
+
+
+```python
+# Activates self.bb_sendevent_touch
+# Read more about it: https://github.com/hansalemaos/sendevent_touch
+
+self.aa_activate_sendevent_touch(
+    sdcard="/storage/emulated/0/",
+    tmp_folder_on_sd_card="AUTOMAT",
+    bluestacks_divider=32767,
+    use_bluestacks_coordinates=True,
+)  # needs root access
+
+# Here is one example:
+self.bb_sendevent_touch.touch(10,10)
+```
+
+
+
+```python
+# Activates https://github.com/hansalemaos/a_pandas_ex_tesseract_multirow_regex_fuzz
+# You can download the 64 bit version of tesseract here: 
+# https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
+
+self.aa_activate_tesseract(
+        tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
+    )
+
+# Once activated, you can call:
+# self.aa_ocr_with_tesseract()
+
+    left  top  width  height       conf        text  middle_x  middle_y  end_x  end_y
+8    382   42    499      49  37.512093         RH,       631        66    881     91
+9    728   34     98      61  30.925949          2.       777        64    826     95
+13   370  101     37      11   84.72541     'system       388       106    407    112
+14   411  101     24      10  79.929901        Apps       423       106    435    111
+15   536   90     36      28  85.425911      Roblox       554       104    572    118
+16   676  100     55       9  88.744247  BlueStacks       703       104    731    109
+17   735  101      7       8  80.470955           X       738       105    742    109
+18   814  101     31      10  90.271423      Spiele       829       106    845    111
+19   848  101     18       8  93.303749         und       857       105    866    109
+20   869  103     41       9  87.963295     gewinne       889       107    910    112
+28    72  100     20      12  96.004517        Play        82       106     92    112
+29    95  101     27       8  86.986359       Store       108       105    122    109
+33   225  211     49      12  76.804665   Globoplay       249       217    274    223
+37   326  489     25      28  91.894142       Tibia       338       503    351    517
+38   401  500     50       8  91.477989   Guardians       426       504    451    508
+39   455  499     10       9  72.064316          of       460       503    465    508
+41   415  512     37       9  75.078018     Cloudia       433       516    452    521
+
+# and even perform a multiline fuzzy search:
+xxx = self.aa_ocr_with_tesseract(search_for='Kontakte verwalten')
+```
+```python
+# Use this method to update the screenshot 
+# The updated screenshot can be found here: self.screenshot
+self.aa_update_screenshot()
+
+```
+
+
+
+```python
+# get 5 screenshot within 5 seconds
+xx=self.aa_get_screenshots(
+        sleeptime=1,
+        number=5)
+
+```
+
+
+
+```python
+# Now you can use self.df to do operations on the screenshot 
+# More information about a_pandas_ex_image_tools:
+# https://github.com/hansalemaos/a_pandas_ex_image_tools
+self.aa_update_imagedf()
+```
+
+
+```python
+# If you want to capture the logcat output and analyze it in a DataFrame,
+use: 
+logcatcap = self.aa_capture_logcat(
+        exit_keys="ctrl+x",
+        timeout=None,
+    )  
+
+# When you exit using "ctrl+x", the method will return a DataFrame
+# By the way: almost all methods can be interrupted using a key command 
+```
+
+
+
+```python
+# Those 2 methods will help you to identify and interact with views:
+# Read more about it: https://github.com/hansalemaos/androdf
+df1 = self.aa_get_all_displayed_items_from_uiautomator(
+	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+
+df3 = self.aa_get_all_displayed_items_from_activities(
+	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+```
+
+
+
+```python
+# Uses: https://github.com/hansalemaos/a_pandas_ex_adb_to_df
+# lists all files in DataFrame and adds useful functions
+# self.aa_list_all_files_on_device()
+
+dffiles = self.aa_list_folder_content(folder_to_search="data/")  
+print(dffiles)
+                  aa_date  ... ff_pull_file_cat
+0     2022-12-11 06:48:00  ...               ()
+1     2022-12-26 22:16:00  ...               ()
+2     2022-12-06 19:10:00  ...               ()
+3     2022-12-06 13:38:00  ...               ()
+4     2022-12-26 22:16:00  ...               ()
+                   ...  ...              ...
+26120 2021-09-16 04:21:00  ...               ()
+26121 2021-09-16 03:53:00  ...               ()
+26122 2021-09-16 03:53:00  ...               ()
+26123 2021-09-16 04:35:00  ...               ()
+26124 2021-09-16 04:31:00  ...               ()
+[26125 rows x 16 columns]
+```
+
+
+
+```python
+# Search with grep 
+# Uses https://github.com/hansalemaos/adb_grep_search
+dfgrep = self.aa_grep_search(
+        folder_to_search="data/data",
+        filetype="*.db",
+        regular_expression=r"CREATE.TABLE",
+        exit_keys="ctrl+x",
+        timeout=None,
+        remove_control_characters=True,
+    )
+
+dfgrep
+Out[19]: 
+                                               aa_file  ...      aa_regex
+0    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+1    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+2    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+3    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+4    data/data/com.globo.globotv/databases/mcsdk_bf...  ...  CREATE.TABLE
+..                                                 ...  ...           ...
+103  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+104  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+105  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+106  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+107  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+[108 rows x 5 columns]
+```
+
+
+
+```python
+# Uses https://github.com/hansalemaos/a_pandas_ex_adb_settings_to_df
+self.aa_parse_settings_from_all_packages(
+        tempfolder="f:\\tmpfolder", datafolder="data/"
+    )
+
+        index          aa_all_keys  ... level_22 level_23
+0         0.0         (long, name)  ...      NaN      NaN
+1         1.0        (long, value)  ...      NaN      NaN
+2         0.0   (boolean, 0, name)  ...      NaN      NaN
+3         1.0  (boolean, 0, value)  ...      NaN      NaN
+4         2.0   (boolean, 1, name)  ...      NaN      NaN
+       ...                  ...  ...      ...      ...
+110795    NaN            (6, desc)  ...      NaN      NaN
+110796    NaN           (6, label)  ...      NaN      NaN
+110797    NaN             (6, pkg)  ...      NaN      NaN
+110798    NaN          (6, source)  ...      NaN      NaN
+110799    NaN             (6, url)  ...      NaN      NaN
+[110800 rows x 31 columns]
+
+You might see this error messages several times:
+
+"Go to: https://www.sqlite.org/download.html ,
+download the dll and put it in the DLLs folder of your env!"
+
+You can ignore it.
+```
+
+
+
+```python
+#This method helps you find all executable activities from a package 
+# More about it: https://github.com/hansalemaos/a_pandas_ex_adb_execute_activities
+
+self.aa_get_activity_execution_df_from_one_package(
+        packagename="com.roblox.client"
+    ) 
+```
+
+
+
+```python
+# adds new contact, can be saved straight away
+addcon = self.aa_add_new_contact(
+	"hans", "+55119897827552", "hans@something.com", "my address", save=False
+)
+```
+
+
+
+```python
+# If you play Roblox, you can enable/disable some textures to get higher fps
+self.aa_enable_roblox_textures(
+	exit_keys="ctrl+x",
+	print_output=True,
+	timeout=None,
+)
+
+self.aa_disable_roblox_textures(
+	exit_keys="ctrl+x",
+	print_output=True,
+	timeout=None,
+)
+```
+
+
+
+```python
+# goes to the home screen, doesn't close anything
+self.aa_go_to_home_screen()
+```
+
+
+
+```python
+# repeat=5 usually deletes more than 5 characters!!
+self.aa_press_delete_key_repeated_times(repeat=5)
+```
+
+
+
+```python
+# starts the android file manager, pass the file type you want to see
+self.aa_get_content(type_="text/plain")
+```
+
+
+
+```python
+# Here are some methods to get useful information. 
+# Returns DataFrames 
+print(self.aa_whole_dumpsys_to_df())
+print(self.aa_list_all_packages())
+print(self.aa_list_broadcast_stats())
+print(self.aa_list_pending_intents())
+print(self.aa_list_all_activities_from_device())
+print(self.aa_list_all_services())
+print(self.aa_list_all_receivers())
+print(self.aa_list_all_activities())
+print(self.aa_get_procstats())
+print(self.aa_list_all_devices()) # devices on the device (dev ...)
+print(self.aa_list_devices()) # all adb devices (localhost:5555 ...)
+print(self.aa_list_pids_basic())
+print(self.aa_list_pids_complete())
+print(self.aa_list_memory())
+print(self.aa_getprop())
+print(self.aa_list_all_broadcasts())
+print(self.aa_list_all_broadcasts_history())
+print(self.aa_list_users())
+print(self.aa_list_permission_groups())
+print(self.aa_list_disabled_packages())
+print(self.aa_list_apps_in_use())
+print(self.aa_list_3rd_party_packages())
+print(self.aa_list_features())
+```
+
+
+
+```python
+# Smile! :)
+self.aa_open_camera_photo_mode()
+```
+
+
+
+```python
+# works with and without http://
+print(self.aa_open_website("google.com"))
+```
+
+
+
+```python
+# switches to gallery
+self.aa_start_gallery()
+```
+
+
+
+```python
+# cheeeese
+self.aa_take_a_picture()
+```
+
+
+
+```python
+# useful for some apps 
+self.aa_adb_turn_screen_compatibility_off()
+self.aa_adb_turn_screen_compatibility_on()
+```
+
+
+
+```python
+# Be careful! 
+self.aa_remove_file('/sdcard/9.png')
+```
+
+
+
+```python
+# Essential when you use your cell phone (with Whatsapp, Facebook ...) to automize things.
+self.aa_enable_notifications()
+self.aa_disable_notifications()
+```
+
+
+
+```python
+# More useful stuff for notifications
+self.aa_expand_settings() 
+self.aa_expand_notifications()
+```
+
+
+
+```python
+# Changes the screen orientation
+# You can pass:
+# horizontal_upside_down or 2
+# vertical or 1
+# horizontal or 0
+# vertical_upside_down or 3
+self.aa_change_screen_orientation("horizontal")
+```
+
+
+
+```python
+self.aa_get_display_orientation()
+#Out[4]: 0 
+# 0 means horizontal
+```
+
+
+
+```python
+# Sometimes you upload new media files, but you can't see the thumbnails immediately
+# This method updates all thumbnails
+self.aa_rescan_media()
+```
+
+
+
+```python
+# If you are in the middle of a text and want to go to the end of the line
+self.aa_move_to_end_of_line()
+```
+
+
+
+```python
+# Useful keyboard stuff 
+self.aa_hide_keyboard()
+self.aa_is_keyboard_shown()
+```
+
+
+
+```python
+# Doesn't work on BlueStacks, but on my pixel 6 there are no problems
+# (Actually it is not necessary when using BlueStacks hahaha)
+self.aa_is_screen_unlocked()
+```
+
+
+
+```python
+# Don't use this command on BlueStacks, you will have to reboot the device
+self.aa_lock_screen()
+```
+
+
+
+```python
+# Useful commands 
+self.aa_press_home() #back to home screen
+self.aa_press_app_switch()
+```
+
+
+
+```python
+# Configured for my Pixel 6, but should work on any device with a 
+# newer android version. 
+self.aa_swipe_up_to_unlock_screen('3333')
+```
+
+
+
+```python
+# doesn't work with BlueStacks, because of the app switch design, 
+# but it does on my pixel and should work with any device that 
+# has a recent Android version
+self.aa_close_all_apps_with_swipe()
+```
+
+
+
+```python
+# uninstalls a package
+self.aa_uninstall_package('com.google.android.youtube')
+```
+
+
+
+```python
+# Returns the activity needed to open the package 
+self.aa_resolve_activity('com.roblox.client')
+b'priority=0 preferredOrder=0 match=0x108000 specificIndex=-1 isDefault=true\r\n'
+b'com.roblox.client/.startup.ActivitySplash\r\n'
+```
+
+
+
+```python
+# But you can also open any package using:
+self.aa_open_app('com.roblox.client')
+```
+
+
+
+```python
+# This method makes swiping easy
+# x (start), y (start), x (end) y (end), last number in seconds
+self.aa_swipe(500, 400, 500, 100, 1.1) 
+```
+
+
+
+```python
+#opens a separate shell window using cmd.exe 
+self.aa_open_shell() 
+```
+
+
+
+```python
+# It changes the dictionary that you are in
+# and executes a command 
+self.aa_change_cwd_and_execute_adb_shell('ls', 'data/')
+b'5.3.10.1001\r\n'
+b'5.9.300.1014\r\n'
+b'adb\r\n'
+b'anr\r\n'
+b'app\r\n'
+b'app-asec\r\n'
+b'app-ephemeral\r\n'
+b'app-lib\r\n'
+b'app-private\r\n'
+b'arm\r\n'
+....
+```
+
+
+
+```python
+# This can also be accomplished by sending multiple commands: 
+self.aa_execute_multiple_adb_shell_commands(['cd data/', 'ls|grep system'])
+Out[28]: [b'system\r\n', b'system_ce\r\n', b'system_de\r\n']
+```
+
+
+
+```python
+# You can also send non-shell commands: 
+self.aa_execute_non_shell_adb_command('devices')
+```
+
+
+
+```python
+# This method pushes a file to your sdcard:
+self.aa_push_to_sdcard(r'F:\donedone.png')
+```
+
+
+
+```python
+# This method pulls a file to your hdd
+self.aa_pull('/sdcard/donedone.png', 'f:\\dfdffasd')
+```
+
+
+
+```python
+# A fast way of scanning all connected devices:
+# start/end means the ports you want to start/end with
+# After 10 seconds, all processes that have not completed the search
+# will be killed 
+self.aa_connect_do_all_devices(start=4999, end=6000, timeout=10)
+    '''self.aa_list_devices()
+b'List of devices attached\r\n'
+b'localhost:5037\toffline\r\n'
+b'localhost:5040\toffline\r\n'
+b'localhost:5357\toffline\r\n'
+b'localhost:5725\tdevice\r\n'
+b'localhost:5800\toffline\r\n'
+b'localhost:5875\tdevice\r\n'
+b'localhost:5900\toffline\r\n'
+b'localhost:5955\tdevice\r\n'
+b'\r\n'''
+
+    '''
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process'''
+```
+
+
+
+```python
+# Uses https://github.com/hansalemaos/a_cv2_shape_finder 
+# to detect shapes in the screenshot 
+self.get_shapes_from_screenshot_THRESH_OTSU()
+self.get_shapes_from_screenshot_ADAPTIVE_THRESH_MEAN_C()
+self.get_shapes_from_screenshot_ADAPTIVE_THRESH_GAUSSIAN_C()
+```
+
+
+
+```python
+#Some self-explaining stuff  
+
+self.aa_isfolder('/sdcard/donedone.png')
+False
+self.aa_isfolder('/sdcard/')
+True
+next(self.aa_get_screenshots())
+
+self.aa_path_exists('/sdcard/')
+True
+self.aa_path_exists('/sdcard2/')
+False
+
+self.aa_get_screen_resolution()
+(960, 540)
+
+self.aa_restart_server()
+self.aa_reboot_and_listen_to_usb()
+self.aa_start_server()
+self.aa_stop_server()
+self.aa_kill_server()
+self.aa_force_stop('com.roblox.client') #root
+self.aa_show_screenshot_in_browser()
+```
+
```

### Comparing `adbkit-0.17/README.md` & `adbkit-0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,66 @@
+Metadata-Version: 2.1
+Name: adbkit
+Version: 0.18
+Summary: Big automation package for ADB
+Home-page: https://github.com/hansalemaos/adbkit
+Author: Johannes Fischer
+Author-email: aulasparticularesdealemaosp@gmail.com
+License: MIT
+Keywords: adb,android,automation,shell,root
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE.rst
+
+
 # Easier ADB automation 
 
 ## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
 
+**28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
+
+```python
+from adbkit import ADBTools
+from kthread_sleep import sleep
+
+adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
+deviceserial = "localhost:5555"
+ADBTools.aa_kill_all_running_adb_instances()
+
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_start_server() # creates a new process which is not a child process
+sleep(3)
+self.aa_connect_to_device()
+self.aa_activate_scrcpy_screenshots_tcp(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+# for a usb connection:
+# self.aa_activate_scrcpy_screenshots_usb(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+
+# each killkey combination can only be used once!
+self.aa_show_screenshot( sleeptime=1, killkeys="ctrl+alt+h")
+
+# How to stop showing screenshots
+# press the killkeys combination "ctrl+alt+h" and call the method aa_kill_show_screenshot to kill all threads
+self.aa_kill_show_screenshot()
+
+# once your done with everything, make sure to close the scrcpy connection:
+self.aa_kill_scrcpy_connection()
+
+```
+
 **10/03/2023: Tesseract with multiprocessing / Bluestacks Hyper-V connect** 
 
 ```python
 # Connects to all Bluestacks Hyper-V devices (dynamic ADB ports)  and returns a DataFrame 
 from adbkit import ADBTools
 ald=ADBTools.connect_to_all_bluestacks_hyperv_devices(    adb_path="C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
 timeout=10,
```

### Comparing `adbkit-0.17/adbkit/README.MD` & `adbkit-0.18/adbkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,66 @@
+Metadata-Version: 2.1
+Name: adbkit
+Version: 0.18
+Summary: Big automation package for ADB
+Home-page: https://github.com/hansalemaos/adbkit
+Author: Johannes Fischer
+Author-email: aulasparticularesdealemaosp@gmail.com
+License: MIT
+Keywords: adb,android,automation,shell,root
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE.rst
+
+
 # Easier ADB automation 
 
 ## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
 
 ### pip install adbkit
 
 **Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
 
+**28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
+
+```python
+from adbkit import ADBTools
+from kthread_sleep import sleep
+
+adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
+deviceserial = "localhost:5555"
+ADBTools.aa_kill_all_running_adb_instances()
+
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_start_server() # creates a new process which is not a child process
+sleep(3)
+self.aa_connect_to_device()
+self.aa_activate_scrcpy_screenshots_tcp(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+# for a usb connection:
+# self.aa_activate_scrcpy_screenshots_usb(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+
+# each killkey combination can only be used once!
+self.aa_show_screenshot( sleeptime=1, killkeys="ctrl+alt+h")
+
+# How to stop showing screenshots
+# press the killkeys combination "ctrl+alt+h" and call the method aa_kill_show_screenshot to kill all threads
+self.aa_kill_show_screenshot()
+
+# once your done with everything, make sure to close the scrcpy connection:
+self.aa_kill_scrcpy_connection()
+
+```
+
 **10/03/2023: Tesseract with multiprocessing / Bluestacks Hyper-V connect** 
 
 ```python
 # Connects to all Bluestacks Hyper-V devices (dynamic ADB ports)  and returns a DataFrame 
 from adbkit import ADBTools
 ald=ADBTools.connect_to_all_bluestacks_hyperv_devices(    adb_path="C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
 timeout=10,
```

### Comparing `adbkit-0.17/adbkit/__init__.py` & `adbkit-0.18/adbkit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import glob
 import os
 import subprocess
+from collections import deque, defaultdict
 from functools import reduce
 from time import sleep
 from typing import Union
 
 import a_pandas_ex_adb_execute_activities
 import rapidfuzz
 from PIL import Image
@@ -17,14 +18,16 @@
 
 from a_pandas_ex_image_tools import pd_add_image_tools
 from adbescapes import ADBInputEscaped
 
 from adbdevicechanger import AdbChanger
 from bstconnect import connect_to_all_localhost_devices
 from check_if_nan import is_nan
+from cv2imshow.cv2imshow import cv2_imshow_multi
+from taskkill import taskkill_regex_rearch
 from tesseractmultiprocessing import tesser2df
 
 pd_add_adb_execute_activities()
 import kthread
 import numpy as np
 import cv2
 import psutil
@@ -59,20 +62,32 @@
 
 add_imwrite_plus_imread_plus_to_cv2()
 add_imshow_thread_to_cv2()
 from a_pandas_ex_apply_ignore_exceptions import pd_add_apply_ignore_exceptions
 
 pd_add_apply_ignore_exceptions()
 import sys
+from adbblitz import AdbShotUSB, AdbShotTCP, mainprocess
 
 use_root = sys.modules[__name__]
 
 use_root.enabled = False
 pd_add_image_tools()
 
+startupinfo = subprocess.STARTUPINFO()
+creationflags = 0 | subprocess.CREATE_NO_WINDOW
+startupinfo.wShowWindow = subprocess.SW_HIDE
+invisibledict = {
+    "startupinfo": startupinfo,
+    "creationflags": creationflags,
+    "start_new_session": True,
+}
+dequelist = lambda: deque([], 1)
+_screenshots = defaultdict(dequelist)
+
 
 def _draw_shapes_result(image, df, min_area=200):
     for name, group in df.groupby("aa_h3"):
         if name == 0:
             continue
         fabb = (
             np.random.randint(50, 250),
@@ -267,27 +282,43 @@
         command="kill-server",
         exit_keys=exit_keys,
         print_output=print_output,
         timeout=timeout,
     )
 
 
+def kill_all_running_adbs():
+    return taskkill_regex_rearch(
+        dryrun=False,
+        kill_children=True,
+        force_kill=True,
+        flags_title=regex.I,
+        windowtext=".*",
+        flags_windowtext=regex.I,
+        class_name=".*",
+        flags_class_name=regex.I,
+        path=r"\badb.exe$",
+        flags_path=regex.I,
+    )
+
+
 def start_server(
     adb_path,
     exit_keys="ctrl+x",
     print_output=True,
     timeout=None,
 ):
-    return execute_adb_without_shell(
-        adb_path,
-        command="start-server",
-        exit_keys=exit_keys,
-        print_output=print_output,
-        timeout=timeout,
-    )
+    mainprocess([adb_path, "start-server"])
+    # return execute_adb_without_shell(
+    #     adb_path,
+    #     command="start-server",
+    #     exit_keys=exit_keys,
+    #     print_output=print_output,
+    #     timeout=timeout,
+    # )
 
 
 def reboot_and_listen_to_usb(
     adb_path,
     exit_keys="ctrl+x",
     print_output=True,
     timeout=None,
@@ -305,25 +336,42 @@
     _ = subprocess.run(f"{adb_path} start-server", capture_output=True, shell=False)
     _ = subprocess.run(
         f"{adb_path} connect {deviceserial}", capture_output=True, shell=False
     )
 
 
 def get_screen_height_width(adb_path, deviceserial):
-    screenwidth, screenheight = (
-        subprocess.run(
-            rf'{adb_path} -s {deviceserial} shell dumpsys window | grep cur= |tr -s " " | cut -d " " -f 4|cut -d "=" -f 2',
+    try:
+        p = subprocess.run(
+            rf"{adb_path} -s {deviceserial} shell dumpsys window",
             shell=True,
             capture_output=True,
+            **invisibledict,
         )
-        .stdout.decode("utf-8", "ignore")
-        .strip()
-        .split("x")
-    )
-    screenwidth, screenheight = int(screenwidth), int(screenheight)
+        screenwidth, screenheight = [
+            int(x)
+            for x in regex.findall(rb"cur=(\d{,4}x\d{,4}\b)", p.stdout)[0]
+            .lower()
+            .split(b"x")
+        ]
+        print(screenheight, screenwidth)
+
+    except Exception:
+        screenwidth, screenheight = (
+            subprocess.run(
+                rf'{adb_path} -s {deviceserial} shell dumpsys window | grep cur= |tr -s " " | cut -d " " -f 4|cut -d "=" -f 2',
+                shell=True,
+                capture_output=True,
+                **invisibledict,
+            )
+            .stdout.decode("utf-8", "ignore")
+            .strip()
+            .split("x")
+        )
+        screenwidth, screenheight = int(screenwidth), int(screenheight)
     return screenwidth, screenheight
 
 
 def convert_to_ADAPTIVE_THRESH_MEAN_C(im):
     try:
         ima2 = cv2.adaptiveThreshold(
             open_image_in_cv(im, channels_in_output=2),
@@ -442,17 +490,15 @@
     deviceserial,
     alpa,
     folder,
     exit_keys="ctrl+x",
     print_output=False,
     timeout=None,
 ):
-
     for key, item in alpa.iterrows():
-
         apppa = item.aa_path
         savefolder = item.aa_name
         sf = os.path.normpath(os.path.join(folder, savefolder))
         sffile = os.path.normpath(os.path.join(sf, apppa.strip("/").split("/")[-1]))
 
         if not os.path.exists(sf):
             os.makedirs(sf)
@@ -1640,15 +1686,15 @@
                         r"^\s+\*\s+", "Pack: ".ljust(109), k.decode("utf-8", "ignore")
                     )
                     for k in i.splitlines()
                     if regex.findall(r"^\s+", k.decode("utf-8", "ignore"))
                 ]
             )
         )
-        for i in regex.split(b"[\r\n]+\s*[\r\n]+\s*[\r\n]+", b"".join(xx))
+        for i in regex.split(rb"[\r\n]+\s*[\r\n]+\s*[\r\n]+", b"".join(xx))
     ]:
         dfra.columns = range(dfra.shape[1])
         delcol = None
         for col in dfra.columns:
             if not dfra.loc[dfra[col] == "Pack:"].empty:
                 delcol = col
                 dfra.loc[
@@ -2134,15 +2180,14 @@
     email,
     address,
     save=True,
     exit_keys="ctrl+x",
     print_output=True,
     timeout=None,
 ):
-
     reas = execute_multicommands_adb_shell(
         adb_path,
         deviceserial,
         subcommands=[
             f"""am start -a android.intent.action.INSERT \
         -t vnd.android.cursor.dir/contact \
         -e name '{name}' \
@@ -2333,14 +2378,25 @@
     df["aa_adbtools"] = df.localhost.apply(
         lambda x: ADBTools(adb_path=adb_path, deviceserial=f"localhost:{x}")
     )
     df.aa_adbtools.apply(lambda x: x.aa_connect_to_device())
     return df
 
 
+def show_screenshots(title, sleeptime, killkeys="ctrl+alt+h"):
+    while True:
+        sleep(sleeptime)
+        if len(_screenshots[killkeys]) > 0:
+            cv2_imshow_multi(
+                title=title,
+                image=_screenshots[killkeys][0],
+                killkeys=killkeys,  # switch on/off
+            )
+
+
 class ADBTools:
     def __init__(self, adb_path, deviceserial, sdcard="/sdcard/"):
         self.adb_path = adb_path
         self.deviceserial = deviceserial
         self.sdcard = sdcard
         self.tesseractpath = None
         self.bb_adbkeyboard = None
@@ -2349,21 +2405,128 @@
         self.bb_sendevent_touch = None
         self.bb_adbdevicechanger = None
         self.screenshot = None
         self.screenshot_gray = None
         self.tesseract = None
         self.df = None
         self.bb_input_text = None
+        self.scrcpy_screenshot_usb = None
+        self.scrcpy_screenshot_tcp = None
+        self._show_screenshot_thread = None
+        self._add_new_screenshot_thread = None
+        self._screenshotkillkeys = None
 
     def __str__(self):
         return self.deviceserial
 
     def __repr__(self):
         return self.deviceserial
 
+    def _start_show_screenshot(self, title, killkeys="ctrl+alt+h", sleeptime=1):
+        self._add_new_screenshot_thread = kthread.KThread(
+            target=self._add_new_screenshots,
+            name=str(killkeys),
+            args=(sleeptime, killkeys),
+        )
+        self._add_new_screenshot_thread.start()
+        self._show_screenshot_thread = kthread.KThread(
+            target=show_screenshots,
+            name=str(killkeys),
+            args=(title, sleeptime, killkeys),
+        )
+        self._show_screenshot_thread.start()
+
+    def _add_new_screenshots(self, sleeptime, killkeys):
+        self._screenshotkillkeys = killkeys
+        while True:
+            _screenshots[killkeys].append(self.screenshot.copy())
+            sleep(sleeptime)
+
+    def aa_kill_show_screenshot(self):
+        print(
+            f"Press {self._screenshotkillkeys} to close the screenshot window if you haven't closed it yet"
+        )
+        try:
+            if self._add_new_screenshot_thread:
+                while self._add_new_screenshot_thread.is_alive():
+                    self._add_new_screenshot_thread.kill()
+        except Exception:
+            pass
+        try:
+            if self._show_screenshot_thread:
+                while self._show_screenshot_thread.is_alive():
+                    self._show_screenshot_thread.kill()
+        except Exception:
+            pass
+        try:
+            del _screenshots[self._screenshotkillkeys]
+        except Exception:
+            pass
+
+    def aa_kill_scrcpy_connection(self):
+        if self.scrcpy_screenshot_usb:
+            try:
+                self.scrcpy_screenshot_usb.quit()
+            except Exception:
+                pass
+        if self.scrcpy_screenshot_tcp:
+            try:
+                self.scrcpy_screenshot_tcp.quit()
+            except Exception:
+                pass
+
+    def aa_show_screenshot(self, sleeptime=1, killkeys="ctrl+alt+h"):
+        if is_nan(self.screenshot):
+            self.aa_update_screenshot()
+        if killkeys in _screenshots:
+            raise ValueError(f"Killkeys {killkeys} are already being used!")
+        else:
+            print(f"Use {killkeys} to turn imshow on/off")
+            self._start_show_screenshot(str(self.deviceserial), killkeys, sleeptime)
+
+    def aa_activate_scrcpy_screenshots_usb(
+        self, adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0
+    ):
+        self.scrcpy_screenshot_usb = AdbShotUSB(
+            device_serial=self.deviceserial,
+            adb_path=self.adb_path,
+            adb_host_address=adb_host_address,
+            adb_host_port=adb_host_port,
+            sleep_after_exception=0.05,
+            frame_buffer=4,
+            lock_video_orientation=lock_video_orientation,
+            max_frame_rate=0,
+            byte_package_size=131072,
+            scrcpy_server_version="2.0",
+            log_level="info",
+            max_video_width=0,
+            start_server=False,
+            connect_to_device=False,
+        )
+
+    def aa_activate_scrcpy_screenshots_tcp(
+        self, adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0
+    ):
+        self.scrcpy_screenshot_tcp = AdbShotTCP(
+            device_serial=self.deviceserial,
+            adb_path=self.adb_path,
+            ip=adb_host_address,
+            port=adb_host_port,
+            sleep_after_exception=0.05,
+            frame_buffer=4,
+            lock_video_orientation=lock_video_orientation,
+            max_frame_rate=0,
+            byte_package_size=131072,
+            scrcpy_server_version="2.0",
+            log_level="info",
+            max_video_width=0,
+            start_server=False,
+            connect_to_device=False,
+        )
+
     @staticmethod
     def connect_to_all_bluestacks_hyperv_devices(
         adb_path,
         timeout=10,
         bluestacks_config=r"C:\ProgramData\BlueStacks_nxt\bluestacks.conf",
     ):
         return connect_to_all_bluestacks_hyperv_devices(
@@ -2482,21 +2645,26 @@
             tisl = f"sleep {round(ti, 3)}"
             allco.append(coadd)
             allco.append(tisl)
         self.aa_execute_multiple_adb_shell_commands(allco)
         return self
 
     def aa_update_screenshot(self, color_and_gray=True):
-        self.screenshot = next(
-            self.aa_get_screenshots(
-                sleeptime=0,
-                number=1,
-                gray=False,
+        if self.scrcpy_screenshot_tcp:
+            self.screenshot = self.scrcpy_screenshot_tcp.get_one_screenshot()
+        elif self.scrcpy_screenshot_usb:
+            self.screenshot = self.scrcpy_screenshot_usb.get_one_screenshot()
+        else:
+            self.screenshot = next(
+                self.aa_get_screenshots(
+                    sleeptime=0,
+                    number=1,
+                    gray=False,
+                )
             )
-        )
         if color_and_gray:
             self.screenshot_gray = open_image_in_cv(
                 self.screenshot, channels_in_output=2
             )
         return self
 
     def aa_activate_sendevent_touch(
@@ -2675,15 +2843,14 @@
         )
         andf.screenshot = self.screenshot
         andf.get_df_from_activity(with_screenshot=with_screenshot)
         df_activities, _, _ = andf.get_all_results()
         return df_activities
 
     def aa_list_folder_content(self, folder_to_search):
-
         return get_folder_df(self.deviceserial, self.adb_path, folder=folder_to_search)
 
     def aa_list_all_files_on_device(self):
         return get_folder_df(self.deviceserial, self.adb_path, folder="")
 
     def aa_list_all_packages(
         self,
@@ -3112,15 +3279,14 @@
             self.deviceserial,
             exit_keys=exit_keys,
             print_output=print_output,
             timeout=timeout,
         )
 
     def aa_getprop(self, exit_keys="ctrl+x", print_output=True, timeout=None):
-
         return getprop(
             self.adb_path,
             self.deviceserial,
             exit_keys=exit_keys,
             print_output=print_output,
             timeout=timeout,
         )
@@ -3461,15 +3627,14 @@
         self,
         package,
         user=0,
         exit_keys="ctrl+x",
         print_output=True,
         timeout=None,
     ):
-
         return disable_autoupdate_for_package(
             self.adb_path,
             self.deviceserial,
             package,
             user=user,
             exit_keys=exit_keys,
             print_output=print_output,
@@ -3480,15 +3645,14 @@
         self,
         package,
         user=0,
         exit_keys="ctrl+x",
         print_output=True,
         timeout=None,
     ):
-
         return enable_autoupdate_for_package(
             self.adb_path,
             self.deviceserial,
             package,
             user=user,
             exit_keys=exit_keys,
             print_output=print_output,
@@ -3687,15 +3851,14 @@
         sleeptime=1,
         number=1,
         gray=False,
         ADAPTIVE_THRESH_MEAN_C=False,
         ADAPTIVE_THRESH_GAUSSIAN_C=False,
         THRESH_OTSU=False,
     ):
-
         return _get_n_adb_screenshots(
             self.adb_path,
             self.deviceserial,
             sleeptime=sleeptime,
             n=number,
             gray=gray,
             ADAPTIVE_THRESH_MEAN_C=ADAPTIVE_THRESH_MEAN_C,
@@ -3712,14 +3875,16 @@
     def aa_connect_to_device(self):
         connect_to_adb(self.adb_path, self.deviceserial)
 
     def aa_restart_server(self, killadb=True):
         self.aa_kill_server()
         sleep(2)
         if killadb:
+            kill_all_running_adbs()
+
             PROCNAME = "adb.exe"
             for proc in psutil.process_iter():
                 try:
                     if proc.name().lower() == PROCNAME:
                         proc.kill()
                 except Exception:
                     continue
@@ -3738,25 +3903,28 @@
             exit_keys=exit_keys,
             print_output=print_output,
             timeout=timeout,
         )
 
     def aa_start_server(
         self,
-        exit_keys="ctrl+x",
-        print_output=True,
-        timeout=None,
+        *args,
+        **kwargs
+        # exit_keys="ctrl+x",
+        # print_output=True,
+        # timeout=None,
     ):
         start_server(
             self.adb_path,
-            exit_keys=exit_keys,
-            print_output=print_output,
-            timeout=timeout,
         )
 
+    @staticmethod
+    def aa_kill_all_running_adb_instances():
+        return kill_all_running_adbs()
+
     def aa_stop_server(
         self,
         exit_keys="ctrl+x",
         print_output=True,
         timeout=None,
     ):
         stop_server(
@@ -3910,15 +4078,14 @@
             minpercentage=minpercentage,
             maxtolerance=maxtolerance,
         )
 
     def _ocr_with_tesseract_and_fuzzy_search(
         self, df, prefix, allstrings, minpercentage=85, maxtolerance=10
     ):
-
         prefix = "bb_"
         checkpref = [x for x in df.columns if str(x).startswith(prefix)]
         if not checkpref:
             prefix = "aa_"
         # df=update_screenshot_and_get_activities_df(self,screenshotfolder=screenshotfolder)
         drodf = df.dropna(subset=f"{prefix}screenshot").copy()
         tesserscan = drodf.copy()
@@ -4084,15 +4251,14 @@
                     glob.glob(os.path.normpath(os.path.join(x, "bluestacks.conf")))
                     for x in glob.glob(os.environ.get("PROGRAMDATA") + rf"{os.sep}*")
                     if regex.search("bluestacks", x, flags=regex.I)
                 ]
             )
         )[0]
         try:
-
             updatedlines = []
             with open(conffile, mode="rb") as f:
                 data = f.read()
 
             for line in data.splitlines():
                 if b'enable_root_access="' in line:
                     if activate:
```

### Comparing `adbkit-0.17/adbkit/requirements.txt` & `adbkit-0.18/adbkit.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-a_cv2_imshow_thread
-a_cv2_shape_finder
-a_cv_imwrite_imread_plus
-a_pandas_ex_adb_execute_activities
-a_pandas_ex_adb_settings_to_df
-a_pandas_ex_adb_to_df
-a_pandas_ex_apply_ignore_exceptions
-a_pandas_ex_csv_plus
-a_pandas_ex_image_tools
-a_pandas_ex_logcat2df
-a_pandas_ex_tesseract_multirow_regex_fuzz
-adb_grep_search
-adb_unicode_keyboard
-adbdevicechanger
-adbescapes
-androdf
-bstconnect
-check_if_nan
-flatten_everything
-getevent_sendevent
-kthread
-numpy
-opencv_python
-pandas
-Pillow
-psutil
-pyperclip
-rapidfuzz
-regex
-sendevent_getevent_keyboard
-sendevent_touch
-subprocess_print_and_capture
-tesseractmultiprocessing
-touchtouch
+a_cv2_imshow_thread
+a_cv2_shape_finder
+a_cv_imwrite_imread_plus
+a_pandas_ex_adb_execute_activities
+a_pandas_ex_adb_settings_to_df
+a_pandas_ex_adb_to_df
+a_pandas_ex_apply_ignore_exceptions
+a_pandas_ex_csv_plus
+a_pandas_ex_image_tools
+a_pandas_ex_logcat2df
+a_pandas_ex_tesseract_multirow_regex_fuzz
+adb_grep_search
+adb_unicode_keyboard
+adbblitz
+adbdevicechanger
+adbescapes
+androdf
+bstconnect
+check_if_nan
+cv2imshow
+flatten_everything
+getevent_sendevent
+kthread
+numpy
+opencv_python
+pandas
+Pillow
+Pillow
+psutil
+pyperclip
+rapidfuzz
+regex
+sendevent_getevent_keyboard
+sendevent_touch
+subprocess_print_and_capture
+taskkill
+tesseractmultiprocessing
+touchtouch
```

### Comparing `adbkit-0.17/adbkit.egg-info/PKG-INFO` & `adbkit-0.18/adbkit/README.MD`

 * *Files 9% similar despite different names*

```diff
@@ -1,1031 +1,1041 @@
-Metadata-Version: 2.1
-Name: adbkit
-Version: 0.17
-Summary: Big automation package for ADB
-Home-page: https://github.com/hansalemaos/adbkit
-Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
-License: MIT
-Keywords: adb,android,automation,shell,root
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
-# Easier ADB automation 
-
-## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
-
-### pip install adbkit
-
-**Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
-
-**10/03/2023: Tesseract with multiprocessing / Bluestacks Hyper-V connect** 
-
-```python
-# Connects to all Bluestacks Hyper-V devices (dynamic ADB ports)  and returns a DataFrame 
-from adbkit import ADBTools
-ald=ADBTools.connect_to_all_bluestacks_hyperv_devices(    adb_path="C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
-timeout=10,
-bluestacks_config=r"C:\ProgramData\BlueStacks_nxt\bluestacks.conf",)
-
-# Tesseract OCR on all found elements - multiprocessing 
-adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
-deviceserial = "localhost:52249"
-self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
-self.aa_connect_to_device()
-self.aa_activate_tesseract(
-    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
-)
-self.aa_update_screenshot()
-df=self.aa_get_all_displayed_items_from_uiautomator(
-	screenshotfolder="f:\\compare_android2",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
-
-
-      bb_area  bb_bounds  bb_center_x  bb_center_x_cropped  bb_center_y  bb_center_y_cropped  bb_checkable  bb_checked   bb_class  bb_clickable bb_content_desc  bb_cropped_x_end  bb_cropped_x_start  bb_cropped_y_end  bb_cropped_y_start  bb_enabled  bb_focusable  bb_focused  bb_height  bb_height_cropped  bb_index bb_keys_hierarchy  bb_long_clickable  bb_old_index bb_package  bb_password bb_pure_id bb_resource_id bb_screenshot  bb_scrollable  bb_selected bb_shapely    bb_text  bb_valid_square  bb_width  bb_width_cropped  bb_x_end  bb_x_start  bb_y_end  bb_y_start ee_bb_longtouch ee_bb_longtouch_bs ee_bb_longtouch_offset ee_bb_longtouch_offset_bs ee_bb_touch ee_bb_touch_bs ee_bb_touch_offset ee_bb_touch_offset_bs ff_bb_downswipe ff_bb_save_screenshot ff_bb_show_screenshot ff_bb_tap_center_offset ff_bb_tap_center_offset_long ff_bb_tap_center_variation ff_bb_tap_center_variation_long ff_bb_tap_exact_center ff_bb_tap_exact_center_long ff_bb_upswipe bb_scanned_text
-0   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0    (node,)             False                  0     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-1   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  1     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-2   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  2     com.bl...      False    id/con...  androi...      [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-3   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  3     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
-4   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  4     com.bl...      False    id/dra...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-5   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  5     com.bl...      False    id/ite...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-6   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  6     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-7   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 1  (node,...             False                  7     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
-8    771120.0  (44, 8...        800          800                  335          335                False         False     a.q.a.b      False                          1556                44                 590                80                True        True         False         510        510                 0  (node,...             False                  8     com.bl...      False    id/des...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
-9    281464.0  (196, ...        800          800                  783          783                False         False   androi...      False                          1404               196                 900               667                True       False         False         233        233                 3  (node,...             False                  9     com.bl...      False      id/dock  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        667          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
-10   771120.0  (44, 8...        800          800                  335          335                False         False   androi...      False                          1556                44                 590                80                True       False         False         510        510                 0  (node,...             False                 10     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
-11    21744.0  (196, ...        800          800                  685          685                False         False   androi...      False                          1404               196                 694               676                True       False         False          18         18                 0  (node,...             False                 11     com.bl...      False    id/pop...  com.bl...      [[[35,...         False          False    POLYGO...  JOGOS ...       True            1208       1208             1404        196        694        676          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     JOGOS ...     
-12   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 1  (node,...             False                 12     com.bl...      False    id/fra...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
-13    42840.0  (44, 8...        170          170                  165          165                False         False   androi...       True                           296                44                 250                80                True        True         False         170        170                 0  (node,...              True                 13     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              296         44        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Play S...     
-14    42840.0  (296, ...        422          422                  165          165                False         False   androi...       True                           548               296                 250                80                True        True         False         170        170                 1  (node,...              True                 14     com.bl...      False         <NA>                 [[[36,...         False          False    POLYGO...                  True             252        252              548        296        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Centra...     
-15    42840.0  (548, ...        674          674                  165          165                False         False   androi...       True                           800               548                 250                80                True        True         False         170        170                 2  (node,...              True                 15     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              800        548        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Ga ...     
-16    42840.0  (800, ...        926          926                  165          165                False         False   androi...       True                          1052               800                 250                80                True        True         False         170        170                 3  (node,...              True                 16     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1052        800        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Jogue ...     
-17    42840.0  (1052,...       1178         1178                  165          165                False         False   androi...       True                          1304              1052                 250                80                True        True         False         170        170                 4  (node,...              True                 17     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1304       1052        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     IMEI/P...     
-18    42840.0  (1304,...       1430         1430                  165          165                False         False   androi...       True                          1556              1304                 250                80                True        True         False         170        170                 5  (node,...              True                 18     com.bl...      False         <NA>                 [[[38,...         False          False    POLYGO...                  True             252        252             1556       1304        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     SocksD...     
-19   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 0  (node,...             False                 19     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
-20   140128.0  (196, ...        800          800                  842          842                False         False   androi...      False                          1404               196                 900               784                True       False         False         116        116                 1  (node,...             False                 20     com.bl...      False    id/vie...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        784          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-21   197288.0  (258, ...        800          800                  785          785                False         False   androi...      False                          1342               258                 876               694                True       False         False         182        182                 0  (node,...             False                 21     com.bl...      False    id/all...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1084       1084             1342        258        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     a 2e4 ...     
-22    28938.0  (324, ...        403          403                  785          785                False         False   androi...       True                           483               324                 876               694                True        True         False         182        182                 0  (node,...             False                 22     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              483        324        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
-23    28938.0  (483, ...        562          562                  785          785                False         False   androi...       True                           642               483                 876               694                True        True         False         182        182                 1  (node,...             False                 23     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              642        483        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Ly m V...     
-24    28938.0  (642, ...        721          721                  785          785                False         False   androi...       True                           801               642                 876               694                True        True         False         182        182                 2  (node,...             False                 24     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              801        642        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-25    28938.0  (801, ...        880          880                  785          785                False         False   androi...       True                           960               801                 876               694                True        True         False         182        182                 3  (node,...             False                 25     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              960        801        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
-26    28756.0  (960, ...       1039         1039                  785          785                False         False   androi...       True                          1118               960                 876               694                True        True         False         182        182                 4  (node,...             False                 26     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1118        960        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
-27    28756.0  (1118,...       1197         1197                  785          785                False         False   androi...       True                          1276              1118                 876               694                True        True         False         182        182                 5  (node,...             False                 27     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1276       1118        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
-28    10000.0  (353, ...        403          403                  770          770                False         False   androi...      False                           453               353                 820               720                True       False         False         100        100                 0  (node,...             False                 28     com.bl...      False    id/app...  com.bl...      [[[44,...         False          False    POLYGO...                  True             100        100              453        353        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-29     7632.0  (324, ...        403          403                  852          852                False         False   androi...      False                           483               324                 876               828                True       False         False          48         48                 1  (node,...             False                 29     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Street...       True             159        159              483        324        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
-30    10000.0  (512, ...        562          562                  770          770                False         False   androi...      False                           612               512                 820               720                True       False         False         100        100                 0  (node,...             False                 30     com.bl...      False    id/app...  com.bl...      [[[46,...         False          False    POLYGO...                  True             100        100              612        512        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()       a wings     
-31     7632.0  (483, ...        562          562                  852          852                False         False   androi...      False                           642               483                 876               828                True       False         False          48         48                 1  (node,...             False                 31     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Viking...       True             159        159              642        483        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Viking...     
-32    10000.0  (671, ...        721          721                  770          770                False         False   androi...      False                           771               671                 820               720                True       False         False         100        100                 0  (node,...             False                 32     com.bl...      False    id/app...  com.bl...      [[[182...         False          False    POLYGO...                  True             100        100              771        671        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-33     7632.0  (642, ...        721          721                  852          852                False         False   androi...      False                           801               642                 876               828                True       False         False          48         48                 1  (node,...             False                 33     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Draken...       True             159        159              801        642        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Draken...     
-34    10000.0  (830, ...        880          880                  770          770                False         False   androi...      False                           930               830                 820               720                True       False         False         100        100                 0  (node,...             False                 34     com.bl...      False    id/app...  com.bl...      [[[184...         False          False    POLYGO...                  True             100        100              930        830        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-35     7632.0  (801, ...        880          880                  852          852                False         False   androi...      False                           960               801                 876               828                True       False         False          48         48                 1  (node,...             False                 35     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  War Ro...       True             159        159              960        801        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
-36    10000.0  (989, ...       1039         1039                  770          770                False         False   androi...      False                          1089               989                 820               720                True       False         False         100        100                 0  (node,...             False                 36     com.bl...      False    id/app...  com.bl...      [[[243...         False          False    POLYGO...                  True             100        100             1089        989        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-37     7584.0  (960, ...       1039         1039                  852          852                False         False   androi...      False                          1118               960                 876               828                True       False         False          48         48                 1  (node,...             False                 37     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Warspe...       True             158        158             1118        960        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
-38    10000.0  (1147,...       1197         1197                  770          770                False         False   androi...      False                          1247              1147                 820               720                True       False         False         100        100                 0  (node,...             False                 38     com.bl...      False    id/app...  com.bl...      [[[59,...         False          False    POLYGO...                  True             100        100             1247       1147        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-39     7584.0  (1118,...       1197         1197                  852          852                False         False   androi...      False                          1276              1118                 876               828                True       False         False          48         48                 1  (node,...             False                 39     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Dark O...       True             158        158             1276       1118        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
-40      529.0  (745, ...        756          756                  734          734                False         False   androi...      False                           768               745                 746               723                True       False         False          23         23                 0  (node,...             False                 40     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23              768        745        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-41      529.0  (1221,...       1232         1232                  734          734                False         False   androi...      False                          1244              1221                 746               723                True       False         False          23         23                 0  (node,...             False                 41     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23             1244       1221        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
-
-
-
-
-
-self.aa_update_screenshot()
-df = self.aa_get_all_displayed_items_from_activities(
-	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-dftesser=self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
-
-
-      aa_area  aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text
-0       529.0  (427, ...        438          438                  734          734            androi...         False          ...            False                  450               427                 746               723                12     True       True      False         True            c741e85       208936581              23         23          app:id...              True        False          7f08011e  213123...         29        False               True               False            False             True                False                      False               False         id/pop...  [[[103...         False                    False              POLYGO...       True                I           23         23              450         97               427          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              28          27          26          24          22          20           6           5           4           3           2           0                 
-1       529.0  (586, ...        597          597                  734          734            androi...         False          ...            False                  609               586                 746               723                12     True       True      False         True            e9bb4da       245085402              23         23          app:id...              True        False          7f080121  213123...         33        False               True               False            False             True                False                      False               False         id/pop...  [[[187...         False                    False              POLYGO...       True                I           23         23              609         97               586          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              32          31          26          24          22          20           6           5           4           3           2           0                 
-2       529.0  (745, ...        756          756                  734          734            androi...         False          ...            False                  768               745                 746               723                12     True       True      False         True            5a48615        94668309              23         23          app:id...              True        False          7f080120  213123...         37        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23              768         97               745          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              36          35          26          24          22          20           6           5           4           3           2           0                 
-3       529.0  (904, ...        915          915                  734          734            androi...         False          ...            False                  927               904                 746               723                12     True       True      False         True            4029d0b        67280139              23         23          app:id...              True        False          7f08011d  213123...         41        False               True               False            False             True                False                      False               False         id/pop...  [[[255...         False                    False              POLYGO...       True                I           23         23              927         97               904          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              40          39          26          24          22          20           6           5           4           3           2           0                 
-4       529.0  (1063,...       1074         1074                  734          734            androi...         False          ...            False                 1086              1063                 746               723                12     True       True      False         True            27867e8        41445352              23         23          app:id...              True        False          7f08011c  213123...         45        False               True               False            False             True                False                      False               False         id/pop...  [[[65,...         False                    False              POLYGO...       True                I           23         23             1086         97              1063          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              44          43          26          24          22          20           6           5           4           3           2           0                 
-5       529.0  (1221,...       1232         1232                  734          734            androi...         False          ...            False                 1244              1221                 746               723                12     True       True      False         True            125ad2a        19246378              23         23          app:id...              True        False          7f08011f  213123...         49        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23             1244         97              1221          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              48          47          26          24          22          20           6           5           4           3           2           0                 
-6     10000.0  (353, ...        403          403                  770          770            androi...         False          ...            False                  453               353                 820               720                11    False       True      False         True            29caf0f        43822863             100        100          app:id...              True        False          7f080058  213123...         28        False              False               False            False            False                False                      False               False         id/app...  [[[44,...         False                    False              POLYGO...       True                V          100        100              453        129               353          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>                 
-7      7632.0  (324, ...        403          403                  852          852            androi...         False          ...            False                  483               324                 876               828                11     True       True      False         True            ea74b9c       245844892              48         48          app:id...              True        False          7f080060  213123...         30        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              483        159               324           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>   Street...     
-8     10000.0  (512, ...        562          562                  770          770            androi...         False          ...            False                  612               512                 820               720                11    False       True      False         True            cece9a5       216852901             100        100          app:id...              True        False          7f08005b  213123...         32        False              False               False            False            False                False                      False               False         id/app...  [[[46,...         False                    False              POLYGO...       True                V          100        100              612        129               512          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>     a wings     
-9      7632.0  (483, ...        562          562                  852          852            androi...         False          ...            False                  642               483                 876               828                11     True       True      False         True            aadf17a       179171706              48         48          app:id...              True        False          7f080063  213123...         34        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              642        159               483           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>   Viking...     
-10    10000.0  (671, ...        721          721                  770          770            androi...         False          ...            False                  771               671                 820               720                11    False       True      False         True            9ff2d2b       167718187             100        100          app:id...              True        False          7f08005a  213123...         36        False              False               False            False            False                False                      False               False         id/app...  [[[182...         False                    False              POLYGO...       True                V          100        100              771        129               671          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>                 
-11     7632.0  (642, ...        721          721                  852          852            androi...         False          ...            False                  801               642                 876               828                11     True       True      False         True            bab8588       195790216              48         48          app:id...              True        False          7f080062  213123...         38        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              801        159               642           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>   Draken...     
-12    10000.0  (830, ...        880          880                  770          770            androi...         False          ...            False                  930               830                 820               720                11    False       True      False         True            9e77b21       166165281             100        100          app:id...              True        False          7f080057  213123...         40        False              False               False            False            False                False                      False               False         id/app...  [[[184...         False                    False              POLYGO...       True                V          100        100              930        129               830          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>                 
-13     7632.0  (801, ...        880          880                  852          852            androi...         False          ...            False                  960               801                 876               828                11     True       True      False         True            b99ab46       194620230              48         48          app:id...              True        False          7f08005f  213123...         42        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              960        159               801           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>   War Ro...     
-14    10000.0  (989, ...       1039         1039                  770          770            androi...         False          ...            False                 1089               989                 820               720                11    False       True      False         True             c17107        12677383             100        100          app:id...              True        False          7f080056  213123...         44        False              False               False            False            False                False                      False               False         id/app...  [[[243...         False                    False              POLYGO...       True                V          100        100             1089        129               989          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>                 
-15     7584.0  (960, ...       1039         1039                  852          852            androi...         False          ...            False                 1118               960                 876               828                11     True       True      False         True            5377234        87519796              48         48          app:id...              True        False          7f08005e  213123...         46        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1118        158               960           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>   Warspe...     
-16    10000.0  (1147,...       1197         1197                  770          770            androi...         False          ...            False                 1247              1147                 820               720                11    False       True      False         True            59fa85d        94349405             100        100          app:id...              True        False          7f080059  213123...         48        False              False               False            False            False                False                      False               False         id/app...  [[[59,...         False                    False              POLYGO...       True                V          100        100             1247        129              1147          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>                 
-17     7584.0  (1118,...       1197         1197                  852          852            androi...         False          ...            False                 1276              1118                 876               828                11     True       True      False         True            f3535d2       255145426              48         48          app:id...              True        False          7f080061  213123...         50        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1276        158              1118           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>   Dark O...     
-18    30210.0  (324, ...        403          403                  781          781            androi...          True          ...            False                  483               324                 876               686                10    False       True       True         True            18369ed        25389549             190        190          app:id...              True        False          7f080050  213123...         27        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              483        225               324          66                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Street...     
-19    30210.0  (483, ...        562          562                  781          781            androi...          True          ...            False                  642               483                 876               686                10    False       True       True         True            9888022       159940642             190        190          app:id...              True        False          7f080053  213123...         31        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              642        384               483         225                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Ly m V...     
-20    30210.0  (642, ...        721          721                  781          781            androi...          True          ...            False                  801               642                 876               686                10    False       True       True         True            2751ab3        41228979             190        190          app:id...              True        False          7f080052  213123...         35        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              801        543               642         384                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   i Drak...     
-21    30210.0  (801, ...        880          880                  781          781            androi...          True          ...            False                  960               801                 876               686                10    False       True       True         True            3711870        57743472             190        190          app:id...              True        False          7f08004f  213123...         39        False              False               False            False            False                False                      False               False         id/app...  [[[87,...         False                    False              POLYGO...       True                V          159        159              960        702               801         543                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   War Ro...     
-22    30020.0  (960, ...       1039         1039                  781          781            androi...          True          ...            False                 1118               960                 876               686                10    False       True       True         True            339b7e9        54114281             190        190          app:id...              True        False          7f08004e  213123...         43        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1118        860               960         702                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Warspe...     
-23    30020.0  (1118,...       1197         1197                  781          781            androi...          True          ...            False                 1276              1118                 876               686                10    False       True       True         True            cd27c6e       215121006             190        190          app:id...              True        False          7f080051  213123...         47        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1276       1018              1118         860                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Dark O...     
-24      900.0  (785, ...        800          800                  797          797            androi...         False          ...            False                  815               785                 812               782                 9     True       True      False         True            268c7fc        40421372              30         30          app:id...              True        False          7f0800a8  213123...         25        False              False               False            False             True                False                      False               False         id/doc...  [[[35,...         False                    False              POLYGO...       True                G           30         30              815        619               785         589                812        118               782          88                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
-25   205960.0  (258, ...        800          800                  781          781            androi...         False          ...            False                 1342               258                 876               686                 9    False       True      False         True            8a2d3cc       144888780             190        190          app:id...              True        False          7f080048  213123...         26        False              False               False            False            False                False                      False               False         id/all...  [[[35,...         False                    False              POLYGO...       True                V         1084       1084             1342       1146               258          62                876        182               686          -8                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>   Street...     
-26    51579.0  (31, 6...        812          812                   78           78            androi...          True          ...            False                 1594                31                  95                62                 9     True       True       True         True            b601a94       190847636              33         33          app:id...              True        False          7f0800c6  213123...         54        False               True               False            False             True                False                      False               False         id/gro...  [[[35,...         False                    False              POLYGO...       True                V         1563       1563             1594       1588                31          25                 95         53                62          20                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
-27  1179406.0  (43, 9...        800          800                  484          484            com.bl...         False          ...            False                 1557                43                 874                95                 9     True       True      False         True            27c993d        41720125             779        779          app:id...              True        False          7f0800c3  213123...         55        False               True               False            False             True                False                      False               False          id/group  [[[35,...         False                    False              POLYGO...       True                V         1514       1514             1557       1551                43          37                874        832                95          53                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>   Ga u i...     
-28    42840.0  (296, ...        422          422                  165          165            com.bl...          True          ...            False                  548               296                 250                80                 8     True       True       True         True              d801f          884767             170        170               <NA>              True         True              <NA>       <NA>         10        False              False               False            False            False                False                      False               False              <NA>  [[[36,...         False                    False              POLYGO...       True                V          252        252              548        504               296         252                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Centra...     
-29    42840.0  (44, 8...        170          170                  165          165            com.bl...          True          ...            False                  296                44                 250                80                 8     True       True       True         True            9c32f6c       163786604             170        170               <NA>              True         True              <NA>       <NA>         11        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              296        252                44           0                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Play S...     
-30    42840.0  (800, ...        926          926                  165          165            com.bl...          True          ...            False                 1052               800                 250                80                 8     True       True       True         True            a164935       169232693             170        170               <NA>              True         True              <NA>       <NA>         12        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1052       1008               800         756                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Jogue ...     
-31    42840.0  (1052,...       1178         1178                  165          165            com.bl...          True          ...            False                 1304              1052                 250                80                 8     True       True       True         True            9c981ca       164200906             170        170               <NA>              True         True              <NA>       <NA>         13        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1304       1260              1052        1008                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   IMEI/P...     
-32    42840.0  (548, ...        674          674                  165          165            com.bl...          True          ...            False                  800               548                 250                80                 8     True       True       True         True            c93ff3b       211025723             170        170               <NA>              True         True              <NA>       <NA>         14        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              800        756               548         504                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   as Ga ...     
-33    42840.0  (1304,...       1430         1430                  165          165            com.bl...          True          ...            False                 1556              1304                 250                80                 8     True       True       True         True            569d658        90822232             170        170               <NA>              True         True              <NA>       <NA>         15        False              False               False            False            False                False                      False               False              <NA>  [[[38,...         False                    False              POLYGO...       True                V          252        252             1556       1512              1304        1260                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   SocksD...     
-34   140128.0  (196, ...        800          800                  842          842            androi...         False          ...            False                 1404               196                 900               784                 8     True       True      False         True            d395417       221860887             116        116          app:id...              True        False          7f08017f  213123...         23        False              False               False            False            False                False                      False               False         id/vie...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               784          90                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>                 
-35   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 8    False       True      False         True            9d20004       164757508             206        206               <NA>              True        False              <NA>       <NA>         24        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               694           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
-36  1352976.0  (6, 42...        800          800                  468          468            androi...         False          ...            False                 1594                 6                 894                42                 8    False       True      False         True            ebbfee7       247201511             852        852               <NA>              True        False              <NA>       <NA>         53        False               True               False            False             True                False                      False               False              <NA>  [[[39,...         False                    False              POLYGO...       True                V         1588       1588             1594       1594                 6           6                894        858                42           6                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   a | | ...     
-37   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 7     True       True      False         True             49b71b         4831003             510        510               <NA>              True        False              <NA>       <NA>          9        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1512                44           0                590        510                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
-38      225.0  (726, ...        733          733                  620          620            androi...         False          ...            False                  741               726                 628               613                 7     True       True      False         True            1b8c9ce        28887502              15         15          app:id...              True        False          7f0800ef  213123...         18        False               True               False            False             True                False                      False               False         id/loa...  [[[35,...         False                    False              POLYGO...       True                V           15         15              741         25               726          10                628         22               613           7                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
-39     2604.0  (751, ...        813          813                  620          620            androi...         False          ...            False                  875               751                 631               610                 7     True       True      False         True            c7ee0ef       209641711              21         21          app:id...              True        False          7f0800dc  213123...         19        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                V          124        124              875        159               751          35                631         25               610           4                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
-40    21744.0  (196, ...        800          800                  685          685            androi...         False          ...            False                 1404               196                 694               676                 7     True       True      False         True            d6f43b1       225395633              18         18          app:id...              True        False          7f08011b  213123...         21        False              False               False            False            False                False                      False               False         id/pop...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                694         27               676           9                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   JOGOS ...     
-41   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 7    False       True      False         True            ae5f096       182841494             206        206          app:id...              True        False          7f0800bd  213123...         22        False              False               False            False            False                False                      False               False         id/fra...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        233               694          27                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
-42  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 7    False       True      False         True            69044a6       110118054             864        864               <NA>              True        False              <NA>       <NA>         52        False               True               False            False             True                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-43  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 6    False       True      False         True            46dee93        74313363             864        864          app:id...              True        False          7f08006c  213123...          7        False              False               False            False             True                False                      False               False         id/bac...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-44   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 6     True       True       True         True            6affac3       112196291             510        510          app:id...              True        False          7f08009e  213123...          8        False              False               False            False            False                False                      False               False         id/des...  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1556                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
-45    25600.0  (0, 59...        800          800                  598          598            com.bl...         False          ...            False                 1600                 0                 606               590                 6     True       True      False         True            a318ed0       171019984              16         16          app:id...              True        False          7f08009f  213123...         16        False               True               False            False             True                False                      False               False         id/des...  [[[28,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                606        570               590         554                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-46     5070.0  (716, ...        800          800                  621          621            androi...         False          ...            False                  885               716                 636               606                 6    False       True      False         True            57d5ec9        92102345              30         30          app:id...              True        False          7f0800db  213123...         17        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                I          169        169              885        885               716         716                636        600               606         570                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-47   281464.0  (196, ...        800          800                  783          783            androi...         False          ...            False                 1404               196                 900               667                 6    False       True      False         True            d275f40       220684096             233        233          app:id...              True        False          7f0800a7  213123...         20        False              False               False            False            False                False                      False               False           id/dock  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1404               196         196                900        864               667         631                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Street...     
-48  1382400.0  (0, 36...        800          800                  468          468            com.bl...          True          ...            False                 1600                 0                 900                36                 6    False       True       True         True            25d1e01        39656961             864        864          app:id...              True        False          7f0800c4  213123...         51        False               True               False            False             True                False                      False               False         id/gro...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-49    19380.0  (44, 8...         63           63                  335          335            androi...         False          ...            False                   82                44                 590                80                 6     True       True      False         True            4493e79        71908985             510        510          app:id...              True        False          7f0800e5  213123...         56        False              False               False            False            False                False                      False               False         id/lef...  [[[35,...         False                    False              POLYGO...       True                V           38         38               82         82                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-50    19380.0  (1518,...       1537         1537                  335          335            androi...         False          ...            False                 1556              1518                 590                80                 6     True       True      False         True            ecea7be       248424382             510        510          app:id...              True        False          7f08012e  213123...         57        False              False               False            False            False                False                      False               False         id/rig...  [[[37,...         False                    False              POLYGO...       True                V           38         38             1556       1556              1518        1518                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-51  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 5    False       True      False         True            294a77d        43296637             864        864               <NA>              True        False              <NA>       <NA>          6        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-52  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 5     True       True      False         True            c019672       201430642             864        864               <NA>              True        False              <NA>       <NA>         58        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-53  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 4     True       True      False         True            38d79ff        59603455             864        864          app:id...              True        False          7f0800df  213123...          5        False              False               False            False            False                False                      False               False         id/ite...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-54  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 3    False       True       True         True            d8cdd1e       227335454             864        864          app:id...              True        False          7f0800b1  213123...          4        False              False                True            False            False                False                      False               False         id/dra...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                36          36                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
-55  1440000.0  (0, 0,...        800          800                  450          450            androi...         False        an...            False                 1600                 0                 900                 0                 2    False       True      False         True            2b36d59        45313369             900        900               <NA>              True        False              <NA>       <NA>          3        False              False               False            False            False                False                      False               False              <NA>  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
-56        0.0  (0, 0,...          0            0                    0            0            androi...         False      andr...            False                    0                 0                   0                 0                 1    False       True      False        False            812b782       135444354               0          0          androi...              True        False           102018a   16908682          1        False              False               False            False             True                False                      False               False         id/act...        NaN         False                    False              POLYGO...      False                G            0          0                0          0                 0           0                  0          0                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()            <NA>                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
-57  1440000.0  (0, 0,...        800          800                  450          450            androi...         False      andr...            False                 1600                 0                 900                 0                 1    False       True      False         True            5f37da0        99843488             900        900          androi...              True        False           1020002   16908290          2        False              False               False            False            False                False                      False               False         id/con...  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
-
-```
-
-**01/03/2023: Added adbdevicechanger** 
-```python
-# https://github.com/hansalemaos/adbdevicechanger
-# tested with bluestacks - root access
-self.aa_activate_adbdevicechanger()
-self.bb_adbdevicechanger.change_android_id()
-
-b'Row: 0 _id=227, name=device_name, value=OnePlus 5T\r\n'
-Out[7]: ('f7a32086dc724a4a', 'OnePlus 5T')
-
-
-self.bb_adbdevicechanger.change_device_name(
-    modelregex=".*",
-    developerregex=".*",
-    androidfullnameregex=".*",
-    year=">1",
-    month=">0",
-    versionnumberaround=7.05,
-)
-b'Row: 0 _id=2340, name=android_id, value=f7a32086dc724a4a\r\n'
-b'Row: 0 _id=228, name=device_name, value=HTC U11\r\n'
-Out[8]: ('f7a32086dc724a4a', 'HTC U11')
-
-self.bb_adbdevicechanger.change_android_id_and_device_name(
-    modelregex=".*",
-    developerregex=".*",
-    androidfullnameregex=".*",
-    year=">1",
-    month=">0",
-    versionnumberaround=7.05,
-)
-b'Row: 0 _id=2341, name=android_id, value=fb9afc93197942d8\r\n'
-b'Row: 0 _id=229, name=device_name, value=Nokia 8\r\n'
-Out[9]: ('fb9afc93197942d8', 'Nokia 8')
-
-
-self.bb_adbdevicechanger.get_random_android_cellphones(    modelregex="Samsung.*",
-    developerregex=".*",
-    androidfullnameregex=".*",
-    year=">2010",
-    month=">0",
-    versionnumberaround=9.05,
-    howmany=10,
-    return_list=False,)
-Out[13]: 
-                       aa_model  ...              uuid
-0  Samsung Galaxy Note 20/Ultra  ...  36f8a604180b4d7f
-1            Samsung Galaxy A70  ...  cb7f374cd85d4330
-2      Samsung Galaxy A30s/A50s  ...  9380749deb5942f6
-3      Samsung Galaxy Note 10/+  ...  c36816b1906542dc
-4    Samsung Galaxy S20/+/Ultra  ...  33dc12217b404a62
-5         Samsung Galaxy A90 5G  ...  cf0084fa8261465d
-6      Samsung Galaxy A51 5G UW  ...  3177aa09b1fc40d9
-7            Samsung Galaxy A01  ...  44db6d59366143cd
-8         Samsung Galaxy A42 5G  ...  a5b6fb2d08ac4475
-9           Samsung Galaxy A20e  ...  806b4ae287ec4d34
-[10 rows x 10 columns]
-
-```
-
-
-**23/02/2023: New methods**
-```python
-from adbkit import ADBTools
-adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
-deviceserial = "localhost:5555"
-self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
-self.aa_connect_to_device()
-self.aa_activate_tesseract(
-    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
-)
-
-#####################################################################################
-# This method uses Tesseract! You can download it here: https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
-self.aa_update_screenshot() # Update the screenshot before 
-df=self.aa_ocr_elements_from_activities(['Play Store'], # pass all strings as a list 
-minpercentage=85, # fuzzy match
-maxtolerance=10,
-screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-
-    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
-32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
-
-
-
-#####################################################################################
-# Another example (Play Store written wrong)
-
-df2=self.aa_ocr_elements_from_uiautomator(['blai Store'],minpercentage=70, maxtolerance=10, )
-
-    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
-32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
-
-#####################################################################################
-# Pass a list of tuples:
-((x,y),time in seconds)
-
-self.aa_multi_input_tap_with_delay([((100,100),2), ((200,200),3)])
-#####################################################################################
-
-self.aa_input_tap(x=100,y=100)
-
-#####################################################################################
-# https://github.com/hansalemaos/adbescapes
-# Converts Unicode string to ASCII and escapes all characters that need to be escaped. 
-# You have to activate it, before using it. The first start takes some time because numba needs to compile the code 
-self.aa_activate_input_text_formated()
-
-# input 
-text="""
-"'ąćęłń'\tóśźż\nĄĆĘŁŃÓŚŹŻ\n\"Junto à Estação de \nCarcavelos;\"" "äöüÄÖÜß"
-"""
-self.aa_input_text_formated_with_delay(text,delay=(0.01, 0.2),respect_german_letters=False, exit_keys="ctrl+x")
-
-
-# output
-"'aceln'    oszz
-ACELNOSZZ
-"Junto a Estacao de 
-Carcavelos;"" "aouAOUb"
-
-# If you want it the German way :)
-self.aa_input_text_formated(text,respect_german_letters=True, exit_keys="ctrl+x")
-
-"'aceln'    oszz
-ACELNOSZZ
-"Junto a Estacao de 
-Carcavelos;"" "aeoeueAeOeUess"
-#####################################################################################
-self.aa_install_apk_from_hdd(r"C:\Users\Gamer\anaconda3\envs\instcont\instagram.apk")
-#####################################################################################
-self.aa_uninstall_package('com.instagram.lite')
-#####################################################################################
-# First argument is a regex 
-self.aa_copy_apk_to_hdd('com.insta.*', 'c:\\instaapkdownload')
-#####################################################################################
-```
-
-
-
-**17/01/2023: Screenshot fix**
-
-
-```python
-$pip install adbkit
-from adbkit import ADBTools
-adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
-deviceserial = "localhost:5875"
-
-# Create an instance
-# Don't get confused about the instance name "self". I did it because it is faster copying methods from the class 
-self = ADBTools(adb_path, deviceserial, sdcard="/sdcard/")
-self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
-
-# connect to the device 
-self.aa_connect_to_device()
-```
-
-
-
-```python
-# If you are using BlueStacks and want to have root access, call:
-self.aa_root_bluestacks_instances() 
-# This method will basically do this steps: https://appuals.com/root-bluestacks/ to root BlueStacks
-# You can run the script every time you use this module. It won't hurt. 
-# The first time, you might have to restart BlueStacks to enable the root access 
-```
-
-
-
-```python
-# If your device/BlueStacks is rooted, enable root so that all commands will be sent as root 
-self.aa_enable_root() 
-# can be disabled by calling :
-self.aa_disable_root()
-```
-
-
-
-```python
-# Activates self.bb_adbkeyboard 
-# Read more about it: https://github.com/hansalemaos/adb_unicode_keyboard
-self.aa_activate_adb_keyboard(exit_keys="ctrl+x") 
-```
-
-
-
-```python
-# Activates self.bb_sendevent_keyboard (needs root access)
-# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
-
-self.aa_activate_sendevent_keyboard(
-    sdcard="/storage/emulated/0/",
-    tmp_folder_on_sd_card="AUTOMAT",
-    exit_keys="ctrl+x",
-)  # needs root access
-
-# Here is one example: 
-self.bb_adbkeyboard.press_7_keycode_0()
-```
-
-
-
-```python
-# Activates self.self.bb_getevent_sendevent
-# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
-
-self.aa_activate_getevent_sendevent(
-    sdcard="/storage/emulated/0/",
-    tmp_folder_on_sd_card="AUTOMAT",
-    bluestacks_divider=32767,
-    exit_keys="ctrl+x",
-)  # needs root access
-```
-
-
-
-```python
-# Activates self.bb_sendevent_touch
-# Read more about it: https://github.com/hansalemaos/sendevent_touch
-
-self.aa_activate_sendevent_touch(
-    sdcard="/storage/emulated/0/",
-    tmp_folder_on_sd_card="AUTOMAT",
-    bluestacks_divider=32767,
-    use_bluestacks_coordinates=True,
-)  # needs root access
-
-# Here is one example:
-self.bb_sendevent_touch.touch(10,10)
-```
-
-
-
-```python
-# Activates https://github.com/hansalemaos/a_pandas_ex_tesseract_multirow_regex_fuzz
-# You can download the 64 bit version of tesseract here: 
-# https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
-
-self.aa_activate_tesseract(
-        tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
-    )
-
-# Once activated, you can call:
-# self.aa_ocr_with_tesseract()
-
-    left  top  width  height       conf        text  middle_x  middle_y  end_x  end_y
-8    382   42    499      49  37.512093         RH,       631        66    881     91
-9    728   34     98      61  30.925949          2.       777        64    826     95
-13   370  101     37      11   84.72541     'system       388       106    407    112
-14   411  101     24      10  79.929901        Apps       423       106    435    111
-15   536   90     36      28  85.425911      Roblox       554       104    572    118
-16   676  100     55       9  88.744247  BlueStacks       703       104    731    109
-17   735  101      7       8  80.470955           X       738       105    742    109
-18   814  101     31      10  90.271423      Spiele       829       106    845    111
-19   848  101     18       8  93.303749         und       857       105    866    109
-20   869  103     41       9  87.963295     gewinne       889       107    910    112
-28    72  100     20      12  96.004517        Play        82       106     92    112
-29    95  101     27       8  86.986359       Store       108       105    122    109
-33   225  211     49      12  76.804665   Globoplay       249       217    274    223
-37   326  489     25      28  91.894142       Tibia       338       503    351    517
-38   401  500     50       8  91.477989   Guardians       426       504    451    508
-39   455  499     10       9  72.064316          of       460       503    465    508
-41   415  512     37       9  75.078018     Cloudia       433       516    452    521
-
-# and even perform a multiline fuzzy search:
-xxx = self.aa_ocr_with_tesseract(search_for='Kontakte verwalten')
-```
-```python
-# Use this method to update the screenshot 
-# The updated screenshot can be found here: self.screenshot
-self.aa_update_screenshot()
-
-```
-
-
-
-```python
-# get 5 screenshot within 5 seconds
-xx=self.aa_get_screenshots(
-        sleeptime=1,
-        number=5)
-
-```
-
-
-
-```python
-# Now you can use self.df to do operations on the screenshot 
-# More information about a_pandas_ex_image_tools:
-# https://github.com/hansalemaos/a_pandas_ex_image_tools
-self.aa_update_imagedf()
-```
-
-
-```python
-# If you want to capture the logcat output and analyze it in a DataFrame,
-use: 
-logcatcap = self.aa_capture_logcat(
-        exit_keys="ctrl+x",
-        timeout=None,
-    )  
-
-# When you exit using "ctrl+x", the method will return a DataFrame
-# By the way: almost all methods can be interrupted using a key command 
-```
-
-
-
-```python
-# Those 2 methods will help you to identify and interact with views:
-# Read more about it: https://github.com/hansalemaos/androdf
-df1 = self.aa_get_all_displayed_items_from_uiautomator(
-	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-
-df3 = self.aa_get_all_displayed_items_from_activities(
-	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
-	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
-	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
-	loung_touch_delay=(
-		1000,
-		1500,
-	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
-	swipe_variation_startx=10,  # swipe coordinate variations in percent
-	swipe_variation_endx=10,
-	swipe_variation_starty=10,
-	swipe_variation_endy=10,
-	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
-	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
-	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
-)
-```
-
-
-
-```python
-# Uses: https://github.com/hansalemaos/a_pandas_ex_adb_to_df
-# lists all files in DataFrame and adds useful functions
-# self.aa_list_all_files_on_device()
-
-dffiles = self.aa_list_folder_content(folder_to_search="data/")  
-print(dffiles)
-                  aa_date  ... ff_pull_file_cat
-0     2022-12-11 06:48:00  ...               ()
-1     2022-12-26 22:16:00  ...               ()
-2     2022-12-06 19:10:00  ...               ()
-3     2022-12-06 13:38:00  ...               ()
-4     2022-12-26 22:16:00  ...               ()
-                   ...  ...              ...
-26120 2021-09-16 04:21:00  ...               ()
-26121 2021-09-16 03:53:00  ...               ()
-26122 2021-09-16 03:53:00  ...               ()
-26123 2021-09-16 04:35:00  ...               ()
-26124 2021-09-16 04:31:00  ...               ()
-[26125 rows x 16 columns]
-```
-
-
-
-```python
-# Search with grep 
-# Uses https://github.com/hansalemaos/adb_grep_search
-dfgrep = self.aa_grep_search(
-        folder_to_search="data/data",
-        filetype="*.db",
-        regular_expression=r"CREATE.TABLE",
-        exit_keys="ctrl+x",
-        timeout=None,
-        remove_control_characters=True,
-    )
-
-dfgrep
-Out[19]: 
-                                               aa_file  ...      aa_regex
-0    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-1    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-2    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-3    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
-4    data/data/com.globo.globotv/databases/mcsdk_bf...  ...  CREATE.TABLE
-..                                                 ...  ...           ...
-103  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-104  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-105  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-106  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-107  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
-[108 rows x 5 columns]
-```
-
-
-
-```python
-# Uses https://github.com/hansalemaos/a_pandas_ex_adb_settings_to_df
-self.aa_parse_settings_from_all_packages(
-        tempfolder="f:\\tmpfolder", datafolder="data/"
-    )
-
-        index          aa_all_keys  ... level_22 level_23
-0         0.0         (long, name)  ...      NaN      NaN
-1         1.0        (long, value)  ...      NaN      NaN
-2         0.0   (boolean, 0, name)  ...      NaN      NaN
-3         1.0  (boolean, 0, value)  ...      NaN      NaN
-4         2.0   (boolean, 1, name)  ...      NaN      NaN
-       ...                  ...  ...      ...      ...
-110795    NaN            (6, desc)  ...      NaN      NaN
-110796    NaN           (6, label)  ...      NaN      NaN
-110797    NaN             (6, pkg)  ...      NaN      NaN
-110798    NaN          (6, source)  ...      NaN      NaN
-110799    NaN             (6, url)  ...      NaN      NaN
-[110800 rows x 31 columns]
-
-You might see this error messages several times:
-
-"Go to: https://www.sqlite.org/download.html ,
-download the dll and put it in the DLLs folder of your env!"
-
-You can ignore it.
-```
-
-
-
-```python
-#This method helps you find all executable activities from a package 
-# More about it: https://github.com/hansalemaos/a_pandas_ex_adb_execute_activities
-
-self.aa_get_activity_execution_df_from_one_package(
-        packagename="com.roblox.client"
-    ) 
-```
-
-
-
-```python
-# adds new contact, can be saved straight away
-addcon = self.aa_add_new_contact(
-	"hans", "+55119897827552", "hans@something.com", "my address", save=False
-)
-```
-
-
-
-```python
-# If you play Roblox, you can enable/disable some textures to get higher fps
-self.aa_enable_roblox_textures(
-	exit_keys="ctrl+x",
-	print_output=True,
-	timeout=None,
-)
-
-self.aa_disable_roblox_textures(
-	exit_keys="ctrl+x",
-	print_output=True,
-	timeout=None,
-)
-```
-
-
-
-```python
-# goes to the home screen, doesn't close anything
-self.aa_go_to_home_screen()
-```
-
-
-
-```python
-# repeat=5 usually deletes more than 5 characters!!
-self.aa_press_delete_key_repeated_times(repeat=5)
-```
-
-
-
-```python
-# starts the android file manager, pass the file type you want to see
-self.aa_get_content(type_="text/plain")
-```
-
-
-
-```python
-# Here are some methods to get useful information. 
-# Returns DataFrames 
-print(self.aa_whole_dumpsys_to_df())
-print(self.aa_list_all_packages())
-print(self.aa_list_broadcast_stats())
-print(self.aa_list_pending_intents())
-print(self.aa_list_all_activities_from_device())
-print(self.aa_list_all_services())
-print(self.aa_list_all_receivers())
-print(self.aa_list_all_activities())
-print(self.aa_get_procstats())
-print(self.aa_list_all_devices()) # devices on the device (dev ...)
-print(self.aa_list_devices()) # all adb devices (localhost:5555 ...)
-print(self.aa_list_pids_basic())
-print(self.aa_list_pids_complete())
-print(self.aa_list_memory())
-print(self.aa_getprop())
-print(self.aa_list_all_broadcasts())
-print(self.aa_list_all_broadcasts_history())
-print(self.aa_list_users())
-print(self.aa_list_permission_groups())
-print(self.aa_list_disabled_packages())
-print(self.aa_list_apps_in_use())
-print(self.aa_list_3rd_party_packages())
-print(self.aa_list_features())
-```
-
-
-
-```python
-# Smile! :)
-self.aa_open_camera_photo_mode()
-```
-
-
-
-```python
-# works with and without http://
-print(self.aa_open_website("google.com"))
-```
-
-
-
-```python
-# switches to gallery
-self.aa_start_gallery()
-```
-
-
-
-```python
-# cheeeese
-self.aa_take_a_picture()
-```
-
-
-
-```python
-# useful for some apps 
-self.aa_adb_turn_screen_compatibility_off()
-self.aa_adb_turn_screen_compatibility_on()
-```
-
-
-
-```python
-# Be careful! 
-self.aa_remove_file('/sdcard/9.png')
-```
-
-
-
-```python
-# Essential when you use your cell phone (with Whatsapp, Facebook ...) to automize things.
-self.aa_enable_notifications()
-self.aa_disable_notifications()
-```
-
-
-
-```python
-# More useful stuff for notifications
-self.aa_expand_settings() 
-self.aa_expand_notifications()
-```
-
-
-
-```python
-# Changes the screen orientation
-# You can pass:
-# horizontal_upside_down or 2
-# vertical or 1
-# horizontal or 0
-# vertical_upside_down or 3
-self.aa_change_screen_orientation("horizontal")
-```
-
-
-
-```python
-self.aa_get_display_orientation()
-#Out[4]: 0 
-# 0 means horizontal
-```
-
-
-
-```python
-# Sometimes you upload new media files, but you can't see the thumbnails immediately
-# This method updates all thumbnails
-self.aa_rescan_media()
-```
-
-
-
-```python
-# If you are in the middle of a text and want to go to the end of the line
-self.aa_move_to_end_of_line()
-```
-
-
-
-```python
-# Useful keyboard stuff 
-self.aa_hide_keyboard()
-self.aa_is_keyboard_shown()
-```
-
-
-
-```python
-# Doesn't work on BlueStacks, but on my pixel 6 there are no problems
-# (Actually it is not necessary when using BlueStacks hahaha)
-self.aa_is_screen_unlocked()
-```
-
-
-
-```python
-# Don't use this command on BlueStacks, you will have to reboot the device
-self.aa_lock_screen()
-```
-
-
-
-```python
-# Useful commands 
-self.aa_press_home() #back to home screen
-self.aa_press_app_switch()
-```
-
-
-
-```python
-# Configured for my Pixel 6, but should work on any device with a 
-# newer android version. 
-self.aa_swipe_up_to_unlock_screen('3333')
-```
-
-
-
-```python
-# doesn't work with BlueStacks, because of the app switch design, 
-# but it does on my pixel and should work with any device that 
-# has a recent Android version
-self.aa_close_all_apps_with_swipe()
-```
-
-
-
-```python
-# uninstalls a package
-self.aa_uninstall_package('com.google.android.youtube')
-```
-
-
-
-```python
-# Returns the activity needed to open the package 
-self.aa_resolve_activity('com.roblox.client')
-b'priority=0 preferredOrder=0 match=0x108000 specificIndex=-1 isDefault=true\r\n'
-b'com.roblox.client/.startup.ActivitySplash\r\n'
-```
-
-
-
-```python
-# But you can also open any package using:
-self.aa_open_app('com.roblox.client')
-```
-
-
-
-```python
-# This method makes swiping easy
-# x (start), y (start), x (end) y (end), last number in seconds
-self.aa_swipe(500, 400, 500, 100, 1.1) 
-```
-
-
-
-```python
-#opens a separate shell window using cmd.exe 
-self.aa_open_shell() 
-```
-
-
-
-```python
-# It changes the dictionary that you are in
-# and executes a command 
-self.aa_change_cwd_and_execute_adb_shell('ls', 'data/')
-b'5.3.10.1001\r\n'
-b'5.9.300.1014\r\n'
-b'adb\r\n'
-b'anr\r\n'
-b'app\r\n'
-b'app-asec\r\n'
-b'app-ephemeral\r\n'
-b'app-lib\r\n'
-b'app-private\r\n'
-b'arm\r\n'
-....
-```
-
-
-
-```python
-# This can also be accomplished by sending multiple commands: 
-self.aa_execute_multiple_adb_shell_commands(['cd data/', 'ls|grep system'])
-Out[28]: [b'system\r\n', b'system_ce\r\n', b'system_de\r\n']
-```
-
-
-
-```python
-# You can also send non-shell commands: 
-self.aa_execute_non_shell_adb_command('devices')
-```
-
-
-
-```python
-# This method pushes a file to your sdcard:
-self.aa_push_to_sdcard(r'F:\donedone.png')
-```
-
-
-
-```python
-# This method pulls a file to your hdd
-self.aa_pull('/sdcard/donedone.png', 'f:\\dfdffasd')
-```
-
-
-
-```python
-# A fast way of scanning all connected devices:
-# start/end means the ports you want to start/end with
-# After 10 seconds, all processes that have not completed the search
-# will be killed 
-self.aa_connect_do_all_devices(start=4999, end=6000, timeout=10)
-    '''self.aa_list_devices()
-b'List of devices attached\r\n'
-b'localhost:5037\toffline\r\n'
-b'localhost:5040\toffline\r\n'
-b'localhost:5357\toffline\r\n'
-b'localhost:5725\tdevice\r\n'
-b'localhost:5800\toffline\r\n'
-b'localhost:5875\tdevice\r\n'
-b'localhost:5900\toffline\r\n'
-b'localhost:5955\tdevice\r\n'
-b'\r\n'''
-
-    '''
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process
-Killing the process'''
-```
-
-
-
-```python
-# Uses https://github.com/hansalemaos/a_cv2_shape_finder 
-# to detect shapes in the screenshot 
-self.get_shapes_from_screenshot_THRESH_OTSU()
-self.get_shapes_from_screenshot_ADAPTIVE_THRESH_MEAN_C()
-self.get_shapes_from_screenshot_ADAPTIVE_THRESH_GAUSSIAN_C()
-```
-
-
-
-```python
-#Some self-explaining stuff  
-
-self.aa_isfolder('/sdcard/donedone.png')
-False
-self.aa_isfolder('/sdcard/')
-True
-next(self.aa_get_screenshots())
-
-self.aa_path_exists('/sdcard/')
-True
-self.aa_path_exists('/sdcard2/')
-False
-
-self.aa_get_screen_resolution()
-(960, 540)
-
-self.aa_restart_server()
-self.aa_reboot_and_listen_to_usb()
-self.aa_start_server()
-self.aa_stop_server()
-self.aa_kill_server()
-self.aa_force_stop('com.roblox.client') #root
-self.aa_show_screenshot_in_browser()
-```
-
+# Easier ADB automation 
+
+## Tested against Windows 10, Python 3.9.13, BlueStacks 5.9.300.1014 N32
+### Cygwin is necessary: https://www.cygwin.com/setup-x86_64.exe and needs to be added to the path variable!
+
+### pip install adbkit
+
+**Don't get confused about the instance "self". I did it because it is faster copying methods from the class :)** 
+
+**28/05/2023: Added fast screenshots with scrcpy - no root required and some other methods** 
+
+```python
+from adbkit import ADBTools
+from kthread_sleep import sleep
+
+adb_path = r'C:\ProgramData\chocolatey\bin\adb.exe'
+deviceserial = "localhost:5555"
+ADBTools.aa_kill_all_running_adb_instances()
+
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_start_server() # creates a new process which is not a child process
+sleep(3)
+self.aa_connect_to_device()
+self.aa_activate_scrcpy_screenshots_tcp(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+# for a usb connection:
+# self.aa_activate_scrcpy_screenshots_usb(adb_host_address="127.0.0.1", adb_host_port=5037, lock_video_orientation=0)
+
+
+# each killkey combination can only be used once!
+self.aa_show_screenshot( sleeptime=1, killkeys="ctrl+alt+h")
+
+# How to stop showing screenshots
+# press the killkeys combination "ctrl+alt+h" and call the method aa_kill_show_screenshot to kill all threads
+self.aa_kill_show_screenshot()
+
+# once your done with everything, make sure to close the scrcpy connection:
+self.aa_kill_scrcpy_connection()
+
+```
+
+**10/03/2023: Tesseract with multiprocessing / Bluestacks Hyper-V connect** 
+
+```python
+# Connects to all Bluestacks Hyper-V devices (dynamic ADB ports)  and returns a DataFrame 
+from adbkit import ADBTools
+ald=ADBTools.connect_to_all_bluestacks_hyperv_devices(    adb_path="C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
+timeout=10,
+bluestacks_config=r"C:\ProgramData\BlueStacks_nxt\bluestacks.conf",)
+
+# Tesseract OCR on all found elements - multiprocessing 
+adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
+deviceserial = "localhost:52249"
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_connect_to_device()
+self.aa_activate_tesseract(
+    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
+)
+self.aa_update_screenshot()
+df=self.aa_get_all_displayed_items_from_uiautomator(
+	screenshotfolder="f:\\compare_android2",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
+
+
+      bb_area  bb_bounds  bb_center_x  bb_center_x_cropped  bb_center_y  bb_center_y_cropped  bb_checkable  bb_checked   bb_class  bb_clickable bb_content_desc  bb_cropped_x_end  bb_cropped_x_start  bb_cropped_y_end  bb_cropped_y_start  bb_enabled  bb_focusable  bb_focused  bb_height  bb_height_cropped  bb_index bb_keys_hierarchy  bb_long_clickable  bb_old_index bb_package  bb_password bb_pure_id bb_resource_id bb_screenshot  bb_scrollable  bb_selected bb_shapely    bb_text  bb_valid_square  bb_width  bb_width_cropped  bb_x_end  bb_x_start  bb_y_end  bb_y_start ee_bb_longtouch ee_bb_longtouch_bs ee_bb_longtouch_offset ee_bb_longtouch_offset_bs ee_bb_touch ee_bb_touch_bs ee_bb_touch_offset ee_bb_touch_offset_bs ff_bb_downswipe ff_bb_save_screenshot ff_bb_show_screenshot ff_bb_tap_center_offset ff_bb_tap_center_offset_long ff_bb_tap_center_variation ff_bb_tap_center_variation_long ff_bb_tap_exact_center ff_bb_tap_exact_center_long ff_bb_upswipe bb_scanned_text
+0   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0    (node,)             False                  0     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+1   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  1     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+2   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  2     com.bl...      False    id/con...  androi...      [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+3   1440000.0  (0, 0,...        800          800                  450          450                False         False   androi...      False                          1600                 0                 900                 0                True       False         False         900        900                 0  (node,...             False                  3     com.bl...      False         <NA>                 [[[144...         False          False    POLYGO...                  True            1600       1600             1600          0        900          0          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Size: ...     
+4   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  4     com.bl...      False    id/dra...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+5   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  5     com.bl...      False    id/ite...  com.bl...      [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+6   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 0  (node,...             False                  6     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+7   1382400.0  (0, 36...        800          800                  468          468                False         False   androi...      False                          1600                 0                 900                36                True       False         False         864        864                 1  (node,...             False                  7     com.bl...      False         <NA>                 [[[32,...         False          False    POLYGO...                  True            1600       1600             1600          0        900         36          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     m6: Â«...     
+8    771120.0  (44, 8...        800          800                  335          335                False         False     a.q.a.b      False                          1556                44                 590                80                True        True         False         510        510                 0  (node,...             False                  8     com.bl...      False    id/des...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
+9    281464.0  (196, ...        800          800                  783          783                False         False   androi...      False                          1404               196                 900               667                True       False         False         233        233                 3  (node,...             False                  9     com.bl...      False      id/dock  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        667          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
+10   771120.0  (44, 8...        800          800                  335          335                False         False   androi...      False                          1556                44                 590                80                True       False         False         510        510                 0  (node,...             False                 10     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1512       1512             1556         44        590         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Â¥ ...     
+11    21744.0  (196, ...        800          800                  685          685                False         False   androi...      False                          1404               196                 694               676                True       False         False          18         18                 0  (node,...             False                 11     com.bl...      False    id/pop...  com.bl...      [[[35,...         False          False    POLYGO...  JOGOS ...       True            1208       1208             1404        196        694        676          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     JOGOS ...     
+12   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 1  (node,...             False                 12     com.bl...      False    id/fra...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
+13    42840.0  (44, 8...        170          170                  165          165                False         False   androi...       True                           296                44                 250                80                True        True         False         170        170                 0  (node,...              True                 13     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              296         44        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Play S...     
+14    42840.0  (296, ...        422          422                  165          165                False         False   androi...       True                           548               296                 250                80                True        True         False         170        170                 1  (node,...              True                 14     com.bl...      False         <NA>                 [[[36,...         False          False    POLYGO...                  True             252        252              548        296        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Centra...     
+15    42840.0  (548, ...        674          674                  165          165                False         False   androi...       True                           800               548                 250                80                True        True         False         170        170                 2  (node,...              True                 15     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252              800        548        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     as Ga ...     
+16    42840.0  (800, ...        926          926                  165          165                False         False   androi...       True                          1052               800                 250                80                True        True         False         170        170                 3  (node,...              True                 16     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1052        800        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Jogue ...     
+17    42840.0  (1052,...       1178         1178                  165          165                False         False   androi...       True                          1304              1052                 250                80                True        True         False         170        170                 4  (node,...              True                 17     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True             252        252             1304       1052        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     IMEI/P...     
+18    42840.0  (1304,...       1430         1430                  165          165                False         False   androi...       True                          1556              1304                 250                80                True        True         False         170        170                 5  (node,...              True                 18     com.bl...      False         <NA>                 [[[38,...         False          False    POLYGO...                  True             252        252             1556       1304        250         80          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     SocksD...     
+19   248848.0  (196, ...        800          800                  797          797                False         False   androi...      False                          1404               196                 900               694                True       False         False         206        206                 0  (node,...             False                 19     com.bl...      False         <NA>                 [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Â¥ 4 e...     
+20   140128.0  (196, ...        800          800                  842          842                False         False   androi...      False                          1404               196                 900               784                True       False         False         116        116                 1  (node,...             False                 20     com.bl...      False    id/vie...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1208       1208             1404        196        900        784          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+21   197288.0  (258, ...        800          800                  785          785                False         False   androi...      False                          1342               258                 876               694                True       False         False         182        182                 0  (node,...             False                 21     com.bl...      False    id/all...  com.bl...      [[[35,...         False          False    POLYGO...                  True            1084       1084             1342        258        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     a 2e4 ...     
+22    28938.0  (324, ...        403          403                  785          785                False         False   androi...       True                           483               324                 876               694                True        True         False         182        182                 0  (node,...             False                 22     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              483        324        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
+23    28938.0  (483, ...        562          562                  785          785                False         False   androi...       True                           642               483                 876               694                True        True         False         182        182                 1  (node,...             False                 23     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              642        483        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Ly m V...     
+24    28938.0  (642, ...        721          721                  785          785                False         False   androi...       True                           801               642                 876               694                True        True         False         182        182                 2  (node,...             False                 24     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              801        642        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+25    28938.0  (801, ...        880          880                  785          785                False         False   androi...       True                           960               801                 876               694                True        True         False         182        182                 3  (node,...             False                 25     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             159        159              960        801        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
+26    28756.0  (960, ...       1039         1039                  785          785                False         False   androi...       True                          1118               960                 876               694                True        True         False         182        182                 4  (node,...             False                 26     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1118        960        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
+27    28756.0  (1118,...       1197         1197                  785          785                False         False   androi...       True                          1276              1118                 876               694                True        True         False         182        182                 5  (node,...             False                 27     com.bl...      False    id/app...  com.bl...      [[[35,...         False          False    POLYGO...                  True             158        158             1276       1118        876        694          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
+28    10000.0  (353, ...        403          403                  770          770                False         False   androi...      False                           453               353                 820               720                True       False         False         100        100                 0  (node,...             False                 28     com.bl...      False    id/app...  com.bl...      [[[44,...         False          False    POLYGO...                  True             100        100              453        353        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+29     7632.0  (324, ...        403          403                  852          852                False         False   androi...      False                           483               324                 876               828                True       False         False          48         48                 1  (node,...             False                 29     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Street...       True             159        159              483        324        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Street...     
+30    10000.0  (512, ...        562          562                  770          770                False         False   androi...      False                           612               512                 820               720                True       False         False         100        100                 0  (node,...             False                 30     com.bl...      False    id/app...  com.bl...      [[[46,...         False          False    POLYGO...                  True             100        100              612        512        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()       a wings     
+31     7632.0  (483, ...        562          562                  852          852                False         False   androi...      False                           642               483                 876               828                True       False         False          48         48                 1  (node,...             False                 31     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Viking...       True             159        159              642        483        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Viking...     
+32    10000.0  (671, ...        721          721                  770          770                False         False   androi...      False                           771               671                 820               720                True       False         False         100        100                 0  (node,...             False                 32     com.bl...      False    id/app...  com.bl...      [[[182...         False          False    POLYGO...                  True             100        100              771        671        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+33     7632.0  (642, ...        721          721                  852          852                False         False   androi...      False                           801               642                 876               828                True       False         False          48         48                 1  (node,...             False                 33     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Draken...       True             159        159              801        642        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Draken...     
+34    10000.0  (830, ...        880          880                  770          770                False         False   androi...      False                           930               830                 820               720                True       False         False         100        100                 0  (node,...             False                 34     com.bl...      False    id/app...  com.bl...      [[[184...         False          False    POLYGO...                  True             100        100              930        830        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+35     7632.0  (801, ...        880          880                  852          852                False         False   androi...      False                           960               801                 876               828                True       False         False          48         48                 1  (node,...             False                 35     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  War Ro...       True             159        159              960        801        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     War Ro...     
+36    10000.0  (989, ...       1039         1039                  770          770                False         False   androi...      False                          1089               989                 820               720                True       False         False         100        100                 0  (node,...             False                 36     com.bl...      False    id/app...  com.bl...      [[[243...         False          False    POLYGO...                  True             100        100             1089        989        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+37     7584.0  (960, ...       1039         1039                  852          852                False         False   androi...      False                          1118               960                 876               828                True       False         False          48         48                 1  (node,...             False                 37     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Warspe...       True             158        158             1118        960        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Warspe...     
+38    10000.0  (1147,...       1197         1197                  770          770                False         False   androi...      False                          1247              1147                 820               720                True       False         False         100        100                 0  (node,...             False                 38     com.bl...      False    id/app...  com.bl...      [[[59,...         False          False    POLYGO...                  True             100        100             1247       1147        820        720          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+39     7584.0  (1118,...       1197         1197                  852          852                False         False   androi...      False                          1276              1118                 876               828                True       False         False          48         48                 1  (node,...             False                 39     com.bl...      False    id/app...  com.bl...      [[[53,...         False          False    POLYGO...  Dark O...       True             158        158             1276       1118        876        828          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()     Dark O...     
+40      529.0  (745, ...        756          756                  734          734                False         False   androi...      False                           768               745                 746               723                True       False         False          23         23                 0  (node,...             False                 40     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23              768        745        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+41      529.0  (1221,...       1232         1232                  734          734                False         False   androi...      False                          1244              1221                 746               723                True       False         False          23         23                 0  (node,...             False                 41     com.bl...      False    id/pop...  com.bl...      [[[0, ...         False          False    POLYGO...                  True              23         23             1244       1221        746        723          ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()                   
+
+
+
+
+
+self.aa_update_screenshot()
+df = self.aa_get_all_displayed_items_from_activities(
+	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+dftesser=self.aa_ocr_df_with_tesseract_multiprocessing(df,language='eng', cpus=5)
+
+
+      aa_area  aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text
+0       529.0  (427, ...        438          438                  734          734            androi...         False          ...            False                  450               427                 746               723                12     True       True      False         True            c741e85       208936581              23         23          app:id...              True        False          7f08011e  213123...         29        False               True               False            False             True                False                      False               False         id/pop...  [[[103...         False                    False              POLYGO...       True                I           23         23              450         97               427          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              28          27          26          24          22          20           6           5           4           3           2           0                 
+1       529.0  (586, ...        597          597                  734          734            androi...         False          ...            False                  609               586                 746               723                12     True       True      False         True            e9bb4da       245085402              23         23          app:id...              True        False          7f080121  213123...         33        False               True               False            False             True                False                      False               False         id/pop...  [[[187...         False                    False              POLYGO...       True                I           23         23              609         97               586          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              32          31          26          24          22          20           6           5           4           3           2           0                 
+2       529.0  (745, ...        756          756                  734          734            androi...         False          ...            False                  768               745                 746               723                12     True       True      False         True            5a48615        94668309              23         23          app:id...              True        False          7f080120  213123...         37        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23              768         97               745          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              36          35          26          24          22          20           6           5           4           3           2           0                 
+3       529.0  (904, ...        915          915                  734          734            androi...         False          ...            False                  927               904                 746               723                12     True       True      False         True            4029d0b        67280139              23         23          app:id...              True        False          7f08011d  213123...         41        False               True               False            False             True                False                      False               False         id/pop...  [[[255...         False                    False              POLYGO...       True                I           23         23              927         97               904          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              40          39          26          24          22          20           6           5           4           3           2           0                 
+4       529.0  (1063,...       1074         1074                  734          734            androi...         False          ...            False                 1086              1063                 746               723                12     True       True      False         True            27867e8        41445352              23         23          app:id...              True        False          7f08011c  213123...         45        False               True               False            False             True                False                      False               False         id/pop...  [[[65,...         False                    False              POLYGO...       True                I           23         23             1086         97              1063          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              44          43          26          24          22          20           6           5           4           3           2           0                 
+5       529.0  (1221,...       1232         1232                  734          734            androi...         False          ...            False                 1244              1221                 746               723                12     True       True      False         True            125ad2a        19246378              23         23          app:id...              True        False          7f08011f  213123...         49        False              False               False            False            False                False                      False               False         id/pop...  [[[0, ...         False                    False              POLYGO...       True                V           23         23             1244         97              1221          74                746         26               723           3                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              48          47          26          24          22          20           6           5           4           3           2           0                 
+6     10000.0  (353, ...        403          403                  770          770            androi...         False          ...            False                  453               353                 820               720                11    False       True      False         True            29caf0f        43822863             100        100          app:id...              True        False          7f080058  213123...         28        False              False               False            False            False                False                      False               False         id/app...  [[[44,...         False                    False              POLYGO...       True                V          100        100              453        129               353          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>                 
+7      7632.0  (324, ...        403          403                  852          852            androi...         False          ...            False                  483               324                 876               828                11     True       True      False         True            ea74b9c       245844892              48         48          app:id...              True        False          7f080060  213123...         30        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              483        159               324           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              27          26          24          22          20           6           5           4           3           2           0        <NA>   Street...     
+8     10000.0  (512, ...        562          562                  770          770            androi...         False          ...            False                  612               512                 820               720                11    False       True      False         True            cece9a5       216852901             100        100          app:id...              True        False          7f08005b  213123...         32        False              False               False            False            False                False                      False               False         id/app...  [[[46,...         False                    False              POLYGO...       True                V          100        100              612        129               512          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>     a wings     
+9      7632.0  (483, ...        562          562                  852          852            androi...         False          ...            False                  642               483                 876               828                11     True       True      False         True            aadf17a       179171706              48         48          app:id...              True        False          7f080063  213123...         34        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              642        159               483           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              31          26          24          22          20           6           5           4           3           2           0        <NA>   Viking...     
+10    10000.0  (671, ...        721          721                  770          770            androi...         False          ...            False                  771               671                 820               720                11    False       True      False         True            9ff2d2b       167718187             100        100          app:id...              True        False          7f08005a  213123...         36        False              False               False            False            False                False                      False               False         id/app...  [[[182...         False                    False              POLYGO...       True                V          100        100              771        129               671          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>                 
+11     7632.0  (642, ...        721          721                  852          852            androi...         False          ...            False                  801               642                 876               828                11     True       True      False         True            bab8588       195790216              48         48          app:id...              True        False          7f080062  213123...         38        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              801        159               642           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              35          26          24          22          20           6           5           4           3           2           0        <NA>   Draken...     
+12    10000.0  (830, ...        880          880                  770          770            androi...         False          ...            False                  930               830                 820               720                11    False       True      False         True            9e77b21       166165281             100        100          app:id...              True        False          7f080057  213123...         40        False              False               False            False            False                False                      False               False         id/app...  [[[184...         False                    False              POLYGO...       True                V          100        100              930        129               830          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>                 
+13     7632.0  (801, ...        880          880                  852          852            androi...         False          ...            False                  960               801                 876               828                11     True       True      False         True            b99ab46       194620230              48         48          app:id...              True        False          7f08005f  213123...         42        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          159        159              960        159               801           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              39          26          24          22          20           6           5           4           3           2           0        <NA>   War Ro...     
+14    10000.0  (989, ...       1039         1039                  770          770            androi...         False          ...            False                 1089               989                 820               720                11    False       True      False         True             c17107        12677383             100        100          app:id...              True        False          7f080056  213123...         44        False              False               False            False            False                False                      False               False         id/app...  [[[243...         False                    False              POLYGO...       True                V          100        100             1089        129               989          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>                 
+15     7584.0  (960, ...       1039         1039                  852          852            androi...         False          ...            False                 1118               960                 876               828                11     True       True      False         True            5377234        87519796              48         48          app:id...              True        False          7f08005e  213123...         46        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1118        158               960           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              43          26          24          22          20           6           5           4           3           2           0        <NA>   Warspe...     
+16    10000.0  (1147,...       1197         1197                  770          770            androi...         False          ...            False                 1247              1147                 820               720                11    False       True      False         True            59fa85d        94349405             100        100          app:id...              True        False          7f080059  213123...         48        False              False               False            False            False                False                      False               False         id/app...  [[[59,...         False                    False              POLYGO...       True                V          100        100             1247        129              1147          29                820        134               720          34                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>                 
+17     7584.0  (1118,...       1197         1197                  852          852            androi...         False          ...            False                 1276              1118                 876               828                11     True       True      False         True            f3535d2       255145426              48         48          app:id...              True        False          7f080061  213123...         50        False              False               False            False            False                False                      False               False         id/app...  [[[53,...         False                    False              POLYGO...       True                V          158        158             1276        158              1118           0                876        190               828         142                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              47          26          24          22          20           6           5           4           3           2           0        <NA>   Dark O...     
+18    30210.0  (324, ...        403          403                  781          781            androi...          True          ...            False                  483               324                 876               686                10    False       True       True         True            18369ed        25389549             190        190          app:id...              True        False          7f080050  213123...         27        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              483        225               324          66                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Street...     
+19    30210.0  (483, ...        562          562                  781          781            androi...          True          ...            False                  642               483                 876               686                10    False       True       True         True            9888022       159940642             190        190          app:id...              True        False          7f080053  213123...         31        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              642        384               483         225                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Ly m V...     
+20    30210.0  (642, ...        721          721                  781          781            androi...          True          ...            False                  801               642                 876               686                10    False       True       True         True            2751ab3        41228979             190        190          app:id...              True        False          7f080052  213123...         35        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          159        159              801        543               642         384                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   i Drak...     
+21    30210.0  (801, ...        880          880                  781          781            androi...          True          ...            False                  960               801                 876               686                10    False       True       True         True            3711870        57743472             190        190          app:id...              True        False          7f08004f  213123...         39        False              False               False            False            False                False                      False               False         id/app...  [[[87,...         False                    False              POLYGO...       True                V          159        159              960        702               801         543                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   War Ro...     
+22    30020.0  (960, ...       1039         1039                  781          781            androi...          True          ...            False                 1118               960                 876               686                10    False       True       True         True            339b7e9        54114281             190        190          app:id...              True        False          7f08004e  213123...         43        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1118        860               960         702                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Warspe...     
+23    30020.0  (1118,...       1197         1197                  781          781            androi...          True          ...            False                 1276              1118                 876               686                10    False       True       True         True            cd27c6e       215121006             190        190          app:id...              True        False          7f080051  213123...         47        False              False               False            False            False                False                      False               False         id/app...  [[[35,...         False                    False              POLYGO...       True                V          158        158             1276       1018              1118         860                876        190               686           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              26          24          22          20           6           5           4           3           2           0        <NA>        <NA>   Dark O...     
+24      900.0  (785, ...        800          800                  797          797            androi...         False          ...            False                  815               785                 812               782                 9     True       True      False         True            268c7fc        40421372              30         30          app:id...              True        False          7f0800a8  213123...         25        False              False               False            False             True                False                      False               False         id/doc...  [[[35,...         False                    False              POLYGO...       True                G           30         30              815        619               785         589                812        118               782          88                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
+25   205960.0  (258, ...        800          800                  781          781            androi...         False          ...            False                 1342               258                 876               686                 9    False       True      False         True            8a2d3cc       144888780             190        190          app:id...              True        False          7f080048  213123...         26        False              False               False            False            False                False                      False               False         id/all...  [[[35,...         False                    False              POLYGO...       True                V         1084       1084             1342       1146               258          62                876        182               686          -8                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              24          22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>   Street...     
+26    51579.0  (31, 6...        812          812                   78           78            androi...          True          ...            False                 1594                31                  95                62                 9     True       True       True         True            b601a94       190847636              33         33          app:id...              True        False          7f0800c6  213123...         54        False               True               False            False             True                False                      False               False         id/gro...  [[[35,...         False                    False              POLYGO...       True                V         1563       1563             1594       1588                31          25                 95         53                62          20                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>                 
+27  1179406.0  (43, 9...        800          800                  484          484            com.bl...         False          ...            False                 1557                43                 874                95                 9     True       True      False         True            27c993d        41720125             779        779          app:id...              True        False          7f0800c3  213123...         55        False               True               False            False             True                False                      False               False          id/group  [[[35,...         False                    False              POLYGO...       True                V         1514       1514             1557       1551                43          37                874        832                95          53                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              53          52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>   Ga u i...     
+28    42840.0  (296, ...        422          422                  165          165            com.bl...          True          ...            False                  548               296                 250                80                 8     True       True       True         True              d801f          884767             170        170               <NA>              True         True              <NA>       <NA>         10        False              False               False            False            False                False                      False               False              <NA>  [[[36,...         False                    False              POLYGO...       True                V          252        252              548        504               296         252                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Centra...     
+29    42840.0  (44, 8...        170          170                  165          165            com.bl...          True          ...            False                  296                44                 250                80                 8     True       True       True         True            9c32f6c       163786604             170        170               <NA>              True         True              <NA>       <NA>         11        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              296        252                44           0                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Play S...     
+30    42840.0  (800, ...        926          926                  165          165            com.bl...          True          ...            False                 1052               800                 250                80                 8     True       True       True         True            a164935       169232693             170        170               <NA>              True         True              <NA>       <NA>         12        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1052       1008               800         756                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Jogue ...     
+31    42840.0  (1052,...       1178         1178                  165          165            com.bl...          True          ...            False                 1304              1052                 250                80                 8     True       True       True         True            9c981ca       164200906             170        170               <NA>              True         True              <NA>       <NA>         13        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252             1304       1260              1052        1008                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   IMEI/P...     
+32    42840.0  (548, ...        674          674                  165          165            com.bl...          True          ...            False                  800               548                 250                80                 8     True       True       True         True            c93ff3b       211025723             170        170               <NA>              True         True              <NA>       <NA>         14        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V          252        252              800        756               548         504                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   as Ga ...     
+33    42840.0  (1304,...       1430         1430                  165          165            com.bl...          True          ...            False                 1556              1304                 250                80                 8     True       True       True         True            569d658        90822232             170        170               <NA>              True         True              <NA>       <NA>         15        False              False               False            False            False                False                      False               False              <NA>  [[[38,...         False                    False              POLYGO...       True                V          252        252             1556       1512              1304        1260                250        170                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   SocksD...     
+34   140128.0  (196, ...        800          800                  842          842            androi...         False          ...            False                 1404               196                 900               784                 8     True       True      False         True            d395417       221860887             116        116          app:id...              True        False          7f08017f  213123...         23        False              False               False            False            False                False                      False               False         id/vie...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               784          90                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>                 
+35   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 8    False       True      False         True            9d20004       164757508             206        206               <NA>              True        False              <NA>       <NA>         24        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        206               694           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              22          20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
+36  1352976.0  (6, 42...        800          800                  468          468            androi...         False          ...            False                 1594                 6                 894                42                 8    False       True      False         True            ebbfee7       247201511             852        852               <NA>              True        False              <NA>       <NA>         53        False               True               False            False             True                False                      False               False              <NA>  [[[39,...         False                    False              POLYGO...       True                V         1588       1588             1594       1594                 6           6                894        858                42           6                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              52          51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>   a | | ...     
+37   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 7     True       True      False         True             49b71b         4831003             510        510               <NA>              True        False              <NA>       <NA>          9        False              False               False            False            False                False                      False               False              <NA>  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1512                44           0                590        510                80           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
+38      225.0  (726, ...        733          733                  620          620            androi...         False          ...            False                  741               726                 628               613                 7     True       True      False         True            1b8c9ce        28887502              15         15          app:id...              True        False          7f0800ef  213123...         18        False               True               False            False             True                False                      False               False         id/loa...  [[[35,...         False                    False              POLYGO...       True                V           15         15              741         25               726          10                628         22               613           7                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
+39     2604.0  (751, ...        813          813                  620          620            androi...         False          ...            False                  875               751                 631               610                 7     True       True      False         True            c7ee0ef       209641711              21         21          app:id...              True        False          7f0800dc  213123...         19        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                V          124        124              875        159               751          35                631         25               610           4                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              17           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>                 
+40    21744.0  (196, ...        800          800                  685          685            androi...         False          ...            False                 1404               196                 694               676                 7     True       True      False         True            d6f43b1       225395633              18         18          app:id...              True        False          7f08011b  213123...         21        False              False               False            False            False                False                      False               False         id/pop...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                694         27               676           9                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   JOGOS ...     
+41   248848.0  (196, ...        800          800                  797          797            androi...         False          ...            False                 1404               196                 900               694                 7    False       True      False         True            ae5f096       182841494             206        206          app:id...              True        False          7f0800bd  213123...         22        False              False               False            False            False                False                      False               False         id/fra...  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1208               196           0                900        233               694          27                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              20           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   Â¥ 4 e...     
+42  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 7    False       True      False         True            69044a6       110118054             864        864               <NA>              True        False              <NA>       <NA>         52        False               True               False            False             True                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()              51           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+43  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 6    False       True      False         True            46dee93        74313363             864        864          app:id...              True        False          7f08006c  213123...          7        False              False               False            False             True                False                      False               False         id/bac...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+44   771120.0  (44, 8...        800          800                  335          335            com.bl...         False          ...            False                 1556                44                 590                80                 6     True       True       True         True            6affac3       112196291             510        510          app:id...              True        False          7f08009e  213123...          8        False              False               False            False            False                False                      False               False         id/des...  [[[35,...         False                    False              POLYGO...       True                V         1512       1512             1556       1556                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   as Â¥ ...     
+45    25600.0  (0, 59...        800          800                  598          598            com.bl...         False          ...            False                 1600                 0                 606               590                 6     True       True      False         True            a318ed0       171019984              16         16          app:id...              True        False          7f08009f  213123...         16        False               True               False            False             True                False                      False               False         id/des...  [[[28,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                606        570               590         554                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+46     5070.0  (716, ...        800          800                  621          621            androi...         False          ...            False                  885               716                 636               606                 6    False       True      False         True            57d5ec9        92102345              30         30          app:id...              True        False          7f0800db  213123...         17        False               True               False            False             True                False                      False               False         id/ins...  [[[35,...         False                    False              POLYGO...       True                I          169        169              885        885               716         716                636        600               606         570                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+47   281464.0  (196, ...        800          800                  783          783            androi...         False          ...            False                 1404               196                 900               667                 6    False       True      False         True            d275f40       220684096             233        233          app:id...              True        False          7f0800a7  213123...         20        False              False               False            False            False                False                      False               False           id/dock  [[[35,...         False                    False              POLYGO...       True                V         1208       1208             1404       1404               196         196                900        864               667         631                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Street...     
+48  1382400.0  (0, 36...        800          800                  468          468            com.bl...          True          ...            False                 1600                 0                 900                36                 6    False       True       True         True            25d1e01        39656961             864        864          app:id...              True        False          7f0800c4  213123...         51        False               True               False            False             True                False                      False               False         id/gro...  [[[32,...         False                    False              POLYGO...       True                I         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+49    19380.0  (44, 8...         63           63                  335          335            androi...         False          ...            False                   82                44                 590                80                 6     True       True      False         True            4493e79        71908985             510        510          app:id...              True        False          7f0800e5  213123...         56        False              False               False            False            False                False                      False               False         id/lef...  [[[35,...         False                    False              POLYGO...       True                V           38         38               82         82                44          44                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+50    19380.0  (1518,...       1537         1537                  335          335            androi...         False          ...            False                 1556              1518                 590                80                 6     True       True      False         True            ecea7be       248424382             510        510          app:id...              True        False          7f08012e  213123...         57        False              False               False            False            False                False                      False               False         id/rig...  [[[37,...         False                    False              POLYGO...       True                V           38         38             1556       1556              1518        1518                590        554                80          44                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+51  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 5    False       True      False         True            294a77d        43296637             864        864               <NA>              True        False              <NA>       <NA>          6        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+52  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 5     True       True      False         True            c019672       201430642             864        864               <NA>              True        False              <NA>       <NA>         58        False              False               False            False            False                False                      False               False              <NA>  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               5           4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+53  1382400.0  (0, 36...        800          800                  468          468            com.bl...         False          ...            False                 1600                 0                 900                36                 4     True       True      False         True            38d79ff        59603455             864        864          app:id...              True        False          7f0800df  213123...          5        False              False               False            False            False                False                      False               False         id/ite...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        864                36           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               4           3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+54  1382400.0  (0, 36...        800          800                  468          468            androi...         False          ...            False                 1600                 0                 900                36                 3    False       True       True         True            d8cdd1e       227335454             864        864          app:id...              True        False          7f0800b1  213123...          4        False              False                True            False            False                False                      False               False         id/dra...  [[[32,...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                36          36                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               3           2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   m6: Â«...     
+55  1440000.0  (0, 0,...        800          800                  450          450            androi...         False        an...            False                 1600                 0                 900                 0                 2    False       True      False         True            2b36d59        45313369             900        900               <NA>              True        False              <NA>       <NA>          3        False              False               False            False            False                False                      False               False              <NA>  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               2           0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
+56        0.0  (0, 0,...          0            0                    0            0            androi...         False      andr...            False                    0                 0                   0                 0                 1    False       True      False        False            812b782       135444354               0          0          androi...              True        False           102018a   16908682          1        False              False               False            False             True                False                      False               False         id/act...        NaN         False                    False              POLYGO...      False                G            0          0                0          0                 0           0                  0          0                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()            <NA>                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>                 
+57  1440000.0  (0, 0,...        800          800                  450          450            androi...         False      andr...            False                 1600                 0                 900                 0                 1    False       True      False         True            5f37da0        99843488             900        900          androi...              True        False           1020002   16908290          2        False              False               False            False            False                False                      False               False         id/con...  [[[144...         False                    False              POLYGO...       True                V         1600       1600             1600       1600                 0           0                900        900                 0           0                  ()              ()                 ()                     ()                        ()          ()             ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                          ()            ()               0        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>        <NA>   Size: ...     
+
+```
+
+**01/03/2023: Added adbdevicechanger** 
+```python
+# https://github.com/hansalemaos/adbdevicechanger
+# tested with bluestacks - root access
+self.aa_activate_adbdevicechanger()
+self.bb_adbdevicechanger.change_android_id()
+
+b'Row: 0 _id=227, name=device_name, value=OnePlus 5T\r\n'
+Out[7]: ('f7a32086dc724a4a', 'OnePlus 5T')
+
+
+self.bb_adbdevicechanger.change_device_name(
+    modelregex=".*",
+    developerregex=".*",
+    androidfullnameregex=".*",
+    year=">1",
+    month=">0",
+    versionnumberaround=7.05,
+)
+b'Row: 0 _id=2340, name=android_id, value=f7a32086dc724a4a\r\n'
+b'Row: 0 _id=228, name=device_name, value=HTC U11\r\n'
+Out[8]: ('f7a32086dc724a4a', 'HTC U11')
+
+self.bb_adbdevicechanger.change_android_id_and_device_name(
+    modelregex=".*",
+    developerregex=".*",
+    androidfullnameregex=".*",
+    year=">1",
+    month=">0",
+    versionnumberaround=7.05,
+)
+b'Row: 0 _id=2341, name=android_id, value=fb9afc93197942d8\r\n'
+b'Row: 0 _id=229, name=device_name, value=Nokia 8\r\n'
+Out[9]: ('fb9afc93197942d8', 'Nokia 8')
+
+
+self.bb_adbdevicechanger.get_random_android_cellphones(    modelregex="Samsung.*",
+    developerregex=".*",
+    androidfullnameregex=".*",
+    year=">2010",
+    month=">0",
+    versionnumberaround=9.05,
+    howmany=10,
+    return_list=False,)
+Out[13]: 
+                       aa_model  ...              uuid
+0  Samsung Galaxy Note 20/Ultra  ...  36f8a604180b4d7f
+1            Samsung Galaxy A70  ...  cb7f374cd85d4330
+2      Samsung Galaxy A30s/A50s  ...  9380749deb5942f6
+3      Samsung Galaxy Note 10/+  ...  c36816b1906542dc
+4    Samsung Galaxy S20/+/Ultra  ...  33dc12217b404a62
+5         Samsung Galaxy A90 5G  ...  cf0084fa8261465d
+6      Samsung Galaxy A51 5G UW  ...  3177aa09b1fc40d9
+7            Samsung Galaxy A01  ...  44db6d59366143cd
+8         Samsung Galaxy A42 5G  ...  a5b6fb2d08ac4475
+9           Samsung Galaxy A20e  ...  806b4ae287ec4d34
+[10 rows x 10 columns]
+
+```
+
+
+**23/02/2023: New methods**
+```python
+from adbkit import ADBTools
+adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
+deviceserial = "localhost:5555"
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+self.aa_connect_to_device()
+self.aa_activate_tesseract(
+    tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
+)
+
+#####################################################################################
+# This method uses Tesseract! You can download it here: https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
+self.aa_update_screenshot() # Update the screenshot before 
+df=self.aa_ocr_elements_from_activities(['Play Store'], # pass all strings as a list 
+minpercentage=85, # fuzzy match
+maxtolerance=10,
+screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+
+    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
+32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
+
+
+
+#####################################################################################
+# Another example (Play Store written wrong)
+
+df2=self.aa_ocr_elements_from_uiautomator(['blai Store'],minpercentage=70, maxtolerance=10, )
+
+    aa_area       aa_bounds  aa_center_x  aa_center_x_cropped  aa_center_y  aa_center_y_cropped   aa_class_name aa_clickable aa_complete_dump aa_context_clickable  aa_cropped_x_end  aa_cropped_x_start  aa_cropped_y_end  aa_cropped_y_start aa_depth aa_drawn aa_enabled aa_focusable  aa_has_screenshot aa_hashcode_hex aa_hashcode_int  aa_height  aa_height_cropped aa_id_information  aa_is_child aa_long_clickable aa_mID_hex aa_mID_int aa_old_index aa_pflag_activated aa_pflag_dirty_mask aa_pflag_focused aa_pflag_hovered aa_pflag_invalidated aa_pflag_is_root_namespace aa_pflag_prepressed aa_pflag_selected aa_pure_id   aa_screenshot aa_scrollbars_horizontal aa_scrollbars_vertical      aa_shapely  aa_valid_square aa_visibility  aa_width  aa_width_cropped  aa_x_end aa_x_end_relative  aa_x_start aa_x_start_relative  aa_y_end aa_y_end_relative  aa_y_start aa_y_start_relative ee_aa_longtouch ee_aa_longtouch_bs ee_aa_longtouch_offset ee_aa_longtouch_offset_bs ee_aa_touch ee_aa_touch_bs ee_aa_touch_offset ee_aa_touch_offset_bs ff_aa_downswipe ff_aa_save_screenshot ff_aa_show_screenshot ff_aa_tap_center_offset ff_aa_tap_center_offset_long ff_aa_tap_center_variation ff_aa_tap_center_variation_long ff_aa_tap_exact_center ff_aa_tap_exact_center_long ff_aa_upswipe ff_show_parents  parent_000  parent_001  parent_002  parent_003  parent_004  parent_005  parent_006  parent_007  parent_008  parent_009  parent_010  parent_011 aa_scanned_text  aa_tesseract aa_closest_word  aa_resultdiff
+32  30192.0  (26, 26, 23...          128             128               100             100       com.bluesta...         True             ...            False                  230                26                 174                26            8     True       True        False            True            7529967       122853735        148             148               <NA>           True            True         <NA>       <NA>           14           False              False               False            False            False                False                      False               False         <NA>  [[[41, 12, ...           False                    False         POLYGON ((2...            True              V       204             204         230             204            26               0           174             148            26               0                  ()              ()                 ()                     ()                    ()             ()              ()                 ()                    ()              ()                    ()                    ()                      ()                           ()                         ()                              ()                     ()                        ()              ()           9           8           6           5           4           3           2           0        <NA>        <NA>        <NA>        <NA>      Play Store         100.0      Play Store            0.0
+
+#####################################################################################
+# Pass a list of tuples:
+((x,y),time in seconds)
+
+self.aa_multi_input_tap_with_delay([((100,100),2), ((200,200),3)])
+#####################################################################################
+
+self.aa_input_tap(x=100,y=100)
+
+#####################################################################################
+# https://github.com/hansalemaos/adbescapes
+# Converts Unicode string to ASCII and escapes all characters that need to be escaped. 
+# You have to activate it, before using it. The first start takes some time because numba needs to compile the code 
+self.aa_activate_input_text_formated()
+
+# input 
+text="""
+"'ąćęłń'\tóśźż\nĄĆĘŁŃÓŚŹŻ\n\"Junto à Estação de \nCarcavelos;\"" "äöüÄÖÜß"
+"""
+self.aa_input_text_formated_with_delay(text,delay=(0.01, 0.2),respect_german_letters=False, exit_keys="ctrl+x")
+
+
+# output
+"'aceln'    oszz
+ACELNOSZZ
+"Junto a Estacao de 
+Carcavelos;"" "aouAOUb"
+
+# If you want it the German way :)
+self.aa_input_text_formated(text,respect_german_letters=True, exit_keys="ctrl+x")
+
+"'aceln'    oszz
+ACELNOSZZ
+"Junto a Estacao de 
+Carcavelos;"" "aeoeueAeOeUess"
+#####################################################################################
+self.aa_install_apk_from_hdd(r"C:\Users\Gamer\anaconda3\envs\instcont\instagram.apk")
+#####################################################################################
+self.aa_uninstall_package('com.instagram.lite')
+#####################################################################################
+# First argument is a regex 
+self.aa_copy_apk_to_hdd('com.insta.*', 'c:\\instaapkdownload')
+#####################################################################################
+```
+
+
+
+**17/01/2023: Screenshot fix**
+
+
+```python
+$pip install adbkit
+from adbkit import ADBTools
+adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe"
+deviceserial = "localhost:5875"
+
+# Create an instance
+# Don't get confused about the instance name "self". I did it because it is faster copying methods from the class 
+self = ADBTools(adb_path, deviceserial, sdcard="/sdcard/")
+self = ADBTools(adb_path=adb_path, deviceserial=deviceserial)
+
+# connect to the device 
+self.aa_connect_to_device()
+```
+
+
+
+```python
+# If you are using BlueStacks and want to have root access, call:
+self.aa_root_bluestacks_instances() 
+# This method will basically do this steps: https://appuals.com/root-bluestacks/ to root BlueStacks
+# You can run the script every time you use this module. It won't hurt. 
+# The first time, you might have to restart BlueStacks to enable the root access 
+```
+
+
+
+```python
+# If your device/BlueStacks is rooted, enable root so that all commands will be sent as root 
+self.aa_enable_root() 
+# can be disabled by calling :
+self.aa_disable_root()
+```
+
+
+
+```python
+# Activates self.bb_adbkeyboard 
+# Read more about it: https://github.com/hansalemaos/adb_unicode_keyboard
+self.aa_activate_adb_keyboard(exit_keys="ctrl+x") 
+```
+
+
+
+```python
+# Activates self.bb_sendevent_keyboard (needs root access)
+# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
+
+self.aa_activate_sendevent_keyboard(
+    sdcard="/storage/emulated/0/",
+    tmp_folder_on_sd_card="AUTOMAT",
+    exit_keys="ctrl+x",
+)  # needs root access
+
+# Here is one example: 
+self.bb_adbkeyboard.press_7_keycode_0()
+```
+
+
+
+```python
+# Activates self.self.bb_getevent_sendevent
+# Read more about it: https://github.com/hansalemaos/sendevent_getevent_keyboard
+
+self.aa_activate_getevent_sendevent(
+    sdcard="/storage/emulated/0/",
+    tmp_folder_on_sd_card="AUTOMAT",
+    bluestacks_divider=32767,
+    exit_keys="ctrl+x",
+)  # needs root access
+```
+
+
+
+```python
+# Activates self.bb_sendevent_touch
+# Read more about it: https://github.com/hansalemaos/sendevent_touch
+
+self.aa_activate_sendevent_touch(
+    sdcard="/storage/emulated/0/",
+    tmp_folder_on_sd_card="AUTOMAT",
+    bluestacks_divider=32767,
+    use_bluestacks_coordinates=True,
+)  # needs root access
+
+# Here is one example:
+self.bb_sendevent_touch.touch(10,10)
+```
+
+
+
+```python
+# Activates https://github.com/hansalemaos/a_pandas_ex_tesseract_multirow_regex_fuzz
+# You can download the 64 bit version of tesseract here: 
+# https://digi.bib.uni-mannheim.de/tesseract/tesseract-ocr-w64-setup-5.3.0.20221222.exe
+
+self.aa_activate_tesseract(
+        tesseractpath=r"C:\Program Files\Tesseract-OCR\tesseract.exe"
+    )
+
+# Once activated, you can call:
+# self.aa_ocr_with_tesseract()
+
+    left  top  width  height       conf        text  middle_x  middle_y  end_x  end_y
+8    382   42    499      49  37.512093         RH,       631        66    881     91
+9    728   34     98      61  30.925949          2.       777        64    826     95
+13   370  101     37      11   84.72541     'system       388       106    407    112
+14   411  101     24      10  79.929901        Apps       423       106    435    111
+15   536   90     36      28  85.425911      Roblox       554       104    572    118
+16   676  100     55       9  88.744247  BlueStacks       703       104    731    109
+17   735  101      7       8  80.470955           X       738       105    742    109
+18   814  101     31      10  90.271423      Spiele       829       106    845    111
+19   848  101     18       8  93.303749         und       857       105    866    109
+20   869  103     41       9  87.963295     gewinne       889       107    910    112
+28    72  100     20      12  96.004517        Play        82       106     92    112
+29    95  101     27       8  86.986359       Store       108       105    122    109
+33   225  211     49      12  76.804665   Globoplay       249       217    274    223
+37   326  489     25      28  91.894142       Tibia       338       503    351    517
+38   401  500     50       8  91.477989   Guardians       426       504    451    508
+39   455  499     10       9  72.064316          of       460       503    465    508
+41   415  512     37       9  75.078018     Cloudia       433       516    452    521
+
+# and even perform a multiline fuzzy search:
+xxx = self.aa_ocr_with_tesseract(search_for='Kontakte verwalten')
+```
+```python
+# Use this method to update the screenshot 
+# The updated screenshot can be found here: self.screenshot
+self.aa_update_screenshot()
+
+```
+
+
+
+```python
+# get 5 screenshot within 5 seconds
+xx=self.aa_get_screenshots(
+        sleeptime=1,
+        number=5)
+
+```
+
+
+
+```python
+# Now you can use self.df to do operations on the screenshot 
+# More information about a_pandas_ex_image_tools:
+# https://github.com/hansalemaos/a_pandas_ex_image_tools
+self.aa_update_imagedf()
+```
+
+
+```python
+# If you want to capture the logcat output and analyze it in a DataFrame,
+use: 
+logcatcap = self.aa_capture_logcat(
+        exit_keys="ctrl+x",
+        timeout=None,
+    )  
+
+# When you exit using "ctrl+x", the method will return a DataFrame
+# By the way: almost all methods can be interrupted using a key command 
+```
+
+
+
+```python
+# Those 2 methods will help you to identify and interact with views:
+# Read more about it: https://github.com/hansalemaos/androdf
+df1 = self.aa_get_all_displayed_items_from_uiautomator(
+	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+
+df3 = self.aa_get_all_displayed_items_from_activities(
+	screenshotfolder="f:\\compare_android",  # screenshots will be saved here
+	max_variation_percent_x=10,  # used for one of the click functions, to not click exactly in the center - more information below
+	max_variation_percent_y=10,  # used for one of the click functions, to not click exactly in the center
+	loung_touch_delay=(
+		1000,
+		1500,
+	),  # with this settings longtouch will take somewhere between 1 and 1,5 seconds
+	swipe_variation_startx=10,  # swipe coordinate variations in percent
+	swipe_variation_endx=10,
+	swipe_variation_starty=10,
+	swipe_variation_endy=10,
+	sdcard="/storage/emulated/0/",  # sdcard will be used if you use the sendevent methods, don't pass a symlink - more information below
+	tmp_folder_on_sd_card="AUTOMAT",  # this folder will be created in the sdcard folder for using sendevent actions
+	bluestacks_divider=32767,  # coordinates must be recalculated for BlueStacks https://stackoverflow.com/a/73733261/15096247 when using sendevent
+)
+```
+
+
+
+```python
+# Uses: https://github.com/hansalemaos/a_pandas_ex_adb_to_df
+# lists all files in DataFrame and adds useful functions
+# self.aa_list_all_files_on_device()
+
+dffiles = self.aa_list_folder_content(folder_to_search="data/")  
+print(dffiles)
+                  aa_date  ... ff_pull_file_cat
+0     2022-12-11 06:48:00  ...               ()
+1     2022-12-26 22:16:00  ...               ()
+2     2022-12-06 19:10:00  ...               ()
+3     2022-12-06 13:38:00  ...               ()
+4     2022-12-26 22:16:00  ...               ()
+                   ...  ...              ...
+26120 2021-09-16 04:21:00  ...               ()
+26121 2021-09-16 03:53:00  ...               ()
+26122 2021-09-16 03:53:00  ...               ()
+26123 2021-09-16 04:35:00  ...               ()
+26124 2021-09-16 04:31:00  ...               ()
+[26125 rows x 16 columns]
+```
+
+
+
+```python
+# Search with grep 
+# Uses https://github.com/hansalemaos/adb_grep_search
+dfgrep = self.aa_grep_search(
+        folder_to_search="data/data",
+        filetype="*.db",
+        regular_expression=r"CREATE.TABLE",
+        exit_keys="ctrl+x",
+        timeout=None,
+        remove_control_characters=True,
+    )
+
+dfgrep
+Out[19]: 
+                                               aa_file  ...      aa_regex
+0    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+1    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+2    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+3    data/data/com.android.providers.media/database...  ...  CREATE.TABLE
+4    data/data/com.globo.globotv/databases/mcsdk_bf...  ...  CREATE.TABLE
+..                                                 ...  ...           ...
+103  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+104  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+105  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+106  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+107  data/data/com.roblox.client/databases/google_a...  ...  CREATE.TABLE
+[108 rows x 5 columns]
+```
+
+
+
+```python
+# Uses https://github.com/hansalemaos/a_pandas_ex_adb_settings_to_df
+self.aa_parse_settings_from_all_packages(
+        tempfolder="f:\\tmpfolder", datafolder="data/"
+    )
+
+        index          aa_all_keys  ... level_22 level_23
+0         0.0         (long, name)  ...      NaN      NaN
+1         1.0        (long, value)  ...      NaN      NaN
+2         0.0   (boolean, 0, name)  ...      NaN      NaN
+3         1.0  (boolean, 0, value)  ...      NaN      NaN
+4         2.0   (boolean, 1, name)  ...      NaN      NaN
+       ...                  ...  ...      ...      ...
+110795    NaN            (6, desc)  ...      NaN      NaN
+110796    NaN           (6, label)  ...      NaN      NaN
+110797    NaN             (6, pkg)  ...      NaN      NaN
+110798    NaN          (6, source)  ...      NaN      NaN
+110799    NaN             (6, url)  ...      NaN      NaN
+[110800 rows x 31 columns]
+
+You might see this error messages several times:
+
+"Go to: https://www.sqlite.org/download.html ,
+download the dll and put it in the DLLs folder of your env!"
+
+You can ignore it.
+```
+
+
+
+```python
+#This method helps you find all executable activities from a package 
+# More about it: https://github.com/hansalemaos/a_pandas_ex_adb_execute_activities
+
+self.aa_get_activity_execution_df_from_one_package(
+        packagename="com.roblox.client"
+    ) 
+```
+
+
+
+```python
+# adds new contact, can be saved straight away
+addcon = self.aa_add_new_contact(
+	"hans", "+55119897827552", "hans@something.com", "my address", save=False
+)
+```
+
+
+
+```python
+# If you play Roblox, you can enable/disable some textures to get higher fps
+self.aa_enable_roblox_textures(
+	exit_keys="ctrl+x",
+	print_output=True,
+	timeout=None,
+)
+
+self.aa_disable_roblox_textures(
+	exit_keys="ctrl+x",
+	print_output=True,
+	timeout=None,
+)
+```
+
+
+
+```python
+# goes to the home screen, doesn't close anything
+self.aa_go_to_home_screen()
+```
+
+
+
+```python
+# repeat=5 usually deletes more than 5 characters!!
+self.aa_press_delete_key_repeated_times(repeat=5)
+```
+
+
+
+```python
+# starts the android file manager, pass the file type you want to see
+self.aa_get_content(type_="text/plain")
+```
+
+
+
+```python
+# Here are some methods to get useful information. 
+# Returns DataFrames 
+print(self.aa_whole_dumpsys_to_df())
+print(self.aa_list_all_packages())
+print(self.aa_list_broadcast_stats())
+print(self.aa_list_pending_intents())
+print(self.aa_list_all_activities_from_device())
+print(self.aa_list_all_services())
+print(self.aa_list_all_receivers())
+print(self.aa_list_all_activities())
+print(self.aa_get_procstats())
+print(self.aa_list_all_devices()) # devices on the device (dev ...)
+print(self.aa_list_devices()) # all adb devices (localhost:5555 ...)
+print(self.aa_list_pids_basic())
+print(self.aa_list_pids_complete())
+print(self.aa_list_memory())
+print(self.aa_getprop())
+print(self.aa_list_all_broadcasts())
+print(self.aa_list_all_broadcasts_history())
+print(self.aa_list_users())
+print(self.aa_list_permission_groups())
+print(self.aa_list_disabled_packages())
+print(self.aa_list_apps_in_use())
+print(self.aa_list_3rd_party_packages())
+print(self.aa_list_features())
+```
+
+
+
+```python
+# Smile! :)
+self.aa_open_camera_photo_mode()
+```
+
+
+
+```python
+# works with and without http://
+print(self.aa_open_website("google.com"))
+```
+
+
+
+```python
+# switches to gallery
+self.aa_start_gallery()
+```
+
+
+
+```python
+# cheeeese
+self.aa_take_a_picture()
+```
+
+
+
+```python
+# useful for some apps 
+self.aa_adb_turn_screen_compatibility_off()
+self.aa_adb_turn_screen_compatibility_on()
+```
+
+
+
+```python
+# Be careful! 
+self.aa_remove_file('/sdcard/9.png')
+```
+
+
+
+```python
+# Essential when you use your cell phone (with Whatsapp, Facebook ...) to automize things.
+self.aa_enable_notifications()
+self.aa_disable_notifications()
+```
+
+
+
+```python
+# More useful stuff for notifications
+self.aa_expand_settings() 
+self.aa_expand_notifications()
+```
+
+
+
+```python
+# Changes the screen orientation
+# You can pass:
+# horizontal_upside_down or 2
+# vertical or 1
+# horizontal or 0
+# vertical_upside_down or 3
+self.aa_change_screen_orientation("horizontal")
+```
+
+
+
+```python
+self.aa_get_display_orientation()
+#Out[4]: 0 
+# 0 means horizontal
+```
+
+
+
+```python
+# Sometimes you upload new media files, but you can't see the thumbnails immediately
+# This method updates all thumbnails
+self.aa_rescan_media()
+```
+
+
+
+```python
+# If you are in the middle of a text and want to go to the end of the line
+self.aa_move_to_end_of_line()
+```
+
+
+
+```python
+# Useful keyboard stuff 
+self.aa_hide_keyboard()
+self.aa_is_keyboard_shown()
+```
+
+
+
+```python
+# Doesn't work on BlueStacks, but on my pixel 6 there are no problems
+# (Actually it is not necessary when using BlueStacks hahaha)
+self.aa_is_screen_unlocked()
+```
+
+
+
+```python
+# Don't use this command on BlueStacks, you will have to reboot the device
+self.aa_lock_screen()
+```
+
+
+
+```python
+# Useful commands 
+self.aa_press_home() #back to home screen
+self.aa_press_app_switch()
+```
+
+
+
+```python
+# Configured for my Pixel 6, but should work on any device with a 
+# newer android version. 
+self.aa_swipe_up_to_unlock_screen('3333')
+```
+
+
+
+```python
+# doesn't work with BlueStacks, because of the app switch design, 
+# but it does on my pixel and should work with any device that 
+# has a recent Android version
+self.aa_close_all_apps_with_swipe()
+```
+
+
+
+```python
+# uninstalls a package
+self.aa_uninstall_package('com.google.android.youtube')
+```
+
+
+
+```python
+# Returns the activity needed to open the package 
+self.aa_resolve_activity('com.roblox.client')
+b'priority=0 preferredOrder=0 match=0x108000 specificIndex=-1 isDefault=true\r\n'
+b'com.roblox.client/.startup.ActivitySplash\r\n'
+```
+
+
+
+```python
+# But you can also open any package using:
+self.aa_open_app('com.roblox.client')
+```
+
+
+
+```python
+# This method makes swiping easy
+# x (start), y (start), x (end) y (end), last number in seconds
+self.aa_swipe(500, 400, 500, 100, 1.1) 
+```
+
+
+
+```python
+#opens a separate shell window using cmd.exe 
+self.aa_open_shell() 
+```
+
+
+
+```python
+# It changes the dictionary that you are in
+# and executes a command 
+self.aa_change_cwd_and_execute_adb_shell('ls', 'data/')
+b'5.3.10.1001\r\n'
+b'5.9.300.1014\r\n'
+b'adb\r\n'
+b'anr\r\n'
+b'app\r\n'
+b'app-asec\r\n'
+b'app-ephemeral\r\n'
+b'app-lib\r\n'
+b'app-private\r\n'
+b'arm\r\n'
+....
+```
+
+
+
+```python
+# This can also be accomplished by sending multiple commands: 
+self.aa_execute_multiple_adb_shell_commands(['cd data/', 'ls|grep system'])
+Out[28]: [b'system\r\n', b'system_ce\r\n', b'system_de\r\n']
+```
+
+
+
+```python
+# You can also send non-shell commands: 
+self.aa_execute_non_shell_adb_command('devices')
+```
+
+
+
+```python
+# This method pushes a file to your sdcard:
+self.aa_push_to_sdcard(r'F:\donedone.png')
+```
+
+
+
+```python
+# This method pulls a file to your hdd
+self.aa_pull('/sdcard/donedone.png', 'f:\\dfdffasd')
+```
+
+
+
+```python
+# A fast way of scanning all connected devices:
+# start/end means the ports you want to start/end with
+# After 10 seconds, all processes that have not completed the search
+# will be killed 
+self.aa_connect_do_all_devices(start=4999, end=6000, timeout=10)
+    '''self.aa_list_devices()
+b'List of devices attached\r\n'
+b'localhost:5037\toffline\r\n'
+b'localhost:5040\toffline\r\n'
+b'localhost:5357\toffline\r\n'
+b'localhost:5725\tdevice\r\n'
+b'localhost:5800\toffline\r\n'
+b'localhost:5875\tdevice\r\n'
+b'localhost:5900\toffline\r\n'
+b'localhost:5955\tdevice\r\n'
+b'\r\n'''
+
+    '''
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process
+Killing the process'''
+```
+
+
+
+```python
+# Uses https://github.com/hansalemaos/a_cv2_shape_finder 
+# to detect shapes in the screenshot 
+self.get_shapes_from_screenshot_THRESH_OTSU()
+self.get_shapes_from_screenshot_ADAPTIVE_THRESH_MEAN_C()
+self.get_shapes_from_screenshot_ADAPTIVE_THRESH_GAUSSIAN_C()
+```
+
+
+
+```python
+#Some self-explaining stuff  
+
+self.aa_isfolder('/sdcard/donedone.png')
+False
+self.aa_isfolder('/sdcard/')
+True
+next(self.aa_get_screenshots())
+
+self.aa_path_exists('/sdcard/')
+True
+self.aa_path_exists('/sdcard2/')
+False
+
+self.aa_get_screen_resolution()
+(960, 540)
+
+self.aa_restart_server()
+self.aa_reboot_and_listen_to_usb()
+self.aa_start_server()
+self.aa_stop_server()
+self.aa_kill_server()
+self.aa_force_stop('com.roblox.client') #root
+self.aa_show_screenshot_in_browser()
+```
+
```

### Comparing `adbkit-0.17/setup.py` & `adbkit-0.18/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
 import codecs
 import os
-
-#change to dict
+# 
 here = os.path.abspath(os.path.dirname(__file__))
+# 
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()\
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
+from pathlib import Path
+this_directory = Path(__file__).parent
+#long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.17'
-DESCRIPTION = "Big automation package for ADB"
+VERSION = '''0.18'''
+DESCRIPTION = '''Big automation package for ADB'''
 
 # Setting up
 setup(
     name="adbkit",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/adbkit',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    #packages=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_unicode_keyboard', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'tesseractmultiprocessing', 'touchtouch'],
+long_description = long_description,
+long_description_content_type="text/markdown",
+    #packages=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_unicode_keyboard', 'adbblitz', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'cv2imshow', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'taskkill', 'tesseractmultiprocessing', 'touchtouch'],
     keywords=['adb', 'android', 'automation', 'shell', 'root'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.9', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Text Editors :: Text Processing', 'Topic :: Text Processing :: General', 'Topic :: Text Processing :: Indexing', 'Topic :: Text Processing :: Filters', 'Topic :: Utilities'],
-    install_requires=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_unicode_keyboard', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'tesseractmultiprocessing', 'touchtouch'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    install_requires=['a_cv2_imshow_thread', 'a_cv2_shape_finder', 'a_cv_imwrite_imread_plus', 'a_pandas_ex_adb_execute_activities', 'a_pandas_ex_adb_settings_to_df', 'a_pandas_ex_adb_to_df', 'a_pandas_ex_apply_ignore_exceptions', 'a_pandas_ex_csv_plus', 'a_pandas_ex_image_tools', 'a_pandas_ex_logcat2df', 'a_pandas_ex_tesseract_multirow_regex_fuzz', 'adb_grep_search', 'adb_unicode_keyboard', 'adbblitz', 'adbdevicechanger', 'adbescapes', 'androdf', 'bstconnect', 'check_if_nan', 'cv2imshow', 'flatten_everything', 'getevent_sendevent', 'kthread', 'numpy', 'opencv_python', 'pandas', 'Pillow', 'Pillow', 'psutil', 'pyperclip', 'rapidfuzz', 'regex', 'sendevent_getevent_keyboard', 'sendevent_touch', 'subprocess_print_and_capture', 'taskkill', 'tesseractmultiprocessing', 'touchtouch'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

