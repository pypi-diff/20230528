# Comparing `tmp/py_pdf_term-1.0.0.tar.gz` & `tmp/py_pdf_term-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_pdf_term-1.0.0.tar", max compression
+gzip compressed data, was "py_pdf_term-1.0.2.tar", max compression
```

## Comparing `py_pdf_term-1.0.0.tar` & `py_pdf_term-1.0.2.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0     1065 2021-08-01 13:41:41.018921 py_pdf_term-1.0.0/LICENSE
--rw-r--r--   0        0        0      558 2023-04-22 03:34:12.853470 py_pdf_term-1.0.0/README.md
--rw-r--r--   0        0        0      325 2023-05-21 11:41:58.441154 py_pdf_term-1.0.0/py_pdf_term/__init__.py
--rw-r--r--   0        0        0        0 2021-07-17 01:56:39.528684 py_pdf_term-1.0.0/py_pdf_term/_common/__init__.py
--rw-r--r--   0        0        0     2445 2023-04-30 07:57:40.302941 py_pdf_term-1.0.0/py_pdf_term/_common/consts.py
--rw-r--r--   0        0        0      377 2023-05-07 09:38:40.927900 py_pdf_term-1.0.0/py_pdf_term/_common/data.py
--rw-r--r--   0        0        0      279 2023-05-07 09:38:40.928433 py_pdf_term-1.0.0/py_pdf_term/_common/utils.py
--rw-r--r--   0        0        0       89 2023-04-23 12:35:30.854867 py_pdf_term-1.0.0/py_pdf_term/analysis/__init__.py
--rw-r--r--   0        0        0      442 2023-05-21 10:48:35.970334 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/__init__.py
--rw-r--r--   0        0        0      168 2023-05-21 10:48:35.871081 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/concats/__init__.py
--rw-r--r--   0        0        0     4037 2023-05-07 09:38:40.929139 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/concats/lr.py
--rw-r--r--   0        0        0      151 2023-05-21 10:48:35.871055 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/cooccurrences/__init__.py
--rw-r--r--   0        0        0     3188 2023-05-07 09:38:40.930038 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/cooccurrences/container.py
--rw-r--r--   0        0        0      146 2023-05-21 10:48:35.888277 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/occurrences/__init__.py
--rw-r--r--   0        0        0     3682 2023-05-07 09:38:40.930653 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/occurrences/term.py
--rw-r--r--   0        0        0     2210 2023-05-07 09:38:40.931460 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/runner.py
--rw-r--r--   0        0        0       92 2023-04-23 12:35:30.855657 py_pdf_term-1.0.0/py_pdf_term/candidates/__init__.py
--rw-r--r--   0        0        0      287 2023-05-21 10:48:35.963075 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/__init__.py
--rw-r--r--   0        0        0      315 2023-05-21 10:48:35.923659 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/__init__.py
--rw-r--r--   0        0        0      993 2023-05-07 09:38:40.932281 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/base.py
--rw-r--r--   0        0        0     1451 2023-05-07 09:38:40.933258 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/combiner.py
--rw-r--r--   0        0        0     3499 2023-05-07 09:38:40.934024 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/separation.py
--rw-r--r--   0        0        0      315 2023-05-21 10:48:35.928200 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/__init__.py
--rw-r--r--   0        0        0     3446 2023-05-01 10:52:18.632436 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/base.py
--rw-r--r--   0        0        0      585 2023-05-01 10:52:18.633202 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/english.py
--rw-r--r--   0        0        0      622 2023-05-01 10:52:18.633951 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/japanese.py
--rw-r--r--   0        0        0     1418 2023-05-07 09:38:40.934955 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/marker.py
--rw-r--r--   0        0        0     4479 2023-05-07 09:38:40.936309 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/data.py
--rw-r--r--   0        0        0     8826 2023-05-07 09:38:40.936924 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/extractor.py
--rw-r--r--   0        0        0      985 2023-05-21 10:48:35.957866 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/__init__.py
--rw-r--r--   0        0        0     3422 2023-05-07 09:38:40.938498 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/combiner.py
--rw-r--r--   0        0        0      816 2023-05-21 10:48:35.959032 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/__init__.py
--rw-r--r--   0        0        0     1844 2023-05-07 09:38:40.940803 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/base.py
--rw-r--r--   0        0        0      192 2023-05-21 10:48:36.026802 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/__init__.py
--rw-r--r--   0        0        0     3749 2023-05-07 09:38:40.941707 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py
--rw-r--r--   0        0        0     5446 2023-05-07 09:38:40.942264 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py
--rw-r--r--   0        0        0      168 2023-05-21 10:48:35.977851 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/__init__.py
--rw-r--r--   0        0        0      763 2023-05-07 09:38:40.943040 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py
--rw-r--r--   0        0        0     1142 2023-05-07 09:38:40.943767 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py
--rw-r--r--   0        0        0      180 2023-05-21 10:48:35.985218 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/__init__.py
--rw-r--r--   0        0        0      355 2023-05-07 09:38:40.944518 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/english.py
--rw-r--r--   0        0        0     1053 2023-05-07 09:38:40.945146 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py
--rw-r--r--   0        0        0      180 2023-05-21 10:48:35.994920 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/__init__.py
--rw-r--r--   0        0        0     2254 2023-05-07 09:38:40.945849 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py
--rw-r--r--   0        0        0     2357 2023-05-07 09:38:40.946502 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py
--rw-r--r--   0        0        0      231 2023-05-21 10:48:36.028806 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/__init__.py
--rw-r--r--   0        0        0     1250 2023-05-01 10:52:18.644721 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/base.py
--rw-r--r--   0        0        0     1821 2023-05-01 10:52:18.645564 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/english.py
--rw-r--r--   0        0        0     2956 2023-05-01 10:52:18.646465 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/japanese.py
--rw-r--r--   0        0        0      254 2023-05-21 10:48:36.025521 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/__init__.py
--rw-r--r--   0        0        0     1793 2023-05-07 09:38:40.947207 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/base.py
--rw-r--r--   0        0        0     1235 2023-05-07 09:38:40.947993 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/combiner.py
--rw-r--r--   0        0        0     3013 2023-05-07 09:38:40.949139 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/repeat.py
--rw-r--r--   0        0        0     1474 2023-05-07 09:38:40.950192 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/symname.py
--rw-r--r--   0        0        0     1579 2023-05-01 09:56:20.542921 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/utils.py
--rw-r--r--   0        0        0      115 2023-04-23 12:35:30.856299 py_pdf_term-1.0.0/py_pdf_term/candidates/augmenters.py
--rw-r--r--   0        0        0      117 2023-04-23 12:35:30.857009 py_pdf_term-1.0.0/py_pdf_term/candidates/classifiers.py
--rw-r--r--   0        0        0      109 2023-04-23 12:35:30.858941 py_pdf_term-1.0.0/py_pdf_term/candidates/filters.py
--rw-r--r--   0        0        0      113 2023-04-23 12:35:30.859936 py_pdf_term-1.0.0/py_pdf_term/candidates/splitters.py
--rw-r--r--   0        0        0      430 2023-05-21 10:48:36.041965 py_pdf_term-1.0.0/py_pdf_term/configs.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.860623 py_pdf_term-1.0.0/py_pdf_term/endtoend/__init__.py
--rw-r--r--   0        0        0      333 2023-05-21 10:48:36.055901 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/__init__.py
--rw-r--r--   0        0        0     1024 2023-05-21 10:48:36.093130 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/__init__.py
--rw-r--r--   0        0        0      254 2023-05-21 10:48:36.054361 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/__init__.py
--rw-r--r--   0        0        0     2245 2023-05-01 10:52:18.650657 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py
--rw-r--r--   0        0        0     2388 2023-05-07 09:38:40.950934 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py
--rw-r--r--   0        0        0      788 2023-05-01 10:52:18.652062 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py
--rw-r--r--   0        0        0      184 2023-04-30 03:53:53.377462 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/consts.py
--rw-r--r--   0        0        0      448 2023-05-21 10:48:36.076321 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/__init__.py
--rw-r--r--   0        0        0     6005 2023-05-01 10:52:18.652631 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/base.py
--rw-r--r--   0        0        0     4896 2023-05-07 09:38:40.951642 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/file.py
--rw-r--r--   0        0        0     1777 2023-05-01 10:52:18.653880 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py
--rw-r--r--   0        0        0      227 2023-05-21 10:48:36.069449 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/__init__.py
--rw-r--r--   0        0        0     2222 2023-05-01 10:52:18.654501 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/base.py
--rw-r--r--   0        0        0     2377 2023-05-07 09:38:40.952425 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/file.py
--rw-r--r--   0        0        0      770 2023-05-01 10:52:18.655623 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py
--rw-r--r--   0        0        0      702 2021-07-17 01:56:39.549058 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/util.py
--rw-r--r--   0        0        0      203 2023-05-21 10:48:36.064385 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/__init__.py
--rw-r--r--   0        0        0     2122 2023-05-01 10:52:18.656159 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/base.py
--rw-r--r--   0        0        0     2348 2023-05-03 08:07:06.640739 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/file.py
--rw-r--r--   0        0        0      701 2023-05-01 10:52:18.657277 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py
--rw-r--r--   0        0        0      586 2023-05-21 10:48:36.206572 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/__init__.py
--rw-r--r--   0        0        0      707 2023-05-01 10:52:18.658128 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/base.py
--rw-r--r--   0        0        0     3264 2023-05-01 10:52:18.659057 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/candidate.py
--rw-r--r--   0        0        0     1821 2023-05-01 10:52:18.659640 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/method.py
--rw-r--r--   0        0        0      743 2023-05-01 10:52:18.660263 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/styling.py
--rw-r--r--   0        0        0      752 2023-05-01 10:52:18.660806 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/techterm.py
--rw-r--r--   0        0        0     1005 2023-05-01 10:52:18.662558 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/xml.py
--rw-r--r--   0        0        0      635 2023-05-21 09:40:45.033904 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/data.py
--rw-r--r--   0        0        0    18045 2023-05-21 09:40:45.035210 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/extractor.py
--rw-r--r--   0        0        0      480 2023-05-21 10:48:36.091002 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/__init__.py
--rw-r--r--   0        0        0     6156 2023-05-21 09:44:19.458264 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/candidate.py
--rw-r--r--   0        0        0     9788 2023-05-21 09:44:19.459767 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/method.py
--rw-r--r--   0        0        0     2832 2023-05-21 09:44:19.461295 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/styling.py
--rw-r--r--   0        0        0     5405 2023-05-01 10:52:18.667346 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/techterm.py
--rw-r--r--   0        0        0     2700 2023-05-21 09:44:19.462264 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/xml.py
--rw-r--r--   0        0        0     1077 2023-05-21 10:48:36.178877 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/__init__.py
--rw-r--r--   0        0        0     2925 2023-05-21 09:44:19.463517 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/base.py
--rw-r--r--   0        0        0      407 2023-05-21 10:48:36.215373 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/__init__.py
--rw-r--r--   0        0        0      687 2023-05-21 09:44:19.464771 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py
--rw-r--r--   0        0        0     1392 2023-05-21 09:44:19.466267 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py
--rw-r--r--   0        0        0      652 2023-05-21 09:44:19.467168 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py
--rw-r--r--   0        0        0      616 2023-05-21 09:44:19.468834 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py
--rw-r--r--   0        0        0      446 2023-05-21 10:48:36.239199 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/__init__.py
--rw-r--r--   0        0        0      774 2023-05-21 09:44:19.469622 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py
--rw-r--r--   0        0        0      783 2023-05-21 09:44:19.470490 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py
--rw-r--r--   0        0        0     1727 2023-05-21 09:44:19.471360 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py
--rw-r--r--   0        0        0      742 2023-05-21 09:44:19.472913 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py
--rw-r--r--   0        0        0      644 2023-05-21 09:44:19.473977 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py
--rw-r--r--   0        0        0      204 2023-05-21 10:48:36.187774 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/__init__.py
--rw-r--r--   0        0        0      691 2023-05-21 09:44:19.476084 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py
--rw-r--r--   0        0        0      775 2023-05-21 09:44:19.478488 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py
--rw-r--r--   0        0        0       97 2023-05-21 10:48:36.192351 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/__init__.py
--rw-r--r--   0        0        0      654 2023-05-21 09:44:19.479440 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/binopener.py
--rw-r--r--   0        0        0       93 2023-05-21 10:48:36.200466 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/__init__.py
--rw-r--r--   0        0        0      680 2023-05-21 09:44:19.481386 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py
--rw-r--r--   0        0        0      102 2023-04-23 12:35:30.862807 py_pdf_term-1.0.0/py_pdf_term/endtoend/caches.py
--rw-r--r--   0        0        0      976 2023-05-21 10:48:36.271106 py_pdf_term-1.0.0/py_pdf_term/mappers.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.863506 py_pdf_term-1.0.0/py_pdf_term/methods/__init__.py
--rw-r--r--   0        0        0      536 2023-05-21 10:48:36.254137 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/__init__.py
--rw-r--r--   0        0        0     8534 2023-05-01 10:52:18.677653 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/base.py
--rw-r--r--   0        0        0      567 2023-05-21 10:48:36.245483 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/__init__.py
--rw-r--r--   0        0        0      983 2023-05-01 10:52:18.678289 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/base.py
--rw-r--r--   0        0        0     1000 2023-05-01 10:52:18.678854 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flr.py
--rw-r--r--   0        0        0     1006 2023-05-01 10:52:18.679428 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flrh.py
--rw-r--r--   0        0        0     1006 2023-05-01 10:52:18.679998 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/hits.py
--rw-r--r--   0        0        0     1010 2023-05-01 10:52:18.680523 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/mcvalue.py
--rw-r--r--   0        0        0      740 2023-05-01 10:52:18.681051 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/mdp.py
--rw-r--r--   0        0        0      893 2023-05-01 10:52:18.681650 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/tfidf.py
--rw-r--r--   0        0        0      936 2023-05-02 07:56:39.552792 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/data.py
--rw-r--r--   0        0        0      591 2023-05-01 10:52:18.682880 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flr.py
--rw-r--r--   0        0        0      951 2023-05-01 10:52:18.683430 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flrh.py
--rw-r--r--   0        0        0     1186 2023-05-21 07:39:18.389207 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/hits.py
--rw-r--r--   0        0        0      632 2023-05-01 10:52:18.684461 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/mcvalue.py
--rw-r--r--   0        0        0      589 2023-05-21 10:54:59.338573 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/mdp.py
--rw-r--r--   0        0        0      447 2023-05-21 10:48:36.254929 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/__init__.py
--rw-r--r--   0        0        0     2101 2023-05-01 10:52:18.685791 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/base.py
--rw-r--r--   0        0        0     2029 2023-05-07 09:38:40.961943 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flr.py
--rw-r--r--   0        0        0     2853 2023-05-07 09:38:40.962849 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flrh.py
--rw-r--r--   0        0        0     6342 2023-05-21 09:40:45.036164 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/hits.py
--rw-r--r--   0        0        0     1968 2023-05-07 09:38:40.967316 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/mcvalue.py
--rw-r--r--   0        0        0     3171 2023-05-21 10:54:59.339804 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/mdp.py
--rw-r--r--   0        0        0     2009 2023-05-21 10:54:59.340978 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/tfidf.py
--rw-r--r--   0        0        0      473 2023-05-21 10:48:36.275731 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/__init__.py
--rw-r--r--   0        0        0      561 2023-05-01 10:52:18.689999 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/base.py
--rw-r--r--   0        0        0      970 2023-05-01 10:52:18.690868 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/flr.py
--rw-r--r--   0        0        0      972 2023-05-01 10:52:18.691383 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/flrh.py
--rw-r--r--   0        0        0      972 2023-05-01 10:52:18.691953 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/hits.py
--rw-r--r--   0        0        0     1440 2023-05-01 10:52:18.692557 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/mcvalue.py
--rw-r--r--   0        0        0     1189 2023-05-21 09:40:45.038339 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/mdp.py
--rw-r--r--   0        0        0      860 2023-05-01 10:52:18.693606 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/tfidf.py
--rw-r--r--   0        0        0      610 2023-05-21 10:54:59.341988 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/tfidf.py
--rw-r--r--   0        0        0      110 2023-04-23 12:35:30.865641 py_pdf_term-1.0.0/py_pdf_term/methods/collectors.py
--rw-r--r--   0        0        0      104 2023-04-23 12:35:30.866294 py_pdf_term-1.0.0/py_pdf_term/methods/rankers.py
--rw-r--r--   0        0        0      112 2023-04-23 12:35:30.866995 py_pdf_term-1.0.0/py_pdf_term/methods/rankingdata.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.867710 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/__init__.py
--rw-r--r--   0        0        0      174 2023-05-21 10:48:36.260616 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/__init__.py
--rw-r--r--   0        0        0      155 2023-05-21 10:48:36.285807 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/__init__.py
--rw-r--r--   0        0        0      577 2023-05-01 10:52:18.694863 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py
--rw-r--r--   0        0        0      369 2023-05-01 10:52:18.695436 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/standard.py
--rw-r--r--   0        0        0     4111 2023-05-01 10:52:18.695967 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/converter.py
--rw-r--r--   0        0        0     1421 2023-05-07 09:38:40.970029 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/data.py
--rw-r--r--   0        0        0     6064 2023-05-01 10:52:18.697047 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/textful.py
--rw-r--r--   0        0        0      871 2021-12-23 08:24:58.272396 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/utils.py
--rw-r--r--   0        0        0      111 2023-04-30 07:57:40.332098 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/binopeners.py
--rw-r--r--   0        0        0       88 2023-04-23 12:35:30.870578 py_pdf_term-1.0.0/py_pdf_term/stylings/__init__.py
--rw-r--r--   0        0        0      260 2023-05-21 10:48:36.286348 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/__init__.py
--rw-r--r--   0        0        0     2487 2023-05-02 07:56:40.346196 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/data.py
--rw-r--r--   0        0        0     3474 2023-05-02 07:56:40.422973 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scorer.py
--rw-r--r--   0        0        0      185 2023-05-21 10:48:36.278288 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/__init__.py
--rw-r--r--   0        0        0     1215 2023-05-07 09:38:40.970711 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/base.py
--rw-r--r--   0        0        0     1212 2023-05-07 09:38:40.971530 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/color.py
--rw-r--r--   0        0        0     1512 2023-05-07 09:38:40.972047 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/fontsize.py
--rw-r--r--   0        0        0      102 2023-04-23 12:35:30.871198 py_pdf_term-1.0.0/py_pdf_term/stylings/scores.py
--rw-r--r--   0        0        0       91 2023-04-23 12:35:30.872290 py_pdf_term-1.0.0/py_pdf_term/techterms/__init__.py
--rw-r--r--   0        0        0      287 2023-05-21 10:48:36.292986 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/__init__.py
--rw-r--r--   0        0        0     2415 2023-05-02 07:56:40.104927 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/data.py
--rw-r--r--   0        0        0     6115 2023-05-21 09:40:45.039682 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/extractor.py
--rw-r--r--   0        0        0      494 2023-05-21 09:40:45.040935 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/utils.py
--rw-r--r--   0        0        0       92 2023-04-30 07:57:40.332522 py_pdf_term-1.0.0/py_pdf_term/tokenizers/__init__.py
--rw-r--r--   0        0        0      337 2023-05-21 10:48:36.294274 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/__init__.py
--rw-r--r--   0        0        0     1512 2023-05-07 09:38:40.975403 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/base.py
--rw-r--r--   0        0        0     2560 2023-05-07 09:38:40.976423 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/data.py
--rw-r--r--   0        0        0     1425 2023-05-07 09:38:40.977066 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/english.py
--rw-r--r--   0        0        0     2854 2023-05-07 09:38:40.977733 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/japanese.py
--rw-r--r--   0        0        0     1396 2023-05-01 10:52:18.703945 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/tokenizer.py
--rw-r--r--   0        0        0     1185 2023-05-21 11:41:58.442912 py_pdf_term-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 py_pdf_term-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-08-01 13:41:41.018921 py_pdf_term-1.0.2/LICENSE
+-rw-r--r--   0        0        0      558 2023-04-22 03:34:12.853470 py_pdf_term-1.0.2/README.md
+-rw-r--r--   0        0        0      325 2023-05-28 07:03:53.593903 py_pdf_term-1.0.2/py_pdf_term/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-17 01:56:39.528684 py_pdf_term-1.0.2/py_pdf_term/_common/__init__.py
+-rw-r--r--   0        0        0     2445 2023-04-30 07:57:40.302941 py_pdf_term-1.0.2/py_pdf_term/_common/consts.py
+-rw-r--r--   0        0        0      371 2023-05-28 06:39:10.015087 py_pdf_term-1.0.2/py_pdf_term/_common/data.py
+-rw-r--r--   0        0        0      279 2023-05-07 09:38:40.928433 py_pdf_term-1.0.2/py_pdf_term/_common/utils.py
+-rw-r--r--   0        0        0       89 2023-04-23 12:35:30.854867 py_pdf_term-1.0.2/py_pdf_term/analysis/__init__.py
+-rw-r--r--   0        0        0      442 2023-05-21 10:48:35.970334 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-21 10:48:35.871081 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/concats/__init__.py
+-rw-r--r--   0        0        0     4013 2023-05-28 06:39:10.015976 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/concats/lr.py
+-rw-r--r--   0        0        0      151 2023-05-21 10:48:35.871055 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/cooccurrences/__init__.py
+-rw-r--r--   0        0        0     3159 2023-05-28 06:39:10.017254 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/cooccurrences/container.py
+-rw-r--r--   0        0        0      146 2023-05-21 10:48:35.888277 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/occurrences/__init__.py
+-rw-r--r--   0        0        0     3653 2023-05-28 06:39:10.017958 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/occurrences/term.py
+-rw-r--r--   0        0        0     2210 2023-05-07 09:38:40.931460 py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/runner.py
+-rw-r--r--   0        0        0       92 2023-04-23 12:35:30.855657 py_pdf_term-1.0.2/py_pdf_term/candidates/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-21 10:48:35.963075 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-21 10:48:35.923659 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/__init__.py
+-rw-r--r--   0        0        0      965 2023-05-28 06:39:10.018630 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/base.py
+-rw-r--r--   0        0        0     1405 2023-05-28 06:39:10.019389 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/combiner.py
+-rw-r--r--   0        0        0     3479 2023-05-28 06:39:10.019839 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/separation.py
+-rw-r--r--   0        0        0      315 2023-05-21 10:48:35.928200 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/__init__.py
+-rw-r--r--   0        0        0     3433 2023-05-28 06:39:10.020224 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/base.py
+-rw-r--r--   0        0        0      583 2023-05-28 06:39:10.020907 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/english.py
+-rw-r--r--   0        0        0      620 2023-05-28 06:39:10.021358 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/japanese.py
+-rw-r--r--   0        0        0     1370 2023-05-28 06:39:10.022872 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/marker.py
+-rw-r--r--   0        0        0     4462 2023-05-28 06:39:10.024023 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/data.py
+-rw-r--r--   0        0        0     8744 2023-05-28 06:39:10.024603 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/extractor.py
+-rw-r--r--   0        0        0      985 2023-05-21 10:48:35.957866 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/__init__.py
+-rw-r--r--   0        0        0     3368 2023-05-28 06:39:10.025867 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/combiner.py
+-rw-r--r--   0        0        0      816 2023-05-21 10:48:35.959032 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/__init__.py
+-rw-r--r--   0        0        0     1840 2023-05-28 06:39:10.026666 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/base.py
+-rw-r--r--   0        0        0      192 2023-05-21 10:48:36.026802 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/__init__.py
+-rw-r--r--   0        0        0     3747 2023-05-28 06:39:10.027407 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py
+-rw-r--r--   0        0        0     5444 2023-05-28 06:39:10.027800 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py
+-rw-r--r--   0        0        0      168 2023-05-21 10:48:35.977851 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-28 06:39:10.028185 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py
+-rw-r--r--   0        0        0     1140 2023-05-28 06:39:10.028662 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py
+-rw-r--r--   0        0        0      180 2023-05-21 10:48:35.985218 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/__init__.py
+-rw-r--r--   0        0        0      353 2023-05-28 06:39:10.029476 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/english.py
+-rw-r--r--   0        0        0     1051 2023-05-28 06:39:10.030704 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py
+-rw-r--r--   0        0        0      180 2023-05-21 10:48:35.994920 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/__init__.py
+-rw-r--r--   0        0        0     2252 2023-05-28 06:39:10.031302 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py
+-rw-r--r--   0        0        0     2355 2023-05-28 06:39:10.031818 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py
+-rw-r--r--   0        0        0      231 2023-05-21 10:48:36.028806 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/__init__.py
+-rw-r--r--   0        0        0     1222 2023-05-28 06:39:10.032322 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/base.py
+-rw-r--r--   0        0        0     2006 2023-05-28 06:39:10.032986 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/english.py
+-rw-r--r--   0        0        0     2899 2023-05-28 06:39:10.033582 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/japanese.py
+-rw-r--r--   0        0        0      254 2023-05-21 10:48:36.025521 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/__init__.py
+-rw-r--r--   0        0        0     1751 2023-05-28 06:39:10.034019 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/base.py
+-rw-r--r--   0        0        0     1189 2023-05-28 06:39:10.034514 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/combiner.py
+-rw-r--r--   0        0        0     2964 2023-05-28 06:39:10.034987 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/repeat.py
+-rw-r--r--   0        0        0     1434 2023-05-28 06:39:10.035785 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/symname.py
+-rw-r--r--   0        0        0     1693 2023-05-28 06:39:10.036377 py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/utils.py
+-rw-r--r--   0        0        0      115 2023-04-23 12:35:30.856299 py_pdf_term-1.0.2/py_pdf_term/candidates/augmenters.py
+-rw-r--r--   0        0        0      117 2023-04-23 12:35:30.857009 py_pdf_term-1.0.2/py_pdf_term/candidates/classifiers.py
+-rw-r--r--   0        0        0      109 2023-04-23 12:35:30.858941 py_pdf_term-1.0.2/py_pdf_term/candidates/filters.py
+-rw-r--r--   0        0        0      113 2023-04-23 12:35:30.859936 py_pdf_term-1.0.2/py_pdf_term/candidates/splitters.py
+-rw-r--r--   0        0        0      430 2023-05-21 10:48:36.041965 py_pdf_term-1.0.2/py_pdf_term/configs.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.860623 py_pdf_term-1.0.2/py_pdf_term/endtoend/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-21 10:48:36.055901 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/__init__.py
+-rw-r--r--   0        0        0     1024 2023-05-21 10:48:36.093130 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/__init__.py
+-rw-r--r--   0        0        0      254 2023-05-21 10:48:36.054361 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/__init__.py
+-rw-r--r--   0        0        0     2176 2023-05-28 06:39:10.036961 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py
+-rw-r--r--   0        0        0     2351 2023-05-28 06:39:10.037466 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py
+-rw-r--r--   0        0        0      754 2023-05-28 06:39:10.038609 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py
+-rw-r--r--   0        0        0      184 2023-04-30 03:53:53.377462 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/consts.py
+-rw-r--r--   0        0        0      448 2023-05-21 10:48:36.076321 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/__init__.py
+-rw-r--r--   0        0        0     5886 2023-05-28 06:39:10.039426 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/base.py
+-rw-r--r--   0        0        0     4853 2023-05-28 06:39:10.040018 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/file.py
+-rw-r--r--   0        0        0     1742 2023-05-28 06:39:10.040618 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py
+-rw-r--r--   0        0        0      227 2023-05-21 10:48:36.069449 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/__init__.py
+-rw-r--r--   0        0        0     2153 2023-05-28 06:39:10.041172 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/base.py
+-rw-r--r--   0        0        0     2340 2023-05-28 06:39:10.041835 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/file.py
+-rw-r--r--   0        0        0      736 2023-05-28 06:39:10.042586 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py
+-rw-r--r--   0        0        0      678 2023-05-28 06:39:10.043501 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/util.py
+-rw-r--r--   0        0        0      203 2023-05-21 10:48:36.064385 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/__init__.py
+-rw-r--r--   0        0        0     2043 2023-05-28 06:39:10.045020 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/base.py
+-rw-r--r--   0        0        0     2299 2023-05-28 06:39:10.045547 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/file.py
+-rw-r--r--   0        0        0      655 2023-05-28 06:39:10.046204 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py
+-rw-r--r--   0        0        0      586 2023-05-21 10:48:36.206572 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-28 06:39:10.047362 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/base.py
+-rw-r--r--   0        0        0     3226 2023-05-28 06:39:10.048833 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/candidate.py
+-rw-r--r--   0        0        0     1803 2023-05-28 06:39:10.049262 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/method.py
+-rw-r--r--   0        0        0      715 2023-05-28 06:39:10.049650 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/styling.py
+-rw-r--r--   0        0        0      748 2023-05-28 06:39:10.050003 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/techterm.py
+-rw-r--r--   0        0        0      964 2023-05-28 06:39:10.050616 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/xml.py
+-rw-r--r--   0        0        0      611 2023-05-28 06:39:10.051234 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/data.py
+-rw-r--r--   0        0        0    17896 2023-05-28 06:39:10.053349 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/extractor.py
+-rw-r--r--   0        0        0      480 2023-05-21 10:48:36.091002 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/__init__.py
+-rw-r--r--   0        0        0     6065 2023-05-28 06:39:10.053907 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/candidate.py
+-rw-r--r--   0        0        0     9692 2023-05-28 06:39:10.054462 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/method.py
+-rw-r--r--   0        0        0     2778 2023-05-28 06:39:10.054879 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/styling.py
+-rw-r--r--   0        0        0     5323 2023-05-28 06:39:10.055258 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/techterm.py
+-rw-r--r--   0        0        0     2646 2023-05-28 06:39:10.055631 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/xml.py
+-rw-r--r--   0        0        0     1077 2023-05-21 10:48:36.178877 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/__init__.py
+-rw-r--r--   0        0        0     2880 2023-05-28 06:39:10.056042 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/base.py
+-rw-r--r--   0        0        0      407 2023-05-21 10:48:36.215373 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-28 06:39:10.057414 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py
+-rw-r--r--   0        0        0     1382 2023-05-28 06:39:10.057887 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py
+-rw-r--r--   0        0        0      625 2023-05-28 06:39:10.059023 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py
+-rw-r--r--   0        0        0      589 2023-05-28 06:39:10.059813 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py
+-rw-r--r--   0        0        0      446 2023-05-21 10:48:36.239199 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/__init__.py
+-rw-r--r--   0        0        0      747 2023-05-28 06:39:10.061164 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py
+-rw-r--r--   0        0        0      756 2023-05-28 06:39:10.062123 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py
+-rw-r--r--   0        0        0     1698 2023-05-28 06:39:10.063009 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py
+-rw-r--r--   0        0        0      715 2023-05-28 06:39:10.065667 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py
+-rw-r--r--   0        0        0      617 2023-05-28 06:39:10.066128 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py
+-rw-r--r--   0        0        0      204 2023-05-21 10:48:36.187774 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/__init__.py
+-rw-r--r--   0        0        0      683 2023-05-28 06:39:10.066509 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py
+-rw-r--r--   0        0        0      767 2023-05-28 06:39:10.066879 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py
+-rw-r--r--   0        0        0       97 2023-05-21 10:48:36.192351 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-28 06:39:10.068665 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/binopener.py
+-rw-r--r--   0        0        0       93 2023-05-21 10:48:36.200466 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/stylings/__init__.py
+-rw-r--r--   0        0        0      653 2023-05-28 06:39:10.069219 py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py
+-rw-r--r--   0        0        0      102 2023-04-23 12:35:30.862807 py_pdf_term-1.0.2/py_pdf_term/endtoend/caches.py
+-rw-r--r--   0        0        0      976 2023-05-21 10:48:36.271106 py_pdf_term-1.0.2/py_pdf_term/mappers.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.863506 py_pdf_term-1.0.2/py_pdf_term/methods/__init__.py
+-rw-r--r--   0        0        0      536 2023-05-21 10:48:36.254137 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/__init__.py
+-rw-r--r--   0        0        0     8473 2023-05-28 06:39:10.069816 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/base.py
+-rw-r--r--   0        0        0      567 2023-05-21 10:48:36.245483 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/__init__.py
+-rw-r--r--   0        0        0      981 2023-05-28 06:39:10.070484 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/base.py
+-rw-r--r--   0        0        0      998 2023-05-28 06:39:10.070879 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/flr.py
+-rw-r--r--   0        0        0     1004 2023-05-28 06:39:10.071286 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/flrh.py
+-rw-r--r--   0        0        0     1004 2023-05-28 06:39:10.072142 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/hits.py
+-rw-r--r--   0        0        0     1008 2023-05-28 06:39:10.072766 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/mcvalue.py
+-rw-r--r--   0        0        0      738 2023-05-28 06:39:10.073246 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/mdp.py
+-rw-r--r--   0        0        0      891 2023-05-28 06:39:10.073711 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/tfidf.py
+-rw-r--r--   0        0        0      924 2023-05-28 06:39:10.074373 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/data.py
+-rw-r--r--   0        0        0      583 2023-05-28 06:39:10.074916 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flr.py
+-rw-r--r--   0        0        0      939 2023-05-28 06:39:10.075329 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flrh.py
+-rw-r--r--   0        0        0     1170 2023-05-28 06:39:10.075719 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/hits.py
+-rw-r--r--   0        0        0      624 2023-05-28 06:39:10.076208 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mcvalue.py
+-rw-r--r--   0        0        0      581 2023-05-28 06:39:10.076805 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mdp.py
+-rw-r--r--   0        0        0      447 2023-05-21 10:48:36.254929 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/__init__.py
+-rw-r--r--   0        0        0     2087 2023-05-28 06:39:10.077795 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/base.py
+-rw-r--r--   0        0        0     2027 2023-05-28 06:39:10.078289 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flr.py
+-rw-r--r--   0        0        0     2847 2023-05-28 06:39:10.079027 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flrh.py
+-rw-r--r--   0        0        0     6308 2023-05-28 06:39:10.080583 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/hits.py
+-rw-r--r--   0        0        0     1966 2023-05-28 06:39:10.081142 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mcvalue.py
+-rw-r--r--   0        0        0     3145 2023-05-28 06:39:10.081601 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mdp.py
+-rw-r--r--   0        0        0     1983 2023-05-28 06:39:10.083388 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/tfidf.py
+-rw-r--r--   0        0        0      473 2023-05-21 10:48:36.275731 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/__init__.py
+-rw-r--r--   0        0        0      555 2023-05-28 06:39:10.083958 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/base.py
+-rw-r--r--   0        0        0      946 2023-05-28 06:39:10.084499 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flr.py
+-rw-r--r--   0        0        0      948 2023-05-28 06:39:10.085207 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flrh.py
+-rw-r--r--   0        0        0      948 2023-05-28 06:39:10.085888 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/hits.py
+-rw-r--r--   0        0        0     1429 2023-05-28 06:39:10.086461 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mcvalue.py
+-rw-r--r--   0        0        0     1182 2023-05-28 07:03:53.594747 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mdp.py
+-rw-r--r--   0        0        0      836 2023-05-28 06:39:10.087863 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/tfidf.py
+-rw-r--r--   0        0        0      602 2023-05-28 06:39:10.088395 py_pdf_term-1.0.2/py_pdf_term/methods/_methods/tfidf.py
+-rw-r--r--   0        0        0      110 2023-04-23 12:35:30.865641 py_pdf_term-1.0.2/py_pdf_term/methods/collectors.py
+-rw-r--r--   0        0        0      104 2023-04-23 12:35:30.866294 py_pdf_term-1.0.2/py_pdf_term/methods/rankers.py
+-rw-r--r--   0        0        0      112 2023-04-23 12:35:30.866995 py_pdf_term-1.0.2/py_pdf_term/methods/rankingdata.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.867710 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/__init__.py
+-rw-r--r--   0        0        0      174 2023-05-21 10:48:36.260616 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-21 10:48:36.285807 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/__init__.py
+-rw-r--r--   0        0        0      573 2023-05-28 06:39:10.089345 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py
+-rw-r--r--   0        0        0      367 2023-05-28 06:39:10.089829 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/standard.py
+-rw-r--r--   0        0        0     4054 2023-05-28 06:39:10.090619 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/converter.py
+-rw-r--r--   0        0        0     1415 2023-05-28 06:39:10.091183 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/data.py
+-rw-r--r--   0        0        0     5980 2023-05-28 06:39:10.092194 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/textful.py
+-rw-r--r--   0        0        0      824 2023-05-28 06:39:10.093197 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/utils.py
+-rw-r--r--   0        0        0      111 2023-04-30 07:57:40.332098 py_pdf_term-1.0.2/py_pdf_term/pdftoxml/binopeners.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.870578 py_pdf_term-1.0.2/py_pdf_term/stylings/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-21 10:48:36.286348 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/__init__.py
+-rw-r--r--   0        0        0     2475 2023-05-28 06:39:10.094712 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/data.py
+-rw-r--r--   0        0        0     3418 2023-05-28 06:39:10.095399 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scorer.py
+-rw-r--r--   0        0        0      185 2023-05-21 10:48:36.278288 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/__init__.py
+-rw-r--r--   0        0        0     1213 2023-05-28 06:39:10.096359 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/base.py
+-rw-r--r--   0        0        0     1185 2023-05-28 06:39:10.096968 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/color.py
+-rw-r--r--   0        0        0     1510 2023-05-28 06:39:10.097427 py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/fontsize.py
+-rw-r--r--   0        0        0      102 2023-04-23 12:35:30.871198 py_pdf_term-1.0.2/py_pdf_term/stylings/scores.py
+-rw-r--r--   0        0        0       91 2023-04-23 12:35:30.872290 py_pdf_term-1.0.2/py_pdf_term/techterms/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-21 10:48:36.292986 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/__init__.py
+-rw-r--r--   0        0        0     2403 2023-05-28 06:39:10.098467 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/data.py
+-rw-r--r--   0        0        0     6067 2023-05-28 06:39:10.099038 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/extractor.py
+-rw-r--r--   0        0        0      450 2023-05-28 06:39:10.099699 py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/utils.py
+-rw-r--r--   0        0        0       92 2023-04-30 07:57:40.332522 py_pdf_term-1.0.2/py_pdf_term/tokenizers/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-21 10:48:36.294274 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/__init__.py
+-rw-r--r--   0        0        0     1482 2023-05-28 06:39:10.101451 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/base.py
+-rw-r--r--   0        0        0     2533 2023-05-28 06:39:10.102033 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/data.py
+-rw-r--r--   0        0        0     1417 2023-05-28 06:39:10.102730 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/english.py
+-rw-r--r--   0        0        0     2864 2023-05-28 06:39:10.103262 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/japanese.py
+-rw-r--r--   0        0        0     1350 2023-05-28 06:39:10.103860 py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     1185 2023-05-28 07:03:53.595227 py_pdf_term-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 py_pdf_term-1.0.2/PKG-INFO
```

### Comparing `py_pdf_term-1.0.0/LICENSE` & `py_pdf_term-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/README.md` & `py_pdf_term-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/_common/consts.py` & `py_pdf_term-1.0.2/py_pdf_term/_common/consts.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/concats/lr.py` & `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/concats/lr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from typing import Dict
 
 from py_pdf_term.candidates import DomainCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from ..runner import AnalysisRunner
 
 
@@ -20,16 +19,16 @@
             If token or left is meaningless, this is fixed at zero.
         right_freq:
             Number of occurrences of lemmatized (token, right) in the domain.
             If token or right is meaningless, this is fixed at zero.
     """
 
     domain: str
-    left_freq: Dict[str, Dict[str, int]]
-    right_freq: Dict[str, Dict[str, int]]
+    left_freq: dict[str, dict[str, int]]
+    right_freq: dict[str, dict[str, int]]
 
 
 class TermLeftRightFrequencyAnalyzer:
     """Analyze left/right frequency of terms in a domain.
 
     Args
     ----
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/cooccurrences/container.py` & `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/cooccurrences/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from typing import Dict, Set
 
 from py_pdf_term.candidates import DomainCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from ..runner import AnalysisRunner
 
 
@@ -18,15 +17,15 @@
         container_terms:
             Set of lemmatized containers of the lemmatized term in the domain.
             (term, container) is valid if and only if the container contains the term as
             a proper subsequence.
     """
 
     domain: str
-    container_terms: Dict[str, Set[str]]
+    container_terms: dict[str, set[str]]
 
 
 class ContainerTermsAnalyzer:
     """Analyze container terms of the domain.
 
     Args
     ----
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/occurrences/term.py` & `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/occurrences/term.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from typing import Dict, Set
 
 from py_pdf_term.candidates import DomainCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from ..runner import AnalysisRunner
 
 
@@ -20,16 +19,16 @@
             Count even if the lemmatized term occurs as a part of a lemmatized phrase.
         doc_term_freq:
             Number of documents in the domain that contain the lemmatized term.
             Count even if the lemmatized term occurs as a part of a lemmatized phrase.
     """
 
     domain: str
-    term_freq: Dict[str, int]
-    doc_term_freq: Dict[str, int]
+    term_freq: dict[str, int]
+    doc_term_freq: dict[str, int]
 
 
 @dataclass(frozen=True)
 class _DomainTermOccurrence:
     """Domain name and term occurrence of the domain
 
     Args
@@ -41,16 +40,16 @@
             Count even if the lemmatized term occurs as a part of a lemmatized phrase.
         doc_term_set:
             Set of document IDs in the domain that contain the lemmatized term.
             Add even if the lemmatized term occurs as a part of a lemmatized phrase.
     """
 
     domain: str
-    term_freq: Dict[str, int]
-    doc_term_set: Dict[str, Set[int]]
+    term_freq: dict[str, int]
+    doc_term_set: dict[str, set[int]]
 
 
 class TermOccurrenceAnalyzer:
     """Analyze term occurrences in a domain.
 
     Args
     ----
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/runner.py` & `py_pdf_term-1.0.2/py_pdf_term/analysis/_analysis/runner.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/base.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABCMeta, abstractmethod
-from typing import List
 
 from py_pdf_term.tokenizers import Term
 
 
 class BaseAugmenter(metaclass=ABCMeta):
     """Base class for augmenters of a candidate term.
 
@@ -14,22 +13,22 @@
     This class is used to augment a candidate term to its subterms.
     """
 
     def __init__(self) -> None:
         pass
 
     @abstractmethod
-    def augment(self, term: Term) -> List[Term]:
+    def augment(self, term: Term) -> list[Term]:
         """Augment a candidate term.
 
         Args
         ----
             term:
-                A candidate term to be augmented.
+                Candidate term to be augmented.
 
         Returns
         -------
-            List[Term]:
-                A list of augmented terms. The first term is the original term.
+            list[Term]:
+                List of augmented terms. The first term is the original term.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.augment()")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/combiner.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/combiner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-from typing import List, Optional
-
 from py_pdf_term.tokenizers import Term
 
 from .base import BaseAugmenter
 from .separation import EnglishConnectorTermAugmenter, JapaneseConnectorTermAugmenter
 
 
 class AugmenterCombiner:
-    """A combiner of augmenters of a candidate term.
+    """Combiner of augmenters of a candidate term.
 
     Args
     ----
         augmenters:
-            A list of augmenters to be combined. The augmenters are applied in order.
+            List of augmenters to be combined. The augmenters are applied in order.
             If None, the default augmenters are used. The default augmenters are
             JapaneseConnectorTermAugmenter and EnglishConnectorTermAugmenter.
     """
 
-    def __init__(self, augmenters: Optional[List[BaseAugmenter]] = None) -> None:
+    def __init__(self, augmenters: list[BaseAugmenter] | None = None) -> None:
         if augmenters is None:
             augmenters = [
                 JapaneseConnectorTermAugmenter(),
                 EnglishConnectorTermAugmenter(),
             ]
 
         self._augmenters = augmenters
 
-    def augment(self, term: Term) -> List[Term]:
+    def augment(self, term: Term) -> list[Term]:
         """Augment a candidate term.
 
         Args
         ----
             term:
-                A candidate term to be augmented.
+                Candidate term to be augmented.
 
         Returns
         -------
-            List[Term]:
-                A list of augmented terms. The the original term is not included in the
+            list[Term]:
+                List of augmented terms. The the original term is not included in the
                 list.
         """
 
         augmented_terms = [term]
         for augmenter in self._augmenters:
-            start: List[Term] = []
+            start: list[Term] = []
             augmented_terms += sum(map(augmenter.augment, augmented_terms), start)
 
         return augmented_terms[1:]
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/separation.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/augmenters/separation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from abc import ABCMeta
-from typing import Callable, List
+from typing import Callable
 
 from py_pdf_term.tokenizers import Term, Token
 
 from ..classifiers import EnglishTokenClassifier, JapaneseTokenClassifier
 from .base import BaseAugmenter
 
 
 class BaseSeparationAugmenter(BaseAugmenter, metaclass=ABCMeta):
     """Base class for augmenters of a candidate term by separating tokens.
 
     Args
     ----
         is_separator:
-            A function to test whether a token is a separator or not.
+            Function to test whether a token is a separator or not.
     """
 
     def __init__(self, is_separator: Callable[[Token], bool]) -> None:
         self._is_separator = is_separator
 
-    def augment(self, term: Term) -> List[Term]:
+    def augment(self, term: Term) -> list[Term]:
         """Augment a candidate term by separating tokens.
 
         Args
         ----
             term:
-                A candidate term to be augmented.
+                Candidate term to be augmented.
 
         Returns
         -------
-            List[Term]:
-                A list of augmented terms. If a term consists of
+            list[Term]:
+                List of augmented terms. If a term consists of
                 "A separator B separator C", the list contains the following terms:
                 "A separator B separator C", "A separator B," "B separator C",
                 "A", "B", "C".
         """
 
         num_tokens = len(term.tokens)
         separation_positions = (
             [-1]
             + [i for i in range(num_tokens) if self._is_separator(term.tokens[i])]
             + [num_tokens]
         )
         num_positions = len(separation_positions)
 
-        augmented_terms: List[Term] = []
+        augmented_terms: list[Term] = []
         for length in range(1, num_positions - 1):
             for idx in range(num_positions - length):
                 i = separation_positions[idx]
                 j = separation_positions[idx + length]
                 tokens = term.tokens[i + 1 : j]
                 augmented_term = Term(tokens, term.fontsize, term.ncolor, True)
                 augmented_terms.append(augmented_term)
@@ -61,27 +61,27 @@
     terms.
     """
 
     def __init__(self) -> None:
         classifier = JapaneseTokenClassifier()
         super().__init__(classifier.is_connector_term)
 
-    def augment(self, term: Term) -> List[Term]:
+    def augment(self, term: Term) -> list[Term]:
         """Augment a candidate term by separating tokens based on Japanese connector
         terms.
 
         Args
         ----
             term:
-                A candidate term to be augmented.
+                Candidate term to be augmented.
 
         Returns
         -------
-            List[Term]:
-                A list of augmented terms.
+            list[Term]:
+                List of augmented terms.
                 If a given term is not a Japanese term, the list is empty.
         """
 
         if term.lang != "ja":
             return []
 
         return super().augment(term)
@@ -92,27 +92,27 @@
     terms.
     """
 
     def __init__(self) -> None:
         classifier = EnglishTokenClassifier()
         super().__init__(classifier.is_connector_term)
 
-    def augment(self, term: Term) -> List[Term]:
+    def augment(self, term: Term) -> list[Term]:
         """Augment a candidate term by separating tokens based on English connector
         terms.
 
         Args
         ----
             term:
-                A candidate term to be augmented.
+                Candidate term to be augmented.
 
         Returns
         -------
-            List[Term]:
-                A list of augmented terms.
+            list[Term]:
+                List of augmented terms.
                 If a given term is not an English term, the list is empty.
         """
 
         if term.lang != "en":
             return []
 
         return super().augment(term)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/base.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     @abstractmethod
     def inscope(self, token: Token) -> bool:
         """Test whether a token is in the scope of this classifier or not.
 
         Args
         ----
             token:
-                A token to be tested.
+                Token to be tested.
 
         Returns
         -------
             bool:
                 True if the token is in the scope of this classifier, False otherwise.
         """
 
@@ -31,15 +31,15 @@
     @abstractmethod
     def is_symbol(self, token: Token) -> bool:
         """Test whether a token is a symbol or not.
 
         Args
         ----
             token:
-                A token to be tested.
+               Token to be tested.
 
         Returns
         -------
             bool:
                 True if the token is a symbol, False otherwise.
         """
 
@@ -50,15 +50,15 @@
         """Test whether a token is a connector symbol or not. A connector symbol is a
         symbol that is used to connect two terms such as - and ・.
         If this method returns True, is_symbol() must also return True.
 
         Args
         ----
             token:
-                A token to be tested.
+                Token to be tested.
 
         Returns
         -------
             bool:
                 True if the token is a connector symbol, False otherwise.
         """
 
@@ -69,15 +69,15 @@
         """Test whether a token is a connector term or not. A connector term is a term
         that is used to connect two terms such as "of" and "in" in English, and "の" in
         Japanese.
 
         Args
         ----
             token:
-                A token to be tested.
+                Token to be tested.
 
         Returns
         -------
             bool:
                 True if the token is a connector term, False otherwise.
         """
 
@@ -86,15 +86,15 @@
     def is_meaningless(self, token: Token) -> bool:
         """Test whether a token is meaningless or not. A meaningless token is a token
         that does not have any meaning such as a symbol and a connector term.
 
         Args
         ----
             token:
-                A token to be tested.
+                Token to be tested.
 
         Returns
         -------
             bool:
                 True if the token is meaningless, False otherwise.
         """
 
@@ -107,15 +107,15 @@
     def is_connector(self, token: Token) -> bool:
         """Test whether a token is a connector or not. A connector is a token that is
         used to connect two terms such as a connector symbol and a connector term.
 
         Args
         ----
             token:
-                A token to be tested.
+                Token to be tested.
 
         Returns
         -------
             bool:
                 True if the token is a connector, False otherwise.
         """
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/english.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/english.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from py_pdf_term.tokenizers import Token
 
 from .base import BaseTokenClassifier
 
 
 class EnglishTokenClassifier(BaseTokenClassifier):
-    """A token classifier for English tokens."""
+    """Token classifier for English tokens."""
 
     def inscope(self, token: Token) -> bool:
         return token.lang == "en"
 
     def is_symbol(self, token: Token) -> bool:
         return token.pos in {"SYM"}
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/japanese.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/japanese.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from py_pdf_term.tokenizers import Token
 
 from .base import BaseTokenClassifier
 
 
 class JapaneseTokenClassifier(BaseTokenClassifier):
-    """A token classifier for Japanese tokens."""
+    """Token classifier for Japanese tokens."""
 
     def inscope(self, token: Token) -> bool:
         return token.lang == "ja"
 
     def is_symbol(self, token: Token) -> bool:
         return token.pos in {"補助記号"}
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/marker.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/classifiers/marker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-from typing import List, Optional
-
 from py_pdf_term.tokenizers import Term
 
 from .base import BaseTokenClassifier
 from .english import EnglishTokenClassifier
 from .japanese import JapaneseTokenClassifier
 
 
 class MeaninglessMarker:
-    """The marker class to mark meaningless tokens in a term.
+    """Marker class to mark meaningless tokens in a term.
 
     Args
     ----
         classifiers:
-            A list of token classifiers to mark meaningless tokens.
+            List of token classifiers to mark meaningless tokens.
             If None, JapaneseTokenClassifier and EnglishTokenClassifier are used.
     """
 
-    def __init__(self, classifiers: Optional[List[BaseTokenClassifier]] = None) -> None:
+    def __init__(self, classifiers: list[BaseTokenClassifier] | None = None) -> None:
         if classifiers is None:
             classifiers = [
                 JapaneseTokenClassifier(),
                 EnglishTokenClassifier(),
             ]
 
         self._classifiers = classifiers
 
     def mark(self, term: Term) -> Term:
         """Mark meaningless tokens in a term. The original term is modified in-place.
 
         Args
         ----
             term:
-                A term to be marked.
+                Term to be marked.
 
         Returns
         -------
             Term:
-                A term with meaningless tokens marked.
+                Term with meaningless tokens marked.
         """
 
         for token in term.tokens:
             token.is_meaningless = any(
                 map(
                     lambda classifier: classifier.inscope(token)
                     and classifier.is_meaningless(token),
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/data.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Set
+from typing import Any, Callable
 
 from py_pdf_term.tokenizers import Term
 
 
 @dataclass(frozen=True)
 class PageCandidateTermList:
     """Page number and candidate terms of the page.
@@ -13,38 +13,38 @@
         page_num:
             Page number of a PDF file.
         candidates:
             Candidate terms of the page.
     """
 
     page_num: int
-    candidates: List[Term]
+    candidates: list[Term]
 
     def to_nostyle_candidates_dict(
         self, to_str: Callable[[Term], str] = str
-    ) -> Dict[str, Term]:
-        term_dict: Dict[str, Term] = dict()
+    ) -> dict[str, Term]:
+        term_dict: dict[str, Term] = dict()
         for candidate in self.candidates:
             candidate_str = to_str(candidate)
             if candidate_str in term_dict:
                 continue
             term_dict[candidate_str] = Term(candidate.tokens, 0.0, "", False)
         return term_dict
 
-    def to_candidates_str_set(self, to_str: Callable[[Term], str] = str) -> Set[str]:
+    def to_candidates_str_set(self, to_str: Callable[[Term], str] = str) -> set[str]:
         return {to_str(candidate) for candidate in self.candidates}
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "page_num": self.page_num,
             "candidates": list(map(lambda term: term.to_dict(), self.candidates)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PageCandidateTermList":
+    def from_dict(cls, obj: dict[str, Any]) -> "PageCandidateTermList":
         page_num, candidates = obj["page_num"], obj["candidates"]
         return cls(
             page_num,
             list(map(lambda item: Term.from_dict(item), candidates)),
         )
 
 
@@ -57,42 +57,42 @@
         pdf_path:
             Path of a PDF file.
         pages:
             Candidate terms of each page of the PDF file.
     """
 
     pdf_path: str
-    pages: List[PageCandidateTermList]
+    pages: list[PageCandidateTermList]
 
     def to_nostyle_candidates_dict(
         self, to_str: Callable[[Term], str] = str
-    ) -> Dict[str, Term]:
-        term_dict: Dict[str, Term] = dict()
+    ) -> dict[str, Term]:
+        term_dict: dict[str, Term] = dict()
         for page in self.pages:
             candidate_items = page.to_nostyle_candidates_dict(to_str).items()
             for candidate_str, candidate in candidate_items:
                 if candidate_str in term_dict:
                     continue
                 term_dict[candidate_str] = candidate
         return term_dict
 
-    def to_candidates_str_set(self, to_str: Callable[[Term], str] = str) -> Set[str]:
-        empty: Set[str] = set()
+    def to_candidates_str_set(self, to_str: Callable[[Term], str] = str) -> set[str]:
+        empty: set[str] = set()
         return empty.union(
             *map(lambda page: page.to_candidates_str_set(to_str), self.pages)
         )
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "pdf_path": self.pdf_path,
             "pages": list(map(lambda page: page.to_dict(), self.pages)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PDFCandidateTermList":
+    def from_dict(cls, obj: dict[str, Any]) -> "PDFCandidateTermList":
         pdf_path, pages = obj["pdf_path"], obj["pages"]
         return cls(
             pdf_path,
             list(map(lambda item: PageCandidateTermList.from_dict(item), pages)),
         )
 
 
@@ -105,40 +105,40 @@
         domain:
             Domain name. (e.g., "natural language processing")
         pdfs:
             Candidate terms of each PDF file of the domain.
     """
 
     domain: str
-    pdfs: List[PDFCandidateTermList]
+    pdfs: list[PDFCandidateTermList]
 
     def to_nostyle_candidates_dict(
         self, to_str: Callable[[Term], str] = str
-    ) -> Dict[str, Term]:
-        term_dict: Dict[str, Term] = dict()
+    ) -> dict[str, Term]:
+        term_dict: dict[str, Term] = dict()
         for pdf in self.pdfs:
             candidate_items = pdf.to_nostyle_candidates_dict(to_str).items()
             for candidate_str, candidate in candidate_items:
                 if candidate_str in term_dict:
                     continue
                 term_dict[candidate_str] = candidate
         return term_dict
 
-    def to_candidates_str_set(self, to_str: Callable[[Term], str] = str) -> Set[str]:
-        empty: Set[str] = set()
+    def to_candidates_str_set(self, to_str: Callable[[Term], str] = str) -> set[str]:
+        empty: set[str] = set()
         return empty.union(
             *map(lambda pdf: pdf.to_candidates_str_set(to_str), self.pdfs)
         )
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "domain": self.domain,
             "pdfs": list(map(lambda pdf: pdf.to_dict(), self.pdfs)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "DomainCandidateTermList":
+    def from_dict(cls, obj: dict[str, Any]) -> "DomainCandidateTermList":
         domain, pdfs = obj["domain"], obj["pdfs"]
         return cls(
             domain,
             list(map(lambda item: PDFCandidateTermList.from_dict(item), pdfs)),
         )
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/extractor.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from typing import List, Optional, Type, cast
+from typing import cast
 from xml.etree.ElementTree import Element, parse
 
 from py_pdf_term.pdftoxml import PDFnXMLElement, PDFnXMLPath
 from py_pdf_term.tokenizers import BaseLanguageTokenizer, Term, Token, Tokenizer
 
 from .augmenters import AugmenterCombiner, BaseAugmenter
 from .classifiers import BaseTokenClassifier, MeaninglessMarker
 from .data import DomainCandidateTermList, PageCandidateTermList, PDFCandidateTermList
 from .filters import BaseCandidateTermFilter, BaseCandidateTokenFilter, FilterCombiner
 from .splitters import BaseSplitter, SplitterCombiner
 from .utils import textnode_fontsize, textnode_ncolor, textnode_text
 
 
 class CandidateTermExtractor:
-    """A term extractor which extracts candidate terms from a XML file.
+    """Term extractor which extracts candidate terms from a XML file.
 
     Args
     ----
         lang_tokenizer_clses:
-            A list of language tokenizer classes to tokenize texts. If None, the default
+            List of language tokenizer classes to tokenize texts. If None, the default
             language tokenizers are used.
 
         token_classifier_clses:
-            A list of token classifier classes to classify tokens. If None, the default
+            List of token classifier classes to classify tokens. If None, the default
             token classifiers are used.
 
         token_filter_clses:
-            A list of token filter classes to filter tokens. If None, the default token
+            List of token filter classes to filter tokens. If None, the default token
             filters are used.
 
         term_filter_clses:
-            A list of term filter classes to filter candidate terms. If None, the
+            List of term filter classes to filter candidate terms. If None, the
             default term filters are used.
 
         splitter_clses:
-            A list of splitter classes to split candidate terms. If None, the default
+            List of splitter classes to split candidate terms. If None, the default
             splitters are used.
 
         augmenter_clses:
-            A list of augmenter classes to augment candidate terms. If None, the default
+            List of augmenter classes to augment candidate terms. If None, the default
             augmenters are used.
     """
 
     def __init__(
         self,
-        lang_tokenizer_clses: Optional[List[Type[BaseLanguageTokenizer]]] = None,
-        token_classifier_clses: Optional[List[Type[BaseTokenClassifier]]] = None,
-        token_filter_clses: Optional[List[Type[BaseCandidateTokenFilter]]] = None,
-        term_filter_clses: Optional[List[Type[BaseCandidateTermFilter]]] = None,
-        splitter_clses: Optional[List[Type[BaseSplitter]]] = None,
-        augmenter_clses: Optional[List[Type[BaseAugmenter]]] = None,
+        lang_tokenizer_clses: list[type[BaseLanguageTokenizer]] | None = None,
+        token_classifier_clses: list[type[BaseTokenClassifier]] | None = None,
+        token_filter_clses: list[type[BaseCandidateTokenFilter]] | None = None,
+        term_filter_clses: list[type[BaseCandidateTermFilter]] | None = None,
+        splitter_clses: list[type[BaseSplitter]] | None = None,
+        augmenter_clses: list[type[BaseAugmenter]] | None = None,
     ) -> None:
         lang_tokenizers = (
             list(map(lambda cls: cls(), lang_tokenizer_clses))
             if lang_tokenizer_clses is not None
             else None
         )
         self._tokenizer = Tokenizer(lang_tokenizers=lang_tokenizers)
@@ -88,141 +88,141 @@
             list(map(lambda cls: cls(), augmenter_clses))
             if augmenter_clses is not None
             else None
         )
         self._augmenter = AugmenterCombiner(augmenters)
 
     def extract_from_domain_files(
-        self, domain: str, pdfnxmls: List[PDFnXMLPath]
+        self, domain: str, pdfnxmls: list[PDFnXMLPath]
     ) -> DomainCandidateTermList:
         """Extract candidte terms from pairs of PDF and XML files in a domain.
 
         Args
         ----
             domain:
-                A domain name of PDF files.
+                Domain name of PDF files.
             pdfnxmls:
-                A list of pairs of paths to PDF and XML files in a domain.
+                List of pairs of paths to PDF and XML files in a domain.
 
         Returns
         -------
             DomainCandidateTermList:
-                A list of candidate terms in a domain.
+                List of candidate terms in a domain.
         """
 
         xmls = list(map(self.extract_from_xml_file, pdfnxmls))
         return DomainCandidateTermList(domain, xmls)
 
     def extract_from_xml_file(self, pdfnxml: PDFnXMLPath) -> PDFCandidateTermList:
         """Extract candidate terms from a pair of PDF and XML files.
 
         Args
         ----
             pdfnxml:
-                A pair of paths to a PDF and XML file.
+                Pair of paths to a PDF and XML file.
 
         Returns
         -------
             PDFCandidateTermList:
-                A list of candidate terms in a PDF file.
+                List of candidate terms in a PDF file.
         """
 
         xml_root = parse(pdfnxml.xml_path).getroot()
         xml_candidates = self._extract_from_xmlroot(pdfnxml.pdf_path, xml_root)
         return xml_candidates
 
     def extract_from_domain_elements(
-        self, domain: str, pdfnxmls: List[PDFnXMLElement]
+        self, domain: str, pdfnxmls: list[PDFnXMLElement]
     ) -> DomainCandidateTermList:
         """Extract candidate terms from pairs of PDF and XML elements in a domain.
 
         Args
         ----
             domain:
-                A domain name of PDF files.
+                Domain name of PDF files.
             pdfnxmls:
-                A list of pairs of paths to PDF and XML elements in a domain.
+                List of pairs of paths to PDF and XML elements in a domain.
 
         Returns
         -------
             DomainCandidateTermList:
-                A list of candidate terms in a domain.
+                List of candidate terms in a domain.
         """
 
         xmls = list(map(self.extract_from_xml_element, pdfnxmls))
         return DomainCandidateTermList(domain, xmls)
 
     def extract_from_xml_element(self, pdfnxml: PDFnXMLElement) -> PDFCandidateTermList:
         """Extract candidate terms from a pair of PDF and XML elements.
 
         Args
         ----
             pdfnxml:
-                A pair of path to a PDF and XML elements.
+                Pair of path to a PDF and XML elements.
 
         Returns
         -------
             PDFCandidateTermList:
-                A list of candidate terms in a PDF file.
+                List of candidate terms in a PDF file.
         """
 
         xml_candidates = self._extract_from_xmlroot(pdfnxml.pdf_path, pdfnxml.xml_root)
         return xml_candidates
 
     def extract_from_text(
         self, text: str, fontsize: float = 0.0, ncolor: str = ""
-    ) -> List[Term]:
+    ) -> list[Term]:
         """Extract candidate terms from a text. This method is mainly used for testing.
 
         Args
         ----
             text:
-                A text to extract candidate terms.
+                Text to extract candidate terms.
             fontsize:
-                A font size of output terms.
+                Font size of output terms.
             ncolor:
-                A color of output terms.
+                Color of output terms.
 
         Returns
         -------
-            List[Term]:
-                A list of candidate terms in a text.
+            list[Term]:
+                List of candidate terms in a text.
         """
 
         tokens = self._tokenizer.tokenize(text)
         return self._extract_from_tokens(tokens, fontsize, ncolor)
 
     def _extract_from_xmlroot(
         self, pdf_path: str, xml_root: Element
     ) -> PDFCandidateTermList:
-        page_candidates: List[PageCandidateTermList] = []
+        page_candidates: list[PageCandidateTermList] = []
         for page in xml_root.iter("page"):
             page_candidates.append(self._extract_from_page(page))
 
         return PDFCandidateTermList(pdf_path, page_candidates)
 
     def _extract_from_page(self, page: Element) -> PageCandidateTermList:
         page_num = int(cast(str, page.get("id")))
 
-        candicate_terms: List[Term] = []
+        candicate_terms: list[Term] = []
         for textnode in page.iter("text"):
             text = textnode_text(textnode)
             fontsize = textnode_fontsize(textnode)
             ncolor = textnode_ncolor(textnode)
             tokens = self._tokenizer.tokenize(text)
             terms = self._extract_from_tokens(tokens, fontsize, ncolor)
             candicate_terms.extend(terms)
 
         return PageCandidateTermList(page_num, candicate_terms)
 
     def _extract_from_tokens(
-        self, tokens: List[Token], fontsize: float, ncolor: str
-    ) -> List[Term]:
-        candicate_terms: List[Term] = []
-        candicate_tokens: List[Token] = []
+        self, tokens: list[Token], fontsize: float, ncolor: str
+    ) -> list[Term]:
+        candicate_terms: list[Term] = []
+        candicate_tokens: list[Token] = []
         for idx, token in enumerate(tokens):
             if self._filter.is_partof_candidate(tokens, idx):
                 candicate_tokens.append(token)
                 continue
 
             terms = self._terms_from_tokens(candicate_tokens, fontsize, ncolor)
             candicate_terms.extend(terms)
@@ -230,19 +230,19 @@
 
         terms = self._terms_from_tokens(candicate_tokens, fontsize, ncolor)
         candicate_terms.extend(terms)
 
         return candicate_terms
 
     def _terms_from_tokens(
-        self, candicate_tokens: List[Token], fontsize: float, ncolor: str
-    ) -> List[Term]:
+        self, candicate_tokens: list[Token], fontsize: float, ncolor: str
+    ) -> list[Term]:
         candidate_term = Term(candicate_tokens, fontsize, ncolor)
 
-        candicate_terms: List[Term] = []
+        candicate_terms: list[Term] = []
         splitted_candidates = self._splitter.split(candidate_term)
         for splitted_candidate in splitted_candidates:
             augmented_candidates = self._augmenter.augment(splitted_candidate)
             candicate_terms.extend(augmented_candidates)
             candicate_terms.append(splitted_candidate)
 
         return list(
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/__init__.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/combiner.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/combiner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List, Optional
-
 from py_pdf_term.tokenizers import Term, Token
 
 from .term import (
     BaseCandidateTermFilter,
     EnglishConcatenationFilter,
     EnglishNumericFilter,
     EnglishProperNounFilter,
@@ -13,35 +11,35 @@
     JapaneseProperNounFilter,
     JapaneseSymbolLikeFilter,
 )
 from .token import BaseCandidateTokenFilter, EnglishTokenFilter, JapaneseTokenFilter
 
 
 class FilterCombiner:
-    """A combiner of token filters and term filters.
+    """Combiner of token filters and term filters.
 
     Args
     ----
         token_filters:
-            A list of token filters to filter tokens. If None, the default token filters
+            List of token filters to filter tokens. If None, the default token filters
             are used. The default token filters are JapaneseTokenFilter and
             EnglishTokenFilter.
 
         term_filters:
-            A list of term filters to filter candidate terms. If None, the default term
+            List of term filters to filter candidate terms. If None, the default term
             filters are used. The default term filters are JapaneseConcatenationFilter,
             EnglishConcatenationFilter, JapaneseSymbolLikeFilter,
             EnglishSymbolLikeFilter, JapaneseProperNounFilter,
             EnglishProperNounFilter, JapaneseNumericFilter, and EnglishNumericFilter.
     """
 
     def __init__(
         self,
-        token_filters: Optional[List[BaseCandidateTokenFilter]] = None,
-        term_filters: Optional[List[BaseCandidateTermFilter]] = None,
+        token_filters: list[BaseCandidateTokenFilter] | None = None,
+        term_filters: list[BaseCandidateTermFilter] | None = None,
     ) -> None:
         if token_filters is None:
             token_filters = [
                 JapaneseTokenFilter(),
                 EnglishTokenFilter(),
             ]
         if term_filters is None:
@@ -55,23 +53,23 @@
                 JapaneseNumericFilter(),
                 EnglishNumericFilter(),
             ]
 
         self._token_filters = token_filters
         self._term_filters = term_filters
 
-    def is_partof_candidate(self, tokens: List[Token], idx: int) -> bool:
+    def is_partof_candidate(self, tokens: list[Token], idx: int) -> bool:
         """Test if a token can be part of a candidate term using token filters.
 
         Args
         ----
             tokens:
-                A list of tokens.
+                List of tokens.
             idx:
-                An index of the token to be tested.
+                Index of the token to be tested.
 
         Returns
         -------
             bool:
                 True if the token can be part of a candidate term, False otherwise.
         """
 
@@ -88,15 +86,15 @@
 
     def is_candidate(self, term: Term) -> bool:
         """Test if a term is a candidate term using term filters.
 
         Args
         ----
             term:
-                A term to be tested.
+                Term to be tested.
 
         Returns
         -------
             bool:
                 True if the term is a candidate term, False otherwise.
         """
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/__init__.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/base.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     @abstractmethod
     def inscope(self, term: Term) -> bool:
         """Test if a term is in scope of this filter.
 
         Args
         ----
             term:
-                A term to be tested.
+                Term to be tested.
 
 
         Returns
         -------
             bool:
                 True if the term is in scope of this filter, False otherwise.
         """
@@ -32,15 +32,15 @@
     @abstractmethod
     def is_candidate(self, scoped_term: Term) -> bool:
         """Test if a scoped term is a candidate term.
 
         Args
         ----
             scoped_term:
-                A scoped term to be tested.
+                Scoped term to be tested.
 
         Returns
         -------
             bool:
                 True if the scoped term is a candidate term, False otherwise.
         """
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ....classifiers import EnglishTokenClassifier
 from ..base import BaseEnglishCandidateTermFilter
 
 PHONETIC_REGEX = ALPHABET_REGEX
 
 
 class EnglishConcatenationFilter(BaseEnglishCandidateTermFilter):
-    """A candidate term filter to filter out invalidly concatenated English terms."""
+    """Candidate term filter to filter out invalidly concatenated English terms."""
 
     def __init__(self) -> None:
         self._classifier = EnglishTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return (
             self._is_norn_phrase(scoped_term)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ....classifiers import JapaneseTokenClassifier
 from ..base import BaseJapaneseCandidateTermFilter
 
 PHONETIC_REGEX = rf"{HIRAGANA_REGEX}|{KATAKANA_REGEX}|{ALPHABET_REGEX}"
 
 
 class JapaneseConcatenationFilter(BaseJapaneseCandidateTermFilter):
-    """A candidate term filter to filter out invalidly concatenated Japanese terms."""
+    """Candidate term filter to filter out invalidly concatenated Japanese terms."""
 
     def __init__(self) -> None:
         self._classifier = JapaneseTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return (
             self._is_norn_phrase(scoped_term)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from py_pdf_term.tokenizers import Term, Token
 
 from ....classifiers import EnglishTokenClassifier
 from ..base import BaseEnglishCandidateTermFilter
 
 
 class EnglishNumericFilter(BaseEnglishCandidateTermFilter):
-    """A term filter to remove English numeric phrases from candidate terms."""
+    """Term filter to remove English numeric phrases from candidate terms."""
 
     def __init__(self) -> None:
         self._classifier = EnglishTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return not self._is_numeric_phrase(scoped_term)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from py_pdf_term.tokenizers import Term, Token
 
 from ....classifiers import JapaneseTokenClassifier
 from ..base import BaseJapaneseCandidateTermFilter
 
 
 class JapaneseNumericFilter(BaseJapaneseCandidateTermFilter):
-    """A term filter to remove Japanese numeric phrases from candidate terms."""
+    """Term filter to remove Japanese numeric phrases from candidate terms."""
 
     def __init__(self) -> None:
         self._classifier = JapaneseTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return not self._is_numeric_phrase(scoped_term)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from py_pdf_term.tokenizers import Term, Token
 
 from ....classifiers import JapaneseTokenClassifier
 from ..base import BaseJapaneseCandidateTermFilter
 
 
 class JapaneseProperNounFilter(BaseJapaneseCandidateTermFilter):
-    """A term filter to remove Japanese proper nouns from candidate terms."""
+    """Term filter to remove Japanese proper nouns from candidate terms."""
 
     def __init__(self) -> None:
         self._classifier = JapaneseTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return not self._is_region_or_person(scoped_term)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ....classifiers import EnglishTokenClassifier
 from ..base import BaseEnglishCandidateTermFilter
 
 PHONETIC_REGEX = ALPHABET_REGEX
 
 
 class EnglishSymbolLikeFilter(BaseEnglishCandidateTermFilter):
-    """A candidate term filter to filter out symbol-like English terms."""
+    """Candidate term filter to filter out symbol-like English terms."""
 
     def __init__(self) -> None:
         self._classifier = EnglishTokenClassifier()
         self._phonetic_regex = re.compile(PHONETIC_REGEX)
         self._indexed_phonetic_regex = re.compile(
             rf"({PHONETIC_REGEX}{NUMBER_REGEX}+)+{PHONETIC_REGEX}?"
             + "|"
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ....classifiers import JapaneseTokenClassifier
 from ..base import BaseJapaneseCandidateTermFilter
 
 PHONETIC_REGEX = rf"(?:{HIRAGANA_REGEX}|{KATAKANA_REGEX}|{ALPHABET_REGEX})"
 
 
 class JapaneseSymbolLikeFilter(BaseJapaneseCandidateTermFilter):
-    """A candidate term filter to filter out symbol-like Japanese terms."""
+    """Candidate term filter to filter out symbol-like Japanese terms."""
 
     def __init__(self) -> None:
         self._classifier = JapaneseTokenClassifier()
         self._phonetic_regex = re.compile(PHONETIC_REGEX)
         self._indexed_phonetic_regex = re.compile(
             rf"({PHONETIC_REGEX}{NUMBER_REGEX}+)+{PHONETIC_REGEX}?"
             + "|"
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/base.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABCMeta, abstractmethod
-from typing import List
 
 from py_pdf_term.tokenizers import Token
 
 
 class BaseCandidateTokenFilter(metaclass=ABCMeta):
     """Base class for filters of tokens which can be part of a candidate term."""
 
@@ -13,33 +12,33 @@
     @abstractmethod
     def inscope(self, token: Token) -> bool:
         """Test if a token is in scope of this filter.
 
         Args
         ----
             token:
-                A token to be tested.
+                Token to be tested.
 
 
         Returns
         -------
             bool:
                 True if the token is in scope of this filter, False otherwise.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.inscope()")
 
     @abstractmethod
-    def is_partof_candidate(self, tokens: List[Token], idx: int) -> bool:
+    def is_partof_candidate(self, tokens: list[Token], idx: int) -> bool:
         """Test if a token can be part of a candidate term.
 
         Args
         ----
             tokens:
-                A list of tokens.
+                List of tokens.
             idx:
                 An index of the token to be tested.
 
 
         Returns
         -------
             bool:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/english.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/english.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 import re
-from typing import List
 
 from py_pdf_term._common.consts import ENGLISH_REGEX, NUMBER_REGEX
 from py_pdf_term.tokenizers import Token
 
 from .base import BaseCandidateTokenFilter
 
 
 class EnglishTokenFilter(BaseCandidateTokenFilter):
-    """A candidate token filter to filter out English tokens which cannot be part of
+    """Candidate token filter to filter out English tokens which cannot be part of
     candidate terms.
     """
 
     def __init__(self) -> None:
         self._regex = re.compile(rf"({ENGLISH_REGEX}|{NUMBER_REGEX})+")
 
     def inscope(self, token: Token) -> bool:
         token_str = str(token)
         return token.lang == "en" and (
             self._regex.fullmatch(token_str) is not None or token_str == "-"
         )
 
-    def is_partof_candidate(self, tokens: List[Token], idx: int) -> bool:
+    def is_partof_candidate(self, tokens: list[Token], idx: int) -> bool:
         scoped_token = tokens[idx]
         num_tokens = len(tokens)
 
-        if scoped_token.pos in {"NOUN", "PROPN", "NUM"}:
-            return True
-        elif scoped_token.pos == "ADJ":
-            return (
-                idx < num_tokens - 1
-                and tokens[idx + 1].pos in {"NOUN", "PROPN", "ADJ", "VERB", "SYM"}
-                # No line break
-            )
-        elif scoped_token.pos == "VERB":
-            return scoped_token.category == "VBG" or (
-                scoped_token.category == "VBN"
-                and idx < num_tokens - 1
-                and tokens[idx + 1].pos in {"NOUN", "PROPN", "ADJ", "VERB", "SYM"}
-            )
-        elif scoped_token.pos == "ADP":
-            return scoped_token.category == "IN"
-        elif scoped_token.pos == "SYM":
-            return (
-                scoped_token.surface_form == "-"
-                and 0 < idx < num_tokens - 1
-                and self._regex.match(str(tokens[idx - 1])) is not None
-                and self._regex.match(str(tokens[idx + 1])) is not None
-            )
-
-        return False
+        match scoped_token.pos:
+            case "NOUN" | "PROPN" | "NUM":
+                return True
+            case "ADJ":
+                return (
+                    idx < num_tokens - 1
+                    and tokens[idx + 1].pos in {"NOUN", "PROPN", "ADJ", "VERB", "SYM"}
+                    # No line break
+                )
+            case "VERB":
+                if scoped_token.category == "VBG":
+                    return True
+                elif scoped_token.category == "VBN":
+                    return (
+                        idx < num_tokens - 1
+                        and tokens[idx + 1].pos
+                        in {"NOUN", "PROPN", "ADJ", "VERB", "SYM"}
+                        # No line break
+                    )
+                return False
+            case "ADP":
+                return scoped_token.category in {"IN"}
+            case "SYM":
+                return (
+                    scoped_token.surface_form == "-"
+                    and 0 < idx < num_tokens - 1
+                    and self._regex.match(str(tokens[idx - 1])) is not None
+                    and self._regex.match(str(tokens[idx + 1])) is not None
+                )
+            case _:
+                return False
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/japanese.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/filters/token/japanese.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,72 @@
 import re
-from typing import List
 
 from py_pdf_term._common.consts import ENGLISH_REGEX, JAPANESE_REGEX, NUMBER_REGEX
 from py_pdf_term.tokenizers import Token
 
 from .base import BaseCandidateTokenFilter
 
 
 class JapaneseTokenFilter(BaseCandidateTokenFilter):
-    """A candidate token filter to filter out Japanese tokens which cannot be part of
+    """Candidate token filter to filter out Japanese tokens which cannot be part of
     candidate terms.
     """
 
     def __init__(self) -> None:
         self._regex = re.compile(rf"({JAPANESE_REGEX}|{ENGLISH_REGEX}|{NUMBER_REGEX})+")
 
     def inscope(self, token: Token) -> bool:
         token_str = str(token)
         return token.lang == "ja" and (
             self._regex.fullmatch(token_str) is not None or token_str == "-"
         )
 
-    def is_partof_candidate(self, tokens: List[Token], idx: int) -> bool:
+    def is_partof_candidate(self, tokens: list[Token], idx: int) -> bool:
         scoped_token = tokens[idx]
         num_tokens = len(tokens)
 
-        if scoped_token.pos == "名詞":
-            return (
-                (
-                    scoped_token.category == "普通名詞"
+        match scoped_token.pos:
+            case "名詞":
+                return (
+                    scoped_token.category in {"普通名詞"}
                     and scoped_token.subcategory
                     in {"一般", "サ変可能", "形状詞可能", "サ変形状詞可能", "助数詞可能"}
+                ) or scoped_token.category in {"固有名詞", "数詞"}
+            case "形状詞" | "形容詞":
+                return (
+                    scoped_token.category in {"一般"}
+                    and idx < num_tokens - 1
+                    and tokens[idx + 1].pos in {"名詞", "記号", "接尾辞", "形状詞", "形容詞"}
                 )
-                or scoped_token.category == "固有名詞"
-                or scoped_token.category == "数詞"
-            )
-        elif scoped_token.pos in {"形状詞", "形容詞"}:
-            return (
-                scoped_token.category in {"一般"}
-                and idx < num_tokens - 1
-                and tokens[idx + 1].pos in {"名詞", "記号", "接尾辞", "形状詞", "形容詞"}
-            )
-        elif scoped_token.pos == "動詞":
-            return (
-                scoped_token.category in {"一般"}
-                and idx < num_tokens - 1
-                and tokens[idx + 1].pos in {"接尾辞", "動詞"}
-            )
-        elif scoped_token.pos == "接頭辞":
-            return (
-                idx < num_tokens - 1
-                and tokens[idx + 1].pos in {"名詞", "記号", "形状詞"}
-                # No line break
-            )
-        elif scoped_token.pos == "接尾辞":
-            return (
-                scoped_token.category in {"名詞的", "形状詞的"}
-                and idx > 0
-                and tokens[idx - 1].pos in {"名詞", "形状詞", "動詞", "形容詞", "記号"}
-            )
-        elif scoped_token.pos == "助詞":
-            return scoped_token.surface_form == "の"
-        elif scoped_token.pos == "記号":
-            return self._regex.match(str(scoped_token)) is not None
-        elif scoped_token.pos == "補助記号":
-            scoped_token_str = str(scoped_token)
-            if scoped_token_str not in {"-", "・"}:
+            case "動詞":
+                return (
+                    scoped_token.category in {"一般"}
+                    and idx < num_tokens - 1
+                    and tokens[idx + 1].pos in {"接尾辞", "動詞"}
+                )
+            case "接頭辞":
+                return (
+                    idx < num_tokens - 1
+                    and tokens[idx + 1].pos in {"名詞", "記号", "形状詞"}
+                    # No line break
+                )
+            case "接尾辞":
+                return (
+                    scoped_token.category in {"名詞的", "形状詞的"}
+                    and idx > 0
+                    and tokens[idx - 1].pos in {"名詞", "形状詞", "動詞", "形容詞", "記号"}
+                )
+            case "助詞":
+                return scoped_token.surface_form == "の"
+            case "記号":
+                return self._regex.match(str(scoped_token)) is not None
+            case "補助記号":
+                scoped_token_str = str(scoped_token)
+                if scoped_token_str not in {"-", "・"}:
+                    return False
+                return (
+                    0 < idx < num_tokens - 1
+                    and self._regex.match(str(tokens[idx - 1])) is not None
+                    and self._regex.match(str(tokens[idx + 1])) is not None
+                )
+            case _:
                 return False
-            return (
-                0 < idx < num_tokens - 1
-                and self._regex.match(str(tokens[idx - 1])) is not None
-                and self._regex.match(str(tokens[idx + 1])) is not None
-            )
-
-        return False
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/base.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta, abstractmethod
-from typing import List, Optional
+
 
 from py_pdf_term.tokenizers import Term
 
 from ..classifiers import (
     BaseTokenClassifier,
     EnglishTokenClassifier,
     JapaneseTokenClassifier,
@@ -20,36 +20,36 @@
     case, "quick sort", "merge sort", and "heap sort" are wrongly concatenated.
 
     This class is used to split a wrongly concatenated term into subterms.
 
     Args
     ----
         classifiers:
-            A list of token classifiers to classify tokens into specific categories.
+            List of token classifiers to classify tokens into specific categories.
             If None, the default classifiers are used. The default classifiers are
             JapaneseTokenClassifier and EnglishTokenClassifier.
     """
 
-    def __init__(self, classifiers: Optional[List[BaseTokenClassifier]] = None) -> None:
+    def __init__(self, classifiers: list[BaseTokenClassifier] | None = None) -> None:
         if classifiers is None:
             classifiers = [
                 JapaneseTokenClassifier(),
                 EnglishTokenClassifier(),
             ]
 
         self._classifiers = classifiers
 
     @abstractmethod
-    def split(self, term: Term) -> List[Term]:
+    def split(self, term: Term) -> list[Term]:
         """Split a wrongly concatenated term.
 
         Args
         ----
             term:
-                A wrongly concatenated term to be split.
+                Wrongly concatenated term to be split.
 
         Returns
         -------
-            List[Term]:
-                A list of split terms.
+            list[Term]:
+                List of split terms.
         """
         raise NotImplementedError(f"{self.__class__.__name__}.split()")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/combiner.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/combiner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-from typing import List, Optional
-
 from py_pdf_term.tokenizers import Term
 
 from .base import BaseSplitter
 from .repeat import RepeatSplitter
 from .symname import SymbolNameSplitter
 
 
 class SplitterCombiner:
-    """A combiner of splitters.
+    """Combiner of splitters.
 
     Args
     ----
         splitters:
-            A list of splitters to split terms. The splitters are applied in order.
+            List of splitters to split terms. The splitters are applied in order.
             If None, the default splitters are used. The default splitters are
             SymbolNameSplitter and RepeatSplitter.
     """
 
-    def __init__(self, splitters: Optional[List[BaseSplitter]] = None) -> None:
+    def __init__(self, splitters: list[BaseSplitter] | None = None) -> None:
         if splitters is None:
             splitters = [SymbolNameSplitter(), RepeatSplitter()]
 
         self._splitters = splitters
 
-    def split(self, term: Term) -> List[Term]:
+    def split(self, term: Term) -> list[Term]:
         """Split a wrongly concatenated term.
 
         Args
         ----
             term:
-                A wrongly concatenated term to be split.
+                Wrongly concatenated term to be split.
 
         Returns
         -------
-            List[Term]:
-                A list of split terms.
+            list[Term]:
+                List of split terms.
         """
 
         splitted_terms = [term]
 
         for splitter in self._splitters:
-            start: List[Term] = []
+            start: list[Term] = []
             splitted_terms = sum(map(splitter.split, splitted_terms), start)
 
         return splitted_terms
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/repeat.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/repeat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-from typing import List, Optional, Tuple
-
 from py_pdf_term.tokenizers import Term
 
 from ..classifiers import BaseTokenClassifier
 from .base import BaseSplitter
 
 
 class RepeatSplitter(BaseSplitter):
-    """A splitter to split a term by repeated tokens. For example, "quick sort merge
+    """Splitter to split a term by repeated tokens. For example, "quick sort merge
     sort heap sort" is split into "quick sort", "merge sort", and "heap sort".
 
     Args
     ----
         classifiers:
-            A list of token classifiers to classify tokens into specific categories.
+            List of token classifiers to classify tokens into specific categories.
             If None, the default classifiers are used. The default classifiers are
             JapaneseTokenClassifier and EnglishTokenClassifier.
     """
 
-    def __init__(self, classifiers: Optional[List[BaseTokenClassifier]] = None) -> None:
+    def __init__(self, classifiers: list[BaseTokenClassifier] | None = None) -> None:
         super().__init__(classifiers=classifiers)
 
-    def split(self, term: Term) -> List[Term]:
+    def split(self, term: Term) -> list[Term]:
         if self._contains_connector_token(term):
             return [term]
 
         head, backward_splitted_terms = self._backward_split(term)
         forward_splitted_terms, center_term = self._forward_split(head)
         return forward_splitted_terms + [center_term] + backward_splitted_terms
 
@@ -38,16 +36,16 @@
                         self._classifiers,
                     )
                 ),
                 term.tokens,
             )
         )
 
-    def _backward_split(self, term: Term) -> Tuple[Term, List[Term]]:
-        splitted_terms: List[Term] = []
+    def _backward_split(self, term: Term) -> tuple[Term, list[Term]]:
+        splitted_terms: list[Term] = []
         head = term.tokens
         fontsize, ncolor, augmented = term.fontsize, term.ncolor, term.augmented
 
         while True:
             head_length = len(head)
             j = head_length
             for i in range(head_length - 1, 0, -1):
@@ -60,16 +58,16 @@
 
             if j == head_length:
                 break
 
         splitted_terms.reverse()
         return Term(head, fontsize, ncolor, augmented), splitted_terms
 
-    def _forward_split(self, term: Term) -> Tuple[List[Term], Term]:
-        splitted_terms: List[Term] = []
+    def _forward_split(self, term: Term) -> tuple[list[Term], Term]:
+        splitted_terms: list[Term] = []
         tail = term.tokens
         fontsize, ncolor, augmented = term.fontsize, term.ncolor, term.augmented
 
         while True:
             tail_length = len(tail)
             i = 0
             for j in range(1, tail_length):
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/symname.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/splitters/symname.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import re
-from typing import List, Optional
+
 
 from py_pdf_term._common.consts import ALPHABET_REGEX, NUMBER_REGEX
 from py_pdf_term.tokenizers import Term
 
 from ..classifiers import BaseTokenClassifier
 from .base import BaseSplitter
 
 
 class SymbolNameSplitter(BaseSplitter):
-    """A splitter to split down a symbol at the end of a term. For example, given
+    """Splitter to split down a symbol at the end of a term. For example, given
     "Programming Language 2", this splitter splits it into "Programming Language" and
     "2", and then "2" is ignored as a meaningless term.
 
     Args
     ----
         classifiers:
-            A list of token classifiers to classify tokens into specific categories.
+            List of token classifiers to classify tokens into specific categories.
             If None, the default classifiers are used. The default classifiers are
             JapaneseTokenClassifier and EnglishTokenClassifier.
     """
 
-    def __init__(self, classifiers: Optional[List[BaseTokenClassifier]] = None) -> None:
+    def __init__(self, classifiers: list[BaseTokenClassifier] | None = None) -> None:
         super().__init__(classifiers=classifiers)
 
-    def split(self, term: Term) -> List[Term]:
+    def split(self, term: Term) -> list[Term]:
         num_tokens = len(term.tokens)
         if num_tokens < 2:
             return [term]
 
         regex = re.compile(rf"{ALPHABET_REGEX}|{NUMBER_REGEX}+|\-")
         last_str = str(term.tokens[-1])
         second_last_str = str(term.tokens[-2])
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/utils.py` & `py_pdf_term-1.0.2/py_pdf_term/candidates/_candidates/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 
 
 def textnode_ncolor(textnode: Element, default: str = str((0.0, 0.0, 0.0))) -> str:
     raw_ncolor = textnode.get("ncolor")
     if raw_ncolor is None:
         return default
 
-    match = re.fullmatch(FLOAT_REGEX, raw_ncolor)
-    if match:
-        color = float(match[0])
+    regex_match = re.fullmatch(FLOAT_REGEX, raw_ncolor)
+    if regex_match:
+        color = float(regex_match[0])
         return str((color, color, color))
 
-    match = re.fullmatch(BRACKET_MONO_REGEX, raw_ncolor)
-    if match:
-        color = float(match[1])
+    regex_match = re.fullmatch(BRACKET_MONO_REGEX, raw_ncolor)
+    if regex_match:
+        color = float(regex_match[1])
         return str((color, color, color))
 
-    match = re.fullmatch(PAREN_MONO_REGEX, raw_ncolor)
-    if match:
-        color = float(match[1])
+    regex_match = re.fullmatch(PAREN_MONO_REGEX, raw_ncolor)
+    if regex_match:
+        color = float(regex_match[1])
         return str((color, color, color))
 
-    match = re.fullmatch(BRACKET_TRI_REGEX, raw_ncolor)
-    if match:
-        color = float(match[1]), float(match[2]), float(match[3])
+    regex_match = re.fullmatch(BRACKET_TRI_REGEX, raw_ncolor)
+    if regex_match:
+        color = float(regex_match[1]), float(regex_match[2]), float(regex_match[3])
         return str(color)
 
-    match = re.fullmatch(PAREN_TRI_REGEX, raw_ncolor)
-    if match:
-        color = float(match[1]), float(match[2]), float(match[3])
+    regex_match = re.fullmatch(PAREN_TRI_REGEX, raw_ncolor)
+    if regex_match:
+        color = float(regex_match[1]), float(regex_match[2]), float(regex_match[3])
         return str(color)
 
     return default
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/__init__.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 from abc import ABCMeta, abstractmethod
-from typing import Union
 
 from py_pdf_term.candidates import PDFCandidateTermList
 
 from ...configs import CandidateLayerConfig
 
 
 class BaseCandidateLayerCache(metaclass=ABCMeta):
     """Base class for candidate layer caches. A candidate layer cache is expected to
     store and load candidate terms per a PDF file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
     @abstractmethod
     def load(
         self, pdf_path: str, config: CandidateLayerConfig
-    ) -> Union[PDFCandidateTermList, None]:
+    ) -> PDFCandidateTermList | None:
         """Load candidate terms from a cache file.
 
         Args
         ----
             pdf_path:
-                The path to a PDF file to load candidate terms.
+                Path to a PDF file to load candidate terms.
             config:
-                The configuration for the candidate layer. The configuration is used to
+                Configuration for the candidate layer. The configuration is used to
                 determine the cache file path.
 
         Returns
         -------
-            Union[PDFCandidateTermList, None]:
-                The loaded candidate terms. If there is no cache file, this method
+            PDFCandidateTermList | None:
+                Loaded candidate terms. If there is no cache file, this method
                 returns None.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.load()")
 
     @abstractmethod
     def store(
         self, candidates: PDFCandidateTermList, config: CandidateLayerConfig
     ) -> None:
         """Store candidate terms to a cache file.
 
         Args
         ----
             candidates:
-                The candidate terms to store.
+                Candidate terms to store.
             config:
-                The configuration for the candidate layer. The configuration is used to
+                Configuration for the candidate layer. The configuration is used to
                 determine the cache file path.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.store()")
 
     @abstractmethod
     def remove(self, pdf_path: str, config: CandidateLayerConfig) -> None:
         """Remove a cache file.
 
         Args
         ----
             pdf_path:
-                The path to a PDF file to remove a cache file.
+                Path to a PDF file to remove a cache file.
             config:
-                The configuration for the candidate layer. The configuration is used to
+                Configuration for the candidate layer. The configuration is used to
                 determine the cache file path.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.remove()")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 import os
 from glob import glob
 from shutil import rmtree
-from typing import Union
 
 from py_pdf_term.candidates import PDFCandidateTermList
 
 from ...configs import CandidateLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_path
 from .base import BaseCandidateLayerCache
 
 
 class CandidateLayerFileCache(BaseCandidateLayerCache):
-    """A candidate layer cache that stores and loads candidate terms to/from a file.
+    """Candidate layer cache that stores and loads candidate terms to/from a file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
     """
 
     def __init__(self, cache_dir: str) -> None:
         super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
         self, pdf_path: str, config: CandidateLayerConfig
-    ) -> Union[PDFCandidateTermList, None]:
+    ) -> PDFCandidateTermList | None:
         dir_name = create_dir_name_from_config(config)
         file_name = create_file_name_from_path(pdf_path, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import Union
-
 from py_pdf_term.candidates import PDFCandidateTermList
 
 from ...configs import CandidateLayerConfig
 from .base import BaseCandidateLayerCache
 
 
 class CandidateLayerNoCache(BaseCandidateLayerCache):
-    """A candidate layer cache that does not store and load candidate terms.
+    """Candidate layer cache that does not store and load candidate terms.
 
     Args
     ----
         cache_dir:
             This argument is ignored.
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
     def load(
         self, pdf_path: str, config: CandidateLayerConfig
-    ) -> Union[PDFCandidateTermList, None]:
+    ) -> PDFCandidateTermList | None:
         pass
 
     def store(
         self, candidates: PDFCandidateTermList, config: CandidateLayerConfig
     ) -> None:
         pass
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/file.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import json
 import os
 from glob import glob
 from shutil import rmtree
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable
 
 from py_pdf_term.methods import MethodTermRanking
 from py_pdf_term.methods._methods.rankingdata import RankingData
 
 from ...configs import BaseMethodLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_paths
 from .base import BaseMethodLayerDataCache, BaseMethodLayerRankingCache
 
 
 class MethodLayerRankingFileCache(BaseMethodLayerRankingCache):
-    """A method layer ranking cache that stores and loads term rankings to/from a file.
+    """Method layer ranking cache that stores and loads term rankings to/from a file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
     """
 
     def __init__(self, cache_dir: str) -> None:
         super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         config: BaseMethodLayerConfig,
-    ) -> Union[MethodTermRanking, None]:
+    ) -> MethodTermRanking | None:
         dir_name = create_dir_name_from_config(config, prefix="rank")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
 
@@ -43,28 +43,28 @@
             except json.JSONDecodeError:
                 return None
 
         return MethodTermRanking.from_dict(obj)
 
     def store(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         term_ranking: MethodTermRanking,
         config: BaseMethodLayerConfig,
     ) -> None:
         dir_name = create_dir_name_from_config(config, prefix="rank")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
 
         with open(cache_file_path, "w") as json_file:
             json.dump(term_ranking.to_dict(), json_file, ensure_ascii=False)
 
-    def remove(self, pdf_paths: List[str], config: BaseMethodLayerConfig) -> None:
+    def remove(self, pdf_paths: list[str], config: BaseMethodLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config, prefix="rank")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_dir_path = os.path.join(self._cache_dir, dir_name)
         cache_file_path = os.path.join(cache_dir_path, file_name)
 
         if not os.path.isfile(cache_file_path):
             return
@@ -73,33 +73,33 @@
 
         cache_file_paths = glob(os.path.join(cache_dir_path, "*.json"))
         if not cache_file_paths:
             rmtree(cache_dir_path)
 
 
 class MethodLayerDataFileCache(BaseMethodLayerDataCache[RankingData]):
-    """A method layer data cache that stores and loads metadata to to generate term
+    """Method layer data cache that stores and loads metadata to to generate term
     rankings to/from a file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
     """
 
     def __init__(self, cache_dir: str) -> None:
         super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         config: BaseMethodLayerConfig,
-        from_dict: Callable[[Dict[str, Any]], RankingData],
-    ) -> Union[RankingData, None]:
+        from_dict: Callable[[dict[str, Any]], RankingData],
+    ) -> RankingData | None:
         dir_name = create_dir_name_from_config(config, prefix="data")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
 
@@ -109,28 +109,28 @@
             except json.JSONDecodeError:
                 return None
 
         return from_dict(obj)
 
     def store(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         ranking_data: RankingData,
         config: BaseMethodLayerConfig,
     ) -> None:
         dir_name = create_dir_name_from_config(config, prefix="data")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
 
         with open(cache_file_path, "w") as json_file:
             json.dump(ranking_data.to_dict(), json_file, ensure_ascii=False)
 
-    def remove(self, pdf_paths: List[str], config: BaseMethodLayerConfig) -> None:
+    def remove(self, pdf_paths: list[str], config: BaseMethodLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config, prefix="data")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_dir_path = os.path.join(self._cache_dir, dir_name)
         cache_file_path = os.path.join(cache_dir_path, file_name)
 
         if not os.path.isfile(cache_file_path):
             return
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from typing import Any, Callable, Dict, List, Union
+from typing import Any, Callable
 
 from py_pdf_term.methods import MethodTermRanking
 from py_pdf_term.methods._methods.rankingdata import RankingData
 
 from ...configs import BaseMethodLayerConfig
 from .base import BaseMethodLayerDataCache, BaseMethodLayerRankingCache
 
 
 class MethodLayerRankingNoCache(BaseMethodLayerRankingCache):
-    """A method layer ranking cache that does not store and load term rankings.
+    """Method layer ranking cache that does not store and load term rankings.
 
     Args
     ----
         cache_dir:
             This argument is ignored.
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
     def load(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         config: BaseMethodLayerConfig,
-    ) -> Union[MethodTermRanking, None]:
+    ) -> MethodTermRanking | None:
         pass
 
     def store(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         term_ranking: MethodTermRanking,
         config: BaseMethodLayerConfig,
     ) -> None:
         pass
 
-    def remove(self, pdf_paths: List[str], config: BaseMethodLayerConfig) -> None:
+    def remove(self, pdf_paths: list[str], config: BaseMethodLayerConfig) -> None:
         pass
 
 
 class MethodLayerDataNoCache(BaseMethodLayerDataCache[RankingData]):
-    """A method layer data cache that does not store and load metadata to generate term
+    """Method layer data cache that does not store and load metadata to generate term
     rankings.
 
     Args
     ----
         cache_dir:
             This argument is ignored.
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
     def load(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         config: BaseMethodLayerConfig,
-        from_dict: Callable[[Dict[str, Any]], RankingData],
-    ) -> Union[RankingData, None]:
+        from_dict: Callable[[dict[str, Any]], RankingData],
+    ) -> RankingData | None:
         pass
 
     def store(
         self,
-        pdf_paths: List[str],
+        pdf_paths: list[str],
         ranking_data: RankingData,
         config: BaseMethodLayerConfig,
     ) -> None:
         pass
 
-    def remove(self, pdf_paths: List[str], config: BaseMethodLayerConfig) -> None:
+    def remove(self, pdf_paths: list[str], config: BaseMethodLayerConfig) -> None:
         pass
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/base.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,76 +1,75 @@
 from abc import ABCMeta, abstractmethod
-from typing import Union
 
 from py_pdf_term.stylings import PDFStylingScoreList
 
 from ...configs import StylingLayerConfig
 
 
 class BaseStylingLayerCache(metaclass=ABCMeta):
     """Base class for styling layer caches. A styling layer cache is expected to store
     and load styling scores per a PDF file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
 
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
     @abstractmethod
     def load(
         self, pdf_path: str, config: StylingLayerConfig
-    ) -> Union[PDFStylingScoreList, None]:
+    ) -> PDFStylingScoreList | None:
         """Load styling scores from a cache file.
 
         Args
         ----
             pdf_path:
-                The path to a PDF file to load styling scores.
+                Path to a PDF file to load styling scores.
             config:
-                The configuration for the styling layer. The configuration is used to
+                Configuration for the styling layer. The configuration is used to
                 determine the cache file path.
 
         Returns
         -------
-            Union[PDFStylingScoreList, None]:
-                The loaded styling scores. If there is no cache file, this method
+            PDFStylingScoreList | None:
+                Loaded styling scores. If there is no cache file, this method
                 returns None.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.load()")
 
     @abstractmethod
     def store(
         self, styling_scores: PDFStylingScoreList, config: StylingLayerConfig
     ) -> None:
         """Store styling scores to a cache file.
 
         Args
         ----
             styling_scores:
-                The styling scores to store.
+                Styling scores to store.
             config:
-                The configuration for the styling layer. The configuration is used to
+                Configuration for the styling layer. The configuration is used to
                 determine the cache file path.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.store()")
 
     @abstractmethod
     def remove(self, pdf_path: str, config: StylingLayerConfig) -> None:
         """Remove a cache file.
 
         Args
         ----
             pdf_path:
-                The path to a PDF file to remove a cache file.
+                Path to a PDF file to remove a cache file.
             config:
-                The configuration for the styling layer. The configuration is used to
+                Configuration for the styling layer. The configuration is used to
                 determine the cache file path.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.remove()")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/file.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import json
 import os
 from glob import glob
 from shutil import rmtree
-from typing import Union
 
 from py_pdf_term.stylings import PDFStylingScoreList
 
 from ...configs import StylingLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_path
 from .base import BaseStylingLayerCache
 
 
 class StylingLayerFileCache(BaseStylingLayerCache):
-    """A styling layer cache that stores and loads styling scores to/from a file.
+    """Styling layer cache that stores and loads styling scores to/from a file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
     """
 
     def __init__(self, cache_dir: str) -> None:
         super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
         self, pdf_path: str, config: StylingLayerConfig
-    ) -> Union[PDFStylingScoreList, None]:
+    ) -> PDFStylingScoreList | None:
         dir_name = create_dir_name_from_config(config)
         file_name = create_file_name_from_path(pdf_path, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import Union
-
 from py_pdf_term.stylings import PDFStylingScoreList
 
 from ...configs import StylingLayerConfig
 from .base import BaseStylingLayerCache
 
 
 class StylingLayerNoCache(BaseStylingLayerCache):
-    """A styling layer cache that does not store and load styling scores.
+    """Styling layer cache that does not store and load styling scores.
 
     Args
     ----
         cache_dir:
             This argument is ignored.
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
     def load(
         self, pdf_path: str, config: StylingLayerConfig
-    ) -> Union[PDFStylingScoreList, None]:
+    ) -> PDFStylingScoreList | None:
         pass
 
     def store(
         self, styling_scores: PDFStylingScoreList, config: StylingLayerConfig
     ) -> None:
         pass
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/base.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 from abc import ABCMeta, abstractmethod
-from typing import Union
 
 from py_pdf_term.pdftoxml import PDFnXMLElement
 
 from ...configs import XMLLayerConfig
 
 
 class BaseXMLLayerCache(metaclass=ABCMeta):
     """Base class for XML layer caches. An XML layer cache is expected to store and
     load XML elements per a PDF file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
     @abstractmethod
-    def load(
-        self, pdf_path: str, config: XMLLayerConfig
-    ) -> Union[PDFnXMLElement, None]:
+    def load(self, pdf_path: str, config: XMLLayerConfig) -> PDFnXMLElement | None:
         """Load XML elements from a cache file.
 
         Args
         ----
             pdf_path:
-                The path to a PDF file to load XML elements.
+                Path to a PDF file to load XML elements.
             config:
-                The configuration for the XML layer. The configuration is used to
+                Configuration for the XML layer. The configuration is used to
                 determine the cache file path.
 
         Returns
         -------
-            Union[PDFnXMLElement, None]:
-                The loaded XML elements. If there is no cache file, this method returns
+            PDFnXMLElement | None:
+                Loaded XML elements. If there is no cache file, this method returns
                 None.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.load()")
 
     @abstractmethod
     def store(self, pdfnxml: PDFnXMLElement, config: XMLLayerConfig) -> None:
         """Store XML elements to a cache file.
 
         Args
         ----
             pdfnxml:
                 The XML elements to store.
             config:
-                The configuration for the XML layer. The configuration is used to
+                Configuration for the XML layer. The configuration is used to
                 determine the cache file path.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.store()")
 
     @abstractmethod
     def remove(self, pdf_path: str, config: XMLLayerConfig) -> None:
         """Remove a cache file.
 
         Args
         ----
             pdf_path:
-                The path to a PDF file to remove a cache file.
+                Path to a PDF file to remove a cache file.
             config:
-                The configuration for the XML layer. The configuration is used to
+                Configuration for the XML layer. The configuration is used to
                 determine the cache file path.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.remove()")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/file.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 from glob import glob
 from shutil import rmtree
-from typing import Union
 from xml.etree.ElementTree import ParseError, fromstring, tostring
 
 from py_pdf_term.pdftoxml import PDFnXMLElement
 
 from ...configs import XMLLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_path
 from .base import BaseXMLLayerCache
@@ -13,23 +12,21 @@
 
 class XMLLayerFileCache(BaseXMLLayerCache):
     """A XML layer cache that stores and loads XML elements to/from a file.
 
     Args
     ----
         cache_dir:
-            The directory path to store cache files.
+            Directory path to store cache files.
     """
 
     def __init__(self, cache_dir: str) -> None:
         self._cache_dir = cache_dir
 
-    def load(
-        self, pdf_path: str, config: XMLLayerConfig
-    ) -> Union[PDFnXMLElement, None]:
+    def load(self, pdf_path: str, config: XMLLayerConfig) -> PDFnXMLElement | None:
         dir_name = create_dir_name_from_config(config)
         file_name = create_file_name_from_path(pdf_path, "xml")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Union
-
 from py_pdf_term.pdftoxml import PDFnXMLElement
 
 from ...configs import XMLLayerConfig
 from .base import BaseXMLLayerCache
 
 
 class XMLLayerNoCache(BaseXMLLayerCache):
@@ -14,17 +12,15 @@
         cache_dir:
             This argument is ignored.
     """
 
     def __init__(self, cache_dir: str) -> None:
         pass
 
-    def load(
-        self, pdf_path: str, config: XMLLayerConfig
-    ) -> Union[PDFnXMLElement, None]:
+    def load(self, pdf_path: str, config: XMLLayerConfig) -> PDFnXMLElement | None:
         pass
 
     def store(self, pdfnxml: PDFnXMLElement, config: XMLLayerConfig) -> None:
         pass
 
     def remove(self, pdf_path: str, config: XMLLayerConfig) -> None:
         pass
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/__init__.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/base.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import asdict, dataclass
-from typing import Any, Dict, Type, TypeVar
+from typing import Any, TypeVar
 
 CACHE_CONFIGS = ["cache", "data_cache", "ranking_cache"]
 
 
 @dataclass(frozen=True)
 class BaseLayerConfig:
     """Base class for layer configuration."""
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return asdict(self)
 
-    def to_dict_without_cache(self) -> Dict[str, Any]:
+    def to_dict_without_cache(self) -> dict[str, Any]:
         config_dict = asdict(self)
         for cache_config in CACHE_CONFIGS:
             config_dict.pop(cache_config, None)
         return config_dict
 
     @classmethod
-    def from_dict(cls: Type["LayerConfig"], obj: Dict[str, Any]) -> "LayerConfig":
+    def from_dict(cls: type["LayerConfig"], obj: dict[str, Any]) -> "LayerConfig":
         return cls(**obj)
 
 
 LayerConfig = TypeVar("LayerConfig", bound=BaseLayerConfig)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/candidate.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/candidate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 from dataclasses import dataclass, field
-from typing import List
 
 from .base import BaseLayerConfig
 
 
 @dataclass(frozen=True)
 class CandidateLayerConfig(BaseLayerConfig):
     """Configuration for candidate layer.
 
     Args
     ----
         lang_tokenizers:
-            a list of language tokenizer class names. The default tokenizers are
+            List of language tokenizer class names. The default tokenizers are
             "py_pdf_term.JapaneseTokenizer" and "py_pdf_term.EnglishTokenizer".
         token_classifiers:
-            a list of token classifier class names. The default classifiers are
+            List of token classifier class names. The default classifiers are
             "py_pdf_term.JapaneseTokenClassifier" and
             "py_pdf_term.EnglishTokenClassifier".
         token_filters:
-            a list of token filter class names. The default filters are
+            List of token filter class names. The default filters are
             "py_pdf_term.JapaneseTokenFilter" and "py_pdf_term.EnglishTokenFilter".
         term_filters:
-            a list of term filter class names. The default filters are
+            List of term filter class names. The default filters are
             "py_pdf_term.JapaneseConcatenationFilter",
             "py_pdf_term.EnglishConcatenationFilter",
             "py_pdf_term.JapaneseSymbolLikeFilter",
             "py_pdf_term.EnglishSymbolLikeFilter",
             "py_pdf_term.JapaneseProperNounFilter",
             "py_pdf_term.EnglishProperNounFilter",
             "py_pdf_term.JapaneseNumericFilter", and
             "py_pdf_term.EnglishNumericFilter".
         splitters:
-            a list of splitter class names. The default splitters are
+            List of splitter class names. The default splitters are
             "py_pdf_term.SymbolNameSplitter" and "py_pdf_term.RepeatSplitter".
         augmenters:
-            a list of augmenter class names. The default augmenters are
+            List of augmenter class names. The default augmenters are
             "py_pdf_term.JapaneseAugmenter" and "py_pdf_term.EnglishAugmenter".
         cache:
-            a cache class name. The default cache is
+            Cache class name. The default cache is
             "py_pdf_term.CandidateLayerFileCache".
     """
 
-    lang_tokenizers: List[str] = field(
+    lang_tokenizers: list[str] = field(
         default_factory=lambda: [
             "py_pdf_term.JapaneseTokenizer",
             "py_pdf_term.EnglishTokenizer",
         ]
     )
-    token_classifiers: List[str] = field(
+    token_classifiers: list[str] = field(
         default_factory=lambda: [
             "py_pdf_term.JapaneseTokenClassifier",
             "py_pdf_term.EnglishTokenClassifier",
         ]
     )
-    token_filters: List[str] = field(
+    token_filters: list[str] = field(
         default_factory=lambda: [
             "py_pdf_term.JapaneseTokenFilter",
             "py_pdf_term.EnglishTokenFilter",
         ]
     )
-    term_filters: List[str] = field(
+    term_filters: list[str] = field(
         default_factory=lambda: [
             "py_pdf_term.JapaneseConcatenationFilter",
             "py_pdf_term.EnglishConcatenationFilter",
             "py_pdf_term.JapaneseSymbolLikeFilter",
             "py_pdf_term.EnglishSymbolLikeFilter",
             "py_pdf_term.JapaneseProperNounFilter",
             "py_pdf_term.EnglishProperNounFilter",
             "py_pdf_term.JapaneseNumericFilter",
             "py_pdf_term.EnglishNumericFilter",
         ]
     )
-    splitters: List[str] = field(
+    splitters: list[str] = field(
         default_factory=lambda: [
             "py_pdf_term.SymbolNameSplitter",
             "py_pdf_term.RepeatSplitter",
         ]
     )
-    augmenters: List[str] = field(
+    augmenters: list[str] = field(
         default_factory=lambda: [
             "py_pdf_term.JapaneseConnectorTermAugmenter",
             "py_pdf_term.EnglishConnectorTermAugmenter",
         ]
     )
     cache: str = "py_pdf_term.CandidateLayerFileCache"
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/method.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/method.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 from dataclasses import dataclass, field
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseLayerConfig
 
 
 @dataclass(frozen=True)
 class BaseMethodLayerConfig(BaseLayerConfig):
     method: str
-    hyper_params: Dict[str, Any] = field(default_factory=dict)
+    hyper_params: dict[str, Any] = field(default_factory=dict)
     ranking_cache: str = "py_pdf_term.MethodLayerRankingFileCache"
     data_cache: str = "py_pdf_term.MethodLayerDataFileCache"
 
 
 @dataclass(frozen=True)
 class SingleDomainMethodLayerConfig(BaseMethodLayerConfig):
     """Configuration for a single-domain method layer.
 
     Args:
         method:
-            a single-domain method class name. The default method is
+            Single-domain method class name. The default method is
             "py_pdf_term.FLRHMethod".
         hyper_params:
-            hyper parameters for the method. The default hyper parameters are
+            Hyper parameters for the method. The default hyper parameters are
             empty.
         ranking_cache:
-            a ranking cache class name. The default cache is
+            Ranking cache class name. The default cache is
             "py_pdf_term.MethodLayerRankingFileCache".
         data_cache:
-            a data cache class name. The default cache is
+            Data cache class name. The default cache is
             "py_pdf_term.MethodLayerDataFileCache".
     """
 
     method: str = "py_pdf_term.FLRHMethod"
 
 
 @dataclass(frozen=True)
 class MultiDomainMethodLayerConfig(BaseMethodLayerConfig):
     """Configuration for a multi-domain method layer.
 
     Args
     ----
         method:
-            a multi-domain method class name. The default method is
+            Multi-domain method class name. The default method is
             "py_pdf_term.TFIDFMethod".
         hyper_params:
-            hyper parameters for the method. The default hyper parameters are
+            Hyper parameters for the method. The default hyper parameters are
             empty.
         ranking_cache:
-            a ranking cache class name. The default cache is
+            Ranking cache class name. The default cache is
             "py_pdf_term.MethodLayerRankingFileCache".
         data_cache:
-            a data cache class name. The default cache is
+            Data cache class name. The default cache is
             "py_pdf_term.MethodLayerDataFileCache".
     """
 
     method: str = "py_pdf_term.TFIDFMethod"
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/styling.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/styling.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from dataclasses import dataclass, field
-from typing import List
 
 from .base import BaseLayerConfig
 
 
 @dataclass(frozen=True)
 class StylingLayerConfig(BaseLayerConfig):
     """Configuration for a styling layer.
 
     Args
     ----
         styling_scores:
-            a list of styling score class names. The default scores are
+            List of styling score class names. The default scores are
             "py_pdf_term.FontsizeScore" and "py_pdf_term.ColorScore".
         cache:
-            a cache class name. The default cache is
+            Cache class name. The default cache is
             "py_pdf_term.StylingLayerFileCache".
     """
 
-    styling_scores: List[str] = field(
+    styling_scores: list[str] = field(
         default_factory=lambda: [
             "py_pdf_term.FontsizeScore",
             "py_pdf_term.ColorScore",
         ]
     )
     cache: str = "py_pdf_term.StylingLayerFileCache"
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/techterm.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/techterm.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 
     Args
     ----
         max_num_terms:
             Maximum number of terms in a page of a PDF file to be extracted. The N-best
             candidates are extracted as technical terms. The default value is 10.
         acceptance_rate:
-            The acceptance rate of the ranking method scores. The candidates whose
+            Acceptance rate of the ranking method scores. The candidates whose
             ranking method scores are lower than the acceptance rate are filtered out
             even if they are in the N-best candidates. The default value is 0.75.
     """
 
     max_num_terms: int = 10
     acceptance_rate: float = 0.75
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/xml.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/configs/xml.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from dataclasses import dataclass
-from typing import Optional
+
 
 from .base import BaseLayerConfig
 
 
 @dataclass(frozen=True)
 class XMLLayerConfig(BaseLayerConfig):
     """Configuration for an XML layer.
 
     Args
     ----
         bin_opener:
-            a binary opener class name. The default opener is
+            Binary opener class name. The default opener is
             "py_pdf_term.StandardBinaryOpener".
         include_pattern:
-            A regular expression pattern of text to include in the output.
+            Regular expression pattern of text to include in the output.
         exclude_pattern:
-            A regular expression pattern of text to exclude from the output (overrides
+            Regular expression pattern of text to exclude from the output (overrides
             include_pattern).
         nfc_norm:
             If True, normalize text to NFC, otherwise keep original.
         cache:
-            a cache class name. The default cache is "py_pdf_term.XMLLayerFileCache".
+            Cache class name. The default cache is "py_pdf_term.XMLLayerFileCache".
     """
 
     bin_opener: str = "py_pdf_term.StandardBinaryOpener"
-    include_pattern: Optional[str] = None
-    exclude_pattern: Optional[str] = None
+    include_pattern: str | None = None
+    exclude_pattern: str | None = None
     nfc_norm: bool = True
     cache: str = "py_pdf_term.XMLLayerFileCache"
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/extractor.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List, Optional
-
 from py_pdf_term.techterms import PDFTechnicalTermList
 
 from .caches import DEFAULT_CACHE_DIR
 from .configs import (
     CandidateLayerConfig,
     MultiDomainMethodLayerConfig,
     SingleDomainMethodLayerConfig,
@@ -133,33 +131,33 @@
         cache_dir:
             Path like string where cache files to be stored. For example, path to a
             local directory, a url or a bucket name of a cloud storage service.
     """
 
     def __init__(
         self,
-        xml_config: Optional[XMLLayerConfig] = None,
-        candidate_config: Optional[CandidateLayerConfig] = None,
-        method_config: Optional[SingleDomainMethodLayerConfig] = None,
-        styling_config: Optional[StylingLayerConfig] = None,
-        techterm_config: Optional[TechnicalTermLayerConfig] = None,
-        bin_opener_mapper: Optional[BinaryOpenerMapper] = None,
-        lang_tokenizer_mapper: Optional[LanguageTokenizerMapper] = None,
-        token_classifier_mapper: Optional[TokenClassifierMapper] = None,
-        token_filter_mapper: Optional[CandidateTokenFilterMapper] = None,
-        term_filter_mapper: Optional[CandidateTermFilterMapper] = None,
-        splitter_mapper: Optional[SplitterMapper] = None,
-        augmenter_mapper: Optional[AugmenterMapper] = None,
-        method_mapper: Optional[SingleDomainRankingMethodMapper] = None,
-        styling_score_mapper: Optional[StylingScoreMapper] = None,
-        xml_cache_mapper: Optional[XMLLayerCacheMapper] = None,
-        candidate_cache_mapper: Optional[CandidateLayerCacheMapper] = None,
-        method_ranking_cache_mapper: Optional[MethodLayerRankingCacheMapper] = None,
-        method_data_cache_mapper: Optional[MethodLayerDataCacheMapper] = None,
-        styling_cache_mapper: Optional[StylingLayerCacheMapper] = None,
+        xml_config: XMLLayerConfig | None = None,
+        candidate_config: CandidateLayerConfig | None = None,
+        method_config: SingleDomainMethodLayerConfig | None = None,
+        styling_config: StylingLayerConfig | None = None,
+        techterm_config: TechnicalTermLayerConfig | None = None,
+        bin_opener_mapper: BinaryOpenerMapper | None = None,
+        lang_tokenizer_mapper: LanguageTokenizerMapper | None = None,
+        token_classifier_mapper: TokenClassifierMapper | None = None,
+        token_filter_mapper: CandidateTokenFilterMapper | None = None,
+        term_filter_mapper: CandidateTermFilterMapper | None = None,
+        splitter_mapper: SplitterMapper | None = None,
+        augmenter_mapper: AugmenterMapper | None = None,
+        method_mapper: SingleDomainRankingMethodMapper | None = None,
+        styling_score_mapper: StylingScoreMapper | None = None,
+        xml_cache_mapper: XMLLayerCacheMapper | None = None,
+        candidate_cache_mapper: CandidateLayerCacheMapper | None = None,
+        method_ranking_cache_mapper: MethodLayerRankingCacheMapper | None = None,
+        method_data_cache_mapper: MethodLayerDataCacheMapper | None = None,
+        styling_cache_mapper: StylingLayerCacheMapper | None = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         xml_layer = XMLLayer(
             config=xml_config,
             bin_opener_mapper=bin_opener_mapper,
             cache_mapper=xml_cache_mapper,
             cache_dir=cache_dir,
@@ -324,33 +322,33 @@
         cache_dir:
             Path like string where cache files to be stored. For example, path to a
             local directory, a url or a bucket name of a cloud storage service.
     """
 
     def __init__(
         self,
-        xml_config: Optional[XMLLayerConfig] = None,
-        candidate_config: Optional[CandidateLayerConfig] = None,
-        method_config: Optional[MultiDomainMethodLayerConfig] = None,
-        styling_config: Optional[StylingLayerConfig] = None,
-        techterm_config: Optional[TechnicalTermLayerConfig] = None,
-        bin_opener_mapper: Optional[BinaryOpenerMapper] = None,
-        lang_tokenizer_mapper: Optional[LanguageTokenizerMapper] = None,
-        token_classifier_mapper: Optional[TokenClassifierMapper] = None,
-        token_filter_mapper: Optional[CandidateTokenFilterMapper] = None,
-        term_filter_mapper: Optional[CandidateTermFilterMapper] = None,
-        splitter_mapper: Optional[SplitterMapper] = None,
-        augmenter_mapper: Optional[AugmenterMapper] = None,
-        method_mapper: Optional[MultiDomainRankingMethodMapper] = None,
-        styling_score_mapper: Optional[StylingScoreMapper] = None,
-        xml_cache_mapper: Optional[XMLLayerCacheMapper] = None,
-        candidate_cache_mapper: Optional[CandidateLayerCacheMapper] = None,
-        method_ranking_cache_mapper: Optional[MethodLayerRankingCacheMapper] = None,
-        method_data_cache_mapper: Optional[MethodLayerDataCacheMapper] = None,
-        styling_cache_mapper: Optional[StylingLayerCacheMapper] = None,
+        xml_config: XMLLayerConfig | None = None,
+        candidate_config: CandidateLayerConfig | None = None,
+        method_config: MultiDomainMethodLayerConfig | None = None,
+        styling_config: StylingLayerConfig | None = None,
+        techterm_config: TechnicalTermLayerConfig | None = None,
+        bin_opener_mapper: BinaryOpenerMapper | None = None,
+        lang_tokenizer_mapper: LanguageTokenizerMapper | None = None,
+        token_classifier_mapper: TokenClassifierMapper | None = None,
+        token_filter_mapper: CandidateTokenFilterMapper | None = None,
+        term_filter_mapper: CandidateTermFilterMapper | None = None,
+        splitter_mapper: SplitterMapper | None = None,
+        augmenter_mapper: AugmenterMapper | None = None,
+        method_mapper: MultiDomainRankingMethodMapper | None = None,
+        styling_score_mapper: StylingScoreMapper | None = None,
+        xml_cache_mapper: XMLLayerCacheMapper | None = None,
+        candidate_cache_mapper: CandidateLayerCacheMapper | None = None,
+        method_ranking_cache_mapper: MethodLayerRankingCacheMapper | None = None,
+        method_data_cache_mapper: MethodLayerDataCacheMapper | None = None,
+        styling_cache_mapper: StylingLayerCacheMapper | None = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         xml_layer = XMLLayer(
             config=xml_config,
             bin_opener_mapper=bin_opener_mapper,
             cache_mapper=xml_cache_mapper,
             cache_dir=cache_dir,
@@ -388,15 +386,15 @@
             styling_layer=styling_layer,
             config=techterm_config,
         )
 
         self._techterm_layer = techterm_layer
 
     def extract(
-        self, domain: str, pdf_path: str, multi_domain_pdfs: List[DomainPDFList]
+        self, domain: str, pdf_path: str, multi_domain_pdfs: list[DomainPDFList]
     ) -> PDFTechnicalTermList:
         """Extract technical terms from a PDF file.
 
         Args
         ----
             domain:
                 Domain name which the input PDF file belongs to. This may be the name of
@@ -419,15 +417,15 @@
 
         pdf_techterms = self._techterm_layer.create_pdf_techterms(
             domain, pdf_path, multi_domain_pdfs
         )
         return pdf_techterms
 
     def _validate(
-        self, domain: str, pdf_path: str, multi_domain_pdfs: List[DomainPDFList]
+        self, domain: str, pdf_path: str, multi_domain_pdfs: list[DomainPDFList]
     ) -> None:
         if domain == "":
             raise ValueError("domain name must not be empty")
 
         if len(multi_domain_pdfs) < 2:
             raise ValueError("multi_domain_pdfs must have at least two elements")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/candidate.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/candidate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List, Optional
-
 from py_pdf_term.candidates import (
     CandidateTermExtractor,
     DomainCandidateTermList,
     PDFCandidateTermList,
 )
 
 from ..caches import DEFAULT_CACHE_DIR
@@ -18,59 +16,59 @@
     SplitterMapper,
     TokenClassifierMapper,
 )
 from .xml import XMLLayer
 
 
 class CandidateLayer:
-    """A layer to extract candidate terms using XMLLayer.
+    """Layer to extract candidate terms using XMLLayer.
 
     Args
     ----
         xml_layer:
-            a layer to create textful XML elements from a PDF file.
+            Layer to create textful XML elements from a PDF file.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
         lang_tokenizer_mapper:
-            a mapper to find language tokenizer classes from configuration. If None, the
+            Mapper to find language tokenizer classes from configuration. If None, the
             default mapper is used.
         token_classifier_mapper:
-            a mapper to find token classifier classes from configuration. If None, the
+            Mapper to find token classifier classes from configuration. If None, the
             default mapper is used.
         token_filter_mapper:
-            a mapper to find token filter classes from configuration. If None, the
+            Mapper to find token filter classes from configuration. If None, the
             default mapper is used.
         term_filter_mapper:
-            a mapper to find term filter classes from configuration. If None, the
+            Mapper to find term filter classes from configuration. If None, the
             default mapper is used.
         splitter_mapper:
-            a mapper to find splitter classes from configuration. If None, the default
+            Mapper to find splitter classes from configuration. If None, the default
             mapper is used.
         augmenter_mapper:
-            a mapper to find augmenter classes from configuration. If None, the default
+            Mapper to find augmenter classes from configuration. If None, the default
             mapper is used.
         cache_mapper:
-            a mapper to find cache class from configuration. If None, the default mapper
+            Mapper to find cache class from configuration. If None, the default mapper
             is used.
         cache_dir:
-            a directory path to store cache files. If None, the default directory is
+            Directory path to store cache files. If None, the default directory is
             used.
     """
 
     def __init__(
         self,
         xml_layer: XMLLayer,
-        config: Optional[CandidateLayerConfig] = None,
-        lang_tokenizer_mapper: Optional[LanguageTokenizerMapper] = None,
-        token_classifier_mapper: Optional[TokenClassifierMapper] = None,
-        token_filter_mapper: Optional[CandidateTokenFilterMapper] = None,
-        term_filter_mapper: Optional[CandidateTermFilterMapper] = None,
-        splitter_mapper: Optional[SplitterMapper] = None,
-        augmenter_mapper: Optional[AugmenterMapper] = None,
-        cache_mapper: Optional[CandidateLayerCacheMapper] = None,
+        config: CandidateLayerConfig | None = None,
+        lang_tokenizer_mapper: LanguageTokenizerMapper | None = None,
+        token_classifier_mapper: TokenClassifierMapper | None = None,
+        token_filter_mapper: CandidateTokenFilterMapper | None = None,
+        term_filter_mapper: CandidateTermFilterMapper | None = None,
+        splitter_mapper: SplitterMapper | None = None,
+        augmenter_mapper: AugmenterMapper | None = None,
+        cache_mapper: CandidateLayerCacheMapper | None = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         if config is None:
             config = CandidateLayerConfig()
         if lang_tokenizer_mapper is None:
             lang_tokenizer_mapper = LanguageTokenizerMapper.default_mapper()
         if token_classifier_mapper is None:
@@ -111,41 +109,41 @@
         self, domain_pdfs: DomainPDFList
     ) -> DomainCandidateTermList:
         """Create candidate term list from a list of PDF files in a domain.
 
         Args
         ----
             domain_pdfs:
-                a list of PDF files in a domain.
+                List of PDF files in a domain.
 
         Returns
         -------
             DomainCandidateTermList:
-                a list of candidate terms in a domain.
+                List of candidate terms in a domain.
         """
 
-        pdf_candidates_list: List[PDFCandidateTermList] = []
+        pdf_candidates_list: list[PDFCandidateTermList] = []
         for pdf_path in domain_pdfs.pdf_paths:
             pdf_candidates = self.create_pdf_candidates(pdf_path)
             pdf_candidates_list.append(pdf_candidates)
 
         return DomainCandidateTermList(domain_pdfs.domain, pdf_candidates_list)
 
     def create_pdf_candidates(self, pdf_path: str) -> PDFCandidateTermList:
         """Create candidate term list from a PDF file.
 
         Args
         ----
             pdf_path:
-                a path to a PDF file.
+                Path to a PDF file.
 
         Returns
         -------
             PDFCandidateTermList:
-                a list of candidate terms in a PDF file.
+                List of candidate terms in a PDF file.
         """
 
         pdf_candidates = self._cache.load(pdf_path, self._config)
 
         if pdf_candidates is None:
             pdfnxml = self._xml_layer.create_pdfnxml(pdf_path)
             pdf_candidates = self._extractor.extract_from_xml_element(pdfnxml)
@@ -156,11 +154,11 @@
 
     def remove_cache(self, pdf_path: str) -> None:
         """Remove a cache file for a PDF file.
 
         Args
         ----
             pdf_path:
-                a path to a PDF file to remove a cache file.
+                Path to a PDF file to remove a cache file.
         """
 
         self._cache.remove(pdf_path, self._config)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/method.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/method.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta
-from typing import Any, List, Optional
+from typing import Any
 
 from py_pdf_term.candidates import DomainCandidateTermList
 from py_pdf_term.methods import MethodTermRanking
 
 from ..caches import DEFAULT_CACHE_DIR
 from ..configs import (
     BaseMethodLayerConfig,
@@ -23,34 +23,34 @@
 class BaseMethodLayer(metaclass=ABCMeta):
     """Base class for method layers to calculate term ranking from candidate terms
     using candidate layer.
 
     Args
     ----
         candidate_layer:
-            a layer to extract candidate terms.
+            Layer to extract candidate terms.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
         ranking_cache_mapper:
-            a mapper to find ranking cache classes from configuration. If None, the
+            Mapper to find ranking cache classes from configuration. If None, the
             default mapper is used.
         data_cache_mapper:
-            a mapper to find data cache classes from configuration. If None, the default
+            Mapper to find data cache classes from configuration. If None, the default
             mapper is used.
         cache_dir:
-            a directory path to store cache files. If None, the default directory is
+            Directory path to store cache files. If None, the default directory is
             used.
     """
 
     def __init__(
         self,
         candidate_layer: CandidateLayer,
         config: BaseMethodLayerConfig,
-        ranking_cache_mapper: Optional[MethodLayerRankingCacheMapper],
-        data_cache_mapper: Optional[MethodLayerDataCacheMapper],
+        ranking_cache_mapper: MethodLayerRankingCacheMapper | None,
+        data_cache_mapper: MethodLayerDataCacheMapper | None,
         cache_dir: str,
     ) -> None:
         if ranking_cache_mapper is None:
             ranking_cache_mapper = MethodLayerRankingCacheMapper.default_mapper()
         if data_cache_mapper is None:
             data_cache_mapper = MethodLayerDataCacheMapper.default_mapper()
 
@@ -59,58 +59,58 @@
 
         self._ranking_cache = ranking_cache_cls(cache_dir=cache_dir)
         self._data_cache = data_cache_cls(cache_dir=cache_dir)
         self._config = config
 
         self._candidate_layer = candidate_layer
 
-    def remove_cache(self, pdf_paths: List[str]) -> None:
+    def remove_cache(self, pdf_paths: list[str]) -> None:
         """Remove cache file for given PDF paths in a domain.
 
         Args
         ----
             pdf_paths:
-                a list of PDF paths in a domain to remove a cache file.
+                List of PDF paths in a domain to remove a cache file.
         """
 
         self._ranking_cache.remove(pdf_paths, self._config)
         self._data_cache.remove(pdf_paths, self._config)
 
 
 class SingleDomainMethodLayer(BaseMethodLayer):
-    """A method layer to calculate term ranking with an algorithm which does not require
+    """Method layer to calculate term ranking with an algorithm which does not require
     cross-domain information using candidate terms.
 
     Args
     ----
         candidate_layer:
-            a layer to extract candidate terms.
+            Layer to extract candidate terms.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
         method_mapper:
-            a mapper to find ranking method classes from configuration. If None, the
+            Mapper to find ranking method classes from configuration. If None, the
             default mapper is used.
         ranking_cache_mapper:
-            a mapper to find ranking cache classes from configuration. If None, the
+            Mapper to find ranking cache classes from configuration. If None, the
             default mapper is used.
         data_cache_mapper:
-            a mapper to find data cache classes from configuration. If None, the default
+            Mapper to find data cache classes from configuration. If None, the default
             mapper is used.
         cache_dir:
-            a directory path to store cache files. If None, the default directory is
+            Directory path to store cache files. If None, the default directory is
             used.
     """
 
     def __init__(
         self,
         candidate_layer: CandidateLayer,
-        config: Optional[SingleDomainMethodLayerConfig] = None,
-        method_mapper: Optional[SingleDomainRankingMethodMapper] = None,
-        ranking_cache_mapper: Optional[MethodLayerRankingCacheMapper] = None,
-        data_cache_mapper: Optional[MethodLayerDataCacheMapper] = None,
+        config: SingleDomainMethodLayerConfig | None = None,
+        method_mapper: SingleDomainRankingMethodMapper | None = None,
+        ranking_cache_mapper: MethodLayerRankingCacheMapper | None = None,
+        data_cache_mapper: MethodLayerDataCacheMapper | None = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         if config is None:
             config = SingleDomainMethodLayerConfig()
         if method_mapper is None:
             method_mapper = SingleDomainRankingMethodMapper.default_mapper()
 
@@ -123,20 +123,20 @@
 
     def create_term_ranking(self, domain_pdfs: DomainPDFList) -> MethodTermRanking:
         """Create term ranking from candidate terms in a domain.
 
         Args
         ----
             domain_pdfs:
-                a list of PDFs in a domain to extract term ranking.
+                List of PDFs in a domain to extract term ranking.
 
         Returns
         -------
             MethodTermRanking:
-                a term ranking costructed from candidate terms.
+                Term ranking costructed from candidate terms.
         """
 
         term_ranking = self._ranking_cache.load(domain_pdfs.pdf_paths, self._config)
 
         if term_ranking is None:
             candidates = self._candidate_layer.create_domain_candidates(domain_pdfs)
             ranking_data = self._create_ranking_data(domain_pdfs, candidates)
@@ -160,44 +160,44 @@
 
         self._data_cache.store(domain_pdfs.pdf_paths, ranking_data, self._config)
 
         return ranking_data
 
 
 class MultiDomainMethodLayer(BaseMethodLayer):
-    """A method layer to calculate term ranking with an algorithm which requires
+    """Method layer to calculate term ranking with an algorithm which requires
     cross-domain information using candidate terms.
 
     Args
     ----
         candidate_layer:
-            a layer to extract candidate terms.
+            Layer to extract candidate terms.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
         method_mapper:
-            a mapper to find ranking method classes from configuration. If None, the
+            Mapper to find ranking method classes from configuration. If None, the
             default mapper is used.
         ranking_cache_mapper:
-            a mapper to find ranking cache classes from configuration. If None, the
+            Mapper to find ranking cache classes from configuration. If None, the
             default mapper is used.
         data_cache_mapper:
-            a mapper to find data cache classes from configuration. If None, the default
+            Mapper to find data cache classes from configuration. If None, the default
             mapper is used.
         cache_dir:
-            a directory path to store cache files. If None, the default directory is
+            Directory path to store cache files. If None, the default directory is
             used.
     """
 
     def __init__(
         self,
         candidate_layer: CandidateLayer,
-        config: Optional[MultiDomainMethodLayerConfig] = None,
-        method_mapper: Optional[MultiDomainRankingMethodMapper] = None,
-        ranking_cache_mapper: Optional[MethodLayerRankingCacheMapper] = None,
-        data_cache_mapper: Optional[MethodLayerDataCacheMapper] = None,
+        config: MultiDomainMethodLayerConfig | None = None,
+        method_mapper: MultiDomainRankingMethodMapper | None = None,
+        ranking_cache_mapper: MethodLayerRankingCacheMapper | None = None,
+        data_cache_mapper: MethodLayerDataCacheMapper | None = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         if config is None:
             config = MultiDomainMethodLayerConfig()
         if method_mapper is None:
             method_mapper = MultiDomainRankingMethodMapper.default_mapper()
 
@@ -207,44 +207,44 @@
 
         method_cls = method_mapper.find(config.method)
         self._method = method_cls(**config.hyper_params)
 
     def create_term_ranking(
         self,
         domain: str,
-        multi_domain_pdfs: List[DomainPDFList],
+        multi_domain_pdfs: list[DomainPDFList],
     ) -> MethodTermRanking:
         """Create term ranking from candidate terms in a domain.
 
         Args
         ----
             domain:
-                a domain to construct term ranking.
+                Domain to construct term ranking.
             multi_domain_pdfs:
-                a list of PDFs in each domain.
+                List of PDFs in each domain.
 
         Returns
         -------
             MethodTermRanking:
-                a term ranking costructed from candidate terms in the given domain.
+                Term ranking costructed from candidate terms in the given domain.
         """
 
         target_domain_pdfs = next(
             filter(lambda item: item.domain == domain, multi_domain_pdfs), None
         )
         if target_domain_pdfs is None:
             raise ValueError(f"'multi_domain_pdfs' does not contain domain '{domain}'")
 
         term_ranking = self._ranking_cache.load(
             target_domain_pdfs.pdf_paths, self._config
         )
 
         if term_ranking is None:
-            domain_candidates_list: List[DomainCandidateTermList] = []
-            ranking_data_list: List[Any] = []
+            domain_candidates_list: list[DomainCandidateTermList] = []
+            ranking_data_list: list[Any] = []
             for domain_pdfs in multi_domain_pdfs:
                 candidates = self._candidate_layer.create_domain_candidates(domain_pdfs)
                 ranking_data = self._create_ranking_data(domain_pdfs, candidates)
                 domain_candidates_list.append(candidates)
                 ranking_data_list.append(ranking_data)
 
             term_ranking = self._method.rank_domain_terms(
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/styling.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/styling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
-from typing import Optional
-
 from py_pdf_term.stylings import PDFStylingScoreList, StylingScorer
 
 from ..caches import DEFAULT_CACHE_DIR
 from ..configs import StylingLayerConfig
 from ..mappers import StylingLayerCacheMapper, StylingScoreMapper
 from .candidate import CandidateLayer
 
 
 class StylingLayer:
-    """A layer to calclate styling scores from a PDF file using candidate layer.
+    """Layer to calclate styling scores from a PDF file using candidate layer.
 
     Args
     ----
         candidate_layer:
-            a layer to extract candidate terms.
+            Layer to extract candidate terms.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
         styling_score_mapper:
-            a mapper to find styling score classes from configuration. If None, the
+            Mapper to find styling score classes from configuration. If None, the
             default mapper is used.
         cache_mapper:
-            a mapper to find cache class from configuration. If None, the default mapper
+            Mapper to find cache class from configuration. If None, the default mapper
             is used.
 
     """
 
     def __init__(
         self,
         candidate_layer: CandidateLayer,
-        config: Optional[StylingLayerConfig] = None,
-        styling_score_mapper: Optional[StylingScoreMapper] = None,
-        cache_mapper: Optional[StylingLayerCacheMapper] = None,
+        config: StylingLayerConfig | None = None,
+        styling_score_mapper: StylingScoreMapper | None = None,
+        cache_mapper: StylingLayerCacheMapper | None = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         if config is None:
             config = StylingLayerConfig()
         if styling_score_mapper is None:
             styling_score_mapper = StylingScoreMapper.default_mapper()
         if cache_mapper is None:
@@ -52,20 +50,20 @@
 
     def create_pdf_styling_scores(self, pdf_path: str) -> PDFStylingScoreList:
         """Create style score list from a PDF file.
 
         Args
         ----
             pdf_path:
-                a PDF file path to calculate styling scores.
+                PDF file path to calculate styling scores.
 
         Returns
         -------
             PDFStylingScoreList:
-                a list of styling scores for each page in the PDF file.
+                List of styling scores for each page in the PDF file.
         """
 
         styling_scores = self._cache.load(pdf_path, self._config)
 
         if styling_scores is None:
             pdf_candidates = self._candidate_layer.create_pdf_candidates(pdf_path)
             styling_scores = self._scorer.score_pdf_candidates(pdf_candidates)
@@ -76,11 +74,11 @@
 
     def remove_cache(self, pdf_path: str) -> None:
         """Remove a cache file for a PDF file.
 
         Args
         ----
             pdf_path:
-                a PDF file path to remove a cache file.
+                PDF file path to remove a cache file.
         """
 
         self._cache.remove(pdf_path, self._config)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/techterm.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/techterm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta
-from typing import List, Optional
+
 
 from py_pdf_term.techterms import PDFTechnicalTermList, TechnicalTermExtractor
 
 from ..configs import TechnicalTermLayerConfig
 from ..data import DomainPDFList
 from .candidate import CandidateLayer
 from .method import MultiDomainMethodLayer, SingleDomainMethodLayer
@@ -13,26 +13,26 @@
 class BaseTechnicalTermLayer(metaclass=ABCMeta):
     """Base class for technical term layers to extract technical terms from candidate
     terms using candidate layer and styling layer.
 
     Args
     ----
         candidate_layer:
-            a layer to extract candidate terms.
+            Layer to extract candidate terms.
         styling_layer:
-            a layer to calculate styling scores.
+            Layer to calculate styling scores.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
     """
 
     def __init__(
         self,
         candidate_layer: CandidateLayer,
         styling_layer: StylingLayer,
-        config: Optional[TechnicalTermLayerConfig] = None,
+        config: TechnicalTermLayerConfig | None = None,
     ) -> None:
         if config is None:
             config = TechnicalTermLayerConfig()
 
         self._techterm = TechnicalTermExtractor(
             max_num_terms=config.max_num_terms,
             acceptance_rate=config.acceptance_rate,
@@ -40,116 +40,116 @@
         self._config = config
 
         self._candidate_layer = candidate_layer
         self._styling_layer = styling_layer
 
 
 class SingleDomainTechnicalTermLayer(BaseTechnicalTermLayer):
-    """A technical term layer to extract technical terms from candidate terms using
+    """Technical term layer to extract technical terms from candidate terms using
     candidate layer, single domain method layer and styling layer.
 
     Args
     ----
         candidate_layer:
-            a layer to extract candidate terms.
+            Layer to extract candidate terms.
         method_layer:
-            a layer to calculate term ranking which does not require cross-domain
+            Layer to calculate term ranking which does not require cross-domain
             information.
         styling_layer:
-            a layer to calculate styling scores.
+            Layer to calculate styling scores.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
     """
 
     def __init__(
         self,
         candidate_layer: CandidateLayer,
         method_layer: SingleDomainMethodLayer,
         styling_layer: StylingLayer,
-        config: Optional[TechnicalTermLayerConfig] = None,
+        config: TechnicalTermLayerConfig | None = None,
     ) -> None:
         super().__init__(candidate_layer, styling_layer, config)
 
         self._method_layer = method_layer
 
     def create_pdf_techterms(
         self, pdf_path: str, domain_pdfs: DomainPDFList
     ) -> PDFTechnicalTermList:
         """Extract technical terms from a PDF file in a domain.
 
         Args
         ----
             pdf_path:
-                a PDF path to extract technical terms.
+                PDF path to extract technical terms.
             domain_pdfs:
-                a list of PDF paths in a domain. This is used to calculate term ranking.
+                List of PDF paths in a domain. This is used to calculate term ranking.
                 This must contain the PDF path to extract technical terms.
 
         Returns
         -------
             PDFTechnicalTermList:
-                a list of technical terms extracted from the PDF file.
+                List of technical terms extracted from the PDF file.
         """
 
         pdf_candidates = self._candidate_layer.create_pdf_candidates(pdf_path)
         term_ranking = self._method_layer.create_term_ranking(domain_pdfs)
         pdf_styling_scores = self._styling_layer.create_pdf_styling_scores(pdf_path)
         techterms = self._techterm.extract_from_pdf(
             pdf_candidates, term_ranking, pdf_styling_scores
         )
 
         return techterms
 
 
 class MultiDomainTechnicalTermLayer(BaseTechnicalTermLayer):
-    """A technical term layer to extract technical terms from candidate terms using
+    """Technical term layer to extract technical terms from candidate terms using
     candidate layer, multi domain method layer and styling layer.
 
     Args
     ----
         candidate_layer:
-            a layer to extract candidate terms.
+            Layer to extract candidate terms.
         method_layer:
-            a layer to calculate term ranking which requires cross-domain information.
+            Layer to calculate term ranking which requires cross-domain information.
         styling_layer:
-            a layer to calculate styling scores.
+            Layer to calculate styling scores.
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
     """
 
     def __init__(
         self,
         candidate_layer: CandidateLayer,
         method_layer: MultiDomainMethodLayer,
         styling_layer: StylingLayer,
-        config: Optional[TechnicalTermLayerConfig] = None,
+        config: TechnicalTermLayerConfig | None = None,
     ) -> None:
         super().__init__(candidate_layer, styling_layer, config)
 
         self._method_layer = method_layer
 
     def create_pdf_techterms(
-        self, domain: str, pdf_path: str, multi_domain_pdfs: List[DomainPDFList]
+        self, domain: str, pdf_path: str, multi_domain_pdfs: list[DomainPDFList]
     ) -> PDFTechnicalTermList:
         """Extract technical terms from a PDF file in a domain.
 
         Args
         ----
             domain:
-                a domain to extract technical terms.
+                Domain to extract technical terms.
             pdf_path:
-                a PDF path to extract technical terms. This PDF file is in the domain.
+                PDF path to extract technical terms. This PDF file is in the domain.
             multi_domain_pdfs:
-                a list of PDF paths in each domain. The PDF file in the domain must be
+                List of PDF paths in each domain. The PDF file in the domain must be
                 included in this list.
 
         Returns
         -------
             PDFTechnicalTermList:
-                a list of technical terms extracted from the PDF file.
+                List of technical terms extracted from the PDF file.
         """
 
         pdf_candidates = self._candidate_layer.create_pdf_candidates(pdf_path)
         term_ranking = self._method_layer.create_term_ranking(domain, multi_domain_pdfs)
         pdf_styling_scores = self._styling_layer.create_pdf_styling_scores(pdf_path)
         techterms = self._techterm.extract_from_pdf(
             pdf_candidates, term_ranking, pdf_styling_scores
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/xml.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/layers/xml.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from typing import Optional
-
 from py_pdf_term.pdftoxml import PDFnXMLElement, PDFtoXMLConverter
 
 from ..caches import DEFAULT_CACHE_DIR
 from ..configs import XMLLayerConfig
 from ..mappers import BinaryOpenerMapper, XMLLayerCacheMapper
 
 
 class XMLLayer:
-    """A layer to create textful XML elements from a PDF file.
+    """Layer to create textful XML elements from a PDF file.
 
     Args
     ----
         config:
-            a configuration for this layer. If None, the default configuration is used.
+            Configuration for this layer. If None, the default configuration is used.
         bin_opener_mapper:
-            a mapper to find binary opener classes from configuration. If None, the
+            Mapper to find binary opener classes from configuration. If None, the
             default mapper is used.
         cache_mapper:
-            a mapper to find cache class from configuration. If None, the default mapper
+            Mapper to find cache class from configuration. If None, the default mapper
             is used.
         cache_dir:
-            a directory path to store cache files. If None, the default directory is
+            Directory path to store cache files. If None, the default directory is
             used.
     """
 
     def __init__(
         self,
-        config: Optional[XMLLayerConfig] = None,
-        bin_opener_mapper: Optional[BinaryOpenerMapper] = None,
-        cache_mapper: Optional[XMLLayerCacheMapper] = None,
+        config: XMLLayerConfig | None = None,
+        bin_opener_mapper: BinaryOpenerMapper | None = None,
+        cache_mapper: XMLLayerCacheMapper | None = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         if config is None:
             config = XMLLayerConfig()
         if bin_opener_mapper is None:
             bin_opener_mapper = BinaryOpenerMapper.default_mapper()
         if cache_mapper is None:
@@ -49,19 +47,19 @@
 
     def create_pdfnxml(self, pdf_path: str) -> PDFnXMLElement:
         """Create a PDFnXMLElement from a PDF file.
 
         Args
         ----
             pdf_path:
-                a path to a PDF file.
+                Path to a PDF file.
 
         Returns
         -------
-            a PDFnXMLElement created from the PDF file.
+            PDFnXMLElement created from the PDF file.
         """
 
         pdfnxml = None
         pdfnxml = self._cache.load(pdf_path, self._config)
 
         if pdfnxml is None:
             pdfnxml = self._converter.convert_as_element(
@@ -77,11 +75,11 @@
 
     def remove_cache(self, pdf_path: str) -> None:
         """Remove a cache file for a PDF file.
 
         Args
         ----
             pdf_path:
-                a path to a PDF file.
+                Path to a PDF file.
         """
 
         self._cache.remove(pdf_path, self._config)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/__init__.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/base.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from typing import Dict, Generic, List, TypeVar, Union
+from typing import Generic, TypeVar
 
 MappedValue = TypeVar("MappedValue")
 
 
 class BaseMapper(Generic[MappedValue], metaclass=ABCMeta):
     """Base class for mappers to find mapped values from names."""
 
     def __init__(self) -> None:
-        self._map: Dict[str, MappedValue] = dict()
+        self._map: dict[str, MappedValue] = dict()
 
     def add(self, name: str, value: MappedValue) -> None:
         """Add a new mapping from name to value.
 
         Args
         ----
             name:
-                a name to find the mapped value.
+                Name to find the mapped value.
             value:
-                a mapped value to be found from the name.
+                Mapped value to be found from the name.
         """
 
         self._map[name] = value
 
     def remove(self, name: str) -> None:
         """Remove a mapping from name to value.
 
         Args
         ----
             name:
-                a name to remove the mapped value.
+                Name to remove the mapped value.
         """
 
         del self._map[name]
 
     def find(self, name: str) -> MappedValue:
         """Find a mapped value from name. If not found, raise KeyError.
 
         Args
         ----
             name:
-                a name to find the mapped value.
+                Name to find the mapped value.
 
         Returns
         -------
-            a mapped value found from the name.
+            Mapped value found from the name.
         """
 
         return self._map[name]
 
-    def find_or_none(self, name: str) -> Union[MappedValue, None]:
+    def find_or_none(self, name: str) -> MappedValue | None:
         """Find a mapped value from name. If not found, return None.
 
 
         Args
         ----
             name:
-                a name to find the mapped value.
+                Name to find the mapped value.
 
         Returns
         -------
-            a mapped value found from the name. None if not found.
+            Mapped value found from the name. None if not found.
         """
 
         return self._map.get(name)
 
-    def bulk_find(self, names: List[str]) -> List[MappedValue]:
+    def bulk_find(self, names: list[str]) -> list[MappedValue]:
         """Find mapped values from names. If there is no mapped value for a name, raise
         KeyError.
 
         Args
         ----
             names:
-                names to find the mapped values.
+                Names to find the mapped values.
 
         Returns
         -------
-            mapped values found from the names. The order of the mapped values is the
+            Mapped values found from the names. The order of the mapped values is the
             same as the order of the names.
         """
 
         return list(map(lambda name: self._map[name], names))
 
-    def bulk_find_or_none(self, names: List[str]) -> List[Union[MappedValue, None]]:
+    def bulk_find_or_none(self, names: list[str]) -> list[MappedValue | None]:
         """Find mapped values from names. If there is no mapped value for a name, return
         None.
 
         Args
         ----
             names:
-                names to find the mapped values.
+                Names to find the mapped values.
 
         Returns
         -------
-            mapped values found from the names. The order of the mapped values is the
+            Mapped values found from the names. The order of the mapped values is the
             same as the order of the names. None if there is no mapped value for a name.
         """
 
         return list(map(self._map.get, names))
 
     @classmethod
     @abstractmethod
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 
 from ...caches import (
     BaseCandidateLayerCache,
     CandidateLayerFileCache,
     CandidateLayerNoCache,
 )
 from ..base import BaseMapper
 
 
-class CandidateLayerCacheMapper(BaseMapper[Type[BaseCandidateLayerCache]]):
-    """A mapper to find candidate layer cache classes."""
+class CandidateLayerCacheMapper(BaseMapper[type[BaseCandidateLayerCache]]):
+    """Mapper to find candidate layer cache classes."""
 
     @classmethod
     def default_mapper(cls) -> "CandidateLayerCacheMapper":
         default_mapper = cls()
 
         cache_clses = [CandidateLayerNoCache, CandidateLayerFileCache]
         for cache_cls in cache_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Any, Type
+from typing import Any
 
 from py_pdf_term._common.consts import PACKAGE_NAME
 
 from ...caches import (
     BaseMethodLayerDataCache,
     BaseMethodLayerRankingCache,
     MethodLayerDataFileCache,
     MethodLayerDataNoCache,
     MethodLayerRankingFileCache,
     MethodLayerRankingNoCache,
 )
 from ..base import BaseMapper
 
 
-class MethodLayerRankingCacheMapper(BaseMapper[Type[BaseMethodLayerRankingCache]]):
-    """A mapper to find method layer ranking cache classes."""
+class MethodLayerRankingCacheMapper(BaseMapper[type[BaseMethodLayerRankingCache]]):
+    """Mapper to find method layer ranking cache classes."""
 
     @classmethod
     def default_mapper(cls) -> "MethodLayerRankingCacheMapper":
         default_mapper = cls()
 
         cache_clses = [MethodLayerRankingNoCache, MethodLayerRankingFileCache]
         for cache_cls in cache_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{cache_cls.__name__}", cache_cls)
 
         return default_mapper
 
 
-class MethodLayerDataCacheMapper(BaseMapper[Type[BaseMethodLayerDataCache[Any]]]):
-    """A mapper to find method layer data cache classes."""
+class MethodLayerDataCacheMapper(BaseMapper[type[BaseMethodLayerDataCache[Any]]]):
+    """Mapper to find method layer data cache classes."""
 
     @classmethod
     def default_mapper(cls) -> "MethodLayerDataCacheMapper":
         default_mapper = cls()
 
         cache_clses = [
             ("MethodLayerDataNoCache", MethodLayerDataNoCache[Any]),
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 
 from ...caches import BaseStylingLayerCache, StylingLayerFileCache, StylingLayerNoCache
 from ..base import BaseMapper
 
 
-class StylingLayerCacheMapper(BaseMapper[Type[BaseStylingLayerCache]]):
-    """A mapper to find styling layer cache classes."""
+class StylingLayerCacheMapper(BaseMapper[type[BaseStylingLayerCache]]):
+    """Mapper to find styling layer cache classes."""
 
     @classmethod
     def default_mapper(cls) -> "StylingLayerCacheMapper":
         default_mapper = cls()
 
         cache_clses = [StylingLayerNoCache, StylingLayerFileCache]
         for cache_cls in cache_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 
 from ...caches import BaseXMLLayerCache, XMLLayerFileCache, XMLLayerNoCache
 from ..base import BaseMapper
 
 
-class XMLLayerCacheMapper(BaseMapper[Type[BaseXMLLayerCache]]):
-    """A mapper to find XML layer cache classes."""
+class XMLLayerCacheMapper(BaseMapper[type[BaseXMLLayerCache]]):
+    """Mapper to find XML layer cache classes."""
 
     @classmethod
     def default_mapper(cls) -> "XMLLayerCacheMapper":
         default_mapper = cls()
 
         cache_clses = [XMLLayerNoCache, XMLLayerFileCache]
         for cache_cls in cache_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.candidates.classifiers import (
     BaseTokenClassifier,
     EnglishTokenClassifier,
     JapaneseTokenClassifier,
 )
 
 from ..base import BaseMapper
 
 
-class TokenClassifierMapper(BaseMapper[Type[BaseTokenClassifier]]):
-    """A mapper to find token classifier classes."""
+class TokenClassifierMapper(BaseMapper[type[BaseTokenClassifier]]):
+    """Mapper to find token classifier classes."""
 
     @classmethod
     def default_mapper(cls) -> "TokenClassifierMapper":
         default_mapper = cls()
 
         classifier_clses = [
             JapaneseTokenClassifier,
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.candidates.filters import (
     BaseCandidateTermFilter,
     BaseCandidateTokenFilter,
     EnglishConcatenationFilter,
     EnglishNumericFilter,
     EnglishProperNounFilter,
@@ -15,30 +13,30 @@
     JapaneseSymbolLikeFilter,
     JapaneseTokenFilter,
 )
 
 from ..base import BaseMapper
 
 
-class CandidateTokenFilterMapper(BaseMapper[Type[BaseCandidateTokenFilter]]):
-    """A mapper to find candidate token filter classes."""
+class CandidateTokenFilterMapper(BaseMapper[type[BaseCandidateTokenFilter]]):
+    """Mapper to find candidate token filter classes."""
 
     @classmethod
     def default_mapper(cls) -> "CandidateTokenFilterMapper":
         default_mapper = cls()
 
         token_filter_clses = [JapaneseTokenFilter, EnglishTokenFilter]
         for filter_cls in token_filter_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{filter_cls.__name__}", filter_cls)
 
         return default_mapper
 
 
-class CandidateTermFilterMapper(BaseMapper[Type[BaseCandidateTermFilter]]):
-    """A mapper to find candidate term filter classes."""
+class CandidateTermFilterMapper(BaseMapper[type[BaseCandidateTermFilter]]):
+    """Mapper to find candidate term filter classes."""
 
     @classmethod
     def default_mapper(cls) -> "CandidateTermFilterMapper":
         default_mapper = cls()
 
         term_filter_clses = [
             JapaneseConcatenationFilter,
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.tokenizers import (
     BaseLanguageTokenizer,
     EnglishTokenizer,
     JapaneseTokenizer,
 )
 
 from ..base import BaseMapper
 
 
-class LanguageTokenizerMapper(BaseMapper[Type[BaseLanguageTokenizer]]):
-    """A mapper to find language tokenizer classes."""
+class LanguageTokenizerMapper(BaseMapper[type[BaseLanguageTokenizer]]):
+    """Mapper to find language tokenizer classes."""
 
     @classmethod
     def default_mapper(cls) -> "LanguageTokenizerMapper":
         default_mapper = cls()
 
         lang_tokenizer_clses = [JapaneseTokenizer, EnglishTokenizer]
         for lang_tokenizer_cls in lang_tokenizer_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.candidates.splitters import (
     BaseSplitter,
     RepeatSplitter,
     SymbolNameSplitter,
 )
 
 from ..base import BaseMapper
 
 
-class SplitterMapper(BaseMapper[Type[BaseSplitter]]):
-    """A mapper to find splitter classes."""
+class SplitterMapper(BaseMapper[type[BaseSplitter]]):
+    """Mapper to find splitter classes."""
 
     @classmethod
     def default_mapper(cls) -> "SplitterMapper":
         default_mapper = cls()
 
         splitter_clses = [SymbolNameSplitter, RepeatSplitter]
         for splitter_cls in splitter_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Type
+from typing import Any
 
 from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.methods import BaseMultiDomainRankingMethod, MDPMethod, TFIDFMethod
 
 from ..base import BaseMapper
 
 
 class MultiDomainRankingMethodMapper(
-    BaseMapper[Type[BaseMultiDomainRankingMethod[Any]]]
+    BaseMapper[type[BaseMultiDomainRankingMethod[Any]]]
 ):
-    """A mapper to find multi-domain ranking method classes."""
+    """Mapper to find multi-domain ranking method classes."""
 
     @classmethod
     def default_mapper(cls) -> "MultiDomainRankingMethodMapper":
         default_mapper = cls()
 
         multi_domain_clses = [TFIDFMethod, MDPMethod]
         for method_cls in multi_domain_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Any, Type
+from typing import Any
 
 from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.methods import (
     BaseSingleDomainRankingMethod,
     FLRHMethod,
     FLRMethod,
     HITSMethod,
     MCValueMethod,
 )
 
 from ..base import BaseMapper
 
 
 class SingleDomainRankingMethodMapper(
-    BaseMapper[Type[BaseSingleDomainRankingMethod[Any]]]
+    BaseMapper[type[BaseSingleDomainRankingMethod[Any]]]
 ):
-    """A mapper to find single-domain ranking method classes."""
+    """Mapper to find single-domain ranking method classes."""
 
     @classmethod
     def default_mapper(cls) -> "SingleDomainRankingMethodMapper":
         default_mapper = cls()
 
         single_domain_clses = [MCValueMethod, FLRMethod, HITSMethod, FLRHMethod]
         for method_cls in single_domain_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py` & `py_pdf_term-1.0.2/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import Type
-
 from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.stylings.scores import BaseStylingScore, ColorScore, FontsizeScore
 
 from ..base import BaseMapper
 
 
-class StylingScoreMapper(BaseMapper[Type[BaseStylingScore]]):
-    """A mapper to find styling score classes."""
+class StylingScoreMapper(BaseMapper[type[BaseStylingScore]]):
+    """Mapper to find styling score classes."""
 
     @classmethod
     def default_mapper(cls) -> "StylingScoreMapper":
         default_mapper = cls()
 
         styling_score_clses = [FontsizeScore, ColorScore]
         for styling_score_cls in styling_score_clses:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/mappers.py` & `py_pdf_term-1.0.2/py_pdf_term/mappers.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/__init__.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/base.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta, abstractmethod
-from typing import Any, Dict, Generic, Iterator, List, Optional
+from typing import Any, Generic, Iterator
 
 from py_pdf_term.candidates import DomainCandidateTermList
 
 from .collectors import BaseRankingDataCollector
 from .data import MethodTermRanking
 from .rankers import BaseMultiDomainRanker, BaseSingleDomainRanker
 from .rankingdata.base import RankingData
@@ -12,49 +12,49 @@
 class BaseSingleDomainRankingMethod(Generic[RankingData], metaclass=ABCMeta):
     """Base class for ranking methods with an algorithm which does not require
     cross-domain information.
 
     Args
     ----
         data_collector:
-            A collector of metadata to rank candidate terms in domain-specific PDF
+            Collector of metadata to rank candidate terms in domain-specific PDF
             documents.
         ranker:
-            A ranker of candidate terms in PDF documents by an algorithm which does not
+            Ranker of candidate terms in PDF documents by an algorithm which does not
             require cross-domain information.
     """
 
     def __init__(
         self,
         data_collector: BaseRankingDataCollector[RankingData],
         ranker: BaseSingleDomainRanker[RankingData],
     ) -> None:
         self._data_collector = data_collector
         self._ranker = ranker
 
     def rank_terms(
         self,
         domain_candidates: DomainCandidateTermList,
-        ranking_data: Optional[RankingData] = None,
+        ranking_data: RankingData | None = None,
     ) -> MethodTermRanking:
         """Rank candidate terms in PDF documents in a domain.
 
         Args
         ----
             domain_candidates:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
             ranking_data:
                 Metadata to rank candidate terms in PDF documents. If this argument is
                 not None, this method skips collecting metadata and uses this argument
                 instead. The default is None.
 
         Returns
         -------
             MethodTermRanking:
-                A ranking result of candidate terms in PDF documents.
+                Ranking result of candidate terms in PDF documents.
         """
 
         if ranking_data is None:
             ranking_data = self._data_collector.collect(domain_candidates)
         term_ranking = self._ranker.rank_terms(domain_candidates, ranking_data)
         return term_ranking
 
@@ -76,36 +76,36 @@
 
         This method is useful when you want to utilize cached metadata to rank candidate
         terms in PDF documents.
 
         Args
         ----
             domain_candidates:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
 
         Returns
         -------
             RankingData:
                 Metadata to rank candidate terms in PDF documents.
 
         """
 
         ranking_data = self._data_collector.collect(domain_candidates)
         return ranking_data
 
     @classmethod
     @abstractmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> RankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> RankingData:
         """Collect metadata to rank candidate terms in PDF documents from a dictionary.
         This method is used to load cached metadata.
 
         Args
         ----
             obj:
-                A dictionary which contains metadata to rank candidate terms in PDF
+                Dictionary which contains metadata to rank candidate terms in PDF
                 documents in a domain.
 
         Returns
         -------
             RankingData:
                 Metadata to rank candidate terms in PDF documents.
         """
@@ -116,83 +116,83 @@
 class BaseMultiDomainRankingMethod(Generic[RankingData], metaclass=ABCMeta):
     """Base class for ranking methods with an algorithm which requires cross-domain
     information.
 
     Args
     ----
         data_collector:
-            A collector of metadata to rank candidate terms in domain-specific PDF
+            Collector of metadata to rank candidate terms in domain-specific PDF
             documents.
         ranker:
-            A ranker of candidate terms in PDF documents by an algorithm which requires
+            Ranker of candidate terms in PDF documents by an algorithm which requires
             cross-domain information.
     """
 
     def __init__(
         self,
         data_collector: BaseRankingDataCollector[RankingData],
         ranker: BaseMultiDomainRanker[RankingData],
     ) -> None:
         self._data_collector = data_collector
         self._ranker = ranker
 
     def rank_terms(
         self,
-        domain_candidates_list: List[DomainCandidateTermList],
-        ranking_data_list: Optional[List[RankingData]] = None,
+        domain_candidates_list: list[DomainCandidateTermList],
+        ranking_data_list: list[RankingData] | None = None,
     ) -> Iterator[MethodTermRanking]:
         """Rank candidate terms in PDF documents in multiple domains.
 
         Args
         ----
             domain_candidates_list:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
             ranking_data_list:
                 Metadata to rank candidate terms in PDF documents. If this argument is
                 not None, this method skips collecting metadata and uses this argument
                 instead. The default is None.
 
         Yields
         ------
             MethodTermRanking:
-                A ranking result of candidate terms in PDF documents.
+                Ranking result of candidate terms in PDF documents.
         """
 
         if ranking_data_list is None:
             ranking_data_list = list(
                 map(self._data_collector.collect, domain_candidates_list)
             )
 
         for domain_candidates in domain_candidates_list:
             term_ranking = self._ranker.rank_terms(domain_candidates, ranking_data_list)
             yield term_ranking
 
     def rank_domain_terms(
         self,
         domain: str,
-        domain_candidates_list: List[DomainCandidateTermList],
-        ranking_data_list: Optional[List[RankingData]] = None,
+        domain_candidates_list: list[DomainCandidateTermList],
+        ranking_data_list: list[RankingData] | None = None,
     ) -> MethodTermRanking:
         """Rank candidate terms in PDF documents in a domain.
 
         Args
         ----
             domain:
-                A domain to rank candidate terms in PDF documents.
+                Domain to rank candidate terms in PDF documents.
             domain_candidates_list:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
             ranking_data_list:
                 Metadata to rank candidate terms in PDF documents. If this argument is
                 not None, this method skips collecting metadata and uses this argument
                 instead. The default is None.
 
         Returns
         -------
             MethodTermRanking:
-                A ranking result of candidate terms in PDF documents.
+                Ranking result of candidate terms in PDF documents.
         """
 
         domain_candidates = next(
             filter(lambda item: item.domain == domain, domain_candidates_list)
         )
 
         if ranking_data_list is None:
@@ -221,30 +221,30 @@
 
         This method is useful when you want to utilize cached metadata to rank candidate
         terms in PDF documents.
 
         Args
         ----
             domain_candidates:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
         """
 
         ranking_data = self._data_collector.collect(domain_candidates)
         return ranking_data
 
     @classmethod
     @abstractmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> RankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> RankingData:
         """Collect metadata to rank candidate terms in PDF documents from a dictionary.
         This method is used to load cached metadata.
 
         Args
         ----
             obj:
-                A dictionary which contains metadata to rank candidate terms in PDF
+                Dictionary which contains metadata to rank candidate terms in PDF
                 documents in a domain.
 
         Returns
         -------
             RankingData:
                 Metadata to rank candidate terms in PDF documents.
         """
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/__init__.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/base.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     @abstractmethod
     def collect(self, domain_candidates: DomainCandidateTermList) -> RankingData:
         """Collect metadata to rank candidate terms in domain-specific PDF documents.
 
         Args
         ----
             domain_candidates:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
 
         Returns
         -------
             RankingData:
                 Metadata to rank candidate terms in PDF documents.
         """
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flr.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/hits.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from py_pdf_term.analysis import TermLeftRightFrequencyAnalyzer, TermOccurrenceAnalyzer
 from py_pdf_term.candidates import DomainCandidateTermList
 
-from ..rankingdata import FLRRankingData
+from ..rankingdata import HITSRankingData
 from .base import BaseRankingDataCollector
 
 
-class FLRRankingDataCollector(BaseRankingDataCollector[FLRRankingData]):
-    """A collector of metadata to rank candidate terms in domain-specific PDF documents
-    by FLR algorithm.
+class HITSRankingDataCollector(BaseRankingDataCollector[HITSRankingData]):
+    """Collector of metadata to rank candidate terms in domain-specific PDF documents
+    by HITS algorithm.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
         self._lrfreq_analyzer = TermLeftRightFrequencyAnalyzer()
 
-    def collect(self, domain_candidates: DomainCandidateTermList) -> FLRRankingData:
+    def collect(self, domain_candidates: DomainCandidateTermList) -> HITSRankingData:
         termocc = self._termocc_analyzer.analyze(domain_candidates)
         lrfreq = self._lrfreq_analyzer.analyze(domain_candidates)
 
-        return FLRRankingData(
+        return HITSRankingData(
             domain_candidates.domain,
             termocc.term_freq,
             lrfreq.left_freq,
             lrfreq.right_freq,
         )
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flrh.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/flrh.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from py_pdf_term.candidates import DomainCandidateTermList
 
 from ..rankingdata import FLRHRankingData
 from .base import BaseRankingDataCollector
 
 
 class FLRHRankingDataCollector(BaseRankingDataCollector[FLRHRankingData]):
-    """A collector of metadata to rank candidate terms in domain-specific PDF documents
+    """Collector of metadata to rank candidate terms in domain-specific PDF documents
     by FLRH algorithm.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
         self._lrfreq_analyzer = TermLeftRightFrequencyAnalyzer()
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/mcvalue.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/tfidf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from py_pdf_term.analysis import ContainerTermsAnalyzer, TermOccurrenceAnalyzer
+from py_pdf_term.analysis import TermOccurrenceAnalyzer
 from py_pdf_term.candidates import DomainCandidateTermList
 
-from ..rankingdata import MCValueRankingData
+from ..rankingdata import TFIDFRankingData
 from .base import BaseRankingDataCollector
 
 
-class MCValueRankingDataCollector(BaseRankingDataCollector[MCValueRankingData]):
-    """A collector of metadata to rank candidate terms in domain-specific PDF documents
-    by MC-Value algorithm.
+class TFIDFRankingDataCollector(BaseRankingDataCollector[TFIDFRankingData]):
+    """Collector of metadata to rank candidate terms in domain-specific PDF documents
+    by TF-IDF algorithm.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
-        self._containers_analyzer = ContainerTermsAnalyzer()
 
-    def collect(self, domain_candidates: DomainCandidateTermList) -> MCValueRankingData:
+    def collect(self, domain_candidates: DomainCandidateTermList) -> TFIDFRankingData:
         termocc = self._termocc_analyzer.analyze(domain_candidates)
-        container_terms = self._containers_analyzer.analyze(domain_candidates)
+        num_docs = len(domain_candidates.pdfs)
 
-        return MCValueRankingData(
+        return TFIDFRankingData(
             domain_candidates.domain,
             termocc.term_freq,
-            container_terms.container_terms,
+            termocc.doc_term_freq,
+            num_docs,
         )
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/mdp.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/collectors/mdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from py_pdf_term.candidates import DomainCandidateTermList
 
 from ..rankingdata import MDPRankingData
 from .base import BaseRankingDataCollector
 
 
 class MDPRankingDataCollector(BaseRankingDataCollector[MDPRankingData]):
-    """A collector of metadata to rank candidate terms in domain-specific PDF documents
+    """Collector of metadata to rank candidate terms in domain-specific PDF documents
     by MDP algorithm.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/data.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Dict, List
+from typing import Any
 
 from py_pdf_term._common.data import ScoredTerm
 
 
 @dataclass(frozen=True)
 class MethodTermRanking:
     """Domain name and ranking of technical terms of the domain.
@@ -14,21 +14,21 @@
             Domain name. (e.g., "natural language processing")
         ranking:
             List of pairs of lemmatized term and method score.
             The list is sorted by the score in descending order.
     """
 
     domain: str
-    ranking: List[ScoredTerm]
+    ranking: list[ScoredTerm]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "domain": self.domain,
             "ranking": list(map(lambda term: term.to_dict(), self.ranking)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "MethodTermRanking":
+    def from_dict(cls, obj: dict[str, Any]) -> "MethodTermRanking":
         return cls(
             obj["domain"],
             list(map(lambda item: ScoredTerm.from_dict(item), obj["ranking"])),
         )
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flr.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseSingleDomainRankingMethod
 from .collectors import FLRRankingDataCollector
 from .rankers import FLRRanker
 from .rankingdata import FLRRankingData
 
 
 class FLRMethod(BaseSingleDomainRankingMethod[FLRRankingData]):
-    """A ranking method by FLR algorithm."""
+    """Ranking method by FLR algorithm."""
 
     def __init__(self) -> None:
         collector = FLRRankingDataCollector()
         ranker = FLRRanker()
         super().__init__(collector, ranker)
 
     @classmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> FLRRankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> FLRRankingData:
         return FLRRankingData(**obj)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flrh.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/flrh.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseSingleDomainRankingMethod
 from .collectors import FLRHRankingDataCollector
 from .rankers import FLRHRanker
 from .rankingdata import FLRHRankingData
 
 
 class FLRHMethod(BaseSingleDomainRankingMethod[FLRHRankingData]):
-    """A ranking method by FLRH algorithm. This algorithm is a combination of FLR and
+    """Ranking method by FLRH algorithm. This algorithm is a combination of FLR and
     HITS.
 
     Args
     ----
         threshold:
-            A threshold of the FLRH algorithm. The default is 1e-8.
+            Threshold of the FLRH algorithm. The default is 1e-8.
 
         max_loop:
-            A maximum number of loops of the FLRH algorithm. The default is 1000.
+            Maximum number of loops of the FLRH algorithm. The default is 1000.
     """
 
     def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
         collector = FLRHRankingDataCollector()
         ranker = FLRHRanker(threshold=threshold, max_loop=max_loop)
         super().__init__(collector, ranker)
 
     @classmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> FLRHRankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> FLRHRankingData:
         return FLRHRankingData(**obj)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/hits.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/hits.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseSingleDomainRankingMethod
 from .collectors import HITSRankingDataCollector
 from .rankers import HITSRanker
 from .rankingdata import HITSRankingData
 
 
 class HITSMethod(BaseSingleDomainRankingMethod[HITSRankingData]):
-    """A ranking method by HITS algorithm.
+    """Ranking method by HITS algorithm.
 
     Args
     ----
         threshold:
-            The threshold to determine convergence. If the difference between
+            Threshold to determine convergence. If the difference between
             original auth/hub values and new auth/hub values is less than this
             threshold, the algorithm is considered to be converged. The default is 1e-8.
         max_loop:
-            The maximum number of loops to run the algorithm. If the algorithm
+            Maximum number of loops to run the algorithm. If the algorithm
             does not converge within this number of loops, it is forced to stop. The
             default is 1000.
     """
 
     def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
         collector = HITSRankingDataCollector()
         ranker = HITSRanker(threshold=threshold, max_loop=max_loop)
         super().__init__(collector, ranker)
 
     @classmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> HITSRankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> HITSRankingData:
         return HITSRankingData(**obj)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/mcvalue.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mcvalue.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseSingleDomainRankingMethod
 from .collectors import MCValueRankingDataCollector
 from .rankers import MCValueRanker
 from .rankingdata import MCValueRankingData
 
 
 class MCValueMethod(BaseSingleDomainRankingMethod[MCValueRankingData]):
-    """A ranking method by MC-Value algorithm."""
+    """Ranking method by MC-Value algorithm."""
 
     def __init__(self) -> None:
         collector = MCValueRankingDataCollector()
         ranker = MCValueRanker()
         super().__init__(collector, ranker)
 
     @classmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> MCValueRankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> MCValueRankingData:
         return MCValueRankingData(**obj)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/mdp.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/mdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseMultiDomainRankingMethod
 from .collectors import MDPRankingDataCollector
 from .rankers import MDPRanker
 from .rankingdata import MDPRankingData
 
 
 class MDPMethod(BaseMultiDomainRankingMethod[MDPRankingData]):
-    """A ranking method by MDP algorithm."""
+    """Ranking method by MDP algorithm."""
 
     def __init__(self) -> None:
         collector = MDPRankingDataCollector()
         ranker = MDPRanker()
         super().__init__(collector, ranker)
 
     @classmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> MDPRankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> MDPRankingData:
         return MDPRankingData(**obj)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/base.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABCMeta, abstractmethod
-from typing import Generic, List
+from typing import Generic
 
 from py_pdf_term.candidates import DomainCandidateTermList
 
 from ..data import MethodTermRanking
 from ..rankingdata.base import RankingData
 
 
@@ -22,22 +22,22 @@
         ranking_data: RankingData,
     ) -> MethodTermRanking:
         """Rank candidate terms in domain-specific PDF documents.
 
         Args
         ----
             domain_candidates:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
             ranking_data:
                 Metadata to rank candidate terms in PDF documents.
 
         Returns
         -------
             MethodTermRanking:
-                A ranking result of candidate terms in PDF documents.
+                Ranking result of candidate terms in PDF documents.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.rank_terms()")
 
 
 class BaseMultiDomainRanker(Generic[RankingData], metaclass=ABCMeta):
     """Base class for term rankers with an algorithm which requires cross-domain
@@ -47,26 +47,26 @@
     def __init__(self) -> None:
         pass
 
     @abstractmethod
     def rank_terms(
         self,
         domain_candidates: DomainCandidateTermList,
-        ranking_data_list: List[RankingData],
+        ranking_data_list: list[RankingData],
     ) -> MethodTermRanking:
         """Rank candidate terms in domain-specific PDF documents.
 
         Args
         ----
             domain_candidates:
-                A list of candidate terms in domain-specific PDF documents.
+                List of candidate terms in domain-specific PDF documents.
             ranking_data_list:
                 List of metadata to rank candidate terms in PDF documents for each
                 domain.
 
         Returns
         -------
             MethodTermRanking:
-                A ranking result of candidate terms in PDF documents.
+                Ranking result of candidate terms in PDF documents.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.rank_terms()")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flr.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flr.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..data import MethodTermRanking
 from ..rankingdata import FLRRankingData
 from .base import BaseSingleDomainRanker
 
 
 class FLRRanker(BaseSingleDomainRanker[FLRRankingData]):
-    """A term ranker by FLR algorithm."""
+    """Term ranker by FLR algorithm."""
 
     def __init__(self) -> None:
         pass
 
     def rank_terms(
         self, domain_candidates: DomainCandidateTermList, ranking_data: FLRRankingData
     ) -> MethodTermRanking:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flrh.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/flrh.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from ..rankingdata import FLRHRankingData, FLRRankingData, HITSRankingData
 from .base import BaseSingleDomainRanker
 from .flr import FLRRanker
 from .hits import HITSAuthHubData, HITSRanker
 
 
 class FLRHRanker(BaseSingleDomainRanker[FLRHRankingData]):
-    """A term ranker by FLRH algorithm. This algorithm is a combination of FLR and HITS.
+    """Term ranker by FLRH algorithm. This algorithm is a combination of FLR and HITS.
 
     Args
     ----
         threshold:
-            A threshold value for HITS algorithm. The default is 1e-8.
+            Threshold value for HITS algorithm. The default is 1e-8.
         max_loop:
-            A maximum number of loops for HITS algorithm. The default is 1000.
+            Maximum number of loops for HITS algorithm. The default is 1000.
     """
 
     def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
         self._flr_ranker = FLRRanker()
         self._hits_ranker = HITSRanker(threshold=threshold, max_loop=max_loop)
 
     def rank_terms(
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/hits.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/hits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from dataclasses import dataclass
 from math import sqrt
-from typing import Dict
 
 from py_pdf_term._common.data import ScoredTerm
 from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import DomainCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from ..data import MethodTermRanking
@@ -22,29 +21,29 @@
             Auth value of the token. The more tokens links to, the larger the auth value
             becomes. The initial auth value is 1.0.
         token_hub:
             Hub value of the term. The more tokens is linked from, the larger the hub
             value becomes. The initial hub value is 1.0.
     """
 
-    token_auth: Dict[str, float]
-    token_hub: Dict[str, float]
+    token_auth: dict[str, float]
+    token_hub: dict[str, float]
 
 
 class HITSRanker(BaseSingleDomainRanker[HITSRankingData]):
-    """A term ranker by HITS algorithm.
+    """Term ranker by HITS algorithm.
 
     Args
     ----
         threshold:
-            The threshold to determine convergence. If the difference between
+            Threshold to determine convergence. If the difference between
             original auth/hub values and new auth/hub values is less than this
             threshold, the algorithm is considered to be converged. The default is 1e-8.
         max_loop:
-            The maximum number of loops to run the algorithm. If the algorithm
+            Maximum number of loops to run the algorithm. If the algorithm
             does not converge within this number of loops, it is forced to stop. The
             default is 1000.
     """
 
     def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
         if threshold <= 0:
             raise ValueError("threshold must be positive")
@@ -69,18 +68,18 @@
                 domain_candidates_dict.values(),
             )
         )
         ranking.sort(key=lambda term: term.score, reverse=True)
         return MethodTermRanking(domain_candidates.domain, ranking)
 
     def _create_auth_hub_data(self, ranking_data: HITSRankingData) -> HITSAuthHubData:
-        token_auth: Dict[str, float] = {
+        token_auth: dict[str, float] = {
             token_lemma: 1.0 for token_lemma in ranking_data.left_freq
         }
-        token_hub: Dict[str, float] = {
+        token_hub: dict[str, float] = {
             token_lemma: 1.0 for token_lemma in ranking_data.right_freq
         }
 
         converged = False
         loop = 0
         while not converged and loop < self._max_loop:
             new_token_auth = {
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/mcvalue.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mcvalue.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..data import MethodTermRanking
 from ..rankingdata import MCValueRankingData
 from .base import BaseSingleDomainRanker
 
 
 class MCValueRanker(BaseSingleDomainRanker[MCValueRankingData]):
-    """A term ranker by MC-Value algorithm."""
+    """Term ranker by MC-Value algorithm."""
 
     def __init__(self) -> None:
         pass
 
     def rank_terms(
         self,
         domain_candidates: DomainCandidateTermList,
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/mdp.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/mdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from sys import float_info
-from typing import List
 
 from py_pdf_term._common.data import ScoredTerm
 from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import DomainCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from ..data import MethodTermRanking
 from ..rankingdata import MDPRankingData
 from .base import BaseMultiDomainRanker
 
 
 class MDPRanker(BaseMultiDomainRanker[MDPRankingData]):
-    """A term ranker by MDP algorithm."""
+    """Term ranker by MDP algorithm."""
 
     def __init__(self) -> None:
         pass
 
     def rank_terms(
         self,
         domain_candidates: DomainCandidateTermList,
-        ranking_data_list: List[MDPRankingData],
+        ranking_data_list: list[MDPRankingData],
     ) -> MethodTermRanking:
         domain_candidates_dict = domain_candidates.to_nostyle_candidates_dict(
             to_str=lambda candidate: candidate.lemma()
         )
         ranking_data = next(
             filter(
                 lambda item: item.domain == domain_candidates.domain,
@@ -48,15 +47,15 @@
         ranking.sort(key=lambda term: term.score, reverse=True)
         return MethodTermRanking(domain_candidates.domain, ranking)
 
     def _calculate_score(
         self,
         candidate: Term,
         ranking_data: MDPRankingData,
-        other_ranking_data_list: List[MDPRankingData],
+        other_ranking_data_list: list[MDPRankingData],
     ) -> ScoredTerm:
         candidate_lemma = candidate.lemma()
         score = min(
             map(
                 lambda other_ranking_data: self._calculate_zvalue(
                     candidate, ranking_data, other_ranking_data
                 ),
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/tfidf.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankers/tfidf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from math import log10
-from typing import List
 
 from py_pdf_term._common.data import ScoredTerm
 from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import DomainCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from ..data import MethodTermRanking
 from ..rankingdata import TFIDFRankingData
 from .base import BaseMultiDomainRanker
 
 
 class TFIDFRanker(BaseMultiDomainRanker[TFIDFRankingData]):
-    """A term ranker by TF-IDF algorithm."""
+    """Term ranker by TF-IDF algorithm."""
 
     def __init__(self) -> None:
         pass
 
     def rank_terms(
         self,
         domain_candidates: DomainCandidateTermList,
-        ranking_data_list: List[TFIDFRankingData],
+        ranking_data_list: list[TFIDFRankingData],
     ) -> MethodTermRanking:
         domain_candidates_dict = domain_candidates.to_nostyle_candidates_dict()
         ranking_data = next(
             filter(
                 lambda item: item.domain == domain_candidates.domain,
                 ranking_data_list,
             )
@@ -40,15 +39,15 @@
         ranking.sort(key=lambda term: term.score, reverse=True)
         return MethodTermRanking(domain_candidates.domain, ranking)
 
     def _calculate_score(
         self,
         candidate: Term,
         ranking_data: TFIDFRankingData,
-        ranking_data_list: List[TFIDFRankingData],
+        ranking_data_list: list[TFIDFRankingData],
     ) -> ScoredTerm:
         candidate_lemma = candidate.lemma()
 
         tf = ranking_data.term_freq.get(candidate_lemma, 0)
         log_tf = log10(tf) if tf > 0 else 0.0
 
         num_docs = sum(map(lambda data: data.num_docs, ranking_data_list))
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/base.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from dataclasses import asdict, dataclass
-from typing import Any, Dict, TypeVar
+from typing import Any, TypeVar
 
 
 @dataclass(frozen=True)
 class BaseRankingData:
     """Base class for ranking data of technical terms of a domain.
 
     Args
     ----
         domain:
             Domain name. (e.g., "natural language processing")
     """
 
     domain: str
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return asdict(self)
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "BaseRankingData":
+    def from_dict(cls, obj: dict[str, Any]) -> "BaseRankingData":
         return cls(**obj)
 
 
 RankingData = TypeVar("RankingData", bound=BaseRankingData)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/flr.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flrh.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import dataclass
-from typing import Dict
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
-class FLRRankingData(BaseRankingData):
-    """Data of technical terms of a domain for FLR algorithm.
+class FLRHRankingData(BaseRankingData):
+    """Data of technical terms of a domain for FLRH algorithm.
 
     Args
     ----
         domain:
             Domain name. (e.g., "natural language processing")
         term_freq:
             Brute force counting of lemmatized term occurrences in the domain.
@@ -20,10 +19,10 @@
             If token or left is meaningless this is fixed at zero.
         right_freq:
             Number of occurrences of lemmatized (token, right) in the domain.
             If token or right is meaningless this is fixed at zero.
     """
 
     domain: str
-    term_freq: Dict[str, int]
-    left_freq: Dict[str, Dict[str, int]]
-    right_freq: Dict[str, Dict[str, int]]
+    term_freq: dict[str, int]
+    left_freq: dict[str, dict[str, int]]
+    right_freq: dict[str, dict[str, int]]
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/flrh.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/flr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import dataclass
-from typing import Dict
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
-class FLRHRankingData(BaseRankingData):
-    """Data of technical terms of a domain for FLRH algorithm.
+class FLRRankingData(BaseRankingData):
+    """Data of technical terms of a domain for FLR algorithm.
 
     Args
     ----
         domain:
             Domain name. (e.g., "natural language processing")
         term_freq:
             Brute force counting of lemmatized term occurrences in the domain.
@@ -20,10 +19,10 @@
             If token or left is meaningless this is fixed at zero.
         right_freq:
             Number of occurrences of lemmatized (token, right) in the domain.
             If token or right is meaningless this is fixed at zero.
     """
 
     domain: str
-    term_freq: Dict[str, int]
-    left_freq: Dict[str, Dict[str, int]]
-    right_freq: Dict[str, Dict[str, int]]
+    term_freq: dict[str, int]
+    left_freq: dict[str, dict[str, int]]
+    right_freq: dict[str, dict[str, int]]
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/hits.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/hits.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from typing import Dict
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
 class HITSRankingData(BaseRankingData):
     """Data of technical terms of a domain for HITS algorithm.
@@ -20,10 +19,10 @@
             If token or left is meaningless this is fixed at zero.
         right_freq:
             Number of occurrences of lemmatized (token, right) in the domain.
             If token or right is meaningless this is fixed at zero.
     """
 
     domain: str
-    term_freq: Dict[str, int]
-    left_freq: Dict[str, Dict[str, int]]
-    right_freq: Dict[str, Dict[str, int]]
+    term_freq: dict[str, int]
+    left_freq: dict[str, dict[str, int]]
+    right_freq: dict[str, dict[str, int]]
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/mcvalue.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mcvalue.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Dict, Set
+from typing import Any
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
 class MCValueRankingData(BaseRankingData):
     """Data of technical terms of a domain for MC-Value algorithm.
@@ -18,26 +18,26 @@
         container_terms:
             Set of containers of the lemmatized term in the domain.
             (term, container) is valid iff the container contains the term as a proper
             subsequence.
     """
 
     domain: str
-    term_freq: Dict[str, int]
-    container_terms: Dict[str, Set[str]]
+    term_freq: dict[str, int]
+    container_terms: dict[str, set[str]]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         container_terms = {
             term: list(containers) for term, containers in self.container_terms.items()
         }
         return {
             "domain": self.domain,
             "term_freq": self.term_freq,
             "container_terms": container_terms,
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "MCValueRankingData":
+    def from_dict(cls, obj: dict[str, Any]) -> "MCValueRankingData":
         container_terms = {
             term: set(containers) for term, containers in obj["container_terms"].items()
         }
         return MCValueRankingData(obj["domain"], obj["term_freq"], container_terms)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/mdp.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/mdp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from dataclasses import asdict, dataclass, field
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
 class MDPRankingData(BaseRankingData):
     """Data of technical terms of a domain for MDP algorithm.
 
-     Args
+    Args
     ----
         domain:
             Domain name. (e.g., "natural language processing")
         term_freq:
             Brute force counting of lemmatized term occurrences in the domain.
             Count even if the lemmatized term occurs as a part of a lemmatized phrase.
         num_terms:
             Brute force counting of all lemmatized terms occurrences in the domain.
             Count even if the lemmatized term occurs as a part of a lemmatized phrase.
     """
 
     domain: str
-    term_freq: Dict[str, int]
+    term_freq: dict[str, int]
     num_terms: int = field(init=False)
 
     def __post_init__(self) -> None:
         object.__setattr__(self, "num_terms", sum(self.term_freq.values()))
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         obj = asdict(self)
         obj.pop("num_terms", None)
         return obj
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "MDPRankingData":
+    def from_dict(cls, obj: dict[str, Any]) -> "MDPRankingData":
         obj.pop("num_terms", None)
         return cls(**obj)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/tfidf.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/rankingdata/tfidf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from dataclasses import dataclass
-from typing import Dict
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
 class TFIDFRankingData(BaseRankingData):
     """Data of technical terms of a domain for TF-IDF algorithm.
@@ -19,10 +18,10 @@
             Number of documents in the domain that contain the lemmatized term.
             Count even if the lemmatized term occurs as a part of a lemmatized phrase.
         num_docs:
             Number of documents in the domain.
     """
 
     domain: str
-    term_freq: Dict[str, int]
-    doc_freq: Dict[str, int]
+    term_freq: dict[str, int]
+    doc_freq: dict[str, int]
     num_docs: int
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/tfidf.py` & `py_pdf_term-1.0.2/py_pdf_term/methods/_methods/tfidf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict
+from typing import Any
 
 from .base import BaseMultiDomainRankingMethod
 from .collectors import TFIDFRankingDataCollector
 from .rankers import TFIDFRanker
 from .rankingdata import TFIDFRankingData
 
 
 class TFIDFMethod(BaseMultiDomainRankingMethod[TFIDFRankingData]):
-    """A ranking method by TF-IDF algorithm."""
+    """Ranking method by TF-IDF algorithm."""
 
     def __init__(self) -> None:
         collector = TFIDFRankingDataCollector()
         ranker = TFIDFRanker()
         super().__init__(collector, ranker)
 
     @classmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> TFIDFRankingData:
+    def collect_data_from_dict(cls, obj: dict[str, Any]) -> TFIDFRankingData:
         return TFIDFRankingData(**obj)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py` & `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     @abstractmethod
     def open(self, file: str, mode: Literal["rb", "wb"]) -> BinaryIO:
         """Open a file with binary mode.
 
         Args
         ----
             file:
-                A path to a file.
+                Path to a file.
             mode:
-                A mode to open the file.
+                Mode to open the file.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.open()")
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/converter.py` & `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from io import BytesIO
-from typing import BinaryIO, Optional
+from typing import BinaryIO
 from xml.etree.ElementTree import fromstring
 
 from pdfminer.layout import LAParams
 from pdfminer.pdfinterp import PDFPageInterpreter, PDFResourceManager
 from pdfminer.pdfpage import PDFPage
 
 from .binopeners import BaseBinaryOpener, StandardBinaryOpener
 from .data import PDFnXMLElement, PDFnXMLPath
 from .textful import TextfulXMLConverter
 
 
 class PDFtoXMLConverter:
-    """A converter from PDF to textful XML format.
+    """Converter from PDF to textful XML format.
 
     Args
     ----
         bin_opener:
-            A binary opener to open PDF and XML files. If None, StandardBinaryOpener is
+            Binary opener to open PDF and XML files. If None, StandardBinaryOpener is
             used, which opens files with the standard open function in Python.
     """
 
-    def __init__(self, bin_opener: Optional[BaseBinaryOpener] = None):  # type: ignore
+    def __init__(self, bin_opener: BaseBinaryOpener | None = None) -> None:
         if bin_opener is None:
             bin_opener = StandardBinaryOpener()
 
         self._bin_opener = bin_opener
 
     def convert_as_file(
         self,
         pdf_path: str,
         xml_path: str,
         nfc_norm: bool = True,
-        include_pattern: Optional[str] = None,
-        exclude_pattern: Optional[str] = None,
+        include_pattern: str | None = None,
+        exclude_pattern: str | None = None,
     ) -> PDFnXMLPath:
         """Convert a PDF file to a textful XML file.
 
         Args
         ----
             pdf_path:
-                A path to a PDF file.
+                Path to a PDF file.
             xml_path:
-                A path to a XML file to output.
+                Path to a XML file to output.
             nfc_norm:
                 If True, normalize text to NFC, otherwise keep original.
             include_pattern:
-                A regular expression pattern of text to include in the output.
+                Regular expression pattern of text to include in the output.
             exclude_pattern:
-                A regular expression pattern of text to exclude from the output
+                Regular expression pattern of text to exclude from the output
                 (overrides include_pattern).
 
         Returns
         -------
             Pair of path to the PDF file and that to the output XML file.
         """
 
@@ -63,29 +63,29 @@
         pdf_io.close()
         return PDFnXMLPath(pdf_path, xml_path)
 
     def convert_as_element(
         self,
         pdf_path: str,
         nfc_norm: bool = True,
-        include_pattern: Optional[str] = None,
-        exclude_pattern: Optional[str] = None,
+        include_pattern: str | None = None,
+        exclude_pattern: str | None = None,
     ) -> PDFnXMLElement:
         """Convert a PDF file to a textful XML element.
 
         Args
         ----
             pdf_path:
-                A path to a PDF file.
+                Path to a PDF file.
             nfc_norm:
                 If True, normalize text to NFC, otherwise keep original.
             include_pattern:
-                A regular expression pattern of text to include in the output.
+                Regular expression pattern of text to include in the output.
             exclude_pattern:
-                A regular expression pattern of text to exclude from the output
+                Regular expression pattern of text to exclude from the output
                 (overrides include_pattern).
 
         Returns
         -------
             Pair of path to the PDF file and XML element tree of the output.
         """
 
@@ -98,16 +98,16 @@
         return PDFnXMLElement(pdf_path, xml_element)
 
     def _run(
         self,
         pdf_io: BinaryIO,
         xml_io: BinaryIO,
         nfc_norm: bool,
-        include_pattern: Optional[str],
-        exclude_pattern: Optional[str],
+        include_pattern: str | None,
+        exclude_pattern: str | None,
     ) -> None:
         manager = PDFResourceManager()
         laparams = LAParams(char_margin=2.0, line_margin=0.5, word_margin=0.2)
         converter = TextfulXMLConverter(
             manager,
             xml_io,
             laparams=laparams,
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/data.py` & `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import asdict, dataclass
-from typing import Any, Dict
+from typing import Any
 from xml.etree.ElementTree import Element, fromstring, tostring
 
 
 @dataclass(frozen=True)
 class PDFnXMLPath:
     """Pair of path to a PDF file and that to a XML file.
 
@@ -14,19 +14,19 @@
         xml_path:
             Path to a XML file.
     """
 
     pdf_path: str
     xml_path: str
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return asdict(self)
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PDFnXMLPath":
+    def from_dict(cls, obj: dict[str, Any]) -> "PDFnXMLPath":
         return cls(**obj)
 
 
 @dataclass(frozen=True)
 class PDFnXMLElement:
     """Pair of path to a PDF file and XML element tree.
 
@@ -44,16 +44,16 @@
     def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, PDFnXMLElement)
             and self.pdf_path == other.pdf_path
             and tostring(self.xml_root) == tostring(other.xml_root)
         )
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "pdf_path": self.pdf_path,
             "xml_root": tostring(self.xml_root, encoding="utf-8"),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PDFnXMLElement":
+    def from_dict(cls, obj: dict[str, Any]) -> "PDFnXMLElement":
         return cls(obj["pdf_path"], fromstring(obj["xml_root"]))
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/textful.py` & `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/textful.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,73 @@
 from dataclasses import dataclass
-from typing import Any, BinaryIO, Optional, Sequence, Tuple, Union
+from typing import BinaryIO, Sequence
+
+from pdfminer.converter import PDFConverter
+from pdfminer.utils import Matrix, PathSegment, Rect, bbox2str, enc
+from pdfminer.pdfinterp import PDFGraphicState, PDFResourceManager
+from pdfminer.pdftypes import PDFStream
 
-from pdfminer.converter import (
-    Matrix,
-    PathSegment,
-    PDFConverter,
-    PDFGraphicState,
-    PDFStream,
-    Rect,
-)
 from pdfminer.layout import (
     LAParams,
     LTAnno,
     LTChar,
     LTPage,
-    LTText,
     LTTextBox,
     LTTextLine,
+    LTComponent,
 )
-from pdfminer.pdfinterp import PDFResourceManager
-from pdfminer.utils import bbox2str, enc
 
 from .utils import clean_content_text
 
-NColor = Union[float, Tuple[float, float, float], Tuple[float, float, float, float]]
+NColor = float | tuple[float, float, float] | tuple[float, float, float, float]
 
 
 @dataclass
 class TextboxState:
     within_section: bool
     size: float
-    ncolor: Optional[NColor]
+    ncolor: NColor | None
     bbox: str
     text: str
 
 
 class TextfulXMLConverter(PDFConverter[BinaryIO]):
     """A PDFConverter subclass that outputs textful XML format.
 
     Args
     ----
         rsrcmgr:
-            A PDFResourceManager object from pdfminer.
+            PDFResourceManager object from pdfminer.
         outfp:
-            A file-like object to output XML.
+            File-like object to output XML.
         codec:
-            A codec name to encode XML.
+            Codec name to encode XML.
         pageno:
-            A page number to start.
+            Page number to start.
         laparams:
-            A LAParams object from pdfminer.
+            LAParams object from pdfminer.
         nfc_norm:
             If True, normalize text to NFC, otherwise keep original.
         include_pattern:
-            A regular expression pattern of text to include in the output.
+            Regular expression pattern of text to include in the output.
         exclude_pattern:
-            A regular expression pattern of text to exclude from the output (overrides
+            Regular expression pattern of text to exclude from the output (overrides
             include_pattern).
     """
 
     def __init__(
         self,
         rsrcmgr: PDFResourceManager,
         outfp: BinaryIO,
         codec: str = "utf-8",
         pageno: int = 1,
-        laparams: Optional[LAParams] = None,
+        laparams: LAParams | None = None,
         nfc_norm: bool = True,
-        include_pattern: Optional[str] = None,
-        exclude_pattern: Optional[str] = None,
+        include_pattern: str | None = None,
+        exclude_pattern: str | None = None,
     ) -> None:
         super().__init__(rsrcmgr, outfp, codec, pageno, laparams)
 
         def _clean_content_text(text: str) -> str:
             return clean_content_text(text, nfc_norm, include_pattern, exclude_pattern)
 
         self._clean_content_text = _clean_content_text
@@ -106,61 +101,72 @@
         stroke: bool,
         fill: bool,
         evenodd: bool,
         path: Sequence[PathSegment],
     ) -> None:
         pass
 
-    def _render(self, item: Any) -> None:
-        if isinstance(item, LTPage):
-            self._render_page(item)
-        elif isinstance(item, LTTextBox):
-            self._render_textbox(item)
-        elif isinstance(item, LTText):
-            self._render_text(item)
+    def _render(self, item: LTComponent) -> None:
+        match item:
+            case LTPage():
+                self._render_page(item)
+            case LTTextBox():
+                self._render_textbox(item)
+            case _:
+                pass
 
     def _render_page(self, ltpage: LTPage) -> None:
         self._write('<page id="%s">\n' % ltpage.pageid)
         for child in ltpage:
             self._render(child)
         self._write("</page>\n")
 
     def _render_textbox(self, lttextbox: LTTextBox) -> None:
         state = TextboxState(False, 0.0, None, "", "")
 
-        def render_textbox_child(child: Any) -> None:
-            if isinstance(child, LTTextLine):
-                for grandchild in child:
-                    render_textbox_child(grandchild)
-            elif isinstance(child, LTChar):
-                if not state.within_section:
-                    enter_text_section(child)
-                    state.text += child.get_text()
-                elif text_section_continues(child):
-                    state.text += child.get_text()
-                else:
-                    exit_text_section()
-                    enter_text_section(child)
-                    state.text += child.get_text()
-            elif isinstance(child, LTAnno):
-                if not state.within_section:
-                    pass
-                elif text_section_continues(child):
-                    state.text += child.get_text()
-                else:
-                    exit_text_section()
+        def render_textbox_child(child: LTTextLine | LTChar | LTAnno) -> None:
+            match child:
+                case LTTextLine():
+                    render_textline(child)
+                case LTChar():
+                    render_char(child)
+                case LTAnno():
+                    render_anno(child)
+
+        def render_textline(lttextline: LTTextLine) -> None:
+            for child in lttextline:
+                render_textbox_child(child)
+
+        def render_char(ltchar: LTChar) -> None:
+            if not state.within_section:
+                enter_text_section(ltchar)
+                state.text += ltchar.get_text()
+            elif text_section_continues(ltchar):
+                state.text += ltchar.get_text()
+            else:
+                exit_text_section()
+                enter_text_section(ltchar)
+                state.text += ltchar.get_text()
+
+        def render_anno(ltanno: LTAnno) -> None:
+            if not state.within_section:
+                pass
+            elif text_section_continues(ltanno):
+                state.text += ltanno.get_text()
+            else:
+                exit_text_section()
 
         def enter_text_section(item: LTChar) -> None:
             state.within_section = True
             state.size = item.size
             state.ncolor = item.graphicstate.ncolor
             state.bbox = bbox2str(item.bbox)
             state.text = ""
 
-        def text_section_continues(item: Union[LTChar, LTAnno]) -> bool:
+        def text_section_continues(item: LTChar | LTAnno) -> bool:
             if isinstance(item, LTAnno):
                 return True
             return (
                 state.ncolor == item.graphicstate.ncolor
                 and abs(state.size - item.size) < 0.1
             )
 
@@ -184,17 +190,10 @@
             state.text = ""
 
         for child in lttextbox:
             render_textbox_child(child)
 
         exit_text_section()
 
-    def _render_text(self, lttext: LTText) -> None:
-        text = self._clean_content_text(lttext.get_text())
-        if text:
-            self._write("<text>")
-            self._write(enc(text))
-            self._write("</text>\n")
-
     def _write(self, text: str) -> None:
         text_bytes = text.encode(self.codec)
         self.outfp.write(text_bytes)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/utils.py` & `py_pdf_term-1.0.2/py_pdf_term/pdftoxml/_pdftoxml/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import re
-from typing import Optional
 from unicodedata import normalize
 
 from py_pdf_term._common.consts import FULLWIDTH_ASCII_CHARS, HALFWIDTH_ASCII_CHARS
 
 ERROR = re.compile(r"[\x00-\x08\x0b-\x0c\x0e-\x1f]|\(cid:\d+\)")
 SPACES = re.compile(r"\s+")
 ASCII_FULL2HALF_TABLE = str.maketrans(FULLWIDTH_ASCII_CHARS, HALFWIDTH_ASCII_CHARS)
 
 
 def clean_content_text(
-    text: str,
-    nfc_norm: bool,
-    include_pattern: Optional[str],
-    exclude_pattern: Optional[str],
+    text: str, nfc_norm: bool, include_pattern: str | None, exclude_pattern: str | None
 ) -> str:
     text = ERROR.sub("", text)
     text = SPACES.sub(" ", text).strip()
     text = text.translate(ASCII_FULL2HALF_TABLE)
 
     if nfc_norm:
         text = normalize("NFC", text)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/data.py` & `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import asdict, dataclass
-from typing import Any, Dict, List
+from typing import Any
 
 from py_pdf_term._common.data import ScoredTerm
 
 
 @dataclass(frozen=True)
 class PageStylingScoreList:
     """Page number and styling scores of technical terms of the page.
@@ -14,21 +14,21 @@
             Page number of a PDF file.
         ranking:
             List of pairs of lemmatized term and styling score.
             The list is sorted by the score in descending order.
     """
 
     page_num: int
-    ranking: List[ScoredTerm]
+    ranking: list[ScoredTerm]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return asdict(self)
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PageStylingScoreList":
+    def from_dict(cls, obj: dict[str, Any]) -> "PageStylingScoreList":
         page_num, ranking = obj["page_num"], obj["ranking"]
         return cls(
             page_num,
             list(map(lambda item: ScoredTerm.from_dict(item), ranking)),
         )
 
 
@@ -41,24 +41,24 @@
         pdf_path:
             Path of a PDF file.
         pages:
             Styling scores of each page of the PDF file.
     """
 
     pdf_path: str
-    pages: List[PageStylingScoreList]
+    pages: list[PageStylingScoreList]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "pdf_path": self.pdf_path,
             "pages": list(map(lambda page: page.to_dict(), self.pages)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PDFStylingScoreList":
+    def from_dict(cls, obj: dict[str, Any]) -> "PDFStylingScoreList":
         pdf_path, pages = obj["pdf_path"], obj["pages"]
         return cls(
             pdf_path,
             list(map(lambda item: PageStylingScoreList.from_dict(item), pages)),
         )
 
 
@@ -71,22 +71,22 @@
         domain:
             Domain name. (e.g., "natural language processing")
         pdfs:
             Styling scores of each PDF file of the domain.
     """
 
     domain: str
-    pdfs: List[PDFStylingScoreList]
+    pdfs: list[PDFStylingScoreList]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "domain": self.domain,
             "pdfs": list(map(lambda pdf: pdf.to_dict(), self.pdfs)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "DomainStylingScoreList":
+    def from_dict(cls, obj: dict[str, Any]) -> "DomainStylingScoreList":
         domain, pdfs = obj["domain"], obj["pdfs"]
         return cls(
             domain,
             list(map(lambda item: PDFStylingScoreList.from_dict(item), pdfs)),
         )
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scorer.py` & `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scorer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from typing import Dict, List, Optional, Type
-
 from py_pdf_term._common.data import ScoredTerm
 from py_pdf_term.candidates import (
     DomainCandidateTermList,
     PageCandidateTermList,
     PDFCandidateTermList,
 )
 
 from .data import DomainStylingScoreList, PageStylingScoreList, PDFStylingScoreList
 from .scores import BaseStylingScore, ColorScore, FontsizeScore
 
 
 class StylingScorer:
-    """A scorer for styling scores. The styling scores are combined by multiplication of
+    """Scorer for styling scores. The styling scores are combined by multiplication of
     each score.
 
     Args
     ----
         styling_score_clses:
-            styling scorers to be combined. If None, the default scorers are used.
+            Styling scorers to be combined. If None, the default scorers are used.
             The default scorers are FontsizeScore and ColorScore.
     """
 
     def __init__(
-        self, styling_score_clses: Optional[List[Type[BaseStylingScore]]] = None
+        self, styling_score_clses: list[type[BaseStylingScore]] | None = None
     ) -> None:
         if styling_score_clses is None:
             styling_score_clses = [FontsizeScore, ColorScore]
 
         self._styling_score_clses = styling_score_clses
 
     def score_domain_candidates(
@@ -39,15 +37,15 @@
         ----
             domain_candidates:
                 List of candidate terms in a domain. The target of analysis.
 
         Returns
         -------
             DomainStylingScoreList:
-                A list of styling scores for each candidate term in a domain. The
+                List of styling scores for each candidate term in a domain. The
                 scores are sorted in descending order.
         """
 
         return DomainStylingScoreList(
             domain_candidates.domain,
             list(map(self.score_pdf_candidates, domain_candidates.pdfs)),
         )
@@ -61,34 +59,34 @@
         ----
             pdf_candidates:
                 List of candidate terms in a PDF file. The target of analysis.
 
         Returns
         -------
             PDFStylingScoreList:
-                A list of styling scores for each candidate term in a PDF file. The
+                List of styling scores for each candidate term in a PDF file. The
                 scores are sorted in descending order.
         """
 
         return PDFStylingScoreList(
             pdf_candidates.pdf_path,
             list(map(self._score_page_candidates, pdf_candidates.pages)),
         )
 
     def _score_page_candidates(
         self, page_candidates: PageCandidateTermList
     ) -> PageStylingScoreList:
-        styling_scores: Dict[str, float] = {
+        styling_scores: dict[str, float] = {
             candidate.lemma(): 1.0 for candidate in page_candidates.candidates
         }
 
         for styling_score_cls in self._styling_score_clses:
             styling_score = styling_score_cls(page_candidates)
 
-            scores: Dict[str, float] = dict()
+            scores: dict[str, float] = dict()
             for candidate in page_candidates.candidates:
                 candidate_lemma = candidate.lemma()
                 score = styling_score.calculate_score(candidate)
                 if candidate_lemma not in scores or score > scores[candidate_lemma]:
                     scores[candidate_lemma] = score
 
             for candidate_lemma in styling_scores:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/base.py` & `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     @abstractmethod
     def calculate_score(self, candidate: Term) -> float:
         """Calculate the styling score of a candidate term.
 
         Args
         ----
             candidate:
-                A candidate term to calculate the styling score. This term is expected
+                Candidate term to calculate the styling score. This term is expected
                 to be included in the list of candidate terms passed to the constructor.
 
         Returns
         -------
             float:
                 The styling score of the candidate term.
         """
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/color.py` & `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/color.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import Dict
-
 from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import PageCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from .base import BaseStylingScore
 
 
 class ColorScore(BaseStylingScore):
-    """A styling score for font color. The more rarely the color appears in the page,
+    """Styling score for font color. The more rarely the color appears in the page,
     the higher the score is.
 
     Args
     ----
         page_candidates:
             List of candidate terms in a page of a PDF file. The target of analysis.
     """
 
     def __init__(self, page_candidates: PageCandidateTermList) -> None:
         super().__init__(page_candidates)
 
         self._num_candidates = len(page_candidates.candidates)
 
-        self._color_freq: Dict[str, int] = dict()
+        self._color_freq: dict[str, int] = dict()
         for candidate in page_candidates.candidates:
             self._color_freq[candidate.ncolor] = (
                 self._color_freq.get(candidate.ncolor, 0) + 1
             )
 
     def calculate_score(self, candidate: Term) -> float:
         if self._num_candidates == 0 or candidate.ncolor not in self._color_freq:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/fontsize.py` & `py_pdf_term-1.0.2/py_pdf_term/stylings/_stylings/scores/fontsize.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from py_pdf_term.candidates import PageCandidateTermList
 from py_pdf_term.tokenizers import Term
 
 from .base import BaseStylingScore
 
 
 class FontsizeScore(BaseStylingScore):
-    """A styling score for font size. The larger the font size is, the higher the score
+    """Styling score for font size. The larger the font size is, the higher the score
     is. The score is normalized by the mean and the standard deviation of font sizes in
     the page.
 
     Args:
         page_candidates:
             List of candidate terms in a page of a PDF file. The target of analysis.
     """
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/data.py` & `py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing import Any, Dict, List
+from typing import Any
 
 from py_pdf_term._common.data import ScoredTerm
 
 
 @dataclass(frozen=True)
 class PageTechnicalTermList:
     """Page number and technical terms of the page.
@@ -13,24 +13,24 @@
         page_num:
             Page number of a PDF file.
         terms:
             Technical terms of the page.
     """
 
     page_num: int
-    terms: List[ScoredTerm]
+    terms: list[ScoredTerm]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "page_num": self.page_num,
             "terms": list(map(lambda term: term.to_dict(), self.terms)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PageTechnicalTermList":
+    def from_dict(cls, obj: dict[str, Any]) -> "PageTechnicalTermList":
         page_num, terms = obj["page_num"], obj["terms"]
         return cls(page_num, list(map(lambda item: ScoredTerm.from_dict(item), terms)))
 
 
 @dataclass(frozen=True)
 class PDFTechnicalTermList:
     """Path of a PDF file and technical terms of the PDF file.
@@ -40,24 +40,24 @@
         pdf_path:
             Path of a PDF file.
         pages:
             Technical terms of each page of the PDF file.
     """
 
     pdf_path: str
-    pages: List[PageTechnicalTermList]
+    pages: list[PageTechnicalTermList]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "pdf_path": self.pdf_path,
             "pages": list(map(lambda page: page.to_dict(), self.pages)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "PDFTechnicalTermList":
+    def from_dict(cls, obj: dict[str, Any]) -> "PDFTechnicalTermList":
         pdf_path, pages = obj["pdf_path"], obj["pages"]
         return cls(
             pdf_path,
             list(map(lambda item: PageTechnicalTermList.from_dict(item), pages)),
         )
 
 
@@ -70,22 +70,22 @@
         domain:
             Domain name. (e.g., "natural language processing")
         pdfs:
             Technical terms of each PDF file of the domain.
     """
 
     domain: str
-    pdfs: List[PDFTechnicalTermList]
+    pdfs: list[PDFTechnicalTermList]
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "domain": self.domain,
             "pdfs": list(map(lambda pdf: pdf.to_dict(), self.pdfs)),
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "DomainTechnicalTermList":
+    def from_dict(cls, obj: dict[str, Any]) -> "DomainTechnicalTermList":
         domain, pdfs = obj["domain"], obj["pdfs"]
         return cls(
             domain,
             list(map(lambda item: PDFTechnicalTermList.from_dict(item), pdfs)),
         )
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/extractor.py` & `py_pdf_term-1.0.2/py_pdf_term/techterms/_techterms/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict, Optional
-
 from py_pdf_term._common.data import ScoredTerm
 from py_pdf_term.candidates import (
     DomainCandidateTermList,
     PageCandidateTermList,
     PDFCandidateTermList,
 )
 from py_pdf_term.methods import MethodTermRanking
@@ -14,36 +12,36 @@
 )
 
 from .data import DomainTechnicalTermList, PageTechnicalTermList, PDFTechnicalTermList
 from .utils import ranking_to_dict
 
 
 class TechnicalTermExtractor:
-    """A technical term extrator based on ranking method scores and styling scores.
+    """Technical term extrator based on ranking method scores and styling scores.
 
     Args
     ----
         max_num_terms:
             Maximum number of terms in a page of a PDF file to be extracted. The N-best
             candidates are extracted as technical terms. The default value is 10.
         acceptance_rate:
-            The acceptance rate of the ranking method scores. The candidates whose
+            Acceptance rate of the ranking method scores. The candidates whose
             ranking method scores are lower than the acceptance rate are filtered out
             even if they are in the N-best candidates. The default value is 0.75.
     """
 
     def __init__(self, max_num_terms: int = 10, acceptance_rate: float = 0.75) -> None:
         if max_num_terms <= 0:
             raise ValueError("max_num_terms must be positive")
         if acceptance_rate <= 0.0 or acceptance_rate > 1.0:
             raise ValueError("acceptance_rate must be in (0.0, 1.0]")
 
         self._max_num_terms = max_num_terms
         self._acceptance_rate = acceptance_rate
-        self._cache: Optional[Dict[str, float]] = None
+        self._cache: dict[str, float] | None = None
 
     def extract_from_domain(
         self,
         domain_candidates: DomainCandidateTermList,
         term_ranking: MethodTermRanking,
         domain_styling_scores: DomainStylingScoreList,
     ) -> DomainTechnicalTermList:
@@ -58,15 +56,15 @@
                 Ranking method scores for each candidate term in a domain.
             domain_styling_scores:
                 Styling scores for each candidate term in a domain.
 
         Returns
         -------
             DomainTechnicalTermList:
-                A list of technical terms in PDF files in a domain. The terms are sorted
+                List of technical terms in PDF files in a domain. The terms are sorted
                 in appearance order, not in score order.
         """
 
         cache_should_flush = self._cache is None
         if self._cache is None:
             self._cache = ranking_to_dict(term_ranking.ranking, self._acceptance_rate)
 
@@ -99,15 +97,15 @@
                 Ranking method scores for each candidate term in a domain.
             pdf_styling_scores:
                 Styling scores for each candidate term in a PDF file.
 
         Returns
         -------
             PDFTechnicalTermList:
-                A list of technical terms in a PDF file. The terms are sorted in
+                List of technical terms in a PDF file. The terms are sorted in
                 appearance order, not in score order.
         """
 
         cache_should_flush = self._cache is None
         if self._cache is None:
             self._cache = ranking_to_dict(term_ranking.ranking, self._acceptance_rate)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/base.py` & `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABCMeta, abstractmethod
-from typing import List
 
 from .data import Token
 
 
 class BaseLanguageTokenizer(metaclass=ABCMeta):
     """Base class for language tokenizers. A language tokenizer is expected to tokenize
     a text into a list of tokens by SpaCy.
@@ -12,39 +11,39 @@
     @abstractmethod
     def inscope(self, text: str) -> bool:
         """Test whether the text is in the scope of the language tokenizer.
 
         Args
         ----
             text:
-                A text to test.
+                Text to test.
 
         Returns
         -------
             bool:
                 True if the text is in the scope of the language tokenizer, otherwise
                 False.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.inscope()")
 
     @abstractmethod
-    def tokenize(self, scoped_text: str) -> List[Token]:
+    def tokenize(self, scoped_text: str) -> list[Token]:
         """Tokenize a scoped text into a list of tokens.
 
         Args
         ----
             scoped_text:
-                A text to tokenize. This text is expected to be in the scope of the
+                Text to tokenize. This text is expected to be in the scope of the
                 language tokenizer.
 
         Returns
         -------
-            List[Token]:
-                A list of tokens.
+            list[Token]:
+                List of tokens.
         """
 
         raise NotImplementedError(f"{self.__class__.__name__}.tokenize()")
 
     @classmethod
     @abstractmethod
     def class_init(cls) -> None:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/data.py` & `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 from dataclasses import asdict, dataclass
-from typing import Any, ClassVar, Dict, List, Union
+from typing import Any, ClassVar
 
 from py_pdf_term._common.consts import NOSPACE_REGEX
 
 GARBAGE_SPACE = re.compile(rf"(?<={NOSPACE_REGEX}) (?=\S)|(?<=\S) (?={NOSPACE_REGEX})")
 
 
 @dataclass
 class Token:
-    """A token in a text.
+    """Token in a text.
 
     Args
     ----
         lang:
             Language of the token. (e.g., "en", "ja")
         surface_form:
             Surface form of the token.
@@ -39,31 +39,31 @@
     subcategory: str
     lemma: str
     is_meaningless: bool = False
 
     def __str__(self) -> str:
         return self.surface_form
 
-    def to_dict(self) -> Dict[str, str]:
+    def to_dict(self) -> dict[str, str]:
         return asdict(self)
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "Token":
+    def from_dict(cls, obj: dict[str, Any]) -> "Token":
         return cls(**obj)
 
 
 @dataclass(frozen=True)
 class Term:
-    tokens: List[Token]
+    tokens: list[Token]
     fontsize: float = 0.0
     ncolor: str = ""
     augmented: bool = False
 
     @property
-    def lang(self) -> Union[str, None]:
+    def lang(self) -> str | None:
         if not self.tokens:
             return None
 
         lang = self.tokens[0].lang
         if all(map(lambda token: token.lang == lang, self.tokens)):
             return lang
 
@@ -78,23 +78,23 @@
         )
 
     def lemma(self) -> str:
         return GARBAGE_SPACE.sub(
             "", " ".join(map(lambda token: token.lemma, self.tokens))
         )
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self) -> dict[str, Any]:
         return {
             "tokens": list(map(lambda token: token.to_dict(), self.tokens)),
             "fontsize": self.fontsize,
             "ncolor": self.ncolor,
             "augmented": self.augmented,
         }
 
     @classmethod
-    def from_dict(cls, obj: Dict[str, Any]) -> "Term":
+    def from_dict(cls, obj: dict[str, Any]) -> "Term":
         return cls(
             list(map(lambda item: Token.from_dict(item), obj["tokens"])),
             obj.get("fontsize", 0),
             obj.get("ncolor", ""),
             obj.get("augmented", False),
         )
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/english.py` & `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/english.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import re
-from typing import Any, List
+from typing import Any
 
 import en_core_web_sm
 
 from py_pdf_term._common.consts import ALPHABET_REGEX, SYMBOL_REGEX
 
 from .base import BaseLanguageTokenizer
 from .data import Token
 
 
 class EnglishTokenizer(BaseLanguageTokenizer):
-    """A tokenizer for English. This tokenizer uses SpaCy's en_core_web_sm model."""
+    """Tokenizer for English. This tokenizer uses SpaCy's en_core_web_sm model."""
 
     def inscope(self, text: str) -> bool:
         return EnglishTokenizer._regex.search(text) is not None
 
-    def tokenize(self, scoped_text: str) -> List[Token]:
+    def tokenize(self, scoped_text: str) -> list[Token]:
         scoped_text = EnglishTokenizer._symbol_regex.sub(r" \1 ", scoped_text)
         return list(map(self._create_token, EnglishTokenizer._model(scoped_text)))
 
     def _create_token(self, token: Any) -> Token:
         if EnglishTokenizer._symbol_regex.fullmatch(token.text):
             return Token("en", token.text, "SYM", "*", "*", token.text)
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/japanese.py` & `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/japanese.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import re
 from itertools import accumulate
-from typing import Any, List
+from typing import Any
 
 import ja_core_news_sm
 
 from py_pdf_term._common.consts import JAPANESE_REGEX, NOSPACE_REGEX, SYMBOL_REGEX
 
 from .base import BaseLanguageTokenizer
 from .data import Token
 
 SPACES = re.compile(r"\s+")
 DELIM_SPACE = re.compile(rf"(?<={NOSPACE_REGEX}) (?={NOSPACE_REGEX})")
 
 
 class JapaneseTokenizer(BaseLanguageTokenizer):
-    """A tokenizer for Japanese. This tokenizer uses SpaCy's ja_core_news_sm model."""
+    """Tokenizer for Japanese. This tokenizer uses SpaCy's ja_core_news_sm model."""
 
     def inscope(self, text: str) -> bool:
         return JapaneseTokenizer._regex.search(text) is not None
 
-    def tokenize(self, scoped_text: str) -> List[Token]:
+    def tokenize(self, scoped_text: str) -> list[Token]:
         scoped_text = SPACES.sub(" ", scoped_text).strip()
         orginal_space_pos = {
-            match.start() - offset
-            for offset, match in enumerate(re.finditer(r" ", scoped_text))
-            if DELIM_SPACE.match(scoped_text, match.start()) is not None
+            regex_match.start() - offset
+            for offset, regex_match in enumerate(re.finditer(r" ", scoped_text))
+            if DELIM_SPACE.match(scoped_text, regex_match.start()) is not None
         }
 
         scoped_text = DELIM_SPACE.sub("", scoped_text)
         scoped_text = JapaneseTokenizer._symbol_regex.sub(r" \1 ", scoped_text)
         tokens = list(map(self._create_token, JapaneseTokenizer._model(scoped_text)))
 
         if not orginal_space_pos:
```

### Comparing `py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/tokenizer.py` & `py_pdf_term-1.0.2/py_pdf_term/tokenizers/_tokenizers/tokenizer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-from typing import List, Optional
-
 from .base import BaseLanguageTokenizer
 from .data import Token
 from .english import EnglishTokenizer
 from .japanese import JapaneseTokenizer
 
 
 class Tokenizer:
-    """A tokenizer for multiple languages. This tokenizer uses SpaCy.
+    """Tokenizer for multiple languages. This tokenizer uses SpaCy.
 
     Args
     ----
         lang_tokenizers:
-            A list of language tokenizers. The order of the language tokenizers is
+            List of language tokenizers. The order of the language tokenizers is
             important. The first language tokenizer that returns True in inscope() is
             used. If None, this tokenizer uses the default language tokenizers. The
             default language tokenizers are JapaneseTokenizer and EnglishTokenizer.
     """
 
     def __init__(
-        self, lang_tokenizers: Optional[List[BaseLanguageTokenizer]] = None
+        self, lang_tokenizers: list[BaseLanguageTokenizer] | None = None
     ) -> None:
         if lang_tokenizers is None:
             lang_tokenizers = [JapaneseTokenizer(), EnglishTokenizer()]
 
         self._lang_tokenizers = lang_tokenizers
 
-    def tokenize(self, text: str) -> List[Token]:
+    def tokenize(self, text: str) -> list[Token]:
         """Tokenize text into tokens.
 
         Args
         ----
             text:
-                A text to tokenize.
+                Text to tokenize.
 
         Returns
         -------
-            List[Token]:
-                A list of tokens.
+            list[Token]:
+                List of tokens.
         """
 
         if not text:
             return []
 
         for tokenizer in self._lang_tokenizers:
             if tokenizer.inscope(text):
```

### Comparing `py_pdf_term-1.0.0/pyproject.toml` & `py_pdf_term-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-pdf-term"
-version = "1.0.0"
+version = "1.0.2"
 description = "A fully-configurable terminology extraction module written in Python"
 authors = ["Yuya Suwa"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/kumachan-mis/py-pdf-term"
 repository = "https://github.com/kumachan-mis/py-pdf-term"
 keywords = ["terminology extraction", "technical term", "pdf"]
@@ -20,15 +20,15 @@
 flake8-quotes = "^3.3.2"
 ghp-import = "^2.1.0"
 isort = "^5.12.0"
 pep8-naming = "^0.13.3"
 pre-commit = "^3.3.2"
 pytest-mock = "^3.10.0"
 pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 Sphinx = "^7.0.1"
 
 [tool.poetry.group.dev.dependencies.en_core_web_sm]
 url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz"
 
 [tool.poetry.group.dev.dependencies.ja_core_news_sm]
 url = "https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.5.0/ja_core_news_sm-3.5.0.tar.gz"
```

### Comparing `py_pdf_term-1.0.0/PKG-INFO` & `py_pdf_term-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-pdf-term
-Version: 1.0.0
+Version: 1.0.2
 Summary: A fully-configurable terminology extraction module written in Python
 Home-page: https://github.com/kumachan-mis/py-pdf-term
 License: MIT
 Keywords: terminology extraction,technical term,pdf
 Author: Yuya Suwa
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

