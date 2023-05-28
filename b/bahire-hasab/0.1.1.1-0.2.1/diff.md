# Comparing `tmp/bahire-hasab-0.1.1.1.tar.gz` & `tmp/bahire-hasab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.1.1.1.tar", last modified: Sat May 27 08:38:02 2023, max compression
+gzip compressed data, was "bahire-hasab-0.2.1.tar", last modified: Sun May 28 10:35:05 2023, max compression
```

## Comparing `bahire-hasab-0.1.1.1.tar` & `bahire-hasab-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/src/bahire_hasab/
--rw-r--r--   0 runner    (1001) docker     (123)    10946 2023-05-27 08:37:47.000000 bahire-hasab-0.1.1.1/src/bahire_hasab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:38:02.452838 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-27 08:38:02.000000 bahire-hasab-0.1.1.1/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/src/bahire-hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-28 10:34:52.000000 bahire-hasab-0.2.1/src/bahire-hasab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:35:05.974882 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 10:35:05.000000 bahire-hasab-0.2.1/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.1.1.1/LICENSE` & `bahire-hasab-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.1.1.1/PKG-INFO` & `bahire-hasab-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.1.1.1
+Version: 0.2.1
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">📆 Bahire Hassab(ባህረ ሐሳብ) 🇪🇹 📦 </h1>
+
+ [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-hasab/actions/workflows/python-publish.yml)
+ 
  
 - A python module for calculating Ethiopian Holidays and Lents
 ## Table Of Content
+- [Table Of Content](#table-of-content)
 - [Description](#description)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Todo](#todo)
 ## Description
 - This is a python Installation module for Ethiopian Calender method for determining the dates of lents and holidays or in Amharic Bahire Hassab ባህረ ሐሳብ
 - I have used the native calculation method If you want the book I used you can find it [](#)
@@ -30,22 +34,34 @@
 - There is a snippet how to use it for your personal projects
 ```python
 from bahire_hasab import BahireHasab
 from detetime import detetime
 # The year according to the Ethiopian Calender
 year = datetime.now().year -8
 bh = BahireHasab(year)
-eth_easter = bh.tnsea
-print(eth_easter)
+eth_easter = bh.tnsae
+print(eth_easter)# ሚያዚያ 8 this is for the Ethiopian year 2015
 # This is should print the date of the Ethiopian Easter according to the Ethiopian Calendar
 ```
 - The method names are home how different from most methods that we know since I used most of them in Amharic there is their Equivalent in English
 
 |Method|English Equivalent|Description|
 |:-----|:-----------:  |     :----|
 |new_year|Ethiopian New Year|The day of new year in Amharic|
-|meskel|Ethiopian Feast of Cross|The Date of the feast of cross in Amharic|
+|abiy_tsome|Ethiopian Great Lent Begin|The day at which the great lent begin in Ethiopia|
+|neneweh|Ethiopian Fast of Neneviah|The Day of begining of the Neneviah fast|
+|debre_zeyt|Ethiopian Great lent middle|The middle day of the Ethiopian Great lent|
+|hosaena|Ethiopian Hoseana|The day of Entrance of Jesus to Jerusalem in Ethiopian Calender|
+|sklet|The holy Friday|The day of holyfriday in Ethiopian Calender.|
+|tnsae|Ethiopian Easter|The day of Easter in Ethiopian Calender.|
+|rkbe_kahnat| - | - |
+|erget|The day of ascension|Returns the day of ascension of the year.|
+|beale_hamsa|The Pentecost|Returens the day of Pentecost of the year.|
+|tsome_hawaryat|-|-|
+|tsome_dhnet|-|-|
+
+
 ## Todo
 - [x] Releasing the package to pypi.org
 - [ ] Making API for it
 - [ ] Support for Gregorian Calender
-- [ ] Finding corner Canses  
+- [x] Finding corner Canses
```

#### html2text {}

```diff
@@ -1,27 +1,38 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.1.1.1 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.1 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
-- A python module for calculating Ethiopian Holidays and Lents ## Table Of
-Content - [Description](#description) - [Installation](#installation) -
+[![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
+workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
+hasab/actions/workflows/python-publish.yml) - A python module for calculating
+Ethiopian Holidays and Lents ## Table Of Content - [Table Of Content](#table-
+of-content) - [Description](#description) - [Installation](#installation) -
 [Documentation](#documentation) - [Todo](#todo) ## Description - This is a
 python Installation module for Ethiopian Calender method for determining the
 dates of lents and holidays or in Amharic Bahire Hassab á£áá¨ áá³á¥ - I
 have used the native calculation method If you want the book I used you can
 find it [](#) - Each of the names I used in the module is mostly the Amharic
 Equivalent of the holiday if you want all you can get it Click_Here!. ##
 Installation - Bahire Hassab is available now on [](#https://pypi.org/) - You
 can Install it through pip by ```pip pip install bahire-hassab ``` ##
 Documentation - There is a snippet how to use it for your personal projects
 ```python from bahire_hasab import BahireHasab from detetime import detetime #
 The year according to the Ethiopian Calender year = datetime.now().year -8 bh =
-BahireHasab(year) eth_easter = bh.tnsea print(eth_easter) # This is should
-print the date of the Ethiopian Easter according to the Ethiopian Calendar ```
-- The method names are home how different from most methods that we know since
-I used most of them in Amharic there is their Equivalent in English
-|Method|English Equivalent|Description| |:-----|:-----------: | :----
-| |new_year|Ethiopian New Year|The day of new year in Amharic|
-|meskel|Ethiopian Feast of Cross|The Date of the feast of cross in Amharic| ##
-Todo - [x] Releasing the package to pypi.org - [ ] Making API for it - [ ]
-Support for Gregorian Calender - [ ] Finding corner Canses
+BahireHasab(year) eth_easter = bh.tnsae print(eth_easter)# áá«áá« 8 this
+is for the Ethiopian year 2015 # This is should print the date of the Ethiopian
+Easter according to the Ethiopian Calendar ``` - The method names are home how
+different from most methods that we know since I used most of them in Amharic
+there is their Equivalent in English |Method|English Equivalent|Description| |:
+-----|:-----------: | :----| |new_year|Ethiopian New Year|The day of new year
+in Amharic| |abiy_tsome|Ethiopian Great Lent Begin|The day at which the great
+lent begin in Ethiopia| |neneweh|Ethiopian Fast of Neneviah|The Day of begining
+of the Neneviah fast| |debre_zeyt|Ethiopian Great lent middle|The middle day of
+the Ethiopian Great lent| |hosaena|Ethiopian Hoseana|The day of Entrance of
+Jesus to Jerusalem in Ethiopian Calender| |sklet|The holy Friday|The day of
+holyfriday in Ethiopian Calender.| |tnsae|Ethiopian Easter|The day of Easter in
+Ethiopian Calender.| |rkbe_kahnat| - | - | |erget|The day of ascension|Returns
+the day of ascension of the year.| |beale_hamsa|The Pentecost|Returens the day
+of Pentecost of the year.| |tsome_hawaryat|-|-| |tsome_dhnet|-|-| ## Todo - [x]
+Releasing the package to pypi.org - [ ] Making API for it - [ ] Support for
+Gregorian Calender - [x] Finding corner Canses
```

### Comparing `bahire-hasab-0.1.1.1/README.md` & `bahire-hasab-0.2.1/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,25 @@
+Metadata-Version: 2.1
+Name: bahire-hasab
+Version: 0.2.1
+Home-page: https://github.com/hunderaweke/bahire-hasab
+Author: Hundera Awoke
+Author-email: hunderaweke@gmail.com
+Keywords: bahire_hasab
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <h1 align="center">📆 Bahire Hassab(ባህረ ሐሳብ) 🇪🇹 📦 </h1>
+
+ [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-hasab/actions/workflows/python-publish.yml)
+ 
  
 - A python module for calculating Ethiopian Holidays and Lents
 ## Table Of Content
+- [Table Of Content](#table-of-content)
 - [Description](#description)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Todo](#todo)
 ## Description
 - This is a python Installation module for Ethiopian Calender method for determining the dates of lents and holidays or in Amharic Bahire Hassab ባህረ ሐሳብ
 - I have used the native calculation method If you want the book I used you can find it [](#)
@@ -20,22 +34,34 @@
 - There is a snippet how to use it for your personal projects
 ```python
 from bahire_hasab import BahireHasab
 from detetime import detetime
 # The year according to the Ethiopian Calender
 year = datetime.now().year -8
 bh = BahireHasab(year)
-eth_easter = bh.tnsea
-print(eth_easter)
+eth_easter = bh.tnsae
+print(eth_easter)# ሚያዚያ 8 this is for the Ethiopian year 2015
 # This is should print the date of the Ethiopian Easter according to the Ethiopian Calendar
 ```
 - The method names are home how different from most methods that we know since I used most of them in Amharic there is their Equivalent in English
 
 |Method|English Equivalent|Description|
 |:-----|:-----------:  |     :----|
 |new_year|Ethiopian New Year|The day of new year in Amharic|
-|meskel|Ethiopian Feast of Cross|The Date of the feast of cross in Amharic|
+|abiy_tsome|Ethiopian Great Lent Begin|The day at which the great lent begin in Ethiopia|
+|neneweh|Ethiopian Fast of Neneviah|The Day of begining of the Neneviah fast|
+|debre_zeyt|Ethiopian Great lent middle|The middle day of the Ethiopian Great lent|
+|hosaena|Ethiopian Hoseana|The day of Entrance of Jesus to Jerusalem in Ethiopian Calender|
+|sklet|The holy Friday|The day of holyfriday in Ethiopian Calender.|
+|tnsae|Ethiopian Easter|The day of Easter in Ethiopian Calender.|
+|rkbe_kahnat| - | - |
+|erget|The day of ascension|Returns the day of ascension of the year.|
+|beale_hamsa|The Pentecost|Returens the day of Pentecost of the year.|
+|tsome_hawaryat|-|-|
+|tsome_dhnet|-|-|
+
+
 ## Todo
 - [x] Releasing the package to pypi.org
 - [ ] Making API for it
 - [ ] Support for Gregorian Calender
-- [ ] Finding corner Canses  
+- [x] Finding corner Canses
```

#### html2text {}

```diff
@@ -1,23 +1,38 @@
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.1 Home-page: https://
+github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
+hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
+markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
-- A python module for calculating Ethiopian Holidays and Lents ## Table Of
-Content - [Description](#description) - [Installation](#installation) -
+[![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
+workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
+hasab/actions/workflows/python-publish.yml) - A python module for calculating
+Ethiopian Holidays and Lents ## Table Of Content - [Table Of Content](#table-
+of-content) - [Description](#description) - [Installation](#installation) -
 [Documentation](#documentation) - [Todo](#todo) ## Description - This is a
 python Installation module for Ethiopian Calender method for determining the
 dates of lents and holidays or in Amharic Bahire Hassab á£áá¨ áá³á¥ - I
 have used the native calculation method If you want the book I used you can
 find it [](#) - Each of the names I used in the module is mostly the Amharic
 Equivalent of the holiday if you want all you can get it Click_Here!. ##
 Installation - Bahire Hassab is available now on [](#https://pypi.org/) - You
 can Install it through pip by ```pip pip install bahire-hassab ``` ##
 Documentation - There is a snippet how to use it for your personal projects
 ```python from bahire_hasab import BahireHasab from detetime import detetime #
 The year according to the Ethiopian Calender year = datetime.now().year -8 bh =
-BahireHasab(year) eth_easter = bh.tnsea print(eth_easter) # This is should
-print the date of the Ethiopian Easter according to the Ethiopian Calendar ```
-- The method names are home how different from most methods that we know since
-I used most of them in Amharic there is their Equivalent in English
-|Method|English Equivalent|Description| |:-----|:-----------: | :----
-| |new_year|Ethiopian New Year|The day of new year in Amharic|
-|meskel|Ethiopian Feast of Cross|The Date of the feast of cross in Amharic| ##
-Todo - [x] Releasing the package to pypi.org - [ ] Making API for it - [ ]
-Support for Gregorian Calender - [ ] Finding corner Canses
+BahireHasab(year) eth_easter = bh.tnsae print(eth_easter)# áá«áá« 8 this
+is for the Ethiopian year 2015 # This is should print the date of the Ethiopian
+Easter according to the Ethiopian Calendar ``` - The method names are home how
+different from most methods that we know since I used most of them in Amharic
+there is their Equivalent in English |Method|English Equivalent|Description| |:
+-----|:-----------: | :----| |new_year|Ethiopian New Year|The day of new year
+in Amharic| |abiy_tsome|Ethiopian Great Lent Begin|The day at which the great
+lent begin in Ethiopia| |neneweh|Ethiopian Fast of Neneviah|The Day of begining
+of the Neneviah fast| |debre_zeyt|Ethiopian Great lent middle|The middle day of
+the Ethiopian Great lent| |hosaena|Ethiopian Hoseana|The day of Entrance of
+Jesus to Jerusalem in Ethiopian Calender| |sklet|The holy Friday|The day of
+holyfriday in Ethiopian Calender.| |tnsae|Ethiopian Easter|The day of Easter in
+Ethiopian Calender.| |rkbe_kahnat| - | - | |erget|The day of ascension|Returns
+the day of ascension of the year.| |beale_hamsa|The Pentecost|Returens the day
+of Pentecost of the year.| |tsome_hawaryat|-|-| |tsome_dhnet|-|-| ## Todo - [x]
+Releasing the package to pypi.org - [ ] Making API for it - [ ] Support for
+Gregorian Calender - [x] Finding corner Canses
```

