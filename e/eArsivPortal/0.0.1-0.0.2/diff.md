# Comparing `tmp/eArsivPortal-0.0.1.tar.gz` & `tmp/eArsivPortal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eArsivPortal-0.0.1.tar", last modified: Sun May 28 12:05:33 2023, max compression
+gzip compressed data, was "eArsivPortal-0.0.2.tar", last modified: Sun May 28 12:24:49 2023, max compression
```

## Comparing `eArsivPortal-0.0.1.tar` & `eArsivPortal-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)    35149 2023-05-28 11:40:18.000000 eArsivPortal-0.0.1/LICENSE
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       32 2023-05-28 12:03:15.000000 eArsivPortal-0.0.1/MANIFEST.in
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2149 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1559 2023-05-28 11:43:47.000000 eArsivPortal-0.0.1/README.md
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/eArsivPortal/
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/eArsivPortal/Core/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      212 2023-05-28 11:47:10.000000 eArsivPortal-0.0.1/eArsivPortal/Core/Hatalar.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     3778 2023-05-28 11:54:28.000000 eArsivPortal-0.0.1/eArsivPortal/Core/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/eArsivPortal/Libs/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     3405 2023-05-28 11:47:10.000000 eArsivPortal-0.0.1/eArsivPortal/Libs/FaturaVer.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      785 2023-05-28 11:47:10.000000 eArsivPortal-0.0.1/eArsivPortal/Libs/Oturum.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      188 2023-05-28 11:51:43.000000 eArsivPortal-0.0.1/eArsivPortal/Libs/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/eArsivPortal/Models/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2132 2023-05-28 11:47:10.000000 eArsivPortal-0.0.1/eArsivPortal/Models/Komutlar.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      115 2023-05-28 11:53:10.000000 eArsivPortal-0.0.1/eArsivPortal/Models/__init__.py
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      108 2023-05-28 12:01:41.000000 eArsivPortal-0.0.1/eArsivPortal/__init__.py
-drwxr-xr-x   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        0 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/eArsivPortal.egg-info/
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     2149 2023-05-28 12:05:33.000000 eArsivPortal-0.0.1/eArsivPortal.egg-info/PKG-INFO
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)      454 2023-05-28 12:05:33.000000 eArsivPortal-0.0.1/eArsivPortal.egg-info/SOURCES.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)        1 2023-05-28 12:05:33.000000 eArsivPortal-0.0.1/eArsivPortal.egg-info/dependency_links.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       43 2023-05-28 12:05:33.000000 eArsivPortal-0.0.1/eArsivPortal.egg-info/requires.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       13 2023-05-28 12:05:33.000000 eArsivPortal-0.0.1/eArsivPortal.egg-info/top_level.txt
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)       38 2023-05-28 12:05:33.432329 eArsivPortal-0.0.1/setup.cfg
--rw-r--r--   0 keyiflerolsun  (1000) keyiflerolsun  (1000)     1221 2023-05-28 11:56:32.000000 eArsivPortal-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.017140 eArsivPortal-0.0.2/eArsivPortal/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Core/Hatalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Libs/FaturaVer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Models/Komutlar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/eArsivPortal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/eArsivPortal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 12:24:49.000000 eArsivPortal-0.0.2/eArsivPortal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:24:49.021140 eArsivPortal-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-28 12:24:16.000000 eArsivPortal-0.0.2/setup.py
```

### Comparing `eArsivPortal-0.0.1/LICENSE` & `eArsivPortal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.1/PKG-INFO` & `eArsivPortal-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eArsivPortal
-Version: 0.0.1
+Version: 0.0.2
 Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
 Home-page: https://github.com/keyiflerolsun/eArsivPortal
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,14 +16,24 @@
 
 # 🧾 eArsivPortal
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eArsivPortal&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
+[![PyPI Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eArsivPortal/PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml)
+
+[![PyPI](https://img.shields.io/pypi/v/eArsivPortal?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/eArsivPortal)
+[![PyPI - Yüklenme](https://img.shields.io/pypi/dm/eArsivPortal?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/eArsivPortal)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eArsivPortal)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/eArsivPortal?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
+
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
 > Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) paketinin Python dili ile yazılmış versiyonudur.
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
```

#### html2text {}

```diff
@@ -1,28 +1,42 @@
-Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.1 Summary: GÄ°B e-ArÅiv
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.2 Summary: GÄ°B e-ArÅiv
 Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
 keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # ð§¾ eArsivPortal [![Boyut](https://img.shields.io/github/repo-size/
 keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#) [!
 [GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https://github.com/keyiflerolsun/
 eArsivPortal&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/âï¸-
-Kahve_Ismarla-ffdd00] *GÄ°B e-ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil
-OluÅturucu* > Bu paket [Fatih Kadir AkÄ±n](https://github.com/f)'Ä±n
-hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/f/fatura) paketinin Python
-dili ile yazÄ±lmÄ±Å versiyonudur. [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
-Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
-*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
-iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
-Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
-[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
-[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+Kahve_Ismarla-ffdd00] [![PyPI YÃ¼kleyici](https://img.shields.io/github/
+actions/workflow/status/keyiflerolsun/eArsivPortal/
+PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
+keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml) [![PyPI](https://
+img.shields.io/pypi/v/eArsivPortal?logo=pypi&logoColor=white&label=PyPI)]
+(https://pypi.org/project/eArsivPortal) [![PyPI - YÃ¼klenme](https://
+img.shields.io/pypi/dm/eArsivPortal?logo=pypi&logoColor=white&label=YÃ¼klenme)]
+(https://pypi.org/project/eArsivPortal) [![PyPI - Wheel](https://
+img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)]
+(https://pypi.org/project/eArsivPortal) [![Python Version](https://
+img.shields.io/pypi/pyversions/
+eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
+img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/
+eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
+ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
+Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
+github.com/f/fatura) paketinin Python dili ile yazÄ±lmÄ±Å versiyonudur. [!
+[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
+python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
+ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
+keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.1/README.md` & `eArsivPortal-0.0.2/eArsivPortal.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,39 @@
+Metadata-Version: 2.1
+Name: eArsivPortal
+Version: 0.0.2
+Summary: GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu
+Home-page: https://github.com/keyiflerolsun/eArsivPortal
+Author: keyiflerolsun
+Author-email: keyiflerolsun@gmail.com
+License: GPLv3+
+Keywords: eArsivPortal,KekikAkademi,keyiflerolsun
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 🧾 eArsivPortal
 
 [![Boyut](https://img.shields.io/github/repo-size/keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#)
 [![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/eArsivPortal&title=Görüntülenme)](#)
 <a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
 
+[![PyPI Yükleyici](https://img.shields.io/github/actions/workflow/status/keyiflerolsun/eArsivPortal/PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml)
+
+[![PyPI](https://img.shields.io/pypi/v/eArsivPortal?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/eArsivPortal)
+[![PyPI - Yüklenme](https://img.shields.io/pypi/dm/eArsivPortal?logo=pypi&logoColor=white&label=Yüklenme)](https://pypi.org/project/eArsivPortal)
+[![PyPI - Wheel](https://img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)](https://pypi.org/project/eArsivPortal)
+
+[![Python Version](https://img.shields.io/pypi/pyversions/eArsivPortal?logo=python&logoColor=white&label=Python)](#)
+[![Lisans](https://img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#)
+
 *GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu*
 > Bu paket [Fatih Kadir Akın](https://github.com/f)'ın hazırlamış olduğu [fatura](https://github.com/f/fatura) paketinin Python dili ile yazılmış versiyonudur.
 
 [![ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 [![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)
 
 ## 🌐 Telif Hakkı ve Lisans
@@ -21,8 +47,8 @@
 
 ## 💸 Bağış Yap
 
 **[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
 
 ***
 
-> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
+> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*
```

#### html2text {}

```diff
@@ -1,20 +1,42 @@
-# ð§¾ eArsivPortal [![Boyut](https://img.shields.io/github/repo-size/
+Metadata-Version: 2.1 Name: eArsivPortal Version: 0.0.2 Summary: GÄ°B e-ArÅiv
+Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu Home-page: https://github.com/
+keyiflerolsun/eArsivPortal Author: keyiflerolsun Author-email:
+keyiflerolsun@gmail.com License: GPLv3+ Keywords:
+eArsivPortal,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
+Production/Stable Classifier: License :: OSI Approved :: GNU General Public
+License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
+LICENSE # ð§¾ eArsivPortal [![Boyut](https://img.shields.io/github/repo-size/
 keyiflerolsun/eArsivPortal?logo=git&logoColor=white&label=Boyut)](#) [!
 [GÃ¶rÃ¼ntÃ¼lenme](https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https://github.com/keyiflerolsun/
 eArsivPortal&title=GÃ¶rÃ¼ntÃ¼lenme)](#) [https://img.shields.io/badge/âï¸-
-Kahve_Ismarla-ffdd00] *GÄ°B e-ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil
-OluÅturucu* > Bu paket [Fatih Kadir AkÄ±n](https://github.com/f)'Ä±n
-hazÄ±rlamÄ±Å olduÄu [fatura](https://github.com/f/fatura) paketinin Python
-dili ile yazÄ±lmÄ±Å versiyonudur. [![ForTheBadge made-with-python](https://
-ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
-[![ForTheBadge built-with-love](https://ForTheBadge.com/images/badges/built-
-with-love.svg)](https://GitHub.com/keyiflerolsun/) ## ð Telif HakkÄ± ve
-Lisans * *Copyright (C) 2023 by* [keyiflerolsun](https://github.com/
-keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007]
-(https://github.com/keyiflerolsun/eArsivPortal/blob/master/LICENSE)
-*KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ## â»ï¸ Ä°letiÅim *Benimle
-iletiÅime geÃ§mek isterseniz, **Telegram**'dan mesaj gÃ¶ndermekten
-Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ## ð¸ BaÄÄ±Å Yap **
-[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)** *** > **
-[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
+Kahve_Ismarla-ffdd00] [![PyPI YÃ¼kleyici](https://img.shields.io/github/
+actions/workflow/status/keyiflerolsun/eArsivPortal/
+PyPI.yml?label=PyPI%20Y%C3%BCkleyici&logo=github)](https://github.com/
+keyiflerolsun/eArsivPortal/actions/workflows/PyPI.yml) [![PyPI](https://
+img.shields.io/pypi/v/eArsivPortal?logo=pypi&logoColor=white&label=PyPI)]
+(https://pypi.org/project/eArsivPortal) [![PyPI - YÃ¼klenme](https://
+img.shields.io/pypi/dm/eArsivPortal?logo=pypi&logoColor=white&label=YÃ¼klenme)]
+(https://pypi.org/project/eArsivPortal) [![PyPI - Wheel](https://
+img.shields.io/pypi/wheel/eArsivPortal?logo=pypi&logoColor=white&label=Wheel)]
+(https://pypi.org/project/eArsivPortal) [![Python Version](https://
+img.shields.io/pypi/pyversions/
+eArsivPortal?logo=python&logoColor=white&label=Python)](#) [![Lisans](https://
+img.shields.io/pypi/l/eArsivPortal?logo=gnu&logoColor=white&label=Lisans)](#)
+[![Durum](https://img.shields.io/pypi/status/
+eArsivPortal?logo=windowsterminal&logoColor=white&label=Durum)](#) *GÄ°B e-
+ArÅiv Portal e-Fatura, e-SMM, e-MÃ¼stahsil OluÅturucu* > Bu paket [Fatih
+Kadir AkÄ±n](https://github.com/f)'Ä±n hazÄ±rlamÄ±Å olduÄu [fatura](https://
+github.com/f/fatura) paketinin Python dili ile yazÄ±lmÄ±Å versiyonudur. [!
+[ForTheBadge made-with-python](https://ForTheBadge.com/images/badges/made-with-
+python.svg)](https://www.python.org/) [![ForTheBadge built-with-love](https://
+ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/
+keyiflerolsun/) ## ð Telif HakkÄ± ve Lisans * *Copyright (C) 2023 by*
+[keyiflerolsun](https://github.com/keyiflerolsun) â¤ï¸ï¸ * [GNU GENERAL
+PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/
+eArsivPortal/blob/master/LICENSE) *KoÅullarÄ±na gÃ¶re lisanslanmÄ±ÅtÄ±r..* ##
+â»ï¸ Ä°letiÅim *Benimle iletiÅime geÃ§mek isterseniz, **Telegram**'dan
+mesaj gÃ¶ndermekten Ã§ekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve) ##
+ð¸ BaÄÄ±Å Yap **[âï¸ Kahve Ismarla](https://KekikAkademi.org/Kahve)**
+*** > **[@KekikAkademi](https://t.me/KekikAkademi)** *iÃ§in yazÄ±lmÄ±ÅtÄ±r..*
```

### Comparing `eArsivPortal-0.0.1/eArsivPortal/Core/__init__.py` & `eArsivPortal-0.0.2/eArsivPortal/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.1/eArsivPortal/Libs/FaturaVer.py` & `eArsivPortal-0.0.2/eArsivPortal/Libs/FaturaVer.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.1/eArsivPortal/Libs/Oturum.py` & `eArsivPortal-0.0.2/eArsivPortal/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.1/eArsivPortal/Models/Komutlar.py` & `eArsivPortal-0.0.2/eArsivPortal/Models/Komutlar.py`

 * *Files identical despite different names*

### Comparing `eArsivPortal-0.0.1/setup.py` & `eArsivPortal-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eArsivPortal",
-    version      = "0.0.1",
+    version      = "0.0.2",
     url          = "https://github.com/keyiflerolsun/eArsivPortal",
     description  = "GİB e-Arşiv Portal e-Fatura, e-SMM, e-Müstahsil Oluşturucu",
     keywords     = ["eArsivPortal", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

