# Comparing `tmp/eArsivPortal-0.0.2.tar.gz` & `tmp/eArsivPortal-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-0.0.2.tar", last modified: Sun May 28 12:24:49 2023, max compression
+gzip compressed data, was "eArsivPortal-0.0.3.tar", last modified: Sun May 28 13:55:27 2023, max compression
```

## Comparing `eArsivPortal-0.0.2.tar` & `eArsivPortal-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.017140 eArsivPortal-0.0.2/eArsivPortal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/setup.py
```

### Comparing `eArsivPortal-0.0.2/LICENSE` & `eArsivPortal-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.2/PKG-INFO` & `eArsivPortal-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.2
+Version: 0.0.3
 Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,18 @@
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eArsivPortal)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/eArsivPortal?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
-> Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) paketinin Python dili ile yazılmış versiyonudur.
+
+> Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) `(js)` paketinin `Python` dili ile yazılmış versiyonudur.
+
+> Gelişim aşamasında [Mert Levent](https://github.com/mlevent)'in hazırlamış olduğu [fatura](https://github.com/mlevent/fatura) `(php)` paketinden faydalanılmıştır.
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.2 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.3 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
 keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -24,19 +24,22 @@
 img.shields.io/pypi/pyversions/
 eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/
 eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
 ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
 Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
-github.com/f/fatura) paketinin Python dili ile yazÄ±lmÄ±Å versiyonudur. [!
-[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+github.com/f/fatura) `(js)` paketinin `Python` dili ile yazÄ±lmÄ±Å
+versiyonudur. > GeliÅim aÅamasÄ±nda [Mert Levent](https://github.com/
+mlevent)'in hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/mlevent/fatura) `
+(php)` paketinden faydalanÄ±lmÄ±ÅtÄ±r. [![ForTheBadge made-with-python](https:
+//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
+Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.2/README.md` & `eArsivPortal-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eArsivPortal)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/eArsivPortal?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
-> Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) paketinin Python dili ile yazılmış versiyonudur.
+
+> Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) `(js)` paketinin `Python` dili ile yazılmış versiyonudur.
+
+> Gelişim aşamasında [Mert Levent](https://github.com/mlevent)'in hazırlamış olduğu [fatura](https://github.com/mlevent/fatura) `(php)` paketinden faydalanılmıştır.
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
```

#### html2text {}

```diff
@@ -16,19 +16,22 @@
 img.shields.io/pypi/pyversions/
 eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/
 eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
 ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
 Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
-github.com/f/fatura) paketinin Python dili ile yazÄ±lmÄ±Å versiyonudur. [!
-[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+github.com/f/fatura) `(js)` paketinin `Python` dili ile yazÄ±lmÄ±Å
+versiyonudur. > GeliÅim aÅamasÄ±nda [Mert Levent](https://github.com/
+mlevent)'in hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/mlevent/fatura) `
+(php)` paketinden faydalanÄ±lmÄ±ÅtÄ±r. [![ForTheBadge made-with-python](https:
+//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
+Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.2/eArsivPortal/Core/__init__.py` & `eArsivPortal-0.0.3/eArsivPortal/Core/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,35 +3,46 @@
 from ..Libs   import legacy_session, Komut, Komutlar, fatura_ver
 from requests import Response
 from json     import dumps
 from uuid     import uuid4
 
 from .Hatalar import GirisYapilmadi, OturumSuresiDoldu, eArsivPortalHatasi
 
+from datetime import datetime
+from parsel import Selector
+
 class eArsivPortal:
     def __init__(self, kullanici_kodu:str="33333301", sifre:str="1", test_modu:bool=True):
 
         self.kullanici_kodu = kullanici_kodu
         self.sifre          = sifre
         self.test_modu      = test_modu
 
         apiler = {
-            "YAYIN" : "https://earsivportal.efatura.gov.tr",
-            "TEST"  : "https://earsivportaltest.efatura.gov.tr"
+            "YAYIN" : "https://earsivportal.efatura.gov.tr",     # * https://earsivportal.efatura.gov.tr/intragiris.html
+            "TEST"  : "https://earsivportaltest.efatura.gov.tr"  # * https://earsivportaltest.efatura.gov.tr/login.jsp
         }
 
         self.url      = apiler["TEST" if test_modu else "YAYIN"]
         self.oturum   = legacy_session()
         self.komutlar = Komutlar()
 
+        self.oturum.headers.update({
+            "User-Agent" : "https://github.com/keyiflerolsun/eArsivPortal"
+        })
+
         self.__giris_yap(kullanici_kodu, sifre)
 
     def __istek_ayristir(self, istek:Response, veri:dict) -> dict | Exception:
         if istek.status_code != 200 or veri.get("error"):
-            hata_metni = veri["messages"][0]["text"]
+            try:
+                hata_metni = veri["messages"][0]["text"]
+            except Exception:
+                hata_metni = veri["error"]["messages"][0]
+
             if "Oturum zamanaşımına uğradı" in hata_metni:
                 raise OturumSuresiDoldu(hata_metni)
 
             raise eArsivPortalHatasi(hata_metni)
 
         return veri
 
@@ -100,8 +111,44 @@
                 soyad       = soyad,
                 urun_adi    = urun_adi,
                 fiyat       = fiyat,
                 fatura_notu = fatura_notu,
             )
         )
 
-        return "Faturanız başarıyla oluşturulmuştur." in veri.get("data")
+        return "Faturanız başarıyla oluşturulmuştur." in veri.get("data")
+
+    def faturalari_getir(self, baslangic_tarihi:str="01/05/2023", bitis_tarihi:str="28/05/2023") -> list[dict]:
+        veri = self.__kod_calistir(
+            komut = self.komutlar.TASLAKLARI_GETIR,
+            jp    =     {
+                "baslangic" : baslangic_tarihi,
+                "bitis"     : bitis_tarihi,
+                "hangiTip"  :"5000/30000",
+                "table"     : []
+            }
+        )
+
+        return veri.get("data")
+
+    def fatura_html(self, ettn:str, onay_durumu:str) -> str:
+        veri = self.__kod_calistir(
+            komut = self.komutlar.FATURA_GOSTER,
+            jp    = {
+                "ettn"       : ettn,
+                "onayDurumu" : onay_durumu
+            }
+        )
+
+        secici = Selector(veri.get("data"))
+
+        for tr in secici.xpath("//tr"):
+            bos_tdler = tr.xpath(".//td[normalize-space(.)='\xa0']")
+
+            if len(bos_tdler) == len(tr.xpath(".//td")):
+                tr_element = tr.root
+                tr_element.getparent().remove(tr_element)
+
+        return secici.extract()
+
+
+    # TODO: https://github.com/mlevent/fatura 'dan faydalanarak geri kalan fonksiyonlar yazılacaktır..
```

### Comparing `eArsivPortal-0.0.2/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-0.0.3/eArsivPortal/Libs/FaturaVer.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.2/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-0.0.3/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.2/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-0.0.3/eArsivPortal/Models/Komutlar.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.2/eArsivPortal.egg-info/PKG-INFO` & `eArsivPortal-0.0.3/eArsivPortal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.2
+Version: 0.0.3
 Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,15 +27,18 @@
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eArsivPortal)
 
 [![Python Version](https://img.shields.io/pypi/pyversions/eArsivPortal?logo=python&logoColor=white&label=Python)](#)
 [![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
-> Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) paketinin Python dili ile yazılmış versiyonudur.
+
+> Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) `(js)` paketinin `Python` dili ile yazılmış versiyonudur.
+
+> Gelişim aşamasında [Mert Levent](https://github.com/mlevent)'in hazırlamış olduğu [fatura](https://github.com/mlevent/fatura) `(php)` paketinden faydalanılmıştır.
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.2 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.3 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
 keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -24,19 +24,22 @@
 img.shields.io/pypi/pyversions/
 eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/
 eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
 ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
 Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
-github.com/f/fatura) paketinin Python dili ile yazÄ±lmÄ±Å versiyonudur. [!
-[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
-python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
-ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
-keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
-[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
-PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
-eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
-â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
-mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
-ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
-*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+github.com/f/fatura) `(js)` paketinin `Python` dili ile yazÄ±lmÄ±Å
+versiyonudur. > GeliÅim aÅamasÄ±nda [Mert Levent](https://github.com/
+mlevent)'in hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/mlevent/fatura) `
+(php)` paketinden faydalanÄ±lmÄ±ÅtÄ±r. [![ForTheBadge made-with-python](https:
+//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
+) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
+with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
+Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
+keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
+(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
+*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
+iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
+Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
+[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
+[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.2/setup.py` & `eArsivPortal-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "0.0.2",
+    version      = "0.0.3",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
 
@@ -25,15 +25,17 @@
     packages         = ["eArsivPortal"],
     python_requires  = ">=3.10",
     install_requires = [
         "setuptools",
         "wheel",
         "urllib3",
         "requests",
-        "pydantic"
+        "pydantic",
+        "parsel",
+        "cssselect"
     ],
 
     # ? PyPI Bilgileri
     long_description_content_type = "text/markdown",
     long_description              = "".join(open("README.md", encoding="utf-8").readlines()),
     include_package_data          = True
 )
```

