# Comparing `tmp/leaf-focus-0.5.3.tar.gz` & `tmp/leaf-focus-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaf-focus-0.5.3.tar", last modified: Tue Mar 14 10:45:59 2023, max compression
+gzip compressed data, was "leaf-focus-0.6.0.tar", last modified: Sun May 28 10:06:04 2023, max compression
```

## Comparing `leaf-focus-0.5.3.tar` & `leaf-focus-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 10:45:59.500202 leaf-focus-0.5.3/
--rw-rw-rw-   0        0        0    11558 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       73 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3772 2023-03-14 10:45:59.501203 leaf-focus-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2468 2022-12-29 10:38:30.000000 leaf-focus-0.5.3/README.md
--rw-rw-rw-   0        0        0        7 2023-03-14 10:37:09.000000 leaf-focus-0.5.3/VERSION
--rw-rw-rw-   0        0        0     3773 2023-03-14 10:36:11.000000 leaf-focus-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0      452 2022-12-29 08:01:16.000000 leaf-focus-0.5.3/requirements-dev.txt
--rw-rw-rw-   0        0        0      212 2023-03-14 10:33:45.000000 leaf-focus-0.5.3/requirements.txt
--rw-rw-rw-   0        0        0      147 2023-03-14 10:45:59.501203 leaf-focus-0.5.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-14 10:45:59.481901 leaf-focus-0.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-03-14 10:45:59.488903 leaf-focus-0.5.3/src/leaf_focus/
--rw-rw-rw-   0        0        0      116 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/__init__.py
--rw-rw-rw-   0        0        0     5815 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/app.py
--rw-rw-rw-   0        0        0     3127 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-14 10:45:59.494201 leaf-focus-0.5.3/src/leaf_focus/ocr/
--rw-rw-rw-   0        0        0       46 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/ocr/__init__.py
--rw-rw-rw-   0        0        0    10118 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/ocr/keras_ocr.py
--rw-rw-rw-   0        0        0    14278 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/ocr/model.py
-drwxrwxrwx   0        0        0        0 2023-03-14 10:45:59.496201 leaf-focus-0.5.3/src/leaf_focus/pdf/
--rw-rw-rw-   0        0        0       45 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/pdf/__init__.py
--rw-rw-rw-   0        0        0    18067 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/src/leaf_focus/pdf/model.py
--rw-rw-rw-   0        0        0    13000 2022-12-29 08:01:16.000000 leaf-focus-0.5.3/src/leaf_focus/pdf/xpdf.py
--rw-rw-rw-   0        0        0     7076 2022-12-29 09:01:47.000000 leaf-focus-0.5.3/src/leaf_focus/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-14 10:45:59.493198 leaf-focus-0.5.3/src/leaf_focus.egg-info/
--rw-rw-rw-   0        0        0     3772 2023-03-14 10:45:59.000000 leaf-focus-0.5.3/src/leaf_focus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-03-14 10:45:59.000000 leaf-focus-0.5.3/src/leaf_focus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 10:45:59.000000 leaf-focus-0.5.3/src/leaf_focus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-03-14 10:45:59.000000 leaf-focus-0.5.3/src/leaf_focus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      508 2023-03-14 10:45:59.000000 leaf-focus-0.5.3/src/leaf_focus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-14 10:45:59.000000 leaf-focus-0.5.3/src/leaf_focus.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-14 10:45:59.500202 leaf-focus-0.5.3/tests/
--rw-rw-rw-   0        0        0     3111 2022-12-29 08:57:39.000000 leaf-focus-0.5.3/tests/test_cli.py
--rw-rw-rw-   0        0        0     7108 2023-03-14 10:27:55.000000 leaf-focus-0.5.3/tests/test_keras_ocr.py
--rw-rw-rw-   0        0        0     2195 2022-12-10 10:38:01.000000 leaf-focus-0.5.3/tests/test_utils.py
--rw-rw-rw-   0        0        0     3259 2022-12-29 08:57:39.000000 leaf-focus-0.5.3/tests/test_xpdf_image.py
--rw-rw-rw-   0        0        0     9123 2022-12-29 08:57:39.000000 leaf-focus-0.5.3/tests/test_xpdf_info.py
--rw-rw-rw-   0        0        0     3194 2022-12-29 08:57:39.000000 leaf-focus-0.5.3/tests/test_xpdf_text.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.510548 leaf-focus-0.6.0/
+-rw-rw-rw-   0        0        0    11558 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0       73 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3772 2023-05-28 10:06:04.510548 leaf-focus-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2468 2022-12-29 10:38:30.000000 leaf-focus-0.6.0/README.md
+-rw-rw-rw-   0        0        0        7 2023-05-28 03:56:32.000000 leaf-focus-0.6.0/VERSION
+-rw-rw-rw-   0        0        0     4488 2023-05-28 09:56:14.000000 leaf-focus-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0      458 2023-05-28 03:40:07.000000 leaf-focus-0.6.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      170 2023-05-28 09:41:38.000000 leaf-focus-0.6.0/requirements.txt
+-rw-rw-rw-   0        0        0      147 2023-05-28 10:06:04.511549 leaf-focus-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.490492 leaf-focus-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.498545 leaf-focus-0.6.0/src/leaf_focus/
+-rw-rw-rw-   0        0        0      116 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/src/leaf_focus/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-05-28 07:35:10.000000 leaf-focus-0.6.0/src/leaf_focus/app.py
+-rw-rw-rw-   0        0        0     3133 2023-05-28 07:45:43.000000 leaf-focus-0.6.0/src/leaf_focus/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.504546 leaf-focus-0.6.0/src/leaf_focus/ocr/
+-rw-rw-rw-   0        0        0       46 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/src/leaf_focus/ocr/__init__.py
+-rw-rw-rw-   0        0        0    10632 2023-05-28 09:27:03.000000 leaf-focus-0.6.0/src/leaf_focus/ocr/keras_ocr.py
+-rw-rw-rw-   0        0        0    14366 2023-05-28 07:42:51.000000 leaf-focus-0.6.0/src/leaf_focus/ocr/model.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.506548 leaf-focus-0.6.0/src/leaf_focus/pdf/
+-rw-rw-rw-   0        0        0       45 2022-12-10 10:38:01.000000 leaf-focus-0.6.0/src/leaf_focus/pdf/__init__.py
+-rw-rw-rw-   0        0        0    18405 2023-05-28 07:46:32.000000 leaf-focus-0.6.0/src/leaf_focus/pdf/model.py
+-rw-rw-rw-   0        0        0    13199 2023-05-28 08:58:13.000000 leaf-focus-0.6.0/src/leaf_focus/pdf/xpdf.py
+-rw-rw-rw-   0        0        0     7347 2023-05-28 08:58:13.000000 leaf-focus-0.6.0/src/leaf_focus/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.502546 leaf-focus-0.6.0/src/leaf_focus.egg-info/
+-rw-rw-rw-   0        0        0     3772 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      487 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 10:06:04.000000 leaf-focus-0.6.0/src/leaf_focus.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 10:06:04.509547 leaf-focus-0.6.0/tests/
+-rw-rw-rw-   0        0        0     3111 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0     7477 2023-05-28 07:51:11.000000 leaf-focus-0.6.0/tests/test_keras_ocr.py
+-rw-rw-rw-   0        0        0     2191 2023-05-28 07:14:26.000000 leaf-focus-0.6.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0     3259 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_xpdf_image.py
+-rw-rw-rw-   0        0        0     9123 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_xpdf_info.py
+-rw-rw-rw-   0        0        0     3194 2022-12-29 08:57:39.000000 leaf-focus-0.6.0/tests/test_xpdf_text.py
```

### Comparing `leaf-focus-0.5.3/LICENSE` & `leaf-focus-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.5.3/PKG-INFO` & `leaf-focus-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaf-focus
-Version: 0.5.3
+Version: 0.6.0
 Summary: Extract structured text from pdf files.
 Project-URL: Homepage, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Changelog, https://github.com/anotherbyte-net/leaf-focus/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Tracker, https://github.com/anotherbyte-net/leaf-focus/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `leaf-focus-0.5.3/README.md` & `leaf-focus-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.5.3/src/leaf_focus/app.py` & `leaf-focus-0.6.0/src/leaf_focus/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import dataclasses
 import datetime
 import logging
 import pathlib
 import typing
 
 from leaf_focus import utils
-from leaf_focus.ocr import model as ocr_model, keras_ocr
-from leaf_focus.pdf import model as pdf_model, xpdf
+from leaf_focus.ocr import keras_ocr
+from leaf_focus.ocr import model as ocr_model
+from leaf_focus.pdf import model as pdf_model
+from leaf_focus.pdf import xpdf
+from leaf_focus.utils import ValidatePathMethod
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class AppArgs:
     """Arguments for running the application."""
@@ -37,22 +40,23 @@
     log_level: typing.Optional[str] = None
     """the log level"""
 
 
 class App:
     """The main application."""
 
-    def __init__(self, exe_dir: pathlib.Path):
+    def __init__(self, exe_dir: pathlib.Path) -> None:
         """Create a new instance of the application.
 
         Args:
             exe_dir: The path to the directory containing the executable files.
         """
         if not exe_dir or not exe_dir.exists() or not exe_dir.is_dir():
-            raise NotADirectoryError(f"The path '{exe_dir or ''}' is not a directory.")
+            msg = f"The path '{exe_dir or ''}' is not a directory."
+            raise NotADirectoryError(msg)
         self._exe_dir = exe_dir
 
     def run(self, app_args: AppArgs) -> bool:
         """Run the application.
 
         Args:
             app_args: The application arguments.
@@ -60,20 +64,24 @@
         Returns:
             bool: True if the text extraction succeeded, otherwise false.
         """
         timestamp_start = datetime.datetime.utcnow()
         logger.info("Starting leaf-focus")
 
         input_pdf = utils.validate_path(
-            "input pdf", app_args.input_pdf, must_exist=True
+            "input pdf",
+            app_args.input_pdf,
+            ValidatePathMethod.MUST_EXIST,
         )
         app_args.input_pdf = input_pdf
 
         output_dir = utils.validate_path(
-            "output directory", app_args.output_dir, must_exist=False
+            "output directory",
+            app_args.output_dir,
+            ValidatePathMethod.NO_OPINION,
         )
         app_args.output_dir = output_dir
 
         # create the output directory
         if not output_dir.is_dir():
             logger.warning("Creating output directory '%s'.", output_dir)
             output_dir.mkdir(exist_ok=True, parents=True)
@@ -100,15 +108,17 @@
 
         timestamp_finish = datetime.datetime.utcnow()
         program_duration = timestamp_finish - timestamp_start
         logger.info("Finished (duration %s)", program_duration)
         return True
 
     def pdf_info(
-        self, prog: xpdf.XpdfProgram, app_args: AppArgs
+        self,
+        prog: xpdf.XpdfProgram,
+        app_args: AppArgs,
     ) -> pdf_model.XpdfInfoResult:
         """Get the pdf file information.
 
         Args:
             prog: The program to run.
             app_args: The application arguments.
 
@@ -119,15 +129,17 @@
             include_metadata=True,
             first_page=app_args.first_page,
             last_page=app_args.last_page,
         )
         return prog.info(app_args.input_pdf, app_args.output_dir, xpdf_info_args)
 
     def pdf_text(
-        self, prog: xpdf.XpdfProgram, app_args: AppArgs
+        self,
+        prog: xpdf.XpdfProgram,
+        app_args: AppArgs,
     ) -> pdf_model.XpdfTextResult:
         """Get the text embedded in the pdf.
 
         Args:
             prog: The program to run.
             app_args: The application arguments.
 
@@ -139,33 +151,39 @@
             use_original_layout=True,
             first_page=app_args.first_page,
             last_page=app_args.last_page,
         )
         return prog.text(app_args.input_pdf, app_args.output_dir, xpdf_text_args)
 
     def pdf_images(
-        self, prog: xpdf.XpdfProgram, app_args: AppArgs
+        self,
+        prog: xpdf.XpdfProgram,
+        app_args: AppArgs,
     ) -> pdf_model.XpdfImageResult:
         """Get each page in the pdf as a separate image.
 
         Args:
             prog: The program to run.
             app_args: The application arguments.
 
         Returns:
             pdf_model.XpdfImageResult: The result from the program.
         """
         xpdf_image_args = pdf_model.XpdfImageArgs(use_grayscale=True)
         xpdf_image = prog.image(
-            app_args.input_pdf, app_args.output_dir, xpdf_image_args
+            app_args.input_pdf,
+            app_args.output_dir,
+            xpdf_image_args,
         )
         return xpdf_image
 
     def pdf_ocr(
-        self, xpdf_image: pdf_model.XpdfImageResult, app_args: AppArgs
+        self,
+        xpdf_image: pdf_model.XpdfImageResult,
+        app_args: AppArgs,
     ) -> typing.Generator[ocr_model.KerasOcrResult, typing.Any, None]:
         """Recognise text on the pdf page images.
 
         Args:
             xpdf_image: The result from the pdf image program.
             app_args: The application arguments.
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus/cli.py` & `leaf-focus-0.6.0/src/leaf_focus/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     Returns:
         int: Program exit code.
     """
     if args is None:
         args = sys.argv[1:]
 
     logging.basicConfig(
-        format="%(asctime)s [%(levelname)-8s] %(message)s", level=logging.DEBUG
+        format="%(asctime)s [%(levelname)-8s] %(message)s",
+        level=logging.DEBUG,
     )
     logger = logging.getLogger(__name__)
 
     parser = argparse.ArgumentParser(
         prog="leaf-focus",
         description="Extract structured text from a pdf file.",
     )
@@ -96,15 +97,15 @@
         )
 
         logging.getLogger().setLevel((app_args.log_level or "info").upper())
 
         result = app_inst.run(app_args)
         return 0 if result is True else 1
 
-    except utils.LeafFocusException as error:
+    except utils.LeafFocusError as error:
         logger.error("Error: %s - %s", error.__class__.__name__, str(error))
         return 1
 
     except Exception as error:  # pylint: disable=broad-except
         logger.error("Error: %s - %s", error.__class__.__name__, str(error))
         return 2
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus/ocr/keras_ocr.py` & `leaf-focus-0.6.0/src/leaf_focus/ocr/keras_ocr.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import logging
 import os
 import pathlib
 import typing
 
 import numpy as np
 
-from leaf_focus.ocr import model
 from leaf_focus import utils
+from leaf_focus.ocr import model
 
 logger = logging.getLogger(__name__)
 
 
 class OpticalCharacterRecognition:
     """OCR implementation using keras-ocr."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Create a new OpticalCharacterRecognition."""
         self._pipeline = None
 
     def engine_create(self) -> None:
         """Create the OCR engine.
 
         Returns:
@@ -44,20 +44,24 @@
 
         import tensorflow as tf  # pylint: disable=import-outside-toplevel
 
         # also set the tf logger level
 
         tf.get_logger().setLevel(log_level)
 
+        # check the CPU / GPU in use
+        gpus = tf.config.list_physical_devices("GPU")
+        logger.info("GPUs in use: '%s'.", gpus)
+
         try:
             import keras_ocr  # pylint: disable=import-outside-toplevel
         except ModuleNotFoundError as error:
             msg = "Cannot run ocr on this Python version."
             logger.error(msg)
-            raise utils.LeafFocusException(msg) from error
+            raise utils.LeafFocusError(msg) from error
 
         # TODO: allow specifying path to weights files for detector
         # detector_weights_path = ""
         # detector = keras_ocr.detection.Detector(weights=None)
         # detector.model = keras_ocr.detection.build_keras_model(
         #     weights_path=detector_weights_path, backbone_name="vgg"
         # )
@@ -72,19 +76,21 @@
         # recognizer.model.load_weights(recognizer_weights_path)
         recognizer = None
 
         # see: https://github.com/faustomorales/keras-ocr
         # keras-ocr will automatically download pretrained
         # weights for the detector and recognizer.
         self._pipeline = keras_ocr.pipeline.Pipeline(
-            detector=detector, recognizer=recognizer
+            detector=detector,
+            recognizer=recognizer,
         )
 
     def engine_run(
-        self, image_file: pathlib.Path
+        self,
+        image_file: pathlib.Path,
     ) -> typing.Tuple[typing.List, typing.Any]:
         """Run the recognition engine.
 
         Args:
             image_file: The path to the image file.
 
         Returns:
@@ -92,18 +98,23 @@
                 and list of recognition results.
         """
         try:
             import keras_ocr  # pylint: disable=import-outside-toplevel
         except ModuleNotFoundError as error:
             msg = "Cannot run ocr on this Python version."
             logger.error(msg)
-            raise utils.LeafFocusException(msg) from error
+            raise utils.LeafFocusError(msg) from error
 
         self.engine_create()
 
+        if not self._pipeline:
+            msg = "Keras OCR pipeline has not been initialised yet."
+            logger.error(msg)
+            raise utils.LeafFocusError(msg)
+
         images = [keras_ocr.tools.read(str(image_file))]
         return images, self._pipeline.recognize(images)
 
     def engine_annotate(
         self,
         image: typing.Optional[np.ndarray],
         predictions: typing.List[typing.Tuple[typing.Any, typing.Any]],
@@ -120,37 +131,41 @@
             None
         """
         try:
             import keras_ocr  # pylint: disable=import-outside-toplevel
         except ModuleNotFoundError as error:
             msg = "Cannot run ocr on this Python version."
             logger.error(msg)
-            raise utils.LeafFocusException(msg) from error
+            raise utils.LeafFocusError(msg) from error
 
         keras_ocr.tools.drawAnnotations(image=image, predictions=predictions, ax=axis)
 
     def recognise_text(
-        self, image_file: pathlib.Path, output_dir: pathlib.Path
+        self,
+        image_file: pathlib.Path,
+        output_dir: pathlib.Path,
     ) -> model.KerasOcrResult:
         """Recognise text in an image file.
 
         Args:
             image_file: The path to the image file.
             output_dir: The directory to write the results.
 
         Returns:
             model.KerasOcrResult: The text recognition results.
         """
         if not image_file:
-            raise utils.LeafFocusException("Must supply image file.")
+            msg = "Must supply image file."
+            raise utils.LeafFocusError(msg)
         if not output_dir:
-            raise utils.LeafFocusException("Must supply output directory.")
+            msg = "Must supply output directory."
+            raise utils.LeafFocusError(msg)
         if not image_file.exists():
             msg = f"Image file does not exist '{image_file}'."
-            raise utils.LeafFocusException(msg) from FileNotFoundError(image_file)
+            raise utils.LeafFocusError(msg) from FileNotFoundError(image_file)
 
         # check if output files already exist
         annotations_file = utils.output_root(image_file, "annotations", output_dir)
         annotations_file = annotations_file.with_suffix(".png")
 
         predictions_file = utils.output_root(image_file, "predictions", output_dir)
         predictions_file = predictions_file.with_suffix(".csv")
@@ -169,15 +184,16 @@
             )
             all_items = list(model.TextItem.load(predictions_file))
             result.items = model.TextItem.order_text_lines(all_items)
             return result
 
         # read in the image
         logger.debug(
-            "Creating predictions and annotations files for '%s'.", image_file.stem
+            "Creating predictions and annotations files for '%s'.",
+            image_file.stem,
         )
 
         # Each list of predictions in prediction_groups is a list of
         # (word, box) tuples.
         images, prediction_groups = self.engine_run(image_file)
 
         # Plot and save the predictions
@@ -203,41 +219,44 @@
             image: The image data.
             predictions: The text recognition results.
 
         Returns:
             None
         """
         if not annotation_file:
-            raise utils.LeafFocusException("Must supply annotation file.")
-        if image is None or image.size < 1 or len(image.shape) != 3:
+            msg = "Must supply annotation file."
+            raise utils.LeafFocusError(msg)
+
+        expected_image_shape = 3
+        if image is None or image.size < 1 or len(image.shape) != expected_image_shape:
             msg_image = image.shape if image is not None else None
-            raise utils.LeafFocusException(
-                f"Must supply valid image data, not '{msg_image}'."
-            )
+            msg = f"Must supply valid image data, not '{msg_image}'."
+            raise utils.LeafFocusError(msg)
         if not predictions:
             predictions = []
 
         logger.info("Saving OCR image to '%s'.", annotation_file)
 
-        import matplotlib  # pylint: disable=import-outside-toplevel
+        import matplotlib as mpl  # pylint: disable=import-outside-toplevel
         from matplotlib import pyplot as plt  # pylint: disable=import-outside-toplevel
 
-        matplotlib.use("agg")
+        mpl.use("agg")
 
         annotation_file.parent.mkdir(exist_ok=True, parents=True)
 
         fig, axis = plt.subplots(figsize=(20, 20))
 
         self.engine_annotate(image, predictions, axis)
 
         fig.savefig(str(annotation_file))
         plt.close(fig)
 
     def convert_predictions(
-        self, predictions: typing.List[typing.Tuple[typing.Any, typing.Any]]
+        self,
+        predictions: typing.List[typing.Tuple[typing.Any, typing.Any]],
     ) -> typing.List[typing.List[model.TextItem]]:
         """Convert predictions to items.
 
         Args:
             predictions: The list of recognised text.
 
         Returns:
@@ -266,17 +285,19 @@
             items_file: Write the text items to this file.
             items: The text items to save.
 
         Returns:
             None
         """
         if not items_file:
-            raise utils.LeafFocusException("Must supply predictions file.")
+            msg = "Must supply predictions file."
+            raise utils.LeafFocusError(msg)
         if not items:
-            raise utils.LeafFocusException("Must supply predictions data.")
+            msg = "Must supply predictions data."
+            raise utils.LeafFocusError(msg)
 
         logger.info("Saving OCR predictions to '%s'.", items_file)
 
         items_list = list(items)
         model.TextItem.save(items_file, items_list)
 
     def _build_name(self, prefix: str, middle: str, suffix: str):
@@ -289,8 +310,8 @@
 
         Returns:
             str: The built name.
         """
         prefix = prefix.strip("-")
         middle = middle.strip("-")
         suffix = suffix if suffix.startswith(".") else "." + suffix
-        return "-".join([prefix, middle]) + suffix
+        return f"{prefix}-{middle}" + suffix
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus/ocr/model.py` & `leaf-focus-0.6.0/src/leaf_focus/ocr/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Models for OCR processing."""
+from __future__ import annotations
+
 import csv
 import dataclasses
 import logging
 import math
-import pathlib
 import typing
 
-
+if typing.TYPE_CHECKING:
+    import pathlib
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class TextItem:
     """One found text item (could be a word or phrase) in an image."""
 
@@ -25,46 +27,46 @@
 
     bottom_right_x: float
     bottom_right_y: float
 
     bottom_left_x: float
     bottom_left_y: float
 
-    line_number: typing.Optional[int] = None
-    line_order: typing.Optional[int] = None
+    line_number: int | None = None
+    line_order: int | None = None
 
     @property
-    def top_left(self) -> typing.Tuple[float, float]:
+    def top_left(self) -> tuple[float, float]:
         """Get the top left point.
 
         Returns:
             The x and y coordinates.
         """
         return self.top_left_x, self.top_left_y
 
     @property
-    def top_right(self) -> typing.Tuple[float, float]:
+    def top_right(self) -> tuple[float, float]:
         """Get the top right point.
 
         Returns:
             The x and y coordinates.
         """
         return self.top_right_x, self.top_right_y
 
     @property
-    def bottom_right(self) -> typing.Tuple[float, float]:
+    def bottom_right(self) -> tuple[float, float]:
         """Get the bottom right point.
 
         Returns:
              The x and y coordinates.
         """
         return self.bottom_right_x, self.bottom_right_y
 
     @property
-    def bottom_left(self) -> typing.Tuple[float, float]:
+    def bottom_left(self) -> tuple[float, float]:
         """Get the bottom left point.
 
         Returns:
             The x and y coordinates.
         """
         return self.bottom_left_x, self.bottom_left_y
 
@@ -93,25 +95,35 @@
         side1 = abs(self.top_left_y - self.bottom_left_y)
         side2 = abs(self.top_left_x - self.bottom_left_x)
         if side2 == 0:
             return side1
         return math.sqrt(pow(side1, 2) + pow(side2, 2))
 
     @property
-    def line_bounds(self) -> typing.Tuple[float, float]:
+    def line_bounds(self) -> tuple[float, float]:
         """Line bounds from top of text to bottom of text."""
         top_bound = min(
-            [self.top_left_y, self.top_right_y, self.bottom_left_y, self.bottom_right_y]
+            [
+                self.top_left_y,
+                self.top_right_y,
+                self.bottom_left_y,
+                self.bottom_right_y,
+            ],
         )
         bottom_bound = max(
-            [self.top_left_y, self.top_right_y, self.bottom_left_y, self.bottom_right_y]
+            [
+                self.top_left_y,
+                self.top_right_y,
+                self.bottom_left_y,
+                self.bottom_right_y,
+            ],
         )
         return top_bound, bottom_bound
 
-    def is_same_line(self, other: "TextItem") -> bool:
+    def is_same_line(self, other: TextItem) -> bool:
         """Check if the vertical midpoints of this item and another item overlap.
 
         Calculated as the midpoint +- 1/3 of the height of the text.
 
         Args:
             other (TextItem): The text item to compare.
 
@@ -268,15 +280,15 @@
             bool: True if the item is approximately vertical.
         """
         # -0.1 -> 0.1 is strictly vertical
         # give a bit of buffer
         return self.slope_left_top_bottom == math.inf
 
     @classmethod
-    def save(cls, path: pathlib.Path, items: typing.List["TextItem"]) -> None:
+    def save(cls, path: pathlib.Path, items: list[TextItem]) -> None:
         """Save found text items to a file.
 
         Args:
             path: Write the items to this file.
             items: The items to save.
 
         Returns:
@@ -293,45 +305,46 @@
             "top_right_x",
             "top_right_y",
             "bottom_right_x",
             "bottom_right_y",
             "bottom_left_x",
             "bottom_left_y",
         ]
-        with open(path, "wt", newline="", encoding="utf8") as file_path:
+        with open(path, "w", newline="", encoding="utf8") as file_path:
             writer = csv.DictWriter(file_path, fields)
             writer.writeheader()
             sorted_items = sorted(
-                items, key=lambda i: (i.line_number or 0, i.line_order or 0)
+                items,
+                key=lambda i: (i.line_number or 0, i.line_order or 0),
             )
             writer.writerows([dataclasses.asdict(i) for i in sorted_items])
 
         logger.debug("Saved OCR items to '%s'.", path)
 
     @classmethod
-    def load(cls, path: pathlib.Path) -> typing.Generator["TextItem", typing.Any, None]:
+    def load(cls, path: pathlib.Path) -> typing.Generator[TextItem, typing.Any, None]:
         """Load found text items from a file.
 
         Args:
             path: The path to the file containing items.
 
         Returns:
             typing.Generator["TextItem", typing.Any, None]: Items from the file.
         """
         logger.debug("Loading OCR output items.")
         count = 0
 
-        with open(path, "rt", encoding="utf8") as file_path:
+        with open(path, encoding="utf8") as file_path:
             reader = csv.DictReader(file_path)
             for row in reader:
                 line_number = row.get("line_number", "").strip()
-                line_number = int(line_number) if line_number != "" else None
+                line_number = int(line_number) if line_number else None
 
                 line_order = row.get("line_order", "").strip()
-                line_order = int(line_order) if line_order != "" else None
+                line_order = int(line_order) if line_order else None
 
                 count += 1
 
                 yield TextItem(
                     text=row["text"],
                     line_number=line_number,
                     line_order=line_order,
@@ -345,16 +358,17 @@
                     bottom_left_y=float(row["bottom_left_y"]),
                 )
 
         logger.debug("Loaded %s OCR items from '%s'.", count, path)
 
     @classmethod
     def from_prediction(
-        cls, prediction: typing.Tuple[typing.Any, typing.Any]
-    ) -> "TextItem":
+        cls,
+        prediction: tuple[typing.Any, typing.Any],
+    ) -> TextItem:
         """Convert from (text, box) to item.
 
         Box is (top left, top right, bottom right, bottom left).
         Its structure is [[startX,startY], [endX,startY], [endX,endY], [startX, endY]].
 
         Args:
             prediction: The text recognised in an image.
@@ -378,33 +392,34 @@
             bottom_right_y=bottom_right_y,
             bottom_left_x=bottom_left_x,
             bottom_left_y=bottom_left_y,
         )
 
     @classmethod
     def order_text_lines(
-        cls, items: typing.List["TextItem"]
-    ) -> typing.List[typing.List["TextItem"]]:
+        cls,
+        items: list[TextItem],
+    ) -> list[list[TextItem]]:
         """Put items into lines of text (top -> bottom, left -> right)."""
         if not items:
             items = []
 
         logger.debug("Arranging text into lines.")
 
         lines = []
-        current_line: typing.List[TextItem] = []
+        current_line: list[TextItem] = []
         for item in items:
             if not item.is_horizontal_level:
                 # exclude items that are too sloped
                 continue
 
             if len(current_line) < 1:
                 current_line.append(item)
 
-            elif any((item.is_same_line(i) for i in current_line)):
+            elif any(item.is_same_line(i) for i in current_line):
                 current_line.append(item)
 
             elif len(current_line) > 0:
                 # store current line
                 current_line = sorted(current_line, key=lambda x: x.top_left)
                 lines.append(current_line)
 
@@ -422,21 +437,21 @@
                 item.line_order = item_index + 1
 
         return lines
 
     @property
     def to_prediction(
         self,
-    ) -> typing.Tuple[
+    ) -> tuple[
         str,
-        typing.Tuple[
-            typing.Tuple[float, float],
-            typing.Tuple[float, float],
-            typing.Tuple[float, float],
-            typing.Tuple[float, float],
+        tuple[
+            tuple[float, float],
+            tuple[float, float],
+            tuple[float, float],
+            tuple[float, float],
         ],
     ]:
         """Convert to prediction format."""
         return (
             self.text,
             (
                 (self.top_left_x, self.top_left_y),
@@ -465,8 +480,8 @@
 @dataclasses.dataclass
 class KerasOcrResult:
     """Result from running keras-ocr."""
 
     output_dir: pathlib.Path
     annotations_file: pathlib.Path
     predictions_file: pathlib.Path
-    items: typing.List[typing.List[TextItem]]
+    items: list[list[TextItem]]
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus/pdf/model.py` & `leaf-focus-0.6.0/src/leaf_focus/pdf/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,242 +11,257 @@
 
 
 @dataclasses.dataclass
 class XpdfArgs:
     """xpdf arguments common to all commands."""
 
     owner_password: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-opw", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-opw", "cmd_type": "single"}},
+        default=None,
     )
     """
     Specify the owner password for the PDF file.
     Providing this will bypass all security restrictions.
 
     -opw <string>          : owner password (for encrypted files)
     """
 
     user_password: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-upw", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-upw", "cmd_type": "single"}},
+        default=None,
     )
     """
     Specify the user password for the PDF file.
 
     -upw <string>          : user password (for encrypted files)
     """
 
     first_page: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-f", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-f", "cmd_type": "single"}},
+        default=None,
     )
     """
     Specifies the first page to convert.
 
     -f <int>               : first page to convert
     """
 
     last_page: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-l", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-l", "cmd_type": "single"}},
+        default=None,
     )
     """
     Specifies the last page to convert.
 
     -l <int>               : last page to convert
     """
 
     use_verbose: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-verbose", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-verbose", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Print a status message (to stdout) before processing each page.
 
     -verbose               : print per-page status information
     """
 
     config_file: typing.Optional[pathlib.Path] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-cfg", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-cfg", "cmd_type": "single"}},
+        default=None,
     )
     """
     Read config-file in place of ~/.xpdfrc or the system-wide config file.
 
     -cfg <string>     : configuration file to use in place of .xpdfrc
     """
 
     program_info: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-v", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-v", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Print copyright and version information.
 
     -v                : print copyright and version info
     """
 
 
 @dataclasses.dataclass
 class XpdfInfoArgs(XpdfArgs):
     """Arguments for xpdf pdfinfo program."""
 
     include_page_bounding_boxes: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-box", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-box", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Prints the page box bounding boxes:
     MediaBox, CropBox, BleedBox, TrimBox, and ArtBox.
 
     -box              : print the page bounding boxes
     """
 
     include_metadata: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-meta", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-meta", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Prints document-level metadata.
-    This is the "Metadata" stream from the PDF file’s Catalog object.
+    This is the "Metadata" stream from the PDF file`s Catalog object.
 
     -meta             : print the document metadata (XML)
     """
 
     include_raw_dates: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-rawdates", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-rawdates", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Prints the raw (undecoded) date strings, directly from the PDF file.
 
     -rawdates         : print the undecoded date strings directly from the PDF file
     """
 
     encoding: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-enc", "cmd_type": "single"}}, default="Latin1"
+        metadata={"leaf_focus": {"cmd": "-enc", "cmd_type": "single"}},
+        default="Latin1",
     )
     """
     Sets the encoding to use for text output.
-    The encoding−name must be defined with the unicodeMap command.
+    The encoding-name must be defined with the unicodeMap command.
     This defaults to "Latin1" (which is a built-in encoding).
 
     -enc <string>          : output text encoding name
     """
 
 
 @dataclasses.dataclass
 class XpdfInfoResult:
     """Result from xpdf pdfinfo program."""
 
     # pdf info
     title: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Title"}}
+        metadata={"leaf_focus": {"name": "Title"}},
     )
     subject: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Subject"}}
+        metadata={"leaf_focus": {"name": "Subject"}},
     )
     keywords: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Keywords"}}
+        metadata={"leaf_focus": {"name": "Keywords"}},
     )
     author: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Author"}}
+        metadata={"leaf_focus": {"name": "Author"}},
     )
     creator: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Creator"}}
+        metadata={"leaf_focus": {"name": "Creator"}},
     )
     producer: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Producer"}}
+        metadata={"leaf_focus": {"name": "Producer"}},
     )
     creation_date: typing.Optional[datetime] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "CreationDate"}}
+        metadata={"leaf_focus": {"name": "CreationDate"}},
     )
     modification_date: typing.Optional[datetime] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "ModDate"}}
+        metadata={"leaf_focus": {"name": "ModDate"}},
     )
 
     # addtional info
     tagged: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Tagged"}}
+        metadata={"leaf_focus": {"name": "Tagged"}},
     )
     form: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Form"}}
+        metadata={"leaf_focus": {"name": "Form"}},
     )
     pages: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Pages"}}
+        metadata={"leaf_focus": {"name": "Pages"}},
     )
     encrypted: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Encrypted"}}
+        metadata={"leaf_focus": {"name": "Encrypted"}},
     )
     page_size: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Page size"}}
+        metadata={"leaf_focus": {"name": "Page size"}},
     )
     media_box: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "MediaBox"}}
+        metadata={"leaf_focus": {"name": "MediaBox"}},
     )
     crop_box: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "CropBox"}}
+        metadata={"leaf_focus": {"name": "CropBox"}},
     )
     bleed_box: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "BleedBox"}}
+        metadata={"leaf_focus": {"name": "BleedBox"}},
     )
     trim_box: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "TrimBox"}}
+        metadata={"leaf_focus": {"name": "TrimBox"}},
     )
     art_box: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "ArtBox"}}
+        metadata={"leaf_focus": {"name": "ArtBox"}},
     )
     file_size_bytes: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "File size"}}
+        metadata={"leaf_focus": {"name": "File size"}},
     )
     optimized: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Optimized"}}
+        metadata={"leaf_focus": {"name": "Optimized"}},
     )
     pdf_version: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "PDF version"}}
+        metadata={"leaf_focus": {"name": "PDF version"}},
     )
 
     # xml metadata
     metadata: typing.Optional[dict] = dataclasses.field(
-        metadata={"leaf_focus": {"name": "Metadata"}}
+        metadata={"leaf_focus": {"name": "Metadata"}},
     )
 
 
 @dataclasses.dataclass
 class XpdfTextArgs(XpdfArgs):
     """Arguments for xpdf pdftotext program."""
 
     use_original_layout: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-layout", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-layout", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Maintain (as best as possible) the original physical layout of the text.
 
     -layout                : maintain original physical layout
     """
 
     use_simple_layout: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-simple", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-simple", "cmd_type": "bool"}},
+        default=False,
     )
     """
     optimized for simple one-column pages.
     This mode will do a better job of maintaining horizontal spacing,
     but it will only work properly with a single column of text.
 
     -simple                : simple one-column page layout
     """
 
     use_simple2_layout: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-simple2", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-simple2", "cmd_type": "bool"}},
+        default=False,
     )
     """
     handles slightly rotated text (e.g., OCR output) better.
     Only works for pages with a single column of text.
 
     -simple2               : simple one-column page layout, version 2
     """
 
     use_table_layout: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-table", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-table", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Table mode is similar to physical layout mode, but optimized for tabular data,
     with the goal of keeping rows and columns aligned
     (at the expense of inserting extra whitespace).
-    If the −fixed option is given, character spacing within
+    If the -fixed option is given, character spacing within
     each line will be determined by the specified character pitch.
 
     -table                 : similar to -layout, but optimized for tables
     """
 
     use_line_printer: typing.Optional[bool] = dataclasses.field(
         metadata={"leaf_focus": {"cmd": "-lineprinter", "cmd_type": "bool"}},
@@ -254,83 +269,90 @@
     )
     """
     Line printer mode uses a strict fixed-character-pitch and -height layout.
     That is, the page is broken into a grid, and characters are placed into that grid.
     If the grid spacing is too small for the actual characters,
     the result is extra whitespace.
     If the grid spacing is too large, the result is missing whitespace.
-    The grid spacing can be specified using the −fixed and −linespacing options.
+    The grid spacing can be specified using the -fixed and -linespacing options.
     If one or both are not given on the command line,
     pdftotext will attempt to compute appropriate value(s).
 
     -lineprinter           : use strict fixed-pitch/height layout
     """
 
     use_raw_string_order: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-raw", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-raw", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Keep the text in content stream order.
     Depending on how the PDF file was generated, this may or may not be useful.
 
     -raw                   : keep strings in content stream order
     """
 
     use_text_clip: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-clip", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-clip", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Text which is hidden because of clipping is removed before doing layout,
     and then added back in. This can be helpful for tables where
     clipped (invisible) text would overlap the next column.
 
     -clip                  : separate clipped text
     """
 
     use_no_diag: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-nodiag", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-nodiag", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Diagonal text, i.e., text that is not close to one of
     the 0, 90, 180, or 270 degree axes, is discarded.
     This is useful to skip watermarks drawn on top of body text, etc.
 
     -nodiag                : discard diagonal text
     """
 
     use_no_page_break: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-nopgbrk", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-nopgbrk", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Don't insert a page break (form feed character) at the
     end of each page.
 
     -nopgbrk               : don't insert a page break at the end of each page
     """
 
     use_bom: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-nom", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-nom", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Insert a Unicode byte order marker (BOM) at the start of the text output.
 
     -bom                   : insert a Unicode BOM at the start of the text file
     """
 
     use_verbose: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-verbose", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-verbose", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Print a status message (to stdout) before processing each page.
 
     -verbose               : print per-page status information
     """
 
     fixed_text_number: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-fixed", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-fixed", "cmd_type": "single"}},
+        default=None,
     )
     """
     Specify the character pitch (character width), in points,
     for physical layout, table, or line printer mode.
     This is ignored in all other modes.
 
     -fixed <number>        : assume fixed-pitch (or tabular) text
@@ -344,60 +366,65 @@
     Specify the line spacing, in points, for line printer mode.
     This is ignored in all other modes.
 
     -linespacing <number>  : fixed line spacing for LinePrinter mode
     """
 
     line_end_type: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-eol", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-eol", "cmd_type": "single"}},
+        default=None,
     )
     """
     Sets the end-of-line convention to use for text output.
 
     -eol <string>          : output end-of-line convention (unix, dos, or mac)
     """
 
     margin_left_number: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-marginl", "cmd_type": "single"}}, default=0
+        metadata={"leaf_focus": {"cmd": "-marginl", "cmd_type": "single"}},
+        default=0,
     )
     """
     Specifies the left margin, in points.
     Text in the left margin
     (i.e., within that many points of the left edge of the page) is discarded.
     The default value is zero.
 
     -marginl <number>      : left page margin
     """
 
     margin_right_number: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-marginr", "cmd_type": "single"}}, default=0
+        metadata={"leaf_focus": {"cmd": "-marginr", "cmd_type": "single"}},
+        default=0,
     )
     """
     Specifies the right margin, in points.
     Text in the right margin (i.e., within that many points of the
     right edge of the page) is discarded.
     The default value is zero.
 
     -marginr <number>      : right page margin
     """
 
     margin_topnumber: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-margint", "cmd_type": "single"}}, default=0
+        metadata={"leaf_focus": {"cmd": "-margint", "cmd_type": "single"}},
+        default=0,
     )
     """
     Specifies the top margin, in points.
     Text in the top margin (i.e., within that many points of the top
     edge of the page) is discarded.
     The default value is zero.
 
     -margint <number>      : top page margin
     """
 
     margin_bottom_number: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-marginb", "cmd_type": "single"}}, default=0
+        metadata={"leaf_focus": {"cmd": "-marginb", "cmd_type": "single"}},
+        default=0,
     )
     """
     Specifies the bottom margin, in points.
     Text in the bottom margin (i.e., within that many points of the
     bottom edge of the page) is discarded.
     The default value is zero.
 
@@ -431,52 +458,57 @@
 
 
 @dataclasses.dataclass
 class XpdfImageArgs(XpdfArgs):
     """Arguments for xpdf pdftopng program."""
 
     resolution: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-r", "cmd_type": "single"}}, default=150
+        metadata={"leaf_focus": {"cmd": "-r", "cmd_type": "single"}},
+        default=150,
     )
     """
     Specifies the resolution, in DPI. The default is 150 DPI.
 
     -r <number>       : resolution, in DPI (default is 150)
     """
     use_monochrome: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-mono", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-mono", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Generate a monochrome image (instead of a color image).
 
     -mono             : generate a monochrome PNG file
     """
 
     use_grayscale: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-gray", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-gray", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Generate a grayscale image (instead of a color image).
 
     -gray             : generate a grayscale PNG file
     """
     use_alpha_channel: typing.Optional[bool] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-alpha", "cmd_type": "bool"}}, default=False
+        metadata={"leaf_focus": {"cmd": "-alpha", "cmd_type": "bool"}},
+        default=False,
     )
     """
     Generate an alpha channel in the PNG file.
     This is only useful with PDF files that have been constructed
     with a transparent background.
-    The −alpha flag cannot be used with −mono.
+    The -alpha flag cannot be used with -mono.
 
     -alpha            : include an alpha channel in the PNG file
     """
 
     rotation: typing.Optional[int] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-rot", "cmd_type": "single"}}, default=None
+        metadata={"leaf_focus": {"cmd": "-rot", "cmd_type": "single"}},
+        default=None,
     )
     """
     Rotate pages by 0 (the default), 90, 180, or 270 degrees.
 
     -rot <int>        : set page rotation: 0, 90, 180, or 270
     """
 
@@ -487,15 +519,16 @@
     """
     Enable or disable FreeType (a TrueType / Type 1 font rasterizer).
     This defaults to "yes".
 
     -freetype <string>: enable FreeType font rasterizer: yes, no
     """
     anti_aliasing: typing.Optional[str] = dataclasses.field(
-        metadata={"leaf_focus": {"cmd": "-aa", "cmd_type": "single"}}, default="yes"
+        metadata={"leaf_focus": {"cmd": "-aa", "cmd_type": "single"}},
+        default="yes",
     )
     """
     Enable or disable font anti-aliasing.
     This defaults to "yes".
 
     -aa <string>      : enable font anti-aliasing: yes, no
     """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus/pdf/xpdf.py` & `leaf-focus-0.6.0/src/leaf_focus/pdf/xpdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Text extraction from pdf using xpdf tools."""
+from __future__ import annotations
 
 import dataclasses
 import json
 import logging
 import pathlib
 import subprocess
 import typing
 from datetime import datetime
+
 from defusedxml import ElementTree
 
 from leaf_focus import utils
 from leaf_focus.pdf import model
 
-
 logger = logging.getLogger(__name__)
 
 
 class XpdfProgram:
     """Interact with xpdf tools."""
 
     OPTS_TEXT_ENCODING = [
@@ -29,15 +30,15 @@
     ]
     OPTS_TEXT_LINE_ENDING = ["unix", "dos", "mac"]
     OPTS_IMAGE_ROTATION = [0, 90, 180, 270]
     OPTS_IMAGE_FREETYPE = ["yes", "no"]
     OPTS_IMAGE_ANTI_ALIAS = ["yes", "no"]
     OPTS_IMAGE_VEC_ANTI_ALIAS = ["yes", "no"]
 
-    def __init__(self, directory: pathlib.Path):
+    def __init__(self, directory: pathlib.Path) -> None:
         """Create a new xpdf program class to interact with xpdf tools.
 
         Args:
             directory: The path to the directory containing xpdf tools.
         """
         self._directory = directory
 
@@ -59,22 +60,22 @@
         """
         # validation
         enc = xpdf_args.encoding
         utils.validate("text encoding", enc, self.OPTS_TEXT_ENCODING)
 
         if not pdf_path.exists():
             msg = f"Pdf file not found '{pdf_path}'."
-            raise utils.LeafFocusException(msg) from FileNotFoundError(pdf_path)
+            raise utils.LeafFocusError(msg) from FileNotFoundError(pdf_path)
 
         output_file = utils.output_root(pdf_path, "info", output_dir)
         output_file = output_file.with_suffix(".json")
 
         if output_file.exists():
             logger.info("Loading existing pdf info file.")
-            with open(output_file, "rt", encoding="utf-8") as info_file:
+            with pathlib.Path.open(output_file, encoding="utf-8") as info_file:
                 return model.XpdfInfoResult(**json.load(info_file))
 
         logger.info("Extracting pdf info and saving to file.")
 
         # build command
         exe_path = utils.select_exe(self._directory / "pdfinfo")
         cmd = [str(exe_path)]
@@ -82,25 +83,29 @@
         cmd_args = self.build_cmd(xpdf_args)
 
         cmd.extend(cmd_args)
         cmd.append(str(pdf_path.resolve()))
 
         # execute program
         result = subprocess.run(
-            cmd, capture_output=True, check=True, timeout=30, text=True
+            cmd,
+            capture_output=True,
+            check=True,
+            timeout=30,
+            text=True,
         )
         lines = result.stdout.splitlines()
 
         fields_map = {
             field.metadata.get("leaf_focus", {}).get("name"): field
             for field in dataclasses.fields(model.XpdfInfoResult)
         }
-        metadata_line_index: typing.Optional[int] = None
+        metadata_line_index: int | None = None
 
-        data: typing.Dict[str, typing.Any] = {i.name: None for i in fields_map.values()}
+        data: dict[str, typing.Any] = {i.name: None for i in fields_map.values()}
         for index, line in enumerate(lines):
             if line.startswith("Metadata:"):
                 metadata_line_index = index
                 break
 
             value: typing.Any = None
             key, value = line.split(":", maxsplit=1)
@@ -135,15 +140,15 @@
             metadata = "\n".join(lines[start:])
             root = ElementTree.fromstring(metadata)
             data["metadata"] = utils.xml_to_element(root).to_dict()
 
         if output_dir and output_dir.exists():
             logger.debug("Saving pdf info to '%s'.", output_file)
             output_file.write_text(
-                json.dumps(data, indent=2, cls=utils.CustomJsonEncoder)
+                json.dumps(data, indent=2, cls=utils.CustomJsonEncoder),
             )
 
         return model.XpdfInfoResult(**data)
 
     def text(
         self,
         pdf_path: pathlib.Path,
@@ -162,15 +167,15 @@
         """
         # validation
         eol = xpdf_args.line_end_type
         utils.validate("end of line", eol, self.OPTS_TEXT_LINE_ENDING)
 
         if not pdf_path.exists():
             msg = f"Pdf file not found '{pdf_path}'."
-            raise utils.LeafFocusException(msg) from FileNotFoundError(str(pdf_path))
+            raise utils.LeafFocusError(msg) from FileNotFoundError(str(pdf_path))
 
         # build command
 
         cmd_args = self.build_cmd(xpdf_args)
 
         output_file = utils.output_root(pdf_path, "output", output_path, cmd_args)
         output_file = output_file.with_suffix(".txt")
@@ -195,15 +200,15 @@
 
         logger.info("Extracting pdf embedded text and saving to file.")
 
         exe_path = utils.select_exe(self._directory / "pdftotext")
 
         cmd = [str(exe_path)]
 
-        cmd.extend(cmd_args + [str(pdf_path), str(output_file)])
+        cmd.extend([*cmd_args, str(pdf_path), str(output_file)])
 
         # execute program
         result = subprocess.run(
             cmd,
             capture_output=True,
             check=True,
             timeout=30,
@@ -242,51 +247,59 @@
         utils.validate("freetype", free_type, self.OPTS_IMAGE_FREETYPE)
 
         anti_alias = xpdf_args.anti_aliasing
         utils.validate("anti-aliasing", anti_alias, self.OPTS_IMAGE_ANTI_ALIAS)
 
         anti_alias_vec = xpdf_args.anti_aliasing
         utils.validate(
-            "vector anti-aliasing", anti_alias_vec, self.OPTS_IMAGE_VEC_ANTI_ALIAS
+            "vector anti-aliasing",
+            anti_alias_vec,
+            self.OPTS_IMAGE_VEC_ANTI_ALIAS,
         )
 
         if not pdf_path.exists():
             msg = f"Pdf file not found '{pdf_path}'."
-            raise utils.LeafFocusException(msg) from FileNotFoundError(str(pdf_path))
+            raise utils.LeafFocusError(msg) from FileNotFoundError(str(pdf_path))
 
         logger.info("Saving each pdf page as an image.")
 
         # build command
         cmd_args = self.build_cmd(xpdf_args)
 
         output_type = "page-image"
 
         # don't include the page limits when building the output prefix
         xpdf_args.first_page = None
         xpdf_args.last_page = None
         output_cmd_args = self.build_cmd(xpdf_args)
         output_dir = utils.output_root(
-            pdf_path, output_type, output_path, output_cmd_args
+            pdf_path,
+            output_type,
+            output_path,
+            output_cmd_args,
         )
 
         for pdf_image_file in output_dir.parent.iterdir():
             if not pdf_image_file.name.startswith(output_dir.name):
                 continue
 
             logger.info("Found existing pdf images.")
 
             output_files = self.find_images(output_dir)
             return model.XpdfImageResult(
-                stdout=[], stderr=[], output_dir=output_dir, output_files=output_files
+                stdout=[],
+                stderr=[],
+                output_dir=output_dir,
+                output_files=output_files,
             )
 
         exe_path = utils.select_exe(self._directory / "pdftopng")
         cmd = [str(exe_path)]
 
-        cmd.extend(cmd_args + [str(pdf_path), str(output_dir)])
+        cmd.extend([*cmd_args, str(pdf_path), str(output_dir)])
 
         # execute program
         result = subprocess.run(
             cmd,
             capture_output=True,
             check=True,
             timeout=30,
@@ -311,69 +324,67 @@
         for field in dataclasses.fields(arg_class):
             name = field.name
             value = getattr(tool_args, name)
 
             field_default = field.default
 
             # TODO: account for default_factory
-            # field_default_factory = field.default_factory
 
             # validate the arg config
             cmd_key = field.metadata.get("leaf_focus", {}).get("cmd")
             if not cmd_key:
-                raise ValueError(
-                    f"Args incorrectly configured: missing 'cmd' for '{name}'."
-                )
+                msg = f"Args incorrectly configured: missing 'cmd' for '{name}'."
+                raise ValueError(msg)
 
             cmd_type = field.metadata.get("leaf_focus", {}).get("cmd_type")
             if not cmd_type:
-                raise ValueError(
-                    f"Args incorrectly configured: missing 'cmd_type' for '{name}'."
-                )
+                msg = f"Args incorrectly configured: missing 'cmd_type' for '{name}'."
+                raise ValueError(msg)
 
             # add the arg
             if cmd_type == "bool":
                 if value is not None and value is not True and value is not False:
-                    raise ValueError(
-                        f"Argument '{name}' must be None, True, or False, "
-                        f"not '{value}'."
-                    )
+                    msg = f"Argument '{name}' must be None, True, or False, not '{value}'."
+                    raise ValueError(msg)
 
                 if value is True:
                     cmd_args.extend([str(cmd_key)])
 
             elif cmd_type == "single":
                 if field_default is None and value is not None:
                     cmd_args.extend([str(cmd_key), str(value)])
                 elif field_default != value:
                     cmd_args.extend([str(cmd_key), str(value)])
 
             else:
-                raise ValueError(
+                msg = (
                     f"Argument '{name}' has unknown cmd_type '{cmd_type}'. "
-                    f"Expected one of 'bool, single'."
+                    "Expected one of 'bool, single'."
                 )
+                raise ValueError(msg)
 
         return cmd_args
 
-    def find_images(self, output_dir: pathlib.Path):
+    def find_images(self, output_dir: pathlib.Path) -> list[pathlib.Path]:
         """Find image files in a directory."""
+        stem_parts = 7
+        stem_digit_parts = 6
         output_files = []
         for file_path in output_dir.parent.iterdir():
             if not file_path.is_file():
                 continue
             if not file_path.name.startswith(output_dir.stem):
                 continue
             if file_path.suffix != ".png":
                 continue
-            if len(file_path.stem) < 7:
+            if len(file_path.stem) < stem_parts:
                 continue
-            if file_path.stem[-7] != "-":
+            if file_path.stem[-stem_parts] != "-":
                 continue
-            if not all(i.isdigit() for i in file_path.stem[-6:]):
+            if not all(i.isdigit() for i in file_path.stem[-stem_digit_parts:]):
                 continue
             output_files.append(file_path)
 
         if not output_files:
             logger.warning("No page images found.")
 
         return output_files
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus/utils.py` & `leaf-focus-0.6.0/src/leaf_focus/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """Small utility functions."""
+from __future__ import annotations
+
 import dataclasses
+import datetime
 import json
-import pathlib
 import platform
 import re
 import typing
-import datetime
-
-from xml.etree.ElementTree import Element
 import unicodedata
+from enum import Enum
 
-from importlib_metadata import distribution, PackageNotFoundError
+if typing.TYPE_CHECKING:
+    import pathlib
+    from xml.etree.ElementTree import Element
+
+from importlib_metadata import PackageNotFoundError, distribution
 from importlib_resources import as_file, files
 
 
 def get_name_dash() -> str:
     """Get the package name with word separated by dashes."""
     return "leaf-focus"
 
 
 def get_name_under() -> str:
     """Get the package name with word separated by underscores."""
     return "leaf_focus"
 
 
-def get_version() -> typing.Optional[str]:
+def get_version() -> str | None:
     """Get the package version."""
     try:
         dist = distribution(get_name_dash())
         return dist.version
     except PackageNotFoundError:
         pass
 
@@ -37,70 +41,80 @@
             return (file_path.parent.parent.parent / "VERSION").read_text().strip()
     except FileNotFoundError:
         pass
 
     return None
 
 
-def parse_date(value: str) -> typing.Optional[datetime.datetime]:
+def parse_date(value: str) -> datetime.datetime | None:
     """Parse a date from a string."""
     formats = [
         # e.g. 'Thu Aug 13 11:09:00 2020'
         "%a %b %d %H:%M:%S %Y",
     ]
     for fmt in formats:
         try:
             return datetime.datetime.strptime(value, fmt)
         except ValueError:
             pass
     return None
 
 
-def validate(name: str, value, expected: typing.List) -> None:
+def validate(name: str, value, expected: list) -> None:
     """Validate that a value is one of the expected values."""
     if value is not None and value not in expected:
         opts = ", ".join(sorted([str(i) for i in expected]))
-        raise LeafFocusException(f"Invalid {name} '{value}'. Expected one of '{opts}'.")
+        msg = f"Invalid {name} '{value}'. Expected one of '{opts}'."
+        raise LeafFocusError(msg)
+
+
+class ValidatePathMethod(Enum):
+    NO_OPINION = 0
+    MUST_EXIST = 1
 
 
 def validate_path(
-    name: str, value: pathlib.Path, must_exist: bool = False
+    name: str,
+    value: pathlib.Path,
+    must_exist: ValidatePathMethod = ValidatePathMethod.NO_OPINION,
 ) -> pathlib.Path:
     """Validate a path."""
     if not value:
-        raise LeafFocusException(f"Must provide path {name}.")
+        msg = f"Must provide path {name}."
+        raise LeafFocusError(msg)
 
     try:
-        if must_exist is True:
+        if must_exist == ValidatePathMethod.MUST_EXIST:
             abs_path = value.resolve(strict=True)
         else:
             abs_path = value.absolute()
 
         return abs_path
     except Exception as error:
-        raise LeafFocusException(f"Invalid path '{value}'.") from error
+        msg = f"Invalid path '{value}'."
+        raise LeafFocusError(msg) from error
 
 
 def select_exe(value: pathlib.Path) -> pathlib.Path:
     """Select the executable path based on the platform."""
     if platform.system() == "Windows":
         value = value.with_suffix(".exe")
 
     if not value.exists():
         msg = f"Exe file not found '{value}'."
-        raise LeafFocusException(msg) from FileNotFoundError(value)
+        raise LeafFocusError(msg) from FileNotFoundError(value)
 
     return value
 
 
 def output_root(
     input_file: pathlib.Path,
     output_type: str,
     output_path: pathlib.Path,
-    additional: typing.Optional[typing.Collection[str]] = None,
+    additional: typing.Collection[str] | None = None,
 ) -> pathlib.Path:
     """Build the path to the output."""
     name_parts = [input_file.stem, output_type]
     name_parts.extend(additional or [])
     name_parts = [str(i) for i in name_parts if i is not None]
     name_parts = [str_norm(i.strip("-")) for i in name_parts if i and i.strip()]
 
@@ -111,15 +125,15 @@
     return output
 
 
 _slug_re_1 = re.compile(r"[^\w\s-]")
 _slug_re_2 = re.compile(r"[-\s]+")
 
 
-def str_norm(value: str):
+def str_norm(value: str) -> str:
     """Normalise a string into the 'slug' format."""
     separator = "-"
     encoding = "utf-8"
 
     norm = unicodedata.normalize("NFKD", value)
     enc = norm.encode(encoding, "ignore")
     de_enc = enc.decode(encoding)
@@ -131,39 +145,39 @@
 
 # 45206-win10-win8-win7-release-notes-page-image-gray-000022.png
 
 
 class CustomJsonEncoder(json.JSONEncoder):
     """A custom json encoder."""
 
-    def default(self, o):
+    def default(self, o: typing.Any) -> typing.Any:
         """Conversion used by default."""
         if isinstance(o, (datetime.datetime, datetime.date, datetime.time)):
             return o.isoformat()
 
         return super().default(o)
 
 
 @dataclasses.dataclass
 class XmlElement:
     """A simple xml element.
 
     <tag attrib>text<child/>...</tag>tail
     """
 
-    attrib: typing.Collection[typing.Tuple[str, str, str]]
+    attrib: typing.Collection[tuple[str, str, str]]
     tag: str
     name_space: str
     text: str
     tail: str
-    children: typing.Collection["XmlElement"]
+    children: typing.Collection[XmlElement]
 
-    def to_dict(self) -> typing.Dict:
+    def to_dict(self) -> dict:
         """Convert xml element to a dict."""
-        result: typing.Dict[str, typing.Any] = {"name": self.tag.strip()}
+        result: dict[str, typing.Any] = {"name": self.tag.strip()}
 
         value = ((self.text or "").strip() + " " + (self.tail or "").strip()).strip()
         if value:
             result["value"] = value
 
         attributes = {k.strip(): (v or "").strip() for n, k, v, in self.attrib}
         if attributes:
@@ -171,15 +185,15 @@
 
         children = [i.to_dict() for i in self.children]
         if children:
             result["children"] = children
 
         return result
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Convert to a string."""
         tag1 = (self.tag or "").strip()
         tag2 = f"</{tag1}>"
         text = (self.text or "").strip()
         tail = (self.tail or "").strip()
 
         count = len(self.children)
@@ -233,15 +247,15 @@
         tail=tail or "",
         children=children,
     )
 
     return item
 
 
-def xml_tag_ns(value: str) -> typing.Tuple[str, str]:
+def xml_tag_ns(value: str) -> tuple[str, str]:
     """Get the XML namespace and name.
 
     Args:
         value: The combined namespace and name
 
     Returns:
         The separate namespace and name
@@ -252,9 +266,9 @@
     else:
         name_space = ""
         name = value
 
     return name_space, name
 
 
-class LeafFocusException(Exception):
-    """A custom error."""
+class LeafFocusError(Exception):
+    """A custom error for leaf focus."""
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus.egg-info/PKG-INFO` & `leaf-focus-0.6.0/src/leaf_focus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaf-focus
-Version: 0.5.3
+Version: 0.6.0
 Summary: Extract structured text from pdf files.
 Project-URL: Homepage, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Changelog, https://github.com/anotherbyte-net/leaf-focus/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/anotherbyte-net/leaf-focus
 Project-URL: Tracker, https://github.com/anotherbyte-net/leaf-focus/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `leaf-focus-0.5.3/src/leaf_focus.egg-info/SOURCES.txt` & `leaf-focus-0.6.0/src/leaf_focus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.5.3/tests/test_cli.py` & `leaf-focus-0.6.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.5.3/tests/test_keras_ocr.py` & `leaf-focus-0.6.0/tests/test_keras_ocr.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     output_path = tmp_path / "output-dir"
     output_path.mkdir(exist_ok=True, parents=True)
 
     prog = OpticalCharacterRecognition()
 
     if sys.version_info.major == 3 and sys.version_info.minor > keras_max_version_minor:
         with pytest.raises(
-            utils.LeafFocusException, match="Cannot run ocr on this Python version."
+            utils.LeafFocusError, match="Cannot run ocr on this Python version."
         ):
             prog.recognise_text(image_file, output_path)
 
     else:
         result = prog.recognise_text(image_file, output_path)
         expected_lines = 33
         expected_items = 300
@@ -78,15 +78,15 @@
     output_path = tmp_path / "output-dir"
     output_path.mkdir(exist_ok=True, parents=True)
 
     prog = OpticalCharacterRecognition()
 
     if sys.version_info.major == 3 and sys.version_info.minor > keras_max_version_minor:
         with pytest.raises(
-            utils.LeafFocusException, match="Cannot run ocr on this Python version."
+            utils.LeafFocusError, match="Cannot run ocr on this Python version."
         ):
             prog.recognise_text(image_file, output_path)
 
     else:
 
         def mock_engine_create():
             pass
@@ -199,14 +199,23 @@
 
 
 @given(
     items=st.one_of(
         st.lists(
             st.builds(
                 TextItem,
+                text=st.text(),
+                top_left_x=st.floats(),
+                top_left_y=st.floats(),
+                top_right_x=st.floats(),
+                top_right_y=st.floats(),
+                bottom_right_x=st.floats(),
+                bottom_right_y=st.floats(),
+                bottom_left_x=st.floats(),
+                bottom_left_y=st.floats(),
                 line_number=st.one_of(st.none(), st.one_of(st.none(), st.integers())),
                 line_order=st.one_of(st.none(), st.one_of(st.none(), st.integers())),
             )
         )
     )
 )
 def test_fuzz_TextItem_order_text_lines(items):
```

### Comparing `leaf-focus-0.5.3/tests/test_utils.py` & `leaf-focus-0.6.0/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     value_str = value.strftime("%a %b %d %H:%M:%S %Y")
 #     assert utils.parse_date(value=value_str)
 
 
 @given(name=st.text(), value=st.text(), expected=st.builds(list))
 def test_fuzz_validate(name, value, expected):
     if value not in expected:
-        with pytest.raises(utils.LeafFocusException):
+        with pytest.raises(utils.LeafFocusError):
             utils.validate(name=name, value=value, expected=expected)
     else:
         utils.validate(name=name, value=value, expected=expected)
 
 
 @given(name=st.text(), value=st.builds(pathlib.Path), must_exist=st.booleans())
 def test_fuzz_validate_path(name, value, must_exist):
```

### Comparing `leaf-focus-0.5.3/tests/test_xpdf_image.py` & `leaf-focus-0.6.0/tests/test_xpdf_image.py`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.5.3/tests/test_xpdf_info.py` & `leaf-focus-0.6.0/tests/test_xpdf_info.py`

 * *Files identical despite different names*

### Comparing `leaf-focus-0.5.3/tests/test_xpdf_text.py` & `leaf-focus-0.6.0/tests/test_xpdf_text.py`

 * *Files identical despite different names*

