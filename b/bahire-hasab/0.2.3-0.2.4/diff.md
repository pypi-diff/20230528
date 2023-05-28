# Comparing `tmp/bahire-hasab-0.2.3.tar.gz` & `tmp/bahire-hasab-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bahire-hasab-0.2.3.tar", last modified: Sun May 28 10:50:41 2023, max compression
+gzip compressed data, was "bahire-hasab-0.2.4.tar", last modified: Sun May 28 10:57:42 2023, max compression
```

## Comparing `bahire-hasab-0.2.3.tar` & `bahire-hasab-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:50:41.714022 bahire-hasab-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 10:50:30.000000 bahire-hasab-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:50:41.714022 bahire-hasab-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-28 10:50:30.000000 bahire-hasab-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 10:50:30.000000 bahire-hasab-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 10:50:41.714022 bahire-hasab-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-28 10:50:30.000000 bahire-hasab-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:50:41.710022 bahire-hasab-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:50:41.714022 bahire-hasab-0.2.3/src/bahire_hasab/
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-28 10:50:30.000000 bahire-hasab-0.2.3/src/bahire_hasab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:50:41.714022 bahire-hasab-0.2.3/src/bahire_hasab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:50:41.000000 bahire-hasab-0.2.3/src/bahire_hasab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 10:50:41.000000 bahire-hasab-0.2.3/src/bahire_hasab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:50:41.000000 bahire-hasab-0.2.3/src/bahire_hasab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 10:50:41.000000 bahire-hasab-0.2.3/src/bahire_hasab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/src/bahire_hasab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-28 10:57:31.000000 bahire-hasab-0.2.4/src/bahire_hasab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 10:57:42.589565 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-28 10:57:42.000000 bahire-hasab-0.2.4/src/bahire_hasab.egg-info/top_level.txt
```

### Comparing `bahire-hasab-0.2.3/LICENSE` & `bahire-hasab-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.3/PKG-INFO` & `bahire-hasab-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.3 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.4 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

### Comparing `bahire-hasab-0.2.3/README.md` & `bahire-hasab-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bahire-hasab-0.2.3/src/bahire_hasab/__init__.py` & `bahire-hasab-0.2.4/src/bahire_hasab/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,52 +145,52 @@
         _bw = self.WERAT[self.WERAT.index(_nw) + (_bk // 30)]
         _bk = _bk % 30 if _bk > 30 else _bk
         return f"{_bw} {_bk}"
 
     @property
     def abiy_tsom(self):
         """A Function for finding the day of enterance of the Great lent according to the Ethiopian Calendar."""
-        return self.beal(beal=self.BEALAT[1])
+        return self.atswamat_webealat(beal=self.BEALAT[1])
 
     @property
     def debre_zeyt(self):
         """A function for finding the date of debrezeyt(The middle of Great lent)."""
-        return self.beal(beal=self.BEALAT[2])
+        return self.atswamat_webealat(beal=self.BEALAT[2])
 
     @property
     def hosaena(self):
         """A function for calculating the date of Hosaena in Ethiopian Calendar"""
-        return self.beal(beal=self.BEALAT[3])
+        return self.atswamat_webealat(beal=self.BEALAT[3])
 
     @property
     def sklet(self):
         """A function for calculating the date of Sklet(Crufication) in Ethiopian Calendar."""
-        return self.beal(beal=self.BEALAT[4])
+        return self.atswamat_webealat(beal=self.BEALAT[4])
 
     @property
     def tnsae(self):
         """A function for calculating the date of Tnsae(The end of Great lent) in Ethiopian Calendar."""
-        return self.beal(beal=self.BEALAT[5])
+        return self.atswamat_webealat(beal=self.BEALAT[5])
 
     @property
     def rkbe_kahnat(self):
         """A function for calculating the date of rkbe kahnat(The meeting of Priests) in Ethiopian Calendar."""
-        return self.beal(beal=self.BEALAT[6])
+        return self.atswamat_webealat(beal=self.BEALAT[6])
 
     @property
     def erget(self):
         """A function for calculating the date of Erget in Ethiopian Calendar."""
-        return self.beal(beal=self.BEALAT[7])
+        return self.atswamat_webealat(beal=self.BEALAT[7])
 
     @property
     def beale_hamsa(self):
         """A function for calculating the date of Beale hamsa in Ethiopian Calendar."""
-        return self.beal(beal=self.BEALAT[8])
+        return self.atswamat_webealat(beal=self.BEALAT[8])
 
     @property
     def tsome_hawaryat(self):
         """A function for finding the date of Tsome Hawaryat (Lent of The Apostels) in Ethiopian Calendar."""
-        return self.beal(beal=self.BEALAT[9])
+        return self.atswamat_webealat(beal=self.BEALAT[9])
 
     @property
     def tsome_dhnet(self):
-        return self.beal(beal=self.BEALAT[10])
+        return self.atswamat_webealat(beal=self.BEALAT[10])
```

### Comparing `bahire-hasab-0.2.3/src/bahire_hasab.egg-info/PKG-INFO` & `bahire-hasab-0.2.4/src/bahire_hasab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bahire-hasab
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/hunderaweke/bahire-hasab
 Author: Hundera Awoke
 Author-email: hunderaweke@gmail.com
 Keywords: bahire_hasab
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.3 Home-page: https://
+Metadata-Version: 2.1 Name: bahire-hasab Version: 0.2.4 Home-page: https://
 github.com/hunderaweke/bahire-hasab Author: Hundera Awoke Author-email:
 hunderaweke@gmail.com Keywords: bahire_hasab Description-Content-Type: text/
 markdown License-File: LICENSE
       ****** ð Bahire Hassab(á£áá¨ áá³á¥) ðªð¹ ð¦ ******
 [![Upload Python Package](https://github.com/hunderaweke/bahire-hasab/actions/
 workflows/python-publish.yml/badge.svg)](https://github.com/hunderaweke/bahire-
 hasab/actions/workflows/python-publish.yml) - A python module for calculating
```

