# Comparing `tmp/RStockvn-2.1.8.tar.gz` & `tmp/RStockvn-2.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RStockvn-2.1.8.tar", last modified: Thu Apr 27 03:05:18 2023, max compression
+gzip compressed data, was "RStockvn-2.1.81.tar", last modified: Sun May 28 03:36:43 2023, max compression
```

## Comparing `RStockvn-2.1.8.tar` & `RStockvn-2.1.81.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 03:05:18.641405 RStockvn-2.1.8/
--rw-rw-rw-   0        0        0     1090 2023-01-29 04:27:43.000000 RStockvn-2.1.8/LICENSE
--rw-rw-rw-   0        0        0     9446 2023-04-27 03:05:18.640404 RStockvn-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8586 2023-03-01 05:06:26.000000 RStockvn-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 03:05:18.589154 RStockvn-2.1.8/RStockvn/
--rw-rw-rw-   0        0        0      833 2023-04-27 02:56:04.000000 RStockvn-2.1.8/RStockvn/__init__.py
--rw-rw-rw-   0        0        0     2668 2023-04-27 03:01:50.000000 RStockvn-2.1.8/RStockvn/cafef_test.py
--rw-rw-rw-   0        0        0     6344 2023-03-01 05:00:59.000000 RStockvn-2.1.8/RStockvn/data_cafef.py
--rw-rw-rw-   0        0        0    19726 2023-03-01 05:09:24.000000 RStockvn-2.1.8/RStockvn/stockvn.py
--rw-rw-rw-   0        0        0   139694 2023-02-06 06:33:27.000000 RStockvn-2.1.8/RStockvn/user_agent.py
-drwxrwxrwx   0        0        0        0 2023-04-27 03:05:18.638021 RStockvn-2.1.8/RStockvn.egg-info/
--rw-rw-rw-   0        0        0     9446 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 03:05:18.000000 RStockvn-2.1.8/RStockvn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 03:05:18.641405 RStockvn-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1215 2023-04-27 03:02:27.000000 RStockvn-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 03:36:43.804501 RStockvn-2.1.81/
+-rw-rw-rw-   0        0        0     1090 2023-01-29 04:27:43.000000 RStockvn-2.1.81/LICENSE
+-rw-rw-rw-   0        0        0    10092 2023-05-28 03:36:43.804501 RStockvn-2.1.81/PKG-INFO
+-rw-rw-rw-   0        0        0     9223 2023-04-27 03:17:24.000000 RStockvn-2.1.81/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 03:36:43.757636 RStockvn-2.1.81/RStockvn/
+-rw-rw-rw-   0        0        0      833 2023-05-28 03:34:29.000000 RStockvn-2.1.81/RStockvn/__init__.py
+-rw-rw-rw-   0        0        0     2726 2023-05-28 03:34:16.000000 RStockvn-2.1.81/RStockvn/cafef_test.py
+-rw-rw-rw-   0        0        0     6344 2023-03-01 05:00:59.000000 RStockvn-2.1.81/RStockvn/data_cafef.py
+-rw-rw-rw-   0        0        0    19726 2023-03-01 05:09:24.000000 RStockvn-2.1.81/RStockvn/stockvn.py
+-rw-rw-rw-   0        0        0   139694 2023-02-06 06:33:27.000000 RStockvn-2.1.81/RStockvn/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-05-28 03:36:43.804501 RStockvn-2.1.81/RStockvn.egg-info/
+-rw-rw-rw-   0        0        0    10092 2023-05-28 03:36:43.000000 RStockvn-2.1.81/RStockvn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2023-05-28 03:36:43.000000 RStockvn-2.1.81/RStockvn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 03:36:43.000000 RStockvn-2.1.81/RStockvn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-28 03:36:43.000000 RStockvn-2.1.81/RStockvn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 03:36:43.000000 RStockvn-2.1.81/RStockvn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 03:36:43.804501 RStockvn-2.1.81/setup.cfg
+-rw-rw-rw-   0        0        0     1216 2023-05-28 03:35:20.000000 RStockvn-2.1.81/setup.py
```

### Comparing `RStockvn-2.1.8/LICENSE` & `RStockvn-2.1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.8/PKG-INFO` & `RStockvn-2.1.81/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,195 +1,189 @@
-Metadata-Version: 2.1
-Name: RStockvn
-Version: 2.1.8
-Summary: Report Finance of Companies in Vietnamese and macro data - Lấy báo cáo tài chính của các công ty ở Việt Nam và số liệu vĩ mô
-Home-page: https://github.com/NPhucBinh/RStockvn
-Author: NGUYEN PHUC BINH
-Author-email: nguyenphucbinh67@gmail.com
-Keywords: RStockvn,rpv,rstockvn,report stock vn,báo cáo tài chính việt nam,lấy báo cáo tài chính việt nam bằng python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# [RStockvn](https://pypi.org/project/RStockvn/)
-Financial statements of companies on the Vietnamese stock exchange
-
-
-# Introduce
-Hi, my name is Nguyen Phuc Binh.
-The reason that I do [RStockvn](https://pypi.org/project/RStockvn/) is to support the collection of basic data for analysis.
-
-The financial statements that RStockvn collects mainly come from websites: [Cổ phiếu 68](https://www.cophieu68.vn), [Cafef](https://cafef.vn).
-
-For the exchange rate, RStockvn collects at ["exchangerate.host"](https://exchangerate.host/#/donate) if you have more interest or support for their project you can visit at:[Exchangerate](https://exchangerate.host/#/donate)
-### From update 1.0.3 onwards, you can used rstockvn to get macro data.
-The figures CPI, FDI, GDP, ... are taken from websites: [Vietstock](https://finance.vietstock.vn/du-lieu-vi-mo)
-
-If you are on the old version and have errors, please update to the new version of RStockvn by: ``pip install --upgrade RStockvn``
-
-Also you can refer to the library:'vnstock', written by Mr. Thinh Vu
-# User guide
-First you need to install RStockvn by:
-``pip install RStockvn`` or ``conda install RStockvn``
-To use you need to: ``import RStockvn as rpv`` or ``from RStockvn import *``
-
-## 1.Function to view stock adjusted price history
-This function will return the adjusted price history of the ticker, from dividend events.
-``
-event_price_cp68(symbol)
-``
-```
-rpv.event_price_cp68('HSG')
-```
-## 2.Function retrieves financial statements of stock tickers from websites: 'Cophieu68.vn'
-To use this function you need to do the following:
-``report_finance_cp68(symbol,reporty,timely)``
-
-Here `symbol` is stock ticker, reporty corresponds to the following options: ``'CDKT' - BalanceSheet``,``'KQKD' - Business results``.And `timely` corresponds to the choice: `'Year' - year` or `'quy' - quarter.`
-#### Example
-```
-rpv.report_finance_cp68('ACB','cdkt','quy')
-```
-
-## 3.Function retrieves financial statements of stock tickers from websites: 'Cafef.vn'
-``report_finance_cf(symbol,report,year,timely)``
-This function is similar to x except with some differences:
-'report' will have the following options: `'CDKT' - BalanceSheet`, `'KQKD' - Business results`, `'CFD' - Direct Cash Flows`, `'CF' - Indirect Cash Flows`. `year` corresponds to the reporting datum you want to get. And `timely` corresponds to the choice: `'Year' - year` or `'quy' - quarter.`
-#### Example
-```
-rpv.report_finance_cf('nkg','cfd','2022','year')
-```
-
-## 4.Function used to view company information
-``info_company(symbol)``
-#### Example
-```
-rpv.info_company('HSG')
-```
-## 5.View insider trading transactions
-``trade_internal(symbol)``
-#### Example
-```
-rpv.trade_internal('ACB')
-```
-## 6.View exchange rate change history
-At the present time when accessing "exchangerate.host" can only get the history of exchange rates within the last 9 months.``exchange_currency(current,cover_current,from_date,to_date)``
-#### Example
-```
-rpv.exchange_currency('USD','VND','2022-11-23','2023-01-10')
-```
-You can also convert other currencies, such as Japanese Yen and USD
-```
-rpv.exchange_currency('JPY','USD','2022-11-23','2023-01-10')
-```
-## 7.View a quick report on the profit, revenue, ... of a company
-For this report I use the financial statements collected from the website 'Cophieu68', because it is similar to the financial statements provided by securities companies such as VNDirect, SSI.``baocaonhanh(mcp,loai,time)``
-
-Here mcp corresponds to the ticker, 'type' corresponds to the following selection:
-``'TM' - Thương mại``
-For companies that manufacture, retail, basic materials, consumer goods,...
-``'TC' - Finance``
-For companies in the financial sector.
-
-Because companies in the financial sector are quite separate in nature.
-For example, the banking industry is an industry that uses capital to generate cash flow, so RStockvn currently does not provide a quick report template for these industriedsđ
-
-About this kind of report I will add later
-#### Example
-```
-rpv.baocaonhanh('HSG','TM','QUY')
-```
-
-## 8.Get historical interest rate data (Vietnam)
-To get the interest rate data you need to use the function ``laisuat_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.laisuat_vietstock('2022-10-12','2023-02-01')
-```
-## 9.Get data for CPI (Vietnam)
-To get data for CPI you need to use the function ``getCPI_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.getCPI_vietstock('2022-10-01','2023-02-01')
-```
-
-## 10.Get data on industrial production (Vietnam)
-To get data on industrial production you need to use the function ``solieu_sanxuat_congnghiep(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.solieu_sanxuat_congnghiep('2022-10-01','2023-02-01')
-```
-## 11.Get data on retail (Vietnam)
-To get data on retail you need to use the function ``solieu_banle_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.solieu_banle_vietstock('2022-10-01','2023-02-01')
-```
-
-## 12.Get data on import and export (Vietnam)
-To get data on import and export you need to use the function ``solieu_XNK_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.solieu_XNK_vietstock('2022-10-01','2023-02-01')
-```
-
-## 13.Get data on FDI capital (Vietnam)
-To get data on FDI capital you need to use the function ``solieu_FDI_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.solieu_FDI_vietstock('2022-10-01','2023-02-01')
-```
-
-## 14.Get data on the exchange rate of USD/VND
-To get data on the exchange rate of USD/VND you need to use the function ``tygia_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.tygia_vietstock('2022-10-01','2023-02-01')
-```
-
-## 15.Get data on credit in Vietnam
-To get data on credit in Vietnam you need to use the function ``solieu_tindung_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.solieu_tindung_vietstock('2022-10-01','2023-02-01')
-```
-
-## 16.Get data on population, unemployment rate (Vietnam)
-To get data on population, unemployment rate you need to use the function ``solieu_danso_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
-#### Example
-```
-rpv.solieu_danso_vietstock('2022-10-01','2023-02-01')
-```
-
-## 17.Get GDP index (Vietnam)
-To get the GDP index you need to use the ``solieu_GDP_vietstock(fromyear,fromQ,toyear,toQ)`` function. ``fromyear`` ``toyear`` are the year milestones to be taken, ``fromQ``, ``toQ`` is the quarters you choose.
-#### Example
-You want to get the GDP index from 2nd quarter 2020 to 3rd quarter 2022.
-```
-rpv.solieu_GDP_vietstock('2020','2','2022','3')
-```
-
-## 18.Get price historical data of CafeF
-To get historical stock price data from [CafeF](https://cafef.vn) websites you need to use the function ``get_data_history_cafef(symbol,fromdate,todate)``. ``symbol`` is the stock symbol you need to get data from, ``fromdate`` is the start date and ``todate`` is the end date.
-
-#### Example
-For example, you want to get the price history of VNINDEX from January 20, 2022 to February 20, 2023
-```
-rpv.get_data_history_cafef('VNINDEX','20/01/2022','20/02/2023')
-```
-OR you want to get the price history of symbol stock ``SSI`` from January 20, 2022 to February 20, 2023
-```
-rpv.get_data_history_cafef('SSI','20/01/2022','20/02/2023')
-```
-
-## Explore more:``historical_price_cp68(day,symbol)``
-The function looks at the price history of a stock code with the corresponding time of ``100``,``200``,``300``,``400``,``500`` and ``ALL``
-
-#### Example
-```
-rpv.historical_price_cp68(100,'HSG')
-```
-# Epilogue
-If you like the idea or want to add more suggestions about RStockvn. 
-Please send your comments to email: nguyenphucbinh67@gmail.com, thank you for testing RStockvn
+# [RStockvn](https://pypi.org/project/RStockvn/)
+Financial statements of companies on the Vietnamese stock exchange
+
+
+# Introduce
+Hi, my name is Nguyen Phuc Binh.
+The reason that I do [RStockvn](https://pypi.org/project/RStockvn/) is to support the collection of basic data for analysis.
+
+The financial statements that RStockvn collects mainly come from websites: [Cổ phiếu 68](https://www.cophieu68.vn), [Cafef](https://cafef.vn).
+
+For the exchange rate, RStockvn collects at ["exchangerate.host"](https://exchangerate.host/#/donate) if you have more interest or support for their project you can visit at:[Exchangerate](https://exchangerate.host/#/donate)
+### From update 1.0.3 onwards, you can used rstockvn to get macro data.
+The figures CPI, FDI, GDP, ... are taken from websites: [Vietstock](https://finance.vietstock.vn/du-lieu-vi-mo)
+
+If you are on the old version and have errors, please update to the new version of RStockvn by: ``pip install --upgrade RStockvn``
+
+Also you can refer to the library:'vnstock', written by Mr. Thinh Vu
+
+#Ghi chú: 
+Xin chào, tôi nhận được một số mail phản hồi từ một trong các website mà thư viện RStockvn đang thu thập thông tin. 
+Nội dung các mail đó nói về việc thông tin họ được sử dụng không phù hợp, vì vậy khi các bạn sử dụng thư viện này để lấy thông tin cho các bài tiểu luận, luận án, viết báo,...
+Vui lòng ghi rõ nguồn của thông tin mà bạn lấy, cảm ơn.
+~~~ Hãy tôn trọng chính chủ và tác giả ~~~
+Nếu có vấn đề hay cần chia sẻ ý kiến, vui lòng liên hệ qua mail: nguyenphucbinh67@gmail.com
+
+# User guide
+First you need to install RStockvn by:
+``pip install RStockvn`` or ``conda install RStockvn``
+To use you need to: ``import RStockvn as rpv`` or ``from RStockvn import *``
+
+## 1.Function to view stock adjusted price history
+This function will return the adjusted price history of the ticker, from dividend events.
+``
+event_price_cp68(symbol)
+``
+```
+rpv.event_price_cp68('HSG')
+```
+## 2.Function retrieves financial statements of stock tickers from websites: 'Cophieu68.vn'
+To use this function you need to do the following:
+``report_finance_cp68(symbol,reporty,timely)``
+
+Here `symbol` is stock ticker, reporty corresponds to the following options: ``'CDKT' - BalanceSheet``,``'KQKD' - Business results``.And `timely` corresponds to the choice: `'Year' - year` or `'quy' - quarter.`
+#### Example
+```
+rpv.report_finance_cp68('ACB','cdkt','quy')
+```
+
+## 3.Function retrieves financial statements of stock tickers from websites: 'Cafef.vn'
+``report_finance_cf(symbol,report,year,timely)``
+This function is similar to x except with some differences:
+'report' will have the following options: `'CDKT' - BalanceSheet`, `'KQKD' - Business results`, `'CFD' - Direct Cash Flows`, `'CF' - Indirect Cash Flows`. `year` corresponds to the reporting datum you want to get. And `timely` corresponds to the choice: `'Year' - year` or `'quy' - quarter.`
+#### Example
+```
+rpv.report_finance_cf('nkg','cfd','2022','year')
+```
+
+## 4.Function used to view company information
+``info_company(symbol)``
+#### Example
+```
+rpv.info_company('HSG')
+```
+## 5.View insider trading transactions
+``trade_internal(symbol)``
+#### Example
+```
+rpv.trade_internal('ACB')
+```
+## 6.View exchange rate change history
+At the present time when accessing "exchangerate.host" can only get the history of exchange rates within the last 9 months.``exchange_currency(current,cover_current,from_date,to_date)``
+#### Example
+```
+rpv.exchange_currency('USD','VND','2022-11-23','2023-01-10')
+```
+You can also convert other currencies, such as Japanese Yen and USD
+```
+rpv.exchange_currency('JPY','USD','2022-11-23','2023-01-10')
+```
+## 7.View a quick report on the profit, revenue, ... of a company
+For this report I use the financial statements collected from the website 'Cophieu68', because it is similar to the financial statements provided by securities companies such as VNDirect, SSI.``baocaonhanh(mcp,loai,time)``
+
+Here mcp corresponds to the ticker, 'type' corresponds to the following selection:
+``'TM' - Thương mại``
+For companies that manufacture, retail, basic materials, consumer goods,...
+``'TC' - Finance``
+For companies in the financial sector.
+
+Because companies in the financial sector are quite separate in nature.
+For example, the banking industry is an industry that uses capital to generate cash flow, so RStockvn currently does not provide a quick report template for these industriedsđ
+
+About this kind of report I will add later
+#### Example
+```
+rpv.baocaonhanh('HSG','TM','QUY')
+```
+
+## 8.Get historical interest rate data (Vietnam)
+To get the interest rate data you need to use the function ``laisuat_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.laisuat_vietstock('2022-10-12','2023-02-01')
+```
+## 9.Get data for CPI (Vietnam)
+To get data for CPI you need to use the function ``getCPI_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.getCPI_vietstock('2022-10-01','2023-02-01')
+```
+
+## 10.Get data on industrial production (Vietnam)
+To get data on industrial production you need to use the function ``solieu_sanxuat_congnghiep(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.solieu_sanxuat_congnghiep('2022-10-01','2023-02-01')
+```
+## 11.Get data on retail (Vietnam)
+To get data on retail you need to use the function ``solieu_banle_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.solieu_banle_vietstock('2022-10-01','2023-02-01')
+```
+
+## 12.Get data on import and export (Vietnam)
+To get data on import and export you need to use the function ``solieu_XNK_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.solieu_XNK_vietstock('2022-10-01','2023-02-01')
+```
+
+## 13.Get data on FDI capital (Vietnam)
+To get data on FDI capital you need to use the function ``solieu_FDI_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.solieu_FDI_vietstock('2022-10-01','2023-02-01')
+```
+
+## 14.Get data on the exchange rate of USD/VND
+To get data on the exchange rate of USD/VND you need to use the function ``tygia_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.tygia_vietstock('2022-10-01','2023-02-01')
+```
+
+## 15.Get data on credit in Vietnam
+To get data on credit in Vietnam you need to use the function ``solieu_tindung_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.solieu_tindung_vietstock('2022-10-01','2023-02-01')
+```
+
+## 16.Get data on population, unemployment rate (Vietnam)
+To get data on population, unemployment rate you need to use the function ``solieu_danso_vietstock(fromdate,todate)``, ``fromdate`` is from the date you need to get the ``todate`` to the date you want to get the data.
+#### Example
+```
+rpv.solieu_danso_vietstock('2022-10-01','2023-02-01')
+```
+
+## 17.Get GDP index (Vietnam)
+To get the GDP index you need to use the ``solieu_GDP_vietstock(fromyear,fromQ,toyear,toQ)`` function. ``fromyear`` ``toyear`` are the year milestones to be taken, ``fromQ``, ``toQ`` is the quarters you choose.
+#### Example
+You want to get the GDP index from 2nd quarter 2020 to 3rd quarter 2022.
+```
+rpv.solieu_GDP_vietstock('2020','2','2022','3')
+```
+
+## 18.Get price historical data of CafeF
+To get historical stock price data from [CafeF](https://cafef.vn) websites you need to use the function ``get_data_history_cafef(symbol,fromdate,todate)``. ``symbol`` is the stock symbol you need to get data from, ``fromdate`` is the start date and ``todate`` is the end date.
+
+#### Example
+For example, you want to get the price history of VNINDEX from January 20, 2022 to February 20, 2023
+```
+rpv.get_data_history_cafef('VNINDEX','20/01/2022','20/02/2023')
+```
+OR you want to get the price history of symbol stock ``SSI`` from January 20, 2022 to February 20, 2023
+```
+rpv.get_data_history_cafef('SSI','20/01/2022','20/02/2023')
+```
+
+## Explore more:``historical_price_cp68(day,symbol)``
+The function looks at the price history of a stock code with the corresponding time of ``100``,``200``,``300``,``400``,``500`` and ``ALL``
+
+#### Example
+```
+rpv.historical_price_cp68(100,'HSG')
+```
+# Epilogue
+If you like the idea or want to add more suggestions about RStockvn. 
+Please send your comments to email: nguyenphucbinh67@gmail.com, thank you for testing RStockvn
```

### Comparing `RStockvn-2.1.8/RStockvn/__init__.py` & `RStockvn-2.1.81/RStockvn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2023 Nguyen Phuc Binh @ GitHub
 # See LICENSE for details.
-__version__ = "2.1.6"
+__version__ = "2.1.8"
 __author__ ="Nguyen Phuc Binh"
 __copyright__ = "Copyright 2023, Nguyen Phuc Binh"
 __license__ = "MIT"
 __email__ = "nguyenphucbinh67@gmail.com"
 __website__ = "https://github.com/NPhucBinh"
 
 from . import user_agent
```

### Comparing `RStockvn-2.1.8/RStockvn/cafef_test.py` & `RStockvn-2.1.81/RStockvn/cafef_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 self.lis.append(df)
             except:
                 df=self.dataframe()
                 self.lis.append(df)
                 break
         data=pd.concat(self.lis)
         data.drop(['Thay đổi (+/-%).1'],axis=1,inplace=True)
-        data.rename(columns={'KL':'KLGD khớp lệnh','GT':'GTGD khớp lệnh','KL.1':'KLGD thỏa thuận','GT.1':'GTGD thỏa thuận'}, inplace=True)
+        data.rename(columns={'GD khớp lệnh':'KLGD khớp lệnh','GD khớp lệnh.1':'GTGD khớp lệnh','GD thỏa thuận':'KLGD thỏa thuận','GD thỏa thuận.1':'GTGD thỏa thuận'}, inplace=True)
         self.close()
         return data.reset_index(drop=True)
     
     def dataframe(self):
         import pandas as pd
         df=pd.read_html(self.br.page_source,encoding='utf-8',header=0)
         data=pd.DataFrame(df[2])
```

### Comparing `RStockvn-2.1.8/RStockvn/data_cafef.py` & `RStockvn-2.1.81/RStockvn/data_cafef.py`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.8/RStockvn/stockvn.py` & `RStockvn-2.1.81/RStockvn/stockvn.py`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.8/RStockvn/user_agent.py` & `RStockvn-2.1.81/RStockvn/user_agent.py`

 * *Files identical despite different names*

### Comparing `RStockvn-2.1.8/RStockvn.egg-info/PKG-INFO` & `RStockvn-2.1.81/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RStockvn
-Version: 2.1.8
+Version: 2.1.81
 Summary: Report Finance of Companies in Vietnamese and macro data - Lấy báo cáo tài chính của các công ty ở Việt Nam và số liệu vĩ mô
 Home-page: https://github.com/NPhucBinh/RStockvn
 Author: NGUYEN PHUC BINH
 Author-email: nguyenphucbinh67@gmail.com
 Keywords: RStockvn,rpv,rstockvn,report stock vn,báo cáo tài chính việt nam,lấy báo cáo tài chính việt nam bằng python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +25,22 @@
 For the exchange rate, RStockvn collects at ["exchangerate.host"](https://exchangerate.host/#/donate) if you have more interest or support for their project you can visit at:[Exchangerate](https://exchangerate.host/#/donate)
 ### From update 1.0.3 onwards, you can used rstockvn to get macro data.
 The figures CPI, FDI, GDP, ... are taken from websites: [Vietstock](https://finance.vietstock.vn/du-lieu-vi-mo)
 
 If you are on the old version and have errors, please update to the new version of RStockvn by: ``pip install --upgrade RStockvn``
 
 Also you can refer to the library:'vnstock', written by Mr. Thinh Vu
+
+#Ghi chú: 
+Xin chào, tôi nhận được một số mail phản hồi từ một trong các website mà thư viện RStockvn đang thu thập thông tin. 
+Nội dung các mail đó nói về việc thông tin họ được sử dụng không phù hợp, vì vậy khi các bạn sử dụng thư viện này để lấy thông tin cho các bài tiểu luận, luận án, viết báo,...
+Vui lòng ghi rõ nguồn của thông tin mà bạn lấy, cảm ơn.
+~~~ Hãy tôn trọng chính chủ và tác giả ~~~
+Nếu có vấn đề hay cần chia sẻ ý kiến, vui lòng liên hệ qua mail: nguyenphucbinh67@gmail.com
+
 # User guide
 First you need to install RStockvn by:
 ``pip install RStockvn`` or ``conda install RStockvn``
 To use you need to: ``import RStockvn as rpv`` or ``from RStockvn import *``
 
 ## 1.Function to view stock adjusted price history
 This function will return the adjusted price history of the ticker, from dividend events.
```

### Comparing `RStockvn-2.1.8/setup.py` & `RStockvn-2.1.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fh.read()
 
 DS = 'Report Finance of Companies in Vietnamese and macro data - Lấy báo cáo tài chính của các công ty ở Việt Nam và số liệu vĩ mô'
 
 #Setting
 setup(
     name='RStockvn',
-    version='2.1.8',
+    version='2.1.81',
     author='NGUYEN PHUC BINH',
     author_email='nguyenphucbinh67@gmail.com',
     description=DS,
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     url="https://github.com/NPhucBinh/RStockvn",
```

