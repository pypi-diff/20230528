# Comparing `tmp/look_like_scanned-0.2.0.tar.gz` & `tmp/look_like_scanned-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "look_like_scanned-0.2.0.tar", max compression
+gzip compressed data, was "look_like_scanned-0.2.2.tar", max compression
```

## Comparing `look_like_scanned-0.2.0.tar` & `look_like_scanned-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1091 2023-05-20 08:40:06.705094 look_like_scanned-0.2.0/LICENSE
--rw-r--r--   0        0        0     1817 2023-05-28 04:01:51.286875 look_like_scanned-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10029 2023-05-27 16:07:22.306458 look_like_scanned-0.2.0/README.md
--rw-r--r--   0        0        0      176 2023-05-27 10:54:18.968022 look_like_scanned-0.2.0/scanner/__init__.py
--rw-r--r--   0        0        0    12521 2023-05-28 03:09:38.710171 look_like_scanned-0.2.0/scanner/scanner.py
--rw-r--r--   0        0        0    11401 1970-01-01 00:00:00.000000 look_like_scanned-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/LICENSE
+-rw-r--r--   0        0        0    10207 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/README.md
+-rw-r--r--   0        0        0     1758 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/scanner/__init__.py
+-rw-r--r--   0        0        0    12157 2023-05-28 09:42:46.701398 look_like_scanned-0.2.2/scanner/scanner.py
+-rw-r--r--   0        0        0    11684 1970-01-01 00:00:00.000000 look_like_scanned-0.2.2/PKG-INFO
```

### Comparing `look_like_scanned-0.2.0/pyproject.toml` & `look_like_scanned-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-[tool.poetry]
-name = "look-like-scanned"
-version = "0.2.0"
-description = "Python script to make documents look like they were scanned."
-authors = ["navchandar <12165092+navchandar@users.noreply.github.com>"]
-repository    = "https://github.com/navchandar/look-like-scanned"
-homepage = "https://github.com/navchandar/look-like-scanned"
-readme = "README.md"
-keywords = ["pdf", "scan", "scanner", "image-to-pdf", "pdf-to-scan"]
-packages = [
-    { include = "scanner" },
-]
-classifiers = [
-    "Development Status :: 4 - Beta",
-    'Intended Audience :: Developers',
-    'License :: OSI Approved :: MIT License',
-    'Operating System :: Microsoft :: Windows',
-    'Operating System :: Microsoft :: Windows :: Windows 10',
-    'Operating System :: POSIX :: Linux',
-    'Environment :: Console',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3.8',
-    'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
-    'Topic :: Software Development :: Libraries :: Python Modules',
-    'Topic :: Utilities',
-]
-
-
-[tool.poetry.dependencies]
-python = "^3.7"
-pillow = "^9.5.0"
-pypdfium2 = "^4.11.0"
-
-
-[tool.poetry.scripts]
-scanner = "scanner:main"
-
-
-[tool.poetry.urls]
-"Bug Tracker" = "https://github.com/navchandar/look-like-scanned/issues"
-"Funding" = "https://www.buymeacoffee.com/navchandar/"
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-pytest = "^7.3.1"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-minversion = "6.0"
-log_cli = 1
-log_cli_level = "INFO"
-log_cli_format = "%(asctime)s [%(levelname)s] %(module)s.%(funcName)s.%(lineno)d: %(message)s"
-log_cli_date_format = "%H:%M:%S"
+[tool.poetry]
+name = "look-like-scanned"
+version = "0.2.2"
+description = "Python script to make documents look like they were scanned."
+authors = ["navchandar <12165092+navchandar@users.noreply.github.com>"]
+repository    = "https://github.com/navchandar/look-like-scanned"
+homepage = "https://github.com/navchandar/look-like-scanned"
+readme = "README.md"
+keywords = ["pdf", "scan", "scanner", "image-to-pdf", "pdf-to-scan"]
+packages = [
+    { include = "scanner" },
+]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    'Intended Audience :: Developers',
+    'License :: OSI Approved :: MIT License',
+    'Operating System :: Microsoft :: Windows',
+    'Operating System :: Microsoft :: Windows :: Windows 10',
+    'Operating System :: POSIX :: Linux',
+    'Environment :: Console',
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Topic :: Software Development :: Libraries :: Python Modules',
+    'Topic :: Utilities',
+]
+
+
+[tool.poetry.dependencies]
+python = "^3.7"
+pillow = "^9.5.0"
+pypdfium2 = "^4.11.0"
+
+
+[tool.poetry.scripts]
+scanner = "scanner:main"
+
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/navchandar/look-like-scanned/issues"
+"Funding" = "https://www.buymeacoffee.com/navchandar/"
+
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+pytest = "^7.3.1"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+log_cli = 1
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)s] %(module)s.%(funcName)s.%(lineno)d: %(message)s"
+log_cli_date_format = "%H:%M:%S"
```

### Comparing `look_like_scanned-0.2.0/README.md` & `look_like_scanned-0.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,105 +1,116 @@
-# look-like-scanned
-
-[![Pylint](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml)  [![PyTest](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml)
-![license](https://img.shields.io/badge/license-MIT-blue.svg)
-[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/navchandar/look-like-scanned/issues)
-[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) 
-
- - Python script to make documents look like they were scanned. 
-
- - It converts every page of a given PDF file into an image-based page and applies random askew and brightness (very mild) effects to simulate the appearance of scanned documents.
- 
- - The resulting pages are then combined back into an Output PDF file.
-
- - There are options to combine / convert image files into PDF as well.
-
- - Output PDF files are saved in the same input folder with a suffix _"filename_output.pdf"_
-
-
-## Installation
-
-```shell
-git clone https://github.com/navchandar/look-like-scanned.git
-pip install poetry
-poetry install
-pip install .
-```
-
-
-## Usage
-
-This package uses [PIL](https://pypi.org/project/Pillow/) and [pypdfium2](https://pypi.org/project/pypdfium2/) to convert and manipulate image and pdf objects.
-
-This is extended to provide a command-line interface (CLI) for easy usage.
-
-
-```shell
-# Convert all pdf files in folder to scanned pdf
-scanner -i .\tests
-scanner -i .\tests -f "pdf"
-
-# Convert all pdf files in folder to scanned without askew
-scanner -i .\tests -a no
-
-# Convert specific pdf file in folder to scanned pdf
-scanner -i .\tests -f "test.pdf"
-
-# Convert all jpg, jpeg, png, webp files in folder to one pdf file
-scanner -i .\tests -f "image"
-
-# Convert all png files in folder to pdf with 100% quality to one pdf file
-scanner -i .\tests -f "png" -q 100
-
-# Convert specific jpg file in folder to pdf with 75% quality to one pdf file
-scanner -i .\tests -f "JPG_Test.jpg" -q 75
-
-# Convert all PDF files including sub folders
-scanner -i .\tests -f "pdf" -r yes
-
-# Convert all Images including sub folders into one PDF
-scanner -i .\tests -f "image" -r yes
-
-```
-
-## Arguments
-
-These are the command-line arguments accepted:
-
-- `-i, --input_folder` : Specifies the input folder to read files from and convert. The default value is the current directory. 
-    - Example: `-i /path/to/files` or `-i C:\files\documents`
-
-- `-f, --file_type_or_name` : Specifies the file types to process or the file name to convert. The default value is "pdf" to convert all pdf files in the given input folder.
-    - Example: `-f pdf` or `-f image.jpg` or `-f image`
-
-- `-q, --file_quality` : Specifies the quality of the converted output files. The value must be between 50 and 100. The default value is 95. 
-    - Example: `-q 90`
-
-- `-a, --askew` : Controls whether to make the output documents slightly askew or slightly tilted. Accepted values are "yes" or "no". The default value is "yes". 
-    - Example: `-a yes` or `--askew no`
-
-- `-r, --recurse` : Allows scripts to find all matching files including subdirectories. Accepted values are "yes" or "no". The default value is "yes". 
-    - Example: `-r yes` or `--recurse no`
-
-
-❗❗ **Note:** ❗❗
-
-- The supported file types are: ".jpg", ".png", ".jpeg", ".webp", ".pdf".
-
-- The output PDF file size will be bigger compared to the input because the files are stored in image format.
-
-- Bookmarks / Links / Metadata will be removed when saving the output file.
-
-- Password protected PDF files are not yet supported.
-
-
-## License
- 
- [MIT license](LICENSE)
-
-
-## Support This Project
-
-[![Paypal Badge](https://img.shields.io/badge/-Paypal-0070ba?style=flat-square&logo=data%3Aimage%2Fjpeg%3Bbase64%2C%2F9j%2F4AAQSkZJRgABAQAAAQABAAD%2F2wBDAAIBAQIBAQICAgICAgICAwUDAwMDAwYEBAMFBwYHBwcGBwcICQsJCAgKCAcHCg0KCgsMDAwMBwkODw0MDgsMDAz%2F2wBDAQICAgMDAwYDAwYMCAcIDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAz%2FwgARCAAwADADAREAAhEBAxEB%2F8QAHQAAAgIBBQAAAAAAAAAAAAAABwgGCQIAAwQFCv%2FEABwBAAEEAwEAAAAAAAAAAAAAAAYCAwcIAAEFBP%2FaAAwDAQACEAMQAAAAdZSiYpqCdXycvSppyvSMUbKuLEBqPeeyxsX4su2oRUX2QQweZr0j8qBdJUyhfS8vqPk%2FEV3tVbWaafq4naOlKlyuxybCnaAD9sq5XBxxSVysGLjOdMLWa4WvNYLKIfSoU5sq7yAEYZOOCWb7LwozP%2F%2FEAD0QAAAFAwMBBAQJDQAAAAAAAAECAwQFBgcIABESCSExUbUKd5bTExQXIiM4cYGyMjM3QUJHV2GCg5Oh0f%2FaAAgBAQABPwDA%2FBOyVX4SWdlpaztqZKVlKHhHTx68pJg4cO11GCBzqqHMkJjnMYRMYwiOpvA%2FHWnYpZ49srZts2aJmUWWNRkcBCFKG5hH6HuAA30NqsOAP2W%2FsH7IR%2FuNQdjsQaheC1aW3sO4WN3FJSEf7jTXp94%2BuEiGJZGzqhD9oGCjY7tAf7Os7MFLJ0dhFeSWibNWqi5SLoabeNHbOk2CLhmsmwXOmomoVIDEOUxQMBiiA66eX1ArGer%2BA8tQ11vLjrUB0%2Fat%2BKujs3z8SNkxIqKahimHifYQ7e42lq4lEC8jzEmUviLs%2FwD3Ta6Mk0U5pT0omYP2ivVCj%2BLXo4eXVUVjcyq6Cm6gfTER8QTeMwevTKmanKYxRKnyEfyuW466gwGHAC%2BX0n7v5%2Fy1xrp5ciYBWOKHYBbfQHlzfXpM9x14K0Nu4NAwcJp0%2BFwX%2BSZUBLqpltkiE8e3RC8zCBS8x8ADfXSKoCoLP3IYVYJVmK8m7aJtC8vzqQn3NyAB%2FwBDrqF%2FUAvoXwt9PeWrjrp8Bw6fdkDeNvYDy5vr0mWuzvr80NT3MTN2EWq7%2FqUMBR%2FBrFzGSlbuW6WlqgZKulwcCinxUMQOIfZq32CNKtDg8h6QcvBKOxVNlVQ3%2B4dtYOYMzU5WEZUEwzJHQ0SsksVuqUyainEdwKBdg27tdQr5mAV9fV9P%2BWuddPMAPgFY3l%2FD%2BB8uQ11P%2Bjlc7N%2FIY9VRFQQDWNSQM3bJuhUE5CchEAHYNU3jdIYsMho2SdM3r9qqZRRRrv8ABmEw7bBv9msE6EYw2MdLqHj2qbtymdZUTIFBQxvhTB2jtv3AGg7zcdvm9gB%2BouuoaQwYB3z9X0%2F5c41g5nRY%2BlMG7NRMteW1cXLRVEQjV4ydVbHoOGixGCJTpqEOqBiHIYBKJTAGidQ%2BwJQMX5cbPe2kb77U3d%2FDmpZo0k%2BuDYV2%2BOO5llawj%2BRjfcvqDz0x0gYdFmxvVZtq1alEqSZKyjgAgf5tE6h1gOH6c7P%2B2cb77Wc2dllKtwfvHExd5LVyspK0PNs2bJnVrBZw7WUYLkTTTTKqJjnMbYoFKA6%2F%2F8QAJREAAQMDAgYDAAAAAAAAAAAAAQACAwQFEQYhBxASEyIxQVFS%2F9oACAECAQE%2FAPTyVEySeQRsCFhuDvcZTrFVN9xqSLtPDZRhNGHloRHytDUzJ7k1jgjBGwbgLs0rh5ALiJZqQQNqIAnHJ8VnA6VwspuueSX84VwLx8ppL1WWyOS2TOn9Y2VQOlxaz7K9vXC2EMppXfrCgoWTjL06O307vMgFa21tSw0rqGl3JUjhISftAjGXLSesKOgpe28bqxXZtZRiePYFa9uM0t3lLX%2BITnuduTyzhqcD1BoCptWXWKM08cmGKoqHzydx5yTz%2F8QAJREAAQMCBgIDAQAAAAAAAAAAAQACAwQRBQYSISJRBzEQFUET%2F9oACAEDAQE%2FAG%2BrIyCPmUa%2BDtMxCDtMlAFmFWYNym%2Fqx%2BoMVEXD2mTTu9FXqO1lzEJGnROVZhGoot2t0s4TD%2BTG9qhYAdSufZNlmjNx%2B3pqWgfyaTdUz7Qt%2FTYIbut2s3uvI1vSztnWuwiqFPRuspM2ZoxFuhriWnoLxp41r6itbiNe06RvuomiOPirtJ4hYzgdTUPL2ryPSzfdSQyb2svFGERQZchbJGNe97hMY1gs0W%2BOWi9lyMe6rcg4LUzCpliu8%2ByqSmjp4RFELAfP%2F9k%3D&logoColor=white&link=https://paypal.me/navchandar//)](https://paypal.me/navchandar/) 
-[![Ko-Fi Badge](https://img.shields.io/badge/-Buy%20a%20KoFi-ff5f5f?style=flat-square&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAOiSURBVFhH7ZbLTxRBEMb963gkJIRleS4JyyJnDnqFKA%2BREOXAgcAJhAMEL77xoBdEjSQY8II3wchrgQUUdmZnusqvpofZzfDoBdF4mM2XSae3u%2BrXVdU1c4NLSv4rRUAmRUAmRUAmRUAmRUAmRUAmRUAmRUAmGYBo9jVlLfp1REfHfyjOZGjxM93v59JSMa6fp2QC2ssQMTkuuerqyjmQchTr38ICJZrE%2FllMBiB3M02KtEVflp0f2LmLJrUcV2PIwRBsy5bx2ndqTIR8aRmA1JYPpGDXdhxFsJdTFAzYsl1XhSftHNZrGkFc%2BUrLX2g7LSiYPM7K4NMCl5eH3EEmoO0dDQQf8Ef7BzwzQ733qKuLp6Zodw8EqDB%2B8pR6eqi7myYmaGs7h2joOGHLwSE3NIi1eJwnJ1l5GbRzwtTdU%2BhLqzggnNh16fAnd3aqqipqaBBVx%2BjWbZqb47t3KBaj%2BnqZxKC9nTY2XThGbLAXuxL57NDMY0FBkIjow8dgPlBxQFnLgplXs1RdrVpvcipFLS2EZ1OTcCQSMsYM1NaGNfxoAuuxC1R5ICQIVdzcLJcOBQCg9Y1CX1rFAVkWskAjI1RXCxpOJhUE00kPApJx0hcQe3sdrEeEcMUCIH2nYjG1uS0Fjr929wJHgS4RIRobo5oaam3V7uWsAYeewSCVUnV1PDCA0g6n7NojxEtLUiU6JJojJDhD%2FAD95u0ZKfN0TTWEK2PnbAxGR1G2ChVTGJ6ABsHDVerry7cibCm4ZTRxXbfMu%2FbSWrIWP3ioauJ%2BkAImTVNbSx0dlMlIg9BMf6sPedbBhB7IjkNDQ1wTVwFTczODBplCHzo89LrlCY33hHshgJ3jrBwJ49U1bmwM%2BdIyAZ10atiVCHlxkh4zOqpA4DEhg6gb7u%2Fn4ywuF3q3rNTSWLAAkQZjXlzkpqu%2By%2FJAiJD%2FApHTSz2Nj0v9trSAjAcHJX5K5Wm8Lf5gd492dunHOs2%2Fp55en%2BMsGqjYGgp85Jlw1ulpac3DwxI2ZPOEBuh6sezN7EvrQresrMxbPocGMgDRt1W5n8GtKYgTnlK8y8soW0mirvrC2GAXFmxucUWFbxAcZWWB8TNlAGLkBT%2FLCoBCQpyEww7Pi3T9PnsudkwcgUxAFRX0bl7sotPDsf7gKhQcn573ZuQkKytS77Bzfo5CMgFBCPj0NKfTwcdoUcKn5ouXPs1lVATQv1UEZFIEZFIEZFIEZFIEdLFKSn4Dz0s70NgRCBAAAAAASUVORK5CYII%3D&logoColor=1fb3ef&link=https://ko-fi.com/navchandar//)](https://ko-fi.com/navchandar/) 
-[![BuymeCoffee Badge](https://img.shields.io/badge/-Buy%20a%20Coffee-ff813f?style=flat-square&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAP5SURBVFhH7ZdrTFNnGMfftvSUXmTcBtNCWy6mXBRoAZWL1GAgIRnSiGOZkmF0W3YpJEYXtIm3qPEWP%2BgHRRogQLgmEmPiEpOZGBSX%2BAUZLES3%2Bc0PRiMJX5a5ubPnlCMxT9tznrcDYxae%2FD6c0vP%2Bn185p%2B95ysTjnveKFSE1VoTU%2BF8Ina3NIjL4ST5aqwq30K3PCxzpViLVztVouSrcQk1FaSK59Hr93b0ulKAMn9Bs6wboIXcjVGlJcYt7DQpRhiRUk5UAVGfEGwTw4a7sZPNCQkNOMkoOhSQUo9OWlZXV%2FIdqbm622WwNeakoORSqUFdXl3wZoq3GxsalFBIEvdEYC5gAkxEwA2bTIpa3juGthXOAhVWAwSAsmdD%2B8rRUi%2FChWV%2FsENz5zJXHioBcVpjLCnJYgZOtfwO8LARypXfhHDjZ7WDF6UyjYVszEyAHJYdCEgJ2FaRAonh6o%2Fg74yPAnhxhULd3F6LMsFCFTlQ7rHEG6fhRSEsFppl4kf3wtST09EDZ24GRoApNf1cCoT996RJvWXBXBX6UhL4qZ5vSLSgwElShv45WgVCP1yneiMddFbgmCXmyNLtdH6HASFCFAGeyqb0yXey14a4KjEhCKas0Z2oyUVokOIRgn5W2Wq77OsCen5JuoOufUR%2F7JKHLH6%2B1J1kSLUZTrAEO7FaBSrKwOkGAsiaY7fGxKDYsJKHxPUXwKdva2k5EWy6Xy5OdgmLDQhKaO1QBQqOjo%2FJTgL%2Fchet9G60oNizUe2ibM8nr9crxnDUzMwOfZ%2BIL0mBEFfJX2bIz7HIHzhoaGgKheX8lygwLVWhoR64UOj8vN%2BEpv9%2BfnRqPAiNBFZoJ7tQTExNyE56qr6%2F35i%2FDxijE6Do6OuQmPJVhSzvssaO0SHAIua0f%2BHw%2BuQm55ubmpG9oUx5KiwSHUEtRqmdzpdyHXOPj4yA021qK0iLBIQS%2FyCC6s7MTNqTh4eGBgYG%2Bvr6enh6YbuGPcDUDgUB3d3dvb29%2Ff%2F%2Fg4ODIyMjY2FhdXd0GexKKUoBDCAYaEEKl1Wr0MRqDQWuM1QmCVqfTwHCIao%2BbekcDHELAy4MV%2FdtzwOzPB9q%2FH7N%2Ffgt5mgZ5%2FSt7dZ%2F9cYElGnWwy79oL0c5CvAJAb%2F4SqU9V3VMC45m5bZVaLkq3EKvj1V1NRDGtOBoxnWxFuAWAr6vIIxpwdHsXC11LlskGqF6Z5L6mBZgz06yGzvXobWqRCMEX5xXR6rESS2WWGRS%2Bvdc%2FTSqcPSaAgj9%2FG2JeE%2FAHovckYT2bXmHQudrM6eumKZusvBcYlPtrDLzXQmlxRmk%2FY5QaCGFaNY8%2FKaYCFpIIRqhZWVFSI0VIWWOe%2F4FR6A6eCoawHAAAAAASUVORK5CYII%3D&logoColor=white&link=https://www.buymeacoffee.com/navchandar//)](https://www.buymeacoffee.com/navchandar/) 
-
+# look-like-scanned
+
+[![Pylint](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/pylint.yml)  [![PyTest](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml/badge.svg)](https://github.com/navchandar/look-like-scanned/actions/workflows/tests.yml)
+![license](https://img.shields.io/badge/license-MIT-blue.svg)
+[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/navchandar/look-like-scanned/issues)
+[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) 
+
+ - Python script to make documents look like they were scanned. 
+
+ - It converts every page of a given PDF file into an image-based page and applies random askew and brightness (very mild) effects to simulate the appearance of scanned documents.
+ 
+ - The resulting pages are then combined back into an Output PDF file.
+
+ - There are options to combine / convert image files into PDF as well.
+
+ - Output PDF files are saved in the same input folder with a suffix _"filename_output.pdf"_
+
+
+## Installation
+
+Install from the [Python Package Index (PyPI)](https://pypi.org/project/look-like-scanned/)
+```shell
+pip install look-like-scanned
+```
+
+Or to install latest version from GitHub
+```shell
+git clone https://github.com/navchandar/look-like-scanned.git
+pip install poetry
+poetry install
+pip install .
+```
+
+### Verify Installation:
+```shell
+# Print help message and usage options available
+scanner -h
+```
+
+
+## Usage
+
+This package uses [PIL](https://pypi.org/project/Pillow/) and [pypdfium2](https://pypi.org/project/pypdfium2/) to convert and manipulate image and pdf objects.
+
+This is extended to provide a command-line interface (CLI) for easy usage.
+
+
+```shell
+# Convert all pdf files in folder to scanned pdf
+scanner -i .\tests
+scanner -i .\tests -f "pdf"
+
+# Convert all pdf files in folder to scanned without askew
+scanner -i .\tests -a no
+
+# Convert specific pdf file in folder to scanned pdf
+scanner -i .\tests -f "test.pdf"
+
+# Convert all jpg, jpeg, png, webp files in folder to one pdf file
+scanner -i .\tests -f "image"
+
+# Convert all png files in folder to pdf with 100% quality to one pdf file
+scanner -i .\tests -f "png" -q 100
+
+# Convert specific jpg file in folder to pdf with 75% quality to one pdf file
+scanner -i .\tests -f "JPG_Test.jpg" -q 75
+
+# Convert all PDF files including sub folders
+scanner -i .\tests -f "pdf" -r yes
+
+# Convert all Images including sub folders into one PDF
+scanner -i .\tests -f "image" -r yes
+
+```
+
+## Arguments
+
+These are the command-line arguments accepted:
+
+- `-i, --input_folder` : Specifies the input folder to read files from and convert. The default value is the current directory. 
+    - Example: `-i /path/to/files` or `-i C:\files\documents`
+
+- `-f, --file_type_or_name` : Specifies the file types to process or the file name to convert. The default value is "pdf" to convert all pdf files in the given input folder.
+    - Example: `-f pdf` or `-f image.jpg` or `-f image`
+
+- `-q, --file_quality` : Specifies the quality of the converted output files. The value must be between 50 and 100. The default value is 95. 
+    - Example: `-q 90`
+
+- `-a, --askew` : Controls whether to make the output documents slightly askew or slightly tilted. Accepted values are "yes" or "no". The default value is "yes". 
+    - Example: `-a yes` or `--askew no`
+
+- `-r, --recurse` : Allows scripts to find all matching files including subdirectories. Accepted values are "yes" or "no". The default value is "yes". 
+    - Example: `-r yes` or `--recurse no`
+
+
+❗❗ **Note:** ❗❗
+
+- The supported file types are: ".jpg", ".png", ".jpeg", ".webp", ".pdf".
+
+- The output PDF file size **will be bigger** than the input file because the pages are stored in image format.
+
+- Bookmarks / Links / Metadata will be removed when saving the output file.
+
+- Password protected PDF files are not yet supported.
+
+
+## License
+ 
+ [MIT license](LICENSE)
+
+
+## Support This Project
+
+[![Paypal Badge](https://img.shields.io/badge/-Paypal-0070ba?style=for-the-badge&logo=data%3Aimage%2Fjpeg%3Bbase64%2C%2F9j%2F4AAQSkZJRgABAQAAAQABAAD%2F2wBDAAIBAQIBAQICAgICAgICAwUDAwMDAwYEBAMFBwYHBwcGBwcICQsJCAgKCAcHCg0KCgsMDAwMBwkODw0MDgsMDAz%2F2wBDAQICAgMDAwYDAwYMCAcIDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAz%2FwgARCAAwADADAREAAhEBAxEB%2F8QAHQAAAgIBBQAAAAAAAAAAAAAABwgGCQIAAwQFCv%2FEABwBAAEEAwEAAAAAAAAAAAAAAAYCAwcIAAEFBP%2FaAAwDAQACEAMQAAAAdZSiYpqCdXycvSppyvSMUbKuLEBqPeeyxsX4su2oRUX2QQweZr0j8qBdJUyhfS8vqPk%2FEV3tVbWaafq4naOlKlyuxybCnaAD9sq5XBxxSVysGLjOdMLWa4WvNYLKIfSoU5sq7yAEYZOOCWb7LwozP%2F%2FEAD0QAAAFAwMBBAQJDQAAAAAAAAECAwQFBgcIABESCSExUbUKd5bTExQXIiM4cYGyMjM3QUJHV2GCg5Oh0f%2FaAAgBAQABPwDA%2FBOyVX4SWdlpaztqZKVlKHhHTx68pJg4cO11GCBzqqHMkJjnMYRMYwiOpvA%2FHWnYpZ49srZts2aJmUWWNRkcBCFKG5hH6HuAA30NqsOAP2W%2FsH7IR%2FuNQdjsQaheC1aW3sO4WN3FJSEf7jTXp94%2BuEiGJZGzqhD9oGCjY7tAf7Os7MFLJ0dhFeSWibNWqi5SLoabeNHbOk2CLhmsmwXOmomoVIDEOUxQMBiiA66eX1ArGer%2BA8tQ11vLjrUB0%2Fat%2BKujs3z8SNkxIqKahimHifYQ7e42lq4lEC8jzEmUviLs%2FwD3Ta6Mk0U5pT0omYP2ivVCj%2BLXo4eXVUVjcyq6Cm6gfTER8QTeMwevTKmanKYxRKnyEfyuW466gwGHAC%2BX0n7v5%2Fy1xrp5ciYBWOKHYBbfQHlzfXpM9x14K0Nu4NAwcJp0%2BFwX%2BSZUBLqpltkiE8e3RC8zCBS8x8ADfXSKoCoLP3IYVYJVmK8m7aJtC8vzqQn3NyAB%2FwBDrqF%2FUAvoXwt9PeWrjrp8Bw6fdkDeNvYDy5vr0mWuzvr80NT3MTN2EWq7%2FqUMBR%2FBrFzGSlbuW6WlqgZKulwcCinxUMQOIfZq32CNKtDg8h6QcvBKOxVNlVQ3%2B4dtYOYMzU5WEZUEwzJHQ0SsksVuqUyainEdwKBdg27tdQr5mAV9fV9P%2BWuddPMAPgFY3l%2FD%2BB8uQ11P%2Bjlc7N%2FIY9VRFQQDWNSQM3bJuhUE5CchEAHYNU3jdIYsMho2SdM3r9qqZRRRrv8ABmEw7bBv9msE6EYw2MdLqHj2qbtymdZUTIFBQxvhTB2jtv3AGg7zcdvm9gB%2BouuoaQwYB3z9X0%2F5c41g5nRY%2BlMG7NRMteW1cXLRVEQjV4ydVbHoOGixGCJTpqEOqBiHIYBKJTAGidQ%2BwJQMX5cbPe2kb77U3d%2FDmpZo0k%2BuDYV2%2BOO5llawj%2BRjfcvqDz0x0gYdFmxvVZtq1alEqSZKyjgAgf5tE6h1gOH6c7P%2B2cb77Wc2dllKtwfvHExd5LVyspK0PNs2bJnVrBZw7WUYLkTTTTKqJjnMbYoFKA6%2F%2F8QAJREAAQMDAgYDAAAAAAAAAAAAAQACAwQFEQYhBxASEyIxQVFS%2F9oACAECAQE%2FAPTyVEySeQRsCFhuDvcZTrFVN9xqSLtPDZRhNGHloRHytDUzJ7k1jgjBGwbgLs0rh5ALiJZqQQNqIAnHJ8VnA6VwspuueSX84VwLx8ppL1WWyOS2TOn9Y2VQOlxaz7K9vXC2EMppXfrCgoWTjL06O307vMgFa21tSw0rqGl3JUjhISftAjGXLSesKOgpe28bqxXZtZRiePYFa9uM0t3lLX%2BITnuduTyzhqcD1BoCptWXWKM08cmGKoqHzydx5yTz%2F8QAJREAAQMCBgIDAQAAAAAAAAAAAQACAwQRBQYSISJRBzEQFUET%2F9oACAEDAQE%2FAG%2BrIyCPmUa%2BDtMxCDtMlAFmFWYNym%2Fqx%2BoMVEXD2mTTu9FXqO1lzEJGnROVZhGoot2t0s4TD%2BTG9qhYAdSufZNlmjNx%2B3pqWgfyaTdUz7Qt%2FTYIbut2s3uvI1vSztnWuwiqFPRuspM2ZoxFuhriWnoLxp41r6itbiNe06RvuomiOPirtJ4hYzgdTUPL2ryPSzfdSQyb2svFGERQZchbJGNe97hMY1gs0W%2BOWi9lyMe6rcg4LUzCpliu8%2ByqSmjp4RFELAfP%2F9k%3D&logoColor=white&link=https://paypal.me/navchandar//)](https://paypal.me/navchandar/) 
+[![BuymeCoffee Badge](https://img.shields.io/badge/-Buy%20a%20Coffee-ff813f?style=for-the-badge&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAP5SURBVFhH7ZdrTFNnGMfftvSUXmTcBtNCWy6mXBRoAZWL1GAgIRnSiGOZkmF0W3YpJEYXtIm3qPEWP%2BgHRRogQLgmEmPiEpOZGBSX%2BAUZLES3%2Bc0PRiMJX5a5ubPnlCMxT9tznrcDYxae%2FD6c0vP%2Bn185p%2B95ysTjnveKFSE1VoTU%2BF8Ina3NIjL4ST5aqwq30K3PCxzpViLVztVouSrcQk1FaSK59Hr93b0ulKAMn9Bs6wboIXcjVGlJcYt7DQpRhiRUk5UAVGfEGwTw4a7sZPNCQkNOMkoOhSQUo9OWlZXV%2FIdqbm622WwNeakoORSqUFdXl3wZoq3GxsalFBIEvdEYC5gAkxEwA2bTIpa3juGthXOAhVWAwSAsmdD%2B8rRUi%2FChWV%2FsENz5zJXHioBcVpjLCnJYgZOtfwO8LARypXfhHDjZ7WDF6UyjYVszEyAHJYdCEgJ2FaRAonh6o%2Fg74yPAnhxhULd3F6LMsFCFTlQ7rHEG6fhRSEsFppl4kf3wtST09EDZ24GRoApNf1cCoT996RJvWXBXBX6UhL4qZ5vSLSgwElShv45WgVCP1yneiMddFbgmCXmyNLtdH6HASFCFAGeyqb0yXey14a4KjEhCKas0Z2oyUVokOIRgn5W2Wq77OsCen5JuoOufUR%2F7JKHLH6%2B1J1kSLUZTrAEO7FaBSrKwOkGAsiaY7fGxKDYsJKHxPUXwKdva2k5EWy6Xy5OdgmLDQhKaO1QBQqOjo%2FJTgL%2Fchet9G60oNizUe2ibM8nr9crxnDUzMwOfZ%2BIL0mBEFfJX2bIz7HIHzhoaGgKheX8lygwLVWhoR64UOj8vN%2BEpv9%2BfnRqPAiNBFZoJ7tQTExNyE56qr6%2F35i%2FDxijE6Do6OuQmPJVhSzvssaO0SHAIua0f%2BHw%2BuQm55ubmpG9oUx5KiwSHUEtRqmdzpdyHXOPj4yA021qK0iLBIQS%2FyCC6s7MTNqTh4eGBgYG%2Bvr6enh6YbuGPcDUDgUB3d3dvb29%2Ff%2F%2Fg4ODIyMjY2FhdXd0GexKKUoBDCAYaEEKl1Wr0MRqDQWuM1QmCVqfTwHCIao%2BbekcDHELAy4MV%2FdtzwOzPB9q%2FH7N%2Ffgt5mgZ5%2FSt7dZ%2F9cYElGnWwy79oL0c5CvAJAb%2F4SqU9V3VMC45m5bZVaLkq3EKvj1V1NRDGtOBoxnWxFuAWAr6vIIxpwdHsXC11LlskGqF6Z5L6mBZgz06yGzvXobWqRCMEX5xXR6rESS2WWGRS%2Bvdc%2FTSqcPSaAgj9%2FG2JeE%2FAHovckYT2bXmHQudrM6eumKZusvBcYlPtrDLzXQmlxRmk%2FY5QaCGFaNY8%2FKaYCFpIIRqhZWVFSI0VIWWOe%2F4FR6A6eCoawHAAAAAASUVORK5CYII%3D&logoColor=white&link=https://www.buymeacoffee.com/navchandar//)](https://www.buymeacoffee.com/navchandar/) 
+[![Ko-Fi Badge](https://img.shields.io/badge/-Buy%20a%20KoFi-ff5f5f?style=for-the-badge&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAOiSURBVFhH7ZbLTxRBEMb963gkJIRleS4JyyJnDnqFKA%2BREOXAgcAJhAMEL77xoBdEjSQY8II3wchrgQUUdmZnusqvpofZzfDoBdF4mM2XSae3u%2BrXVdU1c4NLSv4rRUAmRUAmRUAmRUAmRUAmRUAmRUAmRUAmGYBo9jVlLfp1REfHfyjOZGjxM93v59JSMa6fp2QC2ssQMTkuuerqyjmQchTr38ICJZrE%2FllMBiB3M02KtEVflp0f2LmLJrUcV2PIwRBsy5bx2ndqTIR8aRmA1JYPpGDXdhxFsJdTFAzYsl1XhSftHNZrGkFc%2BUrLX2g7LSiYPM7K4NMCl5eH3EEmoO0dDQQf8Ef7BzwzQ733qKuLp6Zodw8EqDB%2B8pR6eqi7myYmaGs7h2joOGHLwSE3NIi1eJwnJ1l5GbRzwtTdU%2BhLqzggnNh16fAnd3aqqipqaBBVx%2BjWbZqb47t3KBaj%2BnqZxKC9nTY2XThGbLAXuxL57NDMY0FBkIjow8dgPlBxQFnLgplXs1RdrVpvcipFLS2EZ1OTcCQSMsYM1NaGNfxoAuuxC1R5ICQIVdzcLJcOBQCg9Y1CX1rFAVkWskAjI1RXCxpOJhUE00kPApJx0hcQe3sdrEeEcMUCIH2nYjG1uS0Fjr929wJHgS4RIRobo5oaam3V7uWsAYeewSCVUnV1PDCA0g6n7NojxEtLUiU6JJojJDhD%2FAD95u0ZKfN0TTWEK2PnbAxGR1G2ChVTGJ6ABsHDVerry7cibCm4ZTRxXbfMu%2FbSWrIWP3ioauJ%2BkAImTVNbSx0dlMlIg9BMf6sPedbBhB7IjkNDQ1wTVwFTczODBplCHzo89LrlCY33hHshgJ3jrBwJ49U1bmwM%2BdIyAZ10atiVCHlxkh4zOqpA4DEhg6gb7u%2Fn4ywuF3q3rNTSWLAAkQZjXlzkpqu%2By%2FJAiJD%2FApHTSz2Nj0v9trSAjAcHJX5K5Wm8Lf5gd492dunHOs2%2Fp55en%2BMsGqjYGgp85Jlw1ulpac3DwxI2ZPOEBuh6sezN7EvrQresrMxbPocGMgDRt1W5n8GtKYgTnlK8y8soW0mirvrC2GAXFmxucUWFbxAcZWWB8TNlAGLkBT%2FLCoBCQpyEww7Pi3T9PnsudkwcgUxAFRX0bl7sotPDsf7gKhQcn573ZuQkKytS77Bzfo5CMgFBCPj0NKfTwcdoUcKn5ouXPs1lVATQv1UEZFIEZFIEZFIEZFIEdLFKSn4Dz0s70NgRCBAAAAAASUVORK5CYII%3D&logoColor=1fb3ef&link=https://ko-fi.com/navchandar//)](https://ko-fi.com/navchandar/)
```

### Comparing `look_like_scanned-0.2.0/scanner/scanner.py` & `look_like_scanned-0.2.2/scanner/scanner.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-#!/usr/bin/env python
-"""Module to convert PDF/Images to look like they were scanned"""
-
-import os
-import io
-import random
-import argparse
-from pprint import pprint
-import pypdfium2 as pdfium
-from PIL import Image, ImageEnhance
-
-SUPPORTED_IMAGES = [".jpg", ".png", ".jpeg", ".webp"]
-SUPPORTED_DOCS = [".pdf", ".PDF"]
-CHOICES = ["y", "yes", "n", "no"]
-
-
-def parse_args():
-    """Parse input command-line arguments for the script"""
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-i",
-        "--input_folder",
-        type=str,
-        help="The input folder to read files from and convert (default: current directory)",
-    )
-    parser.add_argument(
-        "-f",
-        "--file_type_or_name",
-        type=str,
-        help="The file types to process or file name to process. Valid value - image, pdf, file names (default: pdf)",
-    )
-    parser.add_argument(
-        "-q",
-        "--file_quality",
-        type=int,
-        choices=range(50, 101, 5),
-        default=95,
-        help="The quality of the converted output files. Valid range - 50 to 100 increment in steps of 5 (default: 95)",
-    )
-    parser.add_argument(
-        "-a",
-        "--askew",
-        type=str.lower,
-        choices=CHOICES,
-        default="yes",
-        help="Make output documents slightly askew or slightly tilted (default: yes)",
-    )
-    parser.add_argument(
-        "-r",
-        "--recurse",
-        type=str.lower,
-        choices=CHOICES,
-        default="no",
-        help="Recurse in all sub folders to find matching files and convert them (default: no)",
-    )
-
-    return parser.parse_args()
-
-
-def get_argument(argument_name):
-    """
-    Gets the input folder from the command-line argument.
-    If no input folder provided, returns the current working directory.
-    """
-    args = parse_args()
-    if argument_name == "folder":
-        input_folder = os.getcwd()
-        if args.input_folder:
-            input_folder = args.input_folder
-        else:
-            print("Defaulting to current directory")
-        input_folder = os.path.abspath(input_folder)
-
-        # check if folder path exists
-        if os.path.exists(input_folder):
-            print(f"Processing files from {input_folder=}")
-        else:
-            print(f"Error: Input folder path not found: {input_folder}")
-        return input_folder
-
-    if argument_name == "quality":
-        return int(args.file_quality) if args.file_quality else 95
-
-    if argument_name == "askew":
-        return args.askew.lower().startswith("y") if args.askew else True
-
-    if argument_name == "recurse":
-        return args.recurse.lower().startswith("y") if args.recurse else True
-
-    if argument_name == "file_type":
-        match = (None, None)
-        if args.file_type_or_name:
-            file = args.file_type_or_name.lower()
-            if file == "image":
-                match = ("image", SUPPORTED_IMAGES)
-            elif any(f.endswith(file) or file.endswith(f) for f in SUPPORTED_IMAGES):
-                match = ("image", [args.file_type_or_name])
-            elif any(f.endswith(file) or file.endswith(f) for f in SUPPORTED_DOCS):
-                match = ("pdf", [args.file_type_or_name])
-            else:
-                print("Defaulting to find pdf files")
-        else:
-            match = ("pdf", SUPPORTED_DOCS)
-        return match
-
-
-def human_size(num, suffix="B"):
-    """Return file size in a human readable format"""
-    for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
-        if abs(num) < 1024.0:
-            return f"{num:3.1f}{unit}{suffix}"
-        num /= 1024.0
-    return f"{num:.1f}Yi{suffix}"
-
-
-def get_file_size(file_path):
-    """Get file size for a given file path"""
-    return human_size(os.stat(file_path).st_size)
-
-
-def reduce_image_quality(image, quality=100, compression="JPEG"):
-    """Reduce quality of a given image object"""
-    img_byte_array = io.BytesIO()
-    # Save the image to the in-memory file object
-    image.save(img_byte_array, quality=quality, format=compression)
-
-    # Rewind the file object to the beginning
-    img_byte_array.seek(0)
-    # Open the image from the in-memory file object
-    reduced_image = Image.open(img_byte_array)
-    return reduced_image
-
-
-def _change_image_to_byte_buffer(image, compression="JPEG"):
-    """
-    Save the image data to an in-memory file-like object
-    """
-    img_byte_array = io.BytesIO()
-    image.save(img_byte_array, quality=95, format=compression)
-    # Reset the file position to the beginning
-    img_byte_array.seek(0)
-    return img_byte_array
-
-
-def rotate_image(image, angle):
-    """Rotate PIL Image object with given angle value"""
-    rotated_image = image.rotate(
-        angle, resample=Image.BICUBIC, expand=True, fillcolor=(255, 255, 255)
-    )
-    return rotated_image
-
-
-def _convert_pdf_pages_to_jpg_list(pdf_path, image_quality=100, askew=True):
-    """
-    Reads given pdf file and reads all pages and converts them to image objects
-    """
-    images_list = []
-    doc = pdfium.PdfDocument(pdf_path)
-    for page in doc:
-        # increase render resolution for better scanned image quality
-        bitmap = page.render(scale=2)
-        image = bitmap.to_pil()
-
-        # Reduce image quality a little bit
-        image = reduce_image_quality(image, image_quality)
-        image = image.convert("RGB")
-
-        # increase brightness a little bit
-        enhancer = ImageEnhance.Brightness(image)
-        image = enhancer.enhance(random.uniform(1.01, 1.02))
-
-        # Rotate every image by a small random angle
-        if askew:
-            image = rotate_image(image, random.uniform(-0.55, 0.55))
-
-        image = _change_image_to_byte_buffer(image)
-        images_list.append(image)
-        page.close()
-    doc.close()
-    return images_list
-
-
-def _save_image_obj_to_pdf(images_list, output_pdf_path, pdf_version=17):
-    """
-    Save image objects into output pdf
-    """
-    pages_scanned = 0
-    output_pdf = pdfium.PdfDocument.new()
-    for image_file in images_list:
-        pdf_image = pdfium.PdfImage.new(output_pdf)
-        pdf_image.load_jpeg(image_file)
-        width, height = pdf_image.get_size()
-        # since render size increased by 2, decrease by same amount
-        width = width / 2
-        height = height / 2
-
-        matrix = pdfium.PdfMatrix().scale(width, height)
-        pdf_image.set_matrix(matrix)
-
-        page = output_pdf.new_page(width, height)
-        page.insert_obj(pdf_image)
-        page.gen_content()
-        page.close()
-        pdf_image.close()
-        pages_scanned += 1
-
-    output_pdf.save(output_pdf_path, version=pdf_version)
-    output_pdf.close()
-    file_size = get_file_size(output_pdf_path)
-    print(f"{output_pdf_path=} {file_size=}")
-    return pages_scanned
-
-
-def _add_suffix(filename):
-    """Adds output suffix to given file name"""
-    extension = "pdf"
-    suffix = "_output"
-    if "." in filename:
-        base_name, extension = filename.rsplit(".", 1)
-    else:
-        base_name = filename
-    # Add the suffix to the base name
-    new_base_name = base_name + suffix
-    # Combine the new base name and original extension to form the new filename
-    new_filename = new_base_name + "." + extension if extension else new_base_name
-    return new_filename
-
-
-def _calc_energy_savings(pages_scanned):
-    """
-    Calculate energy savings generated by preventing the printing and scanning
-    Approx energy required for production of 1 A4 sheet of paper = 50 Watt Hours
-
-    Sources:
-    https://www.apc.org/sites/default/files/SustainableITtips5_0.pdf
-    https://www.lowtechmagazine.com/what-is-the-embodied-energy-of-materials.html
-
-    Energy per capita usage: https://ourworldindata.org/grapher/per-capita-energy-use?tab=table
-    """
-
-    energy_req_for_one_page = 50
-    energy_saved = pages_scanned * energy_req_for_one_page
-
-    if energy_saved < 1000:
-        energy_saved = f"{energy_saved} Watt hours"
-    elif energy_saved < 1000000:
-        energy_saved = energy_saved / 1000
-        energy_saved = f"{energy_saved:.2f} kilo Watt hours"
-    else:
-        energy_saved = energy_saved / 1000000
-        energy_saved = f"{energy_saved:.2f} Mega Watt hours"
-
-    savings = f"You just saved {energy_saved} energy by avoiding printing {pages_scanned} pages of paper!"
-    print(savings)
-
-
-def convert_images_to_pdf(input_image_list, image_quality, askew):
-    """Converts all image files in a folder to PDF"""
-    images_list = []
-
-    # Output pdf name will be the fetched from first Image's name
-    output_pdf_path = os.path.splitext(input_image_list[0])[0] + "_output.pdf"
-    for image_path in input_image_list:
-        try:
-            image = Image.open(image_path)
-            # reduce image quality a little bit
-            image = reduce_image_quality(image, image_quality)
-            image = image.convert("RGB")
-
-            # Rotate every image by a small random angle
-            if askew:
-                image = rotate_image(image, random.uniform(-0.75, 0.75))
-
-            image = _change_image_to_byte_buffer(image)
-            images_list.append(image)
-        except Exception as e:
-            print(f"Error converting file {image_path} :-", e)
-
-    pages_scanned = _save_image_obj_to_pdf(images_list, output_pdf_path, pdf_version=17)
-    _calc_energy_savings(pages_scanned)
-    return output_pdf_path
-
-
-def convert_pdf_to_scanned(pdf_list, image_quality, askew):
-    """
-    Converts PDF files into scanned PDF files
-    """
-    output_file_list = []
-    pages_scanned = 0
-    for pdf_path in pdf_list:
-        try:
-            output_path = _add_suffix(pdf_path)
-            images = _convert_pdf_pages_to_jpg_list(pdf_path, image_quality, askew)
-            pages_scanned += _save_image_obj_to_pdf(images, output_path)
-            output_file_list.append(output_path)
-        except Exception as e:
-            print(f"Error converting file {pdf_path} :-", e)
-
-    _calc_energy_savings(pages_scanned)
-    return output_file_list
-
-
-def find_matching_files(input_folder, file_type_list, recurse=False):
-    """
-    Find files in given input folder and filter only matching file types.
-    If recurse is True, this method will identify all matching files in all sub directories.
-    """
-    files_list = []
-    try:
-        for file in os.listdir(input_folder):
-            path = os.path.join(input_folder, file)
-            if os.path.isfile(path) and any(
-                file.endswith(ext) for ext in file_type_list
-            ):
-                files_list.append(path)
-            if recurse and os.path.isdir(path):
-                files_list.extend(find_matching_files(path, file_type_list, recurse))
-    except Exception as e:
-        print("Error when searching for files :-", e)
-    return files_list
-
-
-def sort_by_top_level_directory(path):
-    """Method to help sort file paths based on level"""
-    directories = path.split(os.path.sep)
-    return len(directories)
-
-
-def main():
-    """Get input arguments and run the script"""
-
-    # Gather input arguments from command-line
-    input_folder = get_argument("folder")
-    quality = get_argument("quality")
-    askew = get_argument("askew")
-    recurse = get_argument("recurse")
-    doc_type, file_type_list = get_argument("file_type")
-    print(f"{quality=} {recurse=} {askew=} {doc_type=} {file_type_list=}")
-
-    # Gather the input files based on the arguments
-    files_list = find_matching_files(input_folder, file_type_list, recurse)
-    # Sort file paths so output gets saved in top level directory
-    files_list = sorted(files_list, key=sort_by_top_level_directory)
-
-    print(f"Matching Files Found: {len(files_list)}")
-    pprint(files_list)
-
-    # Convert the files found into output files
-    pdf_path = None
-    if doc_type == "image":
-        pdf_path = convert_images_to_pdf(files_list, quality, askew)
-    elif doc_type == "pdf":
-        pdf_path = convert_pdf_to_scanned(files_list, quality, askew)
-    else:
-        print("Error: Unsupported file format!")
-
-    if pdf_path:
-        pprint(f"The Output PDF files saved at {pdf_path}")
-    else:
-        print("No valid file type found. No output documents generated")
-
-
-if __name__ == "__main__":
-    main()
+#!/usr/bin/env python
+"""Module to convert PDF/Images to look like they were scanned"""
+
+import os
+import io
+import random
+import argparse
+from pprint import pprint
+import pypdfium2 as pdfium
+from PIL import Image, ImageEnhance
+
+SUPPORTED_IMAGES = [".jpg", ".png", ".jpeg", ".webp"]
+SUPPORTED_DOCS = [".pdf", ".PDF"]
+CHOICES = ["y", "yes", "n", "no"]
+
+
+def parse_args():
+    """Parse input command-line arguments for the script"""
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-i",
+        "--input_folder",
+        type=str,
+        help="The input folder to read files from and convert (default: current directory)",
+    )
+    parser.add_argument(
+        "-f",
+        "--file_type_or_name",
+        type=str,
+        help="The file types to process or file name to process. Valid value - image, pdf, file names (default: pdf)",
+    )
+    parser.add_argument(
+        "-q",
+        "--file_quality",
+        type=int,
+        choices=range(50, 101, 5),
+        default=95,
+        help="The quality of the converted output files. Valid range - 50 to 100 increment in steps of 5 (default: 95)",
+    )
+    parser.add_argument(
+        "-a",
+        "--askew",
+        type=str.lower,
+        choices=CHOICES,
+        default="yes",
+        help="Make output documents slightly askew or slightly tilted (default: yes)",
+    )
+    parser.add_argument(
+        "-r",
+        "--recurse",
+        type=str.lower,
+        choices=CHOICES,
+        default="no",
+        help="Recurse in all sub folders to find matching files and convert them (default: no)",
+    )
+
+    return parser.parse_args()
+
+
+def get_argument(argument_name):
+    """
+    Gets the input folder from the command-line argument.
+    If no input folder provided, returns the current working directory.
+    """
+    args = parse_args()
+    if argument_name == "folder":
+        input_folder = os.getcwd()
+        if args.input_folder:
+            input_folder = args.input_folder
+        else:
+            print("Defaulting to current directory")
+        input_folder = os.path.abspath(input_folder)
+
+        # check if folder path exists
+        if os.path.exists(input_folder):
+            print(f"Processing files from {input_folder=}")
+        else:
+            print(f"Error: Input folder path not found: {input_folder}")
+        return input_folder
+
+    if argument_name == "quality":
+        return int(args.file_quality) if args.file_quality else 95
+
+    if argument_name == "askew":
+        return args.askew.lower().startswith("y") if args.askew else True
+
+    if argument_name == "recurse":
+        return args.recurse.lower().startswith("y") if args.recurse else True
+
+    if argument_name == "file_type":
+        match = (None, None)
+        if args.file_type_or_name:
+            file = args.file_type_or_name.lower()
+            if file == "image":
+                match = ("image", SUPPORTED_IMAGES)
+            elif any(f.endswith(file) or file.endswith(f) for f in SUPPORTED_IMAGES):
+                match = ("image", [args.file_type_or_name])
+            elif any(f.endswith(file) or file.endswith(f) for f in SUPPORTED_DOCS):
+                match = ("pdf", [args.file_type_or_name])
+            else:
+                print("Defaulting to find pdf files")
+        else:
+            match = ("pdf", SUPPORTED_DOCS)
+        return match
+
+
+def human_size(num, suffix="B"):
+    """Return file size in a human readable format"""
+    for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
+        if abs(num) < 1024.0:
+            return f"{num:3.1f}{unit}{suffix}"
+        num /= 1024.0
+    return f"{num:.1f}Yi{suffix}"
+
+
+def get_file_size(file_path):
+    """Get file size for a given file path"""
+    return human_size(os.stat(file_path).st_size)
+
+
+def reduce_image_quality(image, quality=100, compression="JPEG"):
+    """Reduce quality of a given image object"""
+    img_byte_array = io.BytesIO()
+    # Save the image to the in-memory file object
+    image.save(img_byte_array, quality=quality, format=compression)
+
+    # Rewind the file object to the beginning
+    img_byte_array.seek(0)
+    # Open the image from the in-memory file object
+    reduced_image = Image.open(img_byte_array)
+    return reduced_image
+
+
+def _change_image_to_byte_buffer(image, compression="JPEG"):
+    """
+    Save the image data to an in-memory file-like object
+    """
+    img_byte_array = io.BytesIO()
+    image.save(img_byte_array, quality=95, format=compression)
+    # Reset the file position to the beginning
+    img_byte_array.seek(0)
+    return img_byte_array
+
+
+def rotate_image(image, angle):
+    """Rotate PIL Image object with given angle value"""
+    rotated_image = image.rotate(
+        angle, resample=Image.BICUBIC, expand=True, fillcolor=(255, 255, 255)
+    )
+    return rotated_image
+
+
+def _convert_pdf_pages_to_jpg_list(pdf_path, image_quality=100, askew=True):
+    """
+    Reads given pdf file and reads all pages and converts them to image objects
+    """
+    images_list = []
+    doc = pdfium.PdfDocument(pdf_path)
+    for page in doc:
+        # increase render resolution for better scanned image quality
+        bitmap = page.render(scale=2)
+        image = bitmap.to_pil()
+
+        # Reduce image quality a little bit
+        image = reduce_image_quality(image, image_quality)
+        image = image.convert("RGB")
+
+        # increase brightness a little bit
+        enhancer = ImageEnhance.Brightness(image)
+        image = enhancer.enhance(random.uniform(1.01, 1.02))
+
+        # Rotate every image by a small random angle
+        if askew:
+            image = rotate_image(image, random.uniform(-0.55, 0.55))
+
+        image = _change_image_to_byte_buffer(image)
+        images_list.append(image)
+        page.close()
+    doc.close()
+    return images_list
+
+
+def _save_image_obj_to_pdf(images_list, output_pdf_path, pdf_version=17):
+    """
+    Save image objects into output pdf
+    """
+    pages_scanned = 0
+    output_pdf = pdfium.PdfDocument.new()
+    for image_file in images_list:
+        pdf_image = pdfium.PdfImage.new(output_pdf)
+        pdf_image.load_jpeg(image_file)
+        width, height = pdf_image.get_size()
+        # since render size increased by 2, decrease by same amount
+        width = width / 2
+        height = height / 2
+
+        matrix = pdfium.PdfMatrix().scale(width, height)
+        pdf_image.set_matrix(matrix)
+
+        page = output_pdf.new_page(width, height)
+        page.insert_obj(pdf_image)
+        page.gen_content()
+        page.close()
+        pdf_image.close()
+        pages_scanned += 1
+
+    output_pdf.save(output_pdf_path, version=pdf_version)
+    output_pdf.close()
+    file_size = get_file_size(output_pdf_path)
+    print(f"{output_pdf_path=} {file_size=}")
+    return pages_scanned
+
+
+def _add_suffix(filename):
+    """Adds output suffix to given file name"""
+    extension = "pdf"
+    suffix = "_output"
+    if "." in filename:
+        base_name, extension = filename.rsplit(".", 1)
+    else:
+        base_name = filename
+    # Add the suffix to the base name
+    new_base_name = base_name + suffix
+    # Combine the new base name and original extension to form the new filename
+    new_filename = new_base_name + "." + extension if extension else new_base_name
+    return new_filename
+
+
+def _calc_energy_savings(pages_scanned):
+    """
+    Calculate energy savings generated by preventing the printing and scanning
+    Approx energy required for production of 1 A4 sheet of paper = 50 Watt Hours
+
+    Sources:
+    https://www.apc.org/sites/default/files/SustainableITtips5_0.pdf
+    https://www.lowtechmagazine.com/what-is-the-embodied-energy-of-materials.html
+
+    Energy per capita usage: https://ourworldindata.org/grapher/per-capita-energy-use?tab=table
+    """
+
+    energy_req_for_one_page = 50
+    energy_saved = pages_scanned * energy_req_for_one_page
+
+    if energy_saved < 1000:
+        energy_saved = f"{energy_saved} Watt hours"
+    elif energy_saved < 1000000:
+        energy_saved = energy_saved / 1000
+        energy_saved = f"{energy_saved:.2f} kilo Watt hours"
+    else:
+        energy_saved = energy_saved / 1000000
+        energy_saved = f"{energy_saved:.2f} Mega Watt hours"
+
+    savings = f"You just saved {energy_saved} energy by avoiding printing {pages_scanned} pages of paper!"
+    print(savings)
+
+
+def convert_images_to_pdf(input_image_list, image_quality, askew):
+    """Converts all image files in a folder to PDF"""
+    images_list = []
+
+    # Output pdf name will be the fetched from first Image's name
+    output_pdf_path = os.path.splitext(input_image_list[0])[0] + "_output.pdf"
+    for image_path in input_image_list:
+        try:
+            image = Image.open(image_path)
+            # reduce image quality a little bit
+            image = reduce_image_quality(image, image_quality)
+            image = image.convert("RGB")
+
+            # Rotate every image by a small random angle
+            if askew:
+                image = rotate_image(image, random.uniform(-0.75, 0.75))
+
+            image = _change_image_to_byte_buffer(image)
+            images_list.append(image)
+        except Exception as e:
+            print(f"Error converting file {image_path} :-", e)
+
+    pages_scanned = _save_image_obj_to_pdf(images_list, output_pdf_path, pdf_version=17)
+    _calc_energy_savings(pages_scanned)
+    return output_pdf_path
+
+
+def convert_pdf_to_scanned(pdf_list, image_quality, askew):
+    """
+    Converts PDF files into scanned PDF files
+    """
+    output_file_list = []
+    pages_scanned = 0
+    for pdf_path in pdf_list:
+        try:
+            output_path = _add_suffix(pdf_path)
+            images = _convert_pdf_pages_to_jpg_list(pdf_path, image_quality, askew)
+            pages_scanned += _save_image_obj_to_pdf(images, output_path)
+            output_file_list.append(output_path)
+        except Exception as e:
+            print(f"Error converting file {pdf_path} :-", e)
+
+    _calc_energy_savings(pages_scanned)
+    return output_file_list
+
+
+def find_matching_files(input_folder, file_type_list, recurse=False):
+    """
+    Find files in given input folder and filter only matching file types.
+    If recurse is True, this method will identify all matching files in all sub directories.
+    """
+    files_list = []
+    try:
+        for file in os.listdir(input_folder):
+            path = os.path.join(input_folder, file)
+            if os.path.isfile(path) and any(
+                file.endswith(ext) for ext in file_type_list
+            ):
+                files_list.append(path)
+            if recurse and os.path.isdir(path):
+                files_list.extend(find_matching_files(path, file_type_list, recurse))
+    except Exception as e:
+        print("Error when searching for files :-", e)
+    return files_list
+
+
+def sort_by_top_level_directory(path):
+    """Method to help sort file paths based on level"""
+    directories = path.split(os.path.sep)
+    return len(directories)
+
+
+def main():
+    """Get input arguments and run the script"""
+
+    # Gather input arguments from command-line
+    input_folder = get_argument("folder")
+    quality = get_argument("quality")
+    askew = get_argument("askew")
+    recurse = get_argument("recurse")
+    doc_type, file_type_list = get_argument("file_type")
+    print(f"{quality=} {recurse=} {askew=} {doc_type=} {file_type_list=}")
+
+    # Gather the input files based on the arguments
+    files_list = find_matching_files(input_folder, file_type_list, recurse)
+    # Sort file paths so output gets saved in top level directory
+    files_list = sorted(files_list, key=sort_by_top_level_directory)
+
+    print(f"Matching Files Found: {len(files_list)}")
+    pprint(files_list)
+
+    # Convert the files found into output files
+    pdf_path = None
+    if doc_type == "image":
+        pdf_path = convert_images_to_pdf(files_list, quality, askew)
+    elif doc_type == "pdf":
+        pdf_path = convert_pdf_to_scanned(files_list, quality, askew)
+    else:
+        print("Error: Unsupported file format!")
+
+    if pdf_path:
+        pprint(f"The Output PDF files saved at {pdf_path}")
+    else:
+        print("No valid file type found. No output documents generated")
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `look_like_scanned-0.2.0/PKG-INFO` & `look_like_scanned-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: look-like-scanned
-Version: 0.2.0
+Version: 0.2.2
 Summary: Python script to make documents look like they were scanned.
 Home-page: https://github.com/navchandar/look-like-scanned
 Keywords: pdf,scan,scanner,image-to-pdf,pdf-to-scan
 Author: navchandar
 Author-email: 12165092+navchandar@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -46,21 +46,33 @@
  - There are options to combine / convert image files into PDF as well.
 
  - Output PDF files are saved in the same input folder with a suffix _"filename_output.pdf"_
 
 
 ## Installation
 
+Install from the [Python Package Index (PyPI)](https://pypi.org/project/look-like-scanned/)
+```shell
+pip install look-like-scanned
+```
+
+Or to install latest version from GitHub
 ```shell
 git clone https://github.com/navchandar/look-like-scanned.git
 pip install poetry
 poetry install
 pip install .
 ```
 
+### Verify Installation:
+```shell
+# Print help message and usage options available
+scanner -h
+```
+
 
 ## Usage
 
 This package uses [PIL](https://pypi.org/project/Pillow/) and [pypdfium2](https://pypi.org/project/pypdfium2/) to convert and manipulate image and pdf objects.
 
 This is extended to provide a command-line interface (CLI) for easy usage.
 
@@ -113,26 +125,25 @@
     - Example: `-r yes` or `--recurse no`
 
 
 ❗❗ **Note:** ❗❗
 
 - The supported file types are: ".jpg", ".png", ".jpeg", ".webp", ".pdf".
 
-- The output PDF file size will be bigger compared to the input because the files are stored in image format.
+- The output PDF file size **will be bigger** than the input file because the pages are stored in image format.
 
 - Bookmarks / Links / Metadata will be removed when saving the output file.
 
 - Password protected PDF files are not yet supported.
 
 
 ## License
  
  [MIT license](LICENSE)
 
 
 ## Support This Project
 
-[![Paypal Badge](https://img.shields.io/badge/-Paypal-0070ba?style=flat-square&logo=data%3Aimage%2Fjpeg%3Bbase64%2C%2F9j%2F4AAQSkZJRgABAQAAAQABAAD%2F2wBDAAIBAQIBAQICAgICAgICAwUDAwMDAwYEBAMFBwYHBwcGBwcICQsJCAgKCAcHCg0KCgsMDAwMBwkODw0MDgsMDAz%2F2wBDAQICAgMDAwYDAwYMCAcIDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAz%2FwgARCAAwADADAREAAhEBAxEB%2F8QAHQAAAgIBBQAAAAAAAAAAAAAABwgGCQIAAwQFCv%2FEABwBAAEEAwEAAAAAAAAAAAAAAAYCAwcIAAEFBP%2FaAAwDAQACEAMQAAAAdZSiYpqCdXycvSppyvSMUbKuLEBqPeeyxsX4su2oRUX2QQweZr0j8qBdJUyhfS8vqPk%2FEV3tVbWaafq4naOlKlyuxybCnaAD9sq5XBxxSVysGLjOdMLWa4WvNYLKIfSoU5sq7yAEYZOOCWb7LwozP%2F%2FEAD0QAAAFAwMBBAQJDQAAAAAAAAECAwQFBgcIABESCSExUbUKd5bTExQXIiM4cYGyMjM3QUJHV2GCg5Oh0f%2FaAAgBAQABPwDA%2FBOyVX4SWdlpaztqZKVlKHhHTx68pJg4cO11GCBzqqHMkJjnMYRMYwiOpvA%2FHWnYpZ49srZts2aJmUWWNRkcBCFKG5hH6HuAA30NqsOAP2W%2FsH7IR%2FuNQdjsQaheC1aW3sO4WN3FJSEf7jTXp94%2BuEiGJZGzqhD9oGCjY7tAf7Os7MFLJ0dhFeSWibNWqi5SLoabeNHbOk2CLhmsmwXOmomoVIDEOUxQMBiiA66eX1ArGer%2BA8tQ11vLjrUB0%2Fat%2BKujs3z8SNkxIqKahimHifYQ7e42lq4lEC8jzEmUviLs%2FwD3Ta6Mk0U5pT0omYP2ivVCj%2BLXo4eXVUVjcyq6Cm6gfTER8QTeMwevTKmanKYxRKnyEfyuW466gwGHAC%2BX0n7v5%2Fy1xrp5ciYBWOKHYBbfQHlzfXpM9x14K0Nu4NAwcJp0%2BFwX%2BSZUBLqpltkiE8e3RC8zCBS8x8ADfXSKoCoLP3IYVYJVmK8m7aJtC8vzqQn3NyAB%2FwBDrqF%2FUAvoXwt9PeWrjrp8Bw6fdkDeNvYDy5vr0mWuzvr80NT3MTN2EWq7%2FqUMBR%2FBrFzGSlbuW6WlqgZKulwcCinxUMQOIfZq32CNKtDg8h6QcvBKOxVNlVQ3%2B4dtYOYMzU5WEZUEwzJHQ0SsksVuqUyainEdwKBdg27tdQr5mAV9fV9P%2BWuddPMAPgFY3l%2FD%2BB8uQ11P%2Bjlc7N%2FIY9VRFQQDWNSQM3bJuhUE5CchEAHYNU3jdIYsMho2SdM3r9qqZRRRrv8ABmEw7bBv9msE6EYw2MdLqHj2qbtymdZUTIFBQxvhTB2jtv3AGg7zcdvm9gB%2BouuoaQwYB3z9X0%2F5c41g5nRY%2BlMG7NRMteW1cXLRVEQjV4ydVbHoOGixGCJTpqEOqBiHIYBKJTAGidQ%2BwJQMX5cbPe2kb77U3d%2FDmpZo0k%2BuDYV2%2BOO5llawj%2BRjfcvqDz0x0gYdFmxvVZtq1alEqSZKyjgAgf5tE6h1gOH6c7P%2B2cb77Wc2dllKtwfvHExd5LVyspK0PNs2bJnVrBZw7WUYLkTTTTKqJjnMbYoFKA6%2F%2F8QAJREAAQMDAgYDAAAAAAAAAAAAAQACAwQFEQYhBxASEyIxQVFS%2F9oACAECAQE%2FAPTyVEySeQRsCFhuDvcZTrFVN9xqSLtPDZRhNGHloRHytDUzJ7k1jgjBGwbgLs0rh5ALiJZqQQNqIAnHJ8VnA6VwspuueSX84VwLx8ppL1WWyOS2TOn9Y2VQOlxaz7K9vXC2EMppXfrCgoWTjL06O307vMgFa21tSw0rqGl3JUjhISftAjGXLSesKOgpe28bqxXZtZRiePYFa9uM0t3lLX%2BITnuduTyzhqcD1BoCptWXWKM08cmGKoqHzydx5yTz%2F8QAJREAAQMCBgIDAQAAAAAAAAAAAQACAwQRBQYSISJRBzEQFUET%2F9oACAEDAQE%2FAG%2BrIyCPmUa%2BDtMxCDtMlAFmFWYNym%2Fqx%2BoMVEXD2mTTu9FXqO1lzEJGnROVZhGoot2t0s4TD%2BTG9qhYAdSufZNlmjNx%2B3pqWgfyaTdUz7Qt%2FTYIbut2s3uvI1vSztnWuwiqFPRuspM2ZoxFuhriWnoLxp41r6itbiNe06RvuomiOPirtJ4hYzgdTUPL2ryPSzfdSQyb2svFGERQZchbJGNe97hMY1gs0W%2BOWi9lyMe6rcg4LUzCpliu8%2ByqSmjp4RFELAfP%2F9k%3D&logoColor=white&link=https://paypal.me/navchandar//)](https://paypal.me/navchandar/) 
-[![Ko-Fi Badge](https://img.shields.io/badge/-Buy%20a%20KoFi-ff5f5f?style=flat-square&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAOiSURBVFhH7ZbLTxRBEMb963gkJIRleS4JyyJnDnqFKA%2BREOXAgcAJhAMEL77xoBdEjSQY8II3wchrgQUUdmZnusqvpofZzfDoBdF4mM2XSae3u%2BrXVdU1c4NLSv4rRUAmRUAmRUAmRUAmRUAmRUAmRUAmRUAmGYBo9jVlLfp1REfHfyjOZGjxM93v59JSMa6fp2QC2ssQMTkuuerqyjmQchTr38ICJZrE%2FllMBiB3M02KtEVflp0f2LmLJrUcV2PIwRBsy5bx2ndqTIR8aRmA1JYPpGDXdhxFsJdTFAzYsl1XhSftHNZrGkFc%2BUrLX2g7LSiYPM7K4NMCl5eH3EEmoO0dDQQf8Ef7BzwzQ733qKuLp6Zodw8EqDB%2B8pR6eqi7myYmaGs7h2joOGHLwSE3NIi1eJwnJ1l5GbRzwtTdU%2BhLqzggnNh16fAnd3aqqipqaBBVx%2BjWbZqb47t3KBaj%2BnqZxKC9nTY2XThGbLAXuxL57NDMY0FBkIjow8dgPlBxQFnLgplXs1RdrVpvcipFLS2EZ1OTcCQSMsYM1NaGNfxoAuuxC1R5ICQIVdzcLJcOBQCg9Y1CX1rFAVkWskAjI1RXCxpOJhUE00kPApJx0hcQe3sdrEeEcMUCIH2nYjG1uS0Fjr929wJHgS4RIRobo5oaam3V7uWsAYeewSCVUnV1PDCA0g6n7NojxEtLUiU6JJojJDhD%2FAD95u0ZKfN0TTWEK2PnbAxGR1G2ChVTGJ6ABsHDVerry7cibCm4ZTRxXbfMu%2FbSWrIWP3ioauJ%2BkAImTVNbSx0dlMlIg9BMf6sPedbBhB7IjkNDQ1wTVwFTczODBplCHzo89LrlCY33hHshgJ3jrBwJ49U1bmwM%2BdIyAZ10atiVCHlxkh4zOqpA4DEhg6gb7u%2Fn4ywuF3q3rNTSWLAAkQZjXlzkpqu%2By%2FJAiJD%2FApHTSz2Nj0v9trSAjAcHJX5K5Wm8Lf5gd492dunHOs2%2Fp55en%2BMsGqjYGgp85Jlw1ulpac3DwxI2ZPOEBuh6sezN7EvrQresrMxbPocGMgDRt1W5n8GtKYgTnlK8y8soW0mirvrC2GAXFmxucUWFbxAcZWWB8TNlAGLkBT%2FLCoBCQpyEww7Pi3T9PnsudkwcgUxAFRX0bl7sotPDsf7gKhQcn573ZuQkKytS77Bzfo5CMgFBCPj0NKfTwcdoUcKn5ouXPs1lVATQv1UEZFIEZFIEZFIEZFIEdLFKSn4Dz0s70NgRCBAAAAAASUVORK5CYII%3D&logoColor=1fb3ef&link=https://ko-fi.com/navchandar//)](https://ko-fi.com/navchandar/) 
-[![BuymeCoffee Badge](https://img.shields.io/badge/-Buy%20a%20Coffee-ff813f?style=flat-square&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAP5SURBVFhH7ZdrTFNnGMfftvSUXmTcBtNCWy6mXBRoAZWL1GAgIRnSiGOZkmF0W3YpJEYXtIm3qPEWP%2BgHRRogQLgmEmPiEpOZGBSX%2BAUZLES3%2Bc0PRiMJX5a5ubPnlCMxT9tznrcDYxae%2FD6c0vP%2Bn185p%2B95ysTjnveKFSE1VoTU%2BF8Ina3NIjL4ST5aqwq30K3PCxzpViLVztVouSrcQk1FaSK59Hr93b0ulKAMn9Bs6wboIXcjVGlJcYt7DQpRhiRUk5UAVGfEGwTw4a7sZPNCQkNOMkoOhSQUo9OWlZXV%2FIdqbm622WwNeakoORSqUFdXl3wZoq3GxsalFBIEvdEYC5gAkxEwA2bTIpa3juGthXOAhVWAwSAsmdD%2B8rRUi%2FChWV%2FsENz5zJXHioBcVpjLCnJYgZOtfwO8LARypXfhHDjZ7WDF6UyjYVszEyAHJYdCEgJ2FaRAonh6o%2Fg74yPAnhxhULd3F6LMsFCFTlQ7rHEG6fhRSEsFppl4kf3wtST09EDZ24GRoApNf1cCoT996RJvWXBXBX6UhL4qZ5vSLSgwElShv45WgVCP1yneiMddFbgmCXmyNLtdH6HASFCFAGeyqb0yXey14a4KjEhCKas0Z2oyUVokOIRgn5W2Wq77OsCen5JuoOufUR%2F7JKHLH6%2B1J1kSLUZTrAEO7FaBSrKwOkGAsiaY7fGxKDYsJKHxPUXwKdva2k5EWy6Xy5OdgmLDQhKaO1QBQqOjo%2FJTgL%2Fchet9G60oNizUe2ibM8nr9crxnDUzMwOfZ%2BIL0mBEFfJX2bIz7HIHzhoaGgKheX8lygwLVWhoR64UOj8vN%2BEpv9%2BfnRqPAiNBFZoJ7tQTExNyE56qr6%2F35i%2FDxijE6Do6OuQmPJVhSzvssaO0SHAIua0f%2BHw%2BuQm55ubmpG9oUx5KiwSHUEtRqmdzpdyHXOPj4yA021qK0iLBIQS%2FyCC6s7MTNqTh4eGBgYG%2Bvr6enh6YbuGPcDUDgUB3d3dvb29%2Ff%2F%2Fg4ODIyMjY2FhdXd0GexKKUoBDCAYaEEKl1Wr0MRqDQWuM1QmCVqfTwHCIao%2BbekcDHELAy4MV%2FdtzwOzPB9q%2FH7N%2Ffgt5mgZ5%2FSt7dZ%2F9cYElGnWwy79oL0c5CvAJAb%2F4SqU9V3VMC45m5bZVaLkq3EKvj1V1NRDGtOBoxnWxFuAWAr6vIIxpwdHsXC11LlskGqF6Z5L6mBZgz06yGzvXobWqRCMEX5xXR6rESS2WWGRS%2Bvdc%2FTSqcPSaAgj9%2FG2JeE%2FAHovckYT2bXmHQudrM6eumKZusvBcYlPtrDLzXQmlxRmk%2FY5QaCGFaNY8%2FKaYCFpIIRqhZWVFSI0VIWWOe%2F4FR6A6eCoawHAAAAAASUVORK5CYII%3D&logoColor=white&link=https://www.buymeacoffee.com/navchandar//)](https://www.buymeacoffee.com/navchandar/) 
-
+[![Paypal Badge](https://img.shields.io/badge/-Paypal-0070ba?style=for-the-badge&logo=data%3Aimage%2Fjpeg%3Bbase64%2C%2F9j%2F4AAQSkZJRgABAQAAAQABAAD%2F2wBDAAIBAQIBAQICAgICAgICAwUDAwMDAwYEBAMFBwYHBwcGBwcICQsJCAgKCAcHCg0KCgsMDAwMBwkODw0MDgsMDAz%2F2wBDAQICAgMDAwYDAwYMCAcIDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAz%2FwgARCAAwADADAREAAhEBAxEB%2F8QAHQAAAgIBBQAAAAAAAAAAAAAABwgGCQIAAwQFCv%2FEABwBAAEEAwEAAAAAAAAAAAAAAAYCAwcIAAEFBP%2FaAAwDAQACEAMQAAAAdZSiYpqCdXycvSppyvSMUbKuLEBqPeeyxsX4su2oRUX2QQweZr0j8qBdJUyhfS8vqPk%2FEV3tVbWaafq4naOlKlyuxybCnaAD9sq5XBxxSVysGLjOdMLWa4WvNYLKIfSoU5sq7yAEYZOOCWb7LwozP%2F%2FEAD0QAAAFAwMBBAQJDQAAAAAAAAECAwQFBgcIABESCSExUbUKd5bTExQXIiM4cYGyMjM3QUJHV2GCg5Oh0f%2FaAAgBAQABPwDA%2FBOyVX4SWdlpaztqZKVlKHhHTx68pJg4cO11GCBzqqHMkJjnMYRMYwiOpvA%2FHWnYpZ49srZts2aJmUWWNRkcBCFKG5hH6HuAA30NqsOAP2W%2FsH7IR%2FuNQdjsQaheC1aW3sO4WN3FJSEf7jTXp94%2BuEiGJZGzqhD9oGCjY7tAf7Os7MFLJ0dhFeSWibNWqi5SLoabeNHbOk2CLhmsmwXOmomoVIDEOUxQMBiiA66eX1ArGer%2BA8tQ11vLjrUB0%2Fat%2BKujs3z8SNkxIqKahimHifYQ7e42lq4lEC8jzEmUviLs%2FwD3Ta6Mk0U5pT0omYP2ivVCj%2BLXo4eXVUVjcyq6Cm6gfTER8QTeMwevTKmanKYxRKnyEfyuW466gwGHAC%2BX0n7v5%2Fy1xrp5ciYBWOKHYBbfQHlzfXpM9x14K0Nu4NAwcJp0%2BFwX%2BSZUBLqpltkiE8e3RC8zCBS8x8ADfXSKoCoLP3IYVYJVmK8m7aJtC8vzqQn3NyAB%2FwBDrqF%2FUAvoXwt9PeWrjrp8Bw6fdkDeNvYDy5vr0mWuzvr80NT3MTN2EWq7%2FqUMBR%2FBrFzGSlbuW6WlqgZKulwcCinxUMQOIfZq32CNKtDg8h6QcvBKOxVNlVQ3%2B4dtYOYMzU5WEZUEwzJHQ0SsksVuqUyainEdwKBdg27tdQr5mAV9fV9P%2BWuddPMAPgFY3l%2FD%2BB8uQ11P%2Bjlc7N%2FIY9VRFQQDWNSQM3bJuhUE5CchEAHYNU3jdIYsMho2SdM3r9qqZRRRrv8ABmEw7bBv9msE6EYw2MdLqHj2qbtymdZUTIFBQxvhTB2jtv3AGg7zcdvm9gB%2BouuoaQwYB3z9X0%2F5c41g5nRY%2BlMG7NRMteW1cXLRVEQjV4ydVbHoOGixGCJTpqEOqBiHIYBKJTAGidQ%2BwJQMX5cbPe2kb77U3d%2FDmpZo0k%2BuDYV2%2BOO5llawj%2BRjfcvqDz0x0gYdFmxvVZtq1alEqSZKyjgAgf5tE6h1gOH6c7P%2B2cb77Wc2dllKtwfvHExd5LVyspK0PNs2bJnVrBZw7WUYLkTTTTKqJjnMbYoFKA6%2F%2F8QAJREAAQMDAgYDAAAAAAAAAAAAAQACAwQFEQYhBxASEyIxQVFS%2F9oACAECAQE%2FAPTyVEySeQRsCFhuDvcZTrFVN9xqSLtPDZRhNGHloRHytDUzJ7k1jgjBGwbgLs0rh5ALiJZqQQNqIAnHJ8VnA6VwspuueSX84VwLx8ppL1WWyOS2TOn9Y2VQOlxaz7K9vXC2EMppXfrCgoWTjL06O307vMgFa21tSw0rqGl3JUjhISftAjGXLSesKOgpe28bqxXZtZRiePYFa9uM0t3lLX%2BITnuduTyzhqcD1BoCptWXWKM08cmGKoqHzydx5yTz%2F8QAJREAAQMCBgIDAQAAAAAAAAAAAQACAwQRBQYSISJRBzEQFUET%2F9oACAEDAQE%2FAG%2BrIyCPmUa%2BDtMxCDtMlAFmFWYNym%2Fqx%2BoMVEXD2mTTu9FXqO1lzEJGnROVZhGoot2t0s4TD%2BTG9qhYAdSufZNlmjNx%2B3pqWgfyaTdUz7Qt%2FTYIbut2s3uvI1vSztnWuwiqFPRuspM2ZoxFuhriWnoLxp41r6itbiNe06RvuomiOPirtJ4hYzgdTUPL2ryPSzfdSQyb2svFGERQZchbJGNe97hMY1gs0W%2BOWi9lyMe6rcg4LUzCpliu8%2ByqSmjp4RFELAfP%2F9k%3D&logoColor=white&link=https://paypal.me/navchandar//)](https://paypal.me/navchandar/) 
+[![BuymeCoffee Badge](https://img.shields.io/badge/-Buy%20a%20Coffee-ff813f?style=for-the-badge&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAP5SURBVFhH7ZdrTFNnGMfftvSUXmTcBtNCWy6mXBRoAZWL1GAgIRnSiGOZkmF0W3YpJEYXtIm3qPEWP%2BgHRRogQLgmEmPiEpOZGBSX%2BAUZLES3%2Bc0PRiMJX5a5ubPnlCMxT9tznrcDYxae%2FD6c0vP%2Bn185p%2B95ysTjnveKFSE1VoTU%2BF8Ina3NIjL4ST5aqwq30K3PCxzpViLVztVouSrcQk1FaSK59Hr93b0ulKAMn9Bs6wboIXcjVGlJcYt7DQpRhiRUk5UAVGfEGwTw4a7sZPNCQkNOMkoOhSQUo9OWlZXV%2FIdqbm622WwNeakoORSqUFdXl3wZoq3GxsalFBIEvdEYC5gAkxEwA2bTIpa3juGthXOAhVWAwSAsmdD%2B8rRUi%2FChWV%2FsENz5zJXHioBcVpjLCnJYgZOtfwO8LARypXfhHDjZ7WDF6UyjYVszEyAHJYdCEgJ2FaRAonh6o%2Fg74yPAnhxhULd3F6LMsFCFTlQ7rHEG6fhRSEsFppl4kf3wtST09EDZ24GRoApNf1cCoT996RJvWXBXBX6UhL4qZ5vSLSgwElShv45WgVCP1yneiMddFbgmCXmyNLtdH6HASFCFAGeyqb0yXey14a4KjEhCKas0Z2oyUVokOIRgn5W2Wq77OsCen5JuoOufUR%2F7JKHLH6%2B1J1kSLUZTrAEO7FaBSrKwOkGAsiaY7fGxKDYsJKHxPUXwKdva2k5EWy6Xy5OdgmLDQhKaO1QBQqOjo%2FJTgL%2Fchet9G60oNizUe2ibM8nr9crxnDUzMwOfZ%2BIL0mBEFfJX2bIz7HIHzhoaGgKheX8lygwLVWhoR64UOj8vN%2BEpv9%2BfnRqPAiNBFZoJ7tQTExNyE56qr6%2F35i%2FDxijE6Do6OuQmPJVhSzvssaO0SHAIua0f%2BHw%2BuQm55ubmpG9oUx5KiwSHUEtRqmdzpdyHXOPj4yA021qK0iLBIQS%2FyCC6s7MTNqTh4eGBgYG%2Bvr6enh6YbuGPcDUDgUB3d3dvb29%2Ff%2F%2Fg4ODIyMjY2FhdXd0GexKKUoBDCAYaEEKl1Wr0MRqDQWuM1QmCVqfTwHCIao%2BbekcDHELAy4MV%2FdtzwOzPB9q%2FH7N%2Ffgt5mgZ5%2FSt7dZ%2F9cYElGnWwy79oL0c5CvAJAb%2F4SqU9V3VMC45m5bZVaLkq3EKvj1V1NRDGtOBoxnWxFuAWAr6vIIxpwdHsXC11LlskGqF6Z5L6mBZgz06yGzvXobWqRCMEX5xXR6rESS2WWGRS%2Bvdc%2FTSqcPSaAgj9%2FG2JeE%2FAHovckYT2bXmHQudrM6eumKZusvBcYlPtrDLzXQmlxRmk%2FY5QaCGFaNY8%2FKaYCFpIIRqhZWVFSI0VIWWOe%2F4FR6A6eCoawHAAAAAASUVORK5CYII%3D&logoColor=white&link=https://www.buymeacoffee.com/navchandar//)](https://www.buymeacoffee.com/navchandar/) 
+[![Ko-Fi Badge](https://img.shields.io/badge/-Buy%20a%20KoFi-ff5f5f?style=for-the-badge&logo=data%3Aimage%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAIAAADYYG7QAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAAEnQAABJ0Ad5mH3gAAAOiSURBVFhH7ZbLTxRBEMb963gkJIRleS4JyyJnDnqFKA%2BREOXAgcAJhAMEL77xoBdEjSQY8II3wchrgQUUdmZnusqvpofZzfDoBdF4mM2XSae3u%2BrXVdU1c4NLSv4rRUAmRUAmRUAmRUAmRUAmRUAmRUAmRUAmGYBo9jVlLfp1REfHfyjOZGjxM93v59JSMa6fp2QC2ssQMTkuuerqyjmQchTr38ICJZrE%2FllMBiB3M02KtEVflp0f2LmLJrUcV2PIwRBsy5bx2ndqTIR8aRmA1JYPpGDXdhxFsJdTFAzYsl1XhSftHNZrGkFc%2BUrLX2g7LSiYPM7K4NMCl5eH3EEmoO0dDQQf8Ef7BzwzQ733qKuLp6Zodw8EqDB%2B8pR6eqi7myYmaGs7h2joOGHLwSE3NIi1eJwnJ1l5GbRzwtTdU%2BhLqzggnNh16fAnd3aqqipqaBBVx%2BjWbZqb47t3KBaj%2BnqZxKC9nTY2XThGbLAXuxL57NDMY0FBkIjow8dgPlBxQFnLgplXs1RdrVpvcipFLS2EZ1OTcCQSMsYM1NaGNfxoAuuxC1R5ICQIVdzcLJcOBQCg9Y1CX1rFAVkWskAjI1RXCxpOJhUE00kPApJx0hcQe3sdrEeEcMUCIH2nYjG1uS0Fjr929wJHgS4RIRobo5oaam3V7uWsAYeewSCVUnV1PDCA0g6n7NojxEtLUiU6JJojJDhD%2FAD95u0ZKfN0TTWEK2PnbAxGR1G2ChVTGJ6ABsHDVerry7cibCm4ZTRxXbfMu%2FbSWrIWP3ioauJ%2BkAImTVNbSx0dlMlIg9BMf6sPedbBhB7IjkNDQ1wTVwFTczODBplCHzo89LrlCY33hHshgJ3jrBwJ49U1bmwM%2BdIyAZ10atiVCHlxkh4zOqpA4DEhg6gb7u%2Fn4ywuF3q3rNTSWLAAkQZjXlzkpqu%2By%2FJAiJD%2FApHTSz2Nj0v9trSAjAcHJX5K5Wm8Lf5gd492dunHOs2%2Fp55en%2BMsGqjYGgp85Jlw1ulpac3DwxI2ZPOEBuh6sezN7EvrQresrMxbPocGMgDRt1W5n8GtKYgTnlK8y8soW0mirvrC2GAXFmxucUWFbxAcZWWB8TNlAGLkBT%2FLCoBCQpyEww7Pi3T9PnsudkwcgUxAFRX0bl7sotPDsf7gKhQcn573ZuQkKytS77Bzfo5CMgFBCPj0NKfTwcdoUcKn5ouXPs1lVATQv1UEZFIEZFIEZFIEZFIEdLFKSn4Dz0s70NgRCBAAAAAASUVORK5CYII%3D&logoColor=1fb3ef&link=https://ko-fi.com/navchandar//)](https://ko-fi.com/navchandar/)
```

