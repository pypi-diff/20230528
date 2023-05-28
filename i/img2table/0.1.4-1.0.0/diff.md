# Comparing `tmp/img2table-0.1.4.tar.gz` & `tmp/img2table-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-0.1.4.tar", last modified: Mon May 22 19:44:18 2023, max compression
+gzip compressed data, was "dist/img2table-1.0.0.tar", last modified: Sun May 28 18:07:32 2023, max compression
```

## Comparing `img2table-0.1.4.tar` & `img2table-1.0.0.tar`

### file list

```diff
@@ -1,275 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 19:41:35.000000 img2table-0.1.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-22 19:41:35.000000 img2table-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-22 19:41:35.000000 img2table-0.1.4/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 19:41:35.000000 img2table-0.1.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-22 19:41:35.000000 img2table-0.1.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-22 19:44:18.000000 img2table-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-05-22 19:41:35.000000 img2table-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-22 19:41:35.000000 img2table-0.1.4/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46047 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18538 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/borderless_aws.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/borderless_ocr.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-22 19:41:35.000000 img2table-0.1.4/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-22 19:41:35.000000 img2table-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-22 19:41:35.000000 img2table-0.1.4/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-22 19:41:35.000000 img2table-0.1.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-22 19:41:35.000000 img2table-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-22 19:44:18.000000 img2table-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 19:41:35.000000 img2table-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-22 19:41:35.000000 img2table-0.1.4/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 19:44:18.000000 img2table-0.1.4/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/dark.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/image/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/contours.json
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:18.000000 img2table-0.1.4/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-22 19:41:35.000000 img2table-0.1.4/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-28 18:04:08.000000 img2table-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-28 18:04:08.000000 img2table-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-28 18:04:08.000000 img2table-1.0.0/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 18:04:08.000000 img2table-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-28 18:04:08.000000 img2table-1.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-05-28 18:07:32.000000 img2table-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17155 2023-05-28 18:04:08.000000 img2table-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-28 18:04:08.000000 img2table-1.0.0/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46280 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   728008 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/examples/data/borderless/
+-rw-r--r--   0 runner    (1001) docker     (123)    47122 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/borderless/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   177004 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/borderless/2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   182800 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/borderless/3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132335 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/borderless/4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/borderless.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-28 18:04:08.000000 img2table-1.0.0/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-28 18:04:08.000000 img2table-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-28 18:04:08.000000 img2table-1.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-28 18:04:08.000000 img2table-1.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-28 18:04:08.000000 img2table-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-28 18:07:32.000000 img2table-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-28 18:04:08.000000 img2table-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/easyocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/rows/coherency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-28 18:04:08.000000 img2table-1.0.0/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10485 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 18:07:32.000000 img2table-1.0.0/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)   346353 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/image/test_data/dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/easyocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/easyocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/easyocr/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/easyocr/test_data/ocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/easyocr/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/easyocr/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/easyocr/test_easyocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    34981 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/image/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/image/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_data/contours.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/borderless_tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/column_delimiters/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/test_coherency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/rows/test_rows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50091 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_data/rows.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10673 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:07:32.000000 img2table-1.0.0/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-28 18:04:08.000000 img2table-1.0.0/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-0.1.4/LICENSE.txt` & `img2table-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/Makefile` & `img2table-1.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/PKG-INFO` & `img2table-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.4
+Version: 1.0.0
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -29,14 +29,15 @@
         
         ## Installation <a name="installation"></a>
         The library can be installed via pip:
         
         > <code>pip install img2table</code>: Standard installation, supporting Tesseract<br>
         > <code>pip install img2table[paddle]</code>: For usage with Paddle OCR (Python <= 3.10 only)<br>
         > <code>pip install img2table[paddle-gpu]</code>: For usage with Paddle OCR - GPU (Python <= 3.10 only)<br>
+        > <code>pip install img2table[easyocr]</code>: For usage with EasyOCR<br>
         > <code>pip install img2table[gcp]</code>: For usage with Google Vision OCR<br>
         > <code>pip install img2table[aws]</code>: For usage with AWS Textract OCR<br>
         > <code>pip install img2table[azure]</code>: For usage with Azure Cognitive Services OCR
         
         ## Features <a name="features"></a>
         
         * Table identification for images and PDF files, including bounding boxes at the table cell level
@@ -111,25 +112,28 @@
         #### PDF <a name="pdf-doc"></a>
         PDF files are instantiated as follows :
         ```python
         from img2table.document import PDF
         
         pdf = PDF(src, 
                   pages=[0, 2],
-                  detect_rotation=False)
+                  detect_rotation=False,
+                  pdf_text_extraction=True)
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">PDF source</dd>
         >    <dt>pages : list, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
         >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Detect and correct skew/rotation of extracted images from the PDF</dd>
+        >    <dt>pdf_text_extraction : bool, optional, default <code>True</code></dt>
+        >    <dd style="font-style: italic;">Extract text from the PDF file for native PDFs</dd>
         ></dl>
         
         PDF pages are converted to images with a 200 DPI for table identification.
         
         ---
         
         ### OCR <a name="ocr"></a>
@@ -189,14 +193,38 @@
         >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
         ></dl>
         
         *Released in version 0.0.13*
         <br>
         </details>
         
+        
+        <details>
+        <summary>EasyOCR<a name="easyocr"></a></summary>
+        <br>
+        
+        <a href="https://github.com/JaidedAI/EasyOCR">EasyOCR</a> is an open-source OCR based on Deep Learning models.<br>
+        At first use, relevant languages models will be downloaded.
+        
+        ```python
+        from img2table.ocr import EasyOCR
+        
+        ocr = EasyOCR(lang=["en"])
+        ```
+        
+        > <h4>Parameters</h4>
+        ><dl>
+        >    <dt>lang : list, optional, default <code>["en"]</code></dt>
+        >    <dd style="font-style: italic;">Lang parameter used in EasyOCR for text extraction, check <a href="https://www.jaided.ai/easyocr">documentation for available languages</a></dd>
+        ></dl>
+        
+        *Released in version 0.1.2*
+        <br>
+        </details>
+        
         <details>
         <summary>Google Vision<a name="vision"></a></summary>
         <br>
         
         Authentication to GCP can be done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment variable.<br>
         If this variable is missing, an API key should be provided via the `api_key` parameter.
         
@@ -295,19 +323,21 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
         >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
-        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
+        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted.</dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         
+        <b>NB</b>: Borderless table extraction can, by design, only extract tables with 3 or more columns.
+        
         *Borderless table extraction released in version 0.0.14*
         
         #### Method return
         
         The [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is used to model extracted tables from documents.
         
         > <h4>Attributes</h4>
@@ -406,18 +436,14 @@
         can be found are not returned.
         </li>
         <li>
         The library is tailored for usage on documents with white/light background. 
         Effectiveness can not be guaranteed on other type of documents. 
         </li>
         <li>
-        Borderless tables extraction is still in alpha stage and might be inconsistent on complex cases.
-        Improvements to the algorithm will be released in future versions.
-        </li>
-        <li>
         Table detection using only OpenCV processing can have some limitations. If the library fails to detect tables, 
         you may check CNN based solutions like <a href="https://github.com/DevashishPrasad/CascadeTabNet">CascadeTabNet</a> or 
         the <a href="https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.6/ppstructure/docs/quickstart_en.md#224-table-recognition">PaddleOCR implementation</a>.
         </li>
         </ul>
         
         
@@ -428,7 +454,8 @@
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: gcp
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: paddle
 Provides-Extra: paddle_gpu
+Provides-Extra: easyocr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.4 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.0 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -13,14 +13,15 @@
 extract) * [Excel export](#xlsx) * [Examples](#examples) * [Caveats / FYI]
 (#fyi) ## Installation  The library can be installed via pip: > pip install
 img2table: Standard installation, supporting Tesseract
 > pip install img2table[paddle]: For usage with Paddle OCR (Python <= 3.10
 only)
 > pip install img2table[paddle-gpu]: For usage with Paddle OCR - GPU (Python <=
 3.10 only)
+> pip install img2table[easyocr]: For usage with EasyOCR
 > pip install img2table[gcp]: For usage with Google Vision OCR
 > pip install img2table[aws]: For usage with AWS Textract OCR
 > pip install img2table[azure]: For usage with Azure Cognitive Services OCR ##
 Features  * Table identification for images and PDF files, including bounding
 boxes at the table cell level * Handling of complex table structures such as
 merged cells * Handling of implicit rows - see [example](/examples/
 Implicit_rows.ipynb) * Table content extraction by providing support for OCR
@@ -52,15 +53,15 @@
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
 Setting the detect_rotation parameter to True, image coordinates and bounding
 boxes returned by other methods might not correspond to the original image.
 #### PDF  PDF files are instantiated as follows : ```python from
 img2table.document import PDF pdf = PDF(src, pages=[0, 2],
-detect_rotation=False) ``` >
+detect_rotation=False, pdf_text_extraction=True) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
 If possible (i.e for native PDF), PDF text will be extracted directly from the
@@ -78,14 +79,22 @@
 on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
 *Released in version 0.0.13*
+  EasyOCR
+EasyOCR is an open-source OCR based on Deep Learning models.
+At first use, relevant languages models will be downloaded. ```python from
+img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
+*** Parameters ***
+>
+>
+*Released in version 0.1.2*
   Google Vision
 Authentication to GCP can be done by setting the standard
 `GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
@@ -119,17 +128,18 @@
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) # Table
 extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=False,
 borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
-*Borderless table extraction released in version 0.0.14* #### Method return The
-[`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
-used to model extracted tables from documents. >
+NB: Borderless table extraction can, by design, only extract tables with 3 or
+more columns. *Borderless table extraction released in version 0.0.14* ####
+Method return The [`ExtractedTable`](/src/img2table/tables/objects/
+extraction.py#L35) class is used to model extracted tables from documents. >
 *** Attributes ***
 >
 >
 ** Images **
 `extract_tables` method from the `Image` class returns a list of
 `ExtractedTable` objects. ```Python output = [ExtractedTable(...),
 ExtractedTable(...), ...] ```
@@ -162,18 +172,15 @@
       extract_tables method
 ## Caveats / FYI
     * For table extraction, results are highly dependent on OCR quality. By
       design, tables where no OCR data can be found are not returned.
     * The library is tailored for usage on documents with white/light
       background. Effectiveness can not be guaranteed on other type of
       documents.
-    * Borderless tables extraction is still in alpha stage and might be
-      inconsistent on complex cases. Improvements to the algorithm will be
-      released in future versions.
     * Table detection using only OpenCV processing can have some limitations.
       If the library fails to detect tables, you may check CNN based solutions
       like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
-Provides-Extra: paddle Provides-Extra: paddle_gpu
+Provides-Extra: paddle Provides-Extra: paddle_gpu Provides-Extra: easyocr
```

### Comparing `img2table-0.1.4/README.md` & `img2table-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 ## Installation <a name="installation"></a>
 The library can be installed via pip:
 
 > <code>pip install img2table</code>: Standard installation, supporting Tesseract<br>
 > <code>pip install img2table[paddle]</code>: For usage with Paddle OCR (Python <= 3.10 only)<br>
 > <code>pip install img2table[paddle-gpu]</code>: For usage with Paddle OCR - GPU (Python <= 3.10 only)<br>
+> <code>pip install img2table[easyocr]</code>: For usage with EasyOCR<br>
 > <code>pip install img2table[gcp]</code>: For usage with Google Vision OCR<br>
 > <code>pip install img2table[aws]</code>: For usage with AWS Textract OCR<br>
 > <code>pip install img2table[azure]</code>: For usage with Azure Cognitive Services OCR
 
 ## Features <a name="features"></a>
 
 * Table identification for images and PDF files, including bounding boxes at the table cell level
@@ -104,25 +105,28 @@
 #### PDF <a name="pdf-doc"></a>
 PDF files are instantiated as follows :
 ```python
 from img2table.document import PDF
 
 pdf = PDF(src, 
           pages=[0, 2],
-          detect_rotation=False)
+          detect_rotation=False,
+          pdf_text_extraction=True)
 ```
 
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
 >    <dd style="font-style: italic;">PDF source</dd>
 >    <dt>pages : list, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
 >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Detect and correct skew/rotation of extracted images from the PDF</dd>
+>    <dt>pdf_text_extraction : bool, optional, default <code>True</code></dt>
+>    <dd style="font-style: italic;">Extract text from the PDF file for native PDFs</dd>
 ></dl>
 
 PDF pages are converted to images with a 200 DPI for table identification.
 
 ---
 
 ### OCR <a name="ocr"></a>
@@ -182,14 +186,38 @@
 >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
 ></dl>
 
 *Released in version 0.0.13*
 <br>
 </details>
 
+
+<details>
+<summary>EasyOCR<a name="easyocr"></a></summary>
+<br>
+
+<a href="https://github.com/JaidedAI/EasyOCR">EasyOCR</a> is an open-source OCR based on Deep Learning models.<br>
+At first use, relevant languages models will be downloaded.
+
+```python
+from img2table.ocr import EasyOCR
+
+ocr = EasyOCR(lang=["en"])
+```
+
+> <h4>Parameters</h4>
+><dl>
+>    <dt>lang : list, optional, default <code>["en"]</code></dt>
+>    <dd style="font-style: italic;">Lang parameter used in EasyOCR for text extraction, check <a href="https://www.jaided.ai/easyocr">documentation for available languages</a></dd>
+></dl>
+
+*Released in version 0.1.2*
+<br>
+</details>
+
 <details>
 <summary>Google Vision<a name="vision"></a></summary>
 <br>
 
 Authentication to GCP can be done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment variable.<br>
 If this variable is missing, an API key should be provided via the `api_key` parameter.
 
@@ -288,19 +316,21 @@
 > <h4>Parameters</h4>
 ><dl>
 >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
 >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
 >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
 >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
 >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
->    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
+>    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted.</dd>
 >    <dt>min_confidence : int, optional, default <code>50</code></dt>
 >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
 ></dl>
 
+<b>NB</b>: Borderless table extraction can, by design, only extract tables with 3 or more columns.
+
 *Borderless table extraction released in version 0.0.14*
 
 #### Method return
 
 The [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is used to model extracted tables from documents.
 
 > <h4>Attributes</h4>
@@ -399,16 +429,12 @@
 can be found are not returned.
 </li>
 <li>
 The library is tailored for usage on documents with white/light background. 
 Effectiveness can not be guaranteed on other type of documents. 
 </li>
 <li>
-Borderless tables extraction is still in alpha stage and might be inconsistent on complex cases.
-Improvements to the algorithm will be released in future versions.
-</li>
-<li>
 Table detection using only OpenCV processing can have some limitations. If the library fails to detect tables, 
 you may check CNN based solutions like <a href="https://github.com/DevashishPrasad/CascadeTabNet">CascadeTabNet</a> or 
 the <a href="https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.6/ppstructure/docs/quickstart_en.md#224-table-recognition">PaddleOCR implementation</a>.
 </li>
 </ul>
```

#### html2text {}

```diff
@@ -9,14 +9,15 @@
 extraction](#table-extract) * [Excel export](#xlsx) * [Examples](#examples) *
 [Caveats / FYI](#fyi) ## Installation  The library can be installed via pip: >
 pip install img2table: Standard installation, supporting Tesseract
 > pip install img2table[paddle]: For usage with Paddle OCR (Python <= 3.10
 only)
 > pip install img2table[paddle-gpu]: For usage with Paddle OCR - GPU (Python <=
 3.10 only)
+> pip install img2table[easyocr]: For usage with EasyOCR
 > pip install img2table[gcp]: For usage with Google Vision OCR
 > pip install img2table[aws]: For usage with AWS Textract OCR
 > pip install img2table[azure]: For usage with Azure Cognitive Services OCR ##
 Features  * Table identification for images and PDF files, including bounding
 boxes at the table cell level * Handling of complex table structures such as
 merged cells * Handling of implicit rows - see [example](/examples/
 Implicit_rows.ipynb) * Table content extraction by providing support for OCR
@@ -48,15 +49,15 @@
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
 Setting the detect_rotation parameter to True, image coordinates and bounding
 boxes returned by other methods might not correspond to the original image.
 #### PDF  PDF files are instantiated as follows : ```python from
 img2table.document import PDF pdf = PDF(src, pages=[0, 2],
-detect_rotation=False) ``` >
+detect_rotation=False, pdf_text_extraction=True) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
 If possible (i.e for native PDF), PDF text will be extracted directly from the
@@ -74,14 +75,22 @@
 on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
 *Released in version 0.0.13*
+  EasyOCR
+EasyOCR is an open-source OCR based on Deep Learning models.
+At first use, relevant languages models will be downloaded. ```python from
+img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
+*** Parameters ***
+>
+>
+*Released in version 0.1.2*
   Google Vision
 Authentication to GCP can be done by setting the standard
 `GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
@@ -115,17 +124,18 @@
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) # Table
 extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=False,
 borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
-*Borderless table extraction released in version 0.0.14* #### Method return The
-[`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
-used to model extracted tables from documents. >
+NB: Borderless table extraction can, by design, only extract tables with 3 or
+more columns. *Borderless table extraction released in version 0.0.14* ####
+Method return The [`ExtractedTable`](/src/img2table/tables/objects/
+extraction.py#L35) class is used to model extracted tables from documents. >
 *** Attributes ***
 >
 >
 ** Images **
 `extract_tables` method from the `Image` class returns a list of
 `ExtractedTable` objects. ```Python output = [ExtractedTable(...),
 ExtractedTable(...), ...] ```
@@ -158,13 +168,10 @@
       extract_tables method
 ## Caveats / FYI
     * For table extraction, results are highly dependent on OCR quality. By
       design, tables where no OCR data can be found are not returned.
     * The library is tailored for usage on documents with white/light
       background. Effectiveness can not be guaranteed on other type of
       documents.
-    * Borderless tables extraction is still in alpha stage and might be
-      inconsistent on complex cases. Improvements to the algorithm will be
-      released in future versions.
     * Table detection using only OpenCV processing can have some limitations.
       If the library fails to detect tables, you may check CNN based solutions
       like CascadeTabNet or the PaddleOCR_implementation.
```

### Comparing `img2table-0.1.4/examples/Basic_usage.ipynb` & `img2table-1.0.0/examples/Basic_usage.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985180607956216%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['time: 235 ms (started: 2023-05-04 21:44:08 "*

 * *            "+02:00)\\n']}}}, 4: {'metadata': {delete: ['collapsed']}, 'outputs': {0: {'text': "*

 * *            "['time: 4.33 s (started: 2023-05-04 21:44:10 +02:00)\\n']}}}, 6: {'outputs': {0: "*

 * *            "{'text': ['time: 0 ns (started: 2023-05-04 21:44:15 +02:00)\\n']}}}, 7: {'source': "*

 * *            "{insert: [(5, '  * EasyOCR\\n'), (8, '  * Azure Cognitive Services\\n'), (9, '  "*

 * *            "\\n'), (10, 'For all OCR […]*

```diff
@@ -21,15 +21,15 @@
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 235 ms (started: 2023-03-28 22:34:56 +02:00)\n"
+                        "time: 235 ms (started: 2023-05-04 21:44:08 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "%load_ext autotime\n",
                 "\n",
                 "from IPython.display import display_html\n",
@@ -58,28 +58,27 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "6e7b95fa",
             "metadata": {
-                "collapsed": true,
                 "execution": {
                     "iopub.execute_input": "2023-03-28T20:34:56.334168Z",
                     "iopub.status.busy": "2023-03-28T20:34:56.334168Z",
                     "iopub.status.idle": "2023-03-28T20:34:59.191605Z",
                     "shell.execute_reply": "2023-03-28T20:34:59.191605Z"
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 2.84 s (started: 2023-03-28 22:34:56 +02:00)\n"
+                        "time: 4.33 s (started: 2023-05-04 21:44:10 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "from img2table.document import Image\n",
                 "\n",
                 "img_path = \"data/tables.png\"\n",
@@ -117,15 +116,15 @@
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 0 ns (started: 2023-03-28 22:34:59 +02:00)\n"
+                        "time: 0 ns (started: 2023-05-04 21:44:15 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "from img2table.document import PDF\n",
                 "\n",
                 "pdf_path = \"data/tables.pdf\"\n",
@@ -149,17 +148,20 @@
             "metadata": {},
             "source": [
                 "### OCR instances\n",
                 "\n",
                 "<code>img2table</code> provides supports for several OCR tools and services :\n",
                 "  * Tesseract\n",
                 "  * PaddleOCR\n",
+                "  * EasyOCR\n",
                 "  * Google Vision\n",
                 "  * AWS Textract\n",
-                "  * Azure Cognitive Services"
+                "  * Azure Cognitive Services\n",
+                "  \n",
+                "For all OCRs except Tesseract, a specific installation is needed. Check README for relevant instructions."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "92778211",
             "metadata": {
@@ -171,29 +173,34 @@
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 906 ms (started: 2023-03-28 22:34:59 +02:00)\n"
+                        "time: 2.61 s (started: 2023-05-04 21:44:17 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "# Tesseract OCR\n",
                 "from img2table.ocr import TesseractOCR\n",
                 "\n",
                 "tesseract_ocr = TesseractOCR(n_threads=1, lang=\"eng\")\n",
                 "\n",
                 "# PaddleOCR\n",
                 "from img2table.ocr import PaddleOCR\n",
                 "\n",
                 "paddle_ocr = PaddleOCR(lang=\"en\")\n",
                 "\n",
+                "# EasyOCR\n",
+                "from img2table.ocr import EasyOCR\n",
+                "\n",
+                "easyocr = EasyOCR(lang=[\"en\"])\n",
+                "\n",
                 "# Google Vision OCR\n",
                 "from img2table.ocr import VisionOCR\n",
                 "\n",
                 "vision_ocr = VisionOCR(api_key=\"***\")\n",
                 "\n",
                 "# AWS Textract OCR\n",
                 "from img2table.ocr import TextractOCR\n",
@@ -234,15 +241,15 @@
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 63 ms (started: 2023-03-28 22:35:00 +02:00)\n"
+                        "time: 94 ms (started: 2023-05-04 21:44:19 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "img = Image(src=\"data/tables.png\")\n",
                 "\n",
                 "# Extract tables\n",
@@ -260,28 +267,28 @@
                     "iopub.status.idle": "2023-03-28T20:35:00.260258Z",
                     "shell.execute_reply": "2023-03-28T20:35:00.260258Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD6R/4HAAAAAED/yP8AAAAAAOgf+R8AAAAAAP0j/wMAAAAAoH/kfwAAAAAA9I/8DwAAAACA/pH/AQAAAADQP/I/AAAAAAD69/8Bmd+622f7NwAAAABJRU5ErkJggg==",
                         "text/plain": [
                             "<PIL.Image.Image image mode=RGB size=1365x417>"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 31 ms (started: 2023-03-28 22:35:00 +02:00)\n"
+                        "time: 32 ms (started: 2023-05-04 21:44:19 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "# Display extracted tables\n",
                 "table_img = cv2.imread(\"data/tables.png\")\n",
                 "\n",
@@ -316,29 +323,29 @@
                     "shell.execute_reply": "2023-03-28T20:35:00.918518Z"
                 }
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{0: [ExtractedTable(title=Example of Data Table 1, bbox=(236, 249, 1442, 543),shape=(5, 4)),\n",
+                            "{0: [ExtractedTable(title=Example of Data Table 1, bbox=(235, 249, 1442, 543),shape=(5, 4)),\n",
                             "  ExtractedTable(title=Example of Data Table 2, bbox=(235, 671, 1451, 971),shape=(5, 4))],\n",
                             " 1: [ExtractedTable(title=Example of Data Table 3, bbox=(236, 249, 1442, 543),shape=(5, 4)),\n",
                             "  ExtractedTable(title=Example of Data Table 4, bbox=(235, 671, 1451, 971),shape=(5, 4))]}"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 625 ms (started: 2023-03-28 22:35:00 +02:00)\n"
+                        "time: 906 ms (started: 2023-05-04 21:44:21 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "pdf = PDF(src=\"data/tables.pdf\")\n",
                 "\n",
                 "# Extract tables\n",
@@ -365,15 +372,15 @@
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<h3 style=\"text-align: center\">Page 1 - Extracted table n\u00b01</h3>\n",
                             "                   <p style=\"text-align: center\">\n",
                             "                       <b>Title:</b> Example of Data Table 1<br>\n",
-                            "                       <b>Bounding box:</b> x1=236, y1=249, x2=1442, y2=543\n",
+                            "                       <b>Bounding box:</b> x1=235, y1=249, x2=1442, y2=543\n",
                             "                   </p>\n",
                             "                   <div align=\"center\"><table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>0</th>\n",
                             "      <th>1</th>\n",
@@ -615,15 +622,15 @@
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 16 ms (started: 2023-03-28 22:35:00 +02:00)\n"
+                        "time: 15 ms (started: 2023-05-04 21:44:21 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "for page, tables in extracted_tables.items():\n",
                 "    for idx, table in enumerate(tables):\n",
                 "        display_html(table.html_repr(title=f\"Page {page + 1} - Extracted table n\u00b0{idx + 1}\"), raw=True)"
@@ -653,15 +660,15 @@
                 }
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "time: 625 ms (started: 2023-03-28 22:35:00 +02:00)\n"
+                        "time: 890 ms (started: 2023-05-04 21:44:23 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "pdf = PDF(src=\"data/tables.pdf\")\n",
                 "\n",
                 "# Export to file\n",
@@ -689,15 +696,15 @@
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Worksheet Page 1 - Table 1 : 5 rows, 4 columns\n",
                         "Worksheet Page 1 - Table 2 : 5 rows, 4 columns\n",
                         "Worksheet Page 2 - Table 1 : 5 rows, 4 columns\n",
                         "Worksheet Page 2 - Table 2 : 5 rows, 4 columns\n",
-                        "time: 0 ns (started: 2023-03-28 22:35:01 +02:00)\n"
+                        "time: 0 ns (started: 2023-05-04 21:44:25 +02:00)\n"
                     ]
                 }
             ],
             "source": [
                 "for ws in load_workbook(\"data/tables.xlsx\"):\n",
                 "    print(f\"Worksheet {ws.title} : {len(tuple(ws.rows))} rows, {len(tuple(ws.rows)[0])} columns\")"
             ]
```

### Comparing `img2table-0.1.4/examples/Implicit_rows.ipynb` & `img2table-1.0.0/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/examples/data/borderless_ocr.jpg` & `img2table-1.0.0/examples/data/borderless.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/examples/data/implicit.png` & `img2table-1.0.0/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/examples/data/tables.pdf` & `img2table-1.0.0/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/examples/data/tables.png` & `img2table-1.0.0/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/examples/data/tables.xlsx` & `img2table-1.0.0/examples/data/tables.xlsx`

 * *Files 6% similar despite different names*

```diff
@@ -379,111 +379,111 @@
 000017a0: dd6c 71dd 5bfb 519b c2e1 0365 5fd0 b8a9  .lq.[.Q....e_...
 000017b0: f0d9 62be 1df0 0388 3e9a 4f94 0812 f152  ..b.....>.O....R
 000017c0: ab2c bff9 e610 746e 69c6 65ac fed9 316a  .,....tni.e...1j
 000017d0: 1182 d68a 785f e4f0 a939 bbb1 c2d9 678b  ....x_...9....g.
 000017e0: 7b73 677b 065f 7b67 bbda 5e2e 515b 3bc8  {sg{._{g..^.Q[;.
 000017f0: e4ab a53f 9ef8 f03e c8de 8183 d284 2959  ...?...>......)Y
 00001800: bc4d 7a00 47cd eeec 2f03 e063 2f48 b7fe  .Mz.G.../..c/H..
-00001810: 0650 4b03 0414 0000 0008 0000 0021 00af  .PK..........!..
-00001820: c9a7 2724 0100 0050 0200 0011 0000 0064  ..'$...P.......d
+00001810: 0650 4b03 0414 0000 0008 0000 0021 0031  .PK..........!.1
+00001820: c9df 0425 0100 0050 0200 0011 0000 0064  ...%...P.......d
 00001830: 6f63 5072 6f70 732f 636f 7265 2e78 6d6c  ocProps/core.xml
-00001840: 9d92 cd6a c330 1084 ef7d 0aa3 bb2d d9a6  ...j.0...}...-..
-00001850: 2508 db81 b6e4 d440 a12e 2dbd 0969 9388  %......@..-..i..
-00001860: 5a3f 486a 1dbf 7d15 2771 12f0 a9c7 d5cc  Z?Hj..}.'q......
-00001870: 7e3b bba8 5aee 5597 fc82 f3d2 e81a e519  ~;..Z.U.........
-00001880: 4109 686e 84d4 db1a bdb7 ab74 8112 1f98  A.hn.......t....
-00001890: 16ac 331a 6a34 8047 cbe6 aee2 9672 e3e0  ..3.j4.G.....r..
-000018a0: d519 0b2e 48f0 4904 694f b9ad d12e 044b  ....H.I.iO.....K
-000018b0: 31f6 7c07 8af9 2c3a 7414 37c6 2916 62e9  1.|...,:t.7.).b.
-000018c0: b6d8 32fe cdb6 800b 421e b082 c004 0b0c  ..2.....B.......
-000018d0: 1f80 a99d 88e8 8414 7c42 da1f d78d 00c1  ........|B......
-000018e0: 3174 a040 078f f32c c717 6f00 a7fc 6cc3  1t.@...,..o...l.
-000018f0: a85c 3995 0c83 8559 eb59 9cdc 7b2f 2763  .\9....Y.Y..{/'c
-00001900: dff7 595f 8ed6 983f c79f eb97 b771 d554  ..Y_...?.....q.T
-00001910: eac3 a938 a0a6 129c 7207 2c18 d754 f8ba  ...8....r.,..T..
-00001920: 8887 eb98 0feb 78e2 8d04 f138 447d e6ed  ......x....8D}..
-00001930: b4c8 b10f 4412 03d0 63dc b3f2 513e 3db7  ....D...c...Q>=.
-00001940: 2bd4 14a4 2853 52a6 c5a2 2d08 2def 29c9  +...(SR...-.-.).
-00001950: bf0e 236f fa2f 4075 1af2 6fe2 1970 cc7d  ..#o./@u..o..p.}
-00001960: fb09 9a3f 504b 0304 1400 0000 0800 0000  ...?PK..........
-00001970: 2100 f344 c974 8d01 0000 8903 0000 1000  !..D.t..........
-00001980: 0000 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
-00001990: 6d6c 9d53 5d6b db30 147d dfaf 107a 4fe4  ml.S]k.0.}...zO.
-000019a0: 9830 4690 5546 dad2 878d 05e2 76cf b7f2  .0F.UF......v...
-000019b0: 752c 2a4b 46ba 35c9 7efd 6487 b8ce d6c2  u,*KF.5.~.d.....
-000019c0: 989e cebd f770 38f7 43f2 e6d8 5ad6 6388  .....p8.C...Z.c.
-000019d0: c6bb 82af 9619 67e8 b4af 8c3b 14fc b1bc  ......g....;....
-000019e0: 5f7c e12c 12b8 0aac 7758 f013 467e a33e  _|.,....wX..F~.>
-000019f0: c95d f01d 0632 1859 5270 b1e0 0d51 b711  .]...2.YRp...Q..
-00001a00: 22ea 065b 88cb 5476 a952 fbd0 02a5 301c  "..[..Tv.R....0.
-00001a10: 84af 6ba3 f1d6 ebd7 161d 893c cb3e 0b3c  ..k........<.>.<
-00001a20: 12ba 0aab 4537 09f2 b3e2 a6a7 ff15 adbc  ....E7..........
-00001a30: 1efc c5a7 f2d4 253d 25bf 769d 351a 2835  ......%=%.v.5.(5
-00001a40: a9be 1b1d 7cf4 35b1 bba3 462b c5bc 2893  ....|.5...F+..(.
-00001a50: d01e f56b 3074 5299 14f3 50ee 3558 dc26  ...k0tR...P.5X.&
-00001a60: 6155 838d 28c5 5b42 3e20 0c33 db81 0951  aU..(.[B> .3...Q
-00001a70: c99e 363d 6af2 8145 f32b 4d2d e7ec 1922  ..6=j..E.+M-..."
-00001a80: 0e76 0ade 4330 e088 9f69 e760 c4b6 8b14  .v..C0...i.`....
-00001a90: d44f 1f5e 6283 4851 8a29 39c2 3977 8ecd  .O.^b.HQ.)9.9w..
-00001aa0: 5aad 4742 02d7 4431 1949 f8da 6269 c862  Z.GB..D1.I..bi.b
-00001ab0: fc51 ef20 d03b 8ed7 73c7 a307 3ef3 b883  .Q. .;..s...>...
-00001ac0: 03b2 155b b012 9e6d 4273 a71f 91f2 8f49  ...[...mBs.....I
-00001ad0: f9bf 28e5 ef2b 5db5 f847 535b df76 e0d2  ..(..+]..GS[.v..
-00001ae0: e6c4 84be 19f7 121f bbd2 df02 e165 8fd7  .............e..
-00001af0: 49b9 6f20 6095 563f ed79 4ac8 8734 9060  I.o `.V?.yJ..4.`
-00001b00: 07fe b601 77c0 eac2 f9bb 305c ddd3 f967  ....w.....0\...g
-00001b10: a955 becc d21b 8fed 9293 e2ed 13a9 df50  .U.............P
-00001b20: 4b01 0214 0014 0000 0008 0000 0021 004e  K............!.N
-00001b30: fd85 db5d 0100 0027 0600 0013 0000 0000  ...]...'........
-00001b40: 0000 0000 0000 0080 0100 0000 005b 436f  .............[Co
-00001b50: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
-00001b60: 504b 0102 1400 1400 0000 0800 0000 2100  PK............!.
-00001b70: f29f 49da e900 0000 4b02 0000 0b00 0000  ..I.....K.......
-00001b80: 0000 0000 0000 0000 8001 8e01 0000 5f72  .............._r
-00001b90: 656c 732f 2e72 656c 7350 4b01 0214 0014  els/.relsPK.....
-00001ba0: 0000 0008 0000 0021 00d8 d7ba 39fe 0000  .......!....9...
-00001bb0: 0060 0400 001a 0000 0000 0000 0000 0000  .`..............
-00001bc0: 0080 01a0 0200 0078 6c2f 5f72 656c 732f  .......xl/_rels/
-00001bd0: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
-00001be0: 7350 4b01 0214 0014 0000 0008 0000 0021  sPK............!
-00001bf0: 00e5 fc2a f701 0200 0032 0600 0018 0000  ...*.....2......
-00001c00: 0000 0000 0000 0000 0080 01d6 0300 0078  ...............x
-00001c10: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00001c20: 6574 312e 786d 6c50 4b01 0214 0014 0000  et1.xmlPK.......
-00001c30: 0008 0000 0021 0062 dde9 9ffd 0100 0029  .....!.b.......)
-00001c40: 0600 0018 0000 0000 0000 0000 0000 0080  ................
-00001c50: 010d 0600 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00001c60: 7473 2f73 6865 6574 322e 786d 6c50 4b01  ts/sheet2.xmlPK.
-00001c70: 0214 0014 0000 0008 0000 0021 001f 97e8  ...........!....
-00001c80: 27f8 0100 0028 0600 0018 0000 0000 0000  '....(..........
-00001c90: 0000 0000 0080 0140 0800 0078 6c2f 776f  .......@...xl/wo
-00001ca0: 726b 7368 6565 7473 2f73 6865 6574 332e  rksheets/sheet3.
-00001cb0: 786d 6c50 4b01 0214 0014 0000 0008 0000  xmlPK...........
-00001cc0: 0021 009d 8599 e2fd 0100 002c 0600 0018  .!.........,....
-00001cd0: 0000 0000 0000 0000 0000 0080 016e 0a00  .............n..
-00001ce0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00001cf0: 6865 6574 342e 786d 6c50 4b01 0214 0014  heet4.xmlPK.....
-00001d00: 0000 0008 0000 0021 0065 8a3e 026d 0100  .......!.e.>.m..
-00001d10: 00d8 0200 000f 0000 0000 0000 0000 0000  ................
-00001d20: 0080 01a1 0c00 0078 6c2f 776f 726b 626f  .......xl/workbo
-00001d30: 6f6b 2e78 6d6c 504b 0102 1400 1400 0000  ok.xmlPK........
-00001d40: 0800 0000 2100 e13f 0097 b001 0000 1e06  ....!..?........
-00001d50: 0000 1400 0000 0000 0000 0000 0000 8001  ................
-00001d60: 3b0e 0000 786c 2f73 6861 7265 6453 7472  ;...xl/sharedStr
-00001d70: 696e 6773 2e78 6d6c 504b 0102 1400 1400  ings.xmlPK......
-00001d80: 0000 0800 0000 2100 8b87 bedb e801 0000  ......!.........
-00001d90: c604 0000 0d00 0000 0000 0000 0000 0000  ................
-00001da0: 8001 1d10 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
-00001db0: 786d 6c50 4b01 0214 0014 0000 0008 0000  xmlPK...........
-00001dc0: 0021 0018 fa46 54b0 0500 0052 1b00 0013  .!...FT....R....
-00001dd0: 0000 0000 0000 0000 0000 0080 0130 1200  .............0..
-00001de0: 0078 6c2f 7468 656d 652f 7468 656d 6531  .xl/theme/theme1
-00001df0: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
-00001e00: 0000 2100 afc9 a727 2401 0000 5002 0000  ..!....'$...P...
-00001e10: 1100 0000 0000 0000 0000 0000 8001 1118  ................
-00001e20: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
-00001e30: 786d 6c50 4b01 0214 0014 0000 0008 0000  xmlPK...........
-00001e40: 0021 00f3 44c9 748d 0100 0089 0300 0010  .!..D.t.........
-00001e50: 0000 0000 0000 0000 0000 0080 0164 1900  .............d..
-00001e60: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
-00001e70: 6c50 4b05 0600 0000 000d 000d 0052 0300  lPK..........R..
-00001e80: 001f 1b00 0000 00                        .......
+00001840: 9d92 cb4e c330 1045 f77c 45e4 7de2 bc40  ...N.0.E.|E.}..@
+00001850: 6025 a904 a82b 2a21 5104 6267 d9d3 d422  `%...+*!Q.bg..."
+00001860: 7ec8 36a4 fd7b 9ca4 4d5b a92b 96e3 7be7  ~.6..{..M[.+..{.
+00001870: cc9d 91ab c54e 76d1 2f58 27b4 aa51 96a4  .....Nv./X'..Q..
+00001880: 2802 c534 17aa add1 fb7a 19df a3c8 79aa  (..4.....z....y.
+00001890: 38ed b482 1aed c1a1 4573 5331 4398 b6f0  8.......EsS1C...
+000018a0: 6ab5 01eb 05b8 2880 9423 ccd4 68eb bd21  j.....(..#..h..!
+000018b0: 183b b605 495d 121c 2a88 1b6d 25f5 a1b4  .;..I]..*..m%...
+000018c0: 2d36 947d d316 709e a677 5882 a79c 7a8a  -6.}..p..wX...z.
+000018d0: 0760 6c66 223a 2039 9b91 e6c7 7623 8033  .`lf": 9....v#.3
+000018e0: 0c1d 4850 dee1 2cc9 f0c9 ebc1 4a77 b561  ..HP..,.....Jw.a
+000018f0: 54ce 9c52 f8bd 81ab d6a3 38bb 774e ccc6  T..R......8.wN..
+00001900: beef 93be 18ad 217f 863f 572f 6fe3 aab1  ......!..?W/o...
+00001910: 50c3 a918 a0a6 e28c 300b d46b db54 f8bc  P.......0..k.T..
+00001920: 0887 eba8 f3ab 70e2 8d00 feb8 0ffa 95b7  ......p.........
+00001930: c322 531f f028 0420 53dc a3f2 513c 3daf  ."S..(. S...Q<=.
+00001940: 97a8 c9d3 bc88 d3db 382d d7d9 0329 4b92  ........8-...)K.
+00001950: 175f c3c8 8bfe 1350 1e86 fc9b 7804 4cb9  ._.....P....x.L.
+00001960: 2f3f 41f3 0750 4b03 0414 0000 0008 0000  /?A..PK.........
+00001970: 0021 00f3 44c9 748d 0100 0089 0300 0010  .!..D.t.........
+00001980: 0000 0064 6f63 5072 6f70 732f 6170 702e  ...docProps/app.
+00001990: 786d 6c9d 535d 6bdb 3014 7ddf af10 7a4f  xml.S]k.0.}...zO
+000019a0: e498 3046 9055 46da d287 8d05 e276 cfb7  ..0F.UF......v..
+000019b0: f275 2c2a 4b46 ba35 c97e fd64 87b8 ced6  .u,*KF.5.~.d....
+000019c0: c298 9ece bdf7 7038 f743 f2e6 d85a d663  ......p8.C...Z.c
+000019d0: 88c6 bb82 af96 1967 e8b4 af8c 3b14 fcb1  .......g....;...
+000019e0: bc5f 7ce1 2c12 b80a ac77 58f0 1346 7ea3  ._|.,....wX..F~.
+000019f0: 3ec9 5df0 1d06 3218 5952 70b1 e00d 51b7  >.]...2.YRp...Q.
+00001a00: 1122 ea06 5b88 cb54 76a9 52fb d002 a530  ."..[..Tv.R....0
+00001a10: 1c84 af6b a3f1 d6eb d716 1d89 3ccb 3e0b  ...k........<.>.
+00001a20: 3c12 ba0a ab45 3709 f2b3 e2a6 a7ff 15ad  <....E7.........
+00001a30: bc1e fcc5 a7f2 d425 3d25 bf76 9d35 1a28  .......%=%.v.5.(
+00001a40: 35a9 be1b 1d7c f435 b1bb a346 2bc5 bc28  5....|.5...F+..(
+00001a50: 93d0 1ef5 6b30 7452 9914 f350 ee35 58dc  ....k0tR...P.5X.
+00001a60: 2661 5583 8d28 c55b 423e 200c 33db 8109  &aU..(.[B> .3...
+00001a70: 51c9 9e36 3d6a f281 45f3 2b4d 2de7 ec19  Q..6=j..E.+M-...
+00001a80: 220e 760a de43 30e0 889f 69e7 60c4 b68b  ".v..C0...i.`...
+00001a90: 14d4 4f1f 5e62 8348 518a 2939 c239 778e  ..O.^b.HQ.)9.9w.
+00001aa0: cd5a ad47 4202 d744 3119 49f8 da62 69c8  .Z.GB..D1.I..bi.
+00001ab0: 62fc 51ef 20d0 3b8e d773 c7a3 073e f3b8  b.Q. .;..s...>..
+00001ac0: 8303 b215 5bb0 129e 6d42 73a7 1f91 f28f  ....[...mBs.....
+00001ad0: 49f9 bf28 e5ef 2b5d b5f8 4753 5bdf 76e0  I..(..+]..GS[.v.
+00001ae0: d2e6 c484 be19 f712 1fbb d2df 02e1 658f  ..............e.
+00001af0: d749 b96f 2060 9556 3fed 794a c887 3490  .I.o `.V?.yJ..4.
+00001b00: 6007 feb6 0177 c0ea c2f9 bb30 5cdd d3f9  `....w.....0\...
+00001b10: 67a9 55be ccd2 1b8f ed92 93e2 ed13 a9df  g.U.............
+00001b20: 504b 0102 1400 1400 0000 0800 0000 2100  PK............!.
+00001b30: 4efd 85db 5d01 0000 2706 0000 1300 0000  N...]...'.......
+00001b40: 0000 0000 0000 0000 8001 0000 0000 5b43  ..............[C
+00001b50: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+00001b60: 6c50 4b01 0214 0014 0000 0008 0000 0021  lPK............!
+00001b70: 00f2 9f49 dae9 0000 004b 0200 000b 0000  ...I.....K......
+00001b80: 0000 0000 0000 0000 0080 018e 0100 005f  ..............._
+00001b90: 7265 6c73 2f2e 7265 6c73 504b 0102 1400  rels/.relsPK....
+00001ba0: 1400 0000 0800 0000 2100 d8d7 ba39 fe00  ........!....9..
+00001bb0: 0000 6004 0000 1a00 0000 0000 0000 0000  ..`.............
+00001bc0: 0000 8001 a002 0000 786c 2f5f 7265 6c73  ........xl/_rels
+00001bd0: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
+00001be0: 6c73 504b 0102 1400 1400 0000 0800 0000  lsPK............
+00001bf0: 2100 e5fc 2af7 0102 0000 3206 0000 1800  !...*.....2.....
+00001c00: 0000 0000 0000 0000 0000 8001 d603 0000  ................
+00001c10: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00001c20: 6565 7431 2e78 6d6c 504b 0102 1400 1400  eet1.xmlPK......
+00001c30: 0000 0800 0000 2100 62dd e99f fd01 0000  ......!.b.......
+00001c40: 2906 0000 1800 0000 0000 0000 0000 0000  )...............
+00001c50: 8001 0d06 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00001c60: 6574 732f 7368 6565 7432 2e78 6d6c 504b  ets/sheet2.xmlPK
+00001c70: 0102 1400 1400 0000 0800 0000 2100 1f97  ............!...
+00001c80: e827 f801 0000 2806 0000 1800 0000 0000  .'....(.........
+00001c90: 0000 0000 0000 8001 4008 0000 786c 2f77  ........@...xl/w
+00001ca0: 6f72 6b73 6865 6574 732f 7368 6565 7433  orksheets/sheet3
+00001cb0: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
+00001cc0: 0000 2100 9d85 99e2 fd01 0000 2c06 0000  ..!.........,...
+00001cd0: 1800 0000 0000 0000 0000 0000 8001 6e0a  ..............n.
+00001ce0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00001cf0: 7368 6565 7434 2e78 6d6c 504b 0102 1400  sheet4.xmlPK....
+00001d00: 1400 0000 0800 0000 2100 658a 3e02 6d01  ........!.e.>.m.
+00001d10: 0000 d802 0000 0f00 0000 0000 0000 0000  ................
+00001d20: 0000 8001 a10c 0000 786c 2f77 6f72 6b62  ........xl/workb
+00001d30: 6f6f 6b2e 786d 6c50 4b01 0214 0014 0000  ook.xmlPK.......
+00001d40: 0008 0000 0021 00e1 3f00 97b0 0100 001e  .....!..?.......
+00001d50: 0600 0014 0000 0000 0000 0000 0000 0080  ................
+00001d60: 013b 0e00 0078 6c2f 7368 6172 6564 5374  .;...xl/sharedSt
+00001d70: 7269 6e67 732e 786d 6c50 4b01 0214 0014  rings.xmlPK.....
+00001d80: 0000 0008 0000 0021 008b 87be dbe8 0100  .......!........
+00001d90: 00c6 0400 000d 0000 0000 0000 0000 0000  ................
+00001da0: 0080 011d 1000 0078 6c2f 7374 796c 6573  .......xl/styles
+00001db0: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
+00001dc0: 0000 2100 18fa 4654 b005 0000 521b 0000  ..!...FT....R...
+00001dd0: 1300 0000 0000 0000 0000 0000 8001 3012  ..............0.
+00001de0: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
+00001df0: 312e 786d 6c50 4b01 0214 0014 0000 0008  1.xmlPK.........
+00001e00: 0000 0021 0031 c9df 0425 0100 0050 0200  ...!.1...%...P..
+00001e10: 0011 0000 0000 0000 0000 0000 0080 0111  ................
+00001e20: 1800 0064 6f63 5072 6f70 732f 636f 7265  ...docProps/core
+00001e30: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
+00001e40: 0000 2100 f344 c974 8d01 0000 8903 0000  ..!..D.t........
+00001e50: 1000 0000 0000 0000 0000 0000 8001 6519  ..............e.
+00001e60: 0000 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
+00001e70: 6d6c 504b 0506 0000 0000 0d00 0d00 5203  mlPK..........R.
+00001e80: 0000 201b 0000 0000                      .. .....
```

### Comparing `img2table-0.1.4/setup.cfg` & `img2table-1.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 	azure-cognitiveservices-vision-computervision
 paddle = 
 	paddlepaddle:python_version<'3.11'
 	paddleocr>=2.0.6:python_version<'3.11'
 paddle-gpu = 
 	paddlepaddle-gpu:python_version<'3.11'
 	paddleocr>=2.0.6:python_version<'3.11'
+easyocr = 
+	easyocr>=1.7.0
 
 [pbr]
 skip_authors = True
 skip_changelog = True
 skip_reno = True
 
 [egg_info]
```

### Comparing `img2table-0.1.4/src/img2table/__init__.py` & `img2table-1.0.0/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/document/base/__init__.py` & `img2table-1.0.0/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/document/base/rotation.py` & `img2table-1.0.0/src/img2table/document/base/rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/document/image.py` & `img2table-1.0.0/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/document/pdf.py` & `img2table-1.0.0/src/img2table/document/pdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,27 @@
 from img2table.tables.objects.extraction import ExtractedTable
 
 
 @dataclass
 class PDF(Document):
     pages: List[int] = None
     detect_rotation: bool = False
+    pdf_text_extraction: bool = True
 
     def validate_pages(self, value, **_) -> Optional[List[int]]:
         if value is not None:
             if not isinstance(value, list):
                 raise TypeError(f"Invalid type {type(value)} for pages argument")
             if not all(isinstance(x, int) for x in value):
                 raise TypeError("All values in pages argument should be integers")
         return value
 
-    def validate__images(self, value, **_) -> Optional[List[int]]:
+    def validate_pdf_text_extraction(self, value, **_) -> int:
+        if not isinstance(value, bool):
+            raise TypeError(f"Invalid type {type(value)} for pdf_text_extraction argument")
         return value
 
     @cached_property
     def images(self) -> List[np.ndarray]:
         mat = fitz.Matrix(200 / 72, 200 / 72)
         doc = fitz.Document(stream=self.bytes, filetype='pdf')
 
@@ -59,15 +62,15 @@
         Extract tables from document
         :param ocr: OCRInstance object used to extract table content
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :param borderless_tables: boolean indicating if borderless tables should be detected
         :param min_confidence: minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)
         :return: dictionary with page number as key and list of extracted tables as values
         """
-        if not self.detect_rotation:
+        if not self.detect_rotation and self.pdf_text_extraction:
             # Try to get OCRDataframe from PDF
             self.ocr_df = PdfOCR().of(document=self)
 
         return super().extract_tables(ocr=ocr,
                                       implicit_rows=implicit_rows,
                                       borderless_tables=borderless_tables,
                                       min_confidence=min_confidence)
```

### Comparing `img2table-0.1.4/src/img2table/ocr/aws_textract.py` & `img2table-1.0.0/src/img2table/ocr/aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/ocr/azure.py` & `img2table-1.0.0/src/img2table/ocr/azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/ocr/base.py` & `img2table-1.0.0/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/ocr/data.py` & `img2table-1.0.0/src/img2table/ocr/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                                 pl.col('x2').max(),
                                 pl.col('y1').min(),
                                 pl.col('y2').max(),
                                 pl.col('value').alias('value')])
                           .sort([pl.col("y1"), pl.col("x1")])
                           )
 
-        # Concatenate all lines
+        # Concatenate all rows
         text_lines = (df_text_parent.select(pl.col('value'))
                       .collect(streaming=True)
                       .get_column('value')
                       .to_list()
                       )
 
         return "\n".join([" ".join(line).strip() for line in text_lines]).strip() or None
```

### Comparing `img2table-0.1.4/src/img2table/ocr/google_vision.py` & `img2table-1.0.0/src/img2table/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/ocr/paddle.py` & `img2table-1.0.0/src/img2table/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/ocr/pdf.py` & `img2table-1.0.0/src/img2table/ocr/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/ocr/tesseract.py` & `img2table-1.0.0/src/img2table/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/image.py` & `img2table-1.0.0/src/img2table/tables/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         # Compute image metrics
         self.char_length, self.median_line_sep, self.contours = compute_img_metrics(img=self.img)
 
     @cached_property
     def white_img(self) -> np.ndarray:
         white_img = copy.deepcopy(self.img)
 
-        # Draw white lines on detected lines
+        # Draw white rows on detected rows
         for l in self.lines:
             if l.horizontal:
                 cv2.rectangle(white_img, (l.x1 - l.thickness, l.y1), (l.x2 + l.thickness, l.y2), (255, 255, 255),
                               3 * l.thickness)
             elif l.vertical:
                 cv2.rectangle(white_img, (l.x1, l.y1 - l.thickness), (l.x2, l.y2 + l.thickness), (255, 255, 255),
                               2 * l.thickness)
@@ -66,31 +66,31 @@
         :param implicit_rows: boolean indicating if implicit rows are splitted
         :return:
         """
         # Compute parameters for line detection
         minLinLength = maxLineGap = round(0.33 * self.median_line_sep) if self.median_line_sep else self.dpi // 20
         kernel_size = round(0.66 * self.median_line_sep) if self.median_line_sep else self.dpi // 10
 
-        # Detect lines in image
+        # Detect rows in image
         h_lines, v_lines = detect_lines(image=self.img,
                                         contours=self.contours,
                                         char_length=self.char_length,
                                         rho=0.3,
                                         theta=np.pi / 180,
                                         threshold=10,
                                         minLinLength=minLinLength,
                                         maxLineGap=maxLineGap,
                                         kernel_size=kernel_size)
         self.lines = h_lines + v_lines
 
-        # Create cells from lines
+        # Create cells from rows
         cells = get_cells(horizontal_lines=h_lines,
                           vertical_lines=v_lines)
 
-        # Create tables from lines
+        # Create tables from rows
         self.tables = get_tables(cells=cells)
 
         # If necessary, detect implicit rows
         if implicit_rows:
             self.tables = handle_implicit_rows(img=self.white_img,
                                                tables=self.tables)
```

### Comparing `img2table-0.1.4/src/img2table/tables/metrics.py` & `img2table-1.0.0/src/img2table/tables/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,19 +61,19 @@
     else:
         return None, None
 
 
 def compute_median_line_sep(img: np.ndarray, cc: np.ndarray,
                             char_length: float) -> Tuple[Optional[float], Optional[List[Cell]]]:
     """
-    Compute median separation between lines
+    Compute median separation between rows
     :param img: image array
     :param cc: connected components array
     :param char_length: average character length
-    :return: median separation between lines
+    :return: median separation between rows
     """
     # Create image from connected components
     black_img = np.zeros(img.shape, np.uint8)
     for c in cc:
         cv2.rectangle(black_img,
                       (c[cv2.CC_STAT_LEFT], c[cv2.CC_STAT_TOP]),
                       (c[cv2.CC_STAT_LEFT] + c[cv2.CC_STAT_WIDTH], c[cv2.CC_STAT_TOP] + c[cv2.CC_STAT_HEIGHT]),
@@ -133,11 +133,11 @@
     """
     # Compute average character length based on connected components analysis
     char_length, cc_array = compute_char_length(img=img)
 
     if char_length is None:
         return None, None, None
 
-    # Compute median separation between lines
+    # Compute median separation between rows
     median_line_sep, contours = compute_median_line_sep(img=img, cc=cc_array, char_length=char_length)
 
     return char_length, median_line_sep, contours
```

### Comparing `img2table-0.1.4/src/img2table/tables/objects/__init__.py` & `img2table-1.0.0/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/objects/extraction.py` & `img2table-1.0.0/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/objects/line.py` & `img2table-1.0.0/src/img2table/tables/objects/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         # Reallocate coordinates in proper order
         _x1 = min(self.x1, self.x2)
         _x2 = max(self.x1, self.x2)
         _y1 = min(self.y1, self.y2)
         _y2 = max(self.y1, self.y2)
         self.x1, self.x2, self.y1, self.y2 = _x1, _x2, _y1, _y2
 
-        # Correct "almost" horizontal or vertical lines
+        # Correct "almost" horizontal or vertical rows
         if abs(self.angle) <= 5:
             y_val = round((self.y1 + self.y2) / 2)
             self.y2 = self.y1 = y_val
         elif abs(self.angle - 90) <= 5:
             x_val = round((self.x1 + self.x2) / 2)
             self.x2 = self.x1 = x_val
```

### Comparing `img2table-0.1.4/src/img2table/tables/objects/row.py` & `img2table-1.0.0/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/objects/table.py` & `img2table-1.0.0/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.bordered_tables.cells.deduplication import deduplicate_cells
 from img2table.tables.processing.bordered_tables.cells.identification import get_cells_dataframe
 
 
 def get_cells(horizontal_lines: List[Line], vertical_lines: List[Line]) -> List[Cell]:
     """
-    Identify cells from horizontal and vertical lines
-    :param horizontal_lines: list of horizontal lines
-    :param vertical_lines: list of vertical lines
+    Identify cells from horizontal and vertical rows
+    :param horizontal_lines: list of horizontal rows
+    :param vertical_lines: list of vertical rows
     :return: list of all cells in image
     """
-    # Create dataframe with cells from horizontal and vertical lines
+    # Create dataframe with cells from horizontal and vertical rows
     df_cells = get_cells_dataframe(horizontal_lines=horizontal_lines,
                                    vertical_lines=vertical_lines)
     
     # Handle case of empty cells
     if df_cells.collect(streaming=True).height == 0:
         return []
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 import polars as pl
 
 from img2table.tables.objects.line import Line
 
 
 def get_potential_cells_from_h_lines(df_h_lines: pl.LazyFrame) -> pl.LazyFrame:
     """
-    Identify potential cells by matching corresponding horizontal lines
-    :param df_h_lines: dataframe containing horizontal lines
+    Identify potential cells by matching corresponding horizontal rows
+    :param df_h_lines: dataframe containing horizontal rows
     :return: dataframe containing potential cells
     """
     # Create copy of df_h_lines
     df_h_lines_cp = (df_h_lines.clone()
                      .rename({col: f"{col}_" for col in df_h_lines.columns})
                      )
 
-    # Cross join with itself to get pairs of horizontal lines
+    # Cross join with itself to get pairs of horizontal rows
     cross_h_lines = (df_h_lines.join(df_h_lines_cp, how='cross')
                      .filter(pl.col('y1') < pl.col('y1_'))
                      )
 
-    # Compute horizontal correspondences between lines
+    # Compute horizontal correspondences between rows
     cross_h_lines = cross_h_lines.with_columns([
         (((pl.col('x1') - pl.col('x1_')) / pl.col('width')).abs() <= 0.02).alias("l_corresponds"),
         (((pl.col('x2') - pl.col('x2_')) / pl.col('width')).abs() <= 0.02).alias("r_corresponds"),
         (((pl.col('x1') <= pl.col('x1_')) & (pl.col('x1_') <= pl.col('x2')))
          | ((pl.col('x1_') <= pl.col('x1')) & (pl.col('x1') <= pl.col('x2_')))).alias('l_contained'),
         (((pl.col('x1') <= pl.col('x2_')) & (pl.col('x2_') <= pl.col('x2')))
          | ((pl.col('x1_') <= pl.col('x2')) & (pl.col('x2') <= pl.col('x2_')))).alias('r_contained')
     ])
 
-    # Create condition on horizontal correspondence in order to use both lines and filter on relevant combinations
+    # Create condition on horizontal correspondence in order to use both rows and filter on relevant combinations
     matching_condition = ((pl.col('l_corresponds') | pl.col('l_contained'))
                           & (pl.col('r_corresponds') | pl.col('r_contained')))
     cross_h_lines = cross_h_lines.filter(matching_condition)
 
-    # Create cell bbox from horizontal lines
+    # Create cell bbox from horizontal rows
     df_bbox = (cross_h_lines.select([pl.max([pl.col('x1'), pl.col('x1_')]).alias('x1_bbox'),
                                      pl.min([pl.col('x2'), pl.col('x2_')]).alias('x2_bbox'),
                                      pl.col('y1').alias("y1_bbox"),
                                      pl.col('y1_').alias('y2_bbox')]
                                     )
                .with_row_count(name="idx")
                )
@@ -62,37 +62,37 @@
                )
 
     return df_bbox
 
 
 def get_cells_dataframe(horizontal_lines: List[Line], vertical_lines: List[Line]) -> pl.LazyFrame:
     """
-    Create dataframe of all possible cells from horizontal and vertical lines
-    :param horizontal_lines: list of horizontal lines
-    :param vertical_lines: list of vertical lines
+    Create dataframe of all possible cells from horizontal and vertical rows
+    :param horizontal_lines: list of horizontal rows
+    :param vertical_lines: list of vertical rows
     :return: dataframe containing all cells
     """
-    # Check for empty lines
+    # Check for empty rows
     if len(horizontal_lines) * len(vertical_lines) == 0:
         return pl.DataFrame().lazy()
 
-    # Create dataframe from horizontal and vertical lines
+    # Create dataframe from horizontal and vertical rows
     df_h_lines = pl.LazyFrame(data=[l.dict for l in horizontal_lines])
     df_v_lines = pl.LazyFrame(data=[l.dict for l in vertical_lines])
 
-    # Identify potential cells bboxes from horizontal lines
+    # Identify potential cells bboxes from horizontal rows
     df_bbox = get_potential_cells_from_h_lines(df_h_lines=df_h_lines)
 
-    # Cross join with vertical lines
+    # Cross join with vertical rows
     df_bbox = df_bbox.with_columns(pl.max([(pl.col('x2_bbox') - pl.col('x1_bbox')) * 0.025,
                                            pl.lit(5.0)]).round(0).alias('h_margin')
                                    )
     df_bbox_v = df_bbox.join(df_v_lines, how='cross')
 
-    # Check horizontal correspondence between cell and vertical lines
+    # Check horizontal correspondence between cell and vertical rows
     horizontal_cond = ((pl.col("x1_bbox") - pl.col("h_margin") <= pl.col("x1"))
                        & (pl.col("x2_bbox") + pl.col("h_margin") >= pl.col("x1")))
     df_bbox_v = df_bbox_v.filter(horizontal_cond)
 
     # Check vertical overlapping
     df_bbox_v = (df_bbox_v.with_columns((pl.min([pl.col('y2'), pl.col('y2_bbox')])
                                          - pl.max([pl.col('y1'), pl.col('y1_bbox')])).alias('overlapping')
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,18 +40,18 @@
             thresh[y+margin:y+h-margin, x+margin:x+w-margin] = binary_thresh[y+margin:y+h-margin, x+margin:x+w-margin]
 
     return thresh
 
 
 def dilate_dotted_lines(thresh: np.ndarray, char_length: float) -> np.ndarray:
     """
-    Dilate specific rows/columns of the threshold image in order to detect dotted lines
+    Dilate specific rows/columns of the threshold image in order to detect dotted rows
     :param thresh: threshold image array
     :param char_length: average character length in image
-    :return: threshold image with dilated dotted lines
+    :return: threshold image with dilated dotted rows
     """
     ### Horizontal case
     # Create dilated image
     h_dilated = cv2.dilate(thresh, cv2.getStructuringElement(cv2.MORPH_RECT, (int(char_length // 2), 1)))
 
     # Get rows with at least 2 times the average number of white pixels
     white_rows = np.where(np.mean(thresh, axis=1) > 2 * np.mean(thresh))[0].tolist()
@@ -88,110 +88,110 @@
 
     # Update threshold image
     return np.maximum(thresh, v_dilated)
 
 
 def overlapping_filter(lines: List[Line], max_gap: int = 5) -> List[Line]:
     """
-    Process lines to merge close lines
-    :param lines: lines
-    :param max_gap: maximum gap used to merge lines
-    :return: list of filtered lines
+    Process rows to merge close rows
+    :param lines: rows
+    :param max_gap: maximum gap used to merge rows
+    :return: list of filtered rows
     """
     if len(lines) == 0:
         return []
 
-    # Identify if lines are horizontal
+    # Identify if rows are horizontal
     horizontal = all(map(lambda l: l.horizontal, lines))
 
-    # If not horizontal, transpose all lines
+    # If not horizontal, transpose all rows
     if not horizontal:
         lines = [line.transpose for line in lines]
 
-    # Sort lines by secondary dimension
+    # Sort rows by secondary dimension
     lines = sorted(lines, key=lambda l: (l.y1, l.x1))
 
-    # Create clusters of lines based on "similar" secondary dimension
+    # Create clusters of rows based on "similar" secondary dimension
     previous_sequence, current_sequence = iter(lines), iter(lines)
     line_clusters = [[next(current_sequence)]]
     for previous, line in zip(previous_sequence, current_sequence):
-        # If the vertical difference between consecutive lines is too large, create a new cluster
+        # If the vertical difference between consecutive rows is too large, create a new cluster
         if line.y1 - previous.y1 > 2:
             # Large gap, we create a new empty sublist
             line_clusters.append([])
 
         # Append to last cluster
         line_clusters[-1].append(line)
 
-    # Create final lines by "merging" lines within a cluster
+    # Create final rows by "merging" rows within a cluster
     final_lines = list()
     for cluster in line_clusters:
         # Sort the cluster
         cluster = sorted(cluster, key=lambda l: min(l.x1, l.x2))
 
-        # Loop over lines in the cluster to merge relevant lines together
+        # Loop over rows in the cluster to merge relevant rows together
         seq = iter(cluster)
         sub_clusters = [[next(seq)]]
         for line in seq:
-            # If lines are vertically close, merge line with curr_line
+            # If rows are vertically close, merge line with curr_line
             dim_2_sub_clust = max(map(lambda l: l.x2, sub_clusters[-1]))
             if line.x1 - dim_2_sub_clust <= max_gap:
                 sub_clusters[-1].append(line)
             # If the difference in vertical coordinates is too large, create a new sub cluster
             else:
                 sub_clusters.append([line])
 
-        # Create lines from sub clusters
+        # Create rows from sub clusters
         for sub_cl in sub_clusters:
             y_value = round(np.average([l.y1 for l in sub_cl],
                                        weights=list(map(lambda l: l.length, sub_cl))))
             thickness = min(max(1, max(map(lambda l: l.y2, sub_cl)) - min(map(lambda l: l.y1, sub_cl))), 5)
             line = Line(x1=min(map(lambda l: l.x1, sub_cl)),
                         x2=max(map(lambda l: l.x2, sub_cl)),
                         y1=y_value,
                         y2=y_value,
                         thickness=thickness)
 
             if line.length > 0:
                 final_lines.append(line)
 
-    # If not horizontal, transpose all lines
+    # If not horizontal, transpose all rows
     if not horizontal:
         final_lines = [line.transpose for line in final_lines]
 
     return final_lines
 
 
 def remove_word_lines(lines: List[Line], contours: List[Cell]) -> List[Line]:
     """
-    Remove lines that corresponds to contours in image
-    :param lines: list of lines
+    Remove rows that corresponds to contours in image
+    :param lines: list of rows
     :param contours: list of image contours as cell objects
-    :return: list of lines not intersecting with words
+    :return: list of rows not intersecting with words
     """
     # Get contours dataframe
     df_cnts = pl.LazyFrame(data=[{"x1": c.x1, "y1": c.y1, "x2": c.x2, "y2": c.y2} for c in contours])
 
-    # If there are no lines or no contours, do nothing
+    # If there are no rows or no contours, do nothing
     if len(lines) == 0 or df_cnts.collect(streaming=True).height == 0:
         return lines
 
-    # Create dataframe containing lines
+    # Create dataframe containing rows
     df_lines = (pl.LazyFrame(data=[line.dict for line in lines])
                 .with_columns([pl.max([pl.col('width'), pl.col('height')]).alias('length'),
                                (pl.col('x1') == pl.col('x2')).alias('vertical')]
                               )
                 .with_row_count(name="line_id")
                 .rename({"x1": "x1_line", "x2": "x2_line", "y1": "y1_line", "y2": "y2_line"})
                 )
 
     # Merge both dataframes
     df_words_lines = df_cnts.join(df_lines, how='cross')
 
-    # Compute intersection between contours bbox and lines
+    # Compute intersection between contours bbox and rows
     # - vertical case
     vert_int = (
         (((pl.col('x1') + pl.col('x2')) / 2 - pl.col('x1_line')).abs() / (pl.col('x2') - pl.col('x1')) < 0.45)
         * pl.max([(pl.min([pl.col('y2'), pl.col('y2_line')]) - pl.max([pl.col('y1'), pl.col('y1_line')])), pl.lit(0)])
     )
     # - horizontal case
     hor_int = (
@@ -203,70 +203,70 @@
                                                  )
 
     # Compute total intersection for each line
     df_inter = (df_words_lines.groupby(['line_id', 'length'])
                 .agg(pl.col('intersection').sum().alias('intersection'))
                 )
 
-    # Identify lines that intersect contours
+    # Identify rows that intersect contours
     intersecting_lines = (df_inter.filter(pl.col('intersection') / pl.col('length') > 0.5)
                           .collect(streaming=True)
                           .get_column('line_id')
                           .to_list()
                           )
 
     return [line for idx, line in enumerate(lines) if idx not in intersecting_lines]
 
 
 def detect_lines(image: np.ndarray, contours: Optional[List[Cell]], char_length: Optional[float], rho: float = 1,
                  theta: float = np.pi / 180, threshold: int = 50, minLinLength: int = 290, maxLineGap: int = 6,
                  kernel_size: int = 20) -> (List[Line], List[Line]):
     """
-    Detect horizontal and vertical lines on image
+    Detect horizontal and vertical rows on image
     :param image: image array
     :param contours: list of image contours as cell objects
     :param char_length: average character length
     :param rho: rho parameter for Hough line transform
     :param theta: theta parameter for Hough line transform
     :param threshold: threshold parameter for Hough line transform
     :param minLinLength: minLinLength parameter for Hough line transform
     :param maxLineGap: maxLineGap parameter for Hough line transform
-    :param kernel_size: kernel size to filter on horizontal / vertical lines
-    :return: horizontal and vertical lines
+    :param kernel_size: kernel size to filter on horizontal / vertical rows
+    :return: horizontal and vertical rows
     """
     # Create copy of image
     img = image.copy()
 
     # Apply thresholding
     thresh = threshold_dark_areas(img=img, char_length=char_length)
 
     if char_length is not None:
-        # Process threshold image in order to detect dotted lines
+        # Process threshold image in order to detect dotted rows
         thresh = dilate_dotted_lines(thresh=thresh, char_length=char_length)
 
-    # Identify both vertical and horizontal lines
+    # Identify both vertical and horizontal rows
     for kernel_tup, gap in [((kernel_size, 1), 2 * maxLineGap), ((1, kernel_size), maxLineGap)]:
         # Apply masking on image
         kernel = cv2.getStructuringElement(cv2.MORPH_RECT, kernel_tup)
         mask = cv2.morphologyEx(thresh, cv2.MORPH_OPEN, kernel, iterations=1)
 
-        # Compute Hough lines on image and get lines
+        # Compute Hough rows on image and get rows
         hough_lines = cv2.HoughLinesP(mask, rho, theta, threshold, None, minLinLength, maxLineGap)
 
-        # Handle case with no lines
+        # Handle case with no rows
         if hough_lines is None:
             yield []
             continue
 
         lines = [Line(*line[0].tolist()).reprocess() for line in hough_lines]
 
-        # Remove lines that are not horizontal or vertical
+        # Remove rows that are not horizontal or vertical
         lines = [line for line in lines if line.horizontal or line.vertical]
 
-        # Merge lines
+        # Merge rows
         merged_lines = overlapping_filter(lines=lines, max_gap=gap)
 
-        # If possible, remove lines that corresponds to words
+        # If possible, remove rows that corresponds to words
         if contours is not None:
             merged_lines = remove_word_lines(lines=merged_lines, contours=contours)
 
         yield merged_lines
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         list_splitted_rows += row.split_in_rows(vertical_delimiters=vertical_delimiters)
 
     return Table(rows=list_splitted_rows)
 
 
 def handle_implicit_rows(img: np.ndarray, tables: List[Table]) -> List[Table]:
     """
-    Detect and handle implicit lines in image tables
+    Detect and handle implicit rows in image tables
     :param img: image array
     :param tables: list of Table objects
     :return: list of Table objects updated taking into account implicit rows
     """
     # Detect implicit rows
     tables_implicit_rows = [handle_implicit_rows_table(img=img, table=table) for table in tables]
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-1.0.0/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-1.0.0/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 from typing import List
 
 import numpy as np
 
 from img2table.tables.objects.line import Line
 from img2table.tables.objects.table import Table
-from img2table.tables.processing.borderless_tables.column_delimiters import get_whitespace_column_delimiters
-from img2table.tables.processing.borderless_tables.lines import identify_line_groups
+from img2table.tables.processing.borderless_tables.column_delimiters import identify_column_groups
+from img2table.tables.processing.borderless_tables.rows import detect_delimiter_group_rows
 from img2table.tables.processing.borderless_tables.segment_image import segment_image
 from img2table.tables.processing.borderless_tables.table import identify_table
 from img2table.tables.processing.common import is_contained_cell
 
 
 def deduplicate_tables(identified_tables: List[Table], existing_tables: List[Table]) -> List[Table]:
     """
@@ -34,44 +34,39 @@
 
 
 def identify_borderless_tables(img: np.ndarray, lines: List[Line], char_length: float, median_line_sep: float,
                                existing_tables: List[Table]) -> List[Table]:
     """
     Identify borderless tables in image
     :param img: image array
-    :param lines: list of lines detected in image
+    :param lines: list of rows detected in image
     :param char_length: average character length
     :param median_line_sep: median line separation
     :param existing_tables: list of detected bordered tables
     :return: list of detected borderless tables
     """
     # Segment image
     img_segments = segment_image(img=img,
                                  lines=lines,
                                  char_length=char_length,
                                  median_line_sep=median_line_sep)
 
-    # In each segment, create groups of lines and identify tables
+    # In each segment, create groups of rows and identify tables
     tables = list()
     for seg in img_segments:
-        # Identify line groups in segment
-        seg_line_groups = identify_line_groups(segment=seg,
-                                               char_length=char_length,
-                                               median_line_sep=median_line_sep)
-
-        # For each line group, identify column delimiters and create tables
-        for line_gp in seg_line_groups.line_groups:
-            # Get column delimiters
-            col_delimiters = get_whitespace_column_delimiters(line_group=line_gp,
-                                                              segment_elements=seg_line_groups.elements)
-
-            # Create table
-            table = identify_table(line_group=line_gp,
-                                   column_delimiters=col_delimiters,
-                                   lines=lines,
-                                   elements=seg_line_groups.elements)
-
-            if table:
-                tables.append(table)
+        # Identify column groups in segment
+        column_groups = identify_column_groups(segment=seg,
+                                               char_length=char_length)
+
+        for column_group in column_groups:
+            # Identify potential table rows
+            table_rows = detect_delimiter_group_rows(delimiter_group=column_group)
+
+            if table_rows:
+                # Create table from column group and rows
+                borderless_table = identify_table(columns=column_group,
+                                                  table_rows=table_rows,
+                                                  lines=lines)
+                tables.append(borderless_table)
 
     return deduplicate_tables(identified_tables=tables,
                               existing_tables=existing_tables)
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-1.0.0/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,121 @@
 # coding: utf-8
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List
 
-import numpy as np
-
 from img2table.tables.objects.cell import Cell
 
 
 @dataclass
-class TableLine:
-    cells: List[Cell]
+class ImageSegment:
+    x1: int
+    y1: int
+    x2: int
+    y2: int
+    elements: List[Cell] = None
+
+    @property
+    def height(self) -> int:
+        return self.y2 - self.y1
+
+    def set_elements(self, elements: List[Cell]):
+        self.elements = elements
+
+    def __hash__(self):
+        return hash(repr(self))
+
+
+@dataclass
+class DelimiterGroup:
+    delimiters: List[Cell]
+    elements: List[Cell] = field(default_factory=lambda: [])
 
     @property
     def x1(self) -> int:
-        return min([c.x1 for c in self.cells])
+        return min([d.x1 for d in self.delimiters])
 
     @property
     def y1(self) -> int:
-        return min([c.y1 for c in self.cells])
+        return min([d.y1 for d in self.delimiters])
 
     @property
     def x2(self) -> int:
-        return max([c.x2 for c in self.cells])
+        return max([d.x2 for d in self.delimiters])
 
     @property
     def y2(self) -> int:
-        return max([c.y2 for c in self.cells])
+        return max([d.y2 for d in self.delimiters])
 
     @property
-    def v_center(self) -> float:
-        return (self.y1 + self.y2) / 2
+    def bbox(self) -> Cell:
+        return Cell(x1=self.x1, y1=self.y1, x2=self.x2, y2=self.y2)
 
     @property
     def height(self) -> int:
         return self.y2 - self.y1
 
     @property
-    def size(self) -> int:
-        return len(self.cells)
+    def width(self) -> int:
+        return self.x2 - self.x1
 
     @property
-    def cell(self) -> Cell:
-        return Cell(x1=self.x1, y1=self.y1, x2=self.x2, y2=self.y2)
-
-    def add(self, c: Cell):
-        self.cells.append(c)
-
-    def overlaps(self, other: "TableLine") -> bool:
-        # Compute y overlap
-        y_top = max(self.y1, other.y1)
-        y_bottom = min(self.y2, other.y2)
-
-        return (y_bottom - y_top) / min(self.height, other.height) >= 0.5
-
-    def merge(self, other: "TableLine") -> "TableLine":
-        return TableLine(cells=self.cells + other.cells)
-
-    def __eq__(self, other):
-        return self.cells == other.cells
+    def area(self) -> int:
+        return (self.x2 - self.x1) * (self.y2 - self.y1)
 
-    def __hash__(self):
-        return hash(f"{self.x1},{self.y1},{self.x2},{self.y2}")
+    def add(self, delimiter: Cell):
+        self.delimiters.append(delimiter)
 
 
 @dataclass
-class LineGroup:
-    lines: List[TableLine]
+class TableRow:
+    cells: List[Cell]
 
     @property
     def x1(self) -> int:
-        return min([c.x1 for c in self.lines])
+        return min([c.x1 for c in self.cells])
 
     @property
     def y1(self) -> int:
-        return min([c.y1 for c in self.lines])
+        return min([c.y1 for c in self.cells])
 
     @property
     def x2(self) -> int:
-        return max([c.x2 for c in self.lines])
+        return max([c.x2 for c in self.cells])
 
     @property
     def y2(self) -> int:
-        return max([c.y2 for c in self.lines])
+        return max([c.y2 for c in self.cells])
+
+    @property
+    def v_center(self) -> float:
+        return (self.y1 + self.y2) / 2
 
     @property
     def height(self) -> int:
         return self.y2 - self.y1
 
     @property
     def size(self) -> int:
-        return len(self.lines)
-
-    @property
-    def median_line_sep(self) -> float:
-        if len(self.lines) <= 1:
-            return 0
-
-        # Sort lines
-        sorted_lines = sorted(self.lines, key=lambda line: line.y1 + line.y2)
-
-        return np.median([nxt.v_center - prev.v_center for prev, nxt in zip(sorted_lines, sorted_lines[1:])])
+        return len(self.cells)
 
     @property
-    def median_line_gap(self) -> float:
-        if len(self.lines) <= 1:
-            return 0
-
-        # Sort lines
-        sorted_lines = sorted(self.lines, key=lambda line: line.y1 + line.y2)
-
-        return np.median([nxt.y1 - prev.y2 for prev, nxt in zip(sorted_lines, sorted_lines[1:])])
+    def cell(self) -> Cell:
+        return Cell(x1=self.x1, y1=self.y1, x2=self.x2, y2=self.y2)
 
-    def add(self, line: TableLine):
-        self.lines.append(line)
+    def add(self, c: Cell):
+        self.cells.append(c)
 
-    def __hash__(self):
-        return hash(repr(self))
+    def overlaps(self, other: "TableRow") -> bool:
+        # Compute y overlap
+        y_top = max(self.y1, other.y1)
+        y_bottom = min(self.y2, other.y2)
 
+        return (y_bottom - y_top) / min(self.height, other.height) >= 0.33
 
-@dataclass
-class ImageSegment:
-    x1: int
-    y1: int
-    x2: int
-    y2: int
-    elements: List[Cell] = None
-    line_groups: List[LineGroup] = None
+    def merge(self, other: "TableRow") -> "TableRow":
+        return TableRow(cells=self.cells + other.cells)
 
-    def set_elements(self, elements: List[Cell]):
-        self.elements = elements
+    def __eq__(self, other):
+        return self.cells == other.cells
 
     def __hash__(self):
-        return hash(repr(self))
+        return hash(f"{self.x1},{self.y1},{self.x2},{self.y2}")
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-1.0.0/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,30 +7,32 @@
 
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.borderless_tables.model import ImageSegment
 from img2table.tables.processing.common import is_contained_cell, merge_contours
 
 
-def create_image_segments(img: np.ndarray, median_line_sep: float) -> List[ImageSegment]:
+def create_image_segments(img: np.ndarray, median_line_sep: float, char_length: float) -> List[ImageSegment]:
     """
     Create segmentation of the image into specific parts
     :param img: image array
     :param median_line_sep: median line separation
+    :param char_length: average character length
     :return: list of image segments as Cell objects
     """
     # Reprocess images
     blur = cv2.GaussianBlur(img, (5, 5), 0)
     thresh = cv2.Canny(blur, 0, 0)
 
-    # Define kernel size by using median line separation
-    kernel_size = round(median_line_sep / 3)
+    # Define kernel by using median line separation and character length
+    kernel_size = (max(int(2 * char_length), round(median_line_sep / 3)),
+                   round(median_line_sep / 3))
 
     # Dilate to combine adjacent text contours
-    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (kernel_size, kernel_size))
+    kernel = cv2.getStructuringElement(cv2.MORPH_RECT, kernel_size)
     dilate = cv2.dilate(thresh, kernel, iterations=4)
 
     # Create new image by adding black borders
     margin = 10
     back_borders = np.zeros(tuple(map(operator.add, img.shape, (2 * margin, 2 * margin))), dtype=np.uint8)
     back_borders[margin:img.shape[0] + margin, margin:img.shape[1] + margin] = dilate
 
@@ -55,26 +57,26 @@
 
 
 def get_segment_elements(img: np.ndarray, lines: List[Line], img_segments: List[ImageSegment], char_length: float,
                          median_line_sep: float, blur_size: int = 3) -> List[ImageSegment]:
     """
     Identify image elements that correspond to each segment
     :param img: image array
-    :param lines: list of image lines
+    :param lines: list of image rows
     :param img_segments: list of ImageSegment objects
     :param char_length: average character length
     :param median_line_sep: median line separation
     :param blur_size: kernel size for blurring operation
     :return: list of ImageSegment objects with corresponding elements
     """
     # Reprocess image
     blur = cv2.GaussianBlur(img, (blur_size, blur_size), 0)
     thresh = cv2.Canny(blur, 85, 255)
 
-    # Mask lines
+    # Mask rows
     for l in lines:
         if l.horizontal:
             cv2.rectangle(thresh, (l.x1 - l.thickness, l.y1), (l.x2 + l.thickness, l.y2), (0, 0, 0), 3 * l.thickness)
         elif l.vertical:
             cv2.rectangle(thresh, (l.x1, l.y1 - l.thickness), (l.x2, l.y2 + l.thickness), (0, 0, 0), 2 * l.thickness)
 
     # Dilate to combine adjacent text contours
@@ -96,29 +98,30 @@
                               vertically=None)
 
     # Get elements corresponding to each image segment
     for seg in img_segments:
         segment_elements = [cnt for cnt in elements if is_contained_cell(inner_cell=cnt, outer_cell=seg)]
         seg.set_elements(elements=segment_elements)
 
-    return img_segments
+    return [seg for seg in img_segments if len(seg.elements) > 0]
 
 
 def segment_image(img: np.ndarray, lines: List[Line], char_length: float, median_line_sep: float) -> List[ImageSegment]:
     """
     Segment image and its elements
     :param img: image array
     :param lines: list of Line objects of the image
     :param char_length: average character length
     :param median_line_sep: median line separation
     :return: list of ImageSegment objects with corresponding elements
     """
     # Create image segments
     image_segments = create_image_segments(img=img,
-                                           median_line_sep=median_line_sep)
+                                           median_line_sep=median_line_sep,
+                                           char_length=char_length)
 
     # Detect elements corresponding to each segment
     image_segments = get_segment_elements(img=img,
                                           lines=lines,
                                           img_segments=image_segments,
                                           char_length=char_length,
                                           median_line_sep=median_line_sep,
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-1.0.0/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # coding: utf-8
-from typing import List, Optional
+from typing import List
 
-from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
 from img2table.tables.objects.table import Table
-from img2table.tables.processing.borderless_tables.model import LineGroup
+from img2table.tables.processing.borderless_tables.model import DelimiterGroup, TableRow
 from img2table.tables.processing.borderless_tables.table.headers import process_headers
-from img2table.tables.processing.borderless_tables.table.table_creation import create_table
+from img2table.tables.processing.borderless_tables.table.table_creation import get_table
 
 
-def identify_table(line_group: LineGroup, column_delimiters: List[Cell], lines: List[Line],
-                   elements: List[Cell]) -> Optional[Table]:
+def identify_table(columns: DelimiterGroup, table_rows: List[TableRow], lines: List[Line]) -> Table:
     """
-    Identify potential tables from line group and column delimiters
-    :param line_group: group of line as LineGroup object
-    :param column_delimiters: list of column delimiters
-    :param lines: list of lines in image
-    :param elements: list of elements from image
-    :return: Table object if relevant
+    Identify table from column delimiters and rows
+    :param columns: column delimiters group
+    :param table_rows: list of table rows corresponding to columns
+    :param lines: list of detected solid rows in image
+    :return: Table object
     """
-    # Create table from lines and columns delimiters
-    table = create_table(line_group=line_group,
-                         column_delimiters=column_delimiters)
-
-    if table is None:
-        return table
+    # Create table from rows and columns delimiters
+    table = get_table(columns=columns,
+                      table_rows=table_rows)
 
     # Identify headers
-    table_headers = process_headers(table=table, lines=lines, elements=elements)
+    table_headers = process_headers(table=table,
+                                    lines=lines,
+                                    elements=columns.elements)
 
     # Reset table content
     for id_row, row in enumerate(table_headers.items):
         for id_col, col in enumerate(row.items):
             table_headers.items[id_row].items[id_col].content = None
 
     return table_headers
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-1.0.0/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,132 +19,120 @@
         for id_col, cell in enumerate(row.items):
             table.items[id_row].items[id_col].content = max([is_contained_cell(inner_cell=el, outer_cell=cell)
                                                              for el in elements])
 
     return table
 
 
-def check_header_coherency(table: Table, elements: List[Cell]) -> Table:
-    """
-    Check header coherency in order to restrict table height
-    :param table: Table object
-    :param elements: list of elements
-    :return: Table with top rows coherent with an header
-    """
-    # Identify for each table cell if some elements are present
-    table = match_table_elements(table=table, elements=elements)
-
-    # Get first complete row
-    first_complete_row = table.items[0]
-    for row in table.items:
-        if min([c.content for c in row.items]):
-            first_complete_row = row
-            break
-
-    # Get all next rows in final rows
-    final_rows = [row for row in table.items if row.y1 >= first_complete_row.y1]
-
-    # Check if other rows are coherent
-    prev_rows = [row for row in table.items if row.y1 < first_complete_row.y1]
-    prev_rows = sorted(prev_rows, key=lambda r: r.y1, reverse=True)
-
-    if prev_rows:
-        complete_indices = set(range(table.nb_columns))
-        for row in prev_rows:
-            # Check if the row completeness is coherent with the previous ones
-            row_indices = set([idx for idx, cell in enumerate(row.items) if cell.content])
-            if len(row_indices.difference(complete_indices)) > 0:
-                break
-            final_rows.insert(0, row)
-            complete_indices = row_indices
-
-        # Create final table
-        return Table(rows=final_rows)
-
-    return table
-
-
 def identify_table_lines(table: Table, lines: List[Line]) -> List[int]:
     """
-    Identify horizontal lines that correspond to the table
+    Identify horizontal rows that correspond to the table
     :param table: Table object
-    :param lines: list of lines
-    :return: list of y values corresponding to lines
+    :param lines: list of rows
+    :return: list of y values corresponding to rows
     """
-    # Get horizontal lines
+    # Get horizontal rows
     h_lines = [line for line in lines if line.horizontal]
 
-    # Match lines with table rows
+    # Match rows with table rows
     y_lines = dict()
     y_values = sorted(list(set([row.y1 for row in table.items] + [row.y2 for row in table.items])))
     for line in h_lines:
-        matching_y = [y for y in y_values
-                      if abs(line.y1 - y) / (table.height / table.nb_rows) <= 0.25]
+        matching_y = sorted([y for y in y_values
+                             if abs(line.y1 - y) / (table.height / table.nb_rows) <= 0.25],
+                            key=lambda y: abs(line.y1 - y))
         if matching_y:
-            y_val = matching_y.pop()
+            y_val = matching_y.pop(0)
             y_lines[y_val] = y_lines.get(y_val, []) + [line]
 
     # Return y values where the line represent at least 75% of the table width
     final_lines = list()
     for k, v in y_lines.items():
-        # Compute total length of lines
+        # Compute total length of rows
         x_vals = sorted(list(set([max(min(table.x2, l.x1), table.x1) for l in v]
                                  + [max(min(table.x2, l.x2), table.x1) for l in v])))
         total_length = sum([x_right - x_left for x_left, x_right in zip(x_vals, x_vals[1:])
                             if any([l for l in v if min(l.x2, x_right) - max(l.x1, x_left) > 0])])
 
         if total_length / table.width >= 0.75:
             final_lines.append(k)
 
     return final_lines
 
 
+def check_header_coherency(header_rows: List[Row]) -> bool:
+    """
+    Check if detected header is coherent
+    :param header_rows: list of rows creating the header
+    :return: boolean indicating if the header is coherent
+    """
+    # Sort rows
+    header_rows = sorted(header_rows, key=lambda r: r.y1, reverse=True)
+
+    # Check if all columns of first header row are complete (except first one that can be missing)
+    if not min([c.content for c in header_rows[0].items[1:]]):
+        return False
+
+    # Check coherent completeness of following rows
+    complete_idx = set(list(range(header_rows[0].nb_columns)))
+    for row in header_rows:
+        complete_idx_row = {idx for idx, c in enumerate(row.items) if c.content}
+        if len(complete_idx_row.difference(complete_idx)) > 0:
+            return False
+        complete_idx = complete_idx_row
+
+    return True
+
+
 def headers_from_lines(table: Table, lines: List[Line]) -> Table:
     """
-    Detect potential headers from horizontal lines in image
+    Detect potential headers from horizontal rows in image
     :param table: Table object
-    :param lines: list of lines
-    :return: table with processed header from lines
+    :param lines: list of rows
+    :return: table with processed header from rows
     """
-    # Identify horizontal lines that correspond to the table
+    # Identify horizontal rows that correspond to the table
     y_values = identify_table_lines(table=table, lines=lines)
 
-    # Create dict of rows indicating if all cells are complete
+    # Create dict of rows indicating if all cells are complete (except the first one that can be missing in the header)
     dict_row_completeness = {(row.y1, row.y2): min([c.content for c in row.items]) for row in table.items}
 
-    # Get lines that are in the top part of the table
+    # Get rows that are in the top part of the table
     top_lines = [y for y in y_values if (y - table.y1) / table.height <= 0.25][:2]
     top_lines = sorted(list(set(top_lines if len(top_lines) == 2 else [table.y1] + top_lines)))
 
     if len(top_lines) == 2:
-        # Check if there are no complete lines above the expected header
+        # Check if there are no complete rows above the expected header
         if max([v for k, v in dict_row_completeness.items() if k[0] < top_lines[0]] + [False]):
             return table
 
-        # Check if the first line of the header is complete
-        first_row_complete = [v for k, v in dict_row_completeness.items() if k[0] < top_lines[1]][-1]
-        if first_row_complete:
-            # Create new header by replacing lines
+        # Check if the header is coherent
+        header_rows = [row for row in table.items
+                       if top_lines[0] <= (row.y1 + row.y2) / 2 <= top_lines[1]]
+        coherent_header = check_header_coherency(header_rows=header_rows)
+
+        if coherent_header:
+            # Create new header by replacing rows
             final_rows = [row for row in table.items if row.y1 >= top_lines[1]]
             new_row = Row(cells=[Cell(x1=c.x1, x2=c.x2, y1=top_lines[0], y2=top_lines[1])
                                  for c in table.items[0].items])
             final_rows.insert(0, new_row)
             return Table(rows=final_rows)
 
     return table
 
 
 def process_headers(table: Table, lines: List[Line], elements: List[Cell]) -> Table:
     """
-    Detect headers in table from lines and elements
+    Detect headers in table from rows and elements
     :param table: Table object
     :param lines: list of lines
     :param elements: list of elements
     :return: table with processed headers
     """
     # Check header coherency
-    table = check_header_coherency(table=table, elements=elements)
+    table = match_table_elements(table=table, elements=elements)
 
     # Get headers from line
     table_headers = headers_from_lines(table=table, lines=lines)
 
     return table_headers
```

### Comparing `img2table-0.1.4/src/img2table/tables/processing/common.py` & `img2table-1.0.0/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/processing/prepare_image.py` & `img2table-1.0.0/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table/tables/processing/text/titles.py` & `img2table-1.0.0/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/src/img2table.egg-info/PKG-INFO` & `img2table-1.0.0/src/img2table.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.1.4
+Version: 1.0.0
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image 
@@ -29,14 +29,15 @@
         
         ## Installation <a name="installation"></a>
         The library can be installed via pip:
         
         > <code>pip install img2table</code>: Standard installation, supporting Tesseract<br>
         > <code>pip install img2table[paddle]</code>: For usage with Paddle OCR (Python <= 3.10 only)<br>
         > <code>pip install img2table[paddle-gpu]</code>: For usage with Paddle OCR - GPU (Python <= 3.10 only)<br>
+        > <code>pip install img2table[easyocr]</code>: For usage with EasyOCR<br>
         > <code>pip install img2table[gcp]</code>: For usage with Google Vision OCR<br>
         > <code>pip install img2table[aws]</code>: For usage with AWS Textract OCR<br>
         > <code>pip install img2table[azure]</code>: For usage with Azure Cognitive Services OCR
         
         ## Features <a name="features"></a>
         
         * Table identification for images and PDF files, including bounding boxes at the table cell level
@@ -111,25 +112,28 @@
         #### PDF <a name="pdf-doc"></a>
         PDF files are instantiated as follows :
         ```python
         from img2table.document import PDF
         
         pdf = PDF(src, 
                   pages=[0, 2],
-                  detect_rotation=False)
+                  detect_rotation=False,
+                  pdf_text_extraction=True)
         ```
         
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>src : str, <code>pathlib.Path</code>, bytes or <code>io.BytesIO</code>, required</dt>
         >    <dd style="font-style: italic;">PDF source</dd>
         >    <dt>pages : list, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">List of PDF page indexes to be processed. If None, all pages are processed</dd>
         >    <dt>detect_rotation : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Detect and correct skew/rotation of extracted images from the PDF</dd>
+        >    <dt>pdf_text_extraction : bool, optional, default <code>True</code></dt>
+        >    <dd style="font-style: italic;">Extract text from the PDF file for native PDFs</dd>
         ></dl>
         
         PDF pages are converted to images with a 200 DPI for table identification.
         
         ---
         
         ### OCR <a name="ocr"></a>
@@ -189,14 +193,38 @@
         >    <dd style="font-style: italic;">Lang parameter used in Paddle for text extraction, check <a href="https://github.com/Mushroomcat9998/PaddleOCR/blob/main/doc/doc_en/multi_languages_en.md#5-support-languages-and-abbreviations">documentation for available languages</a></dd>
         ></dl>
         
         *Released in version 0.0.13*
         <br>
         </details>
         
+        
+        <details>
+        <summary>EasyOCR<a name="easyocr"></a></summary>
+        <br>
+        
+        <a href="https://github.com/JaidedAI/EasyOCR">EasyOCR</a> is an open-source OCR based on Deep Learning models.<br>
+        At first use, relevant languages models will be downloaded.
+        
+        ```python
+        from img2table.ocr import EasyOCR
+        
+        ocr = EasyOCR(lang=["en"])
+        ```
+        
+        > <h4>Parameters</h4>
+        ><dl>
+        >    <dt>lang : list, optional, default <code>["en"]</code></dt>
+        >    <dd style="font-style: italic;">Lang parameter used in EasyOCR for text extraction, check <a href="https://www.jaided.ai/easyocr">documentation for available languages</a></dd>
+        ></dl>
+        
+        *Released in version 0.1.2*
+        <br>
+        </details>
+        
         <details>
         <summary>Google Vision<a name="vision"></a></summary>
         <br>
         
         Authentication to GCP can be done by setting the standard `GOOGLE_APPLICATION_CREDENTIALS` environment variable.<br>
         If this variable is missing, an API key should be provided via the `api_key` parameter.
         
@@ -295,19 +323,21 @@
         > <h4>Parameters</h4>
         ><dl>
         >    <dt>ocr : OCRInstance, optional, default <code>None</code></dt>
         >    <dd style="font-style: italic;">OCR instance used to parse document text. If None, cells content will not be extracted</dd>
         >    <dt>implicit_rows : bool, optional, default <code>False</code></dt>
         >    <dd style="font-style: italic;">Boolean indicating if implicit rows should be identified - check related <a href="/examples/Implicit_rows.ipynb" target="_self">example</a></dd>
         >    <dt>borderless_tables : bool, optional, default <code>False</code></dt>
-        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted. It requires to provide an OCR to the method in order to be performed - <b>feature in alpha version</b></dd>
+        >    <dd style="font-style: italic;">Boolean indicating if <a href="/examples/borderless.ipynb" target="_self">borderless tables</a> are extracted.</dd>
         >    <dt>min_confidence : int, optional, default <code>50</code></dt>
         >    <dd style="font-style: italic;">Minimum confidence level from OCR in order to process text, from 0 (worst) to 99 (best)</dd>
         ></dl>
         
+        <b>NB</b>: Borderless table extraction can, by design, only extract tables with 3 or more columns.
+        
         *Borderless table extraction released in version 0.0.14*
         
         #### Method return
         
         The [`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is used to model extracted tables from documents.
         
         > <h4>Attributes</h4>
@@ -406,18 +436,14 @@
         can be found are not returned.
         </li>
         <li>
         The library is tailored for usage on documents with white/light background. 
         Effectiveness can not be guaranteed on other type of documents. 
         </li>
         <li>
-        Borderless tables extraction is still in alpha stage and might be inconsistent on complex cases.
-        Improvements to the algorithm will be released in future versions.
-        </li>
-        <li>
         Table detection using only OpenCV processing can have some limitations. If the library fails to detect tables, 
         you may check CNN based solutions like <a href="https://github.com/DevashishPrasad/CascadeTabNet">CascadeTabNet</a> or 
         the <a href="https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.6/ppstructure/docs/quickstart_en.md#224-table-recognition">PaddleOCR implementation</a>.
         </li>
         </ul>
         
         
@@ -428,7 +454,8 @@
 Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: gcp
 Provides-Extra: aws
 Provides-Extra: azure
 Provides-Extra: paddle
 Provides-Extra: paddle_gpu
+Provides-Extra: easyocr
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.1.4 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 1.0.0 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
@@ -13,14 +13,15 @@
 extract) * [Excel export](#xlsx) * [Examples](#examples) * [Caveats / FYI]
 (#fyi) ## Installation  The library can be installed via pip: > pip install
 img2table: Standard installation, supporting Tesseract
 > pip install img2table[paddle]: For usage with Paddle OCR (Python <= 3.10
 only)
 > pip install img2table[paddle-gpu]: For usage with Paddle OCR - GPU (Python <=
 3.10 only)
+> pip install img2table[easyocr]: For usage with EasyOCR
 > pip install img2table[gcp]: For usage with Google Vision OCR
 > pip install img2table[aws]: For usage with AWS Textract OCR
 > pip install img2table[azure]: For usage with Azure Cognitive Services OCR ##
 Features  * Table identification for images and PDF files, including bounding
 boxes at the table cell level * Handling of complex table structures such as
 merged cells * Handling of implicit rows - see [example](/examples/
 Implicit_rows.ipynb) * Table content extraction by providing support for OCR
@@ -52,15 +53,15 @@
 
 The implemented method to handle skewed/rotated images supports skew angles up
 to 45Â° and is based on the publication by Huang,_2020.
 Setting the detect_rotation parameter to True, image coordinates and bounding
 boxes returned by other methods might not correspond to the original image.
 #### PDF  PDF files are instantiated as follows : ```python from
 img2table.document import PDF pdf = PDF(src, pages=[0, 2],
-detect_rotation=False) ``` >
+detect_rotation=False, pdf_text_extraction=True) ``` >
 *** Parameters ***
 >
 >
 PDF pages are converted to images with a 200 DPI for table identification. --
 - ### OCR  `img2table` provides an interface for several OCR services and tools
 in order to parse table content.
 If possible (i.e for native PDF), PDF text will be extracted directly from the
@@ -78,14 +79,22 @@
 on Deep Learning models.
 At first use, relevant languages models will be downloaded. ```python from
 img2table.ocr import PaddleOCR ocr = PaddleOCR(lang="en") ``` >
 *** Parameters ***
 >
 >
 *Released in version 0.0.13*
+  EasyOCR
+EasyOCR is an open-source OCR based on Deep Learning models.
+At first use, relevant languages models will be downloaded. ```python from
+img2table.ocr import EasyOCR ocr = EasyOCR(lang=["en"]) ``` >
+*** Parameters ***
+>
+>
+*Released in version 0.1.2*
   Google Vision
 Authentication to GCP can be done by setting the standard
 `GOOGLE_APPLICATION_CREDENTIALS` environment variable.
 If this variable is missing, an API key should be provided via the `api_key`
 parameter. ```python from img2table.ocr import VisionOCR ocr = VisionOCR
 (api_key="api_key", timeout=15) ``` >
 *** Parameters ***
@@ -119,17 +128,18 @@
 Instantiation of OCR ocr = TesseractOCR(n_threads=1, lang="eng") #
 Instantiation of document, either an image or a PDF doc = Image(src) # Table
 extraction extracted_tables = doc.extract_tables(ocr=ocr, implicit_rows=False,
 borderless_tables=False, min_confidence=50) ``` >
 *** Parameters ***
 >
 >
-*Borderless table extraction released in version 0.0.14* #### Method return The
-[`ExtractedTable`](/src/img2table/tables/objects/extraction.py#L35) class is
-used to model extracted tables from documents. >
+NB: Borderless table extraction can, by design, only extract tables with 3 or
+more columns. *Borderless table extraction released in version 0.0.14* ####
+Method return The [`ExtractedTable`](/src/img2table/tables/objects/
+extraction.py#L35) class is used to model extracted tables from documents. >
 *** Attributes ***
 >
 >
 ** Images **
 `extract_tables` method from the `Image` class returns a list of
 `ExtractedTable` objects. ```Python output = [ExtractedTable(...),
 ExtractedTable(...), ...] ```
@@ -162,18 +172,15 @@
       extract_tables method
 ## Caveats / FYI
     * For table extraction, results are highly dependent on OCR quality. By
       design, tables where no OCR data can be found are not returned.
     * The library is tailored for usage on documents with white/light
       background. Effectiveness can not be guaranteed on other type of
       documents.
-    * Borderless tables extraction is still in alpha stage and might be
-      inconsistent on complex cases. Improvements to the algorithm will be
-      released in future versions.
     * Table detection using only OpenCV processing can have some limitations.
       If the library fails to detect tables, you may check CNN based solutions
       like CascadeTabNet or the PaddleOCR_implementation.
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.7, <3.12 Description-Content-Type: text/
 markdown Provides-Extra: gcp Provides-Extra: aws Provides-Extra: azure
-Provides-Extra: paddle Provides-Extra: paddle_gpu
+Provides-Extra: paddle Provides-Extra: paddle_gpu Provides-Extra: easyocr
```

### Comparing `img2table-0.1.4/src/img2table.egg-info/SOURCES.txt` & `img2table-1.0.0/src/img2table.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 setup.py
 .github/dependabot.yml
 .github/workflows/publish.yml
 .github/workflows/test_workflow.yml
 examples/Basic_usage.ipynb
 examples/Implicit_rows.ipynb
 examples/borderless.ipynb
-examples/data/borderless_aws.jpg
-examples/data/borderless_ocr.jpg
+examples/utils.py
+examples/data/borderless.jpg
 examples/data/implicit.png
 examples/data/tables.pdf
 examples/data/tables.png
 examples/data/tables.xlsx
+examples/data/borderless/1.png
+examples/data/borderless/2.png
+examples/data/borderless/3.png
+examples/data/borderless/4.png
 src/img2table/__init__.py
 src/img2table.egg-info/PKG-INFO
 src/img2table.egg-info/SOURCES.txt
 src/img2table.egg-info/dependency_links.txt
 src/img2table.egg-info/not-zip-safe
 src/img2table.egg-info/pbr.json
 src/img2table.egg-info/requires.txt
@@ -34,14 +38,15 @@
 src/img2table/document/base/__init__.py
 src/img2table/document/base/rotation.py
 src/img2table/ocr/__init__.py
 src/img2table/ocr/aws_textract.py
 src/img2table/ocr/azure.py
 src/img2table/ocr/base.py
 src/img2table/ocr/data.py
+src/img2table/ocr/easyocr.py
 src/img2table/ocr/google_vision.py
 src/img2table/ocr/paddle.py
 src/img2table/ocr/pdf.py
 src/img2table/ocr/tesseract.py
 src/img2table/tables/__init__.py
 src/img2table/tables/image.py
 src/img2table/tables/metrics.py
@@ -60,18 +65,22 @@
 src/img2table/tables/processing/bordered_tables/cells/deduplication.py
 src/img2table/tables/processing/bordered_tables/cells/identification.py
 src/img2table/tables/processing/bordered_tables/tables/__init__.py
 src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
 src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
 src/img2table/tables/processing/bordered_tables/tables/table_creation.py
 src/img2table/tables/processing/borderless_tables/__init__.py
-src/img2table/tables/processing/borderless_tables/column_delimiters.py
-src/img2table/tables/processing/borderless_tables/lines.py
 src/img2table/tables/processing/borderless_tables/model.py
 src/img2table/tables/processing/borderless_tables/segment_image.py
+src/img2table/tables/processing/borderless_tables/column_delimiters/__init__.py
+src/img2table/tables/processing/borderless_tables/column_delimiters/column_groups.py
+src/img2table/tables/processing/borderless_tables/column_delimiters/vertical_whitespaces.py
+src/img2table/tables/processing/borderless_tables/rows/__init__.py
+src/img2table/tables/processing/borderless_tables/rows/coherency.py
+src/img2table/tables/processing/borderless_tables/rows/delimiter_group_rows.py
 src/img2table/tables/processing/borderless_tables/table/__init__.py
 src/img2table/tables/processing/borderless_tables/table/headers.py
 src/img2table/tables/processing/borderless_tables/table/table_creation.py
 src/img2table/tables/processing/text/__init__.py
 src/img2table/tables/processing/text/titles.py
 tests/__init__.py
 tests/conftest.py
@@ -104,14 +113,19 @@
 tests/ocr/azure/test_data/ocr_df.csv
 tests/ocr/azure/test_data/test.png
 tests/ocr/data/__init__.py
 tests/ocr/data/test_ocr_data.py
 tests/ocr/data/test_data/expected_table.json
 tests/ocr/data/test_data/ocr_df.csv
 tests/ocr/data/test_data/table.json
+tests/ocr/easyocr/__init__.py
+tests/ocr/easyocr/test_easyocr.py
+tests/ocr/easyocr/test_data/ocr.json
+tests/ocr/easyocr/test_data/ocr_df.csv
+tests/ocr/easyocr/test_data/test.png
 tests/ocr/google_vision/__init__.py
 tests/ocr/google_vision/test_google_vision.py
 tests/ocr/google_vision/test_data/expected_content.json
 tests/ocr/google_vision/test_data/ocr_df.csv
 tests/ocr/google_vision/test_data/test.png
 tests/ocr/paddle/__init__.py
 tests/ocr/paddle/test_paddle.py
@@ -168,31 +182,40 @@
 tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
 tests/tables/processing/bordered_tables/tables/test_data/expected.json
 tests/tables/processing/bordered_tables/tables/test_data/implicit.png
 tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
 tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
 tests/tables/processing/bordered_tables/tables/test_data/word_image.png
 tests/tables/processing/borderless_tables/__init__.py
-tests/tables/processing/borderless_tables/borderless_table/__init__.py
-tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
-tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
+tests/tables/processing/borderless_tables/borderless_tables/__init__.py
+tests/tables/processing/borderless_tables/borderless_tables/test_borderless_tables.py
+tests/tables/processing/borderless_tables/borderless_tables/test_data/lines.json
+tests/tables/processing/borderless_tables/borderless_tables/test_data/test.png
 tests/tables/processing/borderless_tables/column_delimiters/__init__.py
 tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-tests/tables/processing/borderless_tables/lines/__init__.py
-tests/tables/processing/borderless_tables/lines/test_lines.py
-tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
+tests/tables/processing/borderless_tables/column_delimiters/test_column_groups.py
+tests/tables/processing/borderless_tables/column_delimiters/test_vertical_whitespaces.py
+tests/tables/processing/borderless_tables/column_delimiters/test_data/image_segment.json
+tests/tables/processing/borderless_tables/rows/__init__.py
+tests/tables/processing/borderless_tables/rows/test_coherency.py
+tests/tables/processing/borderless_tables/rows/test_delimiter_group_rows.py
+tests/tables/processing/borderless_tables/rows/test_rows.py
+tests/tables/processing/borderless_tables/rows/test_data/delimiter_group.json
+tests/tables/processing/borderless_tables/rows/test_data/rows.json
 tests/tables/processing/borderless_tables/segment_image/__init__.py
 tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
 tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
 tests/tables/processing/borderless_tables/segment_image/test_data/test.png
 tests/tables/processing/borderless_tables/table/__init__.py
 tests/tables/processing/borderless_tables/table/test_headers.py
 tests/tables/processing/borderless_tables/table/test_table.py
 tests/tables/processing/borderless_tables/table/test_table_creation.py
+tests/tables/processing/borderless_tables/table/test_data/delimiter_group.json
+tests/tables/processing/borderless_tables/table/test_data/lines.json
+tests/tables/processing/borderless_tables/table/test_data/rows.json
 tests/tables/processing/common/__init__.py
 tests/tables/processing/common/test_common.py
 tests/tables/processing/common/test_data/test.jpg
 tests/tables/processing/prepare_image/__init__.py
 tests/tables/processing/prepare_image/test_prepare_image.py
 tests/tables/processing/prepare_image/test_data/test.png
 tests/tables/processing/text/__init__.py
```

### Comparing `img2table-0.1.4/tests/_mock_data/azure.pkl` & `img2table-1.0.0/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/_mock_data/tesseract_hocr.html` & `img2table-1.0.0/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/_mock_data/textract.json` & `img2table-1.0.0/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/_mock_data/vision.json` & `img2table-1.0.0/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/_mock_data/vision.pkl` & `img2table-1.0.0/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/conftest.py` & `img2table-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/base/test_data/test.png` & `img2table-1.0.0/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/base/test_rotation.py` & `img2table-1.0.0/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/image/test_data/blank.png` & `img2table-1.0.0/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/image/test_data/dark.png` & `img2table-1.0.0/tests/document/image/test_data/dark.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/image/test_data/expected.xlsx` & `img2table-1.0.0/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/image/test_data/test.png` & `img2table-1.0.0/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/image/test_image.py` & `img2table-1.0.0/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/pdf/test_data/test.pdf` & `img2table-1.0.0/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/document/pdf/test_pdf.py` & `img2table-1.0.0/tests/document/pdf/test_pdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
     with pytest.raises(TypeError) as e_info:
         pdf = PDF(src="img", pages=12)
 
     with pytest.raises(TypeError) as e_info:
         pdf = PDF(src="img", pages=["12"])
 
+    with pytest.raises(TypeError) as e_info:
+        pdf = PDF(src="img", pages=[1], detect_rotation="a")
+
 
 def test_load_pdf():
     # Load from path
     pdf_from_path = PDF(src="test_data/test.pdf")
 
     # Load from bytes
     with open("test_data/test.pdf", "rb") as f:
```

### Comparing `img2table-0.1.4/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-1.0.0/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/aws_textract/test_data/content.json` & `img2table-1.0.0/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-1.0.0/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/aws_textract/test_data/test.png` & `img2table-1.0.0/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/azure/test_azure.py` & `img2table-1.0.0/tests/ocr/azure/test_azure.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-1.0.0/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/azure/test_data/test.png` & `img2table-1.0.0/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/data/test_data/expected_table.json` & `img2table-1.0.0/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/data/test_data/ocr_df.csv` & `img2table-1.0.0/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/data/test_ocr_data.py` & `img2table-1.0.0/tests/ocr/data/test_ocr_data.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-1.0.0/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-1.0.0/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/google_vision/test_data/test.png` & `img2table-1.0.0/tests/ocr/easyocr/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/google_vision/test_google_vision.py` & `img2table-1.0.0/tests/ocr/google_vision/test_google_vision.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/paddle/test_data/hocr.json` & `img2table-1.0.0/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-1.0.0/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/paddle/test_data/test.png` & `img2table-1.0.0/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/paddle/test_paddle.py` & `img2table-1.0.0/tests/ocr/paddle/test_paddle.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/pdf/test_data/content.json` & `img2table-1.0.0/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-1.0.0/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/pdf/test_data/test.pdf` & `img2table-1.0.0/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-1.0.0/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-1.0.0/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/tesseract/test_data/test.png` & `img2table-1.0.0/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/ocr/tesseract/test_tesseract.py` & `img2table-1.0.0/tests/ocr/tesseract/test_tesseract.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/image/test_data/blank.png` & `img2table-1.0.0/tests/tables/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/image/test_data/ocr.csv` & `img2table-1.0.0/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/image/test_data/test.png` & `img2table-1.0.0/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/image/test_image.py` & `img2table-1.0.0/tests/tables/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/image/test_metrics.py` & `img2table-1.0.0/tests/tables/image/test_metrics.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/objects/test_data/expected_tables.json` & `img2table-1.0.0/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/objects/test_data/ocr.csv` & `img2table-1.0.0/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/objects/test_data/tables.json` & `img2table-1.0.0/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/objects/test_extraction.py` & `img2table-1.0.0/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/objects/test_line.py` & `img2table-1.0.0/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/objects/test_row.py` & `img2table-1.0.0/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/objects/test_table.py` & `img2table-1.0.0/tests/tables/objects/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/contours.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_data/contours.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-1.0.0/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.bordered_tables.lines import overlapping_filter, detect_lines, remove_word_lines
 
 
 def test_overlapping_filter():
-    # Create lines
+    # Create rows
     lines = [Line(x1=10, x2=10, y1=10, y2=100),
              Line(x1=11, x2=11, y1=90, y2=120),
              Line(x1=12, x2=12, y1=210, y2=230),
              Line(x1=12, x2=12, y1=235, y2=255),
              Line(x1=20, x2=20, y1=10, y2=100)]
 
     result = overlapping_filter(lines=lines, max_gap=10)
```

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
 
     with open("test_data/implicit_table.json", 'r') as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
     result = handle_implicit_rows_table(img=img, table=table)
 
-    # Check that 2 more lines have been created
+    # Check that 2 more rows have been created
     assert result.nb_rows == table.nb_rows + 2
 
 
 def test_handle_implicit_rows():
     img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
 
     with open("test_data/implicit_table.json", 'r') as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
     result = handle_implicit_rows(img=img, tables=[table])
 
-    # Check that 2 more lines have been created
+    # Check that 2 more rows have been created
     assert result[0].nb_rows == table.nb_rows + 2
```

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-1.0.0/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py` & `img2table-1.0.0/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # coding: utf-8
-import json
 
-import cv2
+import json
 
+from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.line import Line
-from img2table.tables.processing.borderless_tables import identify_borderless_tables
+from img2table.tables.processing.borderless_tables import identify_table
+from img2table.tables.processing.borderless_tables.model import DelimiterGroup, TableRow
 
 
-def test_identify_borderless_tables():
-    img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
+def test_identify_table():
+    with open("test_data/delimiter_group.json", "r") as f:
+        data = json.load(f)
+    delimiter_group = DelimiterGroup(delimiters=[Cell(**c) for c in data.get('delimiters')],
+                                     elements=[Cell(**c) for c in data.get('elements')])
+
+    with open("test_data/rows.json", "r") as f:
+        table_rows = [TableRow(cells=[Cell(**c) for c in row]) for row in json.load(f)]
 
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
-    result = identify_borderless_tables(img=img,
-                                        char_length=8.44,
-                                        median_line_sep=51,
-                                        lines=lines,
-                                        existing_tables=[])
-
-    assert len(result) == 2
-    assert (result[0].nb_columns, result[0].nb_rows) == (3, 6)
-    assert (result[1].nb_columns, result[1].nb_rows) == (2, 2)
+    result = identify_table(columns=delimiter_group,
+                            table_rows=table_rows,
+                            lines=lines)
+
+    assert result.nb_rows == 16
+    assert result.nb_columns == 8
+    assert (result.x1, result.y1, result.x2, result.y2) == (93, 45, 1233, 1060)
```

### Comparing `img2table-0.1.4/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png` & `img2table-1.0.0/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-1.0.0/tests/tables/processing/common/test_common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,55 @@
 # coding: utf-8
-from img2table.tables.objects.cell import Cell
-from img2table.tables.processing.borderless_tables.column_delimiters import identify_trivial_delimiters, \
-    find_whitespaces, compute_vertical_delimiters, filter_coherent_dels, get_whitespace_column_delimiters
-from img2table.tables.processing.borderless_tables.model import LineGroup, TableLine
-
-
-def test_identify_trivial_delimiters():
-    line_group = LineGroup(lines=[TableLine(cells=[Cell(x1=0, x2=100, y1=0, y2=100)])])
-    elements = [Cell(x1=10, x2=20, y1=10, y2=20), Cell(x1=40, x2=50, y1=10, y2=20)]
-
-    result = identify_trivial_delimiters(line_group=line_group,
-                                         elements=elements)
-
-    expected = [Cell(x1=20, x2=40, y1=0, y2=100)]
+import cv2
 
-    assert result == expected
-
-
-def test_find_whitespaces():
-    line_group = LineGroup(lines=[TableLine(cells=[Cell(x1=0, x2=100, y1=0, y2=100)])])
-    elements = [Cell(x1=10, x2=20, y1=10, y2=20), Cell(x1=40, x2=50, y1=10, y2=20)]
-
-    result = find_whitespaces(line_group=line_group,
-                              elements=elements)
-
-    expected = [Cell(x1=0, y1=20, x2=100, y2=100),
-                Cell(x1=0, y1=0, x2=100, y2=10),
-                Cell(x1=50, y1=10, x2=100, y2=20),
-                Cell(x1=20, y1=10, x2=40, y2=20),
-                Cell(x1=0, y1=10, x2=10, y2=20)]
-
-    assert result == expected
-
-
-def test_compute_vertical_delimiters():
-    whitespaces = [Cell(x1=0, x2=20, y1=0, y2=20),
-                   Cell(x1=4, x2=13, y1=20, y2=40),
-                   Cell(x1=20, x2=24, y1=0, y2=38),
-                   Cell(x1=40, x2=60, y1=0, y2=31),
-                   Cell(x1=60, x2=64, y1=0, y2=31)]
-
-    result = compute_vertical_delimiters(whitespaces=whitespaces,
-                                         ref_height=40)
-
-    expected = [Cell(x1=4, y1=0, x2=13, y2=40),
-                Cell(x1=20, y1=0, x2=24, y2=38),
-                Cell(x1=40, y1=0, x2=64, y2=31)]
-
-    assert result == expected
+from img2table.tables.objects.cell import Cell
+from img2table.tables.processing.common import is_contained_cell, merge_contours, get_contours_cell
 
 
-def test_filter_coherent_dels():
-    v_delimiters = [Cell(x1=12, x2=23, y1=14, y2=57),
-                    Cell(x1=35, x2=48, y1=17, y2=66),
-                    Cell(x1=48, x2=61, y1=14, y2=46),
-                    Cell(x1=61, x2=66, y1=17, y2=66),
-                    Cell(x1=122, x2=143, y1=22, y2=66)]
-    elements = [Cell(x1=0, x2=10, y1=0, y2=20), Cell(x1=110, x2=1200, y1=0, y2=20)]
-
-    result = filter_coherent_dels(v_delimiters=v_delimiters,
-                                  elements=elements)
-
-    expected = [Cell(x1=12, y1=17, x2=23, y2=57),
-                Cell(x1=35, y1=17, x2=48, y2=57),
-                Cell(x1=61, y1=17, x2=66, y2=57)]
+def test_is_contained_cell():
+    cell_1 = Cell(x1=0, x2=20, y1=0, y2=20)
+    cell_2 = Cell(x1=0, x2=40, y1=0, y2=25)
+    cell_3 = Cell(x1=50, x2=70, y1=123, y2=256)
+
+    assert is_contained_cell(inner_cell=cell_1, outer_cell=cell_2)
+    assert not is_contained_cell(inner_cell=cell_2, outer_cell=cell_1)
+    assert not is_contained_cell(inner_cell=cell_1, outer_cell=cell_3)
+    assert not is_contained_cell(inner_cell=cell_2, outer_cell=cell_3)
+
+
+def test_merge_contours():
+    contours = [Cell(x1=0, x2=20, y1=0, y2=20),
+                Cell(x1=0, x2=20, y1=10, y2=20),
+                Cell(x1=60, x2=80, y1=0, y2=20),
+                Cell(x1=10, x2=20, y1=100, y2=200)]
+
+    # Do not merge by axis
+    expected = [Cell(x1=0, x2=20, y1=0, y2=20),
+                Cell(x1=60, x2=80, y1=0, y2=20),
+                Cell(x1=10, x2=20, y1=100, y2=200)]
+    assert set(merge_contours(contours=contours, vertically=None)) == set(expected)
+
+    # Merge vertically
+    expected_vertical = [Cell(x1=0, x2=80, y1=0, y2=20), Cell(x1=10, x2=20, y1=100, y2=200)]
+    assert merge_contours(contours=contours, vertically=True) == expected_vertical
+
+    # Merge horizontally
+    expected_horizontal = [Cell(x1=0, x2=20, y1=0, y2=200), Cell(x1=60, x2=80, y1=0, y2=20)]
+    assert merge_contours(contours=contours, vertically=False) == expected_horizontal
+
+
+def test_get_contours_cell():
+    img = cv2.imread("test_data/test.jpg", cv2.IMREAD_GRAYSCALE)
+    cell = Cell(x1=0, x2=img.shape[1], y1=0, y2=img.shape[0])
+
+    result = get_contours_cell(img=img,
+                               cell=cell,
+                               margin=5,
+                               blur_size=5,
+                               kernel_size=9,
+                               merge_vertically=True)
+
+    expected = [Cell(x1=51, y1=19, x2=518, y2=146),
+                Cell(x1=60, y1=156, x2=534, y2=691),
+                Cell(x1=52, y1=765, x2=543, y2=811)]
 
     assert result == expected
-
-
-def test_get_whitespace_column_delimiters():
-    line_group = LineGroup(lines=[TableLine(cells=[Cell(x1=0, x2=100, y1=0, y2=100)])])
-    elements = [Cell(x1=10, x2=20, y1=10, y2=20), Cell(x1=40, x2=50, y1=10, y2=20)]
-
-    result = get_whitespace_column_delimiters(line_group=line_group,
-                                              segment_elements=elements)
-
-    assert result == [Cell(x1=20, y1=0, x2=40, y2=100)]
```

### Comparing `img2table-0.1.4/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-1.0.0/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 from img2table.tables.processing.borderless_tables.segment_image import create_image_segments, get_segment_elements, \
     segment_image
 
 
 def test_create_image_segments():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
 
-    result = create_image_segments(img=img, median_line_sep=51)
+    result = create_image_segments(img=img,
+                                   median_line_sep=66,
+                                   char_length=7.24)
 
-    assert set(result) == {ImageSegment(x1=2, y1=0, x2=804, y2=361), ImageSegment(x1=928, y1=0, x2=1188, y2=157)}
+    assert result == [ImageSegment(x1=53, y1=0, x2=1277, y2=1173)]
 
 
 def test_get_segment_elements():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    img_segments = [ImageSegment(x1=2, y1=0, x2=804, y2=361),
-                    ImageSegment(x1=928, y1=0, x2=1188, y2=157)]
+    img_segments = [ImageSegment(x1=53, y1=0, x2=1277, y2=1173)]
 
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = get_segment_elements(img=img,
                                   lines=lines,
                                   img_segments=img_segments,
                                   blur_size=3,
-                                  char_length=8.44,
-                                  median_line_sep=51)
+                                  char_length=7.24,
+                                  median_line_sep=66)
 
-    assert len(result[0].elements) == 14
-    assert len(result[1].elements) == 4
+    assert len(result[0].elements) == 164
 
 
 def test_segment_image():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = segment_image(img=img,
-                           char_length=8.44,
-                           median_line_sep=51,
+                           char_length=7.24,
+                           median_line_sep=66,
                            lines=lines)
 
-    assert {len(result[0].elements), len(result[1].elements)} == {14, 4}
+    assert len(result[0].elements) == 164
```

### Comparing `img2table-0.1.4/tests/tables/processing/common/test_data/test.jpg` & `img2table-1.0.0/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-1.0.0/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/text/test_data/ocr.csv` & `img2table-1.0.0/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/text/test_data/table.json` & `img2table-1.0.0/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/text/test_data/test.jpg` & `img2table-1.0.0/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.1.4/tests/tables/processing/text/test_titles.py` & `img2table-1.0.0/tests/tables/processing/text/test_titles.py`

 * *Files identical despite different names*

