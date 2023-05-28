# Comparing `tmp/hello2-1.7.6.tar.gz` & `tmp/hello2-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello2-1.7.6.tar", last modified: Sun May 28 04:38:17 2023, max compression
+gzip compressed data, was "hello2-1.7.7.tar", last modified: Sun May 28 05:35:45 2023, max compression
```

## Comparing `hello2-1.7.6.tar` & `hello2-1.7.7.tar`

### file list

```diff
@@ -1,193 +1,194 @@
--rw-r--r--   0        0        0      550 2023-05-27 08:01:43.939155 hello2-1.7.6/.gitignore
--rw-r--r--   0        0        0      715 2023-05-27 08:01:43.939155 hello2-1.7.6/.readthedocs.yaml
--rw-r--r--   0        0        0    11357 2023-05-27 08:01:43.939155 hello2-1.7.6/LICENSE
--rw-r--r--   0        0        0      351 2023-05-27 08:01:43.939155 hello2-1.7.6/README.md
--rw-r--r--   0        0        0      638 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/Makefile
--rw-r--r--   0        0        0      804 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/make.bat
--rw-r--r--   0        0        0      163 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/_templates/.gitkeep
--rw-r--r--   0        0        0     1365 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/conf.py
--rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.data.coco2yolo.rst
--rw-r--r--   0        0        0      231 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.data.rst
--rw-r--r--   0        0        0      187 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.experimental.albu.detection.rst
--rw-r--r--   0        0        0      283 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.experimental.albu.rst
--rw-r--r--   0        0        0      260 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.experimental.rst
--rw-r--r--   0        0        0      157 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.annotate.rst
--rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.brain.rst
--rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.coco.rst
--rw-r--r--   0        0        0      160 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.connected.rst
--rw-r--r--   0        0        0      160 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.copypaste.rst
--rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.core.rst
--rw-r--r--   0        0        0      154 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.dataset.rst
--rw-r--r--   0        0        0      183 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.dataset_annotate.rst
--rw-r--r--   0        0        0      189 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.dataset_detections.rst
--rw-r--r--   0        0        0      198 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.dataset_segmentations.rst
--rw-r--r--   0        0        0      177 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.dataset_yolov5.rst
--rw-r--r--   0        0        0      168 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.dataset_zoo.rst
--rw-r--r--   0        0        0      157 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.evaluate.rst
--rw-r--r--   0        0        0      192 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.evaluate_detections.rst
--rw-r--r--   0        0        0      201 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.evaluate_segmentations.rst
--rw-r--r--   0        0        0      171 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.gen_examples.rst
--rw-r--r--   0        0        0      168 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.mask_ignore.rst
--rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.miou.rst
--rw-r--r--   0        0        0      154 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.patches.rst
--rw-r--r--   0        0        0      876 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.rst
--rw-r--r--   0        0        0      154 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.tarinfo.rst
--rw-r--r--   0        0        0      151 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.unique.rst
--rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.utils.rst
--rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.video.rst
--rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fiftyone.view.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fvcore.core.rst
--rw-r--r--   0        0        0      234 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.fvcore.rst
--rw-r--r--   0        0        0      130 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.io.image.rst
--rw-r--r--   0        0        0      237 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.io.rst
--rw-r--r--   0        0        0      130 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.io.utils.rst
--rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmdet.export.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmdet.flop.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmdet.infer.rst
--rw-r--r--   0        0        0      133 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmdet.log.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmdet.plot.rst
--rw-r--r--   0        0        0      312 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmdet.rst
--rw-r--r--   0        0        0      142 2023-05-27 13:26:40.942344 hello2-1.7.6/docs/source/hello.mmlab.mmdet3.rst
--rw-r--r--   0        0        0      139 2023-05-27 13:26:40.942344 hello2-1.7.6/docs/source/hello.mmlab.mmseg.rst
--rw-r--r--   0        0        0      253 2023-05-27 13:26:40.932344 hello2-1.7.6/docs/source/hello.mmlab.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmseg.infer.rst
--rw-r--r--   0        0        0      133 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmseg.log.rst
--rw-r--r--   0        0        0      130 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmseg.lr.rst
--rw-r--r--   0        0        0      268 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.mmseg.rst
--rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.nanodet.infer.rst
--rw-r--r--   0        0        0      239 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.nanodet.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.onnx.export.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.onnx.infer.rst
--rw-r--r--   0        0        0      248 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.onnx.rst
--rw-r--r--   0        0        0      415 2023-05-27 13:26:40.702344 hello2-1.7.6/docs/source/hello.rst
--rw-r--r--   0        0        0      256 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.transforms.rst
--rw-r--r--   0        0        0      169 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.transforms.transforms.rst
--rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.utils.colors.rst
--rw-r--r--   0        0        0      145 2023-05-27 13:26:41.052344 hello2-1.7.6/docs/source/hello.utils.compare.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.utils.cuda.rst
--rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.utils.importer.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.utils.plots.rst
--rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.utils.points.rst
--rw-r--r--   0        0        0      365 2023-05-27 13:26:41.032344 hello2-1.7.6/docs/source/hello.utils.rst
--rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.utils.strtime.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.align.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.clip.rst
--rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.fisheye.rst
--rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.frames.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.info.rst
--rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.resize.rst
--rw-r--r--   0        0        0      425 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.rtsp.rst
--rw-r--r--   0        0        0      153 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.rtsp_pull.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.split.rst
--rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.unwarp.rst
--rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.video.utils.rst
--rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.x3m.config.rst
--rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.x3m.preprocess.rst
--rw-r--r--   0        0        0      272 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.x3m.rst
--rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/hello.x3m.transforms.rst
--rw-r--r--   0        0        0      572 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/index.rst
--rw-r--r--   0        0        0       52 2023-05-27 08:01:43.939155 hello2-1.7.6/docs/source/modules.rst
--rw-r--r--   0        0        0     3270 2023-05-27 13:33:10.962343 hello2-1.7.6/hello/README.md
--rw-r--r--   0        0        0      773 2023-05-28 04:29:03.092349 hello2-1.7.6/hello/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/__main__.py
--rw-r--r--   0        0        0      471 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/data/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/data/__main__.py
--rw-r--r--   0        0        0     3426 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/data/coco2yolo.py
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/experimental/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/experimental/albu/__init__.py
--rw-r--r--   0        0        0      111 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/experimental/albu/detection.py
--rw-r--r--   0        0        0     1047 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/fiftyone/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/fiftyone/__main__.py
--rw-r--r--   0        0        0     4781 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/fiftyone/annotate.py
--rw-r--r--   0        0        0    10578 2023-05-27 13:22:52.332349 hello2-1.7.6/hello/fiftyone/brain.py
--rw-r--r--   0        0        0    10777 2023-05-28 04:27:24.712346 hello2-1.7.6/hello/fiftyone/coco.py
--rw-r--r--   0        0        0      912 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/fiftyone/connected.py
--rw-r--r--   0        0        0       36 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/fiftyone/copypaste.py
--rw-r--r--   0        0        0    18009 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/fiftyone/core.py
--rw-r--r--   0        0        0    21443 2023-05-28 02:11:35.582349 hello2-1.7.6/hello/fiftyone/dataset.py
--rw-r--r--   0        0        0     7502 2023-05-27 08:01:43.939155 hello2-1.7.6/hello/fiftyone/dataset_detections.py
--rw-r--r--   0        0        0     5693 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/dataset_segmentations.py
--rw-r--r--   0        0        0     1402 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/dataset_yolov5.py
--rw-r--r--   0        0        0      889 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/dataset_zoo.py
--rw-r--r--   0        0        0     1169 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/evaluate.py
--rw-r--r--   0        0        0     5157 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/evaluate_detections.py
--rw-r--r--   0        0        0     4544 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/evaluate_segmentations.py
--rw-r--r--   0        0        0      103 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/examples/README.md
--rw-r--r--   0        0        0     2975 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/examples/examples.py
--rw-r--r--   0        0        0    12021 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/examples/utils.py
--rw-r--r--   0        0        0     3241 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/gen_examples.py
--rw-r--r--   0        0        0     1608 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/mask_ignore.py
--rw-r--r--   0        0        0     5683 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/miou.py
--rw-r--r--   0        0        0     2639 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/patches.py
--rw-r--r--   0        0        0     9325 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/tarinfo.py
--rw-r--r--   0        0        0     4094 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/unique.py
--rw-r--r--   0        0        0     8414 2023-05-28 03:56:14.622347 hello2-1.7.6/hello/fiftyone/utils.py
--rw-r--r--   0        0        0      781 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fiftyone/video.py
--rw-r--r--   0        0        0     8268 2023-05-27 09:29:48.362349 hello2-1.7.6/hello/fiftyone/view.py
--rw-r--r--   0        0        0      435 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fvcore/README.md
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fvcore/__init__.py
--rw-r--r--   0        0        0     1080 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/fvcore/core.py
--rw-r--r--   0        0        0      135 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/io/__init__.py
--rw-r--r--   0        0        0     1382 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/io/image.py
--rw-r--r--   0        0        0      989 2023-05-27 23:53:07.192349 hello2-1.7.6/hello/io/utils.py
--rw-r--r--   0        0        0      851 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmdet/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmdet/__main__.py
--rw-r--r--   0        0        0       97 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmdet/export.py
--rw-r--r--   0        0        0     1736 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmdet/flop.py
--rw-r--r--   0        0        0     5446 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmdet/infer.py
--rw-r--r--   0        0        0     3273 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmdet/log.py
--rw-r--r--   0        0        0     5976 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmdet/plot.py
--rw-r--r--   0        0        0      563 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmlab/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmlab/__main__.py
--rw-r--r--   0        0        0      110 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmlab/mmdet3.py
--rw-r--r--   0        0        0     6549 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmlab/mmseg.py
--rw-r--r--   0        0        0      645 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmseg/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmseg/__main__.py
--rw-r--r--   0        0        0     6040 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmseg/infer.py
--rw-r--r--   0        0        0     2368 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmseg/log.py
--rw-r--r--   0        0        0     7006 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/mmseg/lr.py
--rw-r--r--   0        0        0      462 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/nanodet/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/nanodet/__main__.py
--rw-r--r--   0        0        0     7410 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/nanodet/infer.py
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/onnx/__init__.py
--rw-r--r--   0        0        0      213 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/onnx/examples/README.md
--rw-r--r--   0        0        0     1879 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/onnx/examples/test_sigmoid.py
--rw-r--r--   0        0        0     3024 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/onnx/export.py
--rw-r--r--   0        0        0     1707 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/onnx/infer.py
--rw-r--r--   0        0        0     1334 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/transforms/README.md
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/transforms/__init__.py
--rw-r--r--   0        0        0     2655 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/transforms/transforms.py
--rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/__init__.py
--rw-r--r--   0        0        0     2133 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/colors.py
--rw-r--r--   0        0        0      976 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/compare.py
--rw-r--r--   0        0        0     1815 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/cuda.py
--rw-r--r--   0        0        0      356 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/importer.py
--rw-r--r--   0        0        0      612 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/plots.py
--rw-r--r--   0        0        0     2999 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/points.py
--rw-r--r--   0        0        0      195 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/utils/strtime.py
--rw-r--r--   0        0        0     1135 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/__main__.py
--rw-r--r--   0        0        0     3428 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/align.py
--rw-r--r--   0        0        0     6382 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/clip.py
--rw-r--r--   0        0        0     3290 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/fisheye.py
--rw-r--r--   0        0        0     1565 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/info.py
--rw-r--r--   0        0        0     3502 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/resize.py
--rw-r--r--   0        0        0     4716 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/rtsp.py
--rw-r--r--   0        0        0     5006 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/rtsp_pull.py
--rw-r--r--   0        0        0     3048 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/split.py
--rw-r--r--   0        0        0     4066 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/unwarp.py
--rw-r--r--   0        0        0      968 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/video/utils.py
--rw-r--r--   0        0        0      576 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/x3m/__init__.py
--rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/x3m/__main__.py
--rw-r--r--   0        0        0     4479 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/x3m/config.py
--rw-r--r--   0        0        0     2592 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/x3m/preprocess.py
--rw-r--r--   0        0        0     6928 2023-05-27 08:01:43.949155 hello2-1.7.6/hello/x3m/transforms.py
--rw-r--r--   0        0        0      808 2023-05-27 08:01:43.949155 hello2-1.7.6/hello_c/CMakeLists.txt
--rw-r--r--   0        0        0      776 2023-05-27 08:01:43.949155 hello2-1.7.6/hello_c/README.md
--rw-r--r--   0        0        0     1375 2023-05-27 08:01:43.949155 hello2-1.7.6/hello_c/main.cpp
--rw-r--r--   0        0        0      262 2023-05-27 08:01:43.949155 hello2-1.7.6/hello_c/trace_model.py
--rw-r--r--   0        0        0      787 2023-05-27 08:01:43.949155 hello2-1.7.6/pyproject.toml
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-05-27 08:01:43.939155 hello2-1.7.7/.gitignore
+-rw-r--r--   0        0        0      715 2023-05-27 08:01:43.939155 hello2-1.7.7/.readthedocs.yaml
+-rw-r--r--   0        0        0    11357 2023-05-27 08:01:43.939155 hello2-1.7.7/LICENSE
+-rw-r--r--   0        0        0      351 2023-05-27 08:01:43.939155 hello2-1.7.7/README.md
+-rw-r--r--   0        0        0      638 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/make.bat
+-rw-r--r--   0        0        0      163 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/_templates/.gitkeep
+-rw-r--r--   0        0        0     1365 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/conf.py
+-rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.data.coco2yolo.rst
+-rw-r--r--   0        0        0      231 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.data.rst
+-rw-r--r--   0        0        0      187 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.experimental.albu.detection.rst
+-rw-r--r--   0        0        0      283 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.experimental.albu.rst
+-rw-r--r--   0        0        0      260 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.experimental.rst
+-rw-r--r--   0        0        0      157 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.annotate.rst
+-rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.brain.rst
+-rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.coco.rst
+-rw-r--r--   0        0        0      160 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.connected.rst
+-rw-r--r--   0        0        0      160 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.copypaste.rst
+-rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.core.rst
+-rw-r--r--   0        0        0      154 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.dataset.rst
+-rw-r--r--   0        0        0      183 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.dataset_annotate.rst
+-rw-r--r--   0        0        0      189 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.dataset_detections.rst
+-rw-r--r--   0        0        0      198 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.dataset_segmentations.rst
+-rw-r--r--   0        0        0      177 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.dataset_yolov5.rst
+-rw-r--r--   0        0        0      168 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.dataset_zoo.rst
+-rw-r--r--   0        0        0      157 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.evaluate.rst
+-rw-r--r--   0        0        0      192 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.evaluate_detections.rst
+-rw-r--r--   0        0        0      201 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.evaluate_segmentations.rst
+-rw-r--r--   0        0        0      171 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.gen_examples.rst
+-rw-r--r--   0        0        0      168 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.mask_ignore.rst
+-rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.miou.rst
+-rw-r--r--   0        0        0      154 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.patches.rst
+-rw-r--r--   0        0        0      876 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.rst
+-rw-r--r--   0        0        0      154 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.tarinfo.rst
+-rw-r--r--   0        0        0      151 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.unique.rst
+-rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.utils.rst
+-rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.video.rst
+-rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fiftyone.view.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fvcore.core.rst
+-rw-r--r--   0        0        0      234 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.fvcore.rst
+-rw-r--r--   0        0        0      130 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.io.image.rst
+-rw-r--r--   0        0        0      237 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.io.rst
+-rw-r--r--   0        0        0      130 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.io.utils.rst
+-rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmdet.export.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmdet.flop.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmdet.infer.rst
+-rw-r--r--   0        0        0      133 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmdet.log.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmdet.plot.rst
+-rw-r--r--   0        0        0      312 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmdet.rst
+-rw-r--r--   0        0        0      142 2023-05-27 13:26:40.942344 hello2-1.7.7/docs/source/hello.mmlab.mmdet3.rst
+-rw-r--r--   0        0        0      139 2023-05-27 13:26:40.942344 hello2-1.7.7/docs/source/hello.mmlab.mmseg.rst
+-rw-r--r--   0        0        0      253 2023-05-27 13:26:40.932344 hello2-1.7.7/docs/source/hello.mmlab.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmseg.infer.rst
+-rw-r--r--   0        0        0      133 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmseg.log.rst
+-rw-r--r--   0        0        0      130 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmseg.lr.rst
+-rw-r--r--   0        0        0      268 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.mmseg.rst
+-rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.nanodet.infer.rst
+-rw-r--r--   0        0        0      239 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.nanodet.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.onnx.export.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.onnx.infer.rst
+-rw-r--r--   0        0        0      248 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.onnx.rst
+-rw-r--r--   0        0        0      415 2023-05-27 13:26:40.702344 hello2-1.7.7/docs/source/hello.rst
+-rw-r--r--   0        0        0      256 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.transforms.rst
+-rw-r--r--   0        0        0      169 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.transforms.transforms.rst
+-rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.utils.colors.rst
+-rw-r--r--   0        0        0      145 2023-05-27 13:26:41.052344 hello2-1.7.7/docs/source/hello.utils.compare.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.utils.cuda.rst
+-rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.utils.importer.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.utils.plots.rst
+-rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.utils.points.rst
+-rw-r--r--   0        0        0      365 2023-05-27 13:26:41.032344 hello2-1.7.7/docs/source/hello.utils.rst
+-rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.utils.strtime.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.align.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.clip.rst
+-rw-r--r--   0        0        0      145 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.fisheye.rst
+-rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.frames.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.info.rst
+-rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.resize.rst
+-rw-r--r--   0        0        0      425 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.rtsp.rst
+-rw-r--r--   0        0        0      153 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.rtsp_pull.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.split.rst
+-rw-r--r--   0        0        0      142 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.unwarp.rst
+-rw-r--r--   0        0        0      139 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.video.utils.rst
+-rw-r--r--   0        0        0      136 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.x3m.config.rst
+-rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.x3m.preprocess.rst
+-rw-r--r--   0        0        0      272 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.x3m.rst
+-rw-r--r--   0        0        0      148 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/hello.x3m.transforms.rst
+-rw-r--r--   0        0        0      572 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/index.rst
+-rw-r--r--   0        0        0       52 2023-05-27 08:01:43.939155 hello2-1.7.7/docs/source/modules.rst
+-rw-r--r--   0        0        0     3270 2023-05-27 13:33:10.962343 hello2-1.7.7/hello/README.md
+-rw-r--r--   0        0        0      773 2023-05-28 05:35:04.232349 hello2-1.7.7/hello/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/__main__.py
+-rw-r--r--   0        0        0      471 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/data/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/data/__main__.py
+-rw-r--r--   0        0        0     3426 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/data/coco2yolo.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/experimental/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/experimental/albu/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/experimental/albu/detection.py
+-rw-r--r--   0        0        0     1047 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/fiftyone/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/fiftyone/__main__.py
+-rw-r--r--   0        0        0     4781 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/fiftyone/annotate.py
+-rw-r--r--   0        0        0    10578 2023-05-27 13:22:52.332349 hello2-1.7.7/hello/fiftyone/brain.py
+-rw-r--r--   0        0        0     7807 2023-05-28 05:34:14.242349 hello2-1.7.7/hello/fiftyone/coco.py
+-rw-r--r--   0        0        0     3037 2023-05-28 05:34:47.282349 hello2-1.7.7/hello/fiftyone/coco_utils.py
+-rw-r--r--   0        0        0      912 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/fiftyone/connected.py
+-rw-r--r--   0        0        0       36 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/fiftyone/copypaste.py
+-rw-r--r--   0        0        0    18009 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/fiftyone/core.py
+-rw-r--r--   0        0        0    19758 2023-05-28 05:08:29.392349 hello2-1.7.7/hello/fiftyone/dataset.py
+-rw-r--r--   0        0        0     7502 2023-05-27 08:01:43.939155 hello2-1.7.7/hello/fiftyone/dataset_detections.py
+-rw-r--r--   0        0        0     5693 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/dataset_segmentations.py
+-rw-r--r--   0        0        0     1402 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/dataset_yolov5.py
+-rw-r--r--   0        0        0      889 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/dataset_zoo.py
+-rw-r--r--   0        0        0     1169 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/evaluate.py
+-rw-r--r--   0        0        0     5157 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/evaluate_detections.py
+-rw-r--r--   0        0        0     4544 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/evaluate_segmentations.py
+-rw-r--r--   0        0        0      103 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/examples/README.md
+-rw-r--r--   0        0        0     2975 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/examples/examples.py
+-rw-r--r--   0        0        0    12021 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/examples/utils.py
+-rw-r--r--   0        0        0     3241 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/gen_examples.py
+-rw-r--r--   0        0        0     1608 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/mask_ignore.py
+-rw-r--r--   0        0        0     5683 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/miou.py
+-rw-r--r--   0        0        0     2639 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/patches.py
+-rw-r--r--   0        0        0     9311 2023-05-28 05:30:29.152349 hello2-1.7.7/hello/fiftyone/tarinfo.py
+-rw-r--r--   0        0        0     4094 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/unique.py
+-rw-r--r--   0        0        0     8090 2023-05-28 05:29:01.302348 hello2-1.7.7/hello/fiftyone/utils.py
+-rw-r--r--   0        0        0      781 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fiftyone/video.py
+-rw-r--r--   0        0        0     8268 2023-05-27 09:29:48.362349 hello2-1.7.7/hello/fiftyone/view.py
+-rw-r--r--   0        0        0      435 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fvcore/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fvcore/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/fvcore/core.py
+-rw-r--r--   0        0        0      135 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/io/__init__.py
+-rw-r--r--   0        0        0     1382 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/io/image.py
+-rw-r--r--   0        0        0      989 2023-05-27 23:53:07.192349 hello2-1.7.7/hello/io/utils.py
+-rw-r--r--   0        0        0      851 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmdet/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmdet/__main__.py
+-rw-r--r--   0        0        0       97 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmdet/export.py
+-rw-r--r--   0        0        0     1736 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmdet/flop.py
+-rw-r--r--   0        0        0     5446 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmdet/infer.py
+-rw-r--r--   0        0        0     3273 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmdet/log.py
+-rw-r--r--   0        0        0     5976 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmdet/plot.py
+-rw-r--r--   0        0        0      563 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmlab/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmlab/__main__.py
+-rw-r--r--   0        0        0      110 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmlab/mmdet3.py
+-rw-r--r--   0        0        0     6549 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmlab/mmseg.py
+-rw-r--r--   0        0        0      645 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmseg/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmseg/__main__.py
+-rw-r--r--   0        0        0     6040 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmseg/infer.py
+-rw-r--r--   0        0        0     2368 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmseg/log.py
+-rw-r--r--   0        0        0     7006 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/mmseg/lr.py
+-rw-r--r--   0        0        0      462 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/nanodet/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/nanodet/__main__.py
+-rw-r--r--   0        0        0     7410 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/nanodet/infer.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/onnx/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/onnx/examples/README.md
+-rw-r--r--   0        0        0     1879 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/onnx/examples/test_sigmoid.py
+-rw-r--r--   0        0        0     3024 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/onnx/export.py
+-rw-r--r--   0        0        0     1707 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/onnx/infer.py
+-rw-r--r--   0        0        0     1334 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/transforms/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/transforms/__init__.py
+-rw-r--r--   0        0        0     2655 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/transforms/transforms.py
+-rw-r--r--   0        0        0        0 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/utils/__init__.py
+-rw-r--r--   0        0        0     2133 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/utils/colors.py
+-rw-r--r--   0        0        0     1349 2023-05-28 05:28:05.432346 hello2-1.7.7/hello/utils/compare.py
+-rw-r--r--   0        0        0     1815 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/utils/cuda.py
+-rw-r--r--   0        0        0      356 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/utils/importer.py
+-rw-r--r--   0        0        0      612 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/utils/plots.py
+-rw-r--r--   0        0        0     2999 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/utils/points.py
+-rw-r--r--   0        0        0      195 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/utils/strtime.py
+-rw-r--r--   0        0        0     1135 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/__main__.py
+-rw-r--r--   0        0        0     3428 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/align.py
+-rw-r--r--   0        0        0     6382 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/clip.py
+-rw-r--r--   0        0        0     3290 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/fisheye.py
+-rw-r--r--   0        0        0     1565 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/info.py
+-rw-r--r--   0        0        0     3502 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/resize.py
+-rw-r--r--   0        0        0     4716 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/rtsp.py
+-rw-r--r--   0        0        0     5006 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/rtsp_pull.py
+-rw-r--r--   0        0        0     3048 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/split.py
+-rw-r--r--   0        0        0     4066 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/unwarp.py
+-rw-r--r--   0        0        0      968 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/video/utils.py
+-rw-r--r--   0        0        0      576 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/x3m/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/x3m/__main__.py
+-rw-r--r--   0        0        0     4479 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/x3m/config.py
+-rw-r--r--   0        0        0     2592 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/x3m/preprocess.py
+-rw-r--r--   0        0        0     6928 2023-05-27 08:01:43.949155 hello2-1.7.7/hello/x3m/transforms.py
+-rw-r--r--   0        0        0      808 2023-05-27 08:01:43.949155 hello2-1.7.7/hello_c/CMakeLists.txt
+-rw-r--r--   0        0        0      776 2023-05-27 08:01:43.949155 hello2-1.7.7/hello_c/README.md
+-rw-r--r--   0        0        0     1375 2023-05-27 08:01:43.949155 hello2-1.7.7/hello_c/main.cpp
+-rw-r--r--   0        0        0      262 2023-05-27 08:01:43.949155 hello2-1.7.7/hello_c/trace_model.py
+-rw-r--r--   0        0        0      787 2023-05-27 08:01:43.949155 hello2-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 hello2-1.7.7/PKG-INFO
```

### Comparing `hello2-1.7.6/.gitignore` & `hello2-1.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/.readthedocs.yaml` & `hello2-1.7.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/LICENSE` & `hello2-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/docs/Makefile` & `hello2-1.7.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/docs/make.bat` & `hello2-1.7.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/docs/source/conf.py` & `hello2-1.7.7/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/docs/source/hello.fiftyone.rst` & `hello2-1.7.7/docs/source/hello.fiftyone.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/docs/source/index.rst` & `hello2-1.7.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/README.md` & `hello2-1.7.7/hello/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/__init__.py` & `hello2-1.7.7/hello/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "1.7.6"
+__version__ = "1.7.7"
 
 help_doc_str = """\
 usage: hello [--version] [--help]
 
 shell command:
     hello -h
     hello-data -h
```

### Comparing `hello2-1.7.6/hello/data/coco2yolo.py` & `hello2-1.7.7/hello/data/coco2yolo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/__init__.py` & `hello2-1.7.7/hello/fiftyone/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/annotate.py` & `hello2-1.7.7/hello/fiftyone/annotate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/brain.py` & `hello2-1.7.7/hello/fiftyone/brain.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/connected.py` & `hello2-1.7.7/hello/fiftyone/connected.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/core.py` & `hello2-1.7.7/hello/fiftyone/core.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/dataset.py` & `hello2-1.7.7/hello/fiftyone/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 import fiftyone.utils.coco as fouc
 import fiftyone.utils.iou as foui
 import fiftyone.utils.yolo as fouy
 from fiftyone.utils.labels import segmentations_to_detections
 
 import hello.fiftyone.core as hoc
 import hello.fiftyone.utils as hou
-from hello.fiftyone.dataset_detections import \
-    load_dataset as _load_detection_dataset
-from hello.fiftyone.dataset_segmentations import \
-    load_dataset as _load_segmentation_dataset
 
 tmpl_info = """\
 info = {
     'dataset_name': '$dataset_name',
     'dataset_type': '$dataset_type',
     'version': '$version',
     'classes': $classes,
@@ -399,48 +395,14 @@
 
     Args:
         name (str): the name of the dataset
     """
     return fo.load_dataset(name)
 
 
-def load_detection_dataset(dataset_dir, info_py="info.py", data_path="data", labels_path="labels.json", field_name="ground_truth", splits=None):
-    dataset_dir = Path(dataset_dir)
-
-    if splits is None:
-        dataset = _load_detection_dataset(str(dataset_dir), info_py=info_py, data_path=data_path, labels_path=labels_path, field_name=field_name)
-        dataset.tag_samples("train")
-    else:
-        _datasets = []
-        for s in splits:
-            _dataset = _load_detection_dataset(str(dataset_dir / s), info_py=info_py, data_path=data_path, labels_path=labels_path, field_name=field_name)
-            _dataset.tag_samples(s)
-            _datasets.append(_dataset)
-        dataset = hoc.merge_samples(_datasets)
-
-    return dataset
-
-
-def load_segmentation_dataset(dataset_dir, info_py="info.py", data_path="data", labels_path="labels/", field_name="ground_truth", splits=None):
-    dataset_dir = Path(dataset_dir)
-
-    if splits is None:
-        dataset = _load_segmentation_dataset(str(dataset_dir), info_py=info_py, data_path=data_path, labels_path=labels_path, field_name=field_name)
-        dataset.tag_samples("train")
-    else:
-        _datasets = []
-        for s in splits:
-            _dataset = _load_segmentation_dataset(str(dataset_dir / s), info_py=info_py, data_path=data_path, labels_path=labels_path, field_name=field_name)
-            _dataset.tag_samples(s)
-            _datasets.append(_dataset)
-        dataset = hoc.merge_samples(_datasets)
-
-    return dataset
-
-
 def export_image_dataset(export_dir, dataset, splits=None):
     shutil.rmtree(export_dir, ignore_errors=True)
 
     _tags = set(dataset.distinct("tags"))
 
     if splits is None:
         splits = ["train", "val", "test"]
```

### Comparing `hello2-1.7.6/hello/fiftyone/dataset_detections.py` & `hello2-1.7.7/hello/fiftyone/dataset_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/dataset_segmentations.py` & `hello2-1.7.7/hello/fiftyone/dataset_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/dataset_yolov5.py` & `hello2-1.7.7/hello/fiftyone/dataset_yolov5.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/dataset_zoo.py` & `hello2-1.7.7/hello/fiftyone/dataset_zoo.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/evaluate.py` & `hello2-1.7.7/hello/fiftyone/evaluate.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/evaluate_detections.py` & `hello2-1.7.7/hello/fiftyone/evaluate_detections.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/evaluate_segmentations.py` & `hello2-1.7.7/hello/fiftyone/evaluate_segmentations.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/examples/examples.py` & `hello2-1.7.7/hello/fiftyone/examples/examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/examples/utils.py` & `hello2-1.7.7/hello/fiftyone/examples/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/gen_examples.py` & `hello2-1.7.7/hello/fiftyone/gen_examples.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/mask_ignore.py` & `hello2-1.7.7/hello/fiftyone/mask_ignore.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/miou.py` & `hello2-1.7.7/hello/fiftyone/miou.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/patches.py` & `hello2-1.7.7/hello/fiftyone/patches.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/tarinfo.py` & `hello2-1.7.7/hello/fiftyone/tarinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 import cv2 as cv
 import numpy as np
 from prettytable import PrettyTable
 
 import hello.io.utils as hou
-from hello.fiftyone.utils import equal_dict, equal_list
+import hello.utils.compare as hoc
 
 
 def list_files(filename, level=2):
     db = []
     with tarfile.open(filename, "r") as tar:
         for name in tar.getnames():
             if len(Path(name).parts) > level:
@@ -267,17 +267,17 @@
     results = {}
     for key in keys:
         a, b = base_info[key], side_info[key]
 
         if isinstance(a, str) and isinstance(b, str):
             result = (a == b)
         elif isinstance(a, list) and isinstance(b, list):
-            result = equal_list(a, b)
+            result = hoc.equal_list(a, b)
         elif isinstance(a, dict) and isinstance(b, dict):
-            result = equal_dict(a, b)
+            result = hoc.equal_dict(a, b)
         else:
             result = "Unkown (BadType)"
 
         if verbose:
             print(f"  <{key}>: {result}")
 
         results[key] = result
```

### Comparing `hello2-1.7.6/hello/fiftyone/unique.py` & `hello2-1.7.7/hello/fiftyone/unique.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/utils.py` & `hello2-1.7.7/hello/fiftyone/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,16 @@
 from collections import defaultdict
 from pathlib import Path
 
 import cv2 as cv
 import fiftyone.core.utils as fou
 import fiftyone.utils.iou as foui
 
-from hello.fiftyone.coco import coco_segmentation_to_mask
-
-
-def equal_list(a: list, b: list) -> bool:
-    if len(a) != len(b):
-        return False
-
-    for _ai, _bi in zip(a, b):
-        if _ai != _bi:
-            return False
-
-    return True
-
-
-def equal_dict(a: dict, b: dict) -> bool:
-    if len(a) != len(b):
-        return False
-
-    for k, v in a.items():
-        if v != b.get(k):
-            return False
-
-    return True
+from hello.fiftyone.coco_utils import coco_segmentation_to_mask
+from hello.utils.compare import equal_dict
 
 
 def _parse_text_slice(vals):
     assert len(vals) == 6
     x1, y1, x2, y2 = vals[:4]
 
     bounding_box = [
```

### Comparing `hello2-1.7.6/hello/fiftyone/video.py` & `hello2-1.7.7/hello/fiftyone/video.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fiftyone/view.py` & `hello2-1.7.7/hello/fiftyone/view.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/fvcore/core.py` & `hello2-1.7.7/hello/fvcore/core.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/io/image.py` & `hello2-1.7.7/hello/io/image.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/io/utils.py` & `hello2-1.7.7/hello/io/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmdet/__init__.py` & `hello2-1.7.7/hello/mmdet/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmdet/flop.py` & `hello2-1.7.7/hello/mmdet/flop.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmdet/infer.py` & `hello2-1.7.7/hello/mmdet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmdet/log.py` & `hello2-1.7.7/hello/mmdet/log.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmdet/plot.py` & `hello2-1.7.7/hello/mmdet/plot.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmlab/__init__.py` & `hello2-1.7.7/hello/mmlab/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmlab/mmseg.py` & `hello2-1.7.7/hello/mmlab/mmseg.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmseg/__init__.py` & `hello2-1.7.7/hello/mmseg/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmseg/infer.py` & `hello2-1.7.7/hello/mmseg/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmseg/log.py` & `hello2-1.7.7/hello/mmseg/log.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/mmseg/lr.py` & `hello2-1.7.7/hello/mmseg/lr.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/nanodet/infer.py` & `hello2-1.7.7/hello/nanodet/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/onnx/examples/test_sigmoid.py` & `hello2-1.7.7/hello/onnx/examples/test_sigmoid.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/onnx/export.py` & `hello2-1.7.7/hello/onnx/export.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/onnx/infer.py` & `hello2-1.7.7/hello/onnx/infer.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/transforms/README.md` & `hello2-1.7.7/hello/transforms/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/transforms/transforms.py` & `hello2-1.7.7/hello/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/utils/colors.py` & `hello2-1.7.7/hello/utils/colors.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/utils/cuda.py` & `hello2-1.7.7/hello/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/utils/plots.py` & `hello2-1.7.7/hello/utils/plots.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/utils/points.py` & `hello2-1.7.7/hello/utils/points.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/__init__.py` & `hello2-1.7.7/hello/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/align.py` & `hello2-1.7.7/hello/video/align.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/clip.py` & `hello2-1.7.7/hello/video/clip.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/fisheye.py` & `hello2-1.7.7/hello/video/fisheye.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/info.py` & `hello2-1.7.7/hello/video/info.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/resize.py` & `hello2-1.7.7/hello/video/resize.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/rtsp.py` & `hello2-1.7.7/hello/video/rtsp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/rtsp_pull.py` & `hello2-1.7.7/hello/video/rtsp_pull.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/split.py` & `hello2-1.7.7/hello/video/split.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/unwarp.py` & `hello2-1.7.7/hello/video/unwarp.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/video/utils.py` & `hello2-1.7.7/hello/video/utils.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/x3m/__init__.py` & `hello2-1.7.7/hello/x3m/__init__.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/x3m/config.py` & `hello2-1.7.7/hello/x3m/config.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/x3m/preprocess.py` & `hello2-1.7.7/hello/x3m/preprocess.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello/x3m/transforms.py` & `hello2-1.7.7/hello/x3m/transforms.py`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello_c/CMakeLists.txt` & `hello2-1.7.7/hello_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello_c/README.md` & `hello2-1.7.7/hello_c/README.md`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/hello_c/main.cpp` & `hello2-1.7.7/hello_c/main.cpp`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/pyproject.toml` & `hello2-1.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hello2-1.7.6/PKG-INFO` & `hello2-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hello2
-Version: 1.7.6
+Version: 1.7.7
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scikit-image
```

