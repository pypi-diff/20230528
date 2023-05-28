# Comparing `tmp/onnx-tool-0.6.5.tar.gz` & `tmp/onnx-tool-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-tool-0.6.5.tar", last modified: Wed May 17 12:45:58 2023, max compression
+gzip compressed data, was "onnx-tool-0.7.0.tar", last modified: Sun May 28 06:38:14 2023, max compression
```

## Comparing `onnx-tool-0.6.5.tar` & `onnx-tool-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 12:45:58.846095 onnx-tool-0.6.5/
--rw-rw-rw-   0        0        0     1092 2022-06-28 15:38:19.000000 onnx-tool-0.6.5/LICENSE
--rw-rw-rw-   0        0        0    10353 2023-05-17 12:45:58.846095 onnx-tool-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     9894 2023-05-17 12:36:11.000000 onnx-tool-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 12:45:58.839529 onnx-tool-0.6.5/onnx_tool/
--rw-rw-rw-   0        0        0    15585 2023-04-10 11:33:26.000000 onnx-tool-0.6.5/onnx_tool/__init__.py
--rw-rw-rw-   0        0        0     3028 2023-02-07 11:56:14.000000 onnx-tool-0.6.5/onnx_tool/__main__.py
--rw-rw-rw-   0        0        0    11847 2023-04-10 11:33:26.000000 onnx-tool-0.6.5/onnx_tool/fusion.py
--rw-rw-rw-   0        0        0    51652 2023-05-17 12:36:11.000000 onnx-tool-0.6.5/onnx_tool/graph.py
--rw-rw-rw-   0        0        0    61561 2023-05-17 12:36:11.000000 onnx-tool-0.6.5/onnx_tool/node.py
--rw-rw-rw-   0        0        0     6433 2023-05-11 15:44:28.000000 onnx-tool-0.6.5/onnx_tool/serialization.py
--rw-rw-rw-   0        0        0    15948 2023-04-19 13:20:48.000000 onnx-tool-0.6.5/onnx_tool/tensor.py
--rw-rw-rw-   0        0        0     3685 2023-05-17 12:40:01.000000 onnx-tool-0.6.5/onnx_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 12:45:58.844530 onnx-tool-0.6.5/onnx_tool.egg-info/
--rw-rw-rw-   0        0        0    10353 2023-05-17 12:45:58.000000 onnx-tool-0.6.5/onnx_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-05-17 12:45:58.000000 onnx-tool-0.6.5/onnx_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 12:45:58.000000 onnx-tool-0.6.5/onnx_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-17 12:45:58.000000 onnx-tool-0.6.5/onnx_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 12:45:58.000000 onnx-tool-0.6.5/onnx_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-06-28 15:40:35.000000 onnx-tool-0.6.5/onnx_tool.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-05-17 12:45:58.846095 onnx-tool-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0      989 2023-05-17 12:45:46.000000 onnx-tool-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:38:14.404531 onnx-tool-0.7.0/
+-rw-rw-rw-   0        0        0     1092 2022-06-28 15:38:19.000000 onnx-tool-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0    10735 2023-05-28 06:38:14.404531 onnx-tool-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10276 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 06:38:14.398530 onnx-tool-0.7.0/onnx_tool/
+-rw-rw-rw-   0        0        0    14841 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/__init__.py
+-rw-rw-rw-   0        0        0     3051 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/__main__.py
+-rw-rw-rw-   0        0        0    11847 2023-04-10 11:33:26.000000 onnx-tool-0.7.0/onnx_tool/fusion.py
+-rw-rw-rw-   0        0        0    57383 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/graph.py
+-rw-rw-rw-   0        0        0    73170 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/node.py
+-rw-rw-rw-   0        0        0     6433 2023-05-11 15:44:28.000000 onnx-tool-0.7.0/onnx_tool/serialization.py
+-rw-rw-rw-   0        0        0    15758 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/tensor.py
+-rw-rw-rw-   0        0        0     3685 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/onnx_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 06:38:14.403530 onnx-tool-0.7.0/onnx_tool.egg-info/
+-rw-rw-rw-   0        0        0    10735 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-28 06:38:14.000000 onnx-tool-0.7.0/onnx_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-06-28 15:40:35.000000 onnx-tool-0.7.0/onnx_tool.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-28 06:38:14.404531 onnx-tool-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-05-28 05:20:29.000000 onnx-tool-0.7.0/setup.py
```

### Comparing `onnx-tool-0.6.5/LICENSE` & `onnx-tool-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.6.5/PKG-INFO` & `onnx-tool-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-Metadata-Version: 2.1
-Name: onnx-tool
-Version: 0.6.5
-Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
-Home-page: https://github.com/ThanatosShinji/onnx-tool
-Author: Luo Yu
-Author-email: luoyu888888@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a href="README_CN.md">简体中文</a>
 # onnx-tool
 
 **A tool for ONNX model:**
 
 * *Rapid shape inference.*
 * *Profile model.*
+* *<a href="data/ConstantFolding.md">Constant Folding.</a>*
 * *Compute Graph and Shape Engine.*
 * *OPs fusion.*
 * *Activation memory compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT, LLaMa, MPT(<a href="benchmark/transfomer_models.py">TransformerModel</a>)
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
-* CV: Resnet, MobileNet, YOLO, ...
-* Audio: LPCNet
+* CV: <a href="benchmark/compression.py">BEVFormer</a>, MobileNet, YOLO, ...
+* Audio: sovits, LPCNet
 
 ---
 
 ## Shape inference
 
 <p align="center">  
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/shape_inference.jpg">
@@ -97,15 +86,15 @@
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
 BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
-
+Help implement model parallelism.
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_subgraph.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
@@ -153,30 +142,31 @@
 Then `pip install onnx-tool` again.
 
 
 ---
 
 ## Known Issues
 * Loop op is not supported
-
+* Activation Compression is not optimum
+  
 ---
 
 ## Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
 Some models have dynamic input shapes. The MACs varies from input shapes. The input shapes used in these results are writen to [data/public/config.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py).
 These onnx models with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ 
 )(code: p91k) [google drive](https://drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 <p id="results" align="center">
 <table>
 <tr>
 <td>
 
 Model | Params(M) | MACs(M)
 ---|---|---
-GPT-J 1 layer | 464 | 173,398  
-MPT 1 layer | 261 | 79,894
+<a href="benchmark/transfomer_models.py">GPT-J 1 layer</a> | 464 | 173,398  
+<a href="benchmark/transfomer_models.py">MPT 1 layer</a> | 261 | 79,894
 [text_encoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main)| 123.13 | 6,782
 [UNet2DCondition](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main)| 859.52 | 888,870
 [VAE_encoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main) | 34.16 | 566,371
 [VAE_decoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main) | 49.49 | 1,271,959
 [SqueezeNet 1.0](https://github.com/onnx/models/tree/main/vision/classification/squeezenet) | 1.23 | 351
 [AlexNet](https://github.com/onnx/models/tree/main/vision/classification/alexnet) | 60.96 | 665
 [GoogleNet](https://github.com/onnx/models/tree/main/vision/classification/inception_and_googlenet/googlenet) | 6.99 | 1,606
@@ -188,29 +178,29 @@
 [Emotion](https://github.com/onnx/models/tree/main/vision/body_analysis/emotion_ferplus) | 12.95 | 877
 [Mask R-CNN](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/mask-rcnn) | 46.77 | 92,077
 </td>
 
 <td>
 
 Model | Params(M) | MACs(M)
----|---|---
-LLaMa 1 layer | 618 | 211,801  
-[rvm_mobilenetv3](https://github.com/PeterL1n/RobustVideoMatting) | 3.73 | 4,289
-[yolov4](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/yolov4) | 64.33 | 3,319
-[ConvNeXt-L](https://github.com/facebookresearch/ConvNeXt) | 229.79 | 34,872
-[edgenext_small](https://github.com/mmaaz60/EdgeNeXt) | 5.58 | 1,357
-[SSD](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/ssd) | 19.98 | 216,598
-[RealESRGAN](https://github.com/xinntao/Real-ESRGAN) | 16.69 | 73,551
-[ShuffleNet](https://github.com/onnx/models/tree/main/vision/classification/shufflenet) | 2.29 | 146
-[GPT-2](https://github.com/onnx/models/tree/main/text/machine_comprehension/gpt-2) | 137.02 | 1,103
-[T5-encoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 109.62 | 686
-[T5-decoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 162.62 | 1,113
-[RoBERTa-BASE](https://github.com/onnx/models/tree/main/text/machine_comprehension/roberta) | 124.64 | 688
-[Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10 | 46,018
-[FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29 | 37,056
-[MobileNet](https://github.com/onnx/models/blob/main/vision/classification/mobilenet) | 3.3 | 300
-[ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25 | 3,868
+---|-----------|---
+<a href="benchmark/transfomer_models.py">LLaMa 1 layer</a> | 618       | 211,801  
+[BEVFormer Tiny](https://github.com/DerryHub/BEVFormer_tensorrt) | 33.7      | 210,838
+[rvm_mobilenetv3](https://github.com/PeterL1n/RobustVideoMatting) | 3.73      | 4,289
+[yolov4](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/yolov4) | 64.33     | 3,319
+[ConvNeXt-L](https://github.com/facebookresearch/ConvNeXt) | 229.79    | 34,872
+[edgenext_small](https://github.com/mmaaz60/EdgeNeXt) | 5.58      | 1,357
+[SSD](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/ssd) | 19.98     | 216,598
+[RealESRGAN](https://github.com/xinntao/Real-ESRGAN) | 16.69     | 73,551
+[ShuffleNet](https://github.com/onnx/models/tree/main/vision/classification/shufflenet) | 2.29      | 146
+[GPT-2](https://github.com/onnx/models/tree/main/text/machine_comprehension/gpt-2) | 137.02    | 1,103
+[T5-encoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 109.62    | 686
+[T5-decoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 162.62    | 1,113
+[RoBERTa-BASE](https://github.com/onnx/models/tree/main/text/machine_comprehension/roberta) | 124.64    | 688
+[Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10     | 46,018
+[FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29     | 37,056
+[ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25        | 3,868
 
 </td>
 </tr>
 </table>
-</p>
+</p>
```

#### html2text {}

```diff
@@ -1,19 +1,13 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.6.5 Summary: A tool for ONNX
-model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
-fusion;Quantized models and sparse models are supported. Home-page: https://
-github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
-luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
-:: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
-# onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
-model.* * *Compute Graph and Shape Engine.* * *OPs fusion.* * *Activation
-memory compression.* * *Quantized models and sparse models are supported.*
-Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT(TransformerModel) *
-Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV: Resnet, MobileNet,
-YOLO, ... * Audio: LPCNet --- ## Shape inference
+ç®ä½ä¸­æ # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.*
+* *Profile model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* *
+*OPs fusion.* * *Activation memory compression.* * *Quantized models and sparse
+models are supported.* Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT
+(TransformerModel) * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV:
+BEVFormer, MobileNet, YOLO, ... * Audio: sovits, LPCNet --- ## Shape inference
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              shape_inference.jpg]
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/data/Profile.md). pytorch usage: [data/PytorchUsage.md](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md). tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/TensorflowUsage.md). samples: [benchmark/samples.py](https://
@@ -54,15 +48,15 @@
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               resnet18_fused.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). BERT samples: [benchmark/samples.py](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/
 onnx-tool/blob/main/benchmark/do_fusion.py). --- ## Extract subgraph from ONNX
-model
+model Help implement model parallelism.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                             resnet18_subgraph.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). --- ## Memory Compression For large language
 models and high-resolution CV models, the activation memory compression is a
 key to save memory. The compression method achieves 5% memory compression on
 most models. For example: model | Native Memory Size(MB) | Compressed Memory
@@ -78,62 +72,63 @@
 set its static weight tensors as its input tensors* * *Set custom input and
 output tensors' name and dimension, change model from fixed input to dynamic
 input* how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-
 tool/blob/main/data/Tensors.md). --- ## How to install `pip install onnx-tool`
 OR `pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
 python>=3.6 If `pip install onnx-tool` failed by onnx's installation, you may
 try `pip install onnx==1.8.1` (a lower version like this) first. Then `pip
-install onnx-tool` again. --- ## Known Issues * Loop op is not supported --- ##
-Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
-Some models have dynamic input shapes. The MACs varies from input shapes. The
-input shapes used in these results are writen to [data/public/config.py](https:
-//github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These
-onnx models with all tensors' shape can be downloaded: [baidu drive](https://
-pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
+install onnx-tool` again. --- ## Known Issues * Loop op is not supported *
+Activation Compression is not optimum --- ## Results of [ONNX Model Zoo](https:
+//github.com/onnx/models) and SOTA models Some models have dynamic input
+shapes. The MACs varies from input shapes. The input shapes used in these
+results are writen to [data/public/config.py](https://github.com/
+ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These onnx models
+with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/
+s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
 drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 Model | Params(M) | MACs(M) ---|---|--
-- GPT-J 1 layer | 464 | 173,398 MPT 1   Model | Params(M) | MACs(M) ---|---|--
-layer | 261 | 79,894 [text_encoder]     - LLaMa 1 layer | 618 | 211,801
-(https://huggingface.co/bes-dev/stable- [rvm_mobilenetv3](https://github.com/
-diffusion-v1-4-onnx/tree/main)| 123.13  PeterL1n/RobustVideoMatting) | 3.73 |
-| 6,782 [UNet2DCondition](https://      4,289 [yolov4](https://github.com/onnx/
-huggingface.co/bes-dev/stable-          models/tree/main/vision/
-diffusion-v1-4-onnx/tree/main)| 859.52  object_detection_segmentation/yolov4) |
-| 888,870 [VAE_encoder](https://        64.33 | 3,319 [ConvNeXt-L](https://
-huggingface.co/bes-dev/stable-          github.com/facebookresearch/ConvNeXt) |
-diffusion-v1-4-onnx/tree/main) | 34.16  229.79 | 34,872 [edgenext_small](https:
-| 566,371 [VAE_decoder](https://        //github.com/mmaaz60/EdgeNeXt) | 5.58 |
-huggingface.co/bes-dev/stable-          1,357 [SSD](https://github.com/onnx/
-diffusion-v1-4-onnx/tree/main) | 49.49  models/tree/main/vision/
-| 1,271,959 [SqueezeNet 1.0](https://   object_detection_segmentation/ssd) |
+- GPT-J_1_layer | 464 | 173,398 MPT_1   Model | Params(M) | MACs(M) ---|-------
+layer | 261 | 79,894 [text_encoder]     ----|--- LLaMa_1_layer | 618 | 211,801
+(https://huggingface.co/bes-dev/stable- [BEVFormer Tiny](https://github.com/
+diffusion-v1-4-onnx/tree/main)| 123.13  DerryHub/BEVFormer_tensorrt) | 33.7 |
+| 6,782 [UNet2DCondition](https://      210,838 [rvm_mobilenetv3](https://
+huggingface.co/bes-dev/stable-          github.com/PeterL1n/RobustVideoMatting)
+diffusion-v1-4-onnx/tree/main)| 859.52  | 3.73 | 4,289 [yolov4](https://
+| 888,870 [VAE_encoder](https://        github.com/onnx/models/tree/main/
+huggingface.co/bes-dev/stable-          vision/object_detection_segmentation/
+diffusion-v1-4-onnx/tree/main) | 34.16  yolov4) | 64.33 | 3,319 [ConvNeXt-L]
+| 566,371 [VAE_decoder](https://        (https://github.com/facebookresearch/
+huggingface.co/bes-dev/stable-          ConvNeXt) | 229.79 | 34,872
+diffusion-v1-4-onnx/tree/main) | 49.49  [edgenext_small](https://github.com/
+| 1,271,959 [SqueezeNet 1.0](https://   mmaaz60/EdgeNeXt) | 5.58 | 1,357 [SSD]
+github.com/onnx/models/tree/main/       (https://github.com/onnx/models/tree/
+vision/classification/squeezenet) |     main/vision/
+1.23 | 351 [AlexNet](https://           object_detection_segmentation/ssd) |
 github.com/onnx/models/tree/main/       19.98 | 216,598 [RealESRGAN](https://
-vision/classification/squeezenet) |     github.com/xinntao/Real-ESRGAN) | 16.69
-1.23 | 351 [AlexNet](https://           | 73,551 [ShuffleNet](https://
-github.com/onnx/models/tree/main/       github.com/onnx/models/tree/main/
-vision/classification/alexnet) | 60.96  vision/classification/shufflenet) |
-| 665 [GoogleNet](https://github.com/   2.29 | 146 [GPT-2](https://github.com/
-onnx/models/tree/main/vision/           onnx/models/tree/main/text/
-classification/inception_and_googlenet/ machine_comprehension/gpt-2) | 137.02 |
-googlenet) | 6.99 | 1,606               1,103 [T5-encoder](https://github.com/
+vision/classification/alexnet) | 60.96  github.com/xinntao/Real-ESRGAN) | 16.69
+| 665 [GoogleNet](https://github.com/   | 73,551 [ShuffleNet](https://
+onnx/models/tree/main/vision/           github.com/onnx/models/tree/main/
+classification/inception_and_googlenet/ vision/classification/shufflenet) |
+googlenet) | 6.99 | 1,606               2.29 | 146 [GPT-2](https://github.com/
 [googlenet_age](https://github.com/     onnx/models/tree/main/text/
-onnx/models/tree/main/vision/           machine_comprehension/t5) | 109.62 |
-body_analysis/age_gender) | 5.98 |      686 [T5-decoder](https://github.com/
+onnx/models/tree/main/vision/           machine_comprehension/gpt-2) | 137.02 |
+body_analysis/age_gender) | 5.98 |      1,103 [T5-encoder](https://github.com/
 1,605 [LResNet100E-IR](https://         onnx/models/tree/main/text/
-github.com/onnx/models/tree/main/       machine_comprehension/t5) | 162.62 |
-vision/body_analysis/arcface) | 65.22 | 1,113 [RoBERTa-BASE](https://
-12,102 [BERT-Squad](https://github.com/ github.com/onnx/models/tree/main/text/
-onnx/models/tree/main/text/             machine_comprehension/roberta) | 124.64
-machine_comprehension/bert-squad) |     | 688 [Faster R-CNN](https://
-113.61 | 22,767 [BiDAF](https://        github.com/onnx/models/blob/main/
-github.com/onnx/models/tree/main/text/  vision/object_detection_segmentation/
-machine_comprehension/                  faster-rcnn) | 44.10 | 46,018 [FCN
-bidirectional_attention_flow) | 18.08 | ResNet-50](https://github.com/onnx/
-9.87 [EfficientNet-Lite4](https://      models/tree/main/vision/
-github.com/onnx/models/tree/main/       object_detection_segmentation/fcn) |
-vision/classification/efficientnet-     35.29 | 37,056 [MobileNet](https://
-lite4) | 12.96 | 1,361 [Emotion](https: github.com/onnx/models/blob/main/
-//github.com/onnx/models/tree/main/     vision/classification/mobilenet) | 3.3
-vision/body_analysis/emotion_ferplus) | | 300 [ResNet50](https://github.com/
-12.95 | 877 [Mask R-CNN](https://       onnx/models/tree/main/vision/
-github.com/onnx/models/tree/main/       classification/resnet) | 25 | 3,868
-vision/object_detection_segmentation/
+github.com/onnx/models/tree/main/       machine_comprehension/t5) | 109.62 |
+vision/body_analysis/arcface) | 65.22 | 686 [T5-decoder](https://github.com/
+12,102 [BERT-Squad](https://github.com/ onnx/models/tree/main/text/
+onnx/models/tree/main/text/             machine_comprehension/t5) | 162.62 |
+machine_comprehension/bert-squad) |     1,113 [RoBERTa-BASE](https://
+113.61 | 22,767 [BiDAF](https://        github.com/onnx/models/tree/main/text/
+github.com/onnx/models/tree/main/text/  machine_comprehension/roberta) | 124.64
+machine_comprehension/                  | 688 [Faster R-CNN](https://
+bidirectional_attention_flow) | 18.08 | github.com/onnx/models/blob/main/
+9.87 [EfficientNet-Lite4](https://      vision/object_detection_segmentation/
+github.com/onnx/models/tree/main/       faster-rcnn) | 44.10 | 46,018 [FCN
+vision/classification/efficientnet-     ResNet-50](https://github.com/onnx/
+lite4) | 12.96 | 1,361 [Emotion](https: models/tree/main/vision/
+//github.com/onnx/models/tree/main/     object_detection_segmentation/fcn) |
+vision/body_analysis/emotion_ferplus) | 35.29 | 37,056 [ResNet50](https://
+12.95 | 877 [Mask R-CNN](https://       github.com/onnx/models/tree/main/
+github.com/onnx/models/tree/main/       vision/classification/resnet) | 25 |
+vision/object_detection_segmentation/   3,868
 mask-rcnn) | 46.77 | 92,077
```

### Comparing `onnx-tool-0.6.5/README.md` & `onnx-tool-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,38 @@
+Metadata-Version: 2.1
+Name: onnx-tool
+Version: 0.7.0
+Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
+Home-page: https://github.com/ThanatosShinji/onnx-tool
+Author: Luo Yu
+Author-email: luoyu888888@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a href="README_CN.md">简体中文</a>
 # onnx-tool
 
 **A tool for ONNX model:**
 
 * *Rapid shape inference.*
 * *Profile model.*
+* *<a href="data/ConstantFolding.md">Constant Folding.</a>*
 * *Compute Graph and Shape Engine.*
 * *OPs fusion.*
 * *Activation memory compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT, LLaMa, MPT(<a href="benchmark/transfomer_models.py">TransformerModel</a>)
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
-* CV: Resnet, MobileNet, YOLO, ...
-* Audio: LPCNet
+* CV: <a href="benchmark/compression.py">BEVFormer</a>, MobileNet, YOLO, ...
+* Audio: sovits, LPCNet
 
 ---
 
 ## Shape inference
 
 <p align="center">  
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/shape_inference.jpg">
@@ -85,15 +98,15 @@
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
 BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
-
+Help implement model parallelism.
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_subgraph.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
@@ -141,30 +154,31 @@
 Then `pip install onnx-tool` again.
 
 
 ---
 
 ## Known Issues
 * Loop op is not supported
-
+* Activation Compression is not optimum
+  
 ---
 
 ## Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
 Some models have dynamic input shapes. The MACs varies from input shapes. The input shapes used in these results are writen to [data/public/config.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py).
 These onnx models with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ 
 )(code: p91k) [google drive](https://drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 <p id="results" align="center">
 <table>
 <tr>
 <td>
 
 Model | Params(M) | MACs(M)
 ---|---|---
-GPT-J 1 layer | 464 | 173,398  
-MPT 1 layer | 261 | 79,894
+<a href="benchmark/transfomer_models.py">GPT-J 1 layer</a> | 464 | 173,398  
+<a href="benchmark/transfomer_models.py">MPT 1 layer</a> | 261 | 79,894
 [text_encoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main)| 123.13 | 6,782
 [UNet2DCondition](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main)| 859.52 | 888,870
 [VAE_encoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main) | 34.16 | 566,371
 [VAE_decoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main) | 49.49 | 1,271,959
 [SqueezeNet 1.0](https://github.com/onnx/models/tree/main/vision/classification/squeezenet) | 1.23 | 351
 [AlexNet](https://github.com/onnx/models/tree/main/vision/classification/alexnet) | 60.96 | 665
 [GoogleNet](https://github.com/onnx/models/tree/main/vision/classification/inception_and_googlenet/googlenet) | 6.99 | 1,606
@@ -176,29 +190,29 @@
 [Emotion](https://github.com/onnx/models/tree/main/vision/body_analysis/emotion_ferplus) | 12.95 | 877
 [Mask R-CNN](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/mask-rcnn) | 46.77 | 92,077
 </td>
 
 <td>
 
 Model | Params(M) | MACs(M)
----|---|---
-LLaMa 1 layer | 618 | 211,801  
-[rvm_mobilenetv3](https://github.com/PeterL1n/RobustVideoMatting) | 3.73 | 4,289
-[yolov4](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/yolov4) | 64.33 | 3,319
-[ConvNeXt-L](https://github.com/facebookresearch/ConvNeXt) | 229.79 | 34,872
-[edgenext_small](https://github.com/mmaaz60/EdgeNeXt) | 5.58 | 1,357
-[SSD](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/ssd) | 19.98 | 216,598
-[RealESRGAN](https://github.com/xinntao/Real-ESRGAN) | 16.69 | 73,551
-[ShuffleNet](https://github.com/onnx/models/tree/main/vision/classification/shufflenet) | 2.29 | 146
-[GPT-2](https://github.com/onnx/models/tree/main/text/machine_comprehension/gpt-2) | 137.02 | 1,103
-[T5-encoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 109.62 | 686
-[T5-decoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 162.62 | 1,113
-[RoBERTa-BASE](https://github.com/onnx/models/tree/main/text/machine_comprehension/roberta) | 124.64 | 688
-[Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10 | 46,018
-[FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29 | 37,056
-[MobileNet](https://github.com/onnx/models/blob/main/vision/classification/mobilenet) | 3.3 | 300
-[ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25 | 3,868
+---|-----------|---
+<a href="benchmark/transfomer_models.py">LLaMa 1 layer</a> | 618       | 211,801  
+[BEVFormer Tiny](https://github.com/DerryHub/BEVFormer_tensorrt) | 33.7      | 210,838
+[rvm_mobilenetv3](https://github.com/PeterL1n/RobustVideoMatting) | 3.73      | 4,289
+[yolov4](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/yolov4) | 64.33     | 3,319
+[ConvNeXt-L](https://github.com/facebookresearch/ConvNeXt) | 229.79    | 34,872
+[edgenext_small](https://github.com/mmaaz60/EdgeNeXt) | 5.58      | 1,357
+[SSD](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/ssd) | 19.98     | 216,598
+[RealESRGAN](https://github.com/xinntao/Real-ESRGAN) | 16.69     | 73,551
+[ShuffleNet](https://github.com/onnx/models/tree/main/vision/classification/shufflenet) | 2.29      | 146
+[GPT-2](https://github.com/onnx/models/tree/main/text/machine_comprehension/gpt-2) | 137.02    | 1,103
+[T5-encoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 109.62    | 686
+[T5-decoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 162.62    | 1,113
+[RoBERTa-BASE](https://github.com/onnx/models/tree/main/text/machine_comprehension/roberta) | 124.64    | 688
+[Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10     | 46,018
+[FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29     | 37,056
+[ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25        | 3,868
 
 </td>
 </tr>
 </table>
-</p>
+</p>
```

#### html2text {}

```diff
@@ -1,13 +1,19 @@
-ç®ä½ä¸­æ # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.*
-* *Profile model.* * *Compute Graph and Shape Engine.* * *OPs fusion.* *
-*Activation memory compression.* * *Quantized models and sparse models are
-supported.* Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.0 Summary: A tool for ONNX
+model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
+fusion;Quantized models and sparse models are supported. Home-page: https://
+github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
+luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
+:: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
+# onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
+model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
+fusion.* * *Activation memory compression.* * *Quantized models and sparse
+models are supported.* Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT
 (TransformerModel) * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV:
-Resnet, MobileNet, YOLO, ... * Audio: LPCNet --- ## Shape inference
+BEVFormer, MobileNet, YOLO, ... * Audio: sovits, LPCNet --- ## Shape inference
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              shape_inference.jpg]
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/data/Profile.md). pytorch usage: [data/PytorchUsage.md](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md). tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/TensorflowUsage.md). samples: [benchmark/samples.py](https://
@@ -48,15 +54,15 @@
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               resnet18_fused.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). BERT samples: [benchmark/samples.py](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/
 onnx-tool/blob/main/benchmark/do_fusion.py). --- ## Extract subgraph from ONNX
-model
+model Help implement model parallelism.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                             resnet18_subgraph.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). --- ## Memory Compression For large language
 models and high-resolution CV models, the activation memory compression is a
 key to save memory. The compression method achieves 5% memory compression on
 most models. For example: model | Native Memory Size(MB) | Compressed Memory
@@ -72,62 +78,63 @@
 set its static weight tensors as its input tensors* * *Set custom input and
 output tensors' name and dimension, change model from fixed input to dynamic
 input* how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-
 tool/blob/main/data/Tensors.md). --- ## How to install `pip install onnx-tool`
 OR `pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
 python>=3.6 If `pip install onnx-tool` failed by onnx's installation, you may
 try `pip install onnx==1.8.1` (a lower version like this) first. Then `pip
-install onnx-tool` again. --- ## Known Issues * Loop op is not supported --- ##
-Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
-Some models have dynamic input shapes. The MACs varies from input shapes. The
-input shapes used in these results are writen to [data/public/config.py](https:
-//github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These
-onnx models with all tensors' shape can be downloaded: [baidu drive](https://
-pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
+install onnx-tool` again. --- ## Known Issues * Loop op is not supported *
+Activation Compression is not optimum --- ## Results of [ONNX Model Zoo](https:
+//github.com/onnx/models) and SOTA models Some models have dynamic input
+shapes. The MACs varies from input shapes. The input shapes used in these
+results are writen to [data/public/config.py](https://github.com/
+ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These onnx models
+with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/
+s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
 drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 Model | Params(M) | MACs(M) ---|---|--
-- GPT-J 1 layer | 464 | 173,398 MPT 1   Model | Params(M) | MACs(M) ---|---|--
-layer | 261 | 79,894 [text_encoder]     - LLaMa 1 layer | 618 | 211,801
-(https://huggingface.co/bes-dev/stable- [rvm_mobilenetv3](https://github.com/
-diffusion-v1-4-onnx/tree/main)| 123.13  PeterL1n/RobustVideoMatting) | 3.73 |
-| 6,782 [UNet2DCondition](https://      4,289 [yolov4](https://github.com/onnx/
-huggingface.co/bes-dev/stable-          models/tree/main/vision/
-diffusion-v1-4-onnx/tree/main)| 859.52  object_detection_segmentation/yolov4) |
-| 888,870 [VAE_encoder](https://        64.33 | 3,319 [ConvNeXt-L](https://
-huggingface.co/bes-dev/stable-          github.com/facebookresearch/ConvNeXt) |
-diffusion-v1-4-onnx/tree/main) | 34.16  229.79 | 34,872 [edgenext_small](https:
-| 566,371 [VAE_decoder](https://        //github.com/mmaaz60/EdgeNeXt) | 5.58 |
-huggingface.co/bes-dev/stable-          1,357 [SSD](https://github.com/onnx/
-diffusion-v1-4-onnx/tree/main) | 49.49  models/tree/main/vision/
-| 1,271,959 [SqueezeNet 1.0](https://   object_detection_segmentation/ssd) |
+- GPT-J_1_layer | 464 | 173,398 MPT_1   Model | Params(M) | MACs(M) ---|-------
+layer | 261 | 79,894 [text_encoder]     ----|--- LLaMa_1_layer | 618 | 211,801
+(https://huggingface.co/bes-dev/stable- [BEVFormer Tiny](https://github.com/
+diffusion-v1-4-onnx/tree/main)| 123.13  DerryHub/BEVFormer_tensorrt) | 33.7 |
+| 6,782 [UNet2DCondition](https://      210,838 [rvm_mobilenetv3](https://
+huggingface.co/bes-dev/stable-          github.com/PeterL1n/RobustVideoMatting)
+diffusion-v1-4-onnx/tree/main)| 859.52  | 3.73 | 4,289 [yolov4](https://
+| 888,870 [VAE_encoder](https://        github.com/onnx/models/tree/main/
+huggingface.co/bes-dev/stable-          vision/object_detection_segmentation/
+diffusion-v1-4-onnx/tree/main) | 34.16  yolov4) | 64.33 | 3,319 [ConvNeXt-L]
+| 566,371 [VAE_decoder](https://        (https://github.com/facebookresearch/
+huggingface.co/bes-dev/stable-          ConvNeXt) | 229.79 | 34,872
+diffusion-v1-4-onnx/tree/main) | 49.49  [edgenext_small](https://github.com/
+| 1,271,959 [SqueezeNet 1.0](https://   mmaaz60/EdgeNeXt) | 5.58 | 1,357 [SSD]
+github.com/onnx/models/tree/main/       (https://github.com/onnx/models/tree/
+vision/classification/squeezenet) |     main/vision/
+1.23 | 351 [AlexNet](https://           object_detection_segmentation/ssd) |
 github.com/onnx/models/tree/main/       19.98 | 216,598 [RealESRGAN](https://
-vision/classification/squeezenet) |     github.com/xinntao/Real-ESRGAN) | 16.69
-1.23 | 351 [AlexNet](https://           | 73,551 [ShuffleNet](https://
-github.com/onnx/models/tree/main/       github.com/onnx/models/tree/main/
-vision/classification/alexnet) | 60.96  vision/classification/shufflenet) |
-| 665 [GoogleNet](https://github.com/   2.29 | 146 [GPT-2](https://github.com/
-onnx/models/tree/main/vision/           onnx/models/tree/main/text/
-classification/inception_and_googlenet/ machine_comprehension/gpt-2) | 137.02 |
-googlenet) | 6.99 | 1,606               1,103 [T5-encoder](https://github.com/
+vision/classification/alexnet) | 60.96  github.com/xinntao/Real-ESRGAN) | 16.69
+| 665 [GoogleNet](https://github.com/   | 73,551 [ShuffleNet](https://
+onnx/models/tree/main/vision/           github.com/onnx/models/tree/main/
+classification/inception_and_googlenet/ vision/classification/shufflenet) |
+googlenet) | 6.99 | 1,606               2.29 | 146 [GPT-2](https://github.com/
 [googlenet_age](https://github.com/     onnx/models/tree/main/text/
-onnx/models/tree/main/vision/           machine_comprehension/t5) | 109.62 |
-body_analysis/age_gender) | 5.98 |      686 [T5-decoder](https://github.com/
+onnx/models/tree/main/vision/           machine_comprehension/gpt-2) | 137.02 |
+body_analysis/age_gender) | 5.98 |      1,103 [T5-encoder](https://github.com/
 1,605 [LResNet100E-IR](https://         onnx/models/tree/main/text/
-github.com/onnx/models/tree/main/       machine_comprehension/t5) | 162.62 |
-vision/body_analysis/arcface) | 65.22 | 1,113 [RoBERTa-BASE](https://
-12,102 [BERT-Squad](https://github.com/ github.com/onnx/models/tree/main/text/
-onnx/models/tree/main/text/             machine_comprehension/roberta) | 124.64
-machine_comprehension/bert-squad) |     | 688 [Faster R-CNN](https://
-113.61 | 22,767 [BiDAF](https://        github.com/onnx/models/blob/main/
-github.com/onnx/models/tree/main/text/  vision/object_detection_segmentation/
-machine_comprehension/                  faster-rcnn) | 44.10 | 46,018 [FCN
-bidirectional_attention_flow) | 18.08 | ResNet-50](https://github.com/onnx/
-9.87 [EfficientNet-Lite4](https://      models/tree/main/vision/
-github.com/onnx/models/tree/main/       object_detection_segmentation/fcn) |
-vision/classification/efficientnet-     35.29 | 37,056 [MobileNet](https://
-lite4) | 12.96 | 1,361 [Emotion](https: github.com/onnx/models/blob/main/
-//github.com/onnx/models/tree/main/     vision/classification/mobilenet) | 3.3
-vision/body_analysis/emotion_ferplus) | | 300 [ResNet50](https://github.com/
-12.95 | 877 [Mask R-CNN](https://       onnx/models/tree/main/vision/
-github.com/onnx/models/tree/main/       classification/resnet) | 25 | 3,868
-vision/object_detection_segmentation/
+github.com/onnx/models/tree/main/       machine_comprehension/t5) | 109.62 |
+vision/body_analysis/arcface) | 65.22 | 686 [T5-decoder](https://github.com/
+12,102 [BERT-Squad](https://github.com/ onnx/models/tree/main/text/
+onnx/models/tree/main/text/             machine_comprehension/t5) | 162.62 |
+machine_comprehension/bert-squad) |     1,113 [RoBERTa-BASE](https://
+113.61 | 22,767 [BiDAF](https://        github.com/onnx/models/tree/main/text/
+github.com/onnx/models/tree/main/text/  machine_comprehension/roberta) | 124.64
+machine_comprehension/                  | 688 [Faster R-CNN](https://
+bidirectional_attention_flow) | 18.08 | github.com/onnx/models/blob/main/
+9.87 [EfficientNet-Lite4](https://      vision/object_detection_segmentation/
+github.com/onnx/models/tree/main/       faster-rcnn) | 44.10 | 46,018 [FCN
+vision/classification/efficientnet-     ResNet-50](https://github.com/onnx/
+lite4) | 12.96 | 1,361 [Emotion](https: models/tree/main/vision/
+//github.com/onnx/models/tree/main/     object_detection_segmentation/fcn) |
+vision/body_analysis/emotion_ferplus) | 35.29 | 37,056 [ResNet50](https://
+12.95 | 877 [Mask R-CNN](https://       github.com/onnx/models/tree/main/
+github.com/onnx/models/tree/main/       vision/classification/resnet) | 25 |
+vision/object_detection_segmentation/   3,868
 mask-rcnn) | 46.77 | 92,077
```

### Comparing `onnx-tool-0.6.5/onnx_tool/__init__.py` & `onnx-tool-0.7.0/onnx_tool/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,14 @@
 from .serialization import serialize_shape_engine, serialize_graph
 
 
 def __remove_initilisers(graph: onnx.GraphProto):
     graph.ClearField('initializer')
 
 
-def __remove_constantnodes(graph: onnx.GraphProto):
-    validnodes = []
-    for node in graph.node:
-        if node.op_type != 'Constant':
-            validnodes.append(node)
-    graph.ClearField('node')
-    for node in validnodes:
-        graph.node.append(node)
-
-
 def model_export_tensors_numpy(m, tensornames: [str] = None, savefolder: str = None, fp16: bool = False) -> None:
     if isinstance(m, str):
         m = onnx.load_model(m)
 
     def save_numpy(arr: numpy.ndarray, fp16: bool, filename):
         if fp16 and arr.dtype in [numpy.float32, numpy.float64]:
             arr = arr.astype(numpy.float16)
@@ -74,20 +64,21 @@
     'Identity', 'Constant', 'Shape', 'Squeeze', 'Unsqueeze', 'Reshape', 'ConstantOfShape', 'Cast', 'Pad', 'Concat',
     'Slice', 'Gather'
 )
 
 
 def model_profile(m, dynamic_shapes: {str: tuple} = None, savenode: str = None,
                   saveshapesmodel: str = None, shapesonly: bool = False, verbose: bool = False,
+                  constant_folding: bool = False,
                   hidden_ops: [str] = NoMacsOps,
                   dump_outputs: [str] = None) -> None:
     if isinstance(m, str):
         m = onnx.load_model(m)
     if isinstance(m, onnx.ModelProto):
-        g = Graph(m.graph, verbose=verbose)
+        g = Graph(m.graph, constant_folding=constant_folding, verbose=verbose)
         gtmr = timer()
         g.graph_reorder()
         gtmr.start()
         g.shape_infer(dynamic_shapes)
         if verbose:
             print(f'infered all tensor shapes, time cost {gtmr.stop():.3f} s')
         gtmr.start()
@@ -109,36 +100,20 @@
         G = Graph(m.graph)
         G.graph_reorder()
         shape_engine = G.shape_regress(input_desc, input_range)
         cg = G.get_compute_graph()
         return shape_engine, cg
 
 
-def model_remove_Identity(m, f: str):
+def model_constant_folding(m, f: str):
     if isinstance(m, str):
         m = onnx.load_model(m)
     if isinstance(m, onnx.ModelProto):
-        graph = m.graph
-        iden_map = {}
-        iden_set = []
-        for node in graph.node:
-            if node.op_type == 'Identity':
-                iden_map[node.output[0]] = node.input[0]
-                iden_set.append(node.name)
-        for node in graph.node:
-            for i, input in enumerate(node.input):
-                if input in iden_map.keys():
-                    node.input[i] = iden_map[input]
-        G = Graph(graph)
-        nodes = list(G.nodemap.keys())
-        for idenn in iden_set:
-            nodes.remove(idenn)
-        onnxg = G.get_onnxgraph_by_nodenames(nodes)
-        G = Graph(onnxg)
-        G.save_model(f)
+        g = Graph(m.graph, constant_folding=True, verbose=True)
+        g.save_model(f, rawmodel=m)
 
 
 def model_shape_infer(m, dynamic_shapes: {str: tuple} = None,
                       saveshapesmodel: str = None, shapesonly: bool = False, verbose: bool = False,
                       dump_outputs: [str] = None):
     if isinstance(m, str):
         m = onnx.load_model(m)
@@ -347,15 +322,15 @@
                                 nb.ClearField('dim_param')
                             nb.dim_value = int(shapeval)
                         else:
                             if nb.HasField('dim_value'):
                                 nb.ClearField('dim_value')
                             nb.dim_param = shapeval
         graph = Graph(graph)
-        graph.save_model(savemodel)
+        graph.save_model(savemodel, rawmodel=m)
 
 
 def model_subgraph(m, in_tensor_names: [str] = None, out_tensor_names: [str] = None, nodenames: [str] = None,
                    savefolder='./'):
     if isinstance(m, str):
         mname = os.path.basename(m)
         mname = os.path.splitext(mname)[0]
```

### Comparing `onnx-tool-0.6.5/onnx_tool/__main__.py` & `onnx-tool-0.7.0/onnx_tool/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def get_parser():
     parser = argparse.ArgumentParser(
         "onnx_tool",
         description="Profile MACs(FLOPs) and perform shape inference on fixed-shape ONNX model"
     )
     parser.add_argument(
         "-m", "--mode",
-        choices=['profile', 'export_tensors', 'rm_iden', 'io_modify'],
+        choices=['profile', 'export_tensors', 'constant_folding', 'io_modify'],
         default='profile',
         help="rm_iden: remove Identity layers")
     parser.add_argument(
         "-i", "--in", dest='in_', required=True,
         help="path of input ONNX model")
     parser.add_argument(
         "-o", "--out",
@@ -89,13 +89,13 @@
     if args.dynamic_shapes is not None:
         dynamic = __args2dynamicshapes__(args.dynamic_shapes)
     else:
         dynamic = None
     onnx_tool.model_profile(args.in_, dynamic, args.file, args.out, dump_outputs=args.names)
 elif args.mode == 'export_tensors':
     onnx_tool.model_export_tensors_numpy(args.in_, tensornames=args.names, savefolder=args.out, fp16=args.fp16)
-elif args.mode == 'rm_iden':
-    onnx_tool.model_remove_Identity(args.in_, args.out)
+elif args.mode == 'constant_folding':
+    onnx_tool.model_constant_folding(args.in_, args.out)
 elif args.mode == 'io_modify':
     if args.dynamic_shapes is not None:
         shapedic = __args2strshapes__(args.dynamic_shapes)
-    onnx_tool.model_io_modify(args.in_, args.out, shapedic)
+        onnx_tool.model_io_modify(args.in_, args.out, shapedic)
```

### Comparing `onnx-tool-0.6.5/onnx_tool/fusion.py` & `onnx-tool-0.7.0/onnx_tool/fusion.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.6.5/onnx_tool/graph.py` & `onnx-tool-0.7.0/onnx_tool/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy
 import onnx
 
 import onnx_tool
 from .node import create_node
 from .tensor import get_attribute_data, Tensor, volume
+from .tensor import STATIC_TENSOR, DYNAMIC_TENSOR
 from .utils import VERSION, tuple2str
 
 
 def __shape_of_initializer__(initial):
     shape = []
     # for nb in tensor.shape.dim
     for nb in initial.dims:
@@ -26,16 +27,19 @@
     'Expand': ('1of2',),
     'Slice': ('1,2of3', '1,2,3of4', '1,2,3,4of5'),
     'ConstantOfShape': ('0of1',),
     'Tile': ('1of2',),
     'Range': ('0,1,2of3',),
     'OneHot': ('1of3',),
     'TopK': ('1of2',),
-    'Pad': ('1of3',),
+    'Pad': ('1of2', '1of3',),
     'NonMaxSuppression': ('2of5',),
+    'Split': ('1of2',),
+    'Unsqueeze': ('1of2',),
+    'Squeeze': ('1of2',)
 }
 
 
 def _contains_shape_tensor(n):
     nodeset = _SHAPE_TENSORS.keys()
     shape_tensors = []
     if n.op_type in nodeset:
@@ -152,44 +156,162 @@
         for key in self.input_desc:
             shape = self.get_tensorshape(key)
             tmp_input[key] = numpy.zeros(shape)
         return tmp_input
 
 
 class Graph():
-    def __init__(self, g: onnx.GraphProto, noderename: bool = False, verbose=False):
+    def __init__(self, g: onnx.GraphProto, constant_folding: bool = True, noderename: bool = False, verbose=False):
         self.verbose = verbose
         self.nodemap = {}
         self.tensormap = {}
         self.producedby = {}
         self.consumedby = {}
         self.rawgraph = g
         self.initials = []
         self.dynamics = []
         self.input = []
         self.output = []
         self.__init_graph_from_onnxproto__(g, noderename)
+        self.__constant_search__(constant_folding)
+        self.__update_nodes_tensors__(constant_folding)
         self.__find_shape_tensors__()
         self.valid_shape = False
         self.valid_profile = False
 
     def log(self, str):
         if self.verbose:
             print(str)
 
-    def remove_constant(self):
-        rmlist = []
-        for key in self.nodemap:
-            if self.nodemap[key].op_type == 'Constant':
-                rmlist.append(key)
+    def __update_nodes_tensors__(self, constant_folding):
+        from .utils import timer
+        tm = timer()
+        if constant_folding:
+            rmlist = []
+            for key in self.nodemap:
+                if self.nodemap[key].constant:
+                    rmlist.append(key)
+            self.log(f'GraphProto Nodes Count:{len(self.rawgraph.node)}')
+            self.log(f'Contant folding {rmlist[:3]}... {len(rmlist)} Nodes')
+            for key in rmlist:
+                self.nodemap.pop(key)
+
+        self.initials = []
+        self.dynamics = []
+
+        if constant_folding:
+            for name in self.nodemap.keys():
+                for tname in self.nodemap[name].input:
+                    if self.tensormap[tname].type == STATIC_TENSOR:
+                        if tname not in self.initials:
+                            self.initials.append(tname)
+                    if self.tensormap[tname].type == DYNAMIC_TENSOR:
+                        if tname not in self.dynamics:
+                            self.dynamics.append(tname)
+                for tname in self.nodemap[name].output:
+                    if tname not in self.dynamics:
+                        self.dynamics.append(tname)
+        else:
+            for initial in self.rawgraph.initializer:
+                self.initials.append(initial.name)
+            self.dynamics.extend(self.input)
+            for name in self.nodemap.keys():
+                for tname in self.nodemap[name].input:
+                    if tname not in self.initials and tname not in self.dynamics:
+                        self.dynamics.append(tname)
+                for tname in self.nodemap[name].output:
+                    if tname not in self.dynamics:
+                        self.dynamics.append(tname)
+
+        valid_tensors = []
+        valid_tensors.extend(self.initials)
+        valid_tensors.extend(self.dynamics)
+        rm_list = []
+        for tname in self.tensormap.keys():
+            if tname not in valid_tensors:
+                rm_list.append(tname)
+        for tname in rm_list:
+            self.tensormap.pop(tname)
+
+        self.input = []
+        self.output = []
+        for name in self.nodemap.keys():
+            node = self.nodemap[name]
+            for tensor in node.input:
+                if tensor not in self.producedby and tensor in self.dynamics:
+                    if tensor not in self.input:
+                        self.input.append(tensor)
+            for tensor in node.output:
+                if tensor not in self.consumedby or len(self.consumedby[tensor]) == 0:
+                    if tensor not in self.output:
+                        self.output.append(tensor)
+        self.__update_consumer_producer__()
+        self.log(f'Update Nodes Tensors  Time Elapsed {tm.stop()}')
+
+    def __is_node_constant__(self, node):
+        constant_node = True
+        for tname in node.input:
+            if self.tensormap[tname].type == DYNAMIC_TENSOR:
+                constant_node = False
+                break
+        return constant_node
+
+    def __constant_search__(self, constant_folding):
+        from .utils import timer
+        tm = timer()
+        for name in self.nodemap.keys():
+            node = self.nodemap[name]
+            if hasattr(node, 'constant'):
+                continue
+            constant_node = self.__is_node_constant__(node)
+            node.constant = constant_node
+            if constant_node:
+                search_nodes = [name]
+                while len(search_nodes) > 0:
+                    this_node = self.nodemap[search_nodes[0]]
+                    search_nodes.pop(0)
+                    if constant_folding:
+                        itensors = []
+                        for input in this_node.input:
+                            if self.tensormap[input].numpy is None:
+                                warnings.warn(f'Tensor {input} has shape only, {name} may has wrong value infer result')
+                                itensors.append(self.tensormap[input].get_shape())
+                            else:
+                                itensors.append(self.tensormap[input].numpy)
+                        otensors = this_node.value_infer(itensors)
+                        if len(otensors) > 0:
+                            for i, output in enumerate(this_node.output):
+                                self.tensormap[output].update_tensor(otensors[i])
+                                self.tensormap[output].type = STATIC_TENSOR
+                    else:
+                        for i, output in enumerate(this_node.output):
+                            self.tensormap[output].type = STATIC_TENSOR
+                    for output in this_node.output:
+                        for consumer in self.consumedby[output]:
+                            cnode = self.nodemap[consumer]
+                            if self.__is_node_constant__(cnode):
+                                cnode.constant = True
+                                search_nodes.append(consumer)
+        self.log(f'Constant Search Time Elapsed {tm.stop()}')
 
-        for key in rmlist:
-            self.nodemap.pop(key)
+    def __update_consumer_producer__(self):
+        self.producedby = {}
+        self.consumedby = {}
+        for name in self.nodemap:
+            node = self.nodemap[name]
+            for tensor in node.input:
+                if tensor not in self.consumedby:
+                    self.consumedby[tensor] = []
+                self.consumedby[tensor].append(node.name)
+            for tensor in node.output:
+                if tensor not in self.producedby:
+                    self.producedby[tensor] = []
+                self.producedby[tensor].append(node.name)
 
-    def __init_graph_from_onnxproto__(self, g, noderename, remove_dummytensors=True):
+    def __init_graph_from_onnxproto__(self, g, noderename):
         if g is None:
             return
         ncount = 0
         from .utils import timer
 
         tm = timer()
         tm.start()
@@ -213,98 +335,56 @@
                 newnode.output.append(tensor)
 
             self.nodemap[newnode.name] = newnode
 
         self.log(f'Node Init Time Elapsed {tm.stop()}')
 
         tm.start()
+        # init initials first
+        for initial in g.initializer:
+            tensor = Tensor(initial)
+            self.tensormap[initial.name] = tensor
+
         for input in g.input:
-            tensor = Tensor(input)
-            self.tensormap[input.name] = tensor
-            self.input.append(input.name)
-            self.dynamics.append(input.name)
+            if input.name not in self.tensormap.keys():
+                self.tensormap[input.name] = Tensor(input)
 
         for output in g.output:
-            tensor = Tensor(output)
-            self.tensormap[output.name] = tensor
-            self.output.append(output.name)
-            self.dynamics.append(output.name)
+            if output.name not in self.tensormap.keys():
+                self.tensormap[output.name] = Tensor(output)
 
+        # init dynamic tensor info
+        for valinfo in g.value_info:
+            if valinfo.name not in self.tensormap.keys():
+                tensor = Tensor(valinfo)
+                self.tensormap[valinfo.name] = tensor
+        self.log(f'Tensor Init Time Elapsed {tm.stop()}')
+
+        tm.start()
+        # dynamic tensor info
         for key in self.nodemap.keys():
             node = self.nodemap[key]
-            dummy_lists = []
+            for tensor in node.input:
+                if tensor not in self.tensormap.keys():
+                    self.tensormap[tensor] = Tensor(tensor)
             for tensor in node.output:
+                if tensor not in self.tensormap.keys():
+                    self.tensormap[tensor] = Tensor(tensor)
                 if tensor in self.consumedby:
                     for consumer in self.consumedby[tensor]:
                         self.nodemap[node.name].nextnodes.append(self.nodemap[consumer])
-                else:
-                    if tensor not in self.output:
-                        self.log(f'Dummy tensors detected: {tensor}')
-                        if remove_dummytensors:
-                            dummy_lists.append(tensor)
-            for tensor in dummy_lists:
-                node.output.remove(tensor)
-
-        for valinfo in g.value_info:
-            tensor = Tensor(valinfo)
-            self.tensormap[valinfo.name] = tensor
-
         self.log(f'IO Tensor Init Time Elapsed {tm.stop()}')
 
-        tm.start()
-        for initial in g.initializer:
-            self.initials.append(initial.name)
-            tensor = Tensor(initial)
-            self.tensormap[initial.name] = tensor
-
-        for key in self.nodemap.keys():
-            node = self.nodemap[key]
-            if node.op_type == 'Constant':
-                tensor = Tensor(node)
-                self.tensormap[node.output[0]] = tensor
-                self.initials.append(node.output[0])
-        self.initials = set(self.initials)
-
-        self.log(f'Static Tensor Init Time Elapsed {tm.stop()}')
-
-        rmlist = []
-        for input in self.input:
-            if input in self.initials:
-                rmlist.append(input)
-        for key in rmlist:
-            self.dynamics.remove(key)
-            self.input.remove(key)
-
-        rmlist = []
-        for output in self.output:
-            if output in self.consumedby.keys():
-                rmlist.append(output)
-        for key in rmlist:
-            self.dynamics.remove(key)
-            self.output.remove(key)
-
-        tm.start()
-        for key in self.nodemap.keys():
-            node = self.nodemap[key]
-            for input in node.input:
-                if input not in self.initials:
-                    self.dynamics.append(input)
-                    if input not in self.tensormap.keys():
-                        self.tensormap[input] = Tensor(input)
-
-        # self.dynamics = set(self.dynamics)
         self.sparse_model = False
         for key in self.tensormap.keys():
             tensor = self.tensormap[key]
             if tensor.sparsity is not None and tensor.sparsity['ratio'] > 0.4:
                 self.sparse_model = True
                 break
 
-        self.log(f'Misc Tensor Init Time Elapsed {tm.stop()}')
-
     def __find_shape_tensors__(self):
         self.shape_tensors = []
         for n in self.nodemap.keys():
             shape_tensors = _contains_shape_tensor(self.nodemap[n])
             for st in shape_tensors:
                 self.shape_tensors.append(st)
         self.shape_tensors = set(self.shape_tensors)
@@ -359,15 +439,15 @@
             if node not in graph_level1 and node not in graph_level2:
                 graph_level0.append(node)
 
         return graph_level0, graph_level1, graph_level2
 
     def add_initial(self, name, data):
         from .tensor import create_initial_Tensor
-        self.initials.add(name)
+        self.initials.append(name)
         if isinstance(data, numpy.ndarray):
             self.tensormap[name] = create_initial_Tensor(name, data)
         else:
             raise NotImplementedError('unsupported data type')
 
     def get_subgraph(self, inputs: [], outputs: []):
         graph_level0, graph_level1, graph_level2 = self.__get_subnodes_byio__(inputs, outputs)
@@ -401,18 +481,20 @@
         if len(extern_outputs) != len(self.output):
             warnings.warn("subgraph input and output tensors can not reverse to raw graph.")
 
         return graph_level0, graph_level1, graph_level2
 
     def get_initials_from_nodenames(self, nodenames):
         initializer = []
+        enqueued = []
         for name in nodenames:
             for input in self.nodemap[name].input:
-                if input in self.initials:
-                    initializer.append(self.tensormap[input].proto)
+                if input in self.initials and input not in enqueued:
+                    initializer.append(self.tensormap[input].make_tensor_proto())
+                    enqueued.append(input)
         return initializer
 
     def remove_node(self, nodename):
         node = self.nodemap[nodename]
         # update producer
         for o in node.output:
             self.producedby[o].remove(nodename)
@@ -528,65 +610,64 @@
         if len(nodenames):
             _inputs0, _outputs0 = self.get_iotensors(nodenames)
             graph_level0 = self.reorder_nodes(nodenames, _inputs0)
             subgraph = self.make_graph_onnx(graph_level0, 'subgraph', _inputs0, _outputs0)
             return subgraph
         return None
 
-    def save_model(self, f: str, shape_only: bool = False, rawmodel: onnx.ModelProto = None):
-        graph = self.make_graph_onnx(self.nodemap.keys(), 'graph', self.input, self.output, not shape_only)
+    def save_model(self, f: str, shape_only: bool = False, no_shape: bool = False, rawmodel: onnx.ModelProto = None):
+        graph = self.make_graph_onnx(self.nodemap.keys(), 'graph', self.input, self.output,
+                                     with_initializer=not shape_only, with_shape_info=not no_shape)
         if graph is not None and f is not None:
             attr = {}
             attr['producer_name'] = 'onnx_tool'
             attr['producer_version'] = 'v' + VERSION
             model = onnx.helper.make_model(graph, **attr)
             if rawmodel is not None:
                 model.ir_version = rawmodel.ir_version
                 model.opset_import[0].version = rawmodel.opset_import[0].version
             onnx.save_model(model, f)
 
-    def make_graph_onnx(self, nodenames, gname, inputnames, outputnames, with_initializer=True):
+    def make_graph_onnx(self, nodenames, gname, inputnames, outputnames, with_initializer=True, with_shape_info=True):
         nodes = []
         for name in nodenames:
             nodes.append(self.nodemap[name].make_nodeproto())
 
         initializer = None
         if with_initializer:
             initializer = self.get_initials_from_nodenames(nodenames)
 
         inputs = []
         outputs = []
         for name in inputnames:
             if name in self.tensormap:
-                inputs.append(self.tensormap[name].make_value_proto())
+                proto = self.tensormap[name].make_value_proto()
+                if proto is not None:
+                    inputs.append(proto)
             else:
                 inputs.append(onnx.helper.make_tensor_value_info(name, 1, None))
         for name in outputnames:
             if name in self.tensormap:
                 proto = self.tensormap[name].make_value_proto(make_dummy=True)
-                outputs.append(proto)
+                if proto is not None:
+                    outputs.append(proto)
         value_infos = []
-        for key in self.dynamics:
-            if key in self.input or key in self.output:
-                continue
-            tensor = self.tensormap[key]
-            vinfo = tensor.make_value_proto()
-            if vinfo is None:
-                continue
-            value_infos.append(vinfo)
+        if with_shape_info:
+            for key in self.dynamics:
+                if key in self.input or key in self.output:
+                    continue
+                tensor = self.tensormap[key]
+                vinfo = tensor.make_value_proto()
+                if vinfo is None:
+                    continue
+                value_infos.append(vinfo)
         graph = onnx.helper.make_graph(nodes=nodes, name=gname, inputs=inputs, outputs=outputs, initializer=initializer,
                                        value_info=value_infos)
         return graph
 
-    def is_node_constant(self, node):
-        for input in self.nodemap[node].input:
-            if input not in self.initials:
-                return False
-        return True
-
     def graph_reorder(self):
         old_order = self.nodemap.keys()
         ordered_nodes = self.reorder_nodes(old_order, self.input)
         new_map = {}
         for nname in ordered_nodes:
             new_map[nname] = self.nodemap[nname]
         self.nodemap = new_map
@@ -603,15 +684,15 @@
                 if consumer in nodenames:
                     if consumer not in nextnodes:
                         search_flag[consumer] = True
                         nextnodes.append(consumer)
             tensor_produced.append(name)
 
         for node in nodenames:
-            if self.is_node_constant(node):
+            if self.__is_node_constant__(self.nodemap[node]):
                 dummy_node = True
                 for output in self.nodemap[node].output:
                     if output in self.consumedby.keys():
                         for consumer in self.consumedby[output]:
                             if consumer in nodenames:
                                 if consumer not in nextnodes:
                                     search_flag[consumer] = True
@@ -734,15 +815,14 @@
         if not in_valid:
             raise ValueError(
                 f"The input tensor {tname}'s shape {self.tensormap[tname].shape2str()} is not valid, Please set it to a valid shape.")
         self.shapeinfer_optime_map = {}
         from .utils import timer
         tm = timer()
         for key in self.nodemap.keys():
-
             tm.start()
             node = self.nodemap[key]
             if node.shape_calc:
                 itensors = []
                 for input in node.input:
                     if self.tensormap[input].numpy is None:
                         assert (node.op_type in ('Shape', 'Slice'))
@@ -891,15 +971,14 @@
                                 vidx = vcount + idx
                                 valkey = str(vidx)
                         shapeengine.update_tensor_desc(vkey, i, valkey)
             vcount += len(dstranges)
         return shapeengine
 
     def compress_memory(self, size_padding=64):
-        self.remove_constant()
         tensor_in_mem = copy.deepcopy(self.input)
         tensor_mem_per_node = []
         tensor_consumed = {}
         for node in self.nodemap.keys():
             node_ = self.nodemap[node]
             for name in node_.output:
                 tensor_in_mem.append(name)
@@ -1006,40 +1085,46 @@
             overlap = False
             for tname in nodetensors:
                 block = compress_mem[tname]
                 if block[0] + block[1] > maxmem:
                     maxmem = block[0] + block[1]
             for tname in nodetensors:
                 block0 = compress_mem[tname]
+                if block0[1] == 0:
+                    continue
                 for tname1 in nodetensors:
                     if tname1 == tname:
                         continue
                     block1 = compress_mem[tname1]
+                    if block1[1] == 0:
+                        continue
                     if block0[0] >= block1[0] and block0[0] < block1[0] + block1[1]:
                         overlap = True
                         laptensor = [tname, tname1]
                         break
                     if block1[0] >= block0[0] and block1[0] < block0[0] + block0[1]:
                         overlap = True
                         laptensor = [tname, tname1]
                         break
             if maxmem > compress_size:
                 warnings.warn(f'Wrong compress total memory size:{compress_size}. larger size detected:{maxmem}')
             if overlap:
-                warnings.warn(f'Memory overlap detected!{laptensor[0]} v.s. {laptensor[1]}')
+                if laptensor[0] != '' and laptensor[
+                    1] != '':  # some chaos models use this empty name as an empty tensor name
+                    warnings.warn(f'Memory overlap detected!{laptensor[0]} v.s. {laptensor[1]}')
 
         raw_memsize = 0
         for tname in self.dynamics:
             if tname in self.input or tname in self.output:
                 continue
             raw_memsize += self.tensormap[tname].get_memsize()
 
-        print(f"Raw memory size: {raw_memsize:,} bytes")
-        print(f"Compressed memory size: {compress_size:,} bytes")
-        print(f'Comression ratio: {compress_size / raw_memsize * 100:.3f}%')
+        self.log(f"Raw memory size (without parameter memory): {raw_memsize:,} bytes")
+        self.log(f"Compressed memory size: {compress_size:,} bytes")
+        self.log(f'Comression ratio: {compress_size / raw_memsize * 100:.3f}%')
         return compress_mem, compress_size
 
     def get_compute_graph_onnx(self):
         nodes = []
         for key in self.nodemap.keys():
             node = self.nodemap[key]
             if node.shape_calc:
@@ -1054,22 +1139,21 @@
                             break
                 else:
                     dummy = False
                 dummy_node = dummy_node and dummy
             if dummy_node:
                 continue
             nodes.append(node.name)
-
         _inputs0, _outputs0 = self.get_iotensors(nodes)
         graph_level0 = self.reorder_nodes(nodes, _inputs0)
         subgraph = self.make_graph_onnx(graph_level0, 'compute_graph', self.input, self.output)
         return subgraph
 
     def get_compute_graph(self):
-        cg = self
+        cg = copy.copy(self)
         nodes = []
         rmnodes = []
         for key in cg.nodemap.keys():
             node = cg.nodemap[key]
             if node.shape_calc:
                 rmnodes.append(key)
                 continue
@@ -1082,41 +1166,55 @@
                             dummy = False
                             break
                 else:
                     dummy = False
                 dummy_node = dummy_node and dummy
             if dummy_node:
                 rmnodes.append(key)
+                searchnodes = [key]
+                while len(searchnodes) > 0:
+                    this_node = self.nodemap[searchnodes[0]]
+                    searchnodes.pop(0)
+                    for input in this_node.input:
+                        if input in self.producedby:
+                            if len(self.consumedby[input]) == 1:
+                                pnodename = self.producedby[input][0]
+                                if pnodename not in rmnodes:
+                                    rmnodes.append(pnodename)
+                                searchnodes.append(pnodename)
                 continue
             nodes.append(node.name)
-
+        self.log(f'Total Nodes:{len(cg.nodemap)} Removed Shape Nodes:{len(rmnodes)}')
         for key in rmnodes:
             cg.remove_node(key)
-        cg.graph_reorder()
+        self.log(f'Compute Graph Nodes:{len(cg.nodemap)}')
+
         cg.dynamics = []
         cg.dynamics.extend(cg.input)
         cg.dynamics.extend(cg.output)
         for name in cg.nodemap.keys():
             for output in cg.nodemap[name].output:
                 if name not in cg.dynamics:
                     cg.dynamics.append(output)
+
         return cg
 
     def profile(self):
         self.valid_profile = False
         if not self.valid_shape:
             warnings.warn('Please perform a valid shape_infer() before profile().')
             return
         params_flag_map = {}
         for key in self.initials:
             params_flag_map[key] = 0
 
         self.macs = 0.0
         self.params = 0
         self.memory = 0
+        tensors = []
         for key in self.nodemap.keys():
             node = self.nodemap[key]
             itensors = []
             _params = 0
             _memory = 0
             max_sparsity = 0
             block_sparsity = {'blocksize': (1, 1), 'blockratio': 0, 'ratio': 0}
@@ -1138,14 +1236,15 @@
                     otensors.append(self.tensormap[output].numpy)
                 else:
                     otensors.append(self.tensormap[output].get_shape())
                 if node.op_type == 'Constant':
                     # Constant's output tensors are already counted as weight tensors
                     continue
                 _memory += self.tensormap[output].get_memsize()
+                tensors.append(output)
             macs = node.profile(itensors, otensors)
             outshape = (0,)
             if len(node.output) > 0:
                 outshape = self.tensormap[node.output[0]].get_shape()
                 outshape = (0,) if len(outshape) == 0 else outshape
             inshape = (0,)
             if len(node.input) > 0:
@@ -1157,14 +1256,15 @@
             node.outshape = outshape
             node.params = _params
             node.memory = _memory
             node.sparsity = block_sparsity
             self.macs += macs
             self.params += _params
             self.memory += _memory
+
         self.valid_profile = True
 
     def print_node_map(self, f: str = None, metric='MACs', exclude_nodes=None):
         if not self.valid_profile:
             warnings.warn('Please perform a valid profile() before print_node_map().')
             return
         from tabulate import tabulate
```

### Comparing `onnx-tool-0.6.5/onnx_tool/node.py` & `onnx-tool-0.7.0/onnx_tool/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,40 @@
 import numpy
 import onnx
 import math
 import warnings
 from .tensor import get_attribute_data, volume, is_valid_ndarray, create_ndarray_f32, onnxdtype2npdtype
 from .utils import NODE_REGISTRY, tuple2str
 
-ADD_MACS = 1
-EXP_MACS = 16
-LOG_MACS = 16
-SQRT_MACS = 4
-POW_MACS = 32
+'''
+Real MACs: the number of x86 instructions to finish numeric compute.
+From a low-level view, float-point multiple and add is much expensive than
+bit movement. But current hardware has added more and more float-point
+units to accelerate this. So, we should treat every instruction equally to
+measure the complexity of the model.
+
+
+'''
+
 MUL_MACS = 1
-DIV_MACS = 2
+ADD_MACS = 1
 CMP_MACS = 1
-SIN_MACS = 14
-COS_MACS = 14
+DIV_MACS = 4  # refers to vrcp14ps
+# following refers to https://github.com/reyoung/avx_mathfun
+EXP_MACS = 32
+POW_MACS = EXP_MACS  # similar with exp
+LOG_MACS = 43
+SIN_MACS = 39
+COS_MACS = 39
+
+TANH_MACS = EXP_MACS + 2 * ADD_MACS + DIV_MACS  # (e^2x-1)/(e^2x+1)
+ATANH_MACS = LOG_MACS + 2 * ADD_MACS + DIV_MACS + MUL_MACS  # 1/2*ln((1+x)/(1-x))
+
+SQRT_MACS = 24  # refers to vsqrtps
+ATAN_MACS = SQRT_MACS + 3 * MUL_MACS + MUL_MACS + DIV_MACS  # refers to "Approximations to inverse tangent function"
 
 RESIZE_LINEAR_MACS = 4
 RESIZE_CUBIC_MACS = 8
 
 _SHAPE_TENSORS = {
     'Reshape': ('1of2',),
     'Resize': ('2of3', '3of4'),
@@ -133,15 +149,15 @@
     def shape_infer(self, intensors: []):
         faketensors = [_get_tensor(tensor) for tensor in intensors]
         outtensors = self.value_infer(faketensors)
         outshapes = [_get_shape(tensor) for tensor in outtensors]
         return outshapes
 
     def value_infer(self, intensors: []):
-        return []
+        raise NotImplementedError(f'this Node {self.op_type}-{self.name} has no value_infer')
 
     def profile(self, intensors: [], outtensors: []):
         return 0
 
 
 class FusedBase(Node):
     def shape_infer(self, intensors: []):
@@ -295,30 +311,40 @@
 @NODE_REGISTRY.register()
 class ExpNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = EXP_MACS
         self.ratio = 1
 
+    def value_infer(self, intensors: []):
+        return [numpy.exp(intensors[0])]
+
 
 @NODE_REGISTRY.register()
 class SoftmaxNode(ExpNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = EXP_MACS + DIV_MACS
         self.ratio = 1
 
+    def value_infer(self, intensors: []):
+        xexp = numpy.exp(intensors[0])
+        return [xexp / numpy.sum(xexp)]
+
 
 @NODE_REGISTRY.register()
 class LogNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = LOG_MACS
         self.ratio = 1
 
+    def value_infer(self, intensors: []):
+        return [numpy.log(intensors[0])]
+
 
 @NODE_REGISTRY.register()
 class ImageScalerNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = ADD_MACS + MUL_MACS
         self.ratio = 1
@@ -333,35 +359,47 @@
 
 @NODE_REGISTRY.register()
 class SqrtNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = SQRT_MACS
 
+    def value_infer(self, intensors: []):
+        return [numpy.sqrt(intensors[0])]
+
 
 @NODE_REGISTRY.register()
 class PowNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = POW_MACS
 
+    def value_infer(self, intensors: []):
+        return [numpy.power(intensors[0], intensors[1])]
+
 
 @NODE_REGISTRY.register()
 class SinNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = SIN_MACS
 
+    def value_infer(self, intensors: []):
+        return [numpy.sin(intensors[0])]
+
 
 @NODE_REGISTRY.register()
 class CosNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = COS_MACS
 
+    def value_infer(self, intensors: []):
+        return [numpy.cos(intensors[0])]
+
 
 @NODE_REGISTRY.register()
 class RangeNode(Node):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = 1
 
@@ -370,52 +408,94 @@
         limit = intensors[1]
         delta = intensors[2]
         return [numpy.arange(start, limit, delta, dtype=numpy.float32)]
 
 
 @NODE_REGISTRY.register()
 class SigmoidNode(ExpNode):
-    pass
+    def value_infer(self, intensors: []):
+        y = 1 / (1 + numpy.exp(-intensors[0]))
+        return [y]
 
 
 @NODE_REGISTRY.register()
 class TanhNode(PWNode):
     def __init__(self, n):
         super().__init__(n)
         self.op_mac = EXP_MACS
         self.ratio = 2
 
+    def value_infer(self, intensors: []):
+        return [numpy.tanh(intensors[0])]
+
+
+@NODE_REGISTRY.register()
+class AtanNode(TanhNode):
+    def __init__(self, n):
+        super().__init__(n)
+        self.op_mac = ATAN_MACS
+
+    def value_infer(self, intensors: []):
+        return [numpy.arctan(intensors[0])]
+
+
+@NODE_REGISTRY.register()
+class SignNode(PWNode):
+    def __init__(self, n):
+        super().__init__(n)
+        self.op_mac = CMP_MACS
+
+    def value_infer(self, intensors: []):
+        return [numpy.sign(intensors[0])]
+
 
 @NODE_REGISTRY.register()
 class HardSigmoidNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = MUL_MACS + ADD_MACS + CMP_MACS * 2
+        self.add_default_value('alpha',0.2)
+        self.add_default_value('beta',0.5)
+
+    def value_infer(self, intensors: []):
+        y = max(0, min(1, self.alpha * intensors[0] + self.beta))
+        return [y]
 
 
 @NODE_REGISTRY.register()
 class ReluNode(PWNode):
     def __init__(self, n):
         super().__init__(n)
         self.op_mac = CMP_MACS
 
+    def value_infer(self, intensors: []):
+        return [numpy.clip(intensors[0], 0, None)]
+
 
 @NODE_REGISTRY.register()
 class PReluNode(PWNode):
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
         self.op_mac = CMP_MACS + MUL_MACS
         self.ratio = 1
 
 
 @NODE_REGISTRY.register()
 class LeakyReluNode(PWNode):
     def __init__(self, n):
         super().__init__(n)
         self.op_mac = self.op_mac = MUL_MACS + CMP_MACS
+        self.add_default_value('alpha', 0.01)
+
+    def value_infer(self, intensors: []):
+        outtensor = numpy.zeros_like(intensors[0])
+        for i in numpy.ndindex(intensors[0].shape):
+            x = intensors[0][i]
+            outtensor[i] = x if x >= 0 else x * self.alpha
+        return [outtensor]
 
 
 @NODE_REGISTRY.register()
 class SumNode(PWNode):
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
         self.op_mac = ADD_MACS
@@ -426,20 +506,19 @@
         for i in range(1, len(intensors)):
             y = y + intensors[i]
         return [y]
 
 
 @NODE_REGISTRY.register()
 class NonMaxSuppressionNode(Node):
-    # TODO
-    def value_infer(self, intensors: []):
+    def shape_infer(self, intensors: []):
         if len(intensors) >= 3:
             max_output_boxes_per_class = int(intensors[2][0])
-            return [numpy.zeros((max_output_boxes_per_class, 3), dtype=numpy.int64)]
-        return [numpy.zeros((200, 3), dtype=numpy.int64)]
+            return [(max_output_boxes_per_class, 3)]
+        raise NotImplementedError()
 
 
 @NODE_REGISTRY.register()
 class LRNNode(PWNode):
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
 
@@ -484,18 +563,18 @@
         result = numpy.logical_and(intensors[0].astype(numpy.bool_), intensors[1].astype(numpy.bool_))
         return [result]
 
 
 @NODE_REGISTRY.register()
 class WhereNode(Node):
     def shape_infer(self, intensors: []):
-        cond_shape=_get_shape(intensors[0])
-        x_shape=_get_shape(intensors[1])
-        y_shape=_get_shape(intensors[2])
-        return [_max_shape((cond_shape,x_shape,y_shape))]
+        cond_shape = _get_shape(intensors[0])
+        x_shape = _get_shape(intensors[1])
+        y_shape = _get_shape(intensors[2])
+        return [_max_shape((cond_shape, x_shape, y_shape))]
 
     def value_infer(self, intensors: []):
         result = numpy.where(intensors[0], intensors[1], intensors[2])
         return [result]
 
 
 @NODE_REGISTRY.register()
@@ -538,15 +617,31 @@
                 yshape = xshape[:-1] + [wshape[-1], ]
         else:
             yshape = xshape[:-1] + [wshape[-1], ]
 
         return [yshape]
 
     def value_infer(self, intensors: []):
-        return [intensors[0] * intensors[1]]
+        if self.__class__ == MatMulNode:
+            ashape = _get_shape(intensors[0])
+            bshape = _get_shape(intensors[1])
+            assert (ashape[-1] == bshape[-2])
+            return [numpy.matmul(intensors[0], intensors[1])]
+        if self.transA is not None and self.transA > 0:
+            A = numpy.transpose(intensors[0])
+        else:
+            A = intensors[0]
+        if self.transB is not None and self.transB > 0:
+            B = numpy.transpose(intensors[1])
+        else:
+            B = intensors[1]
+        C = numpy.matmul(A, B)
+        if len(intensors) > 2:
+            C = numpy.add(C, intensors[2])
+        return [C]
 
     def profile(self, intensors: [numpy.ndarray], outtensors: [numpy.ndarray]):
         xshape = _get_shape(intensors[0])
         if len(intensors) >= 2:
             weight_shape = _get_shape(intensors[1])
             macs = volume(xshape)
             if self.__class__ == GemmNode:
@@ -603,30 +698,45 @@
 @NODE_REGISTRY.register()
 class ClipNode(PWNode):
     def __init__(self, n):
         super().__init__(n)
         self.op_mac = CMP_MACS * 2
         self.ratio = 1
 
+    def value_infer(self, intensors: []):
+        y = numpy.clip(intensors[0], intensors[1], intensors[2])
+        return [y]
+
 
 @NODE_REGISTRY.register()
 class ReciprocalNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = DIV_MACS
 
+    def value_infer(self, intensors: []):
+        return [numpy.reciprocal(intensors[0])]
+
 
 @NODE_REGISTRY.register()
 class Relu6Node(PWNode):
-    pass
+    def value_infer(self, intensors: []):
+        return [numpy.clip(intensors[0],0,6)]
 
 
 @NODE_REGISTRY.register()
 class ConstantNode(Node):
-    pass
+    def __init__(self, n):
+        super().__init__(n)
+
+    def shape_infer(self, intensors: []):
+        return [self.value.shape]
+
+    def value_infer(self, intensors: []):
+        return [self.value]
 
 
 @NODE_REGISTRY.register()
 class ConcatNode(Node):
     def shape_infer(self, intensors: [numpy.ndarray]):
         outshape = _get_shape(intensors[0])
         for i in range(len(intensors) - 1):
@@ -663,22 +773,35 @@
     def value_infer(self, intensors: []):
         indices = intensors[0]
         depth = intensors[1]
         values = intensors[2]
         y = one_hot(indices, depth, self.axis)
         return [y]
 
+
 @NODE_REGISTRY.register()
 class TriluNode(Node):
-    def __init__(self,n):
+    def __init__(self, n):
         super().__init__(n)
+        self.add_default_value('upper',1)
+
 
     def shape_infer(self, intensors: []):
         return [_get_shape(intensors[0])]
 
+    def value_infer(self, intensors: []):
+        if len(intensors)==2:
+            k=intensors[1]
+        else:
+            k=numpy.array(0).astype(numpy.int64)
+        if self.upper==0:
+            return [numpy.tril(intensors[0],k)]
+        else:
+            return [numpy.triu(intensors[0],k)]
+
 @NODE_REGISTRY.register()
 class EinsumNode(Node):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         strs = self.equation.split(b',')
         self.ashape = strs[0].replace(b' ', b'')
         strs = strs[1].split(b'->')
@@ -720,18 +843,19 @@
 
     def shape_infer(self, intensors: []):
         inshape = _get_shape(intensors[0])
         if len(intensors) == 2:
             axes = intensors[1]
         else:
             axes = self.axes
-        axes = _axes_neg2pos(len(inshape), axes)
+        newaxis_len = len(inshape) + len(axes)
+        axes = _axes_neg2pos(newaxis_len, axes)
         newshape = []
         idx = 0
-        for i in range(len(inshape) + len(axes)):
+        for i in range(newaxis_len):
             if i in axes:
                 newshape.append(1)
             else:
                 newshape.append(inshape[idx])
                 idx += 1
         return [newshape]
 
@@ -911,14 +1035,38 @@
 
 @NODE_REGISTRY.register()
 class MaxPoolNode(PoolBase):
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
         self.op_mac = CMP_MACS
 
+    def value_infer(self, intensors: []):
+        xshape=intensors[0].shape
+        oshape=self.shape_infer(intensors)[0]
+        ot=numpy.zeros(oshape)
+        for i in numpy.ndindex(ot.shape):
+            batch = i[0]
+            ocn = i[1]
+            oh = i[2]
+            ow = i[3]
+            t = ot[i]
+            ks=tuple(self.kernel_shape)
+            for j in numpy.ndindex(ks):
+                kh = j[0]
+                kw = j[1]
+                srch = oh * self.strides[0] + kh - self.pads[0]
+                srcw = ow * self.strides[1] + kw - self.pads[1]
+                if srch < 0 or srch >= xshape[2] or srcw < 0 or srcw >= xshape[3]:
+                    continue
+                else:
+                    srcv = intensors[0][batch, ocn, srch, srcw]
+                t = max(srcv,t)
+            ot[i] = t
+        return [ot]
+
 
 @NODE_REGISTRY.register()
 class DropoutNode(FusedBase):
     def shape_infer(self, intensors: []):
         if len(self.input) == 1:
             return [_get_shape(intensors[0])]
         return [_get_shape(intensors[0]), _get_shape(intensors[0])]
@@ -929,14 +1077,28 @@
     def shape_infer(self, intensors: []):
         inshape = _get_shape(intensors[0])
         shape = inshape[0:2]
         for i in range(2, len(inshape)):
             shape += (1,)
         return [shape]
 
+    def value_infer(self, intensors: []):
+        x=intensors[0]
+        h=x.shape[2]
+        w=x.shape[3]
+        y=numpy.zeros(x.shape[:2],dtype=numpy.float32)
+        for i in numpy.ndindex(y.shape):
+            t=0
+            for j in numpy.ndindex((h,w)):
+                xi=i+j
+                t+=x[xi]
+            t/=(h*w)
+            y[i]=t
+        return [y]
+
     def profile(self, intensors: [], outtensors: []):
         inshape = _get_shape(intensors[0])
         outshape = _get_shape(outtensors[0])
         macs = volume(inshape) * ADD_MACS + volume(outshape) * DIV_MACS
         return macs
 
 
@@ -945,14 +1107,17 @@
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
 
     def shape_infer(self, intensors: []):
         xshape = _get_shape(intensors[0])
         expandshape = intensors[1]
         yshape = []
+        if len(xshape) < len(expandshape):
+            for i in range(len(xshape), len(expandshape)):
+                xshape = [1, ] + xshape
         for x, e in zip(xshape, expandshape):
             yshape.append(max(x, e))
         return [yshape]
 
     def value_infer(self, intensors: []):
         output = intensors[0] * numpy.ones(intensors[1].astype(numpy.int64), dtype=numpy.float32)
         return [output]
@@ -988,16 +1153,35 @@
 @NODE_REGISTRY.register()
 class ErfNode(FusedBase):
     pass
 
 
 @NODE_REGISTRY.register()
 class BatchNormalizationNode(FusedBase):
-    pass
-
+    def __init__(self,n):
+        super().__init__(n)
+        self.add_default_value('epsilon',1e-05)
+        self.add_default_value('momentum',0.9)
+        self.add_default_value('training_mode',int(0))
+
+    def value_infer(self, intensors: []):
+        x=intensors[0]
+        scale=intensors[1]
+        b=intensors[2]
+        mean=intensors[3]
+        var=intensors[4]
+        y=numpy.zeros_like(x)
+        for i in numpy.ndindex(y.shape):
+            cn=i[1]
+            sqrt_var=math.sqrt(var[cn]+self.epsilon)
+            sm=scale[cn]/sqrt_var
+            sv=b[cn]
+            m=mean[cn]
+            y[i]=(x[i]-m)*sm+sv
+        return [y]
 
 @NODE_REGISTRY.register()
 class FlattenNode(Node):
     def __init__(self, node):
         super().__init__(node)
         self.add_default_value('axis', None)
 
@@ -1383,14 +1567,49 @@
             elif len(xshape) == 3:
                 oh = _conv_output_shape(xshape[2], self.pads[0] + self.pads[1], wshape[2], self.strides[0],
                                         self.dilations[0])
                 shape = (xshape[0], wshape[0], oh)
         outshapes.append(shape)
         return outshapes
 
+    def value_infer(self, intensors: []):
+        if self.group != 1:
+            raise NotImplementedError()
+        outshape = self.shape_infer(intensors)[0]
+        outtensor = numpy.zeros(outshape, dtype=numpy.float32)
+        has_bias = len(intensors) > 2
+        xshape = _get_shape(intensors[0])
+        wshape = _get_shape(intensors[1])
+        if len(wshape) != 4:
+            raise NotImplementedError()
+
+        reduce_shape = tuple(wshape[1:])
+        for i in numpy.ndindex(outshape):
+            batch = i[0]
+            ocn = i[1]
+            oh = i[2]
+            ow = i[3]
+            t = outtensor[i]
+            if has_bias:
+                t = intensors[2][ocn]
+            for j in numpy.ndindex(reduce_shape):
+                icn = j[0]
+                kh = j[1]
+                kw = j[2]
+                srch = oh * self.strides[0] + kh * self.dilations[0] - self.pads[0]
+                srcw = ow * self.strides[1] + kw * self.dilations[1] - self.pads[1]
+                if srch < 0 or srch >= xshape[2] or srcw < 0 or srcw >= xshape[3]:
+                    srcv = 0
+                else:
+                    srcv = intensors[0][batch, icn, srch, srcw]
+                wv = intensors[1][(ocn,) + j]
+                t += srcv * wv
+            outtensor[i] = t
+        return [outtensor]
+
     def profile(self, intensors: [], outtensors: []):
         macs = 0
         if len(outtensors) == 1:
             if len(intensors) == 3 or len(intensors) == 2:
                 kernel_shape = _get_shape(intensors[1])
                 outvol = volume(_get_shape(outtensors[0]))
                 if len(kernel_shape) > 3:
@@ -1406,28 +1625,35 @@
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
         self.add_default_value('axes', None)
         self.add_default_value('keepdims', 1)
         self.axes = tuple(self.axes) if self.axes is not None else None
 
     def value_infer(self, intensors: []):
-        reduced = numpy.sqrt(numpy.sum(intensors[0], axis=self.axes, keepdims=self.keepdims == 1))
+        reduced = numpy.sqrt(numpy.sum(intensors[0] * intensors[0], axis=self.axes, keepdims=self.keepdims == 1))
         return [reduced]
 
     def profile(self, intensors: [numpy.ndarray], outtensors: [numpy.ndarray]):
         vol = volume(_get_shape(intensors[0]))
         return vol * (ADD_MACS + SQRT_MACS)
 
 
 @NODE_REGISTRY.register()
 class CumSumNode(PWNode):
     def __init__(self, node_proto):
         super().__init__(node_proto)
         self.op_mac = ADD_MACS
         self.ratio = 1
+        self.add_default_value('exclusive', 0)
+        self.add_default_value('reverse', 0)
+
+    def value_infer(self, intensors: []):
+        if self.exclusive == 0 and self.reverse == 0:
+            return [numpy.cumsum(intensors[0], intensors[1])]
+        raise NotImplementedError(f"CumSum doesnt support {self.exclusive} {self.reverse}")
 
 
 @NODE_REGISTRY.register()
 class NonZeroNode(Node):
     def value_infer(self, intensors: []):
         condi = intensors[0]
         result = numpy.array(numpy.nonzero(condi), dtype=numpy.int64)
@@ -1491,35 +1717,141 @@
     # Check tensor shapes
     assert indices.shape[-1] <= len(data.shape)
     assert updates.shape == indices.shape[:-1] + data.shape[indices.shape[-1]:]
 
     # Compute output
     output = numpy.copy(data)
     for i in numpy.ndindex(indices.shape[:-1]):
+        rawoutput = output[tuple(indices[i])]
         # NOTE: The order of iteration in this loop is not specified.
         if reduction == "add":
-            output[indices[i]] += updates[i]
+            rawoutput += updates[i]
         elif reduction == "mul":
-            output[indices[i]] *= updates[i]
+            rawoutput *= updates[i]
         elif reduction == "max":
-            output[indices[i]] = np.maximum(output[indices[i]], updates[i])
+            rawoutput = numpy.maximum(rawoutput, updates[i])
         elif reduction == "min":
-            output[indices[i]] = np.minimum(output[indices[i]], updates[i])
+            rawoutput = numpy.minimum(rawoutput, updates[i])
         else:
-            output[indices[i]] = updates[i]
+            rawoutput = updates[i]
+        output[tuple(indices[i])] = rawoutput
     return output
 
 
+# copy from https://github.com/onnx/onnx/blob/main/onnx/backend/test/case/node/gathernd.py
+def gather_nd_impl(
+        data: numpy.ndarray, indices: numpy.ndarray, batch_dims: int
+) -> numpy.ndarray:
+    # Note the data rank - will be reused multiple times later
+    data_rank = len(data.shape)
+
+    # Check input tensors' shape/rank condition
+    assert indices.shape[-1] <= data_rank
+
+    # The list of data/indice shape of batch_dims
+    batch_dims_shape = []
+
+    # The number of elements in the batch_dims for data/indice array
+    batch_dims_size = 1
+
+    # Check the shape of indice and data are identicial for batch dims.
+    for i in range(batch_dims):
+        batch_dims_shape.append(indices.shape[i])
+        batch_dims_size *= indices.shape[i]
+
+    # Compute output of the op as below
+
+    # Compute shape of output array
+    output_shape = (
+        batch_dims_shape + list(indices.shape)[batch_dims:-1]
+        if (indices.shape[-1] == data_rank - batch_dims)
+        else batch_dims_shape
+             + list(indices.shape)[batch_dims:-1]
+             + list(data.shape)[batch_dims + indices.shape[-1]:]
+    )
+
+    # Placeholder for output data
+    output_data_buffer = []
+
+    # Flatten 'indices' to 2D array
+    reshaped_indices = indices.reshape(batch_dims_size, -1, indices.shape[-1])
+
+    # Flatten 'data' to array of shape (batch_dim_size, data.shape[batch_dimes:])
+    reshaped_data = data.reshape((batch_dims_size,) + data.shape[batch_dims:])
+
+    # gather each scalar value from 'data'
+    for batch_dim in range(reshaped_indices.shape[0]):
+        for outer_dim in range(reshaped_indices.shape[1]):
+            gather_index = tuple(reshaped_indices[batch_dim][outer_dim])
+            output_data_buffer.append(reshaped_data[(batch_dim, *gather_index)])
+    return numpy.asarray(output_data_buffer, dtype=data.dtype).reshape(output_shape)
+
+
 @NODE_REGISTRY.register()
 class ScatterNDNode(Node):
+    def shape_infer(self, intensors: []):
+        return [_get_shape(intensors[0])]  # output=copy(data)
+
     def value_infer(self, intensors: []):
         data = intensors[0]
-        indices = intensors[1]
+        indices = intensors[1].astype(numpy.int64)
         updates = intensors[2]
-        return [scatter_nd_impl(data, indices, updates)]
+        return [scatter_nd_impl(data, indices, updates)]  # TODO this impl may fail some cases
+
+
+@NODE_REGISTRY.register()
+class GatherNDNode(Node):
+    def shape_infer(self, intensors: []):
+        data_shape = _get_shape(intensors[0])
+        indice_shape = _get_shape(intensors[1])
+        batch_dims = 0
+        # Note the data rank - will be reused multiple times later
+        data_rank = len(data_shape)
+
+        # Check input tensors' shape/rank condition
+        assert indice_shape[-1] <= data_rank
+
+        # The list of data/indice shape of batch_dims
+        batch_dims_shape = []
+
+        # The number of elements in the batch_dims for data/indice array
+        batch_dims_size = 1
+
+        # Check the shape of indice and data are identicial for batch dims.
+        for i in range(batch_dims):
+            batch_dims_shape.append(indice_shape[i])
+            batch_dims_size *= indice_shape[i]
+
+        # Compute output of the op as below
+
+        # Compute shape of output array
+        output_shape = (
+            batch_dims_shape + list(indice_shape)[batch_dims:-1]
+            if (indice_shape[-1] == data_rank - batch_dims)
+            else batch_dims_shape
+                 + list(indice_shape)[batch_dims:-1]
+                 + list(data_shape)[batch_dims + indice_shape[-1]:]
+        )
+        return [output_shape]
+
+    def value_infer(self, intensors: []):
+        data = intensors[0]
+        indices = intensors[1].astype(numpy.int64)
+        return [gather_nd_impl(data, indices, 0)]
+
+
+@NODE_REGISTRY.register()
+class RandomUniformLikeNode(Node):
+    def shape_infer(self, intensors: []):
+        return [_get_shape(intensors[0])]
+
+
+@NODE_REGISTRY.register()
+class RandomNormalLikeNode(RandomUniformLikeNode):
+    pass
 
 
 @NODE_REGISTRY.register()
 class GreaterNode(Node):
     def value_infer(self, intensors: []):
         result = numpy.greater(intensors[0], intensors[1])
         return [result]
@@ -1676,15 +2008,15 @@
                 shape[2] = self.output_shape[0]
         return [shape, ]
 
     def profile(self, intensors: [], outtensors: []):
         macs = 0
         if len(outtensors) == 1:
             if len(intensors) == 3 or len(intensors) == 2:
-                kernel_shape = intensors[1].shape
+                kernel_shape = _get_shape(intensors[1])
                 if len(kernel_shape) > 3:
                     outvol = volume(_get_shape(outtensors[0]))
                     macs += outvol * kernel_shape[1] * kernel_shape[2] * kernel_shape[3]
                     macs += outvol * ADD_MACS  # treat bias add as 0.5 MACs
                 elif len(kernel_shape) == 3:
                     outvol = volume(_get_shape(outtensors[0]))
                     macs += outvol * kernel_shape[1] * kernel_shape[2]
@@ -1715,30 +2047,30 @@
                     break
         assert raw == volume(newshape)
         return [newshape]
 
     def value_infer(self, intensors: []):
         return [intensors[0].reshape(intensors[1])]
 
+
 @NODE_REGISTRY.register()
 class GatherElementsNode(Node):
     def shape_infer(self, intensors: []):
         return [_get_shape(intensors[1])]
 
     def value_infer(self, intensors: []):
-        if self.axis==1:
-            if len(intensors[1].shape)==4:
-                outtensor=numpy.zeros_like(intensors[1])
-                for i in range(intensors[1].shape[0]):
-                    for j in range(intensors[1].shape[1]):
-                        for k in range(intensors[1].shape[2]):
-                            for l in range(intensors[1].shape[3]):
-                                outtensor[i,j,k,l]= intensors[0][i,intensors[1][i,j,k,l],k,l]
-                return [outtensor]
-        raise NotImplementedError()
+        x=intensors[0]
+        indice=intensors[1].astype(numpy.int64)
+        outtensor = numpy.zeros_like(indice)
+        for i in numpy.ndindex(outtensor.shape):
+            idx = list(i)
+            idx[self.axis] = indice[i]
+            outtensor[i] = x[tuple(idx)]
+        return [outtensor]
+
 
 @NODE_REGISTRY.register()
 class GRUNode(Node):
     def shape_infer(self, intensors: []):
         xshape = _get_shape(intensors[0])
         wshape = _get_shape(intensors[1])
         seq_len = xshape[0]
```

### Comparing `onnx-tool-0.6.5/onnx_tool/serialization.py` & `onnx-tool-0.7.0/onnx_tool/serialization.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.6.5/onnx_tool/tensor.py` & `onnx-tool-0.7.0/onnx_tool/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,20 +362,14 @@
             self.type = DYNAMIC_TENSOR
         elif isinstance(t, onnx.TensorProto):
             self.name = t.name
             self.proto = t
             self.numpy = tensorproto2ndarray(t)
             self.shape = self.numpy.shape
             self.type = STATIC_TENSOR
-        elif isinstance(t, Node):
-            if t.op_type == 'Constant':
-                self.name = t.output[0]
-                self.update_proto(t.value)
-                self.shape = self.numpy.shape
-                self.type = STATIC_TENSOR
         else:
             assert 0
         self.sparsity_search()
 
     def update_tensor(self, data: numpy.ndarray):
         if not isinstance(data, numpy.ndarray):
             data = numpy.array(data)
@@ -405,16 +399,14 @@
     def get_shape(self):
         shape = []
         for s in self.shape:
             if isinstance(s, str):
                 shape.append(s)
             else:
                 shape.append(int(s))
-        if len(shape) == 0:  # scalar
-            return [1, ]
         return shape
 
     def get_valueorshape(self):
         if self.numpy is not None:
             return self.numpy
         return self.shape
 
@@ -445,15 +437,18 @@
             if self.proto is None and make_dummy:
                 warnings.warn('Creating a dummpy tensor proto:' + self.name)
                 return onnx.helper.make_tensor_value_info(self.name, 1, None)
             return self.proto
         else:
             shape = self.get_shape()
         if self.numpy is None:
-            dtype = onnx.TensorProto.FLOAT
+            if self.proto is not None:
+                dtype = self.proto.type.tensor_type.elem_type
+            else:
+                dtype = onnx.TensorProto.FLOAT
         else:
             dtype = npdtype2onnxdtype(self.numpy.dtype)
         # shape = [int(i) for i in shape]
         vinf = onnx.helper.make_tensor_value_info(self.name, dtype, shape)
         return vinf
 
     def make_tensor_proto(self):
```

### Comparing `onnx-tool-0.6.5/onnx_tool/utils.py` & `onnx-tool-0.7.0/onnx_tool/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import warnings
 
-VERSION = "0.6.5"
+VERSION = "0.7.0"
 
 
 class timer():
     def __init__(self):
         self._startt = time.time()
 
     def start(self):
```

### Comparing `onnx-tool-0.6.5/onnx_tool.egg-info/PKG-INFO` & `onnx-tool-0.7.0/onnx_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-tool
-Version: 0.6.5
+Version: 0.7.0
 Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
 Home-page: https://github.com/ThanatosShinji/onnx-tool
 Author: Luo Yu
 Author-email: luoyu888888@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -13,25 +13,26 @@
 <a href="README_CN.md">简体中文</a>
 # onnx-tool
 
 **A tool for ONNX model:**
 
 * *Rapid shape inference.*
 * *Profile model.*
+* *<a href="data/ConstantFolding.md">Constant Folding.</a>*
 * *Compute Graph and Shape Engine.*
 * *OPs fusion.*
 * *Activation memory compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT, LLaMa, MPT(<a href="benchmark/transfomer_models.py">TransformerModel</a>)
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
-* CV: Resnet, MobileNet, YOLO, ...
-* Audio: LPCNet
+* CV: <a href="benchmark/compression.py">BEVFormer</a>, MobileNet, YOLO, ...
+* Audio: sovits, LPCNet
 
 ---
 
 ## Shape inference
 
 <p align="center">  
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/shape_inference.jpg">
@@ -97,15 +98,15 @@
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
 BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
-
+Help implement model parallelism.
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_subgraph.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
@@ -153,30 +154,31 @@
 Then `pip install onnx-tool` again.
 
 
 ---
 
 ## Known Issues
 * Loop op is not supported
-
+* Activation Compression is not optimum
+  
 ---
 
 ## Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
 Some models have dynamic input shapes. The MACs varies from input shapes. The input shapes used in these results are writen to [data/public/config.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py).
 These onnx models with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ 
 )(code: p91k) [google drive](https://drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 <p id="results" align="center">
 <table>
 <tr>
 <td>
 
 Model | Params(M) | MACs(M)
 ---|---|---
-GPT-J 1 layer | 464 | 173,398  
-MPT 1 layer | 261 | 79,894
+<a href="benchmark/transfomer_models.py">GPT-J 1 layer</a> | 464 | 173,398  
+<a href="benchmark/transfomer_models.py">MPT 1 layer</a> | 261 | 79,894
 [text_encoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main)| 123.13 | 6,782
 [UNet2DCondition](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main)| 859.52 | 888,870
 [VAE_encoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main) | 34.16 | 566,371
 [VAE_decoder](https://huggingface.co/bes-dev/stable-diffusion-v1-4-onnx/tree/main) | 49.49 | 1,271,959
 [SqueezeNet 1.0](https://github.com/onnx/models/tree/main/vision/classification/squeezenet) | 1.23 | 351
 [AlexNet](https://github.com/onnx/models/tree/main/vision/classification/alexnet) | 60.96 | 665
 [GoogleNet](https://github.com/onnx/models/tree/main/vision/classification/inception_and_googlenet/googlenet) | 6.99 | 1,606
@@ -188,29 +190,29 @@
 [Emotion](https://github.com/onnx/models/tree/main/vision/body_analysis/emotion_ferplus) | 12.95 | 877
 [Mask R-CNN](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/mask-rcnn) | 46.77 | 92,077
 </td>
 
 <td>
 
 Model | Params(M) | MACs(M)
----|---|---
-LLaMa 1 layer | 618 | 211,801  
-[rvm_mobilenetv3](https://github.com/PeterL1n/RobustVideoMatting) | 3.73 | 4,289
-[yolov4](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/yolov4) | 64.33 | 3,319
-[ConvNeXt-L](https://github.com/facebookresearch/ConvNeXt) | 229.79 | 34,872
-[edgenext_small](https://github.com/mmaaz60/EdgeNeXt) | 5.58 | 1,357
-[SSD](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/ssd) | 19.98 | 216,598
-[RealESRGAN](https://github.com/xinntao/Real-ESRGAN) | 16.69 | 73,551
-[ShuffleNet](https://github.com/onnx/models/tree/main/vision/classification/shufflenet) | 2.29 | 146
-[GPT-2](https://github.com/onnx/models/tree/main/text/machine_comprehension/gpt-2) | 137.02 | 1,103
-[T5-encoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 109.62 | 686
-[T5-decoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 162.62 | 1,113
-[RoBERTa-BASE](https://github.com/onnx/models/tree/main/text/machine_comprehension/roberta) | 124.64 | 688
-[Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10 | 46,018
-[FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29 | 37,056
-[MobileNet](https://github.com/onnx/models/blob/main/vision/classification/mobilenet) | 3.3 | 300
-[ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25 | 3,868
+---|-----------|---
+<a href="benchmark/transfomer_models.py">LLaMa 1 layer</a> | 618       | 211,801  
+[BEVFormer Tiny](https://github.com/DerryHub/BEVFormer_tensorrt) | 33.7      | 210,838
+[rvm_mobilenetv3](https://github.com/PeterL1n/RobustVideoMatting) | 3.73      | 4,289
+[yolov4](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/yolov4) | 64.33     | 3,319
+[ConvNeXt-L](https://github.com/facebookresearch/ConvNeXt) | 229.79    | 34,872
+[edgenext_small](https://github.com/mmaaz60/EdgeNeXt) | 5.58      | 1,357
+[SSD](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/ssd) | 19.98     | 216,598
+[RealESRGAN](https://github.com/xinntao/Real-ESRGAN) | 16.69     | 73,551
+[ShuffleNet](https://github.com/onnx/models/tree/main/vision/classification/shufflenet) | 2.29      | 146
+[GPT-2](https://github.com/onnx/models/tree/main/text/machine_comprehension/gpt-2) | 137.02    | 1,103
+[T5-encoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 109.62    | 686
+[T5-decoder](https://github.com/onnx/models/tree/main/text/machine_comprehension/t5) | 162.62    | 1,113
+[RoBERTa-BASE](https://github.com/onnx/models/tree/main/text/machine_comprehension/roberta) | 124.64    | 688
+[Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10     | 46,018
+[FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29     | 37,056
+[ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25        | 3,868
 
 </td>
 </tr>
 </table>
 </p>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.6.5 Summary: A tool for ONNX
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.0 Summary: A tool for ONNX
 model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
 fusion;Quantized models and sparse models are supported. Home-page: https://
 github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
 luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
 # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
-model.* * *Compute Graph and Shape Engine.* * *OPs fusion.* * *Activation
-memory compression.* * *Quantized models and sparse models are supported.*
-Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT(TransformerModel) *
-Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV: Resnet, MobileNet,
-YOLO, ... * Audio: LPCNet --- ## Shape inference
+model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
+fusion.* * *Activation memory compression.* * *Quantized models and sparse
+models are supported.* Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT
+(TransformerModel) * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV:
+BEVFormer, MobileNet, YOLO, ... * Audio: sovits, LPCNet --- ## Shape inference
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              shape_inference.jpg]
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/data/Profile.md). pytorch usage: [data/PytorchUsage.md](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md). tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/TensorflowUsage.md). samples: [benchmark/samples.py](https://
@@ -54,15 +54,15 @@
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               resnet18_fused.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). BERT samples: [benchmark/samples.py](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/
 onnx-tool/blob/main/benchmark/do_fusion.py). --- ## Extract subgraph from ONNX
-model
+model Help implement model parallelism.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                             resnet18_subgraph.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). --- ## Memory Compression For large language
 models and high-resolution CV models, the activation memory compression is a
 key to save memory. The compression method achieves 5% memory compression on
 most models. For example: model | Native Memory Size(MB) | Compressed Memory
@@ -78,62 +78,63 @@
 set its static weight tensors as its input tensors* * *Set custom input and
 output tensors' name and dimension, change model from fixed input to dynamic
 input* how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-
 tool/blob/main/data/Tensors.md). --- ## How to install `pip install onnx-tool`
 OR `pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
 python>=3.6 If `pip install onnx-tool` failed by onnx's installation, you may
 try `pip install onnx==1.8.1` (a lower version like this) first. Then `pip
-install onnx-tool` again. --- ## Known Issues * Loop op is not supported --- ##
-Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
-Some models have dynamic input shapes. The MACs varies from input shapes. The
-input shapes used in these results are writen to [data/public/config.py](https:
-//github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These
-onnx models with all tensors' shape can be downloaded: [baidu drive](https://
-pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
+install onnx-tool` again. --- ## Known Issues * Loop op is not supported *
+Activation Compression is not optimum --- ## Results of [ONNX Model Zoo](https:
+//github.com/onnx/models) and SOTA models Some models have dynamic input
+shapes. The MACs varies from input shapes. The input shapes used in these
+results are writen to [data/public/config.py](https://github.com/
+ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These onnx models
+with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/
+s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
 drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 Model | Params(M) | MACs(M) ---|---|--
-- GPT-J 1 layer | 464 | 173,398 MPT 1   Model | Params(M) | MACs(M) ---|---|--
-layer | 261 | 79,894 [text_encoder]     - LLaMa 1 layer | 618 | 211,801
-(https://huggingface.co/bes-dev/stable- [rvm_mobilenetv3](https://github.com/
-diffusion-v1-4-onnx/tree/main)| 123.13  PeterL1n/RobustVideoMatting) | 3.73 |
-| 6,782 [UNet2DCondition](https://      4,289 [yolov4](https://github.com/onnx/
-huggingface.co/bes-dev/stable-          models/tree/main/vision/
-diffusion-v1-4-onnx/tree/main)| 859.52  object_detection_segmentation/yolov4) |
-| 888,870 [VAE_encoder](https://        64.33 | 3,319 [ConvNeXt-L](https://
-huggingface.co/bes-dev/stable-          github.com/facebookresearch/ConvNeXt) |
-diffusion-v1-4-onnx/tree/main) | 34.16  229.79 | 34,872 [edgenext_small](https:
-| 566,371 [VAE_decoder](https://        //github.com/mmaaz60/EdgeNeXt) | 5.58 |
-huggingface.co/bes-dev/stable-          1,357 [SSD](https://github.com/onnx/
-diffusion-v1-4-onnx/tree/main) | 49.49  models/tree/main/vision/
-| 1,271,959 [SqueezeNet 1.0](https://   object_detection_segmentation/ssd) |
+- GPT-J_1_layer | 464 | 173,398 MPT_1   Model | Params(M) | MACs(M) ---|-------
+layer | 261 | 79,894 [text_encoder]     ----|--- LLaMa_1_layer | 618 | 211,801
+(https://huggingface.co/bes-dev/stable- [BEVFormer Tiny](https://github.com/
+diffusion-v1-4-onnx/tree/main)| 123.13  DerryHub/BEVFormer_tensorrt) | 33.7 |
+| 6,782 [UNet2DCondition](https://      210,838 [rvm_mobilenetv3](https://
+huggingface.co/bes-dev/stable-          github.com/PeterL1n/RobustVideoMatting)
+diffusion-v1-4-onnx/tree/main)| 859.52  | 3.73 | 4,289 [yolov4](https://
+| 888,870 [VAE_encoder](https://        github.com/onnx/models/tree/main/
+huggingface.co/bes-dev/stable-          vision/object_detection_segmentation/
+diffusion-v1-4-onnx/tree/main) | 34.16  yolov4) | 64.33 | 3,319 [ConvNeXt-L]
+| 566,371 [VAE_decoder](https://        (https://github.com/facebookresearch/
+huggingface.co/bes-dev/stable-          ConvNeXt) | 229.79 | 34,872
+diffusion-v1-4-onnx/tree/main) | 49.49  [edgenext_small](https://github.com/
+| 1,271,959 [SqueezeNet 1.0](https://   mmaaz60/EdgeNeXt) | 5.58 | 1,357 [SSD]
+github.com/onnx/models/tree/main/       (https://github.com/onnx/models/tree/
+vision/classification/squeezenet) |     main/vision/
+1.23 | 351 [AlexNet](https://           object_detection_segmentation/ssd) |
 github.com/onnx/models/tree/main/       19.98 | 216,598 [RealESRGAN](https://
-vision/classification/squeezenet) |     github.com/xinntao/Real-ESRGAN) | 16.69
-1.23 | 351 [AlexNet](https://           | 73,551 [ShuffleNet](https://
-github.com/onnx/models/tree/main/       github.com/onnx/models/tree/main/
-vision/classification/alexnet) | 60.96  vision/classification/shufflenet) |
-| 665 [GoogleNet](https://github.com/   2.29 | 146 [GPT-2](https://github.com/
-onnx/models/tree/main/vision/           onnx/models/tree/main/text/
-classification/inception_and_googlenet/ machine_comprehension/gpt-2) | 137.02 |
-googlenet) | 6.99 | 1,606               1,103 [T5-encoder](https://github.com/
+vision/classification/alexnet) | 60.96  github.com/xinntao/Real-ESRGAN) | 16.69
+| 665 [GoogleNet](https://github.com/   | 73,551 [ShuffleNet](https://
+onnx/models/tree/main/vision/           github.com/onnx/models/tree/main/
+classification/inception_and_googlenet/ vision/classification/shufflenet) |
+googlenet) | 6.99 | 1,606               2.29 | 146 [GPT-2](https://github.com/
 [googlenet_age](https://github.com/     onnx/models/tree/main/text/
-onnx/models/tree/main/vision/           machine_comprehension/t5) | 109.62 |
-body_analysis/age_gender) | 5.98 |      686 [T5-decoder](https://github.com/
+onnx/models/tree/main/vision/           machine_comprehension/gpt-2) | 137.02 |
+body_analysis/age_gender) | 5.98 |      1,103 [T5-encoder](https://github.com/
 1,605 [LResNet100E-IR](https://         onnx/models/tree/main/text/
-github.com/onnx/models/tree/main/       machine_comprehension/t5) | 162.62 |
-vision/body_analysis/arcface) | 65.22 | 1,113 [RoBERTa-BASE](https://
-12,102 [BERT-Squad](https://github.com/ github.com/onnx/models/tree/main/text/
-onnx/models/tree/main/text/             machine_comprehension/roberta) | 124.64
-machine_comprehension/bert-squad) |     | 688 [Faster R-CNN](https://
-113.61 | 22,767 [BiDAF](https://        github.com/onnx/models/blob/main/
-github.com/onnx/models/tree/main/text/  vision/object_detection_segmentation/
-machine_comprehension/                  faster-rcnn) | 44.10 | 46,018 [FCN
-bidirectional_attention_flow) | 18.08 | ResNet-50](https://github.com/onnx/
-9.87 [EfficientNet-Lite4](https://      models/tree/main/vision/
-github.com/onnx/models/tree/main/       object_detection_segmentation/fcn) |
-vision/classification/efficientnet-     35.29 | 37,056 [MobileNet](https://
-lite4) | 12.96 | 1,361 [Emotion](https: github.com/onnx/models/blob/main/
-//github.com/onnx/models/tree/main/     vision/classification/mobilenet) | 3.3
-vision/body_analysis/emotion_ferplus) | | 300 [ResNet50](https://github.com/
-12.95 | 877 [Mask R-CNN](https://       onnx/models/tree/main/vision/
-github.com/onnx/models/tree/main/       classification/resnet) | 25 | 3,868
-vision/object_detection_segmentation/
+github.com/onnx/models/tree/main/       machine_comprehension/t5) | 109.62 |
+vision/body_analysis/arcface) | 65.22 | 686 [T5-decoder](https://github.com/
+12,102 [BERT-Squad](https://github.com/ onnx/models/tree/main/text/
+onnx/models/tree/main/text/             machine_comprehension/t5) | 162.62 |
+machine_comprehension/bert-squad) |     1,113 [RoBERTa-BASE](https://
+113.61 | 22,767 [BiDAF](https://        github.com/onnx/models/tree/main/text/
+github.com/onnx/models/tree/main/text/  machine_comprehension/roberta) | 124.64
+machine_comprehension/                  | 688 [Faster R-CNN](https://
+bidirectional_attention_flow) | 18.08 | github.com/onnx/models/blob/main/
+9.87 [EfficientNet-Lite4](https://      vision/object_detection_segmentation/
+github.com/onnx/models/tree/main/       faster-rcnn) | 44.10 | 46,018 [FCN
+vision/classification/efficientnet-     ResNet-50](https://github.com/onnx/
+lite4) | 12.96 | 1,361 [Emotion](https: models/tree/main/vision/
+//github.com/onnx/models/tree/main/     object_detection_segmentation/fcn) |
+vision/body_analysis/emotion_ferplus) | 35.29 | 37,056 [ResNet50](https://
+12.95 | 877 [Mask R-CNN](https://       github.com/onnx/models/tree/main/
+github.com/onnx/models/tree/main/       vision/classification/resnet) | 25 |
+vision/object_detection_segmentation/   3,868
 mask-rcnn) | 46.77 | 92,077
```

### Comparing `onnx-tool-0.6.5/setup.py` & `onnx-tool-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
-readme = open("README.md",encoding="utf-8").read()
-VERSION = "0.6.5"
-
+readme = open("README.md", encoding="utf-8").read()
+VERSION = "0.7.0"
 
 requirements = [
     "onnx",
     "numpy",
     'tabulate'
 ]
```

