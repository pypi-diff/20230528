# Comparing `tmp/ptrFinance-0.1.2.tar.gz` & `tmp/ptrFinance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptrFinance-0.1.2.tar", last modified: Thu Mar 30 23:40:37 2023, max compression
+gzip compressed data, was "ptrFinance-0.1.3.tar", last modified: Sun May 28 02:10:52 2023, max compression
```

## Comparing `ptrFinance-0.1.2.tar` & `ptrFinance-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 23:40:37.387481 ptrFinance-0.1.2/
--rw-rw-rw-   0        0        0     2584 2023-03-30 22:12:04.000000 ptrFinance-0.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1072 2023-02-08 18:15:55.000000 ptrFinance-0.1.2/LICENCE.txt
--rw-rw-rw-   0        0        0       39 2023-02-14 00:15:14.000000 ptrFinance-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3563 2023-03-30 23:40:37.387481 ptrFinance-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-03-19 01:05:14.000000 ptrFinance-0.1.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-03-30 23:40:37.374469 ptrFinance-0.1.2/ptrFinance/
--rw-rw-rw-   0        0        0    22307 2023-03-30 23:39:47.000000 ptrFinance-0.1.2/ptrFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 23:40:37.385977 ptrFinance-0.1.2/ptrFinance/__pycache__/
--rw-rw-rw-   0        0        0     1374 2023-02-13 23:43:16.000000 ptrFinance-0.1.2/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc
--rw-rw-rw-   0        0        0       38 2023-02-14 11:26:40.000000 ptrFinance-0.1.2/ptrFinance/repetitionCSV.csv
-drwxrwxrwx   0        0        0        0 2023-03-30 23:40:37.384977 ptrFinance-0.1.2/ptrFinance.egg-info/
--rw-rw-rw-   0        0        0     3563 2023-03-30 23:40:37.000000 ptrFinance-0.1.2/ptrFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-03-30 23:40:37.000000 ptrFinance-0.1.2/ptrFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 23:40:37.000000 ptrFinance-0.1.2/ptrFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-03-30 23:40:37.000000 ptrFinance-0.1.2/ptrFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-30 23:40:37.000000 ptrFinance-0.1.2/ptrFinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 23:40:37.388499 ptrFinance-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      798 2023-03-30 22:08:02.000000 ptrFinance-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.433061 ptrFinance-0.1.3/
+-rw-rw-rw-   0        0        0     2645 2023-05-28 02:09:26.000000 ptrFinance-0.1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1072 2023-02-08 18:15:55.000000 ptrFinance-0.1.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       39 2023-02-14 00:15:14.000000 ptrFinance-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3624 2023-05-28 02:10:52.433061 ptrFinance-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-03-19 01:05:14.000000 ptrFinance-0.1.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.416984 ptrFinance-0.1.3/ptrFinance/
+-rw-rw-rw-   0        0        0    23005 2023-05-27 15:19:31.000000 ptrFinance-0.1.3/ptrFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.432041 ptrFinance-0.1.3/ptrFinance/__pycache__/
+-rw-rw-rw-   0        0        0     1374 2023-02-13 23:43:16.000000 ptrFinance-0.1.3/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc
+-rw-rw-rw-   0        0        0       38 2023-02-14 11:26:40.000000 ptrFinance-0.1.3/ptrFinance/repetitionCSV.csv
+drwxrwxrwx   0        0        0        0 2023-05-28 02:10:52.426537 ptrFinance-0.1.3/ptrFinance.egg-info/
+-rw-rw-rw-   0        0        0     3624 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-05-28 02:10:52.000000 ptrFinance-0.1.3/ptrFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 02:10:51.000000 ptrFinance-0.1.3/ptrFinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 02:10:52.434425 ptrFinance-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-05-28 02:09:08.000000 ptrFinance-0.1.3/setup.py
```

### Comparing `ptrFinance-0.1.2/CHANGELOG.txt` & `ptrFinance-0.1.3/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Change Log
 ==========
 Version "0.1.2" (2/30/2023)
+getLiveValues function added
+
+Version "0.1.2" (2/30/2023)
 returnDailyStockReviewArticle different companies bug fix
 
 Version "0.1.1" (2/30/2023)
 Bug Fix
 
 Version "0.1.0" (2/30/2023)
 impliedVolatilityFunc creation. Used to return the current specified stocks volatility, as well as the previous months volitility.
```

### Comparing `ptrFinance-0.1.2/LICENCE.txt` & `ptrFinance-0.1.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `ptrFinance-0.1.2/PKG-INFO` & `ptrFinance-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptrFinance
-Version: 0.1.2
+Version: 0.1.3
 Summary: Financial Web Scraping Library
 Home-page: 
 Author: Rocco Pio Maria Petruccio
 Author-email: whatsappbackuprocco@gmail.com
 License: MIT
 Keywords: Web Scraping,Finance
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,17 @@
 
 The GitHub repository is located at: https://github.com/123Rocco123/Web-Scraping-Pip-Library
 
 
 Change Log
 ==========
 Version "0.1.2" (2/30/2023)
+getLiveValues function added
+
+Version "0.1.2" (2/30/2023)
 returnDailyStockReviewArticle different companies bug fix
 
 Version "0.1.1" (2/30/2023)
 Bug Fix
 
 Version "0.1.0" (2/30/2023)
 impliedVolatilityFunc creation. Used to return the current specified stocks volatility, as well as the previous months volitility.
```

### Comparing `ptrFinance-0.1.2/ptrFinance/__init__.py` & `ptrFinance-0.1.3/ptrFinance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,31 @@
 from bs4 import BeautifulSoup
 from datetime import datetime
 from csv import writer
 
 # Class Variable
 previousVol = 0
 
+# Function used to get the current stock values of the specified stocks
+    # stocks parameter is used to contain the array with all the names of the stocks
+def getLiveValues(stocks):
+    # Return array used to contain the live values for each stock
+    liveValues = {}
+
+    # Iterate over the file
+    for x in stocks:
+        session = HTMLSession()
+        stockValues = session.get("https://finance.yahoo.com/quote/{stock}".format(stock = x)).text
+        soup = BeautifulSoup(stockValues, "html5lib")
+
+        # Append the stock with the current value
+        liveValues[x] = soup.find("fin-streamer", {"class" : "Fw(b) Fz(36px) Mb(-4px) D(ib)"}).text
+
+    return liveValues
+
 # Used for the whileTrueStock
 def repetitionsFunc(stockName, interval, repetitions):
     global previousVol
 
     session = HTMLSession()
     requests = session.get("https://finance.yahoo.com/quote/{stockName}/history?p={stockName}".format(stockName = stockName)).text
```

### Comparing `ptrFinance-0.1.2/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc` & `ptrFinance-0.1.3/ptrFinance/__pycache__/repetitionFunction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ptrFinance-0.1.2/ptrFinance.egg-info/PKG-INFO` & `ptrFinance-0.1.3/ptrFinance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptrFinance
-Version: 0.1.2
+Version: 0.1.3
 Summary: Financial Web Scraping Library
 Home-page: 
 Author: Rocco Pio Maria Petruccio
 Author-email: whatsappbackuprocco@gmail.com
 License: MIT
 Keywords: Web Scraping,Finance
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,14 +20,17 @@
 
 The GitHub repository is located at: https://github.com/123Rocco123/Web-Scraping-Pip-Library
 
 
 Change Log
 ==========
 Version "0.1.2" (2/30/2023)
+getLiveValues function added
+
+Version "0.1.2" (2/30/2023)
 returnDailyStockReviewArticle different companies bug fix
 
 Version "0.1.1" (2/30/2023)
 Bug Fix
 
 Version "0.1.0" (2/30/2023)
 impliedVolatilityFunc creation. Used to return the current specified stocks volatility, as well as the previous months volitility.
```

### Comparing `ptrFinance-0.1.2/setup.py` & `ptrFinance-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='ptrFinance',
-  version='0.1.2',
+  version='0.1.3',
   description='Financial Web Scraping Library',
   long_description= open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',
   author='Rocco Pio Maria Petruccio',
   author_email='whatsappbackuprocco@gmail.com',
   license='MIT',
   classifiers=classifiers,
```

