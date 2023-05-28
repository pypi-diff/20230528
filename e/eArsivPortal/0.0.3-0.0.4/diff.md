# Comparing `tmp/eArsivPortal-0.0.3.tar.gz` & `tmp/eArsivPortal-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-0.0.3.tar", last modified: Sun May 28 13:55:27 2023, max compression
+gzip compressed data, was "eArsivPortal-0.0.4.tar", last modified: Sun May 28 14:16:29 2023, max compression
```

## Comparing `eArsivPortal-0.0.3.tar` & `eArsivPortal-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/eArsivPortal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/eArsivPortal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 13:55:27.000000 eArsivPortal-0.0.3/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 13:55:27.243828 eArsivPortal-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-28 13:54:31.000000 eArsivPortal-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:16:29.542039 eArsivPortal-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-28 14:16:29.542039 eArsivPortal-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:16:29.538039 eArsivPortal-0.0.4/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:16:29.542039 eArsivPortal-0.0.4/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:16:29.542039 eArsivPortal-0.0.4/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:16:29.542039 eArsivPortal-0.0.4/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:16:29.542039 eArsivPortal-0.0.4/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-28 14:16:29.000000 eArsivPortal-0.0.4/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-28 14:16:29.000000 eArsivPortal-0.0.4/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:16:29.000000 eArsivPortal-0.0.4/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 14:16:29.000000 eArsivPortal-0.0.4/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 14:16:29.000000 eArsivPortal-0.0.4/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:16:29.542039 eArsivPortal-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-28 14:15:30.000000 eArsivPortal-0.0.4/setup.py
```

### Comparing `eArsivPortal-0.0.3/LICENSE` & `eArsivPortal-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.3/PKG-INFO` & `eArsivPortal-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.3
+Version: 0.0.4
 Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,16 +30,14 @@
 [![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
 
 > Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) `(js)` paketinin `Python` dili ile yazılmış versiyonudur.
 
-> Gelişim aşamasında [Mert Levent](https://github.com/mlevent)'in hazırlamış olduğu [fatura](https://github.com/mlevent/fatura) `(php)` paketinden faydalanılmıştır.
-
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.3 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.4 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
 keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -25,21 +25,18 @@
 eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/
 eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
 ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
 Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
 github.com/f/fatura) `(js)` paketinin `Python` dili ile yazÄ±lmÄ±Å
-versiyonudur. > GeliÅim aÅamasÄ±nda [Mert Levent](https://github.com/
-mlevent)'in hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/mlevent/fatura) `
-(php)` paketinden faydalanÄ±lmÄ±ÅtÄ±r. [![ForTheBadge made-with-python](https:
-//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
-) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
-Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
-*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
-iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
-Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
-[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
-[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+versiyonudur. [![ForTheBadge made-with-python](https://ForTheBadge.com/images/
+badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge built-
+with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023
+by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.3/README.md` & `eArsivPortal-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 [![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
 
 > Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) `(js)` paketinin `Python` dili ile yazılmış versiyonudur.
 
-> Gelişim aşamasında [Mert Levent](https://github.com/mlevent)'in hazırlamış olduğu [fatura](https://github.com/mlevent/fatura) `(php)` paketinden faydalanılmıştır.
-
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
```

#### html2text {}

```diff
@@ -17,21 +17,18 @@
 eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/
 eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
 ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
 Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
 github.com/f/fatura) `(js)` paketinin `Python` dili ile yazÄ±lmÄ±Å
-versiyonudur. > GeliÅim aÅamasÄ±nda [Mert Levent](https://github.com/
-mlevent)'in hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/mlevent/fatura) `
-(php)` paketinden faydalanÄ±lmÄ±ÅtÄ±r. [![ForTheBadge made-with-python](https:
-//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
-) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
-Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
-*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
-iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
-Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
-[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
-[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+versiyonudur. [![ForTheBadge made-with-python](https://ForTheBadge.com/images/
+badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge built-
+with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023
+by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.3/eArsivPortal/Core/__init__.py` & `eArsivPortal-0.0.4/eArsivPortal/Core/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 from ..Libs   import legacy_session, Komut, Komutlar, fatura_ver
 from requests import Response
 from json     import dumps
 from uuid     import uuid4
-
+from parsel   import Selector
 from .Hatalar import GirisYapilmadi, OturumSuresiDoldu, eArsivPortalHatasi
 
 from datetime import datetime
-from parsel import Selector
+from pytz     import timezone
 
 class eArsivPortal:
     def __init__(self, kullanici_kodu:str="33333301", sifre:str="1", test_modu:bool=True):
 
         self.kullanici_kodu = kullanici_kodu
         self.sifre          = sifre
         self.test_modu      = test_modu
@@ -32,16 +32,16 @@
 
         self.__giris_yap(kullanici_kodu, sifre)
 
     def __istek_ayristir(self, istek:Response, veri:dict) -> dict | Exception:
         if istek.status_code != 200 or veri.get("error"):
             try:
                 hata_metni = veri["messages"][0]["text"]
-            except Exception:
-                hata_metni = veri["error"]["messages"][0]
+            except TypeError:
+                hata_metni = veri["messages"][0]
 
             if "Oturum zamanaşımına uğradı" in hata_metni:
                 raise OturumSuresiDoldu(hata_metni)
 
             raise eArsivPortalHatasi(hata_metni)
 
         return veri
@@ -88,45 +88,63 @@
         veri = self.__kod_calistir(
             komut = self.komutlar.KULLANICI_BILGILERI_GETIR,
             jp    = {}
         )
 
         return veri.get("data")
 
+    def kisi_getir(self, vkn_veya_tckn:str):
+        veri = self.__kod_calistir(
+            komut = self.komutlar.MERNISTEN_BILGILERI_GETIR,
+            jp    = {
+                "vknTckn" : vkn_veya_tckn
+            }
+        )
+
+        return veri.get("data")
+
     def fatura_olustur(
         self,
         tarih:str         = "07/10/1995",
         saat:str          = "14:28:37",
+        vkn_veya_tckn:str = "11111111111",
         ad:str            = "Ömer Faruk",
         soyad:str         = "Sancak",
+        unvan:str         = "",
+        vergi_dairesi:str = "",
         urun_adi:str      = "Python Yazılım Hizmeti",
         fiyat:int | float = 100,
         fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
     ) -> bool:
+        kisi_bilgi = self.kisi_getir(vkn_veya_tckn)
+
         veri = self.__kod_calistir(
             komut = self.komutlar.FATURA_OLUSTUR,
             jp    = fatura_ver(
-                tarih       = tarih,
-                saat        = saat,
-                ad          = ad,
-                soyad       = soyad,
-                urun_adi    = urun_adi,
-                fiyat       = fiyat,
-                fatura_notu = fatura_notu,
+                tarih         = tarih or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
+                saat          = saat,
+                vkn_veya_tckn = vkn_veya_tckn,
+                ad            = kisi_bilgi.get("adi") or ad,
+                soyad         = kisi_bilgi.get("soyadi") or soyad,
+                unvan         = kisi_bilgi.get("unvan") or unvan,
+                vergi_dairesi = kisi_bilgi.get("vergiDairesi") or vergi_dairesi,
+                urun_adi      = urun_adi,
+                fiyat         = fiyat,
+                fatura_notu   = fatura_notu
             )
         )
 
         return "Faturanız başarıyla oluşturulmuştur." in veri.get("data")
 
     def faturalari_getir(self, baslangic_tarihi:str="01/05/2023", bitis_tarihi:str="28/05/2023") -> list[dict]:
         veri = self.__kod_calistir(
             komut = self.komutlar.TASLAKLARI_GETIR,
             jp    =     {
                 "baslangic" : baslangic_tarihi,
-                "bitis"     : bitis_tarihi,
+                "bitis"     : bitis_tarihi or datetime.now(timezone("Turkey")).strftime("%d/%m/%Y"),
                 "hangiTip"  :"5000/30000",
                 "table"     : []
             }
         )
 
         return veri.get("data")
```

### Comparing `eArsivPortal-0.0.3/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-0.0.4/eArsivPortal/Libs/FaturaVer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Bu araç @keyiflerolsun tarafından | @KekikAkademi için yazılmıştır.
 
 from uuid import uuid4
 
 def fatura_ver(
     tarih:str         = "07/10/1995",
     saat:str          = "14:28:37",
+    vkn_veya_tckn:str = "11111111111",
     ad:str            = "Ömer Faruk",
     soyad:str         = "Sancak",
+    unvan:str         = "",
+    vergi_dairesi:str = "",
     urun_adi:str      = "Python Yazılım Hizmeti",
     fiyat:int | float = 100,
     fatura_notu:str   = "— QNB Finansbank —\nTR70 0011 1000 0000 0118 5102 59\nÖmer Faruk Sancak"
 ):
     matrah = fiyat / 1.18
     kdv    = fiyat - matrah
     return {
@@ -18,23 +21,23 @@
         "belgeNumarasi"     : "",
         "faturaTarihi"      : tarih,
         "saat"              : saat,
         "paraBirimi"        : "TRY",
         "dovzTLkur"         : "0",
         "faturaTipi"        : "SATIS",
         "hangiTip"          : "5000/30000",
-        "vknTckn"           : "11111111111",
-        "aliciUnvan"        : "",
+        "vknTckn"           : vkn_veya_tckn,
+        "aliciUnvan"        : unvan,
         "aliciAdi"          : ad,
         "aliciSoyadi"       : soyad,
         "binaAdi"           : "",
         "binaNo"            : "",
         "kapiNo"            : "",
         "kasabaKoy"         : "",
-        "vergiDairesi"      : "",
+        "vergiDairesi"      : vergi_dairesi,
         "ulke"              : "Türkiye",
         "bulvarcaddesokak"  : "",
         "irsaliyeNumarasi"  : "",
         "irsaliyeTarihi"    : "",
         "mahalleSemtIlce"   : "",
         "sehir"             : " ",
         "postaKodu"         : "",
```

### Comparing `eArsivPortal-0.0.3/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-0.0.4/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.3/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-0.0.4/eArsivPortal/Models/Komutlar.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.3/eArsivPortal.egg-info/PKG-INFO` & `eArsivPortal-0.0.4/eArsivPortal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.3
+Version: 0.0.4
 Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,16 +30,14 @@
 [![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
 
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
 
 > Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) `(js)` paketinin `Python` dili ile yazılmış versiyonudur.
 
-> Gelişim aşamasında [Mert Levent](https://github.com/mlevent)'in hazırlamış olduğu [fatura](https://github.com/mlevent/fatura) `(php)` paketinden faydalanılmıştır.
-
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
 
 * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
 * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.3 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.4 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
 keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
@@ -25,21 +25,18 @@
 eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
 img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
 [![Durum](https://img.shields.io/pypi/status/
 eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
 ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
 Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
 github.com/f/fatura) `(js)` paketinin `Python` dili ile yazÄ±lmÄ±Å
-versiyonudur. > GeliÅim aÅamasÄ±nda [Mert Levent](https://github.com/
-mlevent)'in hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/mlevent/fatura) `
-(php)` paketinden faydalanÄ±lmÄ±ÅtÄ±r. [![ForTheBadge made-with-python](https:
-//ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/
-) [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
-Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
-*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
-iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
-Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
-[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
-[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+versiyonudur. [![ForTheBadge made-with-python](https://ForTheBadge.com/images/
+badges/made-with-python.svg)](https://www.python.org/) [![ForTheBadge built-
+with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://
+GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023
+by* [keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.3/setup.py` & `eArsivPortal-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "0.0.3",
+    version      = "0.0.4",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

