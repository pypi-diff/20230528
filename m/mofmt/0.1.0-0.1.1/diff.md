# Comparing `tmp/mofmt-0.1.0-py3-none-any.whl.zip` & `tmp/mofmt-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 73142 bytes, number of entries: 25
+Zip file size: 73146 bytes, number of entries: 25
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mofmt/__init__.py
 -rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 mofmt/__main__.py
 -rw-r--r--  2.0 unx       69 b- defN 80-Jan-01 00:00 mofmt/collecting/__init__.py
 -rw-r--r--  2.0 unx     4553 b- defN 80-Jan-01 00:00 mofmt/collecting/collector.py
 -rw-r--r--  2.0 unx       80 b- defN 80-Jan-01 00:00 mofmt/io/__init__.py
--rw-r--r--  2.0 unx     1217 b- defN 80-Jan-01 00:00 mofmt/io/io.py
--rw-r--r--  2.0 unx      974 b- defN 80-Jan-01 00:00 mofmt/mofmt.py
+-rw-r--r--  2.0 unx     1216 b- defN 80-Jan-01 00:00 mofmt/io/io.py
+-rw-r--r--  2.0 unx      982 b- defN 80-Jan-01 00:00 mofmt/mofmt.py
 -rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 mofmt/parsing/__init__.py
 -rw-r--r--  2.0 unx    41279 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/Modelica.interp
 -rw-r--r--  2.0 unx   302166 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/Modelica.py
 -rw-r--r--  2.0 unx     1818 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/Modelica.tokens
 -rw-r--r--  2.0 unx    27480 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/ModelicaLexer.interp
 -rw-r--r--  2.0 unx    27122 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/ModelicaLexer.py
 -rw-r--r--  2.0 unx     1818 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/ModelicaLexer.tokens
 -rw-r--r--  2.0 unx    36457 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/ModelicaListener.py
 -rw-r--r--  2.0 unx      166 b- defN 80-Jan-01 00:00 mofmt/parsing/generated/__init__.py
 -rw-r--r--  2.0 unx     7775 b- defN 80-Jan-01 00:00 mofmt/parsing/parser.py
 -rw-r--r--  2.0 unx      890 b- defN 80-Jan-01 00:00 mofmt/parsing/parsing.py
 -rw-r--r--  2.0 unx       75 b- defN 80-Jan-01 00:00 mofmt/printing/__init__.py
 -rw-r--r--  2.0 unx     1223 b- defN 80-Jan-01 00:00 mofmt/printing/printing.py
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 mofmt-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3792 b- defN 80-Jan-01 00:00 mofmt-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mofmt-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 mofmt-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2091 b- defN 16-Jan-01 00:00 mofmt-0.1.0.dist-info/RECORD
-25 files, 462360 bytes uncompressed, 69752 bytes compressed:  84.9%
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 mofmt-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3792 b- defN 80-Jan-01 00:00 mofmt-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mofmt-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 mofmt-0.1.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2091 b- defN 16-Jan-01 00:00 mofmt-0.1.1.dist-info/RECORD
+25 files, 462367 bytes uncompressed, 69756 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: mofmt/printing/__init__.py
 Comment: 
 
 Filename: mofmt/printing/printing.py
 Comment: 
 
-Filename: mofmt-0.1.0.dist-info/LICENSE
+Filename: mofmt-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: mofmt-0.1.0.dist-info/METADATA
+Filename: mofmt-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: mofmt-0.1.0.dist-info/WHEEL
+Filename: mofmt-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: mofmt-0.1.0.dist-info/entry_points.txt
+Filename: mofmt-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mofmt-0.1.0.dist-info/RECORD
+Filename: mofmt-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mofmt/io/io.py

```diff
@@ -9,15 +9,15 @@
     def __init__(self, file: Path) -> None:
         self.message = f"{file} is not a valid Modelica file"
         super().__init__(self.message)
 
 
 def get_files_from_dir(directory: Path) -> list[Path]:
     """Return list of Modelica files inside directory"""
-    return list(directory.glob("*/*.mo"))
+    return list(directory.rglob("*.mo"))
 
 
 def read_file(path: Path) -> str:
     """Return file contents"""
 
     if not path.is_file():
         raise FileNotFoundError(f"file {path} not found")
```

## mofmt/mofmt.py

```diff
@@ -6,22 +6,22 @@
 from mofmt.printing import pretty_print
 
 
 class ParsingError(Exception):
     """Raised when parsing fails"""
 
     def __init__(self, f: Path) -> None:
-        self.message = f"cannot parse {f}. Probably it not a valid modelica file"
+        self.message = f"cannot parse {f}. Probably it is not a valid modelica file"
         super().__init__(self.message)
 
 
 def main():
     argv = sys.argv
     if len(argv) != 2:
-        raise SystemExit("mofmt takes one argument (file/directory path)")
+        raise SystemExit("mofmt takes only one argument (file/directory path)")
     p = Path(argv[1])
     if p.is_dir():
         modelica_files = get_files_from_dir(p)
     else:
         modelica_files = [p]
     for file in modelica_files:
         contents = read_file(file)
```

## Comparing `mofmt-0.1.0.dist-info/LICENSE` & `mofmt-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mofmt-0.1.0.dist-info/METADATA` & `mofmt-0.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mofmt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Modelica Code Formatter
 License: MIT
 Author: Eryk Mroczek
 Author-email: mroczek.eryk@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mofmt-0.1.0.dist-info/RECORD` & `mofmt-0.1.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 mofmt/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mofmt/__main__.py,sha256=b73MqZ_xxbl_zEFZng6tA0cfbJWun8WjT0Ddsqkt1bY,33
 mofmt/collecting/__init__.py,sha256=lmS7soEjmgYn-BZdD4HnQiXAlK5LU8HrM5hl1Yb9gtE,69
 mofmt/collecting/collector.py,sha256=9QD125_v2iLjTllnxMsI9BjlXVchIQ0Qu7Uqvh7kogA,4553
 mofmt/io/__init__.py,sha256=21XaFTNHuEAoBaaUufgLHeFBmEoTG184x_zsCyDW3LY,80
-mofmt/io/io.py,sha256=pXOucsF1v-UZT0TBWHhPBC98ByET9U8Zm6RZ3hhBilM,1217
-mofmt/mofmt.py,sha256=2aoVuDw5s9G9wMMtQ6A_V_dCm2oLqN-6kalw4OxQQo4,974
+mofmt/io/io.py,sha256=w0zcnDh_Y0UL4hHUwtlZ81sl--BFucUQuBWDNN54beA,1216
+mofmt/mofmt.py,sha256=mvyS9tz8qCT1AKXTxkUEUIrDVgBAy7lJ_Ur2NNyTtbk,982
 mofmt/parsing/__init__.py,sha256=7uZXBN_534KW1-OmESAEWh-DOWAxu3rqemLPIojd4g0,83
 mofmt/parsing/generated/Modelica.interp,sha256=4pKUOhSzpu4bSa1sL4SmDNzwGuxMIEkua0dRKCDuO5I,41279
 mofmt/parsing/generated/Modelica.py,sha256=WzhI_gYfKeRjlhNscQYmafgo3-dhXoeUBoEba4vrgW4,302166
 mofmt/parsing/generated/Modelica.tokens,sha256=nEhvvcJjSLDfCmzOXwOZ7uy_wl309tu3IgUel69e__g,1818
 mofmt/parsing/generated/ModelicaLexer.interp,sha256=S0R2oKpQjjbejkpIPk2keJVbfMGq9OyD533dt-gwDv4,27480
 mofmt/parsing/generated/ModelicaLexer.py,sha256=fCnzeG4GfLgIZxbF-qlOWi-tDKQcwnilV7c-H91dWOo,27122
 mofmt/parsing/generated/ModelicaLexer.tokens,sha256=nEhvvcJjSLDfCmzOXwOZ7uy_wl309tu3IgUel69e__g,1818
 mofmt/parsing/generated/ModelicaListener.py,sha256=4XqKTnjuI_w6ikQa5TZIaXQS3ObwfVw0iIiRyXTJwLQ,36457
 mofmt/parsing/generated/__init__.py,sha256=lS_HjJcS0HyiJ4HZx8nzE5oWBHELFgcf9p9XJkTO-zY,166
 mofmt/parsing/parser.py,sha256=WWy9DcNjecg_Ej8OOZbaSadeMUwneS93i3NZcWlq0oo,7775
 mofmt/parsing/parsing.py,sha256=A2n_-xK-LviRCnQAJxkt5UBI5xZKrRmZOjkxvZMuN54,890
 mofmt/printing/__init__.py,sha256=WoIdWUdCMjPu05xxEDkiQsqLvgT6BJd5IQylrDgbh00,75
 mofmt/printing/printing.py,sha256=ugvAg96L5rXHIQGxtkrnMyqO84vDlgVVEuZ2V29U4A8,1223
-mofmt-0.1.0.dist-info/LICENSE,sha256=dgflMB87NFabDKfZVu7XBg2M3fvv6MzfrQ6eLeDoYic,1069
-mofmt-0.1.0.dist-info/METADATA,sha256=wFK9NtIUr6xy2KSGsdnRmagEBo359K9pSuRTByd9wsU,3792
-mofmt-0.1.0.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-mofmt-0.1.0.dist-info/entry_points.txt,sha256=OX5RiOFxcysf3SizHLEHHf5n6MdMjFqsZp5QgfA4umM,42
-mofmt-0.1.0.dist-info/RECORD,,
+mofmt-0.1.1.dist-info/LICENSE,sha256=dgflMB87NFabDKfZVu7XBg2M3fvv6MzfrQ6eLeDoYic,1069
+mofmt-0.1.1.dist-info/METADATA,sha256=Z_uFry1BiofOGwIb8ovH_23HzwS5a1zPQwWMTx6lLgc,3792
+mofmt-0.1.1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+mofmt-0.1.1.dist-info/entry_points.txt,sha256=OX5RiOFxcysf3SizHLEHHf5n6MdMjFqsZp5QgfA4umM,42
+mofmt-0.1.1.dist-info/RECORD,,
```

