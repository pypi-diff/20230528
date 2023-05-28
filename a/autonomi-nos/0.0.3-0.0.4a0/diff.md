# Comparing `tmp/autonomi_nos-0.0.3-py3-none-any.whl.zip` & `tmp/autonomi_nos-0.0.4a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,51 +1,59 @@
-Zip file size: 42344 bytes, number of entries: 49
--rw-rw-r--  2.0 unx      119 b- defN 23-Apr-23 00:49 nos/__init__.py
--rw-rw-r--  2.0 unx      561 b- defN 23-May-16 21:17 nos/constants.py
--rw-rw-r--  2.0 unx       93 b- defN 23-May-01 21:40 nos/exceptions.py
--rw-rw-r--  2.0 unx      940 b- defN 23-May-01 21:40 nos/logging.py
--rw-rw-r--  2.0 unx     2778 b- defN 23-May-19 23:50 nos/protoc.py
--rw-rw-r--  2.0 unx       22 b- defN 23-May-19 23:53 nos/version.py
--rw-rw-r--  2.0 unx      110 b- defN 23-Apr-23 00:49 nos/cli/benchmark.py
--rw-rw-r--  2.0 unx      455 b- defN 23-May-16 21:17 nos/cli/cli.py
--rw-rw-r--  2.0 unx     1983 b- defN 23-May-16 21:17 nos/cli/docker.py
--rw-rw-r--  2.0 unx     1294 b- defN 23-Apr-23 00:49 nos/cli/hub.py
--rw-rw-r--  2.0 unx     6094 b- defN 23-May-19 20:10 nos/cli/serve_grpc.py
--rw-rw-r--  2.0 unx     5962 b- defN 23-May-16 21:17 nos/cli/serve_http.py
--rw-rw-r--  2.0 unx     3479 b- defN 23-May-16 21:17 nos/cli/system.py
--rw-rw-r--  2.0 unx      425 b- defN 23-May-05 01:05 nos/cli/utils.py
--rw-rw-r--  2.0 unx      141 b- defN 23-May-18 22:36 nos/client/__init__.py
--rw-rw-r--  2.0 unx       92 b- defN 23-May-12 23:31 nos/client/exceptions.py
--rw-rw-r--  2.0 unx     7307 b- defN 23-May-19 20:10 nos/client/grpc.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-18 22:36 nos/executors/__init__.py
--rw-rw-r--  2.0 unx     6237 b- defN 23-May-19 22:34 nos/executors/ray.py
--rw-rw-r--  2.0 unx     2985 b- defN 23-May-19 20:10 nos/hub/__init__.py
--rw-rw-r--  2.0 unx     2195 b- defN 23-May-19 20:10 nos/hub/config.py
--rw-rw-r--  2.0 unx      902 b- defN 23-May-12 23:31 nos/hub/spec.py
--rw-rw-r--  2.0 unx      242 b- defN 23-May-15 21:54 nos/models/__init__.py
--rw-rw-r--  2.0 unx     2370 b- defN 23-May-10 21:27 nos/models/clip.py
--rw-rw-r--  2.0 unx     2028 b- defN 23-May-12 23:31 nos/models/faster_rcnn.py
--rw-rw-r--  2.0 unx     2651 b- defN 23-May-01 21:36 nos/models/stable_diffusion.py
--rw-rw-r--  2.0 unx       66 b- defN 23-May-13 02:32 nos/models/openmmlab/mmdetection/detection_tensorrt_dynamic-320x320-1344x1344.py
--rw-rw-r--  2.0 unx     2589 b- defN 23-May-13 02:01 nos/models/openmmlab/mmdetection/mmdetection.py
--rw-rw-r--  2.0 unx      370 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py
--rw-rw-r--  2.0 unx     3187 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py
--rw-rw-r--  2.0 unx     1765 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_instance.py
--rw-rw-r--  2.0 unx     3828 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/models/faster-rcnn_r50_fpn.py
--rw-rw-r--  2.0 unx      304 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py
--rw-rw-r--  2.0 unx     5340 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py
--rw-rw-r--  2.0 unx      177 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py
--rw-rw-r--  2.0 unx     1409 b- defN 23-May-19 20:10 nos/proto/nos_service.proto
--rw-rw-r--  2.0 unx      156 b- defN 23-May-16 21:17 nos/server/__init__.py
--rw-rw-r--  2.0 unx     6229 b- defN 23-May-19 20:10 nos/server/docker.py
--rw-rw-r--  2.0 unx     3004 b- defN 23-May-18 22:36 nos/server/runtime.py
--rw-rw-r--  2.0 unx     8880 b- defN 23-May-19 22:34 nos/server/service.py
--rw-rw-r--  2.0 unx      373 b- defN 23-Apr-23 00:49 nos/test/benchmark.py
--rw-rw-r--  2.0 unx     1317 b- defN 23-May-19 22:34 nos/test/conftest.py
--rw-rw-r--  2.0 unx     1324 b- defN 23-May-18 22:36 nos/test/utils.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5917 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4266 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/RECORD
-49 files, 103216 bytes uncompressed, 35480 bytes compressed:  65.6%
+Zip file size: 55583 bytes, number of entries: 57
+-rw-rw-r--  2.0 unx       50 b- defN 23-May-21 21:25 nos/__init__.py
+-rw-rw-r--  2.0 unx      561 b- defN 23-May-16 21:26 nos/constants.py
+-rw-rw-r--  2.0 unx       93 b- defN 23-May-11 04:43 nos/exceptions.py
+-rw-rw-r--  2.0 unx      940 b- defN 23-May-09 22:15 nos/logging.py
+-rw-rw-r--  2.0 unx     2778 b- defN 23-May-19 22:25 nos/protoc.py
+-rw-rw-r--  2.0 unx       23 b- defN 23-May-23 00:10 nos/version.py
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-05 08:07 nos/cli/benchmark.py
+-rw-rw-r--  2.0 unx      455 b- defN 23-May-15 21:47 nos/cli/cli.py
+-rw-rw-r--  2.0 unx     1983 b- defN 23-May-15 21:47 nos/cli/docker.py
+-rw-rw-r--  2.0 unx     1294 b- defN 23-May-05 08:07 nos/cli/hub.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-May-26 22:01 nos/cli/serve_grpc.py
+-rw-rw-r--  2.0 unx     5962 b- defN 23-May-15 21:47 nos/cli/serve_http.py
+-rw-rw-r--  2.0 unx     3479 b- defN 23-May-15 21:47 nos/cli/system.py
+-rw-rw-r--  2.0 unx      425 b- defN 23-May-09 22:15 nos/cli/utils.py
+-rw-rw-r--  2.0 unx      372 b- defN 23-May-26 22:01 nos/client/__init__.py
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-11 04:42 nos/client/exceptions.py
+-rw-rw-r--  2.0 unx    12657 b- defN 23-May-26 22:01 nos/client/grpc.py
+-rw-rw-r--  2.0 unx      286 b- defN 23-May-26 22:01 nos/common/__init__.py
+-rw-rw-r--  2.0 unx     3715 b- defN 23-May-27 23:58 nos/common/spec.py
+-rw-rw-r--  2.0 unx      518 b- defN 23-May-26 22:01 nos/common/tasks.py
+-rw-rw-r--  2.0 unx     4851 b- defN 23-May-27 23:51 nos/common/types.py
+-rw-rw-r--  2.0 unx     3470 b- defN 23-May-08 23:12 nos/examples/vid2bbox.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 17:00 nos/executors/__init__.py
+-rw-rw-r--  2.0 unx     7401 b- defN 23-May-26 22:01 nos/executors/ray.py
+-rw-rw-r--  2.0 unx     1246 b- defN 23-May-15 21:47 nos/experimental/conversion_flows/openmmlab/tensorrt/run_model.py
+-rw-rw-r--  2.0 unx     4559 b- defN 23-May-15 21:47 nos/experimental/http/__init__.py
+-rw-rw-r--  2.0 unx     1153 b- defN 23-May-15 21:47 nos/experimental/http/client.py
+-rw-rw-r--  2.0 unx     2605 b- defN 23-May-26 22:01 nos/experimental/http/ingress.py
+-rw-rw-r--  2.0 unx     2688 b- defN 23-May-15 21:47 nos/experimental/http/service.py
+-rw-rw-r--  2.0 unx     3436 b- defN 23-May-26 22:01 nos/hub/__init__.py
+-rw-rw-r--  2.0 unx     2195 b- defN 23-May-19 04:30 nos/hub/config.py
+-rw-rw-r--  2.0 unx      242 b- defN 23-May-12 00:37 nos/models/__init__.py
+-rw-rw-r--  2.0 unx     3460 b- defN 23-May-27 23:33 nos/models/clip.py
+-rw-rw-r--  2.0 unx     2804 b- defN 23-May-27 23:33 nos/models/faster_rcnn.py
+-rw-rw-r--  2.0 unx     3150 b- defN 23-May-27 23:29 nos/models/stable_diffusion.py
+-rw-rw-r--  2.0 unx     2628 b- defN 23-May-26 22:01 nos/models/openmmlab/mmdetection/mmdetection.py
+-rw-rw-r--  2.0 unx      370 b- defN 23-May-09 22:15 nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py
+-rw-rw-r--  2.0 unx     3187 b- defN 23-May-09 22:15 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py
+-rw-rw-r--  2.0 unx     1765 b- defN 23-May-09 22:15 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_instance.py
+-rw-rw-r--  2.0 unx     3828 b- defN 23-May-10 02:43 nos/models/openmmlab/mmdetection/configs/_base_/models/faster-rcnn_r50_fpn.py
+-rw-rw-r--  2.0 unx      304 b- defN 23-May-09 22:15 nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py
+-rw-rw-r--  2.0 unx     5340 b- defN 23-May-09 22:15 nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py
+-rw-rw-r--  2.0 unx      177 b- defN 23-May-10 02:43 nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py
+-rw-rw-r--  2.0 unx     2437 b- defN 23-May-26 22:01 nos/proto/nos_service.proto
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-23 17:24 nos/server/__init__.py
+-rw-rw-r--  2.0 unx     6229 b- defN 23-May-19 03:42 nos/server/docker.py
+-rw-rw-r--  2.0 unx     2976 b- defN 23-May-22 17:53 nos/server/runtime.py
+-rw-rw-r--  2.0 unx     9887 b- defN 23-May-26 22:01 nos/server/service.py
+-rw-rw-r--  2.0 unx      373 b- defN 23-May-05 08:07 nos/test/benchmark.py
+-rw-rw-r--  2.0 unx     5764 b- defN 23-May-26 22:01 nos/test/conftest.py
+-rw-rw-r--  2.0 unx     1347 b- defN 23-May-21 21:52 nos/test/utils.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6257 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4934 b- defN 23-May-28 00:10 autonomi_nos-0.0.4a0.dist-info/RECORD
+57 files, 144316 bytes uncompressed, 47687 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -45,44 +45,68 @@
 
 Filename: nos/client/exceptions.py
 Comment: 
 
 Filename: nos/client/grpc.py
 Comment: 
 
+Filename: nos/common/__init__.py
+Comment: 
+
+Filename: nos/common/spec.py
+Comment: 
+
+Filename: nos/common/tasks.py
+Comment: 
+
+Filename: nos/common/types.py
+Comment: 
+
+Filename: nos/examples/vid2bbox.py
+Comment: 
+
 Filename: nos/executors/__init__.py
 Comment: 
 
 Filename: nos/executors/ray.py
 Comment: 
 
-Filename: nos/hub/__init__.py
+Filename: nos/experimental/conversion_flows/openmmlab/tensorrt/run_model.py
 Comment: 
 
-Filename: nos/hub/config.py
+Filename: nos/experimental/http/__init__.py
 Comment: 
 
-Filename: nos/hub/spec.py
+Filename: nos/experimental/http/client.py
+Comment: 
+
+Filename: nos/experimental/http/ingress.py
+Comment: 
+
+Filename: nos/experimental/http/service.py
+Comment: 
+
+Filename: nos/hub/__init__.py
+Comment: 
+
+Filename: nos/hub/config.py
 Comment: 
 
 Filename: nos/models/__init__.py
 Comment: 
 
 Filename: nos/models/clip.py
 Comment: 
 
 Filename: nos/models/faster_rcnn.py
 Comment: 
 
 Filename: nos/models/stable_diffusion.py
 Comment: 
 
-Filename: nos/models/openmmlab/mmdetection/detection_tensorrt_dynamic-320x320-1344x1344.py
-Comment: 
-
 Filename: nos/models/openmmlab/mmdetection/mmdetection.py
 Comment: 
 
 Filename: nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py
 Comment: 
 
 Filename: nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py
@@ -123,26 +147,26 @@
 
 Filename: nos/test/conftest.py
 Comment: 
 
 Filename: nos/test/utils.py
 Comment: 
 
-Filename: autonomi_nos-0.0.3.dist-info/LICENSE
+Filename: autonomi_nos-0.0.4a0.dist-info/LICENSE
 Comment: 
 
-Filename: autonomi_nos-0.0.3.dist-info/METADATA
+Filename: autonomi_nos-0.0.4a0.dist-info/METADATA
 Comment: 
 
-Filename: autonomi_nos-0.0.3.dist-info/WHEEL
+Filename: autonomi_nos-0.0.4a0.dist-info/WHEEL
 Comment: 
 
-Filename: autonomi_nos-0.0.3.dist-info/entry_points.txt
+Filename: autonomi_nos-0.0.4a0.dist-info/entry_points.txt
 Comment: 
 
-Filename: autonomi_nos-0.0.3.dist-info/top_level.txt
+Filename: autonomi_nos-0.0.4a0.dist-info/top_level.txt
 Comment: 
 
-Filename: autonomi_nos-0.0.3.dist-info/RECORD
+Filename: autonomi_nos-0.0.4a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nos/__init__.py

```diff
@@ -1,5 +1 @@
-from nos import (
-    hub,  # noqa: F401
-    models,  # noqa: F401
-)
 from nos.version import __version__  # noqa: F401
```

## nos/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.3"
+__version__ = "0.0.4a"
```

## nos/cli/serve_grpc.py

```diff
@@ -15,14 +15,15 @@
 import rich.console
 import rich.status
 import rich.table
 import typer
 
 from nos.client import InferenceClient
 from nos.client.exceptions import NosClientException
+from nos.common import TaskType
 
 
 serve_grpc_cli = typer.Typer(name="serve-grpc", help="NOS gRPC Serve CLI.", no_args_is_help=True)
 console = rich.console.Console()
 
 
 @dataclass
@@ -32,15 +33,15 @@
     address: str
     client: InferenceClient
 
 
 @serve_grpc_cli.callback()
 def grpc_config(
     ctx: typer.Context,
-    address: str = typer.Option("localhost:50051", "-a", "--address", help="Address of the gRPC server."),
+    address: str = typer.Option("[::]:50051", "-a", "--address", help="Address of the gRPC server."),
 ):
     """Common gRPC options"""
     client = InferenceClient(address)
     ctx.obj = gRPCConfig(address, client)
     # TODO (spillai): Deploy the gRPC server here in the background (as a docker daemon)
     # TOOD (spillai): Ping the gRPC server otherwise raise an error
 
@@ -67,20 +68,21 @@
     filename: str = typer.Option(..., "-i", "--input", help="Input image filename."),
 ) -> None:
     from PIL import Image
 
     img = Image.open(filename)
 
     st = time.perf_counter()
-    with rich.status.Status("[bold green] Generating embedding ...[/bold green]"):
-        try:
-            response = ctx.obj.client.Predict(method="img2vec", model_name=model_name, img=img)
-        except NosClientException as exc:
-            console.print(f"[red] ✗ Failed to encode image. [/red]\n[bold red]{exc}[/bold red]")
-            return
+    # with rich.status.Status("[bold green] Generating embedding ...[/bold green]"):
+    try:
+        model = ctx.obj.client.Module(task=TaskType.IMAGE_EMBEDDING, model_name=model_name)
+        response = model(images=img)
+    except NosClientException as exc:
+        console.print(f"[red] ✗ Failed to encode image. [/red]\n[bold red]{exc}[/bold red]")
+        return
     console.print(
         f"[bold green] ✓ Generated embedding ((1, {response['embedding'].shape[-1]}), time=~{(time.perf_counter() - st) * 1e3:.1f}ms) [/bold green]"
     )
 
 
 @serve_grpc_cli.command("txt2vec", help="Generate an embedding from a text prompt.")
 def _predict_txt2vec(
@@ -94,15 +96,16 @@
     prompt: str = typer.Option(
         ..., "-i", "--input", help="Prompt to generate image. (e.g. a cat dancing on the grass.)"
     ),
 ) -> None:
     st = time.perf_counter()
     with rich.status.Status("[bold green] Generating embedding ...[/bold green]"):
         try:
-            response = ctx.obj.client.Predict(method="txt2vec", model_name=model_name, text=prompt)
+            model = ctx.obj.client.Module(task=TaskType.TEXT_EMBEDDING, model_name=model_name)
+            response = model(texts=prompt)
         except NosClientException as exc:
             console.print(f"[red] ✗ Failed to generate image. [/red]\n[bold red]{exc}[/bold red]")
             return
     console.print(
         f"[bold green] ✓ Generated embedding ({response['embedding'][..., :].shape}..., time=~{(time.perf_counter() - st) * 1e3:.1f}ms) [/bold green]"
     )
 
@@ -120,20 +123,21 @@
         ..., "-i", "--input", help="Prompt to generate image. (e.g. a cat dancing on the grass.)"
     ),
     img_size: int = typer.Option(512, "-s", "--img-size", help="Image size to generate."),
 ) -> None:
     st = time.perf_counter()
     with rich.status.Status("[bold green] Generating image ...[/bold green]"):
         try:
-            response = ctx.obj.client.Predict(method="txt2img", model_name=model_name, text=prompt)
+            model = ctx.obj.client.Module(task=TaskType.IMAGE_GENERATION, model_name=model_name)
+            response = model(prompts=prompt)
         except NosClientException as exc:
             console.print(f"[red] ✗ Failed to generate image. [/red]\n[bold red]{exc}[/bold red]")
             return
     console.print(
-        f"[bold green] ✓ Generated image ({response['image']}..., time=~{(time.perf_counter() - st) * 1e3:.1f}ms) [/bold green]"
+        f"[bold green] ✓ Generated image ({response['images']}..., time=~{(time.perf_counter() - st) * 1e3:.1f}ms) [/bold green]"
     )
 
 
 @serve_grpc_cli.command("img2bbox", help="Predict bounding boxes from image.")
 def _predict_img2bbox(
     ctx: typer.Context,
     model_name: str = typer.Option(
@@ -147,19 +151,16 @@
     from PIL import Image
 
     img = Image.open(filename).resize((640, 480))
     with rich.status.Status("[bold green] Predict bounding boxes ...[/bold green]"):
 
         st = time.perf_counter()
         try:
-            response = ctx.obj.client.Predict(
-                method="img2bbox",
-                model_name=model_name,
-                img=img,
-            )
+            model = ctx.obj.client.Module(task=TaskType.OBJECT_DETECTION_2D, model_name=model_name)
+            response = model(images=img)
             scores, labels, bboxes = response["bboxes"], response["scores"], response["labels"]
             console.print(
                 f"[bold green] ✓ Predicted bounding boxes (bboxes={bboxes.shape}, scores={scores.shape}, labels={labels.shape}, time=~{(time.perf_counter() - st) * 1e3:.1f}ms) [/bold green]"
             )
         except NosClientException as exc:
             console.print(f"[red] ✗ Failed to predict bounding boxes. [/red]\n[bold red]{exc}[/bold red]")
             return
```

## nos/client/__init__.py

```diff
@@ -1,3 +1,6 @@
-from nos.client.exceptions import NosClientException
-from nos.client.grpc import InferenceClient
+from nos.client.exceptions import NosClientException  # noqa: F401
+from nos.client.grpc import InferenceClient  # noqa: F401
+from nos.common.spec import FunctionSignature, ModelSpec  # noqa: F401
+from nos.common.tasks import TaskType  # noqa: F401
+from nos.common.types import EmbeddingSpec, ImageSpec, TensorSpec  # noqa: F401
 from nos.constants import DEFAULT_GRPC_PORT
```

## nos/client/grpc.py

```diff
@@ -1,52 +1,31 @@
 """gRPC client for NOS service."""
-from contextlib import contextmanager
-from dataclasses import dataclass
-from typing import List, Union
+import time
+from dataclasses import dataclass, field
+from functools import lru_cache
+from typing import Any, Callable, Dict, List, Union
 
 import cloudpickle
 import grpc
 import numpy as np
 from google.protobuf import empty_pb2
 from PIL import Image
 
 from nos.client.exceptions import NosClientException
+from nos.common import ModelSpec, TaskType
 from nos.constants import DEFAULT_GRPC_PORT
 from nos.logging import logger
 from nos.protoc import import_module
+from nos.version import __version__
 
 
 nos_service_pb2 = import_module("nos_service_pb2")
 nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
 
 
-@contextmanager
-def InferenceSession(stub: nos_service_pb2_grpc.InferenceServiceStub, model_name: str, num_replicas: int = 1):
-    """Remote model context manager.
-
-    Args:
-        stub (nos_service_pb2_grpc.InferenceServiceStub): gRPC stub.
-        model_name (str): Name of the model to init.
-        num_replicas (int): Number of replicas to init.
-
-    Yields:
-        None (NoneType): Nothing.
-    """
-    # Create inference stub and init model
-    request = nos_service_pb2.InitModelRequest(model_name=model_name, num_replicas=num_replicas)
-    response: nos_service_pb2.InitModelResponse = stub.InitModel(request)
-    logger.info(f"Init Model response: {response}")
-    # Yield so that the model inference can be done
-    yield
-    # Delete model
-    request = nos_service_pb2.DeleteModelRequest(model_name=model_name)
-    response: nos_service_pb2.DeleteModelResponse = stub.DeleteModel(request)
-    logger.info(f"Delete Model response: {response}")
-
-
 @dataclass
 class InferenceClientState:
     """State of the client for serialization purposes."""
 
     address: str
     """Address for the gRPC server."""
 
@@ -55,30 +34,30 @@
     """Main gRPC client for NOS inference service.
 
     Parameters:
         address (str): Address for the gRPC server.
 
     Usage:
         ```py
-        # Create client
-        >>> client = InferenceClient(address="localhost:50051")
 
-        # List all models registered with the server
-        # models = ['openai/clip-vit-base-patch32', ...]
-        >>> models = models client.ListModels()
+        >>> client = InferenceClient(address="localhost:50051")  # create client
+        >>> client.WaitForServer()  # wait for server to start
+        >>> client.CheckCompatibility()  # check compatibility with server
 
-        # Encode "Hello world!" with the CLIP text encoder
-        >>> client.Predict(method=MethodType.TXT2VEC, model_name="openai/clip-vit-base-patch32", text="Hello world!")
+        >>> client.ListModels()  # list all models registered
 
-        # Encode img with the CLIP visual encoder
-        >>> client.Predict(method=MethodType.IMG2VEC, model_name="openai/clip-vit-base-patch32", text="Hello world!")
+        >>> text_model = client.Module(TaskType.TEXT_EMBEDDING, "openai/clip-vit-base-patch32")  # instantiate CLIP module
+        >>> text_model(text="Hello world!")  # predict with CLIP
 
-        # Predict bounding-boxes from with FastRCNN
         >>> img = Image.open("test.jpg")
-        >>> client.Predict(method=MethodType.IMG2BBOX, model_name="torchvision/fasterrcnn_mobilenet_v3_large_320_fpn", img=img)
+        >>> visual_model = client.Module(TaskType.IMAGE_EMBEDDING, "openai/clip-vit-base-patch32")  # instantiate CLIP module
+        >>> visual_model(images=img)  # predict with CLIP
+
+        >>> fastrcnn_model = client.Module(TaskType.OBJECT_DETECTION_2D, "torchvision/fasterrcnn_mobilenet_v3_large_320_fpn")  # instantiate FasterRCNN module
+        >>> fastrcnn_model(images=img)
         ```
     """
 
     def __init__(self, address: str = f"[::]:{DEFAULT_GRPC_PORT}"):
         """Initializes the gRPC client.
 
         Args:
@@ -97,15 +76,14 @@
         return InferenceClientState(address=self.address)
 
     def __setstate__(self, state: InferenceClientState) -> None:
         """Sets the state of the client for de-serialization purposes.
 
         Args:
             state (InferenceClientState): State of the client.
-
         Returns:
             None (NoneType): Nothing.
         """
         self.address = state.address
         self._channel = None
         self._stub = None
 
@@ -115,87 +93,246 @@
 
         Note: The stub is created on-demand for serialization purposes,
         as we don't want to create a channel until we actually need it.
         This is especially useful for pickling/un-pickling the client.
 
         Returns:
             nos_service_pb2_grpc.InferenceServiceStub: gRPC stub.
+        Raises:
+            NosClientException: If the server fails to respond to the connection request.
         """
         if not self._stub:
             self._channel = grpc.insecure_channel(self.address)
-            self._stub = nos_service_pb2_grpc.InferenceServiceStub(self._channel)
+            try:
+                self._stub = nos_service_pb2_grpc.InferenceServiceStub(self._channel)
+            except Exception as e:
+                raise NosClientException(f"Failed to connect to server ({e})")
         assert self._channel
         assert self._stub
         return self._stub
 
-    def ListModels(self) -> List[str]:
+    def IsHealthy(self) -> bool:
+        """Check if the gRPC server is healthy.
+
+        Returns:
+            bool: True if the server is running, False otherwise.
+        Raises:
+            NosClientException: If the server fails to respond to the ping.
+        """
+        try:
+            response: nos_service_pb2.PingResponse = self.stub.Ping(empty_pb2.Empty())
+            return response.status == "ok"
+        except grpc.RpcError as exc:
+            raise NosClientException(f"Failed to ping server ({exc})")
+
+    def WaitForServer(self, timeout: int = 60, retry_interval: int = 5) -> None:
+        """Ping the gRPC server for health.
+
+        Args:
+            timeout (int, optional): Timeout in seconds. Defaults to 60.
+            retry_interval (int, optional): Retry interval in seconds. Defaults to 5.
+        Returns:
+            bool: True if the server is running, False otherwise.
+        Raises:
+            NosClientException: If the server fails to respond to the ping or times out.
+        """
+        exc = None
+        st = time.time()
+        while time.time() - st <= timeout:
+            try:
+                return self.IsHealthy()
+            except Exception:
+                logger.warning("Waiting for server to start... (elapsed={:.0f}s)".format(time.time() - st))
+                time.sleep(retry_interval)
+        raise NosClientException(f"Failed to ping server ({exc})")
+
+    def GetServiceVersion(self) -> str:
+        """Get service version.
+
+        Returns:
+            str: Service version (e.g. 0.0.4).
+        Raises:
+            NosClientException: If the server fails to respond to the request.
+        """
+        try:
+            response: nos_service_pb2.ServiceInfoResponse = self.stub.GetServiceInfo(empty_pb2.Empty())
+            return response.version
+        except grpc.RpcError as e:
+            raise NosClientException(f"Failed to get service info ({e})")
+
+    def CheckCompatibility(self) -> bool:
+        """Check if the service version is compatible with the client.
+
+        Returns:
+            bool: True if the service version is compatible, False otherwise.
+        Raises:
+            NosClientException: If the server fails to respond to the request.
+        """
+        # TODO (spillai): For now, we enforce strict version matching
+        # until we have tests for client-server compatibility.
+        is_compatible = self.GetServiceVersion() == __version__
+        if not is_compatible:
+            raise NosClientException(
+                f"Client-Server version mismatch (client={__version__}, server={self.GetServiceVersion()})"
+            )
+        return is_compatible
+
+    def ListModels(self) -> List[ModelSpec]:
         """List all models.
 
         Returns:
-            List[str]: List of model names.
+            List[ModelInfo]: List of ModelInfo (name, task).
+        Raises:
+            NosClientException: If the server fails to respond to the request.
         """
         try:
             response: nos_service_pb2.ModelListResponse = self.stub.ListModels(empty_pb2.Empty())
             logger.debug(response.models)
-            return list(response.models)
+            return [ModelSpec(name=minfo.name, task=TaskType(minfo.task)) for minfo in response.models]
         except grpc.RpcError as e:
-            logger.error(f"Failed to list models ({e})")
+            raise NosClientException(f"Failed to list models ({e})")
 
-    def GetModelInfo(self, model_name: str):
+    def GetModelInfo(self, model_spec: ModelSpec) -> ModelSpec:
         """Get the relevant model information from the model name.
 
         Note: This may be possible only after initialization, as we need to inspect the
         HW to understand the configurable image resolutions, batch sizes etc.
 
         Args:
-            model_name (str): Model identifier (e.g. openai/clip-vit-base-patch32).
+            model_spec (ModelSpec): Model specification.
         """
-        raise NotImplementedError()
+        try:
+            response: nos_service_pb2.ModelInfoResponse = self.stub.GetModelInfo(
+                nos_service_pb2.ModelInfoRequest(
+                    request=nos_service_pb2.ModelInfo(task=model_spec.task.value, name=model_spec.name)
+                )
+            )
+            logger.debug(response)
+            spec: ModelSpec = cloudpickle.loads(response.response_bytes)
+            return spec
+        except grpc.RpcError as e:
+            raise NosClientException(f"Failed to get model info ({e})")
+
+    @lru_cache(maxsize=32)  # noqa: B019
+    def Module(self, task: TaskType, model_name: str) -> "InferenceModule":
+        """Instantiate a model module.
 
-    def Predict(
+        Args:
+            task (TaskType): Task used for prediction.
+            model_name (str): Name of the model to init.
+        Returns:
+            InferenceModule: Inference module.
+        """
+        return InferenceModule(task, model_name, self)
+
+    @lru_cache(maxsize=32)  # noqa: B019
+    def ModuleFromSpec(self, spec: ModelSpec) -> "InferenceModule":
+        """Instantiate a model module from a model spec.
+
+        Args:
+            spec (ModelSpec): Model specification.
+        Returns:
+            InferenceModule: Inference module.
+        """
+        return InferenceModule(spec.task, spec.name, self)
+
+    def ModuleFromCls(self, cls: Callable) -> "InferenceModule":
+        raise NotImplementedError("ModuleFromCls not implemented yet.")
+
+    def Run(
         self,
-        method: str,
+        task: TaskType,
         model_name: str,
         img: Union[Image.Image, np.ndarray, List[Image.Image], List[np.ndarray]] = None,
         text: str = None,
     ) -> nos_service_pb2.InferenceResponse:
-        """Predict with model identifier.
+        """Run module.
 
         Args:
-            method (str):
-                Method to use for prediction (one of MethodType.TXT2VEC, MethodType.IMG2VEC,
-                MethodType.IMG2BBOX, MethodType.TXT2IMG).
+            task (TaskType): Task used for prediction.
+                Tasks supported:
+                    (TaskType.OBJECT_DETECTION_2D, TaskType.IMAGE_SEGMENTATION_2D,
+                    TaskType.IMAGE_CLASSIFICATION, TaskType.IMAGE_GENERATION,
+                    TaskType.IMAGE_EMBEDDING, TaskType.TEXT_EMBEDDING)
             model_name (str):
                 Model identifier (e.g. openai/clip-vit-base-patch32).
             img (Union[Image.Image, np.ndarray, List[Image.Image], List[np.ndarray]]):
                 Image or text to predict on.
             text (str): Prompt text to use for text-generation or embedding.
-
         Returns:
             nos_service_pb2.InferenceResponse: Inference response.
+        Raises:
+            NosClientException: If the server fails to respond to the request.
         """
-        if method not in ("txt2vec", "img2vec", "img2bbox", "txt2img"):
-            raise NosClientException(f"Invalid method {method}")
+        module: InferenceModule = self.Module(task, model_name)
+        return module(img=img, text=text)
+
 
+@dataclass
+class InferenceModule:
+    """Inference module for remote model execution.
+
+    Usage:
+        ```python
+        # Create client
+        >>> client = InferenceClient()
+        # Instantiate new task module with specific model name
+        >>> model = client.Module(TaskType.IMAGE_EMBEDDING, "openai/clip-vit-base-patch32")
+        # Predict with model using `__call__`
+        >>> predictions = model({"images": img})
+        ```
+    """
+
+    task: TaskType
+    """Task used for prediction.
+       (TaskType.OBJECT_DETECTION_2D, TaskType.IMAGE_SEGMENTATION_2D,
+        TaskType.IMAGE_CLASSIFICATION, TaskType.IMAGE_GENERATION,
+        TaskType.IMAGE_EMBEDDING, TaskType.TEXT_EMBEDDING)
+    """
+    model_name: str
+    """Model identifier (e.g. openai/clip-vit-base-patch32)."""
+    _client: InferenceClient
+    """gRPC client."""
+    _spec: ModelSpec = field(init=False)
+    """Model specification for this module."""
+
+    def __post_init__(self):
+        """Initialize the spec."""
+        self._spec = self._client.GetModelInfo(ModelSpec(name=self.model_name, task=self.task))
+
+    @property
+    def stub(self):
+        return self._client.stub
+
+    def GetModelInfo(self) -> ModelSpec:
+        """Get the relevant model information from the model name."""
+        return self._spec
+
+    def __call__(self, **inputs: Dict[str, Any]) -> nos_service_pb2.InferenceResponse:
+        """Call the instantiated module/model.
+
+        Args:
+            **inputs (Dict[str, Any]): Inputs to the model ("images", "texts", "prompts" etc) as
+                defined in the ModelSpec.signature.inputs.
+        Returns:
+            nos_service_pb2.InferenceResponse: Inference response.
+        Raises:
+            NosClientException: If the server fails to respond to the request.
+        """
+        # Check if the input dictionary is consistent
+        # with inputs/outputs defined in `spec.signature`
+        # and then encode it.
+        inputs = self._spec.signature.encode_inputs(inputs)
+        request = nos_service_pb2.InferenceRequest(
+            model=nos_service_pb2.ModelInfo(
+                task=self.task.value,
+                name=self.model_name,
+            ),
+            inputs=inputs,
+        )
         try:
-            if method in ("txt2vec", "txt2img"):
-                response = self.stub.Predict(
-                    nos_service_pb2.InferenceRequest(
-                        method=method,
-                        model_name=model_name,
-                        text_request=nos_service_pb2.TextRequest(text=text),
-                    )
-                )
-            elif method in ("img2vec", "img2bbox"):
-                response = self.stub.Predict(
-                    nos_service_pb2.InferenceRequest(
-                        method=method,
-                        model_name=model_name,
-                        image_request=nos_service_pb2.ImageRequest(image_bytes=cloudpickle.dumps(img, protocol=4)),
-                    )
-                )
-            response = cloudpickle.loads(response.result)
+            response = self.stub.Run(request)
+            response = cloudpickle.loads(response.response_bytes)
             logger.debug(response)
             return response
         except grpc.RpcError as e:
-            logger.error(f"Failed to predict with model {model_name} ({e})")
-            raise NosClientException(f"Failed to predict with model {model_name} ({e})")
+            raise NosClientException(f"Failed to run model {self.model_name} ({e})")
```

## nos/executors/ray.py

```diff
@@ -86,82 +86,98 @@
         console = rich.console.Console()
         while time.time() - st <= timeout and attempt < max_attempts:
             # Attempt to connect to an existing ray cluster in the background.
             try:
                 with console.status(
                     "[bold green] InferenceExecutor :: Connecting to backend ... [/bold green]"
                 ) as status:
+                    logger.debug(f"Connecting to executor: namespace={self.spec.namespace}")
                     ray.init(
                         address="auto",
                         namespace=self.spec.namespace,
                         runtime_env=self.spec.runtime_env,
                         ignore_reinit_error=True,
                         configure_logging=True,
                         logging_level=logging.ERROR,
                         log_to_driver=level <= logging.ERROR,
                     )
                     status.stop()
                     console.print("[bold green] ✓ InferenceExecutor :: Connected to backend. [/bold green]")
+                    logger.debug(
+                        f"Connected to executor: namespace={self.spec.namespace} (time={time.time() - st:.2f}s)"
+                    )
                 return True
             except ConnectionError as exc:
                 # If Ray head is not running (this results in a ConnectionError),
                 # start it in a background subprocess.
                 if attempt > 0:
                     logger.error(
                         f"Failed to connect to InferenceExecutor.\n"
                         f"{exc}\n"
                         f"Retrying {attempt}/{max_attempts} after {retry_interval}s..."
                     )
+                else:
+                    logger.debug("No executor found, starting a new one")
                 self.start()
                 attempt += 1
 
                 time.sleep(retry_interval)
+        logger.error(f"Failed to connect to InferenceExecutor: namespace={self.spec.namespace}.")
         return False
 
     def start(self) -> None:
         """Force-start a local instance of Ray head."""
         level = getattr(logging, LOGGING_LEVEL)
 
+        st = time.time()
         console = rich.console.Console()
         with console.status(
             "[bold green] InferenceExecutor :: Backend initializing (as daemon) ... [/bold green]"
         ) as status:
             try:
+                logger.debug(f"Starting executor: namespace={self.spec.namespace}")
                 ray.init(
                     _node_name="nos-executor",
                     address="local",
                     namespace=self.spec.namespace,
                     runtime_env=self.spec.runtime_env,
                     ignore_reinit_error=False,
                     include_dashboard=False,
                     configure_logging=True,
                     logging_level=logging.ERROR,
                     log_to_driver=level <= logging.ERROR,
                 )
+                logger.debug(f"Started executor: namespace={self.spec.namespace} (time={time.time() - st:.2f}s)")
                 status.stop()
             except ConnectionError as exc:
+                logger.error(f"Failed to start executor: exc={exc}.")
                 raise RuntimeError(f"Failed to start executor: exc={exc}.")
             console.print("[bold green] ✓ InferenceExecutor :: Backend initialized. [/bold green]")
+            logger.debug(f"Started executor: namespace={self.spec.namespace} (time={time.time() - st}s)")
 
     def stop(self) -> None:
         """Stop Ray head."""
         console = rich.console.Console()
         with console.status("[bold green] InferenceExecutor :: Backend stopping ... [/bold green]"):
             try:
+                logger.debug(f"Stopping executor: namespace={self.spec.namespace}")
                 ray.shutdown()
+                logger.debug(f"Stopped executor: namespace={self.spec.namespace}")
             except Exception as exc:
+                logger.error(f"Failed to stop executor: exc={exc}.")
                 raise RuntimeError(f"Failed to stop executor: exc={exc}.")
             console.print("[bold green] ✓ InferenceExecutor :: Backend stopped. [/bold green]")
 
     @property
     def pid(self) -> Optional[int]:
         """Get PID of Ray head."""
         for proc in psutil.process_iter(attrs=["pid", "name"]):
             if proc.name() == "raylet":
                 return proc.pid
         return None
 
 
 def init(*args, **kwargs) -> bool:
     """Initialize Ray executor."""
+    logger.debug(f"Initializing executor: args={args}, kwargs={kwargs}")
     exector = RayExecutor.get()
     return exector.init(*args, **kwargs)
```

## nos/hub/__init__.py

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Optional, Type
 
+from nos.common import FunctionSignature, ModelSpec, TaskType  # noqa: F401
 from nos.hub.config import HuggingFaceHubConfig, MMLabConfig, NosHubConfig, TorchHubConfig  # noqa: F401
-from nos.hub.spec import MethodType, ModelSpec  # noqa: F401
 from nos.logging import logger
 
 
 class Hub:
     """Registry for models."""
 
     _instance: Optional["Hub"] = None
@@ -21,72 +21,79 @@
             Hub: Singleton instance.
         """
         if cls._instance is None:
             cls._instance = cls()
         return cls._instance
 
     @classmethod
-    def list(cls, private: bool = False) -> List[Dict[str, Any]]:
+    def list(cls, private: bool = False) -> List[ModelSpec]:
         """List models in the registry.
 
         Args:
             private (bool): Whether to include private models.
 
         Returns:
             List[Dict[str, Any]]: List of model specifications.
         """
         if private:
             raise NotImplementedError("Private models not supported.")
-        return [v.name for v in cls.get()._registry.values()]
+        return [v for v in cls.get()._registry.values()]
 
     @classmethod
-    def load_spec(cls, model_name: str) -> ModelSpec:
+    def load_spec(cls, model_name: str, task: TaskType = None) -> ModelSpec:
         """Load model spec from the registry.
 
         Args:
             model_name (str): Model identifier (e.g. `openai/clip-vit-base-patch32`).
+            task (TaskType): Task type (e.g. `TaskType.OBJECT_DETECTION_2D`).
 
         Returns:
             ModelSpec: Model specification.
         """
         try:
-            return cls.get()._registry[model_name]
+            return cls.get()._registry[ModelSpec.get_id(model_name, task=task)]
         except KeyError:
             raise KeyError(f"Unavailable model (name={model_name}).")
 
     @classmethod
-    def load(cls, model_name: str) -> Any:
+    def load(cls, model_name: str, task: TaskType = None) -> Any:
         """Instantiate model from the registry.
 
         Args:
             model_name (str): Model identifier (e.g. `openai/clip-vit-base-patch32`).
+            task (TaskType): Task type (e.g. `TaskType.OBJECT_DETECTION_2D`).
 
         Returns:
             Any: Instantiated model.
         """
-        spec: ModelSpec = cls.load_spec(model_name)
+        spec: ModelSpec = cls.load_spec(model_name, task=task)
         return spec.cls(*spec.args, **spec.kwargs)
 
     @classmethod
-    def register(cls, model_name: str, method: str, model_cls: Type[Any], *args, **kwargs) -> None:
+    def register(cls, model_name: str, task: TaskType, func_or_cls: Type[Any], **kwargs) -> None:
         """Model registry decorator.
 
         Args:
             model_name (str): Model identifier (e.g. `openai/clip-vit-base-patch32`).
-            method (str): Method to use for prediction (one of `MethodType.TXT2VEC`, `MethodType.IMG2VEC`,
-                `MethodType.IMG2BBOX`, `MethodType.TXT2IMG`).
-            model_cls (Type[Any]): Model class.
+            task (TaskType): Task type (e.g. `TaskType.OBJECT_DETECTION_2D`).
+            func_or_cls (Type[Any]): Model function or class.
         """
-        cls.get()._registry[model_name] = ModelSpec(
+        spec = ModelSpec(
             name=model_name,
-            method=MethodType[method.upper()],
-            cls=model_cls,
-            args=kwargs.pop("args", ()),
-            kwargs=kwargs.pop("kwargs", {}),
+            task=task,
+            signature=FunctionSignature(
+                inputs=kwargs.pop("inputs", {}),
+                outputs=kwargs.pop("outputs", {}),
+                func_or_cls=func_or_cls,
+                init_args=kwargs.pop("init_args", ()),
+                init_kwargs=kwargs.pop("init_kwargs", {}),
+                method_name=kwargs.pop("method_name", None),
+            ),
         )
+        cls.get()._registry[ModelSpec.get_id(spec.name, spec.task)] = spec
         logger.debug(f"Registered model: [name={model_name}]")
 
 
 # Alias methods
 list = Hub.list
 load = Hub.load
 register = Hub.register
```

## nos/models/clip.py

```diff
@@ -2,37 +2,47 @@
 from typing import List, Union
 
 import numpy as np
 import torch
 from PIL import Image
 
 from nos import hub
+from nos.common import EmbeddingSpec, TaskType
+from nos.common.types import Batch, ImageT, TensorT
 from nos.hub import HuggingFaceHubConfig
 
 
 @dataclass(frozen=True)
 class CLIPConfig(HuggingFaceHubConfig):
-    pass
+    D: int = 512
 
 
 class CLIP:
     """CLIP model for image and text encoding."""
 
     configs = {
+        "openai/clip": CLIPConfig(
+            model_name="openai/clip-vit-base-patch32",
+            D=512,
+        ),
         "openai/clip-vit-base-patch32": CLIPConfig(
             model_name="openai/clip-vit-base-patch32",
+            D=512,
         ),
         "openai/clip-vit-large-patch14": CLIPConfig(
             model_name="openai/clip-vit-large-patch14",
+            D=768,
         ),
         "laion/CLIP-ViT-H-14-laion2B-s32B-b79K": CLIPConfig(
             model_name="laion/CLIP-ViT-H-14-laion2B-s32B-b79K",
+            D=1024,
         ),
         "laion/CLIP-ViT-L-14-laion2B-s32B-b82K": CLIPConfig(
             model_name="laion/CLIP-ViT-L-14-laion2B-s32B-b82K",
+            D=768,
         ),
     }
 
     def __init__(self, model_name: str = "openai/clip-vit-base-patch32"):
         from transformers import CLIPModel, CLIPProcessor, CLIPTokenizer
 
         self.cfg = CLIP.configs.get(model_name)
@@ -40,30 +50,50 @@
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
         self.model = CLIPModel.from_pretrained(model_name).to(self.device)
         self.model.eval()
         self.tokenizer = CLIPTokenizer.from_pretrained(model_name)
         self.processor = CLIPProcessor.from_pretrained(model_name)
 
     def encode_image(self, images: Union[Image.Image, np.ndarray, List[Image.Image], List[np.ndarray]]) -> np.ndarray:
+        """Encode image into an embedding."""
         with torch.inference_mode():
+            if isinstance(images, (np.ndarray, Image.Image)):
+                images = [images]
             inputs = self.processor(images=images, return_tensors="pt").to(self.device)
             image_features = self.model.get_image_features(**inputs)
             return image_features.cpu().numpy()
 
-    def encode_text(self, text: Union[str, List[str]]) -> np.ndarray:
+    def encode_text(self, texts: Union[str, List[str]]) -> np.ndarray:
+        """Encode text into an embedding."""
         with torch.inference_mode():
-            if isinstance(text, str):
-                text = [
-                    text,
-                ]
+            if isinstance(texts, str):
+                texts = [texts]
             inputs = self.tokenizer(
-                text,
+                texts,
                 padding=True,
                 return_tensors="pt",
             ).to(self.device)
             text_features = self.model.get_text_features(**inputs)
             return text_features.cpu().numpy()
 
 
-# Register all CLIP models
+# Register all CLIP models (for both tasks img2vec and txt2vec)
 for model_name in CLIP.configs:
-    hub.register(model_name, "txt2vec", CLIP, args=(model_name,))
+    cfg = CLIP.configs[model_name]
+    hub.register(
+        model_name,
+        TaskType.TEXT_EMBEDDING,
+        CLIP,
+        init_args=(model_name,),
+        method_name="encode_text",
+        inputs={"texts": Batch[str]},
+        outputs={"embedding": Batch[TensorT[np.ndarray, EmbeddingSpec(shape=(cfg.D,), dtype="float32")]]},
+    )
+    hub.register(
+        model_name,
+        TaskType.IMAGE_EMBEDDING,
+        CLIP,
+        init_args=(model_name,),
+        method_name="encode_image",
+        inputs={"images": Batch[ImageT[Image.Image]]},
+        outputs={"embedding": Batch[TensorT[np.ndarray, EmbeddingSpec(shape=(cfg.D,), dtype="float32")]]},
+    )
```

## nos/models/faster_rcnn.py

```diff
@@ -3,14 +3,16 @@
 
 import numpy as np
 import torch
 import torchvision.transforms.functional as F
 from PIL import Image
 
 from nos import hub
+from nos.common import ImageSpec, TaskType, TensorSpec
+from nos.common.types import Batch, ImageT, TensorT
 from nos.hub import TorchHubConfig
 
 
 @dataclass(frozen=True)
 class FasterRCNNConfig(TorchHubConfig):
     pass
 
@@ -53,11 +55,24 @@
                 "labels": predictions[0]["labels"].cpu().numpy(),
                 "bboxes": predictions[0]["boxes"].cpu().numpy(),
             }
 
 
 hub.register(
     "torchvision/fasterrcnn_mobilenet_v3_large_320_fpn",
-    "img2bbox",
+    TaskType.OBJECT_DETECTION_2D,
     FasterRCNN,
-    args=("torchvision/fasterrcnn_mobilenet_v3_large_320_fpn",),
+    init_args=("torchvision/fasterrcnn_mobilenet_v3_large_320_fpn",),
+    method_name="predict",
+    inputs={
+        "images": Union[
+            Batch[ImageT[Image.Image, ImageSpec(shape=(480, 640, 3), dtype="uint8")], 8],
+            Batch[ImageT[Image.Image, ImageSpec(shape=(960, 1280, 3), dtype="uint8")], 4],
+            Batch[ImageT[Image.Image, ImageSpec(shape=(1080, 1920, 3), dtype="uint8")], 1],
+        ]
+    },
+    outputs={
+        "scores": Batch[TensorT[np.ndarray, TensorSpec(shape=(None), dtype="float32")]],
+        "labels": Batch[TensorT[np.ndarray, TensorSpec(shape=(None), dtype="float32")]],
+        "bboxes": Batch[TensorT[np.ndarray, TensorSpec(shape=(None, 4), dtype="float32")]],
+    },
 )
```

## nos/models/stable_diffusion.py

```diff
@@ -1,13 +1,15 @@
-from typing import List
+from typing import List, Union
 
 import torch
 from PIL import Image
 
 from nos import hub
+from nos.common import TaskType
+from nos.common.types import Batch, ImageSpec, ImageT
 
 
 class StableDiffusion2:
     """StableDiffusion model for text to image generation."""
 
     def __init__(
         self,
@@ -45,38 +47,45 @@
         self.pipe.enable_attention_slicing()
 
         # TODO (spillai): Pending xformers integration
         # self.pipe.enable_xformers_memory_efficient_attention()
 
     def __call__(
         self,
-        prompt: str,
+        prompts: Union[str, List[str]],
         num_images: int = 1,
         num_inference_steps: int = 50,
         guidance_scale: float = 7.5,
         height: int = None,
         width: int = None,
     ) -> List[Image.Image]:
+        """Generate images from text prompt."""
+        if isinstance(prompts, str):
+            prompts = [prompts]
         with torch.inference_mode():
             with torch.autocast("cuda"):
-                return self.pipe(
-                    [prompt] * num_images,
+                images = self.pipe(
+                    prompts * num_images,
                     num_inference_steps=num_inference_steps,
                     guidance_scale=guidance_scale,
                     height=height,
                     width=width,
                 ).images
+                return images
 
 
 # Register the model with the hub
 # TODO (spillai): Ideally, we should do this via a decorator
 # @hub.register("stabilityai/stable-diffusion-2")
 # def stable_diffusion_2_ddim_fp16():
 #     return StableDiffusion2("stabilityai/stable-diffusion-2", scheduler="ddim", dtype=torch.float16)
 #
 hub.register(
     "stabilityai/stable-diffusion-2",
-    "txt2img",
+    TaskType.IMAGE_GENERATION,
     StableDiffusion2,
-    args=("stabilityai/stable-diffusion-2",),
-    kwargs={"scheduler": "ddim", "dtype": torch.float16},
+    init_args=("stabilityai/stable-diffusion-2",),
+    init_kwargs={"scheduler": "ddim", "dtype": torch.float16},
+    method_name="__call__",
+    inputs={"prompts": Batch[str], "num_images": int, "height": int, "width": int},
+    outputs={"images": Batch[ImageT[Image.Image, ImageSpec(shape=(None, None, 3), dtype="uint8")]]},
 )
```

## nos/models/openmmlab/mmdetection/mmdetection.py

```diff
@@ -2,15 +2,14 @@
 from pathlib import Path
 from typing import Dict, List, Union
 
 import numpy as np
 import torch
 from PIL import Image
 
-from nos import hub
 from nos.hub import MMLabConfig
 
 
 @dataclass(frozen=True)
 class MMDetectionConfig(MMLabConfig):
     score_threshold: float = 0.3
 
@@ -54,20 +53,16 @@
             return {
                 "scores": predictions.pred_instances.scores.cpu().numpy(),
                 "labels": predictions.pred_instances.labels.cpu().numpy(),
                 "bboxes": predictions.pred_instances.bboxes.cpu().numpy(),
             }
 
 
-hub.register(
-    "open-mmlab/efficientdet-d3",
-    "img2bbox",
-    MMDetection,
-    args=("open-mmlab/efficientdet-d3",),
-)
-
-hub.register(
-    "open-mmlab/faster-rcnn",
-    "img2bbox",
-    MMDetection,
-    args=("open-mmlab/faster-rcnn",),
-)
+# TODO (spillai): Skip registration until new mmlab docker runtime is available
+# for model_name in MMDetection.configs:
+#     hub.register(
+#         model_name,
+#         TaskType.OBJECT_DETECTION_2D,
+#         MMDetection,
+#         init_args=(model_name,),
+#         method_name="predict",
+#     )
```

## nos/proto/nos_service.proto

```diff
@@ -1,82 +1,94 @@
 syntax = "proto3";
 
 import "google/protobuf/empty.proto";
 
 package nos.inference;
 
 
-message ModelListResponse {
-  repeated string models = 1;
-}
-
-
-message ModelInfoRequest {
-  string model_name = 1;
-}
-
-message ModelInfoResponse {
-}
-
-
+// Base text request
 message TextRequest {
   string text = 1;
 }
 
 
+// Base image request
 message ImageRequest {
   bytes image_bytes = 1;
 }
 
 
-message InitModelRequest {
-  string model_name = 1;
-  optional int32 num_replicas = 2;
+// Model information
+message ModelInfo {
+  // Task identifier (e.g. "image_generation", "image_embedding", "object_detection" etc)
+  string task = 1;
+  // Model identifier (e.g. "openai/clip-vit-large-patch14")
+  string name = 2;
 }
 
-
-message InitModelResponse {
-  string result = 1;
+// ModelList response
+message ModelListResponse {
+  repeated ModelInfo models = 1;
 }
 
+// Model information request
+message ModelInfoRequest {
+  ModelInfo request = 1;
+}
 
-message DeleteModelRequest {
-  string model_name = 1;
+// Model information response
+// Note (spillai): We cloudpickle `ModelSpec` and return the bytes.
+message ModelInfoResponse {
+  bytes response_bytes = 1;
 }
 
+// Inference request specification
+// Note (spillai): We cloudpickle the input dictionary values (image, etc)
+// and do not support any other serialization methods.
+message InferenceRequest {
+  ModelInfo model = 1;
+  map <string, bytes> inputs = 2;
+}
 
-message DeleteModelResponse {
-  string result = 1;
+// Inference response specification
+// Note (spillai): We serialize all the outputs with cloudpickle
+// and do not support any other serialization methods.
+message InferenceResponse {
+  bytes response_bytes = 1;
 }
 
 
-message InferenceRequest {
-  string method = 1;
-  string model_name = 2;
-  oneof request {
-    TextRequest text_request = 3;
-    ImageRequest image_request = 4;
-  }
+// Ping / healthcheck response
+message PingResponse {
+    string status = 1;  // (e.g. "ok" or "not_ok")
 }
 
-
-message InferenceResponse {
-  bytes result = 1;
+// Service information repsonse
+message ServiceInfoResponse {
+    string version = 1;  // (e.g. "0.1.0")
 }
 
 // Service definition
 service InferenceService {
-  // List available models from Hugging Face Hub
-  rpc ListModels(google.protobuf.Empty) returns (ModelListResponse) {};
+  // Check health status of the inference server.
+  rpc Ping(google.protobuf.Empty) returns (PingResponse) {}
 
-  // Load model from Hugging Face Hub
-  rpc InitModel(InitModelRequest) returns (InitModelResponse) {}
+  // Get service information (version, release date etc.)
+  rpc GetServiceInfo(google.protobuf.Empty) returns (ServiceInfoResponse) {}
 
-  // Delete model from deployment
-  rpc DeleteModel(DeleteModelRequest) returns (DeleteModelResponse) {}
+  // List available models from Hugging Face Hub
+  rpc ListModels(google.protobuf.Empty) returns (ModelListResponse) {};
 
   // Get model information from the deployment
   rpc GetModelInfo(ModelInfoRequest) returns (ModelInfoResponse) {};
 
-  // Perform text-to-vector prediction
-  rpc Predict(InferenceRequest) returns (InferenceResponse) {}
+  // Run the inference request
+  rpc Run(InferenceRequest) returns (InferenceResponse) {}
+
+  // Load model from Hugging Face Hub
+  // TODO (spillai): To be implemented later (for power-users)
+  // rpc InitModel(InitModelRequest) returns (InitModelResponse) {}
+
+  // Delete model from deployment
+  // TODO (spillai): To be implemented later (for power-users)
+  // rpc DeleteModel(DeleteModelRequest) returns (DeleteModelResponse) {}
 }
```

## nos/server/__init__.py

```diff
@@ -1,10 +0,0 @@
-00000000: 6672 6f6d 202e 7365 7276 6963 6520 696d  from .service im
-00000010: 706f 7274 2049 6e66 6572 656e 6365 5365  port InferenceSe
-00000020: 7276 6963 6520 2023 206e 6f71 6120 4634  rvice  # noqa F4
-00000030: 3031 0a66 726f 6d20 2e72 756e 7469 6d65  01.from .runtime
-00000040: 2069 6d70 6f72 7420 496e 6665 7265 6e63   import Inferenc
-00000050: 6553 6572 7669 6365 5275 6e74 696d 6520  eServiceRuntime 
-00000060: 2023 206e 6f71 6120 4634 3031 0a66 726f   # noqa F401.fro
-00000070: 6d20 2e64 6f63 6b65 7220 696d 706f 7274  m .docker import
-00000080: 2044 6f63 6b65 7252 756e 7469 6d65 2020   DockerRuntime  
-00000090: 2320 6e6f 7161 2046 3430 310a            # noqa F401.
```

## nos/server/runtime.py

```diff
@@ -56,15 +56,15 @@
             command=[NOS_GRPC_SERVER_CMD],
             ports={DEFAULT_GRPC_PORT: DEFAULT_GRPC_PORT},
             environment={
                 "NOS_LOGGING_LEVEL": LOGGING_LEVEL,
             },
             volumes={
                 str(Path.home() / ".nosd"): {"bind": "/app/.nos", "mode": "rw"},
-                str(Path.home() / ".nosd" / "tmp"): {"bind": "/tmp", "mode": "rw"},
+                "/tmp": {"bind": "/tmp", "mode": "rw"},
             },
             shm_size=shm_size,
             detach=detach,
             remove=True,
             gpu=gpu,
             **kwargs,
         )
```

## nos/server/service.py

```diff
@@ -1,28 +1,29 @@
 from collections import OrderedDict
 from dataclasses import dataclass
 from typing import Union
 
-import cloudpickle
 import grpc
 import numpy as np
 import ray
 import rich.console
 import rich.status
 import torch
 from google.protobuf import empty_pb2
 from PIL import Image
 
 from nos import hub
+from nos.common import dumps
 from nos.constants import DEFAULT_GRPC_PORT  # noqa F401
 from nos.exceptions import ModelNotFoundError
 from nos.executors.ray import RayExecutor
-from nos.hub import MethodType, ModelSpec
+from nos.hub import ModelSpec, TaskType
 from nos.logging import logger
 from nos.protoc import import_module
+from nos.version import __version__
 
 
 nos_service_pb2 = import_module("nos_service_pb2")
 nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
 
 
 class FixedLengthFIFODict(OrderedDict):
@@ -51,15 +52,15 @@
 
     spec: ModelSpec
     """Model specification."""
     handle: Union[ray.remote, ray.actor.ActorHandle]
     """Ray actor handle."""
 
 
-class InferenceService(nos_service_pb2_grpc.InferenceServiceServicer):
+class InferenceServiceImpl(nos_service_pb2_grpc.InferenceServiceServicer):
     """
     Experimental gRPC-based inference service.
 
     This service is used to serve models over gRPC.
 
     Refer to the bring-your-own-schema section:
     https://docs.ray.io/en/master/serve/direct-ingress.html?highlight=grpc#bring-your-own-schema
@@ -70,144 +71,169 @@
         self.executor = RayExecutor.get()
         try:
             self.executor.init()
         except Exception as e:
             logger.info(f"Failed to initialize executor: {e}")
             raise RuntimeError(f"Failed to initialize executor: {e}")
 
-    def init_model(self, model_name: str):
+    @logger.catch
+    def init_model(self, model_name: str, task: TaskType = None):
         """Initialize the model."""
         assert model_name not in self.model_handle, f"Model already initialized: {model_name}"
-
         # Load the model spec
         try:
-            spec = hub.load_spec(model_name)
+            spec: ModelSpec = hub.load_spec(model_name, task=task)
             logger.debug(f"Loaded model spec: {spec}")
         except Exception as e:
             raise ModelNotFoundError(f"Failed to load model spec: {model_name}, {e}")
 
         # If the model handle is full, pop the oldest model
         if len(self.model_handle) >= self.model_handle.maxlen:
-            spec = self.model_handle.popitem(last=False)
-            self.delete_model(spec.model_name)
+            spec: ModelSpec = self.model_handle.popitem(last=False)
+            self.delete_model(spec.name, task=spec.task)
             logger.info(f"Deleting oldest model: {model_name}")
         logger.info(f"Initializing model: {model_name}")
 
         # Create the serve deployment from the model handle
-        model_cls = spec.cls
+        model_cls = spec.signature.func_or_cls
         actor_options = {"num_gpus": 1 if torch.cuda.is_available() else 0}
         logger.debug(f"Creating actor: {actor_options}")
         actor_cls = ray.remote(**actor_options)(model_cls)
-        # TOOD(spillai): Currently only one model per model-name is supported.
-        self.model_handle[spec.name] = ModelHandle(spec, actor_cls.remote(*spec.args, **spec.kwargs))
-        logger.info(f"Created actor: {self.model_handle[spec.name]}, type={type(self.model_handle[spec.name])}")
+        # Note: Currently one model per (model-name, task) is supported.
+        self.model_handle[spec.id] = ModelHandle(
+            spec, actor_cls.remote(*spec.signature.init_args, **spec.signature.init_kwargs)
+        )
+        logger.info(f"Created actor: {self.model_handle[spec.id]}, type={type(self.model_handle[spec.id])}")
         logger.info(f"Models ({len(self.model_handle)}): {self.model_handle.keys()}")
 
-    def delete_model(self, model_name: str):
+    @logger.catch
+    def delete_model(self, model_str: str, task: TaskType = None):
         """Delete the model."""
-        assert model_name in self.model_handle, f"Model not initialized: {model_name}"
+        model_id = ModelSpec.get_id(model_str, task=task)
+        assert model_id in self.model_handle, f"Model not initialized: {model_id}"
 
-        logger.info(f"Deleting model: {model_name}")
-        model_handle = self.model_handle[model_name]
+        logger.info(f"Deleting model: {model_id}")
+        model_handle = self.model_handle[model_id]
         ray.kill(model_handle.handle)
-        self.model_handle.pop(model_name)
-        logger.info(f"Deleted model: {model_name}")
+        self.model_handle.pop(model_id)
+        logger.info(f"Deleted model: {model_id}")
+
+    @logger.catch
+    def Ping(self, request: empty_pb2.Empty, context: grpc.ServicerContext) -> nos_service_pb2.PingResponse:
+        """Health check."""
+        return nos_service_pb2.PingResponse(status="ok")
+
+    @logger.catch
+    def GetServiceInfo(
+        self, request: empty_pb2.Empty, context: grpc.ServicerContext
+    ) -> nos_service_pb2.ServiceInfoResponse:
+        """Get information on the service."""
+        return nos_service_pb2.ServiceInfoResponse(version=__version__)
 
+    @logger.catch
     def ListModels(self, request: empty_pb2.Empty, context: grpc.ServicerContext) -> nos_service_pb2.ModelListResponse:
         """List all models."""
-        return nos_service_pb2.ModelListResponse(models=hub.list())
-
-    def InitModel(
-        self, request: nos_service_pb2.InitModelRequest, context: grpc.ServicerContext
-    ) -> nos_service_pb2.InitModelResponse:
-        """Initialize the model."""
-        if request.model_name in self.model_handle:
-            return nos_service_pb2.InitModelResponse(result="ok")
-
-        # Load the model spec
-        try:
-            self.init_model(request.model_name)
-        except Exception as e:
-            context.abort(context, grpc.StatusCode.NOT_FOUND, str(e))
-        return nos_service_pb2.InitModelResponse(result="ok")
-
-    def DeleteModel(
-        self, request: nos_service_pb2.DeleteModelRequest, context: grpc.ServicerContext
-    ) -> nos_service_pb2.DeleteModelResponse:
-        """Delete the model."""
-        self.delete_model(request.model_name)
-        return nos_service_pb2.DeleteModelResponse(result="ok")
+        response = nos_service_pb2.ModelListResponse()
+        for spec in hub.list():
+            response.models.append(nos_service_pb2.ModelInfo(name=spec.name, task=spec.task.value))
+        return response
 
+    @logger.catch
     def GetModelInfo(
         self, request: nos_service_pb2.ModelInfoRequest, context: grpc.ServicerContext
     ) -> nos_service_pb2.ModelInfoResponse:
         """Get model information."""
-        raise NotImplementedError()
+        try:
+            model_info = request.request
+            spec: ModelSpec = hub.load_spec(model_info.name, task=TaskType(model_info.task))
+        except KeyError as e:
+            context.abort(context, grpc.StatusCode.NOT_FOUND, str(e))
+        return nos_service_pb2.ModelInfoResponse(
+            response_bytes=dumps(spec),
+        )
 
-    def Predict(
+    @logger.catch
+    def Run(
         self, request: nos_service_pb2.InferenceRequest, context: grpc.ServicerContext
     ) -> nos_service_pb2.InferenceResponse:
         """Main model prediction interface."""
-        logger.debug(f"Received request: {request.method}, {request.model_name}")
-        if request.model_name not in self.model_handle:
-            self.init_model(request.model_name)
-
-        # TODO (spillai): This is inconsistent for CLIP which supports both (txt2vec, img2vec)
-        # assert self.model_spec.method.value == request.method
-        handle = self.model_handle.get(request.model_name).handle
-
-        if request.method == MethodType.TXT2IMG.value:
-            prompt = request.text_request.text
-            logger.debug(f"Generating image with prompt: {prompt}")
-            response_ref = handle.__call__.remote(prompt, height=512, width=512)
-            (img,) = ray.get(response_ref)
-            ref_bytes = cloudpickle.dumps({"image": img}, protocol=4)
-            return nos_service_pb2.InferenceResponse(result=ref_bytes)
-
-        elif request.method == MethodType.TXT2VEC.value:
-            prompt = request.text_request.text
-            logger.debug(f"Encoding text: {prompt}")
-            response_ref = handle.encode_text.remote(prompt)
+        model_request = request.model
+        logger.debug(f"Received request: {model_request.task}, {model_request.name}")
+
+        model_id = ModelSpec.get_id(model_request.name, task=TaskType(model_request.task))
+        if model_id not in self.model_handle:
+            self.init_model(model_request.name, TaskType(model_request.task))
+
+        # Get the model handle (model_spec, actor_handle)
+        model_handle: ModelHandle = self.model_handle[model_id]
+        model_spec: ModelSpec = model_handle.spec
+        # TODO (spillai): Validate the inputs
+        model_inputs = model_spec.signature.decode_inputs(request.inputs)
+        actor_handle = model_handle.handle
+        # Get the method function (i.e. `__call__`, or `predict`)
+        actor_method_func = getattr(actor_handle, model_spec.signature.method_name)
+        logger.debug(f"Actor method function: {actor_method_func}")
+        logger.debug(f"Actor handle: {actor_handle}")
+        logger.debug(f"Model spec: {model_spec}")
+
+        if model_request.task == TaskType.IMAGE_GENERATION.value:
+            prompts = model_inputs["prompts"]
+            logger.debug(f"Generating image with prompt: {prompts}")
+
+            response_ref = actor_method_func.remote(prompts, height=512, width=512)
+            images = ray.get(response_ref)
+
+            assert "images" in model_spec.signature.outputs
+            return nos_service_pb2.InferenceResponse(response_bytes=dumps({"images": images}))
+
+        elif model_request.task == TaskType.TEXT_EMBEDDING.value:
+            texts = model_inputs["texts"]
+            logger.debug(f"Encoding text: {texts}")
+
+            response_ref = actor_method_func.remote(texts)
             embedding = ray.get(response_ref)
-            ref_bytes = cloudpickle.dumps({"embedding": embedding}, protocol=4)
-            return nos_service_pb2.InferenceResponse(result=ref_bytes)
 
-        elif request.method == MethodType.IMG2VEC.value:
-            img: Union[np.ndarray, Image.Image] = cloudpickle.loads(request.image_request.image_bytes)
-            logger.debug(f"Encoding img (type={type(img)})")
+            assert "embedding" in model_spec.signature.outputs
+            return nos_service_pb2.InferenceResponse(response_bytes=dumps({"embedding": embedding}))
+
+        elif model_request.task == TaskType.IMAGE_EMBEDDING.value:
+            images: Union[np.ndarray, Image.Image] = model_inputs["images"]
+            logger.debug(f"Encoding images (type={type(images)})")
 
-            response_ref = handle.encode_image.remote(img)
+            response_ref = actor_method_func.remote(images)
             embedding = ray.get(response_ref)
-            ref_bytes = cloudpickle.dumps({"embedding": embedding}, protocol=4)
-            return nos_service_pb2.InferenceResponse(result=ref_bytes)
 
-        elif request.method == MethodType.IMG2BBOX.value:
-            img: Union[np.ndarray, Image.Image] = cloudpickle.loads(request.image_request.image_bytes)
-            logger.debug(f"Encoding img (type={type(img)})")
+            assert "embedding" in model_spec.signature.outputs
+            return nos_service_pb2.InferenceResponse(response_bytes=dumps({"embedding": embedding}))
 
-            response_ref = handle.predict.remote(img)
+        elif model_request.task == TaskType.OBJECT_DETECTION_2D.value:
+            images: Union[np.ndarray, Image.Image] = model_inputs["images"]
+            logger.debug(f"Encoding images (type={type(images)})")
+
+            response_ref = actor_method_func.remote(images)
             prediction = ray.get(response_ref)
-            # prediction: {'scores': np.ndarray, 'labels': np.ndarray, 'bboxes': np.ndarray}
-            ref_bytes = cloudpickle.dumps(prediction, protocol=4)
-            return nos_service_pb2.InferenceResponse(result=ref_bytes)
+
+            for key in prediction.keys():
+                assert key in model_spec.signature.outputs
+            return nos_service_pb2.InferenceResponse(response_bytes=dumps(prediction))
         else:
             context.abort(context, grpc.StatusCode.INVALID_ARGUMENT, f"Invalid method {request.method}")
 
 
 def serve(address: str = f"[::]:{DEFAULT_GRPC_PORT}", max_workers: int = 1) -> None:
     """Start the gRPC server."""
     from concurrent import futures
 
     options = [
         ("grpc.max_message_length", 512 * 1024 * 1024),
         ("grpc.max_send_message_length", 512 * 1024 * 1024),
         ("grpc.max_receive_message_length", 512 * 1024 * 1024),
     ]
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=max_workers), options=options)
-    nos_service_pb2_grpc.add_InferenceServiceServicer_to_server(InferenceService(), server)
+    nos_service_pb2_grpc.add_InferenceServiceServicer_to_server(InferenceServiceImpl(), server)
     server.add_insecure_port(address)
 
     console = rich.console.Console()
     with console.status(f"[bold green] Starting server on {address}[/bold green]") as status:
         server.start()
         console.print(
             f"[bold green] ✓ InferenceService :: Deployment complete [/bold green]",  # noqa
```

## nos/test/conftest.py

```diff
@@ -1,48 +1,187 @@
+import time
 from concurrent import futures
+from pathlib import Path
 
 import grpc
 import pytest
+from loguru import logger
 
-from nos.client import DEFAULT_GRPC_PORT, InferenceClient
-from nos.executors.ray import RayExecutor
+from nos.constants import DEFAULT_GRPC_PORT
 from nos.protoc import import_module
-from nos.server import InferenceService
 
 
 GRPC_TEST_PORT = DEFAULT_GRPC_PORT + 1
+GRPC_TEST_PORT_CPU = DEFAULT_GRPC_PORT + 2
+GRPC_TEST_PORT_GPU = DEFAULT_GRPC_PORT + 3
+CPU_CONTAINER_NAME = "nos-grpc-server-cpu-test"
+GPU_CONTAINER_NAME = "nos-grpc-server-gpu-test"
 
 nos_service_pb2 = import_module("nos_service_pb2")
 nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
 
 
 @pytest.fixture(scope="session")
 def ray_executor():
+    from nos.executors.ray import RayExecutor
+
     executor = RayExecutor.get()
     executor.init()
 
     yield executor
 
     executor.stop()
 
 
 @pytest.fixture(scope="session")
-def test_grpc_server():
+def grpc_server():
+    """Test gRPC server (Port: 50052)."""
     from loguru import logger
 
+    from nos.server.service import InferenceServiceImpl
+
     logger.info(f"Starting gRPC test server on port: {GRPC_TEST_PORT}")
     options = [
         ("grpc.max_message_length", 512 * 1024 * 1024),
         ("grpc.max_send_message_length", 512 * 1024 * 1024),
         ("grpc.max_receive_message_length", 512 * 1024 * 1024),
     ]
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=1), options=options)
-    nos_service_pb2_grpc.add_InferenceServiceServicer_to_server(InferenceService(), server)
+    nos_service_pb2_grpc.add_InferenceServiceServicer_to_server(InferenceServiceImpl(), server)
     server.add_insecure_port(f"[::]:{GRPC_TEST_PORT}")
     server.start()
     yield server
     server.stop(grace=None)
 
 
-@pytest.fixture(scope="function")
-def test_grpc_client():
+@pytest.fixture(scope="session")
+def grpc_client():
+    """Test gRPC client (Port: 50052)."""
+    from nos.client import InferenceClient
+
     yield InferenceClient(f"localhost:{GRPC_TEST_PORT}")
+
+
+@pytest.fixture(scope="session")
+def grpc_client_cpu():
+    """Test gRPC client to be used with CPU docker runtime (Port: 50053)."""
+    from nos.client import InferenceClient
+
+    yield InferenceClient(f"localhost:{GRPC_TEST_PORT_CPU}")
+
+
+@pytest.fixture(scope="session")
+def grpc_client_gpu():
+    """Test gRPC client to be used with GPU docker runtime (Port: 50054)."""
+    from nos.client import InferenceClient
+
+    yield InferenceClient(f"localhost:{GRPC_TEST_PORT_GPU}")
+
+
+@pytest.fixture(scope="session")
+def grpc_server_docker_runtime_cpu():
+    """Test DockerRuntime CPU (Port: 50053)."""
+    from nos.server.docker import DockerRuntime
+    from nos.server.runtime import NOS_DOCKER_IMAGE_CPU, NOS_GRPC_SERVER_CMD
+
+    docker_runtime = DockerRuntime.get()
+
+    # Force stop any existing containers
+    try:
+        docker_runtime.stop(CPU_CONTAINER_NAME)
+    except Exception:
+        logger.info(f"Killing any existing container with name: {CPU_CONTAINER_NAME}")
+
+    # Start grpc server runtime (CPU)
+    container = docker_runtime.start(
+        image=NOS_DOCKER_IMAGE_CPU,
+        container_name=CPU_CONTAINER_NAME,
+        command=[NOS_GRPC_SERVER_CMD],
+        ports={DEFAULT_GRPC_PORT: GRPC_TEST_PORT_CPU},
+        environment={
+            "NOS_LOGGING_LEVEL": "DEBUG",
+        },
+        volumes={
+            str(Path.home() / ".nosd_test"): {"bind": "/app/.nos", "mode": "rw"},
+            "/tmp": {"bind": "/tmp", "mode": "rw"},
+        },
+        detach=True,
+        gpu=False,
+    )
+    assert container is not None
+    assert container.id is not None
+
+    # Get container and status
+    container_ = docker_runtime.get_container(CPU_CONTAINER_NAME)
+    status = docker_runtime.get_container_status(CPU_CONTAINER_NAME)
+    assert container_.id == container.id
+    assert status is not None
+    assert status == "running"
+
+    yield container
+
+    # Tear down (raise errors if this fails)
+    docker_runtime.stop(CPU_CONTAINER_NAME)
+
+    # Wait for container to stop (up to 20 seconds)
+    st = time.time()
+    while time.time() - st <= 20:
+        status = docker_runtime.get_container_status(CPU_CONTAINER_NAME)
+        if status == "exited" or status is None:
+            break
+        time.sleep(1)
+    assert status is None or status == "exited"
+
+
+@pytest.fixture(scope="session")
+def grpc_server_docker_runtime_gpu():
+    """Test DockerRuntime GPU (Port: 50054)."""
+    from nos.server.docker import DockerRuntime
+    from nos.server.runtime import NOS_DOCKER_IMAGE_GPU, NOS_GRPC_SERVER_CMD
+
+    docker_runtime = DockerRuntime.get()
+
+    # Force stop any existing containers
+    try:
+        docker_runtime.stop(GPU_CONTAINER_NAME)
+    except Exception:
+        logger.info(f"Killing any existing container with name: {GPU_CONTAINER_NAME}")
+
+    # Start grpc server runtime (GPU)
+    container = docker_runtime.start(
+        image=NOS_DOCKER_IMAGE_GPU,
+        container_name=GPU_CONTAINER_NAME,
+        command=[NOS_GRPC_SERVER_CMD],
+        ports={DEFAULT_GRPC_PORT: GRPC_TEST_PORT_GPU},
+        environment={
+            "NOS_LOGGING_LEVEL": "DEBUG",
+        },
+        volumes={
+            str(Path.home() / ".nosd_test"): {"bind": "/app/.nos", "mode": "rw"},
+            "/tmp": {"bind": "/tmp", "mode": "rw"},
+        },
+        detach=True,
+        gpu=True,
+    )
+    assert container is not None
+    assert container.id is not None
+
+    # Get container and status
+    container_ = docker_runtime.get_container(GPU_CONTAINER_NAME)
+    status = docker_runtime.get_container_status(GPU_CONTAINER_NAME)
+    assert container_.id == container.id
+    assert status is not None
+    assert status == "running"
+
+    yield container
+
+    # Tear down (raise errors if this fails)
+    docker_runtime.stop(GPU_CONTAINER_NAME)
+
+    # Wait for container to stop (up to 20 seconds)
+    st = time.time()
+    while time.time() - st <= 20:
+        status = docker_runtime.get_container_status(GPU_CONTAINER_NAME)
+        if status == "exited" or status is None:
+            break
+        time.sleep(1)
+    assert status is None or status == "exited"
```

## nos/test/utils.py

```diff
@@ -1,13 +1,12 @@
 """Various test utilities."""
 from enum import Enum
 from pathlib import Path
 
 import pytest
-import torch
 
 
 NOS_TEST_DATA_DIR = Path(__file__).parent.parent.parent / "tests/test_data"
 NOS_TEST_IMAGE = NOS_TEST_DATA_DIR / "test.jpg"
 NOS_TEST_VIDEO = NOS_TEST_DATA_DIR / "test.mp4"
 NOS_TEST_AUDIO = NOS_TEST_DATA_DIR / "test_speech.flac"
 
@@ -24,14 +23,16 @@
 
 def skip_if_no_torch_cuda(test_case):
     """Decorator marking a test that requires torch cuda devices.
 
     These tests are skipped when torch.cuda.is_available() is set to False. If
     `CUDA_VISIBLE_DEVICES=""` then, the decorated test is not run.
     """
+    import torch
+
     return pytest.mark.skipif(not torch.cuda.is_available(), reason="Requires CUDA")(test_case)
 
 
 def skip_all_if_no_torch_cuda():
     """Decorator sugar to mark all tests in a file that requires torch cuda devices.
 
     Usage:
@@ -39,8 +40,10 @@
         To mark all tests in a file that requires torch cuda devices,
         add the following:
 
         ```python
         pytestmark = skip_all_if_no_torch_cuda()
         ```
     """
+    import torch
+
     return pytest.mark.skipif(not torch.cuda.is_available(), reason="Requires CUDA")
```

## Comparing `autonomi_nos-0.0.3.dist-info/LICENSE` & `autonomi_nos-0.0.4a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `autonomi_nos-0.0.3.dist-info/METADATA` & `autonomi_nos-0.0.4a0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomi-nos
-Version: 0.0.3
+Version: 0.0.4a0
 Summary: Nitrous oxide system (NOS) for computer-vision.
 License: MIT License
         
         Copyright (c) 2023 Autonomi AI
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -39,23 +39,21 @@
 License-File: LICENSE
 Requires-Dist: av (>=10.0.0)
 Requires-Dist: cloudpickle (>=2.2.1)
 Requires-Dist: docker (>=6.0.0)
 Requires-Dist: grpcio-tools (<=1.49.1,>=1.32.0)
 Requires-Dist: loguru (>=0.7.0)
 Requires-Dist: opencv-python-headless (>=4.6.0.66)
-Requires-Dist: pandas
+Requires-Dist: Pillow
 Requires-Dist: psutil (>=5.9.5)
+Requires-Dist: pydantic
 Requires-Dist: rich (>=12.5.1)
+Requires-Dist: tqdm
 Requires-Dist: typer (>=0.7.0)
-Requires-Dist: diffusers
-Requires-Dist: huggingface-hub
-Requires-Dist: pyarrow (>=12.0.0)
-Requires-Dist: ray[serve] (>=2.4.0)
-Requires-Dist: transformers (>=4.28.1)
+Requires-Dist: typing-extensions (>=4.5.0)
 Provides-Extra: dev
 Requires-Dist: black[jupyter] (==22.3.0) ; extra == 'dev'
 Requires-Dist: build (==0.10.0) ; extra == 'dev'
 Requires-Dist: pre-commit (==3.2.2) ; extra == 'dev'
 Requires-Dist: ruff (==0.0.262) ; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs ; extra == 'docs'
@@ -63,18 +61,26 @@
 Requires-Dist: mkdocs-include-markdown-plugin ; extra == 'docs'
 Requires-Dist: mkdocs-material ; extra == 'docs'
 Requires-Dist: mkdocs-pymdownx-material-extras ; extra == 'docs'
 Requires-Dist: mkdocs-same-dir ; extra == 'docs'
 Requires-Dist: mkdocstrings ; extra == 'docs'
 Requires-Dist: mkdocstrings-python ; extra == 'docs'
 Requires-Dist: mkdocstrings[python] ; extra == 'docs'
+Provides-Extra: server
+Requires-Dist: diffusers ; extra == 'server'
+Requires-Dist: huggingface-hub ; extra == 'server'
+Requires-Dist: pyarrow (>=12.0.0) ; extra == 'server'
+Requires-Dist: ray[serve] (>=2.4.0) ; extra == 'server'
+Requires-Dist: transformers (>=4.28.1) ; extra == 'server'
+Requires-Dist: torch (<2.0.0,>=1.12.1) ; extra == 'server'
+Requires-Dist: torchaudio (>=0.13.1) ; extra == 'server'
+Requires-Dist: torchvision (>=0.13.0) ; extra == 'server'
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-asyncio ; extra == 'test'
-Requires-Dist: pytest-xdist ; extra == 'test'
 Requires-Dist: typeguard ; extra == 'test'
 Provides-Extra: torch
 Requires-Dist: torch (<2.0.0,>=1.12.1) ; extra == 'torch'
 Requires-Dist: torchaudio (>=0.13.1) ; extra == 'torch'
 Requires-Dist: torchvision (>=0.13.0) ; extra == 'torch'
 
 # nos 🔥: Nitrous Oxide System (NOS) for Computer Vision
```

### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: autonomi-nos Version: 0.0.3 Summary: Nitrous oxide
-system (NOS) for computer-vision. License: MIT License Copyright (c) 2023
+Metadata-Version: 2.1 Name: autonomi-nos Version: 0.0.4a0 Summary: Nitrous
+oxide system (NOS) for computer-vision. License: MIT License Copyright (c) 2023
 Autonomi AI Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
 above copyright notice and this permission notice shall be included in all
@@ -21,34 +21,38 @@
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering :: Image
 Processing Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Requires-Python: >=3.7.10 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: av (>=10.0.0) Requires-Dist: cloudpickle
 (>=2.2.1) Requires-Dist: docker (>=6.0.0) Requires-Dist: grpcio-tools
 (<=1.49.1,>=1.32.0) Requires-Dist: loguru (>=0.7.0) Requires-Dist: opencv-
-python-headless (>=4.6.0.66) Requires-Dist: pandas Requires-Dist: psutil
-(>=5.9.5) Requires-Dist: rich (>=12.5.1) Requires-Dist: typer (>=0.7.0)
-Requires-Dist: diffusers Requires-Dist: huggingface-hub Requires-Dist: pyarrow
-(>=12.0.0) Requires-Dist: ray[serve] (>=2.4.0) Requires-Dist: transformers
-(>=4.28.1) Provides-Extra: dev Requires-Dist: black[jupyter] (==22.3.0) ; extra
-== 'dev' Requires-Dist: build (==0.10.0) ; extra == 'dev' Requires-Dist: pre-
-commit (==3.2.2) ; extra == 'dev' Requires-Dist: ruff (==0.0.262) ; extra ==
-'dev' Provides-Extra: docs Requires-Dist: mkdocs ; extra == 'docs' Requires-
-Dist: mkdocs-exclude ; extra == 'docs' Requires-Dist: mkdocs-include-markdown-
-plugin ; extra == 'docs' Requires-Dist: mkdocs-material ; extra == 'docs'
-Requires-Dist: mkdocs-pymdownx-material-extras ; extra == 'docs' Requires-Dist:
-mkdocs-same-dir ; extra == 'docs' Requires-Dist: mkdocstrings ; extra == 'docs'
+python-headless (>=4.6.0.66) Requires-Dist: Pillow Requires-Dist: psutil
+(>=5.9.5) Requires-Dist: pydantic Requires-Dist: rich (>=12.5.1) Requires-Dist:
+tqdm Requires-Dist: typer (>=0.7.0) Requires-Dist: typing-extensions (>=4.5.0)
+Provides-Extra: dev Requires-Dist: black[jupyter] (==22.3.0) ; extra == 'dev'
+Requires-Dist: build (==0.10.0) ; extra == 'dev' Requires-Dist: pre-commit
+(==3.2.2) ; extra == 'dev' Requires-Dist: ruff (==0.0.262) ; extra == 'dev'
+Provides-Extra: docs Requires-Dist: mkdocs ; extra == 'docs' Requires-Dist:
+mkdocs-exclude ; extra == 'docs' Requires-Dist: mkdocs-include-markdown-plugin
+; extra == 'docs' Requires-Dist: mkdocs-material ; extra == 'docs' Requires-
+Dist: mkdocs-pymdownx-material-extras ; extra == 'docs' Requires-Dist: mkdocs-
+same-dir ; extra == 'docs' Requires-Dist: mkdocstrings ; extra == 'docs'
 Requires-Dist: mkdocstrings-python ; extra == 'docs' Requires-Dist:
-mkdocstrings[python] ; extra == 'docs' Provides-Extra: test Requires-Dist:
+mkdocstrings[python] ; extra == 'docs' Provides-Extra: server Requires-Dist:
+diffusers ; extra == 'server' Requires-Dist: huggingface-hub ; extra ==
+'server' Requires-Dist: pyarrow (>=12.0.0) ; extra == 'server' Requires-Dist:
+ray[serve] (>=2.4.0) ; extra == 'server' Requires-Dist: transformers (>=4.28.1)
+; extra == 'server' Requires-Dist: torch (<2.0.0,>=1.12.1) ; extra == 'server'
+Requires-Dist: torchaudio (>=0.13.1) ; extra == 'server' Requires-Dist:
+torchvision (>=0.13.0) ; extra == 'server' Provides-Extra: test Requires-Dist:
 pytest ; extra == 'test' Requires-Dist: pytest-asyncio ; extra == 'test'
-Requires-Dist: pytest-xdist ; extra == 'test' Requires-Dist: typeguard ; extra
-== 'test' Provides-Extra: torch Requires-Dist: torch (<2.0.0,>=1.12.1) ; extra
-== 'torch' Requires-Dist: torchaudio (>=0.13.1) ; extra == 'torch' Requires-
-Dist: torchvision (>=0.13.0) ; extra == 'torch' # nos ð¥: Nitrous Oxide
-System (NOS) for Computer Vision
+Requires-Dist: typeguard ; extra == 'test' Provides-Extra: torch Requires-Dist:
+torch (<2.0.0,>=1.12.1) ; extra == 'torch' Requires-Dist: torchaudio (>=0.13.1)
+; extra == 'torch' Requires-Dist: torchvision (>=0.13.0) ; extra == 'torch' #
+nos ð¥: Nitrous Oxide System (NOS) for Computer Vision
            [PyPi_Version] [PyPi_Version] [PyPi_Downloads] [Discord]
 **NOS** is a PyTorch library for optimizing and running lightning-fast
 inference of popular computer vision models. NOS inherits its name from
 "Nitrous Oxide System", the performance-enhancing system typically used in
 racing cars. NOS is designed to be modular and easy to extend. ## Why NOS? -
 â¡ï¸ **Fast**: Built for PyTorch and designed to optimize/run models faster -
 ð¥ **Performant**: Run models such as SDv2 or object detection 2-3x faster
```

## Comparing `autonomi_nos-0.0.3.dist-info/RECORD` & `autonomi_nos-0.0.4a0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,57 @@
-nos/__init__.py,sha256=ON7r9-nhUByFaRhC-pr-NcTHa2zdd4fuJUsWwTVQiB0,119
+nos/__init__.py,sha256=51Y_o2LsEI8SmKeCFOZfz1aTYOCqrv8plfrpDyr_ILo,50
 nos/constants.py,sha256=j-nz48q31rE7eclMqkZH6xFJ0eGmtx2Jt5yr_wQA_1Y,561
 nos/exceptions.py,sha256=ocRCxTbzT_Q8WTobAbkbo4jl5a6F3xC_D2N7rtzfWeg,93
 nos/logging.py,sha256=D0QDNFGmAYshfnSC-ctEDSIeBO6TnLPz1babUmJGRSA,940
 nos/protoc.py,sha256=xUck1U30UqUEnTaFuWMGWagyDcIrjmcQo8xozqbypmI,2778
-nos/version.py,sha256=4GZKi13lDTD25YBkGakhZyEQZWTER_OWQMNPoH_UM2c,22
+nos/version.py,sha256=rJdPE5XDOIi-BiClP-ph78BgHXH62hS9N_VMAlrufd0,23
 nos/cli/benchmark.py,sha256=p-EGzEUDMFFv2hpB9Nn8-Xk1zW-hrYDaUzyNvWmSgzk,110
 nos/cli/cli.py,sha256=nO0Eg_zp7L6xt5ST0QteypNHky8TIms8JSOLsvtHhjY,455
 nos/cli/docker.py,sha256=uPGrLe8FlvwSNFGUqp-vw5VAZhCeyvrfUfwJZdqXypk,1983
 nos/cli/hub.py,sha256=USdzVgaZlPZABrrIZzCA7ySwXg1iseEk7GJ7iwanXIg,1294
-nos/cli/serve_grpc.py,sha256=XUxyCcyLkRg9psbhcydCq45V7WgOG7oUH-vF9EEipGE,6094
+nos/cli/serve_grpc.py,sha256=ymFv5qfehj5jNnEOiku-Kp5oqjMUbl7pzG4eVYP3KhE,6202
 nos/cli/serve_http.py,sha256=xMwSE46-_uHLgif1gnJCRoLbBE3ttC2zkm2JXVooWg0,5962
 nos/cli/system.py,sha256=gFm8ngxyxcPThhjkgB8S8ZBmtYBcqLdSo4unaWTl0N8,3479
 nos/cli/utils.py,sha256=uR1lGZyyDEuflNvxKuAmVUP-DTE55PzZL5c0c3l2h4U,425
-nos/client/__init__.py,sha256=u-xpiMdEMYNPzarLAbjDx2KlLCq4XaqpkhqzcMdKTcU,141
+nos/client/__init__.py,sha256=-J19VTXOiv9joF7SwPpoUW4_nBwq5_cBp8A1ghhFg70,372
 nos/client/exceptions.py,sha256=Lqqeu_6oNSZgOUipXHFx20yeASJi9bEewpG1UYuy1gk,92
-nos/client/grpc.py,sha256=3A-3vpk4FFx3kUi9aGzJP_Mn_sAbPQkaM6yRgbtDK3g,7307
+nos/client/grpc.py,sha256=mY0YT9n8DwsvvKX8kJBu8yHJ8ayoXt844T__3i9BTXE,12657
+nos/common/__init__.py,sha256=83smCPabdvR79BJB3iiGQ2rg1a_hYhUwgPVfw4iXgOQ,286
+nos/common/spec.py,sha256=9ypTvsmUO_9yZ9zfyc7_uzLr4MJ72aXEvBGogEVsGVc,3715
+nos/common/tasks.py,sha256=AcEbh5gbpKt_77Ar9zRrRyiD8tyw264Wv2buyX9yxZ8,518
+nos/common/types.py,sha256=PgE1M1FdOhEc6AurFBAXrWk-j_br_pyR2scHasX3sLM,4851
+nos/examples/vid2bbox.py,sha256=UNEYmxI5RILgpOz14m2LEr-WJdgrdHnFeIIsN91k88E,3470
 nos/executors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nos/executors/ray.py,sha256=wxbKvIMinQODTVm0zUlKpCcmj9TkGxNpmlAL3k7vvoE,6237
-nos/hub/__init__.py,sha256=1gZVEGB5dD-QfDTKB1hGiYMBDEa5kmbfiYOcOUYd4hM,2985
+nos/executors/ray.py,sha256=aurGem2kgMMCdV-38kN6ozsNMbmKuIh4ywDEIuWNkBk,7401
+nos/experimental/conversion_flows/openmmlab/tensorrt/run_model.py,sha256=A8LoCm4YvApkw_AAAyGqNLKeAoqzK1xvBy4pLI_Y9TE,1246
+nos/experimental/http/__init__.py,sha256=5LrWYhbfJy60b1eHj_p5gq7huQqFxxt_ThErTEkrKyc,4559
+nos/experimental/http/client.py,sha256=IwsHUg1qQxf8dntIlRSHeabm3_akICgj2LtqzKxMCU8,1153
+nos/experimental/http/ingress.py,sha256=ih6GzTaFHDVxUPUJa0640A78WAY2COHpiZyHnlMFl6M,2605
+nos/experimental/http/service.py,sha256=cZvJ0cOnTr89oFioH9QrEaR3UGZDA3uq2TNgdSYPj7g,2688
+nos/hub/__init__.py,sha256=XqZ9yVrSnNGEPNfsc7pk6N0XS2nuiabZtEvaDtBbH8Y,3436
 nos/hub/config.py,sha256=DK0t6xrB6Sgf71YWnX_htNbbU4H2Bcdu9b7ujiA6QKY,2195
-nos/hub/spec.py,sha256=vC6DDYo0F1PVX9EYGMdnhFDKH7emRBX-Z0JJm54Slwc,902
 nos/models/__init__.py,sha256=FMoBv4glDtKz1eCIvqOy0RDqWM6w0fP7fdT_NJR8Q3k,242
-nos/models/clip.py,sha256=TVeCvHOe-1KfQI0e7CZu0SLIGQusMEI6EM7Z9IgVDDg,2370
-nos/models/faster_rcnn.py,sha256=Wnjdq-B5qZqqgMu3PzHCR2ga8LPGKR5FqaaQYs5MCJw,2028
-nos/models/stable_diffusion.py,sha256=pDc_3PJr7k5rOJuelcGD7i5zCcurQ02lkpfc0TaaUqw,2651
-nos/models/openmmlab/mmdetection/detection_tensorrt_dynamic-320x320-1344x1344.py,sha256=YFx2dzUKL2MkS5mIqw6gDO1TxLkwLIWEFVOxwHIhnYg,66
-nos/models/openmmlab/mmdetection/mmdetection.py,sha256=BFyy-H6EwP3ZvuOgpiEmmn8R0p-sSOdfBIDHMY6Kbms,2589
+nos/models/clip.py,sha256=ggVFUagLMZNA7N7U-sdvCGNRx4gF4qoW7C4Emjje6J0,3460
+nos/models/faster_rcnn.py,sha256=3q3COMvNDXYQLnWHLSfDLBnwq7X37YjKmPgloBSMM8s,2804
+nos/models/stable_diffusion.py,sha256=q--CdCy0QLCEV5kfHOK8FOrUoQUhg63D6pVsdRnMLi4,3150
+nos/models/openmmlab/mmdetection/mmdetection.py,sha256=8M_30LRPv3UcrUuLq7MDB3UtKJPE_Ide5NhvfbBG1kM,2628
 nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py,sha256=tAbybUUg9TtBy_dqiXD5Zgl0kSs39JX7TiTeIYZrOUo,370
 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py,sha256=MxNi_Sf1m8CNkR64vZWaFN2O2P2LBI1-EexpLr166YU,3187
 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_instance.py,sha256=DVkj2zskGrXxiF6hVQ1ofsOsqQGHsdjAh5sXRkaxjiw,1765
 nos/models/openmmlab/mmdetection/configs/_base_/models/faster-rcnn_r50_fpn.py,sha256=Al2qpY2P-MzsfBCod5pjB6HrH7ZzFvQxICc1CVmpnRY,3828
 nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py,sha256=G8gXisLhM7mBRlxrhTOLCsWD17zCyH7kBvVi7J4BICI,304
 nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py,sha256=RSkd9o1IO-YkWhIwnXU83tRyGeySiR1IMlSk14dTw9s,5340
 nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py,sha256=Cm8lyQ3wOT5I9KR0m1TfTsPAGybs-buILRPLDZKzOPQ,177
-nos/proto/nos_service.proto,sha256=akx6q6f7aYjsIvwINPZR93SBjncHapG__ibQHYgwyTA,1409
-nos/server/__init__.py,sha256=kdNIS7NMSFz_ooJC3ZXzTjjS2VHb0me5SiPPFSrOu4U,156
+nos/proto/nos_service.proto,sha256=BEWdRsehHLaSjH2K2QEhtmaDqkwDZYdxKm1t4yg_0V8,2437
+nos/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nos/server/docker.py,sha256=Wbob_pkHXKdMWliD2VTWw1U7R7dojBImYWZTeSNDfLY,6229
-nos/server/runtime.py,sha256=nW2oAYfySqxVcH7B1Np0JZHqkqKFG6SjtMdtfEZOVbo,3004
-nos/server/service.py,sha256=GweoeaDgHY8RLIMSa8HrpqIjdbGJfnRDolEU815slfQ,8880
+nos/server/runtime.py,sha256=BzQsaMCBAxC73xfj2AR6RCjfWWOWwMQBAU0gxKut8rI,2976
+nos/server/service.py,sha256=CEmaKrdp-8f_Bdcxr70xGO8EXYJH3fuYCv_SQVtVf7Y,9887
 nos/test/benchmark.py,sha256=b_QMHfStY5iRjHGPZwaY7VrXzy_VeFKfjld9UEVbn-g,373
-nos/test/conftest.py,sha256=psIsMxzB9g8jgUokP_q6sJ-SZuTYTZSxBtfyYb0hSc8,1317
-nos/test/utils.py,sha256=qZbEN85EhUNBF3BAUTW_dStMCsPwrdosSRlkQp-ShX0,1324
-autonomi_nos-0.0.3.dist-info/LICENSE,sha256=9TQFxQ2AkXOQuIHy9GueB_a18hayRXT7pDt9fJv9WLo,1068
-autonomi_nos-0.0.3.dist-info/METADATA,sha256=a12iqcMfV1vlmTUyyKgPndkj_GXdn0ScgN-GwRMrUu4,5917
-autonomi_nos-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-autonomi_nos-0.0.3.dist-info/entry_points.txt,sha256=UYtJAmFT3RPWmlKM11MMZvZPRHTeKyIh1BbZ3QpbsJs,86
-autonomi_nos-0.0.3.dist-info/top_level.txt,sha256=Tgqk49XI1nXvi6W_Ryy7_YwQ7iFU-mAlIsbNMR1HS6s,4
-autonomi_nos-0.0.3.dist-info/RECORD,,
+nos/test/conftest.py,sha256=-mZNh-D-LsalJ5oL0NOW1B7G88o0W6rJ8dwNA08N8Ys,5764
+nos/test/utils.py,sha256=F8RTOZKIuYPguUOz3beERNbmCg3pYjvLFwS7bMp6ejw,1347
+autonomi_nos-0.0.4a0.dist-info/LICENSE,sha256=9TQFxQ2AkXOQuIHy9GueB_a18hayRXT7pDt9fJv9WLo,1068
+autonomi_nos-0.0.4a0.dist-info/METADATA,sha256=-oR1BExuNhspEPyQCDDULzn0YiuFkmJowgcU_NbQrWc,6257
+autonomi_nos-0.0.4a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+autonomi_nos-0.0.4a0.dist-info/entry_points.txt,sha256=UYtJAmFT3RPWmlKM11MMZvZPRHTeKyIh1BbZ3QpbsJs,86
+autonomi_nos-0.0.4a0.dist-info/top_level.txt,sha256=RgOntmzdTkyrY-Fj9H6bSke7af3bHLscoZnK1-7Aa8o,12
+autonomi_nos-0.0.4a0.dist-info/RECORD,,
```

